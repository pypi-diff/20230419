# Comparing `tmp/emmet-api-0.51.9.tar.gz` & `tmp/emmet-api-0.52.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emmet-api-0.51.9.tar", last modified: Fri Apr  7 23:09:39 2023, max compression
+gzip compressed data, was "emmet-api-0.52.0.tar", last modified: Tue Apr 18 23:20:33 2023, max compression
```

## Comparing `emmet-api-0.51.9.tar` & `emmet-api-0.52.0.tar`

### file list

```diff
@@ -1,339 +1,346 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.466811 emmet-api-0.51.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-04-07 23:09:30.000000 emmet-api-0.51.9/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-07 23:09:39.466811 emmet-api-0.51.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-07 23:09:30.000000 emmet-api-0.51.9/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.438810 emmet-api-0.51.9/emmet/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.446810 emmet-api-0.51.9/emmet/api/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.446810 emmet-api-0.51.9/emmet/api/core/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/core/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.446810 emmet-api-0.51.9/emmet/api/core/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/core/assets/mp_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11087 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/core/assets/mp_logo_small.png
--rw-r--r--   0 runner    (1001) docker     (123)    16534 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/core/documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/core/global_header.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/core/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.446810 emmet-api-0.51.9/emmet/api/routes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.446810 emmet-api-0.51.9/emmet/api/routes/_consumer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/_consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/_consumer/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/_consumer/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.446810 emmet-api-0.51.9/emmet/api/routes/_general_store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/_general_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/_general_store/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/_general_store/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.446810 emmet-api-0.51.9/emmet/api/routes/absorption/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/absorption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/absorption/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.446810 emmet-api-0.51.9/emmet/api/routes/alloys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/alloys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/alloys/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/alloys/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.446810 emmet-api-0.51.9/emmet/api/routes/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/bonds/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/bonds/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.446810 emmet-api-0.51.9/emmet/api/routes/charge_density/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/charge_density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/charge_density/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/charge_density/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.446810 emmet-api-0.51.9/emmet/api/routes/chemenv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/chemenv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/chemenv/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/chemenv/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.446810 emmet-api-0.51.9/emmet/api/routes/dielectric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/dielectric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/dielectric/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/dielectric/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.446810 emmet-api-0.51.9/emmet/api/routes/dois/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/dois/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/dois/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.446810 emmet-api-0.51.9/emmet/api/routes/elasticity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/elasticity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/elasticity/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/elasticity/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.446810 emmet-api-0.51.9/emmet/api/routes/electrodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/electrodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12085 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/electrodes/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/electrodes/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/electrodes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.450810 emmet-api-0.51.9/emmet/api/routes/electronic_structure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/electronic_structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/electronic_structure/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/electronic_structure/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.450810 emmet-api-0.51.9/emmet/api/routes/eos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/eos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/eos/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.450810 emmet-api-0.51.9/emmet/api/routes/fermi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/fermi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/fermi/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.450810 emmet-api-0.51.9/emmet/api/routes/grain_boundary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/grain_boundary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/grain_boundary/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/grain_boundary/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.450810 emmet-api-0.51.9/emmet/api/routes/magnetism/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/magnetism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/magnetism/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/magnetism/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.450810 emmet-api-0.51.9/emmet/api/routes/materials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/materials/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/materials/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/materials/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/materials/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.450810 emmet-api-0.51.9/emmet/api/routes/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/molecules/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/molecules/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.450810 emmet-api-0.51.9/emmet/api/routes/mpcomplete/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcomplete/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcomplete/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.450810 emmet-api-0.51.9/emmet/api/routes/mpcules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.450810 emmet-api-0.51.9/emmet/api/routes/mpcules/association/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/association/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/association/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.450810 emmet-api-0.51.9/emmet/api/routes/mpcules/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/bonds/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/bonds/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.450810 emmet-api-0.51.9/emmet/api/routes/mpcules/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/molecules/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)    17188 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/molecules/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/molecules/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.450810 emmet-api-0.51.9/emmet/api/routes/mpcules/orbitals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/orbitals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19772 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/orbitals/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/orbitals/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.450810 emmet-api-0.51.9/emmet/api/routes/mpcules/partial_charges/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/partial_charges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/partial_charges/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.450810 emmet-api-0.51.9/emmet/api/routes/mpcules/partial_spins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/partial_spins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/partial_spins/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.454810 emmet-api-0.51.9/emmet/api/routes/mpcules/redox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/redox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/redox/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/redox/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.454810 emmet-api-0.51.9/emmet/api/routes/mpcules/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/summary/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/summary/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/summary/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.454810 emmet-api-0.51.9/emmet/api/routes/mpcules/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/tasks/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/tasks/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/tasks/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.454810 emmet-api-0.51.9/emmet/api/routes/mpcules/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/thermo/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/thermo/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.454810 emmet-api-0.51.9/emmet/api/routes/mpcules/vibrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/vibrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/vibrations/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.454810 emmet-api-0.51.9/emmet/api/routes/oxidation_states/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/oxidation_states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/oxidation_states/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/oxidation_states/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.454810 emmet-api-0.51.9/emmet/api/routes/phonon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/phonon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/phonon/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/phonon/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.454810 emmet-api-0.51.9/emmet/api/routes/piezo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/piezo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/piezo/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/piezo/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.454810 emmet-api-0.51.9/emmet/api/routes/provenance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/provenance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/provenance/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.454810 emmet-api-0.51.9/emmet/api/routes/robocrys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/robocrys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/robocrys/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/robocrys/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.454810 emmet-api-0.51.9/emmet/api/routes/similarity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/similarity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/similarity/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.454810 emmet-api-0.51.9/emmet/api/routes/substrates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/substrates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/substrates/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/substrates/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.454810 emmet-api-0.51.9/emmet/api/routes/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/summary/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/summary/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/summary/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.454810 emmet-api-0.51.9/emmet/api/routes/surface_properties/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/surface_properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/surface_properties/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/surface_properties/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.458810 emmet-api-0.51.9/emmet/api/routes/synthesis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/synthesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/synthesis/data_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/synthesis/data_adaptor_synpro.py
--rw-r--r--   0 runner    (1001) docker     (123)     7556 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/synthesis/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/synthesis/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/synthesis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.458810 emmet-api-0.51.9/emmet/api/routes/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/tasks/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/tasks/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/tasks/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/tasks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.458810 emmet-api-0.51.9/emmet/api/routes/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/thermo/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/thermo/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.458810 emmet-api-0.51.9/emmet/api/routes/xas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/xas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/xas/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/xas/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.458810 emmet-api-0.51.9/emmet_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-07 23:09:38.000000 emmet-api-0.51.9/emmet_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9661 2023-04-07 23:09:39.000000 emmet-api-0.51.9/emmet_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 23:09:38.000000 emmet-api-0.51.9/emmet_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 23:09:38.000000 emmet-api-0.51.9/emmet_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-07 23:09:38.000000 emmet-api-0.51.9/emmet_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-07 23:09:38.000000 emmet-api-0.51.9/emmet_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-04-07 23:09:30.000000 emmet-api-0.51.9/material_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-04-07 23:09:30.000000 emmet-api-0.51.9/mpcule_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.458810 emmet-api-0.51.9/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-04-07 23:09:30.000000 emmet-api-0.51.9/requirements/deployment.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-04-07 23:09:30.000000 emmet-api-0.51.9/requirements/macos-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9081 2023-04-07 23:09:30.000000 emmet-api-0.51.9/requirements/macos-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-04-07 23:09:30.000000 emmet-api-0.51.9/requirements/macos-latest_py3.11.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8905 2023-04-07 23:09:30.000000 emmet-api-0.51.9/requirements/macos-latest_py3.11_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-04-07 23:09:30.000000 emmet-api-0.51.9/requirements/macos-latest_py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9351 2023-04-07 23:09:30.000000 emmet-api-0.51.9/requirements/macos-latest_py3.8_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-04-07 23:09:30.000000 emmet-api-0.51.9/requirements/macos-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9274 2023-04-07 23:09:30.000000 emmet-api-0.51.9/requirements/macos-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-04-07 23:09:30.000000 emmet-api-0.51.9/requirements/ubuntu-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9082 2023-04-07 23:09:30.000000 emmet-api-0.51.9/requirements/ubuntu-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-04-07 23:09:30.000000 emmet-api-0.51.9/requirements/ubuntu-latest_py3.11.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-04-07 23:09:30.000000 emmet-api-0.51.9/requirements/ubuntu-latest_py3.11_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-04-07 23:09:30.000000 emmet-api-0.51.9/requirements/ubuntu-latest_py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9352 2023-04-07 23:09:30.000000 emmet-api-0.51.9/requirements/ubuntu-latest_py3.8_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-04-07 23:09:30.000000 emmet-api-0.51.9/requirements/ubuntu-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9275 2023-04-07 23:09:30.000000 emmet-api-0.51.9/requirements/ubuntu-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 23:09:39.466811 emmet-api-0.51.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-07 23:09:30.000000 emmet-api-0.51.9/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-07 23:09:30.000000 emmet-api-0.51.9/start.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.458810 emmet-api-0.51.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.462811 emmet-api-0.51.9/tests/_consumer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/_consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/_consumer/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.462811 emmet-api-0.51.9/tests/_general_store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/_general_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/_general_store/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.462811 emmet-api-0.51.9/tests/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/bonds/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.462811 emmet-api-0.51.9/tests/charge_density/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/charge_density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/charge_density/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.462811 emmet-api-0.51.9/tests/chemenv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/chemenv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/chemenv/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.462811 emmet-api-0.51.9/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/core/test_mapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.462811 emmet-api-0.51.9/tests/dielectric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/dielectric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/dielectric/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.462811 emmet-api-0.51.9/tests/elasticity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/elasticity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/elasticity/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.462811 emmet-api-0.51.9/tests/electrodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/electrodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/electrodes/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/electrodes/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.462811 emmet-api-0.51.9/tests/electronic_structure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/electronic_structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/electronic_structure/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.462811 emmet-api-0.51.9/tests/eos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/eos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.462811 emmet-api-0.51.9/tests/grain_boundary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/grain_boundary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/grain_boundary/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.462811 emmet-api-0.51.9/tests/magnetism/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/magnetism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/magnetism/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.462811 emmet-api-0.51.9/tests/materials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/materials/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/materials/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/materials/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.462811 emmet-api-0.51.9/tests/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/molecules/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.462811 emmet-api-0.51.9/tests/mpcomplete/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/mpcomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/mpcomplete/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.462811 emmet-api-0.51.9/tests/mpcules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/mpcules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.462811 emmet-api-0.51.9/tests/mpcules/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/mpcules/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/mpcules/bonds/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.462811 emmet-api-0.51.9/tests/mpcules/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/mpcules/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/mpcules/molecules/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/mpcules/molecules/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.462811 emmet-api-0.51.9/tests/mpcules/orbitals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/mpcules/orbitals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9551 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/mpcules/orbitals/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.462811 emmet-api-0.51.9/tests/mpcules/redox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/mpcules/redox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/mpcules/redox/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.466811 emmet-api-0.51.9/tests/mpcules/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/mpcules/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/mpcules/summary/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/mpcules/summary/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.466811 emmet-api-0.51.9/tests/mpcules/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/mpcules/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/mpcules/tasks/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/mpcules/tasks/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.466811 emmet-api-0.51.9/tests/mpcules/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/mpcules/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/mpcules/thermo/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.466811 emmet-api-0.51.9/tests/oxidation_states/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/oxidation_states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/oxidation_states/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.466811 emmet-api-0.51.9/tests/piezo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/piezo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/piezo/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.466811 emmet-api-0.51.9/tests/robocrys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/robocrys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/robocrys/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.466811 emmet-api-0.51.9/tests/substrates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/substrates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/substrates/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.466811 emmet-api-0.51.9/tests/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/summary/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/summary/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.466811 emmet-api-0.51.9/tests/surface_properties/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/surface_properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/surface_properties/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.466811 emmet-api-0.51.9/tests/synthesis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/synthesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/synthesis/test_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/synthesis/test_adaptor_synpro.py
--rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/synthesis/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/synthesis/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.466811 emmet-api-0.51.9/tests/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/tasks/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/tasks/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.466811 emmet-api-0.51.9/tests/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/thermo/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.466811 emmet-api-0.51.9/tests/xas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/xas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/xas/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.242616 emmet-api-0.52.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-18 23:20:27.000000 emmet-api-0.52.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-18 23:20:33.242616 emmet-api-0.52.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-18 23:20:27.000000 emmet-api-0.52.0/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.210616 emmet-api-0.52.0/emmet/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.222616 emmet-api-0.52.0/emmet/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.222616 emmet-api-0.52.0/emmet/api/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/core/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.222616 emmet-api-0.52.0/emmet/api/core/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/core/assets/mp_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11087 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/core/assets/mp_logo_small.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20974 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/core/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/core/global_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/core/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.222616 emmet-api-0.52.0/emmet/api/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.222616 emmet-api-0.52.0/emmet/api/routes/_consumer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/_consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/_consumer/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/_consumer/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.222616 emmet-api-0.52.0/emmet/api/routes/_general_store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/_general_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/_general_store/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/_general_store/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.222616 emmet-api-0.52.0/emmet/api/routes/dois/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/dois/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/dois/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.222616 emmet-api-0.52.0/emmet/api/routes/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.222616 emmet-api-0.52.0/emmet/api/routes/legacy/jcesr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/legacy/jcesr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/legacy/jcesr/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/legacy/jcesr/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.222616 emmet-api-0.52.0/emmet/api/routes/materials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.222616 emmet-api-0.52.0/emmet/api/routes/materials/absorption/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/absorption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/absorption/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.222616 emmet-api-0.52.0/emmet/api/routes/materials/alloys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/alloys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/alloys/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/alloys/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.226616 emmet-api-0.52.0/emmet/api/routes/materials/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/bonds/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/bonds/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.226616 emmet-api-0.52.0/emmet/api/routes/materials/charge_density/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/charge_density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/charge_density/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/charge_density/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.226616 emmet-api-0.52.0/emmet/api/routes/materials/chemenv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/chemenv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/chemenv/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/chemenv/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.226616 emmet-api-0.52.0/emmet/api/routes/materials/dielectric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/dielectric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/dielectric/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/dielectric/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.226616 emmet-api-0.52.0/emmet/api/routes/materials/elasticity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/elasticity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/elasticity/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/elasticity/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.226616 emmet-api-0.52.0/emmet/api/routes/materials/electrodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/electrodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/electrodes/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/electrodes/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/electrodes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.226616 emmet-api-0.52.0/emmet/api/routes/materials/electronic_structure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/electronic_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/electronic_structure/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/electronic_structure/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.226616 emmet-api-0.52.0/emmet/api/routes/materials/eos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/eos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/eos/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.226616 emmet-api-0.52.0/emmet/api/routes/materials/fermi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/fermi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/fermi/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.226616 emmet-api-0.52.0/emmet/api/routes/materials/grain_boundary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/grain_boundary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/grain_boundary/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/grain_boundary/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.226616 emmet-api-0.52.0/emmet/api/routes/materials/magnetism/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/magnetism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/magnetism/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/magnetism/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.226616 emmet-api-0.52.0/emmet/api/routes/materials/materials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/materials/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/materials/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/materials/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/materials/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.226616 emmet-api-0.52.0/emmet/api/routes/materials/mpcomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/mpcomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/mpcomplete/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/mpcomplete/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.226616 emmet-api-0.52.0/emmet/api/routes/materials/oxidation_states/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/oxidation_states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/oxidation_states/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/oxidation_states/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.226616 emmet-api-0.52.0/emmet/api/routes/materials/phonon/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/phonon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/phonon/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/phonon/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.230616 emmet-api-0.52.0/emmet/api/routes/materials/piezo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/piezo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/piezo/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/piezo/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.230616 emmet-api-0.52.0/emmet/api/routes/materials/provenance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/provenance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/provenance/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.230616 emmet-api-0.52.0/emmet/api/routes/materials/robocrys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/robocrys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/robocrys/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/robocrys/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.230616 emmet-api-0.52.0/emmet/api/routes/materials/similarity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/similarity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/similarity/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.230616 emmet-api-0.52.0/emmet/api/routes/materials/substrates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/substrates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/substrates/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/substrates/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.230616 emmet-api-0.52.0/emmet/api/routes/materials/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/summary/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/summary/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/summary/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.230616 emmet-api-0.52.0/emmet/api/routes/materials/surface_properties/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/surface_properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/surface_properties/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/surface_properties/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.230616 emmet-api-0.52.0/emmet/api/routes/materials/synthesis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/synthesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/synthesis/data_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/synthesis/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/synthesis/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/synthesis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.230616 emmet-api-0.52.0/emmet/api/routes/materials/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/tasks/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/tasks/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/tasks/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/tasks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.230616 emmet-api-0.52.0/emmet/api/routes/materials/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/thermo/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/thermo/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.230616 emmet-api-0.52.0/emmet/api/routes/materials/xas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/xas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/xas/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/materials/xas/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.230616 emmet-api-0.52.0/emmet/api/routes/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/molecules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.230616 emmet-api-0.52.0/emmet/api/routes/molecules/association/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/molecules/association/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/molecules/association/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.230616 emmet-api-0.52.0/emmet/api/routes/molecules/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/molecules/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/molecules/bonds/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/molecules/bonds/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.234616 emmet-api-0.52.0/emmet/api/routes/molecules/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/molecules/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/molecules/molecules/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14504 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/molecules/molecules/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/molecules/molecules/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.234616 emmet-api-0.52.0/emmet/api/routes/molecules/orbitals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/molecules/orbitals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19168 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/molecules/orbitals/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/molecules/orbitals/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.234616 emmet-api-0.52.0/emmet/api/routes/molecules/partial_charges/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/molecules/partial_charges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/molecules/partial_charges/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.234616 emmet-api-0.52.0/emmet/api/routes/molecules/partial_spins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/molecules/partial_spins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/molecules/partial_spins/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.234616 emmet-api-0.52.0/emmet/api/routes/molecules/redox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/molecules/redox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/molecules/redox/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/molecules/redox/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.234616 emmet-api-0.52.0/emmet/api/routes/molecules/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/molecules/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/molecules/summary/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/molecules/summary/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/molecules/summary/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.234616 emmet-api-0.52.0/emmet/api/routes/molecules/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/molecules/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/molecules/tasks/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/molecules/tasks/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/molecules/tasks/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.234616 emmet-api-0.52.0/emmet/api/routes/molecules/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/molecules/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/molecules/thermo/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/molecules/thermo/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/molecules/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.234616 emmet-api-0.52.0/emmet/api/routes/molecules/vibrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/molecules/vibrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-18 23:20:27.000000 emmet-api-0.52.0/emmet/api/routes/molecules/vibrations/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.234616 emmet-api-0.52.0/emmet_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-18 23:20:32.000000 emmet-api-0.52.0/emmet_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11275 2023-04-18 23:20:33.000000 emmet-api-0.52.0/emmet_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 23:20:32.000000 emmet-api-0.52.0/emmet_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 23:20:32.000000 emmet-api-0.52.0/emmet_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-18 23:20:32.000000 emmet-api-0.52.0/emmet_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-18 23:20:32.000000 emmet-api-0.52.0/emmet_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-18 23:20:27.000000 emmet-api-0.52.0/legacy_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12110 2023-04-18 23:20:27.000000 emmet-api-0.52.0/material_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-04-18 23:20:27.000000 emmet-api-0.52.0/molecule_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.238616 emmet-api-0.52.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-04-18 23:20:27.000000 emmet-api-0.52.0/requirements/deployment.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5864 2023-04-18 23:20:27.000000 emmet-api-0.52.0/requirements/macos-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9084 2023-04-18 23:20:27.000000 emmet-api-0.52.0/requirements/macos-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-04-18 23:20:27.000000 emmet-api-0.52.0/requirements/macos-latest_py3.11.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-04-18 23:20:27.000000 emmet-api-0.52.0/requirements/macos-latest_py3.11_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-04-18 23:20:27.000000 emmet-api-0.52.0/requirements/macos-latest_py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-04-18 23:20:27.000000 emmet-api-0.52.0/requirements/macos-latest_py3.8_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-04-18 23:20:27.000000 emmet-api-0.52.0/requirements/macos-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-04-18 23:20:27.000000 emmet-api-0.52.0/requirements/macos-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-04-18 23:20:27.000000 emmet-api-0.52.0/requirements/ubuntu-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-04-18 23:20:27.000000 emmet-api-0.52.0/requirements/ubuntu-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-04-18 23:20:27.000000 emmet-api-0.52.0/requirements/ubuntu-latest_py3.11.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8909 2023-04-18 23:20:27.000000 emmet-api-0.52.0/requirements/ubuntu-latest_py3.11_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-04-18 23:20:27.000000 emmet-api-0.52.0/requirements/ubuntu-latest_py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-04-18 23:20:27.000000 emmet-api-0.52.0/requirements/ubuntu-latest_py3.8_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-04-18 23:20:27.000000 emmet-api-0.52.0/requirements/ubuntu-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9299 2023-04-18 23:20:27.000000 emmet-api-0.52.0/requirements/ubuntu-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 23:20:33.242616 emmet-api-0.52.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-18 23:20:27.000000 emmet-api-0.52.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-18 23:20:27.000000 emmet-api-0.52.0/start.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.238616 emmet-api-0.52.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.238616 emmet-api-0.52.0/tests/_consumer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/_consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/_consumer/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.238616 emmet-api-0.52.0/tests/_general_store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/_general_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/_general_store/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.238616 emmet-api-0.52.0/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/core/test_mapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.218616 emmet-api-0.52.0/tests/legacy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.238616 emmet-api-0.52.0/tests/legacy/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/legacy/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/legacy/molecules/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.222616 emmet-api-0.52.0/tests/materials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.238616 emmet-api-0.52.0/tests/materials/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/bonds/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.238616 emmet-api-0.52.0/tests/materials/charge_density/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/charge_density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/charge_density/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.238616 emmet-api-0.52.0/tests/materials/chemenv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/chemenv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/chemenv/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.238616 emmet-api-0.52.0/tests/materials/dielectric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/dielectric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/dielectric/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.238616 emmet-api-0.52.0/tests/materials/elasticity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/elasticity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/elasticity/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.238616 emmet-api-0.52.0/tests/materials/electrodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/electrodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/electrodes/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/electrodes/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.238616 emmet-api-0.52.0/tests/materials/electronic_structure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/electronic_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/electronic_structure/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.238616 emmet-api-0.52.0/tests/materials/eos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/eos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.238616 emmet-api-0.52.0/tests/materials/grain_boundary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/grain_boundary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/grain_boundary/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.238616 emmet-api-0.52.0/tests/materials/magnetism/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/magnetism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/magnetism/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.238616 emmet-api-0.52.0/tests/materials/materials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/materials/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6528 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/materials/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/materials/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.238616 emmet-api-0.52.0/tests/materials/mpcomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/mpcomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/mpcomplete/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.238616 emmet-api-0.52.0/tests/materials/oxidation_states/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/oxidation_states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/oxidation_states/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.238616 emmet-api-0.52.0/tests/materials/piezo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/piezo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/piezo/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.238616 emmet-api-0.52.0/tests/materials/robocrys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/robocrys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/robocrys/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.238616 emmet-api-0.52.0/tests/materials/substrates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/substrates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/substrates/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.242616 emmet-api-0.52.0/tests/materials/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/summary/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/summary/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.242616 emmet-api-0.52.0/tests/materials/surface_properties/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/surface_properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/surface_properties/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.242616 emmet-api-0.52.0/tests/materials/synthesis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/synthesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/synthesis/test_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/synthesis/test_adaptor_synpro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/synthesis/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/synthesis/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.242616 emmet-api-0.52.0/tests/materials/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/tasks/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/tasks/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.242616 emmet-api-0.52.0/tests/materials/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/thermo/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.242616 emmet-api-0.52.0/tests/materials/xas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/xas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/materials/xas/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.242616 emmet-api-0.52.0/tests/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/molecules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.242616 emmet-api-0.52.0/tests/molecules/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/molecules/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/molecules/bonds/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.242616 emmet-api-0.52.0/tests/molecules/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/molecules/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/molecules/molecules/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/molecules/molecules/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.242616 emmet-api-0.52.0/tests/molecules/orbitals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/molecules/orbitals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9230 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/molecules/orbitals/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.242616 emmet-api-0.52.0/tests/molecules/redox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/molecules/redox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/molecules/redox/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.242616 emmet-api-0.52.0/tests/molecules/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/molecules/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/molecules/summary/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/molecules/summary/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.242616 emmet-api-0.52.0/tests/molecules/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/molecules/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/molecules/tasks/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/molecules/tasks/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:33.242616 emmet-api-0.52.0/tests/molecules/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/molecules/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-18 23:20:27.000000 emmet-api-0.52.0/tests/molecules/thermo/test_query_operators.py
```

### Comparing `emmet-api-0.51.9/Dockerfile` & `emmet-api-0.52.0/Dockerfile`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,16 @@
     DD_TRACE_HOST=localhost:8126 \
     DD_SERVICE=next-gen-api \
     DD_ENV=prod \
     DD_VERSION=$VERSION
 
 COPY app.py .
 COPY material_resources.py .
-COPY mpcule_resources.py .
+COPY molecule_resources.py .
+COPY legacy_resources.py .
 COPY start.sh .
 RUN chmod +x start.sh
 
 LABEL com.datadoghq.ad.logs='[{"source": "gunicorn", "service": "next-gen-api"}]'
 
 EXPOSE 10001 20001
 CMD wait-for-it.sh $DD_TRACE_HOST -q -s -t 60 -- ./start.sh
```

### Comparing `emmet-api-0.51.9/emmet/api/core/api.py` & `emmet-api-0.52.0/emmet/api/core/api.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/emmet/api/core/assets/mp_logo.svg` & `emmet-api-0.52.0/emmet/api/core/assets/mp_logo.svg`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/emmet/api/core/assets/mp_logo_small.png` & `emmet-api-0.52.0/emmet/api/core/assets/mp_logo_small.png`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/emmet/api/core/documentation.py` & `emmet-api-0.52.0/emmet/api/core/documentation.py`

 * *Files 25% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 3. Since this is a REST API, and offers a fully-compliant OpenAPI specification, it's possible to use the API with many libraries in many languages and environments, including JavaScript, MATLAB, Mathematica, etc. However, we do not offer first-party support for explaining how to do this, and you will have to follow the specification yourself.
 
 """
 
 tags_meta = [
     {
-        "name": "Summary",
+        "name": "Materials Summary",
         "description": "Route providing a large amount of amalgamated data for a material. This is constructed by \
             combining subsets of data from many of the other API endpoints. The summary endpoint is very useful for \
             performing queries for materials over a large property space. Note that every unique material within \
             the Materials Project should have a set of summary data. See the `SummaryDoc` schema for a full list of \
             fields returned by this route.",
     },
     {
@@ -50,210 +50,279 @@
             this context refers to the crystal structure, information associated with it such as the density \
             and chemical formula, and the associated calculations which are identified with unique `task_id` \
             values. It does not contain any materials properties such as the formation energy or band gap, please \
             consult other property-specific endpoints for this information. See the `MaterialsDoc` schema for \
             a full list of fields returned by this route.',
     },
     {
-        "name": "Tasks",
+        "name": "Materials Tasks",
         "description": 'Route for "core" information associated with a given calculation in the Materials Project \
             database. Multiple calculations can ultimately be associated with a unique material, and are the source \
             of its reported properties. The unique identifier for a calculation is its `task_id`. Note \
             that the `material_id` chosen for a given material is sourced from one of the `task_id` values \
             associated with it. Core data in this context refers to calculation quantities such as parsed input \
             and output data (e.g. VASP input flags, atomic forces, structures) and runtime statistics. See the \
             `TaskDoc` schema for a full list of fields returned by this route.',
     },
     {
-        "name": "Thermo",
+        "name": "Materials Thermo",
         "description": "Route providing computed thermodynamic data for a material such as \
             formation energy and energy above hull. Corrected energy values are also available that employ \
             the schemes discussed by \
             [Jain *et al.*](https://journals.aps.org/prb/abstract/10.1103/PhysRevB.84.045115) \
             and [Wang *et al.*](https://chemrxiv.org/engage/chemrxiv/article-details/60c758d9469df42a4ef45757)\
             See the `ThermoDoc` schema for a full list of fields returned by this route.",
         "externalDocs": {
             "description": "For a more detailed description",
             "url": "https://docs.materialsproject.org/methodology/total-energies",
         },
     },
     {
-        "name": "Dielectric",
+        "name": "Materials Dielectric",
         "description": "Route providing computed dielectric data for a material following the \
             methodology discussed by [Petousis *et al.*](https://doi.org/10.1038/sdata.2016.134) \
             Note that dielectric data has not been calculated for all materials in the Materials \
             Project database. See the `DielectricDoc` schema for a full list of fields returned by this route.",
         "externalDocs": {
             "description": "For a more detailed description",
             "url": "https://docs.materialsproject.org/methodology/dielectricity",
         },
     },
     {
-        "name": "Magnetism",
+        "name": "Materials Magnetism",
         "description": "Route providing computed magnetic ordering related data for a material following the \
             methodology discussed by [Horton *et al.*](https://doi.org/10.1038/s41524-019-0199-7) \
             Note that magnetic data has not been calculated for all materials in the Materials \
             Project database. See the `MagnetismDoc` schema for a full list of fields returned by this route.",
     },
     {
-        "name": "Piezoelectric",
+        "name": "Materials Piezoelectric",
         "description": "Route providing computed piezoelectric data for a material following the \
             methodology discussed by [de Jong *et al.*](https://doi.org/10.1038/sdata.2015.53) \
             Note that piezoelectric data has not been calculated for all materials in the Materials \
             Project database. See the `PiezoDoc` schema for a full list of fields returned by this route.",
         "externalDocs": {
             "description": "For a more detailed description",
             "url": "https://docs.materialsproject.org/methodology/piezoelectricity",
         },
     },
     {
-        "name": "Phonon",
+        "name": "Materials Phonon",
         "description": "Route providing computed phonon data for a material following the \
             methodology discussed by [Petretto *et al.*](https://doi.org/10.1038/sdata.2018.65) \
             Note that phonon data has not been calculated for all materials in the Materials \
             Project database. See the `PhononBSDOSDoc` schema for a full list of fields returned by this route.",
         "externalDocs": {
             "description": "For a more detailed description",
             "url": "https://docs.materialsproject.org/methodology/phonons",
         },
     },
     {
-        "name": "EOS",
+        "name": "Materials EOS",
         "description": "Route providing computed equations of state data for a material following the \
             methodology discussed by [Latimer *et al.*](https://doi.org/10.1038/s41524-018-0091-x) \
             Note that equations of state data has not been calculated for all materials in the Materials \
             Project database. See the `EOSDoc` schema for a full list of fields returned by this route.",
         "externalDocs": {
             "description": "For a more detailed description",
             "url": "https://docs.materialsproject.org/methodology/equations-of-state",
         },
     },
     {
-        "name": "Similarity",
+        "name": "Materials Similarity",
         "description": "Route providing a computed similarity metric between materials following the \
             methodology discussed by Zimmerman *et al.* in [10.3389/fmats.2017.00034](https://doi.org/10.3389/fmats.2017.00034) \
             and [10.1039/C9RA07755C](https://doi.org/10.1039/C9RA07755C). \
             Note that similarity data has not been calculated for all materials in the Materials \
             Project database. See the `imilarityDoc` schema for a full list of fields returned by this route.",
     },
     {
-        "name": "XAS",
+        "name": "Materials XAS",
         "description": "Route providing computed x-ray absorption spectroscopy data for a material following the \
             methodology discussed by [Mathew *et al.*](https://doi.org/10.1038/sdata.2018.151) \
             and [Chen *et al.*](https://doi.org/10.1038/s41597-021-00936-5) \
             Note that x-ray absorption spectroscopy data has not been calculated for all materials in the Materials \
             Project database. See the `XASDoc` schema for a full list of fields returned by this route.",
     },
     {
-        "name": "Grain Boundaries",
+        "name": "Materials Grain Boundaries",
         "description": "Route providing computed grain boundary data for a material following the \
             methodology discussed by [Hui *et al.*](https://doi.org/10.1016/j.actamat.2019.12.030) \
             Note that grain boundary data has not been calculated for all materials in the Materials \
             Project database. See the `GrainBoundaryDoc` schema for a full list of fields returned by this route.",
     },
     {
-        "name": "Electronic Structure",
+        "name": "Materials Electronic Structure",
         "description": "Routes providing computed electronic structure related data for a material such as \
             band gap and fermi level. Python objects for line-mode band structures, density of states, and \
             fermi surfaces are also available. This data was obtained following the methodology discussed by \
             [Munro *et al.*](https://doi.org/10.1038/s41524-020-00383-7) and [Ganose *et al.*](https://doi.org/10.21105/joss.03089) \
             Note that full band structure, density of states, and fermi surface data has not been calculated for \
             all materials in the Materials Project database. See the `ElectronicStructureDoc` and `FermiDoc` schema \
             for a full list of fields returned by the associated routes.",
         "externalDocs": {
             "description": "For a more detailed description",
             "url": "https://docs.materialsproject.org/methodology/electronic-structure",
         },
     },
     {
-        "name": "Elasticity",
+        "name": "Materials Elasticity",
         "description": "Route providing computed elasticity data for a material following the \
             methodology discussed by [de Jong *et al.*](https://doi.org/10.1038/sdata.2015.9) \
             Note that elasticity data has not been calculated for all materials in the Materials \
             Project database. See the `ElasticityDoc` schema for a full list of fields returned by this route.",
         "externalDocs": {
             "description": "For a more detailed description",
             "url": "https://docs.materialsproject.org/methodology/elasticity",
         },
     },
     {
-        "name": "DOIs",
-        "description": "Route providing DOI and bibtex reference information for a material. \
-            Note that this data may not be available for all materials in the Materials \
-            Project database. See the `DOIDoc` schema for a full list of fields returned by this route.",
-    },
-    {
-        "name": "Substrates",
+        "name": "Materials Substrates",
         "description": "Route providing computed suggested substrate data for a material following the \
             methodology discussed by [Ding *et al.*](https://doi.org/10.1021/acsami.6b01630) \
             Note that substrate data has not been calculated for all materials in the Materials \
             Project database. See the `SubstratesDoc` schema for a full list of fields returned by this route.",
     },
     {
-        "name": "Surface Properties",
+        "name": "Materials Surface Properties",
         "description": "Route providing computed surface property data for a material following the \
             methodology discussed by [Tran *et al.*](https://doi.org/10.1038/sdata.2016.80) \
             Note that surface data has not been calculated for all materials in the Materials \
             Project database. See the `SurfacePropDoc` schema for a full list of fields returned by this route.",
     },
     {
         "name": "Robocrystallographer",
         "description": "Route providing a computed text description for a material following the \
             methodology discussed by [Ganose *et al.*](https://doi.org/10.1557/mrc.2019.94) \
             Note that descriptions may not been calculated for all materials in the Materials \
             Project database. See the `RobocrysDoc` schema for a full list of fields returned by this route.",
     },
     {
-        "name": "Synthesis",
+        "name": "Materials Synthesis",
         "description": "Route providing a synthesis recipes for materials extracted from literature \
             following the methodology discussed by [Kononova *et al.*](https://doi.org/10.1038/s41597-019-0224-1) \
             Note that synthesis recipes may not be available for all materials in the Materials \
             Project database. See the `SynthesisSearchResultModel` schema for a full list of fields returned by this route.",
     },
     {
         "name": "Electrodes",
         "description": "Route providing computed electrode data for a material following the \
             methodology discussed by [Shen *et al.*](https://doi.org/10.1038/s41524-020-00422-3) \
             Note that electrode data has not been calculated for all materials in the Materials \
             Project database. See the `InsertionElectrodeDoc` schema for a full list of fields returned by this route.",
     },
     {
-        "name": "Molecules",
-        "description": "Route providing computed data for a molecule such as charge, \
-            electron affinity, and ionization energy. The unique identifier for a molecule \
-            is its `task_id` (e.g. `mol-45807`). See the `MoleculesDoc` schema for a full list of \
-            fields returned by this route.",
-    },
-    {
-        "name": "Oxidation States",
+        "name": "Materials Oxidation States",
         "description": "Route providing computed oxidation state data for a material following the \
             methodology employed by the [BVAnalyzer](https://pymatgen.org/pymatgen.analysis.bond_valence.html) \
             in Pymatgen. Note that oxidation state data has not been calculated for all materials in the Materials \
             Project database. See the `OxidationStateDoc` schema for a full list of fields returned by this route.",
     },
     {
-        "name": "Provenance",
+        "name": "Materials Provenance",
         "description": "Route providing provenance data for a material such as whether it is theoretical, \
             its associated ICSD entries, and relevant references in literature. Note that provenance data \
             may not be available for all materials in the Materials Project database. See the `ProvenanceDoc` \
             schema for a full list of fields returned by this route.",
     },
     {
-        "name": "Charge Density",
+        "name": "Materials Charge Density",
         "description": "Route providing computed charge density data for a material following the \
             methodology discussed by [Shen *et al.*](https://arxiv.org/abs/2107.03540). Please email \
             <heavy.api.use@materialsproject.org> if you would like to retrieve a large amount of this data. \
             Note that charge densities may not be calculated for all materials in the Materials \
             Project database. See the `ChgcarDataDoc` schema for a full list of fields returned by this route.",
     },
     {
+        "name": "Materials Alloys",
+        "description": "Route for retrevial of information about which hypothetical alloy(s) a given material might "
+                       "belong to, following the methodolgy discussed by "
+                       "[Woods-Robinson, Horton and Persson](https://arxiv.org/pdf/2206.10715)."
+    },
+    {
         "name": "MPComplete",
         "description": "Route for submitting structures to the Materials Project. If calculations are run with the \
             submitted structure, the submitter will be credited with the submitted public name and email.",
     },
     {
-        "name": "Alloys",
-        "description": "Route for retrevial of information about which hypothetical alloy(s) a given material might "
-                       "belong to, following the methodolgy discussed by "
-                       "[Woods-Robinson, Horton and Persson](https://arxiv.org/pdf/2206.10715)."
-    }
+        "name": "DOIs",
+        "description": "Route providing DOI and bibtex reference information for a material. \
+            Note that this data may not be available for all materials in the Materials \
+            Project database. See the `DOIDoc` schema for a full list of fields returned by this route.",
+    },
+    {
+        "name": "Molecules Tasks",
+        "description": "Route for basic task information for DFT calculations in the Materials Project \
+            molecules database. Multiple calculations can ultimately be associated with a unique molecule, \
+            and are the source of its reported properties. The unique identifier for a calculation is its \
+            `task_id`. See the `TaskDocument` schema for a full list of fields returned by this route."
+    },
+    {
+        "name": "Associated Molecules",
+        "description": "Route for 'associated' molecule data. Construction of the Materials Project molecules \
+            database occurs in two stages. In the first stage, calculations using the exact same formula, charge, \
+            spin multiplicity, and molecular geometry (defined by bond lengths, angles, etc.) are associated. \
+            In the second stage, multiple 'associated molecules' with the same basic properties (formula, charge, spin) \
+            and connectivity (based on molecular graph isomorphism) are collected, forming the 'core' molecules \
+            collection. This route provides access to data for individual 'associated molecules'. The 'Core Molecules' \
+            route (/molecules/molecules/) contains data for core molecules. See the `MoleculeDoc` schema for a full list \
+            of fields returned by this route."
+    },
+    {
+        "name": "Core Molecules",
+        "description": "Route for 'core' molecule data. Construction of the Materials Project molecules \
+            database occurs in two stages. In the first stage, calculations using the exact same formula, charge, \
+            spin multiplicity, and molecular geometry (defined by bond lengths, angles, etc.) are associated. \
+            In the second stage, multiple 'associated molecules' with the same basic properties (formula, charge, spin) \
+            and connectivity (based on molecular graph isomorphism) are collected, forming the 'core' molecules \
+            collection. This route provides access to data for individual 'associated molecules'. The 'Associated Molecules' \
+            route (/molecules/assoc/) contains data for 'associated' molecules. See the `MoleculeDoc` schema for a full list \
+            of fields returned by this route."
+    },
+    {
+        "name": "Molecules Partial Charges",
+        "description": "Route for molecular partial charge data. See the `PartialChargesDoc` schema for a full list \
+            of fields returned by this route."
+    },
+    {
+        "name": "Molecules Partial Spins",
+        "description": "Route for molecular partial spin data. See the `PartialSpinsDoc` schema for a full list \
+            of fields returned by this route."
+    },
+    {
+        "name": "Molecules Bonds",
+        "description": "Route for molecular bonding data. See the `MoleculeBondingDoc` schema for a full list \
+            of fields returned by this route."
+    },
+    {
+        "name": "Molecules Orbitals",
+        "description": "Route for molecular orbital information obtained via Natural Bonding Orbital analysis. \
+            See the `OrbitalDoc` schema for a full list of fields returned by this route."
+    },
+    {
+        "name": "Molecules Redox",
+        "description": "Route for molecular redox information (e.g. ionization energy, reduction free energy, \
+            redox potentials). See the `RedoxDoc` schema for a full list of fields returned by this route."
+    },
+    {
+        "name": "Molecules Thermo",
+        "description": "Route for molecular thermochemistry information. See the `MoleculeThermoDoc` schema for \
+            a full list of fields returned by this route."
+    },
+    {
+        "name": "Molecules Vibrations",
+        "description": "Route for molecular normal mode and IR spectroscopy data. See the `VibrationDoc` schema for \
+            a full list of fields returned by this route."
+    },
+    {
+        "name": "Molecules Summary",
+        "description": "Route for a summary of all data calculated on 'core' molecules in the Materials Project \
+            molecules database. See the `MoleculeSummaryDoc` schema for a full list of fields returned by this route."
+    },
+    {
+        "name": "JCESR Electrolyte Genome",
+        "description": "Route providing computed data for a legacy molecule such as charge, \
+            electron affinity, and ionization energy. The unique identifier for a molecule \
+            is its `task_id` (e.g. `mol-45807`). See the `MoleculesDoc` schema for a full list of \
+            fields returned by this route.",
+    },
 ]
```

### Comparing `emmet-api-0.51.9/emmet/api/core/global_header.py` & `emmet-api-0.52.0/emmet/api/core/global_header.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/emmet/api/core/settings.py` & `emmet-api-0.52.0/emmet/api/core/settings.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/emmet/api/routes/_consumer/query_operator.py` & `emmet-api-0.52.0/emmet/api/routes/_consumer/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/emmet/api/routes/_consumer/resources.py` & `emmet-api-0.52.0/emmet/api/routes/_consumer/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/emmet/api/routes/_general_store/query_operator.py` & `emmet-api-0.52.0/emmet/api/routes/_general_store/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/emmet/api/routes/_general_store/resources.py` & `emmet-api-0.52.0/emmet/api/routes/_general_store/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/emmet/api/routes/absorption/resources.py` & `emmet-api-0.52.0/emmet/api/routes/materials/absorption/resources.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from maggma.api.query_operator import PaginationQuery, SortQuery, SparseFieldsQuery, NumericQuery
 from maggma.api.resource import ReadOnlyResource
 
 from emmet.api.core.global_header import GlobalHeaderProcessor
 from emmet.api.core.settings import MAPISettings
-from emmet.api.routes.materials.query_operators import MultiMaterialIDQuery
+from emmet.api.routes.materials.materials.query_operators import MultiMaterialIDQuery
 from emmet.core.absorption import AbsorptionDoc
 
 
 def absorption_resource(absorption_store):
     resource = ReadOnlyResource(
         absorption_store,
         AbsorptionDoc,
@@ -25,13 +25,14 @@
                 ],
             ),
             SortQuery(),
             PaginationQuery(),
             SparseFieldsQuery(AbsorptionDoc, default_fields=["material_id", "last_updated"],),
         ],
         header_processor=GlobalHeaderProcessor(),
-        tags=["Absorption"],
+        tags=["Materials Absorption"],
+        sub_path="/absorption/",
         disable_validation=True,
         timeout=MAPISettings().TIMEOUT,
     )
 
     return resource
```

### Comparing `emmet-api-0.51.9/emmet/api/routes/alloys/query_operators.py` & `emmet-api-0.52.0/emmet/api/routes/materials/alloys/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/emmet/api/routes/alloys/resources.py` & `emmet-api-0.52.0/emmet/api/routes/materials/alloys/resources.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from maggma.api.resource import ReadOnlyResource
 
 from maggma.api.query_operator import PaginationQuery, SortQuery, SparseFieldsQuery
 
 from emmet.core.alloys import AlloyPairDoc
 
 from emmet.api.core.settings import MAPISettings
-from emmet.api.routes.alloys.query_operators import (
+from emmet.api.routes.materials.alloys.query_operators import (
     MaterialIDsSearchQuery,
     FormulaSearchQuery,
 )
 
 
 def alloy_pairs_resource(alloy_pairs_store):
     resource = ReadOnlyResource(
@@ -18,13 +18,14 @@
         query_operators=[
             MaterialIDsSearchQuery(),
             FormulaSearchQuery(),
             SortQuery(),
             PaginationQuery(),
             SparseFieldsQuery(AlloyPairDoc, default_fields=["pair_id"],),
         ],
-        tags=["Alloys"],
+        tags=["Materials Alloys"],
+        sub_path="/alloys/",
         disable_validation=True,
         timeout=MAPISettings().TIMEOUT,
     )
 
     return resource
```

### Comparing `emmet-api-0.51.9/emmet/api/routes/bonds/query_operators.py` & `emmet-api-0.52.0/emmet/api/routes/materials/bonds/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/emmet/api/routes/bonds/resources.py` & `emmet-api-0.52.0/emmet/api/routes/materials/xas/resources.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,47 @@
 from maggma.api.resource import ReadOnlyResource
-from emmet.core.bonds import BondingDoc
+from emmet.core.xas import XASDoc
 
 from maggma.api.query_operator import PaginationQuery, SortQuery, SparseFieldsQuery
-
-from emmet.api.routes.bonds.query_operators import (
-    BondLengthQuery,
-    CoordinationEnvsQuery,
+from emmet.api.routes.materials.materials.query_operators import (
+    ElementsQuery,
+    FormulaQuery,
+    ChemsysQuery,
 )
-from emmet.api.routes.materials.query_operators import MultiMaterialIDQuery
-from emmet.api.core.settings import MAPISettings
 from emmet.api.core.global_header import GlobalHeaderProcessor
+from emmet.api.routes.materials.xas.query_operators import XASQuery, XASTaskIDQuery
+from emmet.api.core.settings import MAPISettings
 
 
-def bonds_resource(bonds_store):
+def xas_resource(xas_store):
     resource = ReadOnlyResource(
-        bonds_store,
-        BondingDoc,
+        xas_store,
+        XASDoc,
         query_operators=[
-            MultiMaterialIDQuery(),
-            BondLengthQuery(),
-            CoordinationEnvsQuery(),
+            FormulaQuery(),
+            ChemsysQuery(),
+            ElementsQuery(),
+            XASQuery(),
+            XASTaskIDQuery(),
             SortQuery(),
             PaginationQuery(),
-            SparseFieldsQuery(BondingDoc, default_fields=["material_id", "last_updated"],),
+            SparseFieldsQuery(
+                XASDoc,
+                default_fields=[
+                    "xas_id",
+                    "task_id",
+                    "edge",
+                    "absorbing_element",
+                    "formula_pretty",
+                    "spectrum_type",
+                    "last_updated",
+                ],
+            ),
         ],
         header_processor=GlobalHeaderProcessor(),
-        tags=["Bonds"],
+        tags=["Materials XAS"],
+        sub_path="/xas/",
         disable_validation=True,
         timeout=MAPISettings().TIMEOUT,
     )
 
     return resource
```

### Comparing `emmet-api-0.51.9/emmet/api/routes/charge_density/query_operators.py` & `emmet-api-0.52.0/emmet/api/routes/materials/charge_density/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/emmet/api/routes/charge_density/resources.py` & `emmet-api-0.52.0/emmet/api/routes/materials/charge_density/resources.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from maggma.api.resource import ReadOnlyResource
 from maggma.api.query_operator import PaginationQuery, SparseFieldsQuery
 from emmet.core.charge_density import ChgcarDataDoc
-from emmet.api.routes.charge_density.query_operators import ChgcarTaskIDQuery
+from emmet.api.routes.materials.charge_density.query_operators import ChgcarTaskIDQuery
 from emmet.api.core.global_header import GlobalHeaderProcessor
 
 
 def charge_density_resource(s3_store):
     resource = ReadOnlyResource(
         s3_store,
         ChgcarDataDoc,
@@ -13,29 +13,31 @@
             ChgcarTaskIDQuery(),
             PaginationQuery(),
             SparseFieldsQuery(
                 ChgcarDataDoc, default_fields=["task_id", "last_updated", "fs_id"]
             ),
         ],
         header_processor=GlobalHeaderProcessor(),
-        tags=["Charge Density"],
+        tags=["Materials Charge Density"],
+        sub_path="/charge_density/",
         enable_default_search=True,
         enable_get_by_key=False,
         disable_validation=True,
         query_disk_use=False,
     )
 
     return resource
 
 
 def charge_density_url_resource(s3_store):
     resource = ReadOnlyResource(
         s3_store,
         ChgcarDataDoc,
         key_fields=["task_id", "fs_id", "url", "s3_url_prefix", "requested_datetime", "expiry_datetime"],
-        tags=["Charge Density"],
+        tags=["Materials Charge Density"],
+        sub_path="/charge_density/",
         enable_default_search=False,
         enable_get_by_key=True,
         disable_validation=True,
     )
 
     return resource
```

### Comparing `emmet-api-0.51.9/emmet/api/routes/chemenv/query_operators.py` & `emmet-api-0.52.0/emmet/api/routes/materials/chemenv/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/emmet/api/routes/chemenv/resources.py` & `emmet-api-0.52.0/emmet/api/routes/materials/chemenv/resources.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from maggma.api.query_operator import PaginationQuery, SortQuery, SparseFieldsQuery, NumericQuery
 from maggma.api.resource import ReadOnlyResource
 
 from emmet.api.core.global_header import GlobalHeaderProcessor
 from emmet.api.core.settings import MAPISettings
-from emmet.api.routes.materials.query_operators import MultiMaterialIDQuery
-from emmet.api.routes.chemenv.query_operators import ChemEnvQuery
+from emmet.api.routes.materials.materials.query_operators import MultiMaterialIDQuery
+from emmet.api.routes.materials.chemenv.query_operators import ChemEnvQuery
 from emmet.core.chemenv import ChemEnvDoc
 
 
 def chemenv_resource(chemenv_store):
     resource = ReadOnlyResource(
         chemenv_store,
         ChemEnvDoc,
@@ -17,13 +17,14 @@
             ChemEnvQuery(),
             NumericQuery(model=ChemEnvDoc, excluded_fields=["valences"]),
             SortQuery(),
             PaginationQuery(),
             SparseFieldsQuery(ChemEnvDoc, default_fields=["material_id", "formula_pretty", "last_updated"],),
         ],
         header_processor=GlobalHeaderProcessor(),
-        tags=["Chemical Environment"],
+        tags=["Materials Chemical Environment"],
+        sub_path="/chemenv/",
         disable_validation=True,
         timeout=MAPISettings().TIMEOUT,
     )
 
     return resource
```

### Comparing `emmet-api-0.51.9/emmet/api/routes/dielectric/query_operators.py` & `emmet-api-0.52.0/emmet/api/routes/materials/dielectric/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/emmet/api/routes/dielectric/resources.py` & `emmet-api-0.52.0/emmet/api/routes/materials/dielectric/resources.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from maggma.api.resource import ReadOnlyResource
 from emmet.core.polar import DielectricDoc
 
 from maggma.api.query_operator import PaginationQuery, SortQuery, SparseFieldsQuery
-from emmet.api.routes.dielectric.query_operators import DielectricQuery
-from emmet.api.routes.materials.query_operators import MultiMaterialIDQuery
+from emmet.api.routes.materials.dielectric.query_operators import DielectricQuery
+from emmet.api.routes.materials.materials.query_operators import MultiMaterialIDQuery
 from emmet.api.core.global_header import GlobalHeaderProcessor
 from emmet.api.core.settings import MAPISettings
 
 
 def dielectric_resource(dielectric_store):
     resource = ReadOnlyResource(
         dielectric_store,
@@ -16,13 +16,14 @@
             MultiMaterialIDQuery(),
             DielectricQuery(),
             SortQuery(),
             PaginationQuery(),
             SparseFieldsQuery(DielectricDoc, default_fields=["material_id", "last_updated"]),
         ],
         header_processor=GlobalHeaderProcessor(),
-        tags=["Dielectric"],
+        tags=["Materials Dielectric"],
+        sub_path="/dielectric/",
         disable_validation=True,
         timeout=MAPISettings().TIMEOUT,
     )
 
     return resource
```

### Comparing `emmet-api-0.51.9/emmet/api/routes/dois/resources.py` & `emmet-api-0.52.0/emmet/api/routes/dois/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/emmet/api/routes/elasticity/query_operators.py` & `emmet-api-0.52.0/emmet/api/routes/materials/elasticity/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/emmet/api/routes/elasticity/resources.py` & `emmet-api-0.52.0/emmet/api/routes/materials/elasticity/resources.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from maggma.api.resource import ReadOnlyResource
 from emmet.core.elasticity_legacy import ElasticityDoc
 from emmet.api.core.global_header import GlobalHeaderProcessor
 from maggma.api.query_operator import PaginationQuery, SortQuery, SparseFieldsQuery
-from emmet.api.routes.elasticity.query_operators import (
+from emmet.api.routes.materials.elasticity.query_operators import (
     ElasticityChemsysQuery,
     BulkModulusQuery,
     ShearModulusQuery,
     PoissonQuery,
 )
 
 from emmet.api.core.settings import MAPISettings
@@ -24,13 +24,14 @@
             SortQuery(),
             PaginationQuery(),
             SparseFieldsQuery(
                 ElasticityDoc, default_fields=["task_id", "pretty_formula"],
             ),
         ],
         header_processor=GlobalHeaderProcessor(),
-        tags=["Elasticity"],
+        tags=["Materials Elasticity"],
+        sub_path="/elasticity/",
         disable_validation=False,
         timeout=MAPISettings().TIMEOUT
     )
 
     return resource
```

### Comparing `emmet-api-0.51.9/emmet/api/routes/electrodes/query_operators.py` & `emmet-api-0.52.0/emmet/api/routes/materials/electrodes/query_operators.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional
 from fastapi import Query
 from maggma.api.query_operator import QueryOperator
 from maggma.api.utils import STORE_PARAMS
-from emmet.api.routes.electrodes.utils import (
+from emmet.api.routes.materials.electrodes.utils import (
     electrodes_formula_to_criteria,
     electrodes_chemsys_to_criteria,
 )
 from pymatgen.core.periodic_table import Element
 from fastapi import HTTPException
 
 from collections import defaultdict
```

### Comparing `emmet-api-0.51.9/emmet/api/routes/electrodes/resources.py` & `emmet-api-0.52.0/emmet/api/routes/materials/electrodes/resources.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from maggma.api.query_operator.dynamic import NumericQuery
 from maggma.api.resource import ReadOnlyResource
 from emmet.core.electrode import InsertionElectrodeDoc
 from emmet.api.core.global_header import GlobalHeaderProcessor
 
 from maggma.api.query_operator import PaginationQuery, SortQuery, SparseFieldsQuery
-from emmet.api.routes.electrodes.query_operators import (
+from emmet.api.routes.materials.electrodes.query_operators import (
     ElectrodeFormulaQuery,
     ElectrodeElementsQuery,
     ElectrodesChemsysQuery,
     WorkingIonQuery,
     ElectrodeMultiMaterialIDQuery,
     MultiBatteryIDQuery
 )
@@ -32,12 +32,13 @@
             PaginationQuery(),
             SparseFieldsQuery(
                 InsertionElectrodeDoc, default_fields=["battery_id", "last_updated"],
             ),
         ],
         header_processor=GlobalHeaderProcessor(),
         tags=["Electrodes"],
+        sub_path="/insertion_electrodes/",
         disable_validation=True,
         timeout=MAPISettings().TIMEOUT
     )
 
     return resource
```

### Comparing `emmet-api-0.51.9/emmet/api/routes/electrodes/utils.py` & `emmet-api-0.52.0/emmet/api/routes/materials/electrodes/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/emmet/api/routes/electronic_structure/query_operators.py` & `emmet-api-0.52.0/emmet/api/routes/materials/electronic_structure/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/emmet/api/routes/electronic_structure/resources.py` & `emmet-api-0.52.0/emmet/api/routes/materials/electronic_structure/resources.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from maggma.api.query_operator.dynamic import NumericQuery
 from maggma.api.resource import ReadOnlyResource
 from emmet.core.electronic_structure import ElectronicStructureDoc
 from maggma.api.query_operator import PaginationQuery, SortQuery, SparseFieldsQuery
 
-from emmet.api.routes.materials.query_operators import (
+from emmet.api.routes.materials.materials.query_operators import (
     ElementsQuery,
     FormulaQuery,
     ChemsysQuery,
     DeprecationQuery,
     MultiMaterialIDQuery
 )
 
-from emmet.api.routes.electronic_structure.query_operators import (
+from emmet.api.routes.materials.electronic_structure.query_operators import (
     ESSummaryDataQuery,
     BSDataQuery,
     DOSDataQuery,
     ObjectQuery,
 )
 from emmet.core.electronic_structure import BSObjectDoc, DOSObjectDoc
 from emmet.api.core.global_header import GlobalHeaderProcessor
@@ -39,15 +39,16 @@
             SortQuery(),
             PaginationQuery(),
             SparseFieldsQuery(
                 ElectronicStructureDoc, default_fields=["material_id", "last_updated"]
             ),
         ],
         header_processor=GlobalHeaderProcessor(),
-        tags=["Electronic Structure"],
+        tags=["Materials Electronic Structure"],
+        sub_path="/electronic_structure/",
         disable_validation=True,
         timeout=timeout,
     )
 
     return resource
 
 
@@ -62,17 +63,17 @@
             PaginationQuery(),
             SparseFieldsQuery(
                 ElectronicStructureDoc,
                 default_fields=["material_id", "last_updated", "bandstructure"],
             ),
         ],
         header_processor=GlobalHeaderProcessor(),
-        tags=["Electronic Structure"],
+        tags=["Materials Electronic Structure"],
         enable_get_by_key=False,
-        sub_path="/bandstructure/",
+        sub_path="/electronic_structure/bandstructure/",
         disable_validation=True,
         timeout=timeout,
     )
 
     return resource
 
 
@@ -81,18 +82,18 @@
         s3_store,
         BSObjectDoc,
         query_operators=[
             ObjectQuery(),
             SparseFieldsQuery(BSObjectDoc, default_fields=["task_id", "last_updated"]),
         ],
         header_processor=GlobalHeaderProcessor(),
-        tags=["Electronic Structure"],
+        tags=["Materials Electronic Structure"],
         enable_get_by_key=False,
         enable_default_search=True,
-        sub_path="/bandstructure/object/",
+        sub_path="/electronic_structure/bandstructure/object/",
         query_disk_use=False,
         disable_validation=True,
     )
     return resource
 
 
 def dos_resource(es_store):
@@ -106,17 +107,17 @@
             PaginationQuery(),
             SparseFieldsQuery(
                 ElectronicStructureDoc,
                 default_fields=["material_id", "last_updated", "dos"],
             ),
         ],
         header_processor=GlobalHeaderProcessor(),
-        tags=["Electronic Structure"],
+        tags=["Materials Electronic Structure"],
         enable_get_by_key=False,
-        sub_path="/dos/",
+        sub_path="/electronic_structure/dos/",
         disable_validation=True,
         timeout=timeout
     )
 
     return resource
 
 
@@ -125,15 +126,15 @@
         s3_store,
         DOSObjectDoc,
         query_operators=[
             ObjectQuery(),
             SparseFieldsQuery(DOSObjectDoc, default_fields=["task_id", "last_updated"]),
         ],
         header_processor=GlobalHeaderProcessor(),
-        tags=["Electronic Structure"],
+        tags=["Materials Electronic Structure"],
         enable_get_by_key=False,
         enable_default_search=True,
-        sub_path="/dos/object/",
+        sub_path="/electronic_structure/dos/object/",
         query_disk_use=False,
         disable_validation=True,
     )
     return resource
```

### Comparing `emmet-api-0.51.9/emmet/api/routes/eos/resources.py` & `emmet-api-0.52.0/emmet/api/routes/materials/eos/resources.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,13 +14,14 @@
         query_operators=[
             NumericQuery(model=EOSDoc),
             SortQuery(),
             PaginationQuery(),
             SparseFieldsQuery(EOSDoc, default_fields=["task_id"]),
         ],
         header_processor=GlobalHeaderProcessor(),
-        tags=["EOS"],
+        tags=["Materials EOS"],
+        sub_path="/eos/",
         disable_validation=True,
         timeout=MAPISettings().TIMEOUT
     )
 
     return resource
```

### Comparing `emmet-api-0.51.9/emmet/api/routes/fermi/resources.py` & `emmet-api-0.52.0/emmet/api/routes/materials/fermi/resources.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,12 +9,13 @@
         fermi_store,
         FermiDoc,
         query_operators=[
             PaginationQuery(),
             SparseFieldsQuery(FermiDoc, default_fields=["task_id", "last_updated"]),
         ],
         header_processor=GlobalHeaderProcessor(),
-        tags=["Electronic Structure"],
+        tags=["Materials Electronic Structure"],
+        sub_path="/fermi/",
         disable_validation=True,
     )
 
     return resource
```

### Comparing `emmet-api-0.51.9/emmet/api/routes/grain_boundary/query_operators.py` & `emmet-api-0.52.0/emmet/api/routes/materials/grain_boundary/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/emmet/api/routes/grain_boundary/resources.py` & `emmet-api-0.52.0/emmet/api/routes/materials/grain_boundary/resources.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from maggma.api.resource import ReadOnlyResource
 from emmet.core.grain_boundary import GrainBoundaryDoc
 
-from emmet.api.routes.grain_boundary.query_operators import (
+from emmet.api.routes.materials.grain_boundary.query_operators import (
     GBStructureQuery,
     GBTaskIDQuery,
 )
 from maggma.api.query_operator import (
     PaginationQuery,
     SortQuery,
     SparseFieldsQuery,
@@ -28,14 +28,15 @@
             SortQuery(),
             PaginationQuery(),
             SparseFieldsQuery(
                 GrainBoundaryDoc, default_fields=["task_id", "last_updated"]
             ),
         ],
         header_processor=GlobalHeaderProcessor(),
-        tags=["Grain Boundaries"],
+        tags=["Materials Grain Boundaries"],
+        sub_path="/grain_boundary/",
         enable_get_by_key=False,
         disable_validation=True,
         timeout=MAPISettings().TIMEOUT
     )
 
     return resource
```

### Comparing `emmet-api-0.51.9/emmet/api/routes/magnetism/query_operators.py` & `emmet-api-0.52.0/emmet/api/routes/materials/magnetism/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/emmet/api/routes/magnetism/resources.py` & `emmet-api-0.52.0/emmet/api/routes/materials/magnetism/resources.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from maggma.api.resource import ReadOnlyResource
 from emmet.core.magnetism import MagnetismDoc
 
 from maggma.api.query_operator import PaginationQuery, SortQuery, SparseFieldsQuery
-from emmet.api.routes.magnetism.query_operators import MagneticQuery
-from emmet.api.routes.materials.query_operators import MultiMaterialIDQuery
+from emmet.api.routes.materials.magnetism.query_operators import MagneticQuery
+from emmet.api.routes.materials.materials.query_operators import MultiMaterialIDQuery
 from emmet.api.core.global_header import GlobalHeaderProcessor
 from emmet.api.core.settings import MAPISettings
 
 
 def magnetism_resource(magnetism_store):
     resource = ReadOnlyResource(
         magnetism_store,
@@ -16,13 +16,14 @@
             MultiMaterialIDQuery(),
             MagneticQuery(),
             SortQuery(),
             PaginationQuery(),
             SparseFieldsQuery(MagnetismDoc, default_fields=["material_id", "last_updated"]),
         ],
         header_processor=GlobalHeaderProcessor(),
-        tags=["Magnetism"],
+        tags=["Materials Magnetism"],
+        sub_path="/magnetism/",
         disable_validation=True,
         timeout=MAPISettings().TIMEOUT,
     )
 
     return resource
```

### Comparing `emmet-api-0.51.9/emmet/api/routes/materials/query_operators.py` & `emmet-api-0.52.0/emmet/api/routes/materials/materials/query_operators.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from itertools import permutations
 from typing import Optional
 
 from emmet.core.symmetry import CrystalSystem
 from fastapi import Body, HTTPException, Query
 from maggma.api.query_operator import QueryOperator
 from maggma.api.utils import STORE_PARAMS
-from emmet.api.routes.materials.utils import formula_to_criteria, chemsys_to_criteria
+from emmet.api.routes.materials.materials.utils import formula_to_criteria, chemsys_to_criteria
 from pymatgen.analysis.structure_matcher import ElementComparator, StructureMatcher
 from pymatgen.core.composition import Composition, CompositionError
 from pymatgen.core.periodic_table import Element
 from pymatgen.core.structure import Structure
 
 
 class FormulaQuery(QueryOperator):
```

### Comparing `emmet-api-0.51.9/emmet/api/routes/materials/resources.py` & `emmet-api-0.52.0/emmet/api/routes/materials/materials/resources.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 from maggma.api.query_operator import (
     PaginationQuery,
     SparseFieldsQuery,
     SortQuery,
     NumericQuery,
 )
 
-from emmet.api.routes.materials.hint_scheme import MaterialsHintScheme
-from emmet.api.routes.materials.query_operators import (
+from emmet.api.routes.materials.materials.hint_scheme import MaterialsHintScheme
+from emmet.api.routes.materials.materials.query_operators import (
     ElementsQuery,
     FormulaQuery,
     ChemsysQuery,
     DeprecationQuery,
     SymmetryQuery,
     MultiTaskIDQuery,
     FindStructureQuery,
@@ -35,28 +35,28 @@
 def find_structure_resource(materials_store):
     resource = PostOnlyResource(
         materials_store,
         FindStructure,
         key_fields=["structure", "task_id"],
         query_operators=[FindStructureQuery()],
         tags=["Materials"],
-        sub_path="/find_structure/",
+        sub_path="/materials/find_structure/",
         timeout=timeout,
     )
 
     return resource
 
 
 def formula_autocomplete_resource(formula_autocomplete_store):
     resource = AggregationResource(
         formula_autocomplete_store,
         FormulaAutocomplete,
         pipeline_query_operator=FormulaAutoCompleteQuery(),
         tags=["Materials"],
-        sub_path="/formula_autocomplete/",
+        sub_path="/materials/formula_autocomplete/",
         header_processor=GlobalHeaderProcessor(),
         timeout=timeout,
     )
 
     return resource
 
 
@@ -77,12 +77,13 @@
             SortQuery(),
             PaginationQuery(),
             SparseFieldsQuery(MaterialsDoc, default_fields=["material_id", "formula_pretty", "last_updated"],),
         ],
         header_processor=GlobalHeaderProcessor(),
         hint_scheme=MaterialsHintScheme(),
         tags=["Materials"],
+        sub_path="/materials/",
         disable_validation=True,
         timeout=MAPISettings().TIMEOUT,
     )
 
     return resource
```

### Comparing `emmet-api-0.51.9/emmet/api/routes/materials/utils.py` & `emmet-api-0.52.0/emmet/api/routes/materials/materials/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/emmet/api/routes/molecules/query_operators.py` & `emmet-api-0.52.0/emmet/api/routes/legacy/jcesr/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/emmet/api/routes/molecules/resources.py` & `emmet-api-0.52.0/emmet/api/routes/materials/surface_properties/resources.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,29 @@
+from maggma.api.query_operator import PaginationQuery, SortQuery, SparseFieldsQuery
+from maggma.api.query_operator.dynamic import NumericQuery
 from maggma.api.resource import ReadOnlyResource
-from emmet.core.molecules_jcesr import MoleculesDoc
+from emmet.api.core.settings import MAPISettings
 
-from maggma.api.query_operator import PaginationQuery, SortQuery, SparseFieldsQuery
-from emmet.api.routes.molecules.query_operators import (
-    MoleculeBaseQuery,
-    MoleculeElementsQuery,
-    MoleculeFormulaQuery,
-)
-from emmet.api.routes.tasks.query_operators import MultipleTaskIDsQuery
 from emmet.api.core.global_header import GlobalHeaderProcessor
-from emmet.api.core.settings import MAPISettings
+from emmet.api.routes.materials.surface_properties.query_operators import ReconstructedQuery
+from emmet.core.surface_properties import SurfacePropDoc
 
 
-def molecules_resource(molecules_store):
+def surface_props_resource(surface_prop_store):
     resource = ReadOnlyResource(
-        molecules_store,
-        MoleculesDoc,
+        surface_prop_store,
+        SurfacePropDoc,
         query_operators=[
-            MoleculeBaseQuery(),
-            MoleculeElementsQuery(),
-            MoleculeFormulaQuery(),
-            MultipleTaskIDsQuery(),
+            NumericQuery(model=SurfacePropDoc),
+            ReconstructedQuery(),
             SortQuery(),
             PaginationQuery(),
-            SparseFieldsQuery(MoleculesDoc, default_fields=["task_id"]),
+            SparseFieldsQuery(SurfacePropDoc, default_fields=["task_id"]),
         ],
         header_processor=GlobalHeaderProcessor(),
-        tags=["Molecules"],
+        tags=["Materials Surface Properties"],
+        sub_path="/surface_properties/",
         disable_validation=True,
-        timeout=MAPISettings().TIMEOUT
+        timeout=MAPISettings().TIMEOUT,
     )
 
     return resource
```

### Comparing `emmet-api-0.51.9/emmet/api/routes/mpcomplete/query_operator.py` & `emmet-api-0.52.0/emmet/api/routes/materials/mpcomplete/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/emmet/api/routes/mpcomplete/resources.py` & `emmet-api-0.52.0/emmet/api/routes/materials/mpcomplete/resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from maggma.api.resource import SubmissionResource
 from maggma.api.query_operator import PaginationQuery
 from emmet.core.mpcomplete import MPCompleteDoc, MPCompleteDataStatus
-from emmet.api.routes.mpcomplete.query_operator import (
+from emmet.api.routes.materials.mpcomplete.query_operator import (
     MPCompletePostQuery,
     MPCompleteGetQuery,
 )
 from emmet.api.core.settings import MAPISettings
 
 
 def mpcomplete_resource(mpcomplete_store):
```

### Comparing `emmet-api-0.51.9/emmet/api/routes/mpcules/association/resources.py` & `emmet-api-0.52.0/emmet/api/routes/molecules/bonds/resources.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,59 +1,56 @@
-from maggma.api.resource.read_resource import ReadOnlyResource
+from maggma.api.resource import ReadOnlyResource
+from emmet.core.molecules.bonds import MoleculeBondingDoc
 
+from maggma.api.query_operator import PaginationQuery, SortQuery, SparseFieldsQuery
 
-from emmet.core.qchem.molecule import MoleculeDoc
-
-from maggma.api.query_operator import (
-    PaginationQuery,
-    SparseFieldsQuery,
-    SortQuery,
-    NumericQuery,
+from emmet.api.routes.molecules.bonds.query_operators import (
+    BondTypeLengthQuery,
 )
-
-from emmet.api.routes.mpcules.molecules.hint_scheme import MoleculesHintScheme
-from emmet.api.routes.mpcules.molecules.query_operators import (
+from emmet.api.routes.molecules.molecules.query_operators import (
+    MultiMPculeIDQuery,
+    ExactCalcMethodQuery,
     FormulaQuery,
     ChemsysQuery,
     ElementsQuery,
-    ChargeSpinQuery,
-    DeprecationQuery,
-    MultiTaskIDQuery,
-    MultiMPculeIDQuery,
-    CalcMethodQuery,
-    HashQuery
+    ChargeSpinQuery
 )
-
-from emmet.api.core.global_header import GlobalHeaderProcessor
+from emmet.api.routes.molecules.utils import MethodQuery, MultiPropertyIDQuery
 from emmet.api.core.settings import MAPISettings
-
-timeout = MAPISettings().TIMEOUT
+from emmet.api.core.global_header import GlobalHeaderProcessor
 
 
-def mol_assoc_resource(assoc_store):
+def bonding_resource(bonds_store):
     resource = ReadOnlyResource(
-        assoc_store,
-        MoleculeDoc,
+        bonds_store,
+        MoleculeBondingDoc,
         query_operators=[
             MultiMPculeIDQuery(),
+            ExactCalcMethodQuery(),
             FormulaQuery(),
             ChemsysQuery(),
             ElementsQuery(),
             ChargeSpinQuery(),
-            MultiTaskIDQuery(),
-            CalcMethodQuery(),
-            HashQuery(),
-            DeprecationQuery(),
-            NumericQuery(model=MoleculeDoc),
+            MethodQuery(),
+            MultiPropertyIDQuery(),
+            BondTypeLengthQuery(),
             SortQuery(),
             PaginationQuery(),
-            SparseFieldsQuery(MoleculeDoc, default_fields=["molecule_id", "formula_alphabetical", "last_updated"],),
+            SparseFieldsQuery(
+                MoleculeBondingDoc,
+                default_fields=[
+                    "molecule_id",
+                    "property_id",
+                    "solvent",
+                    "method",
+                    "last_updated"
+                ],
+            ),
         ],
         header_processor=GlobalHeaderProcessor(),
-        tags=["MPcules Associated Molecules"],
-        sub_path="/assoc/",
+        tags=["Molecules Bonds"],
+        sub_path="/bonding/",
         disable_validation=True,
-        hint_scheme=MoleculesHintScheme(),
         timeout=MAPISettings().TIMEOUT,
     )
 
     return resource
```

### Comparing `emmet-api-0.51.9/emmet/api/routes/mpcules/bonds/query_operators.py` & `emmet-api-0.52.0/emmet/api/routes/molecules/bonds/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/emmet/api/routes/mpcules/bonds/resources.py` & `emmet-api-0.52.0/emmet/api/routes/molecules/redox/resources.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,56 +1,63 @@
 from maggma.api.resource import ReadOnlyResource
-from emmet.core.molecules.bonds import MoleculeBondingDoc
+from emmet.core.molecules.redox import RedoxDoc
 
-from maggma.api.query_operator import PaginationQuery, SortQuery, SparseFieldsQuery
+from maggma.api.query_operator import (
+    NumericQuery,
+    PaginationQuery,
+    SortQuery,
+    SparseFieldsQuery
+)
 
-from emmet.api.routes.mpcules.bonds.query_operators import (
-    BondTypeLengthQuery,
+from emmet.api.routes.molecules.redox.query_operators import (
+    RedoxPotentialQuery
 )
-from emmet.api.routes.mpcules.molecules.query_operators import (
+from emmet.api.routes.molecules.molecules.query_operators import (
     MultiMPculeIDQuery,
     ExactCalcMethodQuery,
     FormulaQuery,
     ChemsysQuery,
     ElementsQuery,
     ChargeSpinQuery
 )
-from emmet.api.routes.mpcules.utils import MethodQuery, MultiPropertyIDQuery
+from emmet.api.routes.molecules.utils import MultiPropertyIDQuery
 from emmet.api.core.settings import MAPISettings
 from emmet.api.core.global_header import GlobalHeaderProcessor
 
 
-def bonding_resource(bonds_store):
+def redox_resource(redox_store):
     resource = ReadOnlyResource(
-        bonds_store,
-        MoleculeBondingDoc,
+        redox_store,
+        RedoxDoc,
         query_operators=[
             MultiMPculeIDQuery(),
             ExactCalcMethodQuery(),
             FormulaQuery(),
             ChemsysQuery(),
             ElementsQuery(),
             ChargeSpinQuery(),
-            MethodQuery(),
             MultiPropertyIDQuery(),
-            BondTypeLengthQuery(),
+            RedoxPotentialQuery(),
+            NumericQuery(
+                model=RedoxDoc,
+                excluded_fields=[
+                    "charge",
+                    "spin_multiplicity",
+                    "natoms",
+                    "nelements",
+                    "nelectrons",
+                    "reduction_potentials",
+                    "oxidation_potentials"
+                ]
+            ),
             SortQuery(),
             PaginationQuery(),
-            SparseFieldsQuery(
-                MoleculeBondingDoc,
-                default_fields=[
-                    "molecule_id",
-                    "property_id",
-                    "solvent",
-                    "method",
-                    "last_updated"
-                ],
-            ),
+            SparseFieldsQuery(RedoxDoc, default_fields=["molecule_id", "property_id", "solvent", "last_updated"],),
         ],
         header_processor=GlobalHeaderProcessor(),
-        tags=["MPcules Bonds"],
-        sub_path="/bonding/",
+        tags=["Molecules Redox"],
+        sub_path="/redox/",
         disable_validation=True,
         timeout=MAPISettings().TIMEOUT,
     )
 
     return resource
```

### Comparing `emmet-api-0.51.9/emmet/api/routes/mpcules/molecules/query_operators.py` & `emmet-api-0.52.0/emmet/api/routes/molecules/molecules/query_operators.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from typing import Any, Dict, Optional
 
 from fastapi import Body, HTTPException, Query
 
 from maggma.api.query_operator import QueryOperator
 from maggma.api.utils import STORE_PARAMS
 
-from emmet.api.routes.materials.utils import chemsys_to_criteria
+from emmet.api.routes.materials.materials.utils import chemsys_to_criteria
 
 from pymatgen.analysis.molecule_matcher import MoleculeMatcher
-from pymatgen.analysis.graphs import MoleculeGraph
-from pymatgen.analysis.local_env import OpenBabelNN, metal_edge_extender
 from pymatgen.core.periodic_table import Element
 from pymatgen.core.structure import Molecule
 
 
 class FormulaQuery(QueryOperator):
     """
     Factory method to generate a dependency for querying by
@@ -196,27 +194,27 @@
 class MultiMPculeIDQuery(QueryOperator):
     """
     Method to generate a query for different root-level mpcule_id values
     """
 
     def query(
         self,
-        mpcule_ids: Optional[str] = Query(None, description="Comma-separated list of mpcule_id values to query on"),
+        molecule_ids: Optional[str] = Query(None, description="Comma-separated list of MPculeIDs to query on"),
     ) -> STORE_PARAMS:
 
         crit = {}  # type: dict
 
-        if mpcule_ids:
+        if molecule_ids:
 
-            mpcule_ids_list = [mpcule_id.strip() for mpcule_id in mpcule_ids.split(",")]
+            molecule_ids_list = [mpcule_id.strip() for mpcule_id in molecule_ids.split(",")]
 
-            if len(mpcule_ids_list) == 1:
-                crit.update({"molecule_id": mpcule_ids_list[0]})
+            if len(molecule_ids_list) == 1:
+                crit.update({"molecule_id": molecule_ids_list[0]})
             else:
-                crit.update({"molecule_id": {"$in": mpcule_ids_list}})
+                crit.update({"molecule_id": {"$in": molecule_ids_list}})
 
         return {"criteria": crit}
 
 
 class FindMoleculeQuery(QueryOperator):
     """
     Method to generate a find molecule query
@@ -297,97 +295,14 @@
 
         return response
 
     def ensure_indexes(self):  # pragma: no cover
         return [("composition", False)]
 
 
-class FindMoleculeConnectivityQuery(QueryOperator):
-    """
-    Method to generate a find molecule connectivity query
-    """
-
-    def query(
-        self,
-        molecule: Molecule = Body(..., description="Pymatgen Molecule object to query with",),
-        charge: Optional[int] = Query(
-            None, description="Molecule charge. If None (default), don't limit by charge."
-        ),
-        spin_multiplicity: Optional[int] = Query(
-            None, description="Molecule spin_multiplicity. If None (default), don't limit by spin multiplicity."
-        ),
-        _limit: int = Query(
-            10, description="Maximum number of matches to show. Defaults to 10.",
-        ),
-    ) -> STORE_PARAMS:
-
-        self.molecule = molecule
-        self._limit = _limit
-
-        crit: Dict[str, Any] = {}
-
-        if charge is not None:
-            crit.update({"charge": charge})
-
-        if spin_multiplicity is not None:
-            crit.update({"spin_multiplicity": spin_multiplicity})
-
-        try:
-            if isinstance(molecule, dict):
-                m = Molecule.from_dict(molecule)  # type: ignore
-            elif isinstance(molecule, Molecule):
-                m = molecule  # type: ignore
-            elif isinstance(molecule, str):
-                m = Molecule.from_str(molecule)  # type: ignore
-            else:
-                raise Exception("Unexpected type for molecule")
-
-            comp = dict(m.composition)  # type: ignore
-            crit.update({"composition": comp})
-            return {"criteria": crit}
-
-        except Exception:
-            raise HTTPException(
-                status_code=404, detail="Body cannot be converted to a pymatgen Molecule object.",
-            )
-
-    def post_process(self, docs, query):
-
-        m1 = Molecule.from_dict(self.molecule)
-        mg1 = metal_edge_extender(
-            MoleculeGraph.with_local_env_strategy(
-                m1, OpenBabelNN()
-            )
-        )
-
-        matches = list()
-
-        for doc in docs:
-
-            m2 = Molecule.from_dict(doc["molecule"])
-            mg2 = metal_edge_extender(
-                MoleculeGraph.with_local_env_strategy(
-                    m2, OpenBabelNN()
-                )
-            )
-
-            if mg1.isomorphic_to(mg2):
-                matches.append(
-                    {"molecule_id": doc["molecule_id"]}
-                )
-
-        # TODO: should these be sorted? If so, how?
-        response = matches[: self._limit]
-
-        return response
-
-    def ensure_indexes(self):  # pragma: no cover
-        return [("composition", False)]
-
-
 class CalcMethodQuery(QueryOperator):
     """
     Method to generate a query based on level of theory and solvent.
 
     This query differs from ExactCalcMethodQuery in that CalcMethodQuery will check
     that the desired level of theory and/or solvent was used for some calculations
     (they are included in the sets of unique levels of theory, solvents, or lot-solvent
```

### Comparing `emmet-api-0.51.9/emmet/api/routes/mpcules/molecules/resources.py` & `emmet-api-0.52.0/emmet/api/routes/molecules/molecules/resources.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 from maggma.api.resource.read_resource import ReadOnlyResource
 from maggma.api.resource.post_resource import PostOnlyResource
 
-
 from emmet.core.qchem.molecule import MoleculeDoc
-from emmet.core.find_structure import FindMolecule, FindMoleculeConnectivity
+from emmet.core.find_structure import FindMolecule
 
 from maggma.api.query_operator import (
     PaginationQuery,
     SparseFieldsQuery,
     SortQuery,
     NumericQuery,
 )
 
-from emmet.api.routes.mpcules.molecules.hint_scheme import MoleculesHintScheme
-from emmet.api.routes.mpcules.molecules.query_operators import (
+from emmet.api.routes.molecules.molecules.hint_scheme import MoleculesHintScheme
+from emmet.api.routes.molecules.molecules.query_operators import (
     FormulaQuery,
     ChemsysQuery,
     ElementsQuery,
     ChargeSpinQuery,
     DeprecationQuery,
     MultiTaskIDQuery,
     MultiMPculeIDQuery,
     FindMoleculeQuery,
-    FindMoleculeConnectivityQuery,
     CalcMethodQuery,
     HashQuery
 )
 
 from emmet.api.core.global_header import GlobalHeaderProcessor
 from emmet.api.core.settings import MAPISettings
 
@@ -35,30 +33,16 @@
 
 def find_molecule_resource(molecules_store):
     resource = PostOnlyResource(
         molecules_store,
         FindMolecule,
         key_fields=["molecule", "molecule_id"],
         query_operators=[FindMoleculeQuery()],
-        tags=["MPcules Molecules"],
-        sub_path="/find_molecule/",
-        timeout=timeout,
-    )
-
-    return resource
-
-
-def find_molecule_connectivity_resource(molecules_store):
-    resource = PostOnlyResource(
-        molecules_store,
-        FindMoleculeConnectivity,
-        key_fields=["molecule", "molecule_id"],
-        query_operators=[FindMoleculeConnectivityQuery()],
-        tags=["MPcules Molecules"],
-        sub_path="/molecules/find_molecule_connectivity/",
+        tags=["Core Molecules"],
+        sub_path="/molecules/find_molecule/",
         timeout=timeout,
     )
 
     return resource
 
 
 def molecules_resource(molecules_store):
@@ -77,15 +61,15 @@
             DeprecationQuery(),
             NumericQuery(model=MoleculeDoc),
             SortQuery(),
             PaginationQuery(),
             SparseFieldsQuery(MoleculeDoc, default_fields=["molecule_id", "formula_alphabetical", "last_updated"],),
         ],
         header_processor=GlobalHeaderProcessor(),
-        tags=["MPcules Molecules"],
+        tags=["Core Molecules"],
         sub_path="/molecules/",
         disable_validation=True,
         hint_scheme=MoleculesHintScheme(),
         timeout=MAPISettings().TIMEOUT,
     )
 
     return resource
```

### Comparing `emmet-api-0.51.9/emmet/api/routes/mpcules/orbitals/query_operators.py` & `emmet-api-0.52.0/emmet/api/routes/molecules/orbitals/query_operators.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,72 +7,68 @@
 class NBOPopulationQuery(QueryOperator):
     """
     Method to generate a query on NBO natural population data.
     """
 
     def query(
         self,
-        open_shell: Optional[bool] = Query(
-            False,
-            description="Should the molecules have unpaired (radical) electrons?"
-        ),
-        electron_type: Optional[str] = Query(
+        electron_type_population: Optional[str] = Query(
             None,
             description="Should alpha ('alpha'), beta ('beta'), or all electrons be considered (None; default)?"
         ),
-        min_core_electron: Optional[float] = Query(
+        min_core_electrons: Optional[float] = Query(
             None,
             description="Minimum number of core electrons in an atom in this molecule."
         ),
-        max_core_electron: Optional[float] = Query(
+        max_core_electrons: Optional[float] = Query(
             None,
             description="Maximum number of core electrons in an atom in this molecule."
         ),
-        min_valence_electron: Optional[float] = Query(
+        min_valence_electrons: Optional[float] = Query(
             None,
             description="Minimum number of valence electrons in an atom in this molecule."
         ),
-        max_valence_electron: Optional[float] = Query(
+        max_valence_electrons: Optional[float] = Query(
             None,
             description="Maximum number of valence electrons in an atom in this molecule."
         ),
-        min_rydberg_electron: Optional[float] = Query(
+        min_rydberg_electrons: Optional[float] = Query(
             None,
             description="Minimum number of Rydberg electrons in an atom in this molecule."
         ),
-        max_rydberg_electron: Optional[float] = Query(
+        max_rydberg_electrons: Optional[float] = Query(
             None,
             description="Maximum number of Rydberg electrons in an atom in this molecule."
         ),
-        min_total_electron: Optional[float] = Query(
+        min_total_electrons: Optional[float] = Query(
             None,
             description="Minimum number of electrons in an atom in this molecule."
         ),
-        max_total_electron: Optional[float] = Query(
+        max_total_electrons: Optional[float] = Query(
             None,
             description="Maximum number of electrons in an atom in this molecule."
         ),
     ) -> STORE_PARAMS:
 
-        crit: Dict[str, Any] = {"open_shell": open_shell}  # type: ignore
+        crit: Dict[str, Any] = dict()  # type: ignore
 
         d = {
-            "core_electrons": [min_core_electron, max_core_electron],
-            "valence_electrons": [min_valence_electron, max_valence_electron],
-            "rydberg_electrons": [min_rydberg_electron, max_rydberg_electron],
-            "total_electrons": [min_total_electron, max_total_electron]
+            "core_electrons": [min_core_electrons, max_core_electrons],
+            "valence_electrons": [min_valence_electrons, max_valence_electrons],
+            "rydberg_electrons": [min_rydberg_electrons, max_rydberg_electrons],
+            "total_electrons": [min_total_electrons, max_total_electrons]
         }
 
-        if electron_type is None or not open_shell:
+        if electron_type_population is None:
             prefix = "nbo_population."
         else:
             try:
-                if electron_type.lower() == "alpha":
+                if electron_type_population.lower() == "alpha":
                     prefix = "alpha_population."
-                elif electron_type.lower() == "beta":
+                elif electron_type_population.lower() == "beta":
                     prefix = "beta_population."
                 else:
                     raise ValueError("electron_type must be 'alpha' or 'beta' (open-shell), or None (closed-shell)!")
             except AttributeError:
                 raise ValueError("electron_type must be 'alpha' or 'beta' (open-shell), or None (closed-shell)!")
 
         for entry in d:
@@ -107,19 +103,15 @@
 class NBOLonePairQuery(QueryOperator):
     """
     Method to generate a query on NBO lone pair data.
     """
 
     def query(
         self,
-        open_shell: Optional[bool] = Query(
-            False,
-            description="Should the molecules have unpaired (radical) electrons?"
-        ),
-        electron_type: Optional[str] = Query(
+        electron_type_lp: Optional[str] = Query(
             None,
             description="Should alpha ('alpha'), beta ('beta'), or all electrons be considered (None; default)?"
         ),
         lp_type: Optional[str] = Query(
             None,
             description="Type of orbital - 'LP' for 'lone pair' or 'LV' for 'lone vacant'"
         ),
@@ -151,40 +143,40 @@
             None,
             description="Minimum percentage of the lone pair constituted by f atomic orbitals."
         ),
         max_f_character: Optional[float] = Query(
             None,
             description="Maximum percentage of the lone pair constituted by f atomic orbitals."
         ),
-        min_occupancy: Optional[float] = Query(
+        min_lp_occupancy: Optional[float] = Query(
             None,
             description="Minimum number of electrons in the lone pair."
         ),
-        max_occupancy: Optional[float] = Query(
+        max_lp_occupancy: Optional[float] = Query(
             None,
             description="Maximum number of electrons in the lone pair."
         ),
     ) -> STORE_PARAMS:
-        crit: Dict[str, Any] = {"open_shell": open_shell}  # type: ignore
+        crit: Dict[str, Any] = dict()  # type: ignore
 
         d = {
             "s_character": [min_s_character, max_s_character],
             "p_character": [min_p_character, max_p_character],
             "d_character": [min_d_character, max_d_character],
             "f_character": [min_f_character, max_f_character],
-            "occupancy": [min_occupancy, max_occupancy],
+            "occupancy": [min_lp_occupancy, max_lp_occupancy],
         }
 
-        if electron_type is None or not open_shell:
+        if electron_type_lp is None:
             prefix = "nbo_lone_pairs."
         else:
             try:
-                if electron_type.lower() == "alpha":
+                if electron_type_lp.lower() == "alpha":
                     prefix = "alpha_lone_pairs."
-                elif electron_type.lower() == "beta":
+                elif electron_type_lp.lower() == "beta":
                     prefix = "beta_lone_pairs."
                 else:
                     raise ValueError("electron_type must be 'alpha' or 'beta' (open-shell), or None (closed-shell)!")
             except AttributeError:
                 raise ValueError("electron_type must be 'alpha' or 'beta' (open-shell), or None (closed-shell)!")
 
         for entry in d:
@@ -223,19 +215,15 @@
 class NBOBondQuery(QueryOperator):
     """
     Method to generate a query on NBO bond data.
     """
 
     def query(
         self,
-        open_shell: Optional[bool] = Query(
-            False,
-            description="Should the molecules have unpaired (radical) electrons?"
-        ),
-        electron_type: Optional[str] = Query(
+        electron_type_bond: Optional[str] = Query(
             None,
             description="Should alpha ('alpha'), beta ('beta'), or all electrons be considered (None; default)?"
         ),
         bond_type: Optional[str] = Query(
             None,
             description="Type of orbital, e.g. 'BD' for bonding or 'BD*' for antibonding"
         ),
@@ -315,46 +303,46 @@
             None,
             description="Minimum fraction of electrons in the bond donated by the second atom."
         ),
         max_polarization_atom2: Optional[float] = Query(
             None,
             description="Maximum fraction of electrons in the bond donated by the second atom."
         ),
-        min_occupancy: Optional[float] = Query(
+        min_bond_occupancy: Optional[float] = Query(
             None,
             description="Minimum number of electrons in the bond."
         ),
-        max_occupancy: Optional[float] = Query(
+        max_bond_occupancy: Optional[float] = Query(
             None,
             description="Maximum number of electrons in the bond."
         ),
     ) -> STORE_PARAMS:
-        crit: Dict[str, Any] = {"open_shell": open_shell}  # type: ignore
+        crit: Dict[str, Any] = dict()  # type: ignore
 
         d = {
             "atom1_s_character": [min_s_character_atom1, max_s_character_atom1],
             "atom1_p_character": [min_p_character_atom1, max_p_character_atom1],
             "atom1_d_character": [min_d_character_atom1, max_d_character_atom1],
             "atom1_f_character": [min_f_character_atom1, max_f_character_atom1],
             "atom2_s_character": [min_s_character_atom2, max_s_character_atom2],
             "atom2_p_character": [min_p_character_atom2, max_p_character_atom2],
             "atom2_d_character": [min_d_character_atom2, max_d_character_atom2],
             "atom2_f_character": [min_f_character_atom2, max_f_character_atom2],
             "atom1_polarization": [min_polarization_atom1, max_polarization_atom1],
             "atom2_polarization": [min_polarization_atom2, max_polarization_atom2],
-            "occupancy": [min_occupancy, max_occupancy],
+            "occupancy": [min_bond_occupancy, max_bond_occupancy],
         }
 
-        if electron_type is None or not open_shell:
+        if electron_type_bond is None:
             prefix = "nbo_bonds."
         else:
             try:
-                if electron_type.lower() == "alpha":
+                if electron_type_bond.lower() == "alpha":
                     prefix = "alpha_bonds."
-                elif electron_type.lower() == "beta":
+                elif electron_type_bond.lower() == "beta":
                     prefix = "beta_bonds."
                 else:
                     raise ValueError("electron_type must be 'alpha' or 'beta' (open-shell), or None (closed-shell)!")
             except AttributeError:
                 raise ValueError("electron_type must be 'alpha' or 'beta' (open-shell), or None (closed-shell)!")
 
         for entry in d:
@@ -397,19 +385,15 @@
 
 
 class NBOInteractionQuery(QueryOperator):
     """Method to generate a query on NBO orbital-orbital interaction data"""
 
     def query(
         self,
-        open_shell: Optional[bool] = Query(
-            False,
-            description="Should the molecules have unpaired (radical) electrons?"
-        ),
-        electron_type: Optional[str] = Query(
+        electron_type_interaction: Optional[str] = Query(
             None,
             description="Should alpha ('alpha'), beta ('beta'), or all electrons be considered (None; default)?"
         ),
         donor_type: Optional[str] = Query(
             None,
             description="Type of donor orbital, e.g. 'BD' for bonding or 'RY*' for anti-Rydberg"
         ),
@@ -438,29 +422,29 @@
             description="Minimum interaction Fock matrix element"
         ),
         max_fock_element: Optional[float] = Query(
             None,
             description="Maximum interaction Fock matrix element"
         ),
     ) -> STORE_PARAMS:
-        crit: Dict[str, Any] = {"open_shell": open_shell}  # type: ignore
+        crit: Dict[str, Any] = dict()  # type: ignore
 
         d = {
             "perturbation_energy": [min_perturbation_energy, max_perturbation_energy],
             "energy_difference": [min_energy_difference, max_energy_difference],
             "fock_element": [min_fock_element, max_fock_element],
         }
 
-        if electron_type is None or not open_shell:
+        if electron_type_interaction is None:
             prefix = "nbo_interactions."
         else:
             try:
-                if electron_type.lower() == "alpha":
+                if electron_type_interaction.lower() == "alpha":
                     prefix = "alpha_interactions."
-                elif electron_type.lower() == "beta":
+                elif electron_type_interaction.lower() == "beta":
                     prefix = "beta_interactions."
                 else:
                     raise ValueError("electron_type must be 'alpha' or 'beta' (open-shell), or None (closed-shell)!")
             except AttributeError:
                 raise ValueError("electron_type must be 'alpha' or 'beta' (open-shell), or None (closed-shell)!")
 
         for entry in d:
```

### Comparing `emmet-api-0.51.9/emmet/api/routes/mpcules/orbitals/resources.py` & `emmet-api-0.52.0/emmet/api/routes/molecules/orbitals/resources.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from maggma.api.resource import ReadOnlyResource
 from emmet.core.molecules.orbitals import OrbitalDoc
 
 from maggma.api.query_operator import PaginationQuery, SortQuery, SparseFieldsQuery
 
-from emmet.api.routes.mpcules.orbitals.query_operators import (
+from emmet.api.routes.molecules.orbitals.query_operators import (
     NBOPopulationQuery,
     NBOLonePairQuery,
     NBOBondQuery,
     NBOInteractionQuery,
 )
-from emmet.api.routes.mpcules.molecules.query_operators import (
+from emmet.api.routes.molecules.molecules.query_operators import (
     MultiMPculeIDQuery,
     ExactCalcMethodQuery,
     FormulaQuery,
     ChemsysQuery,
     ElementsQuery,
     ChargeSpinQuery
 )
-from emmet.api.routes.mpcules.utils import MultiPropertyIDQuery
+from emmet.api.routes.molecules.utils import MultiPropertyIDQuery
 from emmet.api.core.settings import MAPISettings
 from emmet.api.core.global_header import GlobalHeaderProcessor
 
 
 def orbitals_resource(orbital_store):
     resource = ReadOnlyResource(
         orbital_store,
@@ -39,14 +39,14 @@
             NBOBondQuery(),
             NBOInteractionQuery(),
             SortQuery(),
             PaginationQuery(),
             SparseFieldsQuery(OrbitalDoc, default_fields=["molecule_id", "property_id", "solvent", "last_updated"],),
         ],
         header_processor=GlobalHeaderProcessor(),
-        tags=["MPcules Orbitals"],
+        tags=["Molecules Orbitals"],
         sub_path="/orbitals/",
         disable_validation=True,
         timeout=MAPISettings().TIMEOUT,
     )
 
     return resource
```

### Comparing `emmet-api-0.51.9/emmet/api/routes/mpcules/partial_charges/resources.py` & `emmet-api-0.52.0/emmet/api/routes/molecules/partial_charges/resources.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from maggma.api.resource import ReadOnlyResource
 from emmet.core.molecules.atomic import PartialChargesDoc
 
 from maggma.api.query_operator import PaginationQuery, SortQuery, SparseFieldsQuery
 
-from emmet.api.routes.mpcules.molecules.query_operators import (
+from emmet.api.routes.molecules.molecules.query_operators import (
     MultiMPculeIDQuery,
     ExactCalcMethodQuery,
     FormulaQuery,
     ChemsysQuery,
     ElementsQuery,
     ChargeSpinQuery
 )
-from emmet.api.routes.mpcules.utils import MethodQuery, MultiPropertyIDQuery
+from emmet.api.routes.molecules.utils import MethodQuery, MultiPropertyIDQuery
 from emmet.api.core.settings import MAPISettings
 from emmet.api.core.global_header import GlobalHeaderProcessor
 
 
 def charges_resource(charges_store):
     resource = ReadOnlyResource(
         charges_store,
@@ -39,14 +39,14 @@
                     "solvent",
                     "method",
                     "last_updated"
                 ],
             ),
         ],
         header_processor=GlobalHeaderProcessor(),
-        tags=["MPcules Partial Charges"],
+        tags=["Molecules Partial Charges"],
         sub_path="/partial_charges/",
         disable_validation=True,
         timeout=MAPISettings().TIMEOUT,
     )
 
     return resource
```

### Comparing `emmet-api-0.51.9/emmet/api/routes/mpcules/partial_spins/resources.py` & `emmet-api-0.52.0/emmet/api/routes/molecules/partial_spins/resources.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from maggma.api.resource import ReadOnlyResource
 from emmet.core.molecules.atomic import PartialSpinsDoc
 
 from maggma.api.query_operator import PaginationQuery, SortQuery, SparseFieldsQuery
 
-from emmet.api.routes.mpcules.molecules.query_operators import (
+from emmet.api.routes.molecules.molecules.query_operators import (
     MultiMPculeIDQuery,
     ExactCalcMethodQuery,
     FormulaQuery,
     ChemsysQuery,
     ElementsQuery,
     ChargeSpinQuery
 )
-from emmet.api.routes.mpcules.utils import MethodQuery, MultiPropertyIDQuery
+from emmet.api.routes.molecules.utils import MethodQuery, MultiPropertyIDQuery
 from emmet.api.core.settings import MAPISettings
 from emmet.api.core.global_header import GlobalHeaderProcessor
 
 
 def spins_resource(spins_store):
     resource = ReadOnlyResource(
         spins_store,
@@ -39,14 +39,14 @@
                     "solvent",
                     "method",
                     "last_updated"
                 ],
             ),
         ],
         header_processor=GlobalHeaderProcessor(),
-        tags=["MPcules Partial Spins"],
+        tags=["Molecules Partial Spins"],
         sub_path="/partial_spins/",
         disable_validation=True,
         timeout=MAPISettings().TIMEOUT,
     )
 
     return resource
```

### Comparing `emmet-api-0.51.9/emmet/api/routes/mpcules/redox/query_operators.py` & `emmet-api-0.52.0/emmet/api/routes/molecules/redox/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/emmet/api/routes/mpcules/redox/resources.py` & `emmet-api-0.52.0/emmet/api/routes/molecules/vibrations/resources.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,42 @@
 from maggma.api.resource import ReadOnlyResource
-from emmet.core.molecules.redox import RedoxDoc
+from emmet.core.molecules.vibration import VibrationDoc
 
-from maggma.api.query_operator import (
-    NumericQuery,
-    PaginationQuery,
-    SortQuery,
-    SparseFieldsQuery
-)
+from maggma.api.query_operator import PaginationQuery, SortQuery, SparseFieldsQuery
 
-from emmet.api.routes.mpcules.redox.query_operators import (
-    RedoxPotentialQuery
-)
-from emmet.api.routes.mpcules.molecules.query_operators import (
+from emmet.api.routes.molecules.molecules.query_operators import (
     MultiMPculeIDQuery,
     ExactCalcMethodQuery,
     FormulaQuery,
     ChemsysQuery,
     ElementsQuery,
     ChargeSpinQuery
 )
-from emmet.api.routes.mpcules.utils import MultiPropertyIDQuery
+from emmet.api.routes.molecules.utils import MultiPropertyIDQuery
 from emmet.api.core.settings import MAPISettings
 from emmet.api.core.global_header import GlobalHeaderProcessor
 
 
-def redox_resource(redox_store):
+def vibration_resource(vibes_store):
     resource = ReadOnlyResource(
-        redox_store,
-        RedoxDoc,
+        vibes_store,
+        VibrationDoc,
         query_operators=[
             MultiMPculeIDQuery(),
             ExactCalcMethodQuery(),
             FormulaQuery(),
             ChemsysQuery(),
             ElementsQuery(),
             ChargeSpinQuery(),
             MultiPropertyIDQuery(),
-            RedoxPotentialQuery(),
-            NumericQuery(model=RedoxDoc),
             SortQuery(),
             PaginationQuery(),
-            SparseFieldsQuery(RedoxDoc, default_fields=["molecule_id", "property_id", "solvent", "last_updated"],),
+            SparseFieldsQuery(VibrationDoc, default_fields=["molecule_id", "property_id", "solvent", "last_updated"],),
         ],
         header_processor=GlobalHeaderProcessor(),
-        tags=["MPcules Redox"],
-        sub_path="/redox/",
+        tags=["Molecules Vibrations"],
+        sub_path="/vibrations/",
         disable_validation=True,
         timeout=MAPISettings().TIMEOUT,
     )
 
     return resource
```

### Comparing `emmet-api-0.51.9/emmet/api/routes/mpcules/summary/hint_scheme.py` & `emmet-api-0.52.0/emmet/api/routes/molecules/summary/hint_scheme.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from maggma.api.resource import HintScheme
 
 
 class SummaryHintScheme(HintScheme):
     """
-    Hint scheme for the mpcules summary endpoint.
+    Hint scheme for the molecules/summary endpoint.
     """
 
     def generate_hints(self, query):
 
         for param in query["criteria"]:
 
             if "composition" in param:
```

### Comparing `emmet-api-0.51.9/emmet/api/routes/mpcules/summary/query_operators.py` & `emmet-api-0.52.0/emmet/api/routes/molecules/summary/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/emmet/api/routes/mpcules/summary/resources.py` & `emmet-api-0.52.0/emmet/api/routes/molecules/summary/resources.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 from maggma.api.query_operator import (
     PaginationQuery,
     SortQuery,
     SparseFieldsQuery,
     NumericQuery,
 )
 from maggma.api.resource import ReadOnlyResource
-from emmet.api.routes.mpcules.molecules.query_operators import (
+from emmet.api.routes.molecules.molecules.query_operators import (
     FormulaQuery,
     ChemsysQuery,
     ElementsQuery,
     ChargeSpinQuery,
     DeprecationQuery,
 )
-from emmet.api.routes.summary.query_operators import HasPropsQuery
-from emmet.api.routes.mpcules.summary.hint_scheme import SummaryHintScheme
-from emmet.api.routes.mpcules.summary.query_operators import MPculeIDsSearchQuery
+from emmet.api.routes.materials.summary.query_operators import HasPropsQuery
+from emmet.api.routes.molecules.summary.hint_scheme import SummaryHintScheme
+from emmet.api.routes.molecules.summary.query_operators import MPculeIDsSearchQuery
 from emmet.api.core.global_header import GlobalHeaderProcessor
 from emmet.api.core.settings import MAPISettings
 
 timeout = MAPISettings().TIMEOUT
 
 
 def summary_resource(summary_store):
@@ -28,23 +28,32 @@
         summary_store,
         MoleculeSummaryDoc,
         query_operators=[
             MPculeIDsSearchQuery(),
             FormulaQuery(),
             ChemsysQuery(),
             ElementsQuery(),
-            NumericQuery(model=MoleculeSummaryDoc, excluded_fields=["composition"]),
             HasPropsQuery(),
             ChargeSpinQuery(),
             DeprecationQuery(),
             SortQuery(),
             PaginationQuery(),
+            NumericQuery(
+                model=MoleculeSummaryDoc,
+                fields=[
+                    "nelements",
+                    "ionization_energy",
+                    "electron_affinity",
+                    "reduction_free_energy",
+                    "oxidation_free_energy"
+                ]
+            ),
             SparseFieldsQuery(MoleculeSummaryDoc, default_fields=["molecule_id"]),
         ],
         hint_scheme=SummaryHintScheme(),
         header_processor=GlobalHeaderProcessor(),
-        tags=["MPcules Summary"],
+        tags=["Molecules Summary"],
         disable_validation=True,
         timeout=timeout
     )
 
     return resource
```

### Comparing `emmet-api-0.51.9/emmet/api/routes/mpcules/tasks/query_operators.py` & `emmet-api-0.52.0/emmet/api/routes/molecules/tasks/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/emmet/api/routes/mpcules/tasks/resources.py` & `emmet-api-0.52.0/emmet/api/routes/molecules/tasks/resources.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from maggma.api.query_operator import PaginationQuery, SortQuery, SparseFieldsQuery
 from maggma.api.resource import ReadOnlyResource
 
-from emmet.api.routes.mpcules.molecules.query_operators import (
+from emmet.api.routes.molecules.molecules.query_operators import (
     ChemsysQuery,
     ElementsQuery,
     FormulaQuery,
 )
-from emmet.api.routes.mpcules.tasks.hint_scheme import TasksHintScheme
-from emmet.api.routes.mpcules.tasks.query_operators import (
+from emmet.api.routes.molecules.tasks.hint_scheme import TasksHintScheme
+from emmet.api.routes.molecules.tasks.query_operators import (
     DeprecationQuery,
     MultipleTaskIDsQuery,
     # TODO:
     # TrajectoryQuery,
     # EntryQuery,
 )
 from emmet.api.core.global_header import GlobalHeaderProcessor
@@ -36,29 +36,29 @@
             SparseFieldsQuery(
                 TaskDocument,
                 default_fields=["task_id", "formula_alphabetical", "last_updated"],
             ),
         ],
         header_processor=GlobalHeaderProcessor(),
         hint_scheme=TasksHintScheme(),
-        tags=["MPcules Tasks"],
+        tags=["Molecules Tasks"],
         sub_path="/tasks/",
         timeout=timeout,
         disable_validation=True,
     )
 
     return resource
 
 
 def task_deprecation_resource(task_store):
     resource = ReadOnlyResource(
         task_store,
         DeprecationDoc,
         query_operators=[DeprecationQuery(), PaginationQuery()],
-        tags=["MPcules Tasks"],
+        tags=["Molecules Tasks"],
         enable_get_by_key=False,
         enable_default_search=True,
         sub_path="/tasks/deprecation/",
         header_processor=GlobalHeaderProcessor(),
         timeout=timeout,
     )
```

### Comparing `emmet-api-0.51.9/emmet/api/routes/mpcules/thermo/query_operators.py` & `emmet-api-0.52.0/emmet/api/routes/molecules/thermo/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/emmet/api/routes/mpcules/thermo/resources.py` & `emmet-api-0.52.0/emmet/api/routes/molecules/thermo/resources.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 from maggma.api.query_operator import (
     NumericQuery,
     PaginationQuery,
     SortQuery,
     SparseFieldsQuery
 )
 
-from emmet.api.routes.mpcules.thermo.query_operators import (
+from emmet.api.routes.molecules.thermo.query_operators import (
     ThermoCorrectionQuery,
 )
-from emmet.api.routes.mpcules.molecules.query_operators import (
+from emmet.api.routes.molecules.molecules.query_operators import (
     MultiMPculeIDQuery,
     ExactCalcMethodQuery,
     FormulaQuery,
     ChemsysQuery,
     ElementsQuery,
     ChargeSpinQuery
 )
-from emmet.api.routes.mpcules.utils import MultiPropertyIDQuery
+from emmet.api.routes.molecules.utils import MultiPropertyIDQuery
 from emmet.api.core.settings import MAPISettings
 from emmet.api.core.global_header import GlobalHeaderProcessor
 
 
 def thermo_resource(thermo_store):
     resource = ReadOnlyResource(
         thermo_store,
@@ -33,29 +33,39 @@
             ExactCalcMethodQuery(),
             FormulaQuery(),
             ChemsysQuery(),
             ElementsQuery(),
             ChargeSpinQuery(),
             MultiPropertyIDQuery(),
             ThermoCorrectionQuery(),
-            NumericQuery(model=MoleculeThermoDoc),
+            NumericQuery(
+                model=MoleculeThermoDoc,
+                excluded_fields=[
+                    "charge",
+                    "spin_multiplicity",
+                    "natoms",
+                    "nelements",
+                    "nelectrons",
+                    "rt"
+                ]
+            ),
             SortQuery(),
             PaginationQuery(),
             SparseFieldsQuery(
                 MoleculeThermoDoc,
                 default_fields=[
                     "molecule_id",
                     "property_id",
                     "solvent",
                     "method",
                     "last_updated"
                 ],
             ),
         ],
         header_processor=GlobalHeaderProcessor(),
-        tags=["MPcules Thermo"],
+        tags=["Molecules Thermo"],
         sub_path="/thermo/",
         disable_validation=True,
         timeout=MAPISettings().TIMEOUT,
     )
 
     return resource
```

### Comparing `emmet-api-0.51.9/emmet/api/routes/mpcules/utils.py` & `emmet-api-0.52.0/emmet/api/routes/molecules/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/emmet/api/routes/oxidation_states/query_operators.py` & `emmet-api-0.52.0/emmet/api/routes/materials/oxidation_states/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/emmet/api/routes/oxidation_states/resources.py` & `emmet-api-0.52.0/emmet/api/routes/materials/oxidation_states/resources.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 from maggma.api.query_operator import (
     PaginationQuery,
     SortQuery,
     SparseFieldsQuery,
 )
 
-from emmet.api.routes.materials.query_operators import FormulaQuery, ChemsysQuery, MultiMaterialIDQuery
-from emmet.api.routes.oxidation_states.query_operators import PossibleOxiStateQuery
+from emmet.api.routes.materials.materials.query_operators import FormulaQuery, ChemsysQuery, MultiMaterialIDQuery
+from emmet.api.routes.materials.oxidation_states.query_operators import PossibleOxiStateQuery
 from emmet.api.core.global_header import GlobalHeaderProcessor
 from emmet.api.core.settings import MAPISettings
 
 
 def oxi_states_resource(oxi_states_store):
     resource = ReadOnlyResource(
         oxi_states_store,
@@ -23,13 +23,14 @@
             ChemsysQuery(),
             PossibleOxiStateQuery(),
             SortQuery(),
             PaginationQuery(),
             SparseFieldsQuery(OxidationStateDoc, default_fields=["material_id", "last_updated"]),
         ],
         header_processor=GlobalHeaderProcessor(),
-        tags=["Oxidation States"],
+        tags=["Materials Oxidation States"],
+        sub_path="/oxidation_states/",
         disable_validation=True,
         timeout=MAPISettings().TIMEOUT,
     )
 
     return resource
```

### Comparing `emmet-api-0.51.9/emmet/api/routes/phonon/query_operators.py` & `emmet-api-0.52.0/emmet/api/routes/materials/phonon/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/emmet/api/routes/phonon/resources.py` & `emmet-api-0.52.0/emmet/api/routes/materials/phonon/resources.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,14 +13,15 @@
         query_operators=[
             PaginationQuery(),
             SparseFieldsQuery(
                 PhononBSDOSDoc, default_fields=["task_id", "last_updated"]
             ),
         ],
         header_processor=GlobalHeaderProcessor(),
-        tags=["Phonon"],
+        tags=["Materials Phonon"],
+        sub_path="/phonon/",
         enable_default_search=False,
         disable_validation=True,
         timeout=MAPISettings().TIMEOUT
     )
 
     return resource
```

### Comparing `emmet-api-0.51.9/emmet/api/routes/piezo/query_operators.py` & `emmet-api-0.52.0/emmet/api/routes/materials/piezo/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/emmet/api/routes/piezo/resources.py` & `emmet-api-0.52.0/emmet/api/routes/materials/piezo/resources.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from maggma.api.resource import ReadOnlyResource
 from emmet.core.polar import PiezoelectricDoc
 
 from maggma.api.query_operator import PaginationQuery, SortQuery, SparseFieldsQuery
-from emmet.api.routes.piezo.query_operators import PiezoelectricQuery
-from emmet.api.routes.materials.query_operators import MultiMaterialIDQuery
+from emmet.api.routes.materials.piezo.query_operators import PiezoelectricQuery
+from emmet.api.routes.materials.materials.query_operators import MultiMaterialIDQuery
 from emmet.api.core.global_header import GlobalHeaderProcessor
 from emmet.api.core.settings import MAPISettings
 
 
 def piezo_resource(piezo_store):
     resource = ReadOnlyResource(
         piezo_store,
@@ -16,13 +16,14 @@
             MultiMaterialIDQuery(),
             PiezoelectricQuery(),
             SortQuery(),
             PaginationQuery(),
             SparseFieldsQuery(PiezoelectricDoc, default_fields=["material_id", "last_updated"]),
         ],
         header_processor=GlobalHeaderProcessor(),
-        tags=["Piezoelectric"],
+        tags=["Materials Piezoelectric"],
+        sub_path="/piezoelectric/",
         disable_validation=True,
         timeout=MAPISettings().TIMEOUT,
     )
 
     return resource
```

### Comparing `emmet-api-0.51.9/emmet/api/routes/provenance/resources.py` & `emmet-api-0.52.0/emmet/api/routes/materials/provenance/resources.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from maggma.api.resource import ReadOnlyResource
 from maggma.api.query_operator import PaginationQuery, SparseFieldsQuery
-from emmet.api.routes.materials.query_operators import DeprecationQuery, MultiMaterialIDQuery
+from emmet.api.routes.materials.materials.query_operators import DeprecationQuery, MultiMaterialIDQuery
 from emmet.api.core.global_header import GlobalHeaderProcessor
 from emmet.core.provenance import ProvenanceDoc
 from emmet.api.core.settings import MAPISettings
 
 
 def provenance_resource(provenance_store):
     resource = ReadOnlyResource(
@@ -13,13 +13,14 @@
         query_operators=[
             MultiMaterialIDQuery(),
             DeprecationQuery(),
             PaginationQuery(),
             SparseFieldsQuery(ProvenanceDoc, default_fields=["material_id", "last_updated"]),
         ],
         header_processor=GlobalHeaderProcessor(),
-        tags=["Provenance"],
+        tags=["Materials Provenance"],
+        sub_path="/provenance/",
         disable_validation=True,
         timeout=MAPISettings().TIMEOUT,
     )
 
     return resource
```

### Comparing `emmet-api-0.51.9/emmet/api/routes/robocrys/query_operators.py` & `emmet-api-0.52.0/emmet/api/routes/materials/robocrys/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/emmet/api/routes/robocrys/resources.py` & `emmet-api-0.52.0/emmet/api/routes/materials/robocrys/resources.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from maggma.api.resource import ReadOnlyResource
 from maggma.api.resource.aggregation import AggregationResource
 from maggma.api.query_operator import PaginationQuery, SparseFieldsQuery
 
-from emmet.api.routes.robocrys.query_operators import RoboTextSearchQuery
-from emmet.api.routes.materials.query_operators import MultiMaterialIDQuery
+from emmet.api.routes.materials.robocrys.query_operators import RoboTextSearchQuery
+from emmet.api.routes.materials.materials.query_operators import MultiMaterialIDQuery
 from emmet.core.robocrys import RobocrystallogapherDoc
 from emmet.api.core.global_header import GlobalHeaderProcessor
 from emmet.api.core.settings import MAPISettings
 
 timeout = MAPISettings().TIMEOUT
 
 
@@ -20,26 +20,27 @@
             PaginationQuery(),
             SparseFieldsQuery(
                 RobocrystallogapherDoc, default_fields=["material_id", "last_updated"]
             ),
         ],
         header_processor=GlobalHeaderProcessor(),
         tags=["Robocrystallographer"],
+        sub_path="/robocrys/",
         disable_validation=True,
         timeout=timeout,
     )
 
     return resource
 
 
 def robo_search_resource(robo_store):
     resource = AggregationResource(
         robo_store,
         RobocrystallogapherDoc,
         pipeline_query_operator=RoboTextSearchQuery(),
         tags=["Robocrystallographer"],
-        sub_path="/text_search/",
+        sub_path="/robocrys/text_search/",
         header_processor=GlobalHeaderProcessor(),
         timeout=timeout,
     )
 
     return resource
```

### Comparing `emmet-api-0.51.9/emmet/api/routes/similarity/resources.py` & `emmet-api-0.52.0/emmet/api/routes/materials/similarity/resources.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
         similarity_store,
         SimilarityDoc,
         query_operators=[
             PaginationQuery(),
             SparseFieldsQuery(SimilarityDoc, default_fields=["material_id"]),
         ],
         header_processor=GlobalHeaderProcessor(),
-        tags=["Similarity"],
+        tags=["Materials Similarity"],
+        sub_path="/similarity/",
         enable_default_search=False,
         disable_validation=True,
         timeout=MAPISettings().TIMEOUT
     )
 
     return resource
```

### Comparing `emmet-api-0.51.9/emmet/api/routes/substrates/query_operators.py` & `emmet-api-0.52.0/emmet/api/routes/materials/substrates/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/emmet/api/routes/substrates/resources.py` & `emmet-api-0.52.0/emmet/api/routes/materials/substrates/resources.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     PaginationQuery,
     SortQuery,
     SparseFieldsQuery,
     StringQueryOperator,
 )
 from maggma.api.resource import ReadOnlyResource
 
-from emmet.api.routes.substrates.query_operators import SubstrateStructureQuery
+from emmet.api.routes.materials.substrates.query_operators import SubstrateStructureQuery
 from emmet.api.core.global_header import GlobalHeaderProcessor
 from emmet.core.substrates import SubstratesDoc
 from emmet.api.core.settings import MAPISettings
 
 
 def substrates_resource(substrates_store):
     resource = ReadOnlyResource(
@@ -24,14 +24,15 @@
                 model=SubstratesDoc, excluded_fields=["film_orient", "orient"]
             ),
             SortQuery(),
             PaginationQuery(),
             SparseFieldsQuery(SubstratesDoc, default_fields=["film_id", "sub_id"]),
         ],
         header_processor=GlobalHeaderProcessor(),
-        tags=["Substrates"],
+        tags=["Materials Substrates"],
+        sub_path="/substrates/",
         enable_get_by_key=False,
         disable_validation=True,
         timeout=MAPISettings().TIMEOUT
     )
 
     return resource
```

### Comparing `emmet-api-0.51.9/emmet/api/routes/summary/hint_scheme.py` & `emmet-api-0.52.0/emmet/api/routes/materials/summary/hint_scheme.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/emmet/api/routes/summary/query_operators.py` & `emmet-api-0.52.0/emmet/api/routes/materials/summary/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/emmet/api/routes/summary/resources.py` & `emmet-api-0.52.0/emmet/api/routes/materials/summary/resources.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 from maggma.api.query_operator import (
     PaginationQuery,
     SortQuery,
     SparseFieldsQuery,
     NumericQuery,
 )
 from maggma.api.resource import ReadOnlyResource, AggregationResource
-from emmet.api.routes.materials.query_operators import (
+from emmet.api.routes.materials.materials.query_operators import (
     DeprecationQuery,
     ElementsQuery,
     FormulaQuery,
     ChemsysQuery,
     SymmetryQuery,
 )
-from emmet.api.routes.oxidation_states.query_operators import PossibleOxiStateQuery
+from emmet.api.routes.materials.oxidation_states.query_operators import PossibleOxiStateQuery
 from emmet.core.summary import SummaryStats
-from emmet.api.routes.summary.hint_scheme import SummaryHintScheme
-from emmet.api.routes.summary.query_operators import (
+from emmet.api.routes.materials.summary.hint_scheme import SummaryHintScheme
+from emmet.api.routes.materials.summary.query_operators import (
     HasPropsQuery,
     MaterialIDsSearchQuery,
     SearchIsStableQuery,
     SearchIsTheoreticalQuery,
     SearchMagneticQuery,
     SearchHasReconstructedQuery,
     SearchStatsQuery,
@@ -55,27 +55,28 @@
             DeprecationQuery(),
             SortQuery(),
             PaginationQuery(),
             SparseFieldsQuery(SummaryDoc, default_fields=["material_id"]),
         ],
         hint_scheme=SummaryHintScheme(),
         header_processor=GlobalHeaderProcessor(),
-        tags=["Summary"],
+        tags=["Materials Summary"],
+        sub_path="/summary/",
         disable_validation=True,
         timeout=timeout
     )
 
     return resource
 
 
 def summary_stats_resource(summary_store):
     resource = AggregationResource(
         summary_store,
         SummaryStats,
         pipeline_query_operator=SearchStatsQuery(SummaryDoc),
-        tags=["Summary"],
-        sub_path="/stats/",
+        tags=["Materials Summary"],
+        sub_path="/summary/stats/",
         header_processor=GlobalHeaderProcessor(),
         timeout=timeout
     )
 
     return resource
```

### Comparing `emmet-api-0.51.9/emmet/api/routes/surface_properties/query_operators.py` & `emmet-api-0.52.0/emmet/api/routes/materials/surface_properties/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/emmet/api/routes/synthesis/data_adaptor.py` & `emmet-api-0.52.0/emmet/api/routes/materials/synthesis/data_adaptor.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/emmet/api/routes/synthesis/data_adaptor_synpro.py` & `emmet-api-0.52.0/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/emmet/api/routes/synthesis/query_operators.py` & `emmet-api-0.52.0/emmet/api/routes/materials/synthesis/query_operators.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Optional, List, Dict, Union, Any
 from fastapi import Query
 from pymatgen.core import Composition
 from maggma.api.query_operator import QueryOperator
 from emmet.core.synthesis import SynthesisTypeEnum, OperationTypeEnum
-from emmet.api.routes.synthesis.utils import mask_highlights, mask_paragraphs
+from emmet.api.routes.materials.synthesis.utils import mask_highlights, mask_paragraphs
 
 
 class SynthesisSearchQuery(QueryOperator):
     """
     Method to generate a synthesis text search query
     """
```

### Comparing `emmet-api-0.51.9/emmet/api/routes/synthesis/resources.py` & `emmet-api-0.52.0/emmet/api/routes/materials/synthesis/resources.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from maggma.api.resource import AggregationResource
 from emmet.api.core.settings import MAPISettings
-from emmet.api.routes.synthesis.query_operators import SynthesisSearchQuery
+from emmet.api.routes.materials.synthesis.query_operators import SynthesisSearchQuery
 from emmet.api.core.global_header import GlobalHeaderProcessor
 from emmet.core.synthesis.core import SynthesisSearchResultModel
 
 synth_indexes = [
     ("synthesis_type", False),
     ("targets_formula_s", False),
     ("precursors_formula_s", False),
@@ -18,14 +18,15 @@
 
 
 def synth_resource(synth_store):
 
     resource = AggregationResource(
         synth_store,
         SynthesisSearchResultModel,
-        tags=["Synthesis"],
+        tags=["Materials Synthesis"],
+        sub_path="/synthesis/",
         pipeline_query_operator=SynthesisSearchQuery(),
         header_processor=GlobalHeaderProcessor(),
         timeout=MAPISettings().TIMEOUT
     )
 
     return resource
```

### Comparing `emmet-api-0.51.9/emmet/api/routes/synthesis/utils.py` & `emmet-api-0.52.0/emmet/api/routes/materials/synthesis/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/emmet/api/routes/tasks/hint_scheme.py` & `emmet-api-0.52.0/emmet/api/routes/materials/tasks/hint_scheme.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/emmet/api/routes/tasks/query_operators.py` & `emmet-api-0.52.0/emmet/api/routes/materials/tasks/query_operators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from maggma.api.query_operator import QueryOperator
 from maggma.api.utils import STORE_PARAMS
-from emmet.api.routes.tasks.utils import calcs_reversed_to_trajectory, task_to_entry
+from emmet.api.routes.materials.tasks.utils import calcs_reversed_to_trajectory, task_to_entry
 from fastapi import Query
 from typing import Optional
 from monty.json import jsanitize
 
 
 class MultipleTaskIDsQuery(QueryOperator):
     """
```

### Comparing `emmet-api-0.51.9/emmet/api/routes/tasks/resources.py` & `emmet-api-0.52.0/emmet/api/routes/materials/tasks/resources.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from maggma.api.query_operator import PaginationQuery, SortQuery, SparseFieldsQuery
 from maggma.api.resource import ReadOnlyResource
 
-from emmet.api.routes.materials.query_operators import (
+from emmet.api.routes.materials.materials.query_operators import (
     ChemsysQuery,
     ElementsQuery,
     FormulaQuery,
 )
-from emmet.api.routes.tasks.hint_scheme import TasksHintScheme
-from emmet.api.routes.tasks.query_operators import (
+from emmet.api.routes.materials.tasks.hint_scheme import TasksHintScheme
+from emmet.api.routes.materials.tasks.query_operators import (
     DeprecationQuery,
     MultipleTaskIDsQuery,
     TrajectoryQuery,
     EntryQuery,
 )
 from emmet.api.core.global_header import GlobalHeaderProcessor
 from emmet.api.core.settings import MAPISettings
@@ -34,46 +34,47 @@
             SparseFieldsQuery(
                 TaskDoc,
                 default_fields=["task_id", "formula_pretty", "last_updated"],
             ),
         ],
         header_processor=GlobalHeaderProcessor(),
         hint_scheme=TasksHintScheme(),
-        tags=["Tasks"],
+        tags=["Materials Tasks"],
+        sub_path="/tasks/",
         timeout=timeout,
         disable_validation=True,
     )
 
     return resource
 
 
 def task_deprecation_resource(materials_store):
     resource = ReadOnlyResource(
         materials_store,
         DeprecationDoc,
         query_operators=[DeprecationQuery(), PaginationQuery()],
-        tags=["Tasks"],
+        tags=["Materials Tasks"],
         enable_get_by_key=False,
         enable_default_search=True,
-        sub_path="/deprecation/",
+        sub_path="/tasks/deprecation/",
         header_processor=GlobalHeaderProcessor(),
         timeout=timeout,
     )
 
     return resource
 
 
 def trajectory_resource(task_store):
     resource = ReadOnlyResource(
         task_store,
         TrajectoryDoc,
         query_operators=[TrajectoryQuery(), PaginationQuery()],
         key_fields=["task_id", "calcs_reversed"],
-        tags=["Tasks"],
-        sub_path="/trajectory/",
+        tags=["Materials Tasks"],
+        sub_path="/tasks/trajectory/",
         header_processor=GlobalHeaderProcessor(),
         timeout=timeout,
         disable_validation=True,
     )
 
     return resource
 
@@ -88,15 +89,15 @@
             "input",
             "output",
             "run_type",
             "task_type",
             "completed_at",
             "last_updated",
         ],
-        tags=["Tasks"],
-        sub_path="/entries/",
+        tags=["Materials Tasks"],
+        sub_path="/tasks/entries/",
         header_processor=GlobalHeaderProcessor(),
         timeout=timeout,
         disable_validation=True,
     )
 
     return resource
```

### Comparing `emmet-api-0.51.9/emmet/api/routes/tasks/utils.py` & `emmet-api-0.52.0/emmet/api/routes/materials/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/emmet/api/routes/thermo/query_operators.py` & `emmet-api-0.52.0/emmet/api/routes/materials/thermo/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/emmet/api/routes/thermo/resources.py` & `emmet-api-0.52.0/emmet/api/routes/materials/thermo/resources.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,34 +4,34 @@
 from emmet.core.thermo import PhaseDiagramDoc
 
 from maggma.api.query_operator import (
     PaginationQuery,
     SortQuery,
     SparseFieldsQuery,
 )
-from emmet.api.routes.thermo.query_operators import (
+from emmet.api.routes.materials.thermo.query_operators import (
     IsStableQuery,
     MultiThermoIDQuery,
     MultiThermoTypeQuery,
 )
 from emmet.api.core.global_header import GlobalHeaderProcessor
-from emmet.api.routes.materials.query_operators import (
+from emmet.api.routes.materials.materials.query_operators import (
     MultiMaterialIDQuery,
     FormulaQuery,
     ChemsysQuery,
 )
 from emmet.api.core.settings import MAPISettings
 
 
 def phase_diagram_resource(phase_diagram_store):
     resource = ReadOnlyResource(
         phase_diagram_store,
         PhaseDiagramDoc,
-        tags=["Thermo"],
-        sub_path="/phase_diagram/",
+        tags=["Materials Thermo"],
+        sub_path="/thermo/phase_diagram/",
         disable_validation=True,
         enable_default_search=False,
         header_processor=GlobalHeaderProcessor(),
         query_disk_use=False,
     )
 
     return resource
@@ -52,13 +52,14 @@
             SortQuery(),
             PaginationQuery(),
             SparseFieldsQuery(
                 ThermoDoc, default_fields=["thermo_id", "material_id", "last_updated"]
             ),
         ],
         header_processor=GlobalHeaderProcessor(),
-        tags=["Thermo"],
+        tags=["Materials Thermo"],
+        sub_path="/thermo/",
         disable_validation=True,
         timeout=MAPISettings().TIMEOUT,
     )
 
     return resource
```

### Comparing `emmet-api-0.51.9/emmet/api/routes/xas/query_operators.py` & `emmet-api-0.52.0/emmet/api/routes/materials/xas/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/material_resources.py` & `emmet-api-0.52.0/material_resources.py`

 * *Files 14% similar despite different names*

```diff
@@ -94,16 +94,14 @@
 
     synth_store = MongoURIStore(uri=db_uri, database="mp_core", key="_id", collection_name="synth_descriptions")
 
     insertion_electrodes_store = MongoURIStore(
         uri=db_uri, database=f"mp_core_{db_suffix}", key="battery_id", collection_name="insertion_electrodes"
     )
 
-    molecules_store = MongoURIStore(uri=db_uri, database="mp_core", key="task_id", collection_name="molecules")
-
     oxi_states_store = MongoURIStore(
         uri=db_uri, database=f"mp_core_{db_suffix}", key="material_id", collection_name="oxi_states"
     )
 
     provenance_store = MongoURIStore(
         uri=db_uri, database=f"mp_core_{db_suffix}", key="material_id", collection_name="provenance"
     )
@@ -169,208 +167,201 @@
     general_store = MongoURIStore(
         uri=db_uri, database="mp_consumers", key="submission_id", collection_name="general_store"
     )
 else:
     raise RuntimeError("Must specify MongoDB URI containing inputs.")
 
 # Materials
-from emmet.api.routes.materials.resources import (
+from emmet.api.routes.materials.materials.resources import (
     find_structure_resource,
     formula_autocomplete_resource,
     materials_resource,
 )
 
-resources.update(
-    {
-        "materials": [
-            find_structure_resource(materials_store),
-            formula_autocomplete_resource(formula_autocomplete_store),
-            materials_resource(materials_store),
-        ]
-    }
+materials_resources = list()
+
+materials_resources.extend(
+    [
+        find_structure_resource(materials_store),
+        formula_autocomplete_resource(formula_autocomplete_store),
+        materials_resource(materials_store),
+    ]
 )
 
 # Absorption
-from emmet.api.routes.absorption.resources import absorption_resource
+from emmet.api.routes.materials.absorption.resources import absorption_resource
 
-resources.update({"absorption": [absorption_resource(absorption_store)]})
+materials_resources.extend([absorption_resource(absorption_store)])
 
 # Bonds
-from emmet.api.routes.bonds.resources import bonds_resource
+from emmet.api.routes.materials.bonds.resources import bonds_resource
 
-resources.update({"bonds": [bonds_resource(bonds_store)]})
+materials_resources.extend([bonds_resource(bonds_store)])
 
 # Chemenv
-from emmet.api.routes.chemenv.resources import chemenv_resource
+from emmet.api.routes.materials.chemenv.resources import chemenv_resource
 
-resources.update({"chemenv": [chemenv_resource(chemenv_store)]})
+materials_resources.extend([chemenv_resource(chemenv_store)])
 
 # Tasks
-from emmet.api.routes.tasks.resources import (
+from emmet.api.routes.materials.tasks.resources import (
     entries_resource,
     task_deprecation_resource,
     task_resource,
     trajectory_resource,
 )
 
-resources.update(
-    {
-        "tasks": [
-            trajectory_resource(task_store),
-            entries_resource(task_store),
-            task_deprecation_resource(materials_store),
-            task_resource(task_store),
-        ]
-    }
+materials_resources.extend(
+    [
+        trajectory_resource(task_store),
+        entries_resource(task_store),
+        task_deprecation_resource(materials_store),
+        task_resource(task_store),
+    ]
 )
 
 # Thermo
-from emmet.api.routes.thermo.resources import phase_diagram_resource, thermo_resource
+from emmet.api.routes.materials.thermo.resources import phase_diagram_resource, thermo_resource
 
-resources.update({"thermo": [phase_diagram_resource(phase_diagram_store), thermo_resource(thermo_store)]})
+materials_resources.extend([phase_diagram_resource(phase_diagram_store), thermo_resource(thermo_store)])
 
 # Dielectric
-from emmet.api.routes.dielectric.resources import dielectric_resource
+from emmet.api.routes.materials.dielectric.resources import dielectric_resource
 
-resources.update({"dielectric": [dielectric_resource(dielectric_store)]})
+materials_resources.extend([dielectric_resource(dielectric_store)])
 
 # Piezoelectric
-from emmet.api.routes.piezo.resources import piezo_resource
+from emmet.api.routes.materials.piezo.resources import piezo_resource
 
-resources.update({"piezoelectric": [piezo_resource(piezoelectric_store)]})
+materials_resources.extend([piezo_resource(piezoelectric_store)])
 
 # Magnetism
-from emmet.api.routes.magnetism.resources import magnetism_resource
+from emmet.api.routes.materials.magnetism.resources import magnetism_resource
 
-resources.update({"magnetism": [magnetism_resource(magnetism_store)]})
+materials_resources.extend([magnetism_resource(magnetism_store)])
 
 # Phonon
-from emmet.api.routes.phonon.resources import phonon_bsdos_resource
+from emmet.api.routes.materials.phonon.resources import phonon_bsdos_resource
 
-resources.update({"phonon": [phonon_bsdos_resource(phonon_bs_store)]})
+materials_resources.extend([phonon_bsdos_resource(phonon_bs_store)])
 
 # EOS
-from emmet.api.routes.eos.resources import eos_resource
+from emmet.api.routes.materials.eos.resources import eos_resource
 
-resources.update({"eos": [eos_resource(eos_store)]})
+materials_resources.extend([eos_resource(eos_store)])
 
 # Similarity
-from emmet.api.routes.similarity.resources import similarity_resource
+from emmet.api.routes.materials.similarity.resources import similarity_resource
 
-resources.update({"similarity": [similarity_resource(similarity_store)]})
+materials_resources.extend([similarity_resource(similarity_store)])
 
 # XAS
-from emmet.api.routes.xas.resources import xas_resource
+from emmet.api.routes.materials.xas.resources import xas_resource
 
-resources.update({"xas": [xas_resource(xas_store)]})
+materials_resources.extend([xas_resource(xas_store)])
 
 # Grain Boundaries
-from emmet.api.routes.grain_boundary.resources import gb_resource
+from emmet.api.routes.materials.grain_boundary.resources import gb_resource
 
-resources.update({"grain_boundary": [gb_resource(gb_store)]})
+materials_resources.extend([gb_resource(gb_store)])
 
 # Fermi Surface
-from emmet.api.routes.fermi.resources import fermi_resource
+from emmet.api.routes.materials.fermi.resources import fermi_resource
 
-resources.update({"fermi": [fermi_resource(fermi_store)]})
+materials_resources.extend([fermi_resource(fermi_store)])
 
 # Elasticity
-from emmet.api.routes.elasticity.resources import elasticity_resource
+from emmet.api.routes.materials.elasticity.resources import elasticity_resource
 
-resources.update({"elasticity": [elasticity_resource(elasticity_store)]})
-
-# DOIs
-from emmet.api.routes.dois.resources import dois_resource
-
-resources.update({"doi": [dois_resource(doi_store)]})
+materials_resources.extend([elasticity_resource(elasticity_store)])
 
 # Substrates
-from emmet.api.routes.substrates.resources import substrates_resource
+from emmet.api.routes.materials.substrates.resources import substrates_resource
 
-resources.update({"substrates": [substrates_resource(substrates_store)]})
+materials_resources.extend([substrates_resource(substrates_store)])
 
 # Surface Properties
-from emmet.api.routes.surface_properties.resources import surface_props_resource
+from emmet.api.routes.materials.surface_properties.resources import surface_props_resource
 
-resources.update({"surface_properties": [surface_props_resource(surface_props_store)]})
+materials_resources.extend([surface_props_resource(surface_props_store)])
 
 
 # Robocrystallographer
-from emmet.api.routes.robocrys.resources import robo_resource, robo_search_resource
+from emmet.api.routes.materials.robocrys.resources import robo_resource, robo_search_resource
 
-resources.update({"robocrys": [robo_search_resource(robo_store), robo_resource(robo_store)]})
+materials_resources.extend([robo_search_resource(robo_store), robo_resource(robo_store)])
 
 # Synthesis
-from emmet.api.routes.synthesis.resources import synth_resource
+from emmet.api.routes.materials.synthesis.resources import synth_resource
 
-resources.update({"synthesis": [synth_resource(synth_store)]})
+materials_resources.extend([synth_resource(synth_store)])
 
 # Electrodes
-from emmet.api.routes.electrodes.resources import insertion_electrodes_resource
-
-resources.update({"insertion_electrodes": [insertion_electrodes_resource(insertion_electrodes_store)]})
+from emmet.api.routes.materials.electrodes.resources import insertion_electrodes_resource
 
-# Molecules
-from emmet.api.routes.molecules.resources import molecules_resource
-
-resources.update({"molecules": [molecules_resource(molecules_store)]})
+materials_resources.extend([insertion_electrodes_resource(insertion_electrodes_store)])
 
 # Oxidation States
-from emmet.api.routes.oxidation_states.resources import oxi_states_resource
+from emmet.api.routes.materials.oxidation_states.resources import oxi_states_resource
 
-resources.update({"oxidation_states": [oxi_states_resource(oxi_states_store)]})
+materials_resources.extend([oxi_states_resource(oxi_states_store)])
 
 # Alloys
-from emmet.api.routes.alloys.resources import alloy_pairs_resource
+from emmet.api.routes.materials.alloys.resources import alloy_pairs_resource
 
-resources.update({"alloys": [alloy_pairs_resource(alloy_pairs_store)]})
+materials_resources.extend([alloy_pairs_resource(alloy_pairs_store)])
 
 # Provenance
-from emmet.api.routes.provenance.resources import provenance_resource
+from emmet.api.routes.materials.provenance.resources import provenance_resource
 
-resources.update({"provenance": [provenance_resource(provenance_store)]})
+materials_resources.extend([provenance_resource(provenance_store)])
 
 # Charge Density
-from emmet.api.routes.charge_density.resources import charge_density_resource, charge_density_url_resource
+from emmet.api.routes.materials.charge_density.resources import charge_density_resource, charge_density_url_resource
 
-resources.update({"charge_density": [charge_density_resource(s3_chgcar), charge_density_url_resource(chgcar_url)]})
+materials_resources.extend([charge_density_resource(s3_chgcar), charge_density_url_resource(chgcar_url)])
 
 # Summary
-from emmet.api.routes.summary.resources import summary_resource, summary_stats_resource
+from emmet.api.routes.materials.summary.resources import summary_resource, summary_stats_resource
 
-resources.update({"summary": [summary_stats_resource(summary_store), summary_resource(summary_store)]})
+materials_resources.extend([summary_stats_resource(summary_store), summary_resource(summary_store)])
 
 # Electronic Structure
-from emmet.api.routes.electronic_structure.resources import (
+from emmet.api.routes.materials.electronic_structure.resources import (
     bs_obj_resource,
     bs_resource,
     dos_obj_resource,
     dos_resource,
     es_resource,
 )
 
-resources.update(
-    {
-        "electronic_structure": [
-            bs_resource(es_store),
-            dos_resource(es_store),
-            es_resource(es_store),
-            bs_obj_resource(s3_bs),
-            dos_obj_resource(s3_dos),
-        ]
-    }
+materials_resources.extend(
+    [
+        bs_resource(es_store),
+        dos_resource(es_store),
+        es_resource(es_store),
+        bs_obj_resource(s3_bs),
+        dos_obj_resource(s3_dos),
+    ]
 )
+
 # MPComplete
-from emmet.api.routes.mpcomplete.resources import mpcomplete_resource
+from emmet.api.routes.materials.mpcomplete.resources import mpcomplete_resource
 
 resources.update({"mpcomplete": [mpcomplete_resource(mpcomplete_store)]})
 
+# DOIs
+from emmet.api.routes.dois.resources import dois_resource
+
+resources.update({"dois": [dois_resource(doi_store)]})
+
 # Consumers
 from emmet.api.routes._consumer.resources import settings_resource
 
 resources.update({"_user_settings": [settings_resource(consumer_settings_store)]})
 
 # General Store
 from emmet.api.routes._general_store.resources import general_store_resource
 
 resources.update({"_general_store": [general_store_resource(general_store)]})
 
+resources.update({"materials": materials_resources})
```

### Comparing `emmet-api-0.51.9/mpcule_resources.py` & `emmet-api-0.52.0/molecule_resources.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import os
 from emmet.api.core.settings import MAPISettings
 from maggma.stores import MongoURIStore
 
-from emmet.api.routes.mpcules.tasks.resources import (
+from emmet.api.routes.molecules.tasks.resources import (
     task_resource,
     task_deprecation_resource
 )
-from emmet.api.routes.mpcules.association.resources import mol_assoc_resource
-from emmet.api.routes.mpcules.molecules.resources import (
+from emmet.api.routes.molecules.association.resources import (
+    find_molecule_assoc_resource,
+    mol_assoc_resource
+)
+from emmet.api.routes.molecules.molecules.resources import (
     find_molecule_resource,
-    find_molecule_connectivity_resource,
     molecules_resource
 )
-from emmet.api.routes.mpcules.partial_charges.resources import charges_resource
-from emmet.api.routes.mpcules.partial_spins.resources import spins_resource
-from emmet.api.routes.mpcules.bonds.resources import bonding_resource
-from emmet.api.routes.mpcules.orbitals.resources import orbitals_resource
-from emmet.api.routes.mpcules.redox.resources import redox_resource
-from emmet.api.routes.mpcules.thermo.resources import thermo_resource
-from emmet.api.routes.mpcules.vibrations.resources import vibration_resource
-from emmet.api.routes.mpcules.summary.resources import summary_resource
+from emmet.api.routes.molecules.partial_charges.resources import charges_resource
+from emmet.api.routes.molecules.partial_spins.resources import spins_resource
+from emmet.api.routes.molecules.bonds.resources import bonding_resource
+from emmet.api.routes.molecules.orbitals.resources import orbitals_resource
+from emmet.api.routes.molecules.redox.resources import redox_resource
+from emmet.api.routes.molecules.thermo.resources import thermo_resource
+from emmet.api.routes.molecules.vibrations.resources import vibration_resource
+from emmet.api.routes.molecules.summary.resources import summary_resource
 
 
 resources = {}
 
 default_settings = MAPISettings()
 
 db_uri = os.environ.get("MPCONTRIBS_MONGO_HOST", None)
@@ -81,54 +83,58 @@
         uri=db_uri, database="mp_molecules", key="molecule_id", collection_name="mpcules_summary"
     )
 
 else:
     raise RuntimeError("Must specify MongoDB URI containing inputs.")
 
 
-mpcules_resources = list()
+mp_molecules_resources = list()
 
 # Tasks
-mpcules_resources.extend(
+mp_molecules_resources.extend(
     [
         task_resource(task_store),
         task_deprecation_resource(task_store)
     ]
 )
 
 # Assoc
-mpcules_resources.extend([mol_assoc_resource(assoc_store)])
+mp_molecules_resources.extend(
+    [
+        mol_assoc_resource(assoc_store),
+        find_molecule_assoc_resource(assoc_store)
+    ]
+)
 
 # Molecules
-mpcules_resources.extend(
+mp_molecules_resources.extend(
     [
         molecules_resource(mol_store),
         find_molecule_resource(mol_store),
-        find_molecule_connectivity_resource(mol_store),
     ]
 )
 
 # Partial charges
-mpcules_resources.extend([charges_resource(charges_store)])
+mp_molecules_resources.extend([charges_resource(charges_store)])
 
 # Partial spins
-mpcules_resources.extend([spins_resource(spins_store)])
+mp_molecules_resources.extend([spins_resource(spins_store)])
 
 # Bonds
-mpcules_resources.extend([bonding_resource(bonds_store)])
+mp_molecules_resources.extend([bonding_resource(bonds_store)])
 
 # Orbitals
-mpcules_resources.extend([orbitals_resource(orbitals_store)])
+mp_molecules_resources.extend([orbitals_resource(orbitals_store)])
 
 # Redox
-mpcules_resources.extend([redox_resource(redox_store)])
+mp_molecules_resources.extend([redox_resource(redox_store)])
 
 # Thermo
-mpcules_resources.extend([thermo_resource(thermo_store)])
+mp_molecules_resources.extend([thermo_resource(thermo_store)])
 
 # Vibes
-mpcules_resources.extend([vibration_resource(vibes_store)])
+mp_molecules_resources.extend([vibration_resource(vibes_store)])
 
 # Summary
-mpcules_resources.extend([summary_resource(summary_store)])
+mp_molecules_resources.extend([summary_resource(summary_store)])
 
-resources.update({"mpcules": mpcules_resources})
+resources.update({"molecules": mp_molecules_resources})
```

### Comparing `emmet-api-0.51.9/requirements/deployment.txt` & `emmet-api-0.52.0/requirements/deployment.txt`

 * *Files 5% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 #
 #    pip-compile --output-file=emmet/emmet-api/requirements/deployment.txt --resolver=backtracking emmet/emmet-api/setup.py python/requirements.txt
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.6.2
     # via starlette
-attrs==22.2.0
+attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
-boto3==1.26.106
+boto3==1.26.114
     # via
     #   emmet-api (emmet/emmet-api/setup.py)
     #   maggma
-botocore==1.29.106
+botocore==1.29.114
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.1
     # via ddtrace
 cattrs==22.2.0
     # via ddtrace
@@ -38,37 +38,37 @@
 click==8.1.3
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
 contourpy==1.0.7
     # via matplotlib
-cryptography==40.0.1
+cryptography==40.0.2
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.11.0
+ddtrace==1.11.2
     # via emmet-api (emmet/emmet-api/setup.py)
 deprecated==1.2.13
     # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.50.0
+emmet-core[all]==0.51.13
     # via
     #   emmet-api (emmet/emmet-api/setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
     # via cattrs
-fastapi==0.95.0
+fastapi==0.95.1
     # via
     #   emmet-api (emmet/emmet-api/setup.py)
     #   maggma
 flask==2.2.3
     # via mongogrant
 fonttools==4.39.3
     # via matplotlib
@@ -82,15 +82,15 @@
     # via uvicorn-tschaume
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.0.1
     # via opentelemetry-api
-inflect==6.0.2
+inflect==6.0.4
     # via robocrys
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
 jmespath==1.0.1
     # via
@@ -120,23 +120,23 @@
     # via
     #   -r python/requirements.txt
     #   pymatgen
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
-monty==2022.9.9
+monty==2023.4.10
     # via
     #   emmet-core
     #   maggma
     #   matminer
     #   mp-api
     #   pymatgen
     #   robocrys
-mp-api==0.30.11
+mp-api==0.30.10
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   maggma
     #   mp-api
@@ -157,36 +157,36 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.17.0
     # via ddtrace
-orjson==3.8.9
+orjson==3.8.10
     # via maggma
-packaging==23.0
+packaging==23.1
     # via
     #   ddtrace
     #   matplotlib
     #   mongomock
     #   plotly
-palettable==3.3.0
+palettable==3.3.2
     # via pymatgen
 pandas==2.0.0
     # via
     #   -r python/requirements.txt
     #   matminer
     #   pymatgen
 paramiko==3.1.0
     # via sshtunnel
 pillow==9.5.0
     # via matplotlib
-plotly==5.14.0
+plotly==5.14.1
     # via pymatgen
-protobuf==4.22.1
+protobuf==4.22.3
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
@@ -197,15 +197,15 @@
     # via cffi
 pydantic==1.10.7
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
-pydash==6.0.2
+pydash==7.0.1
     # via maggma
 pymatgen==2023.3.23
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
@@ -310,14 +310,15 @@
     #   pymatgen
 typing-extensions==4.5.0
     # via
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   pydantic
+    #   pydash
 tzdata==2023.3
     # via pandas
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.15
     # via
     #   botocore
```

### Comparing `emmet-api-0.51.9/requirements/macos-latest_py3.10.txt` & `emmet-api-0.52.0/requirements/ubuntu-latest_py3.8.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --output-file=requirements/macos-latest_py3.10.txt --resolver=backtracking
+#    pip-compile --output-file=requirements/ubuntu-latest_py3.8.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.6.2
     # via starlette
 attrs==22.2.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
-boto3==1.26.106
+boto3==1.26.114
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.106
+botocore==1.29.114
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.1
     # via ddtrace
 cattrs==22.2.0
     # via ddtrace
@@ -38,37 +38,37 @@
 click==8.1.3
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
 contourpy==1.0.7
     # via matplotlib
-cryptography==40.0.1
+cryptography==40.0.2
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.11.0
+ddtrace==1.11.2
     # via emmet-api (setup.py)
 deprecated==1.2.13
     # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.50.0
+emmet-core[all]==0.51.13
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
     # via cattrs
-fastapi==0.95.0
+fastapi==0.95.1
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.2.3
     # via mongogrant
 fonttools==4.39.3
     # via matplotlib
@@ -81,16 +81,22 @@
 h11==0.14.0
     # via uvicorn-tschaume
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.0.1
-    # via opentelemetry-api
-inflect==6.0.2
+    # via
+    #   flask
+    #   opentelemetry-api
+importlib-resources==5.12.0
+    # via
+    #   jsonschema
+    #   matplotlib
+inflect==6.0.4
     # via robocrys
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
 jmespath==1.0.1
     # via
@@ -118,23 +124,23 @@
     # via robocrys
 matplotlib==3.7.1
     # via pymatgen
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
-monty==2022.9.9
+monty==2023.4.10
     # via
     #   emmet-core
     #   maggma
     #   matminer
     #   mp-api
     #   pymatgen
     #   robocrys
-mp-api==0.30.11
+mp-api==0.30.10
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   maggma
     #   mp-api
@@ -154,35 +160,37 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.17.0
     # via ddtrace
-orjson==3.8.9
+orjson==3.8.10
     # via maggma
-packaging==23.0
+packaging==23.1
     # via
     #   ddtrace
     #   matplotlib
     #   mongomock
     #   plotly
-palettable==3.3.0
+palettable==3.3.1
     # via pymatgen
 pandas==2.0.0
     # via
     #   matminer
     #   pymatgen
 paramiko==3.1.0
     # via sshtunnel
 pillow==9.5.0
     # via matplotlib
-plotly==5.14.0
+pkgutil-resolve-name==1.3.10
+    # via jsonschema
+plotly==5.14.1
     # via pymatgen
-protobuf==4.22.1
+protobuf==4.22.3
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
@@ -193,15 +201,15 @@
     # via cffi
 pydantic==1.10.7
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
-pydash==6.0.2
+pydash==7.0.1
     # via maggma
 pymatgen==2023.3.23
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
@@ -301,18 +309,22 @@
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
 typing-extensions==4.5.0
     # via
+    #   aioitertools
+    #   bytecode
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   pydantic
+    #   pydash
+    #   starlette
 tzdata==2023.3
     # via pandas
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.15
     # via
     #   botocore
@@ -322,11 +334,13 @@
 werkzeug==2.2.3
     # via flask
 wrapt==1.15.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
 zipp==3.15.0
-    # via importlib-metadata
+    # via
+    #   importlib-metadata
+    #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.51.9/requirements/macos-latest_py3.10_extras.txt` & `emmet-api-0.52.0/requirements/macos-latest_py3.8_extras.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.10_extras.txt --resolver=backtracking
+#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.8_extras.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.6.2
     # via starlette
 attrs==22.2.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
-    #   pytest
 bcrypt==4.0.1
     # via paramiko
-boto3==1.26.106
+boto3==1.26.114
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.106
+botocore==1.29.114
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.1
     # via ddtrace
@@ -46,79 +45,87 @@
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
 colorama==0.4.6
     # via griffe
 contourpy==1.0.7
     # via matplotlib
-coverage[toml]==7.2.2
+coverage[toml]==7.2.3
     # via pytest-cov
-cryptography==40.0.1
+cryptography==40.0.2
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.11.0
+ddtrace==1.11.2
     # via emmet-api (setup.py)
 deprecated==1.2.13
     # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.50.0
+emmet-core[all]==0.51.13
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
     # via
     #   cattrs
     #   pytest
-fastapi==0.95.0
+fastapi==0.95.1
     # via
     #   emmet-api (setup.py)
     #   maggma
-filelock==3.10.7
+filelock==3.11.0
     # via virtualenv
 flake8==6.0.0
     # via emmet-api (setup.py)
 flask==2.2.3
     # via mongogrant
 fonttools==4.39.3
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.26.0
+griffe==0.27.0
     # via mkdocstrings-python
 gunicorn==20.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
     # via uvicorn-tschaume
 htmlmin2==0.1.13
     # via mkdocs-minify-plugin
 identify==2.5.22
     # via pre-commit
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.0.1
-    # via opentelemetry-api
-inflect==6.0.2
+    # via
+    #   flask
+    #   markdown
+    #   mkdocs
+    #   opentelemetry-api
+importlib-resources==5.12.0
+    # via
+    #   jsonschema
+    #   matplotlib
+inflect==6.0.4
     # via robocrys
 iniconfig==2.0.0
     # via pytest
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via
@@ -176,53 +183,53 @@
     #   mkdocs-awesome-pages-plugin
     #   mkdocs-markdownextradata-plugin
     #   mkdocs-material
     #   mkdocs-minify-plugin
     #   mkdocstrings
 mkdocs-autorefs==0.4.1
     # via mkdocstrings
-mkdocs-awesome-pages-plugin==2.8.0
+mkdocs-awesome-pages-plugin==2.9.0
     # via emmet-api (setup.py)
 mkdocs-markdownextradata-plugin==0.2.5
     # via emmet-api (setup.py)
 mkdocs-material==8.2.16
     # via emmet-api (setup.py)
 mkdocs-material-extensions==1.1.1
     # via
     #   emmet-api (setup.py)
     #   mkdocs-material
 mkdocs-minify-plugin==0.6.4
     # via emmet-api (setup.py)
-mkdocstrings[python]==0.20.0
+mkdocstrings[python]==0.21.2
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
 mkdocstrings-python==0.9.0
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
-monty==2022.9.9
+monty==2023.4.10
     # via
     #   emmet-core
     #   maggma
     #   matminer
     #   mp-api
     #   pymatgen
     #   robocrys
-mp-api==0.30.11
+mp-api==0.30.10
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   maggma
     #   mp-api
-mypy==1.1.1
+mypy==1.2.0
     # via emmet-api (setup.py)
 mypy-extensions==1.0.0
     # via
     #   emmet-api (setup.py)
     #   mypy
 natsort==8.3.1
     # via mkdocs-awesome-pages-plugin
@@ -244,43 +251,45 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.17.0
     # via ddtrace
-orjson==3.8.9
+orjson==3.8.10
     # via maggma
-packaging==23.0
+packaging==23.1
     # via
     #   ddtrace
     #   matplotlib
     #   mkdocs
     #   mongomock
     #   plotly
     #   pytest
-palettable==3.3.0
+palettable==3.3.1
     # via pymatgen
 pandas==2.0.0
     # via
     #   matminer
     #   pymatgen
 paramiko==3.1.0
     # via sshtunnel
 pillow==9.5.0
     # via matplotlib
+pkgutil-resolve-name==1.3.10
+    # via jsonschema
 platformdirs==3.2.0
     # via virtualenv
-plotly==5.14.0
+plotly==5.14.1
     # via pymatgen
 pluggy==1.0.0
     # via pytest
 pre-commit==3.2.2
     # via emmet-api (setup.py)
-protobuf==4.22.1
+protobuf==4.22.3
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
@@ -295,50 +304,50 @@
     # via cffi
 pydantic==1.10.7
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
-pydash==6.0.2
+pydash==7.0.1
     # via maggma
 pydocstyle==6.3.0
     # via emmet-api (setup.py)
 pyflakes==3.0.1
     # via flake8
-pygments==2.14.0
+pygments==2.15.0
     # via mkdocs-material
 pymatgen==2023.3.23
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
 pymatgen-analysis-alloys==0.0.6
     # via emmet-core
 pymatgen-analysis-diffusion==2022.7.21
     # via emmet-core
-pymdown-extensions==9.10
+pymdown-extensions==9.11
     # via
     #   mkdocs-material
     #   mkdocstrings
 pymongo==4.3.3
     # via
     #   maggma
     #   matminer
     #   mongogrant
 pynacl==1.5.0
     # via paramiko
 pyparsing==3.0.9
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
-pytest==7.2.2
+pytest==7.3.1
     # via
     #   emmet-api (setup.py)
     #   pytest-cov
 pytest-cov==4.0.0
     # via emmet-api (setup.py)
 python-dateutil==2.8.2
     # via
@@ -444,19 +453,24 @@
     # via emmet-api (setup.py)
 types-setuptools==67.6.0.7
     # via emmet-api (setup.py)
 types-urllib3==1.26.25.10
     # via types-requests
 typing-extensions==4.5.0
     # via
+    #   aioitertools
+    #   bytecode
     #   ddtrace
     #   emmet-core
+    #   mkdocstrings
     #   mp-api
     #   mypy
     #   pydantic
+    #   pydash
+    #   starlette
 tzdata==2023.3
     # via pandas
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.15
     # via
     #   botocore
@@ -474,11 +488,13 @@
 wincertstore==0.2
     # via emmet-api (setup.py)
 wrapt==1.15.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
 zipp==3.15.0
-    # via importlib-metadata
+    # via
+    #   importlib-metadata
+    #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.51.9/requirements/macos-latest_py3.11.txt` & `emmet-api-0.52.0/requirements/macos-latest_py3.9.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --output-file=requirements/macos-latest_py3.11.txt --resolver=backtracking
+#    pip-compile --output-file=requirements/macos-latest_py3.9.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.6.2
     # via starlette
 attrs==22.2.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
-boto3==1.26.106
+boto3==1.26.114
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.106
+botocore==1.29.114
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.1
     # via ddtrace
 cattrs==22.2.0
     # via ddtrace
@@ -38,35 +38,37 @@
 click==8.1.3
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
 contourpy==1.0.7
     # via matplotlib
-cryptography==40.0.1
+cryptography==40.0.2
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.11.0
+ddtrace==1.11.2
     # via emmet-api (setup.py)
 deprecated==1.2.13
     # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.50.0
+emmet-core[all]==0.51.13
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
-fastapi==0.95.0
+exceptiongroup==1.1.1
+    # via cattrs
+fastapi==0.95.1
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.2.3
     # via mongogrant
 fonttools==4.39.3
     # via matplotlib
@@ -79,16 +81,20 @@
 h11==0.14.0
     # via uvicorn-tschaume
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.0.1
-    # via opentelemetry-api
-inflect==6.0.2
+    # via
+    #   flask
+    #   opentelemetry-api
+importlib-resources==5.12.0
+    # via matplotlib
+inflect==6.0.4
     # via robocrys
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
 jmespath==1.0.1
     # via
@@ -116,23 +122,23 @@
     # via robocrys
 matplotlib==3.7.1
     # via pymatgen
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
-monty==2022.9.9
+monty==2023.4.10
     # via
     #   emmet-core
     #   maggma
     #   matminer
     #   mp-api
     #   pymatgen
     #   robocrys
-mp-api==0.30.11
+mp-api==0.30.10
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   maggma
     #   mp-api
@@ -152,35 +158,35 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.17.0
     # via ddtrace
-orjson==3.8.9
+orjson==3.8.10
     # via maggma
-packaging==23.0
+packaging==23.1
     # via
     #   ddtrace
     #   matplotlib
     #   mongomock
     #   plotly
-palettable==3.3.0
+palettable==3.3.1
     # via pymatgen
 pandas==2.0.0
     # via
     #   matminer
     #   pymatgen
 paramiko==3.1.0
     # via sshtunnel
 pillow==9.5.0
     # via matplotlib
-plotly==5.14.0
+plotly==5.14.1
     # via pymatgen
-protobuf==4.22.1
+protobuf==4.22.3
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
@@ -191,15 +197,15 @@
     # via cffi
 pydantic==1.10.7
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
-pydash==6.0.2
+pydash==7.0.1
     # via maggma
 pymatgen==2023.3.23
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
@@ -240,14 +246,16 @@
     #   pymatgen
 robocrys==0.2.7
     # via emmet-core
 ruamel-yaml==0.17.21
     # via
     #   pymatgen
     #   robocrys
+ruamel-yaml-clib==0.2.7
+    # via ruamel-yaml
 s3transfer==0.6.0
     # via boto3
 scikit-learn==1.2.2
     # via matminer
 scipy==1.10.1
     # via
     #   pymatgen
@@ -297,18 +305,22 @@
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
 typing-extensions==4.5.0
     # via
+    #   aioitertools
+    #   bytecode
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   pydantic
+    #   pydash
+    #   starlette
 tzdata==2023.3
     # via pandas
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.15
     # via
     #   botocore
@@ -318,11 +330,13 @@
 werkzeug==2.2.3
     # via flask
 wrapt==1.15.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
 zipp==3.15.0
-    # via importlib-metadata
+    # via
+    #   importlib-metadata
+    #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.51.9/requirements/macos-latest_py3.11_extras.txt` & `emmet-api-0.52.0/requirements/macos-latest_py3.11_extras.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,22 +9,21 @@
 anyio==3.6.2
     # via starlette
 attrs==22.2.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
-    #   pytest
 bcrypt==4.0.1
     # via paramiko
-boto3==1.26.106
+boto3==1.26.114
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.106
+botocore==1.29.114
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.1
     # via ddtrace
@@ -46,59 +45,59 @@
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
 colorama==0.4.6
     # via griffe
 contourpy==1.0.7
     # via matplotlib
-coverage[toml]==7.2.2
+coverage[toml]==7.2.3
     # via pytest-cov
-cryptography==40.0.1
+cryptography==40.0.2
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.11.0
+ddtrace==1.11.2
     # via emmet-api (setup.py)
 deprecated==1.2.13
     # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.50.0
+emmet-core[all]==0.51.13
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
-fastapi==0.95.0
+fastapi==0.95.1
     # via
     #   emmet-api (setup.py)
     #   maggma
-filelock==3.10.7
+filelock==3.11.0
     # via virtualenv
 flake8==6.0.0
     # via emmet-api (setup.py)
 flask==2.2.3
     # via mongogrant
 fonttools==4.39.3
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.26.0
+griffe==0.27.0
     # via mkdocstrings-python
 gunicorn==20.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
     # via uvicorn-tschaume
 htmlmin2==0.1.13
     # via mkdocs-minify-plugin
@@ -106,15 +105,15 @@
     # via pre-commit
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.0.1
     # via opentelemetry-api
-inflect==6.0.2
+inflect==6.0.4
     # via robocrys
 iniconfig==2.0.0
     # via pytest
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via
@@ -172,53 +171,53 @@
     #   mkdocs-awesome-pages-plugin
     #   mkdocs-markdownextradata-plugin
     #   mkdocs-material
     #   mkdocs-minify-plugin
     #   mkdocstrings
 mkdocs-autorefs==0.4.1
     # via mkdocstrings
-mkdocs-awesome-pages-plugin==2.8.0
+mkdocs-awesome-pages-plugin==2.9.0
     # via emmet-api (setup.py)
 mkdocs-markdownextradata-plugin==0.2.5
     # via emmet-api (setup.py)
 mkdocs-material==8.2.16
     # via emmet-api (setup.py)
 mkdocs-material-extensions==1.1.1
     # via
     #   emmet-api (setup.py)
     #   mkdocs-material
 mkdocs-minify-plugin==0.6.4
     # via emmet-api (setup.py)
-mkdocstrings[python]==0.20.0
+mkdocstrings[python]==0.21.2
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
 mkdocstrings-python==0.9.0
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
-monty==2022.9.9
+monty==2023.4.10
     # via
     #   emmet-core
     #   maggma
     #   matminer
     #   mp-api
     #   pymatgen
     #   robocrys
-mp-api==0.30.11
+mp-api==0.30.10
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   maggma
     #   mp-api
-mypy==1.1.1
+mypy==1.2.0
     # via emmet-api (setup.py)
 mypy-extensions==1.0.0
     # via
     #   emmet-api (setup.py)
     #   mypy
 natsort==8.3.1
     # via mkdocs-awesome-pages-plugin
@@ -240,43 +239,43 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.17.0
     # via ddtrace
-orjson==3.8.9
+orjson==3.8.10
     # via maggma
-packaging==23.0
+packaging==23.1
     # via
     #   ddtrace
     #   matplotlib
     #   mkdocs
     #   mongomock
     #   plotly
     #   pytest
-palettable==3.3.0
+palettable==3.3.1
     # via pymatgen
 pandas==2.0.0
     # via
     #   matminer
     #   pymatgen
 paramiko==3.1.0
     # via sshtunnel
 pillow==9.5.0
     # via matplotlib
 platformdirs==3.2.0
     # via virtualenv
-plotly==5.14.0
+plotly==5.14.1
     # via pymatgen
 pluggy==1.0.0
     # via pytest
 pre-commit==3.2.2
     # via emmet-api (setup.py)
-protobuf==4.22.1
+protobuf==4.22.3
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
@@ -291,50 +290,50 @@
     # via cffi
 pydantic==1.10.7
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
-pydash==6.0.2
+pydash==7.0.1
     # via maggma
 pydocstyle==6.3.0
     # via emmet-api (setup.py)
 pyflakes==3.0.1
     # via flake8
-pygments==2.14.0
+pygments==2.15.0
     # via mkdocs-material
 pymatgen==2023.3.23
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
 pymatgen-analysis-alloys==0.0.6
     # via emmet-core
 pymatgen-analysis-diffusion==2022.7.21
     # via emmet-core
-pymdown-extensions==9.10
+pymdown-extensions==9.11
     # via
     #   mkdocs-material
     #   mkdocstrings
 pymongo==4.3.3
     # via
     #   maggma
     #   matminer
     #   mongogrant
 pynacl==1.5.0
     # via paramiko
 pyparsing==3.0.9
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
-pytest==7.2.2
+pytest==7.3.1
     # via
     #   emmet-api (setup.py)
     #   pytest-cov
 pytest-cov==4.0.0
     # via emmet-api (setup.py)
 python-dateutil==2.8.2
     # via
@@ -438,14 +437,15 @@
 typing-extensions==4.5.0
     # via
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   mypy
     #   pydantic
+    #   pydash
 tzdata==2023.3
     # via pandas
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.15
     # via
     #   botocore
```

### Comparing `emmet-api-0.51.9/requirements/macos-latest_py3.8.txt` & `emmet-api-0.52.0/requirements/macos-latest_py3.8.txt`

 * *Files 0% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 attrs==22.2.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
-boto3==1.26.106
+boto3==1.26.114
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.106
+botocore==1.29.114
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.1
     # via ddtrace
 cattrs==22.2.0
     # via ddtrace
@@ -38,37 +38,37 @@
 click==8.1.3
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
 contourpy==1.0.7
     # via matplotlib
-cryptography==40.0.1
+cryptography==40.0.2
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.11.0
+ddtrace==1.11.2
     # via emmet-api (setup.py)
 deprecated==1.2.13
     # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.50.0
+emmet-core[all]==0.51.13
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
     # via cattrs
-fastapi==0.95.0
+fastapi==0.95.1
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.2.3
     # via mongogrant
 fonttools==4.39.3
     # via matplotlib
@@ -88,15 +88,15 @@
     # via
     #   flask
     #   opentelemetry-api
 importlib-resources==5.12.0
     # via
     #   jsonschema
     #   matplotlib
-inflect==6.0.2
+inflect==6.0.4
     # via robocrys
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
 jmespath==1.0.1
     # via
@@ -124,23 +124,23 @@
     # via robocrys
 matplotlib==3.7.1
     # via pymatgen
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
-monty==2022.9.9
+monty==2023.4.10
     # via
     #   emmet-core
     #   maggma
     #   matminer
     #   mp-api
     #   pymatgen
     #   robocrys
-mp-api==0.30.11
+mp-api==0.30.10
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   maggma
     #   mp-api
@@ -160,37 +160,37 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.17.0
     # via ddtrace
-orjson==3.8.9
+orjson==3.8.10
     # via maggma
-packaging==23.0
+packaging==23.1
     # via
     #   ddtrace
     #   matplotlib
     #   mongomock
     #   plotly
-palettable==3.3.0
+palettable==3.3.1
     # via pymatgen
 pandas==2.0.0
     # via
     #   matminer
     #   pymatgen
 paramiko==3.1.0
     # via sshtunnel
 pillow==9.5.0
     # via matplotlib
 pkgutil-resolve-name==1.3.10
     # via jsonschema
-plotly==5.14.0
+plotly==5.14.1
     # via pymatgen
-protobuf==4.22.1
+protobuf==4.22.3
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
@@ -201,15 +201,15 @@
     # via cffi
 pydantic==1.10.7
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
-pydash==6.0.2
+pydash==7.0.1
     # via maggma
 pymatgen==2023.3.23
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
@@ -315,14 +315,15 @@
     # via
     #   aioitertools
     #   bytecode
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   pydantic
+    #   pydash
     #   starlette
 tzdata==2023.3
     # via pandas
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.15
     # via
```

### Comparing `emmet-api-0.51.9/requirements/macos-latest_py3.8_extras.txt` & `emmet-api-0.52.0/requirements/ubuntu-latest_py3.8_extras.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 #
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.8_extras.txt --resolver=backtracking
+#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.8_extras.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.6.2
     # via starlette
 attrs==22.2.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
-    #   pytest
 bcrypt==4.0.1
     # via paramiko
-boto3==1.26.106
+boto3==1.26.114
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.106
+botocore==1.29.114
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.1
     # via ddtrace
@@ -46,63 +45,63 @@
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
 colorama==0.4.6
     # via griffe
 contourpy==1.0.7
     # via matplotlib
-coverage[toml]==7.2.2
+coverage[toml]==7.2.3
     # via pytest-cov
-cryptography==40.0.1
+cryptography==40.0.2
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.11.0
+ddtrace==1.11.2
     # via emmet-api (setup.py)
 deprecated==1.2.13
     # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.50.0
+emmet-core[all]==0.51.13
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
     # via
     #   cattrs
     #   pytest
-fastapi==0.95.0
+fastapi==0.95.1
     # via
     #   emmet-api (setup.py)
     #   maggma
-filelock==3.10.7
+filelock==3.11.0
     # via virtualenv
 flake8==6.0.0
     # via emmet-api (setup.py)
 flask==2.2.3
     # via mongogrant
 fonttools==4.39.3
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.26.0
+griffe==0.27.0
     # via mkdocstrings-python
 gunicorn==20.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
     # via uvicorn-tschaume
 htmlmin2==0.1.13
     # via mkdocs-minify-plugin
@@ -118,15 +117,15 @@
     #   markdown
     #   mkdocs
     #   opentelemetry-api
 importlib-resources==5.12.0
     # via
     #   jsonschema
     #   matplotlib
-inflect==6.0.2
+inflect==6.0.4
     # via robocrys
 iniconfig==2.0.0
     # via pytest
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via
@@ -184,53 +183,53 @@
     #   mkdocs-awesome-pages-plugin
     #   mkdocs-markdownextradata-plugin
     #   mkdocs-material
     #   mkdocs-minify-plugin
     #   mkdocstrings
 mkdocs-autorefs==0.4.1
     # via mkdocstrings
-mkdocs-awesome-pages-plugin==2.8.0
+mkdocs-awesome-pages-plugin==2.9.0
     # via emmet-api (setup.py)
 mkdocs-markdownextradata-plugin==0.2.5
     # via emmet-api (setup.py)
 mkdocs-material==8.2.16
     # via emmet-api (setup.py)
 mkdocs-material-extensions==1.1.1
     # via
     #   emmet-api (setup.py)
     #   mkdocs-material
 mkdocs-minify-plugin==0.6.4
     # via emmet-api (setup.py)
-mkdocstrings[python]==0.20.0
+mkdocstrings[python]==0.21.2
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
 mkdocstrings-python==0.9.0
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
-monty==2022.9.9
+monty==2023.4.10
     # via
     #   emmet-core
     #   maggma
     #   matminer
     #   mp-api
     #   pymatgen
     #   robocrys
-mp-api==0.30.11
+mp-api==0.30.10
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   maggma
     #   mp-api
-mypy==1.1.1
+mypy==1.2.0
     # via emmet-api (setup.py)
 mypy-extensions==1.0.0
     # via
     #   emmet-api (setup.py)
     #   mypy
 natsort==8.3.1
     # via mkdocs-awesome-pages-plugin
@@ -252,45 +251,45 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.17.0
     # via ddtrace
-orjson==3.8.9
+orjson==3.8.10
     # via maggma
-packaging==23.0
+packaging==23.1
     # via
     #   ddtrace
     #   matplotlib
     #   mkdocs
     #   mongomock
     #   plotly
     #   pytest
-palettable==3.3.0
+palettable==3.3.1
     # via pymatgen
 pandas==2.0.0
     # via
     #   matminer
     #   pymatgen
 paramiko==3.1.0
     # via sshtunnel
 pillow==9.5.0
     # via matplotlib
 pkgutil-resolve-name==1.3.10
     # via jsonschema
 platformdirs==3.2.0
     # via virtualenv
-plotly==5.14.0
+plotly==5.14.1
     # via pymatgen
 pluggy==1.0.0
     # via pytest
 pre-commit==3.2.2
     # via emmet-api (setup.py)
-protobuf==4.22.1
+protobuf==4.22.3
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
@@ -305,50 +304,50 @@
     # via cffi
 pydantic==1.10.7
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
-pydash==6.0.2
+pydash==7.0.1
     # via maggma
 pydocstyle==6.3.0
     # via emmet-api (setup.py)
 pyflakes==3.0.1
     # via flake8
-pygments==2.14.0
+pygments==2.15.0
     # via mkdocs-material
 pymatgen==2023.3.23
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
 pymatgen-analysis-alloys==0.0.6
     # via emmet-core
 pymatgen-analysis-diffusion==2022.7.21
     # via emmet-core
-pymdown-extensions==9.10
+pymdown-extensions==9.11
     # via
     #   mkdocs-material
     #   mkdocstrings
 pymongo==4.3.3
     # via
     #   maggma
     #   matminer
     #   mongogrant
 pynacl==1.5.0
     # via paramiko
 pyparsing==3.0.9
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
-pytest==7.2.2
+pytest==7.3.1
     # via
     #   emmet-api (setup.py)
     #   pytest-cov
 pytest-cov==4.0.0
     # via emmet-api (setup.py)
 python-dateutil==2.8.2
     # via
@@ -458,17 +457,19 @@
     # via types-requests
 typing-extensions==4.5.0
     # via
     #   aioitertools
     #   bytecode
     #   ddtrace
     #   emmet-core
+    #   mkdocstrings
     #   mp-api
     #   mypy
     #   pydantic
+    #   pydash
     #   starlette
 tzdata==2023.3
     # via pandas
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.15
     # via
```

### Comparing `emmet-api-0.51.9/requirements/macos-latest_py3.9.txt` & `emmet-api-0.52.0/requirements/ubuntu-latest_py3.9.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --output-file=requirements/macos-latest_py3.9.txt --resolver=backtracking
+#    pip-compile --output-file=requirements/ubuntu-latest_py3.9.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.6.2
     # via starlette
 attrs==22.2.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
-boto3==1.26.106
+boto3==1.26.114
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.106
+botocore==1.29.114
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.1
     # via ddtrace
 cattrs==22.2.0
     # via ddtrace
@@ -38,37 +38,37 @@
 click==8.1.3
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
 contourpy==1.0.7
     # via matplotlib
-cryptography==40.0.1
+cryptography==40.0.2
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.11.0
+ddtrace==1.11.2
     # via emmet-api (setup.py)
 deprecated==1.2.13
     # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.50.0
+emmet-core[all]==0.51.13
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
     # via cattrs
-fastapi==0.95.0
+fastapi==0.95.1
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.2.3
     # via mongogrant
 fonttools==4.39.3
     # via matplotlib
@@ -86,15 +86,15 @@
     #   requests
 importlib-metadata==6.0.1
     # via
     #   flask
     #   opentelemetry-api
 importlib-resources==5.12.0
     # via matplotlib
-inflect==6.0.2
+inflect==6.0.4
     # via robocrys
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
 jmespath==1.0.1
     # via
@@ -122,23 +122,23 @@
     # via robocrys
 matplotlib==3.7.1
     # via pymatgen
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
-monty==2022.9.9
+monty==2023.4.10
     # via
     #   emmet-core
     #   maggma
     #   matminer
     #   mp-api
     #   pymatgen
     #   robocrys
-mp-api==0.30.11
+mp-api==0.30.10
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   maggma
     #   mp-api
@@ -158,35 +158,35 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.17.0
     # via ddtrace
-orjson==3.8.9
+orjson==3.8.10
     # via maggma
-packaging==23.0
+packaging==23.1
     # via
     #   ddtrace
     #   matplotlib
     #   mongomock
     #   plotly
-palettable==3.3.0
+palettable==3.3.1
     # via pymatgen
 pandas==2.0.0
     # via
     #   matminer
     #   pymatgen
 paramiko==3.1.0
     # via sshtunnel
 pillow==9.5.0
     # via matplotlib
-plotly==5.14.0
+plotly==5.14.1
     # via pymatgen
-protobuf==4.22.1
+protobuf==4.22.3
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
@@ -197,15 +197,15 @@
     # via cffi
 pydantic==1.10.7
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
-pydash==6.0.2
+pydash==7.0.1
     # via maggma
 pymatgen==2023.3.23
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
@@ -311,14 +311,15 @@
     # via
     #   aioitertools
     #   bytecode
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   pydantic
+    #   pydash
     #   starlette
 tzdata==2023.3
     # via pandas
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.15
     # via
```

### Comparing `emmet-api-0.51.9/requirements/macos-latest_py3.9_extras.txt` & `emmet-api-0.52.0/requirements/ubuntu-latest_py3.10_extras.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.9_extras.txt --resolver=backtracking
+#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.10_extras.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.6.2
     # via starlette
 attrs==22.2.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
-    #   pytest
 bcrypt==4.0.1
     # via paramiko
-boto3==1.26.106
+boto3==1.26.114
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.106
+botocore==1.29.114
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.1
     # via ddtrace
@@ -46,85 +45,79 @@
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
 colorama==0.4.6
     # via griffe
 contourpy==1.0.7
     # via matplotlib
-coverage[toml]==7.2.2
+coverage[toml]==7.2.3
     # via pytest-cov
-cryptography==40.0.1
+cryptography==40.0.2
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.11.0
+ddtrace==1.11.2
     # via emmet-api (setup.py)
 deprecated==1.2.13
     # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.50.0
+emmet-core[all]==0.51.13
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
     # via
     #   cattrs
     #   pytest
-fastapi==0.95.0
+fastapi==0.95.1
     # via
     #   emmet-api (setup.py)
     #   maggma
-filelock==3.10.7
+filelock==3.11.0
     # via virtualenv
 flake8==6.0.0
     # via emmet-api (setup.py)
 flask==2.2.3
     # via mongogrant
 fonttools==4.39.3
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.26.0
+griffe==0.27.0
     # via mkdocstrings-python
 gunicorn==20.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
     # via uvicorn-tschaume
 htmlmin2==0.1.13
     # via mkdocs-minify-plugin
 identify==2.5.22
     # via pre-commit
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.0.1
-    # via
-    #   flask
-    #   markdown
-    #   mkdocs
-    #   opentelemetry-api
-importlib-resources==5.12.0
-    # via matplotlib
-inflect==6.0.2
+    # via opentelemetry-api
+inflect==6.0.4
     # via robocrys
 iniconfig==2.0.0
     # via pytest
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via
@@ -182,53 +175,53 @@
     #   mkdocs-awesome-pages-plugin
     #   mkdocs-markdownextradata-plugin
     #   mkdocs-material
     #   mkdocs-minify-plugin
     #   mkdocstrings
 mkdocs-autorefs==0.4.1
     # via mkdocstrings
-mkdocs-awesome-pages-plugin==2.8.0
+mkdocs-awesome-pages-plugin==2.9.0
     # via emmet-api (setup.py)
 mkdocs-markdownextradata-plugin==0.2.5
     # via emmet-api (setup.py)
 mkdocs-material==8.2.16
     # via emmet-api (setup.py)
 mkdocs-material-extensions==1.1.1
     # via
     #   emmet-api (setup.py)
     #   mkdocs-material
 mkdocs-minify-plugin==0.6.4
     # via emmet-api (setup.py)
-mkdocstrings[python]==0.20.0
+mkdocstrings[python]==0.21.2
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
 mkdocstrings-python==0.9.0
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
-monty==2022.9.9
+monty==2023.4.10
     # via
     #   emmet-core
     #   maggma
     #   matminer
     #   mp-api
     #   pymatgen
     #   robocrys
-mp-api==0.30.11
+mp-api==0.30.10
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   maggma
     #   mp-api
-mypy==1.1.1
+mypy==1.2.0
     # via emmet-api (setup.py)
 mypy-extensions==1.0.0
     # via
     #   emmet-api (setup.py)
     #   mypy
 natsort==8.3.1
     # via mkdocs-awesome-pages-plugin
@@ -250,43 +243,43 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.17.0
     # via ddtrace
-orjson==3.8.9
+orjson==3.8.10
     # via maggma
-packaging==23.0
+packaging==23.1
     # via
     #   ddtrace
     #   matplotlib
     #   mkdocs
     #   mongomock
     #   plotly
     #   pytest
-palettable==3.3.0
+palettable==3.3.1
     # via pymatgen
 pandas==2.0.0
     # via
     #   matminer
     #   pymatgen
 paramiko==3.1.0
     # via sshtunnel
 pillow==9.5.0
     # via matplotlib
 platformdirs==3.2.0
     # via virtualenv
-plotly==5.14.0
+plotly==5.14.1
     # via pymatgen
 pluggy==1.0.0
     # via pytest
 pre-commit==3.2.2
     # via emmet-api (setup.py)
-protobuf==4.22.1
+protobuf==4.22.3
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
@@ -301,50 +294,50 @@
     # via cffi
 pydantic==1.10.7
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
-pydash==6.0.2
+pydash==7.0.1
     # via maggma
 pydocstyle==6.3.0
     # via emmet-api (setup.py)
 pyflakes==3.0.1
     # via flake8
-pygments==2.14.0
+pygments==2.15.0
     # via mkdocs-material
 pymatgen==2023.3.23
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
 pymatgen-analysis-alloys==0.0.6
     # via emmet-core
 pymatgen-analysis-diffusion==2022.7.21
     # via emmet-core
-pymdown-extensions==9.10
+pymdown-extensions==9.11
     # via
     #   mkdocs-material
     #   mkdocstrings
 pymongo==4.3.3
     # via
     #   maggma
     #   matminer
     #   mongogrant
 pynacl==1.5.0
     # via paramiko
 pyparsing==3.0.9
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
-pytest==7.2.2
+pytest==7.3.1
     # via
     #   emmet-api (setup.py)
     #   pytest-cov
 pytest-cov==4.0.0
     # via emmet-api (setup.py)
 python-dateutil==2.8.2
     # via
@@ -450,22 +443,20 @@
     # via emmet-api (setup.py)
 types-setuptools==67.6.0.7
     # via emmet-api (setup.py)
 types-urllib3==1.26.25.10
     # via types-requests
 typing-extensions==4.5.0
     # via
-    #   aioitertools
-    #   bytecode
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   mypy
     #   pydantic
-    #   starlette
+    #   pydash
 tzdata==2023.3
     # via pandas
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.15
     # via
     #   botocore
@@ -483,13 +474,11 @@
 wincertstore==0.2
     # via emmet-api (setup.py)
 wrapt==1.15.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
 zipp==3.15.0
-    # via
-    #   importlib-metadata
-    #   importlib-resources
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.51.9/requirements/ubuntu-latest_py3.10.txt` & `emmet-api-0.52.0/requirements/macos-latest_py3.10.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --output-file=requirements/ubuntu-latest_py3.10.txt --resolver=backtracking
+#    pip-compile --output-file=requirements/macos-latest_py3.10.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.6.2
     # via starlette
 attrs==22.2.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
-boto3==1.26.106
+boto3==1.26.114
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.106
+botocore==1.29.114
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.1
     # via ddtrace
 cattrs==22.2.0
     # via ddtrace
@@ -38,37 +38,37 @@
 click==8.1.3
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
 contourpy==1.0.7
     # via matplotlib
-cryptography==40.0.1
+cryptography==40.0.2
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.11.0
+ddtrace==1.11.2
     # via emmet-api (setup.py)
 deprecated==1.2.13
     # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.50.0
+emmet-core[all]==0.51.13
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
     # via cattrs
-fastapi==0.95.0
+fastapi==0.95.1
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.2.3
     # via mongogrant
 fonttools==4.39.3
     # via matplotlib
@@ -82,15 +82,15 @@
     # via uvicorn-tschaume
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.0.1
     # via opentelemetry-api
-inflect==6.0.2
+inflect==6.0.4
     # via robocrys
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
 jmespath==1.0.1
     # via
@@ -118,23 +118,23 @@
     # via robocrys
 matplotlib==3.7.1
     # via pymatgen
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
-monty==2022.9.9
+monty==2023.4.10
     # via
     #   emmet-core
     #   maggma
     #   matminer
     #   mp-api
     #   pymatgen
     #   robocrys
-mp-api==0.30.11
+mp-api==0.30.10
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   maggma
     #   mp-api
@@ -154,35 +154,35 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.17.0
     # via ddtrace
-orjson==3.8.9
+orjson==3.8.10
     # via maggma
-packaging==23.0
+packaging==23.1
     # via
     #   ddtrace
     #   matplotlib
     #   mongomock
     #   plotly
-palettable==3.3.0
+palettable==3.3.1
     # via pymatgen
 pandas==2.0.0
     # via
     #   matminer
     #   pymatgen
 paramiko==3.1.0
     # via sshtunnel
 pillow==9.5.0
     # via matplotlib
-plotly==5.14.0
+plotly==5.14.1
     # via pymatgen
-protobuf==4.22.1
+protobuf==4.22.3
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
@@ -193,15 +193,15 @@
     # via cffi
 pydantic==1.10.7
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
-pydash==6.0.2
+pydash==7.0.1
     # via maggma
 pymatgen==2023.3.23
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
@@ -305,14 +305,15 @@
     #   pymatgen
 typing-extensions==4.5.0
     # via
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   pydantic
+    #   pydash
 tzdata==2023.3
     # via pandas
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.15
     # via
     #   botocore
```

### Comparing `emmet-api-0.51.9/requirements/ubuntu-latest_py3.10_extras.txt` & `emmet-api-0.52.0/requirements/macos-latest_py3.10_extras.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.10_extras.txt --resolver=backtracking
+#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.10_extras.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.6.2
     # via starlette
 attrs==22.2.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
-    #   pytest
 bcrypt==4.0.1
     # via paramiko
-boto3==1.26.106
+boto3==1.26.114
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.106
+botocore==1.29.114
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.1
     # via ddtrace
@@ -46,63 +45,63 @@
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
 colorama==0.4.6
     # via griffe
 contourpy==1.0.7
     # via matplotlib
-coverage[toml]==7.2.2
+coverage[toml]==7.2.3
     # via pytest-cov
-cryptography==40.0.1
+cryptography==40.0.2
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.11.0
+ddtrace==1.11.2
     # via emmet-api (setup.py)
 deprecated==1.2.13
     # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.50.0
+emmet-core[all]==0.51.13
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
     # via
     #   cattrs
     #   pytest
-fastapi==0.95.0
+fastapi==0.95.1
     # via
     #   emmet-api (setup.py)
     #   maggma
-filelock==3.10.7
+filelock==3.11.0
     # via virtualenv
 flake8==6.0.0
     # via emmet-api (setup.py)
 flask==2.2.3
     # via mongogrant
 fonttools==4.39.3
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.26.0
+griffe==0.27.0
     # via mkdocstrings-python
 gunicorn==20.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
     # via uvicorn-tschaume
 htmlmin2==0.1.13
     # via mkdocs-minify-plugin
@@ -110,15 +109,15 @@
     # via pre-commit
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.0.1
     # via opentelemetry-api
-inflect==6.0.2
+inflect==6.0.4
     # via robocrys
 iniconfig==2.0.0
     # via pytest
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via
@@ -176,53 +175,53 @@
     #   mkdocs-awesome-pages-plugin
     #   mkdocs-markdownextradata-plugin
     #   mkdocs-material
     #   mkdocs-minify-plugin
     #   mkdocstrings
 mkdocs-autorefs==0.4.1
     # via mkdocstrings
-mkdocs-awesome-pages-plugin==2.8.0
+mkdocs-awesome-pages-plugin==2.9.0
     # via emmet-api (setup.py)
 mkdocs-markdownextradata-plugin==0.2.5
     # via emmet-api (setup.py)
 mkdocs-material==8.2.16
     # via emmet-api (setup.py)
 mkdocs-material-extensions==1.1.1
     # via
     #   emmet-api (setup.py)
     #   mkdocs-material
 mkdocs-minify-plugin==0.6.4
     # via emmet-api (setup.py)
-mkdocstrings[python]==0.20.0
+mkdocstrings[python]==0.21.2
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
 mkdocstrings-python==0.9.0
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
-monty==2022.9.9
+monty==2023.4.10
     # via
     #   emmet-core
     #   maggma
     #   matminer
     #   mp-api
     #   pymatgen
     #   robocrys
-mp-api==0.30.11
+mp-api==0.30.10
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   maggma
     #   mp-api
-mypy==1.1.1
+mypy==1.2.0
     # via emmet-api (setup.py)
 mypy-extensions==1.0.0
     # via
     #   emmet-api (setup.py)
     #   mypy
 natsort==8.3.1
     # via mkdocs-awesome-pages-plugin
@@ -244,43 +243,43 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.17.0
     # via ddtrace
-orjson==3.8.9
+orjson==3.8.10
     # via maggma
-packaging==23.0
+packaging==23.1
     # via
     #   ddtrace
     #   matplotlib
     #   mkdocs
     #   mongomock
     #   plotly
     #   pytest
-palettable==3.3.0
+palettable==3.3.1
     # via pymatgen
 pandas==2.0.0
     # via
     #   matminer
     #   pymatgen
 paramiko==3.1.0
     # via sshtunnel
 pillow==9.5.0
     # via matplotlib
 platformdirs==3.2.0
     # via virtualenv
-plotly==5.14.0
+plotly==5.14.1
     # via pymatgen
 pluggy==1.0.0
     # via pytest
 pre-commit==3.2.2
     # via emmet-api (setup.py)
-protobuf==4.22.1
+protobuf==4.22.3
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
@@ -295,50 +294,50 @@
     # via cffi
 pydantic==1.10.7
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
-pydash==6.0.2
+pydash==7.0.1
     # via maggma
 pydocstyle==6.3.0
     # via emmet-api (setup.py)
 pyflakes==3.0.1
     # via flake8
-pygments==2.14.0
+pygments==2.15.0
     # via mkdocs-material
 pymatgen==2023.3.23
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
 pymatgen-analysis-alloys==0.0.6
     # via emmet-core
 pymatgen-analysis-diffusion==2022.7.21
     # via emmet-core
-pymdown-extensions==9.10
+pymdown-extensions==9.11
     # via
     #   mkdocs-material
     #   mkdocstrings
 pymongo==4.3.3
     # via
     #   maggma
     #   matminer
     #   mongogrant
 pynacl==1.5.0
     # via paramiko
 pyparsing==3.0.9
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
-pytest==7.2.2
+pytest==7.3.1
     # via
     #   emmet-api (setup.py)
     #   pytest-cov
 pytest-cov==4.0.0
     # via emmet-api (setup.py)
 python-dateutil==2.8.2
     # via
@@ -449,14 +448,15 @@
 typing-extensions==4.5.0
     # via
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   mypy
     #   pydantic
+    #   pydash
 tzdata==2023.3
     # via pandas
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.15
     # via
     #   botocore
```

### Comparing `emmet-api-0.51.9/requirements/ubuntu-latest_py3.11.txt` & `emmet-api-0.52.0/requirements/macos-latest_py3.11.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --output-file=requirements/ubuntu-latest_py3.11.txt --resolver=backtracking
+#    pip-compile --output-file=requirements/macos-latest_py3.11.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.6.2
     # via starlette
 attrs==22.2.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
-boto3==1.26.106
+boto3==1.26.114
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.106
+botocore==1.29.114
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.1
     # via ddtrace
 cattrs==22.2.0
     # via ddtrace
@@ -38,35 +38,35 @@
 click==8.1.3
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
 contourpy==1.0.7
     # via matplotlib
-cryptography==40.0.1
+cryptography==40.0.2
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.11.0
+ddtrace==1.11.2
     # via emmet-api (setup.py)
 deprecated==1.2.13
     # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.50.0
+emmet-core[all]==0.51.13
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
-fastapi==0.95.0
+fastapi==0.95.1
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.2.3
     # via mongogrant
 fonttools==4.39.3
     # via matplotlib
@@ -80,15 +80,15 @@
     # via uvicorn-tschaume
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.0.1
     # via opentelemetry-api
-inflect==6.0.2
+inflect==6.0.4
     # via robocrys
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
 jmespath==1.0.1
     # via
@@ -116,23 +116,23 @@
     # via robocrys
 matplotlib==3.7.1
     # via pymatgen
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
-monty==2022.9.9
+monty==2023.4.10
     # via
     #   emmet-core
     #   maggma
     #   matminer
     #   mp-api
     #   pymatgen
     #   robocrys
-mp-api==0.30.11
+mp-api==0.30.10
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   maggma
     #   mp-api
@@ -152,35 +152,35 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.17.0
     # via ddtrace
-orjson==3.8.9
+orjson==3.8.10
     # via maggma
-packaging==23.0
+packaging==23.1
     # via
     #   ddtrace
     #   matplotlib
     #   mongomock
     #   plotly
-palettable==3.3.0
+palettable==3.3.1
     # via pymatgen
 pandas==2.0.0
     # via
     #   matminer
     #   pymatgen
 paramiko==3.1.0
     # via sshtunnel
 pillow==9.5.0
     # via matplotlib
-plotly==5.14.0
+plotly==5.14.1
     # via pymatgen
-protobuf==4.22.1
+protobuf==4.22.3
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
@@ -191,15 +191,15 @@
     # via cffi
 pydantic==1.10.7
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
-pydash==6.0.2
+pydash==7.0.1
     # via maggma
 pymatgen==2023.3.23
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
@@ -301,14 +301,15 @@
     #   pymatgen
 typing-extensions==4.5.0
     # via
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   pydantic
+    #   pydash
 tzdata==2023.3
     # via pandas
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.15
     # via
     #   botocore
```

### Comparing `emmet-api-0.51.9/requirements/ubuntu-latest_py3.11_extras.txt` & `emmet-api-0.52.0/requirements/ubuntu-latest_py3.11_extras.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,22 +9,21 @@
 anyio==3.6.2
     # via starlette
 attrs==22.2.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
-    #   pytest
 bcrypt==4.0.1
     # via paramiko
-boto3==1.26.106
+boto3==1.26.114
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.106
+botocore==1.29.114
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.1
     # via ddtrace
@@ -46,59 +45,59 @@
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
 colorama==0.4.6
     # via griffe
 contourpy==1.0.7
     # via matplotlib
-coverage[toml]==7.2.2
+coverage[toml]==7.2.3
     # via pytest-cov
-cryptography==40.0.1
+cryptography==40.0.2
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.11.0
+ddtrace==1.11.2
     # via emmet-api (setup.py)
 deprecated==1.2.13
     # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.50.0
+emmet-core[all]==0.51.13
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
-fastapi==0.95.0
+fastapi==0.95.1
     # via
     #   emmet-api (setup.py)
     #   maggma
-filelock==3.10.7
+filelock==3.11.0
     # via virtualenv
 flake8==6.0.0
     # via emmet-api (setup.py)
 flask==2.2.3
     # via mongogrant
 fonttools==4.39.3
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.26.0
+griffe==0.27.0
     # via mkdocstrings-python
 gunicorn==20.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
     # via uvicorn-tschaume
 htmlmin2==0.1.13
     # via mkdocs-minify-plugin
@@ -106,15 +105,15 @@
     # via pre-commit
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.0.1
     # via opentelemetry-api
-inflect==6.0.2
+inflect==6.0.4
     # via robocrys
 iniconfig==2.0.0
     # via pytest
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via
@@ -172,53 +171,53 @@
     #   mkdocs-awesome-pages-plugin
     #   mkdocs-markdownextradata-plugin
     #   mkdocs-material
     #   mkdocs-minify-plugin
     #   mkdocstrings
 mkdocs-autorefs==0.4.1
     # via mkdocstrings
-mkdocs-awesome-pages-plugin==2.8.0
+mkdocs-awesome-pages-plugin==2.9.0
     # via emmet-api (setup.py)
 mkdocs-markdownextradata-plugin==0.2.5
     # via emmet-api (setup.py)
 mkdocs-material==8.2.16
     # via emmet-api (setup.py)
 mkdocs-material-extensions==1.1.1
     # via
     #   emmet-api (setup.py)
     #   mkdocs-material
 mkdocs-minify-plugin==0.6.4
     # via emmet-api (setup.py)
-mkdocstrings[python]==0.20.0
+mkdocstrings[python]==0.21.2
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
 mkdocstrings-python==0.9.0
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
-monty==2022.9.9
+monty==2023.4.10
     # via
     #   emmet-core
     #   maggma
     #   matminer
     #   mp-api
     #   pymatgen
     #   robocrys
-mp-api==0.30.11
+mp-api==0.30.10
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   maggma
     #   mp-api
-mypy==1.1.1
+mypy==1.2.0
     # via emmet-api (setup.py)
 mypy-extensions==1.0.0
     # via
     #   emmet-api (setup.py)
     #   mypy
 natsort==8.3.1
     # via mkdocs-awesome-pages-plugin
@@ -240,43 +239,43 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.17.0
     # via ddtrace
-orjson==3.8.9
+orjson==3.8.10
     # via maggma
-packaging==23.0
+packaging==23.1
     # via
     #   ddtrace
     #   matplotlib
     #   mkdocs
     #   mongomock
     #   plotly
     #   pytest
-palettable==3.3.0
+palettable==3.3.1
     # via pymatgen
 pandas==2.0.0
     # via
     #   matminer
     #   pymatgen
 paramiko==3.1.0
     # via sshtunnel
 pillow==9.5.0
     # via matplotlib
 platformdirs==3.2.0
     # via virtualenv
-plotly==5.14.0
+plotly==5.14.1
     # via pymatgen
 pluggy==1.0.0
     # via pytest
 pre-commit==3.2.2
     # via emmet-api (setup.py)
-protobuf==4.22.1
+protobuf==4.22.3
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
@@ -291,50 +290,50 @@
     # via cffi
 pydantic==1.10.7
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
-pydash==6.0.2
+pydash==7.0.1
     # via maggma
 pydocstyle==6.3.0
     # via emmet-api (setup.py)
 pyflakes==3.0.1
     # via flake8
-pygments==2.14.0
+pygments==2.15.0
     # via mkdocs-material
 pymatgen==2023.3.23
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
 pymatgen-analysis-alloys==0.0.6
     # via emmet-core
 pymatgen-analysis-diffusion==2022.7.21
     # via emmet-core
-pymdown-extensions==9.10
+pymdown-extensions==9.11
     # via
     #   mkdocs-material
     #   mkdocstrings
 pymongo==4.3.3
     # via
     #   maggma
     #   matminer
     #   mongogrant
 pynacl==1.5.0
     # via paramiko
 pyparsing==3.0.9
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
-pytest==7.2.2
+pytest==7.3.1
     # via
     #   emmet-api (setup.py)
     #   pytest-cov
 pytest-cov==4.0.0
     # via emmet-api (setup.py)
 python-dateutil==2.8.2
     # via
@@ -438,14 +437,15 @@
 typing-extensions==4.5.0
     # via
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   mypy
     #   pydantic
+    #   pydash
 tzdata==2023.3
     # via pandas
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.15
     # via
     #   botocore
```

### Comparing `emmet-api-0.51.9/requirements/ubuntu-latest_py3.8.txt` & `emmet-api-0.52.0/requirements/ubuntu-latest_py3.10.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --output-file=requirements/ubuntu-latest_py3.8.txt --resolver=backtracking
+#    pip-compile --output-file=requirements/ubuntu-latest_py3.10.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.6.2
     # via starlette
 attrs==22.2.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
-boto3==1.26.106
+boto3==1.26.114
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.106
+botocore==1.29.114
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.1
     # via ddtrace
 cattrs==22.2.0
     # via ddtrace
@@ -38,37 +38,37 @@
 click==8.1.3
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
 contourpy==1.0.7
     # via matplotlib
-cryptography==40.0.1
+cryptography==40.0.2
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.11.0
+ddtrace==1.11.2
     # via emmet-api (setup.py)
 deprecated==1.2.13
     # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.50.0
+emmet-core[all]==0.51.13
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
     # via cattrs
-fastapi==0.95.0
+fastapi==0.95.1
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.2.3
     # via mongogrant
 fonttools==4.39.3
     # via matplotlib
@@ -81,22 +81,16 @@
 h11==0.14.0
     # via uvicorn-tschaume
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.0.1
-    # via
-    #   flask
-    #   opentelemetry-api
-importlib-resources==5.12.0
-    # via
-    #   jsonschema
-    #   matplotlib
-inflect==6.0.2
+    # via opentelemetry-api
+inflect==6.0.4
     # via robocrys
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
 jmespath==1.0.1
     # via
@@ -124,23 +118,23 @@
     # via robocrys
 matplotlib==3.7.1
     # via pymatgen
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
-monty==2022.9.9
+monty==2023.4.10
     # via
     #   emmet-core
     #   maggma
     #   matminer
     #   mp-api
     #   pymatgen
     #   robocrys
-mp-api==0.30.11
+mp-api==0.30.10
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   maggma
     #   mp-api
@@ -160,37 +154,35 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.17.0
     # via ddtrace
-orjson==3.8.9
+orjson==3.8.10
     # via maggma
-packaging==23.0
+packaging==23.1
     # via
     #   ddtrace
     #   matplotlib
     #   mongomock
     #   plotly
-palettable==3.3.0
+palettable==3.3.1
     # via pymatgen
 pandas==2.0.0
     # via
     #   matminer
     #   pymatgen
 paramiko==3.1.0
     # via sshtunnel
 pillow==9.5.0
     # via matplotlib
-pkgutil-resolve-name==1.3.10
-    # via jsonschema
-plotly==5.14.0
+plotly==5.14.1
     # via pymatgen
-protobuf==4.22.1
+protobuf==4.22.3
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
@@ -201,15 +193,15 @@
     # via cffi
 pydantic==1.10.7
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
-pydash==6.0.2
+pydash==7.0.1
     # via maggma
 pymatgen==2023.3.23
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
@@ -309,21 +301,19 @@
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
 typing-extensions==4.5.0
     # via
-    #   aioitertools
-    #   bytecode
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   pydantic
-    #   starlette
+    #   pydash
 tzdata==2023.3
     # via pandas
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.15
     # via
     #   botocore
@@ -333,13 +323,11 @@
 werkzeug==2.2.3
     # via flask
 wrapt==1.15.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
 zipp==3.15.0
-    # via
-    #   importlib-metadata
-    #   importlib-resources
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.51.9/requirements/ubuntu-latest_py3.8_extras.txt` & `emmet-api-0.52.0/requirements/macos-latest_py3.9_extras.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.8_extras.txt --resolver=backtracking
+#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.9_extras.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.6.2
     # via starlette
 attrs==22.2.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
-    #   pytest
 bcrypt==4.0.1
     # via paramiko
-boto3==1.26.106
+boto3==1.26.114
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.106
+botocore==1.29.114
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.1
     # via ddtrace
@@ -46,63 +45,63 @@
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
 colorama==0.4.6
     # via griffe
 contourpy==1.0.7
     # via matplotlib
-coverage[toml]==7.2.2
+coverage[toml]==7.2.3
     # via pytest-cov
-cryptography==40.0.1
+cryptography==40.0.2
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.11.0
+ddtrace==1.11.2
     # via emmet-api (setup.py)
 deprecated==1.2.13
     # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.50.0
+emmet-core[all]==0.51.13
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
     # via
     #   cattrs
     #   pytest
-fastapi==0.95.0
+fastapi==0.95.1
     # via
     #   emmet-api (setup.py)
     #   maggma
-filelock==3.10.7
+filelock==3.11.0
     # via virtualenv
 flake8==6.0.0
     # via emmet-api (setup.py)
 flask==2.2.3
     # via mongogrant
 fonttools==4.39.3
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.26.0
+griffe==0.27.0
     # via mkdocstrings-python
 gunicorn==20.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
     # via uvicorn-tschaume
 htmlmin2==0.1.13
     # via mkdocs-minify-plugin
@@ -115,18 +114,16 @@
 importlib-metadata==6.0.1
     # via
     #   flask
     #   markdown
     #   mkdocs
     #   opentelemetry-api
 importlib-resources==5.12.0
-    # via
-    #   jsonschema
-    #   matplotlib
-inflect==6.0.2
+    # via matplotlib
+inflect==6.0.4
     # via robocrys
 iniconfig==2.0.0
     # via pytest
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via
@@ -184,53 +181,53 @@
     #   mkdocs-awesome-pages-plugin
     #   mkdocs-markdownextradata-plugin
     #   mkdocs-material
     #   mkdocs-minify-plugin
     #   mkdocstrings
 mkdocs-autorefs==0.4.1
     # via mkdocstrings
-mkdocs-awesome-pages-plugin==2.8.0
+mkdocs-awesome-pages-plugin==2.9.0
     # via emmet-api (setup.py)
 mkdocs-markdownextradata-plugin==0.2.5
     # via emmet-api (setup.py)
 mkdocs-material==8.2.16
     # via emmet-api (setup.py)
 mkdocs-material-extensions==1.1.1
     # via
     #   emmet-api (setup.py)
     #   mkdocs-material
 mkdocs-minify-plugin==0.6.4
     # via emmet-api (setup.py)
-mkdocstrings[python]==0.20.0
+mkdocstrings[python]==0.21.2
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
 mkdocstrings-python==0.9.0
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
-monty==2022.9.9
+monty==2023.4.10
     # via
     #   emmet-core
     #   maggma
     #   matminer
     #   mp-api
     #   pymatgen
     #   robocrys
-mp-api==0.30.11
+mp-api==0.30.10
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   maggma
     #   mp-api
-mypy==1.1.1
+mypy==1.2.0
     # via emmet-api (setup.py)
 mypy-extensions==1.0.0
     # via
     #   emmet-api (setup.py)
     #   mypy
 natsort==8.3.1
     # via mkdocs-awesome-pages-plugin
@@ -252,45 +249,43 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.17.0
     # via ddtrace
-orjson==3.8.9
+orjson==3.8.10
     # via maggma
-packaging==23.0
+packaging==23.1
     # via
     #   ddtrace
     #   matplotlib
     #   mkdocs
     #   mongomock
     #   plotly
     #   pytest
-palettable==3.3.0
+palettable==3.3.1
     # via pymatgen
 pandas==2.0.0
     # via
     #   matminer
     #   pymatgen
 paramiko==3.1.0
     # via sshtunnel
 pillow==9.5.0
     # via matplotlib
-pkgutil-resolve-name==1.3.10
-    # via jsonschema
 platformdirs==3.2.0
     # via virtualenv
-plotly==5.14.0
+plotly==5.14.1
     # via pymatgen
 pluggy==1.0.0
     # via pytest
 pre-commit==3.2.2
     # via emmet-api (setup.py)
-protobuf==4.22.1
+protobuf==4.22.3
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
@@ -305,50 +300,50 @@
     # via cffi
 pydantic==1.10.7
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
-pydash==6.0.2
+pydash==7.0.1
     # via maggma
 pydocstyle==6.3.0
     # via emmet-api (setup.py)
 pyflakes==3.0.1
     # via flake8
-pygments==2.14.0
+pygments==2.15.0
     # via mkdocs-material
 pymatgen==2023.3.23
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
 pymatgen-analysis-alloys==0.0.6
     # via emmet-core
 pymatgen-analysis-diffusion==2022.7.21
     # via emmet-core
-pymdown-extensions==9.10
+pymdown-extensions==9.11
     # via
     #   mkdocs-material
     #   mkdocstrings
 pymongo==4.3.3
     # via
     #   maggma
     #   matminer
     #   mongogrant
 pynacl==1.5.0
     # via paramiko
 pyparsing==3.0.9
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
-pytest==7.2.2
+pytest==7.3.1
     # via
     #   emmet-api (setup.py)
     #   pytest-cov
 pytest-cov==4.0.0
     # via emmet-api (setup.py)
 python-dateutil==2.8.2
     # via
@@ -458,17 +453,19 @@
     # via types-requests
 typing-extensions==4.5.0
     # via
     #   aioitertools
     #   bytecode
     #   ddtrace
     #   emmet-core
+    #   mkdocstrings
     #   mp-api
     #   mypy
     #   pydantic
+    #   pydash
     #   starlette
 tzdata==2023.3
     # via pandas
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.15
     # via
```

### Comparing `emmet-api-0.51.9/requirements/ubuntu-latest_py3.9.txt` & `emmet-api-0.52.0/requirements/ubuntu-latest_py3.11.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --output-file=requirements/ubuntu-latest_py3.9.txt --resolver=backtracking
+#    pip-compile --output-file=requirements/ubuntu-latest_py3.11.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.6.2
     # via starlette
 attrs==22.2.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
-boto3==1.26.106
+boto3==1.26.114
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.106
+botocore==1.29.114
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.1
     # via ddtrace
 cattrs==22.2.0
     # via ddtrace
@@ -38,37 +38,35 @@
 click==8.1.3
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
 contourpy==1.0.7
     # via matplotlib
-cryptography==40.0.1
+cryptography==40.0.2
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.11.0
+ddtrace==1.11.2
     # via emmet-api (setup.py)
 deprecated==1.2.13
     # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.50.0
+emmet-core[all]==0.51.13
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
-exceptiongroup==1.1.1
-    # via cattrs
-fastapi==0.95.0
+fastapi==0.95.1
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.2.3
     # via mongogrant
 fonttools==4.39.3
     # via matplotlib
@@ -81,20 +79,16 @@
 h11==0.14.0
     # via uvicorn-tschaume
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.0.1
-    # via
-    #   flask
-    #   opentelemetry-api
-importlib-resources==5.12.0
-    # via matplotlib
-inflect==6.0.2
+    # via opentelemetry-api
+inflect==6.0.4
     # via robocrys
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
 jmespath==1.0.1
     # via
@@ -122,23 +116,23 @@
     # via robocrys
 matplotlib==3.7.1
     # via pymatgen
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
-monty==2022.9.9
+monty==2023.4.10
     # via
     #   emmet-core
     #   maggma
     #   matminer
     #   mp-api
     #   pymatgen
     #   robocrys
-mp-api==0.30.11
+mp-api==0.30.10
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   maggma
     #   mp-api
@@ -158,35 +152,35 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.17.0
     # via ddtrace
-orjson==3.8.9
+orjson==3.8.10
     # via maggma
-packaging==23.0
+packaging==23.1
     # via
     #   ddtrace
     #   matplotlib
     #   mongomock
     #   plotly
-palettable==3.3.0
+palettable==3.3.1
     # via pymatgen
 pandas==2.0.0
     # via
     #   matminer
     #   pymatgen
 paramiko==3.1.0
     # via sshtunnel
 pillow==9.5.0
     # via matplotlib
-plotly==5.14.0
+plotly==5.14.1
     # via pymatgen
-protobuf==4.22.1
+protobuf==4.22.3
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
@@ -197,15 +191,15 @@
     # via cffi
 pydantic==1.10.7
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
-pydash==6.0.2
+pydash==7.0.1
     # via maggma
 pymatgen==2023.3.23
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
@@ -246,16 +240,14 @@
     #   pymatgen
 robocrys==0.2.7
     # via emmet-core
 ruamel-yaml==0.17.21
     # via
     #   pymatgen
     #   robocrys
-ruamel-yaml-clib==0.2.7
-    # via ruamel-yaml
 s3transfer==0.6.0
     # via boto3
 scikit-learn==1.2.2
     # via matminer
 scipy==1.10.1
     # via
     #   pymatgen
@@ -305,21 +297,19 @@
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
 typing-extensions==4.5.0
     # via
-    #   aioitertools
-    #   bytecode
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   pydantic
-    #   starlette
+    #   pydash
 tzdata==2023.3
     # via pandas
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.15
     # via
     #   botocore
@@ -329,13 +319,11 @@
 werkzeug==2.2.3
     # via flask
 wrapt==1.15.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
 zipp==3.15.0
-    # via
-    #   importlib-metadata
-    #   importlib-resources
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.51.9/requirements/ubuntu-latest_py3.9_extras.txt` & `emmet-api-0.52.0/requirements/ubuntu-latest_py3.9_extras.txt`

 * *Files 4% similar despite different names*

```diff
@@ -9,22 +9,21 @@
 anyio==3.6.2
     # via starlette
 attrs==22.2.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
-    #   pytest
 bcrypt==4.0.1
     # via paramiko
-boto3==1.26.106
+boto3==1.26.114
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.106
+botocore==1.29.114
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.1
     # via ddtrace
@@ -46,63 +45,63 @@
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
 colorama==0.4.6
     # via griffe
 contourpy==1.0.7
     # via matplotlib
-coverage[toml]==7.2.2
+coverage[toml]==7.2.3
     # via pytest-cov
-cryptography==40.0.1
+cryptography==40.0.2
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.11.0
+ddtrace==1.11.2
     # via emmet-api (setup.py)
 deprecated==1.2.13
     # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.50.0
+emmet-core[all]==0.51.13
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
     # via
     #   cattrs
     #   pytest
-fastapi==0.95.0
+fastapi==0.95.1
     # via
     #   emmet-api (setup.py)
     #   maggma
-filelock==3.10.7
+filelock==3.11.0
     # via virtualenv
 flake8==6.0.0
     # via emmet-api (setup.py)
 flask==2.2.3
     # via mongogrant
 fonttools==4.39.3
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.26.0
+griffe==0.27.0
     # via mkdocstrings-python
 gunicorn==20.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
     # via uvicorn-tschaume
 htmlmin2==0.1.13
     # via mkdocs-minify-plugin
@@ -116,15 +115,15 @@
     # via
     #   flask
     #   markdown
     #   mkdocs
     #   opentelemetry-api
 importlib-resources==5.12.0
     # via matplotlib
-inflect==6.0.2
+inflect==6.0.4
     # via robocrys
 iniconfig==2.0.0
     # via pytest
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via
@@ -182,53 +181,53 @@
     #   mkdocs-awesome-pages-plugin
     #   mkdocs-markdownextradata-plugin
     #   mkdocs-material
     #   mkdocs-minify-plugin
     #   mkdocstrings
 mkdocs-autorefs==0.4.1
     # via mkdocstrings
-mkdocs-awesome-pages-plugin==2.8.0
+mkdocs-awesome-pages-plugin==2.9.0
     # via emmet-api (setup.py)
 mkdocs-markdownextradata-plugin==0.2.5
     # via emmet-api (setup.py)
 mkdocs-material==8.2.16
     # via emmet-api (setup.py)
 mkdocs-material-extensions==1.1.1
     # via
     #   emmet-api (setup.py)
     #   mkdocs-material
 mkdocs-minify-plugin==0.6.4
     # via emmet-api (setup.py)
-mkdocstrings[python]==0.20.0
+mkdocstrings[python]==0.21.2
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
 mkdocstrings-python==0.9.0
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
-monty==2022.9.9
+monty==2023.4.10
     # via
     #   emmet-core
     #   maggma
     #   matminer
     #   mp-api
     #   pymatgen
     #   robocrys
-mp-api==0.30.11
+mp-api==0.30.10
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   maggma
     #   mp-api
-mypy==1.1.1
+mypy==1.2.0
     # via emmet-api (setup.py)
 mypy-extensions==1.0.0
     # via
     #   emmet-api (setup.py)
     #   mypy
 natsort==8.3.1
     # via mkdocs-awesome-pages-plugin
@@ -250,43 +249,43 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.17.0
     # via ddtrace
-orjson==3.8.9
+orjson==3.8.10
     # via maggma
-packaging==23.0
+packaging==23.1
     # via
     #   ddtrace
     #   matplotlib
     #   mkdocs
     #   mongomock
     #   plotly
     #   pytest
-palettable==3.3.0
+palettable==3.3.1
     # via pymatgen
 pandas==2.0.0
     # via
     #   matminer
     #   pymatgen
 paramiko==3.1.0
     # via sshtunnel
 pillow==9.5.0
     # via matplotlib
 platformdirs==3.2.0
     # via virtualenv
-plotly==5.14.0
+plotly==5.14.1
     # via pymatgen
 pluggy==1.0.0
     # via pytest
 pre-commit==3.2.2
     # via emmet-api (setup.py)
-protobuf==4.22.1
+protobuf==4.22.3
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
@@ -301,50 +300,50 @@
     # via cffi
 pydantic==1.10.7
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
-pydash==6.0.2
+pydash==7.0.1
     # via maggma
 pydocstyle==6.3.0
     # via emmet-api (setup.py)
 pyflakes==3.0.1
     # via flake8
-pygments==2.14.0
+pygments==2.15.0
     # via mkdocs-material
 pymatgen==2023.3.23
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
 pymatgen-analysis-alloys==0.0.6
     # via emmet-core
 pymatgen-analysis-diffusion==2022.7.21
     # via emmet-core
-pymdown-extensions==9.10
+pymdown-extensions==9.11
     # via
     #   mkdocs-material
     #   mkdocstrings
 pymongo==4.3.3
     # via
     #   maggma
     #   matminer
     #   mongogrant
 pynacl==1.5.0
     # via paramiko
 pyparsing==3.0.9
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
-pytest==7.2.2
+pytest==7.3.1
     # via
     #   emmet-api (setup.py)
     #   pytest-cov
 pytest-cov==4.0.0
     # via emmet-api (setup.py)
 python-dateutil==2.8.2
     # via
@@ -454,17 +453,19 @@
     # via types-requests
 typing-extensions==4.5.0
     # via
     #   aioitertools
     #   bytecode
     #   ddtrace
     #   emmet-core
+    #   mkdocstrings
     #   mp-api
     #   mypy
     #   pydantic
+    #   pydash
     #   starlette
 tzdata==2023.3
     # via pandas
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.15
     # via
```

### Comparing `emmet-api-0.51.9/setup.py` & `emmet-api-0.52.0/setup.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/tests/_consumer/test_query_operators.py` & `emmet-api-0.52.0/tests/_consumer/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/tests/_general_store/test_query_operators.py` & `emmet-api-0.52.0/tests/_general_store/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/tests/bonds/test_query_operators.py` & `emmet-api-0.52.0/tests/materials/bonds/test_query_operators.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from emmet.api.routes.bonds.query_operators import (
+from emmet.api.routes.materials.bonds.query_operators import (
     BondLengthQuery,
     CoordinationEnvsQuery,
 )
 
 from monty.tempfile import ScratchDir
 from monty.serialization import loadfn, dumpfn
```

### Comparing `emmet-api-0.51.9/tests/charge_density/test_query_operators.py` & `emmet-api-0.52.0/tests/materials/charge_density/test_query_operators.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from emmet.api.routes.charge_density.query_operators import ChgcarTaskIDQuery
+from emmet.api.routes.materials.charge_density.query_operators import ChgcarTaskIDQuery
 from monty.tempfile import ScratchDir
 from monty.serialization import loadfn, dumpfn
 
 
 def test_chgcar_test_id_query():
     op = ChgcarTaskIDQuery()
```

### Comparing `emmet-api-0.51.9/tests/chemenv/test_query_operators.py` & `emmet-api-0.52.0/tests/materials/chemenv/test_query_operators.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from emmet.api.routes.chemenv.query_operators import ChemEnvQuery
+from emmet.api.routes.materials.chemenv.query_operators import ChemEnvQuery
 
 from monty.tempfile import ScratchDir
 from monty.serialization import loadfn, dumpfn
 
 
 def test_bond_length_query_operator():
     op = ChemEnvQuery()
```

### Comparing `emmet-api-0.51.9/tests/core/test_mapi.py` & `emmet-api-0.52.0/tests/core/test_mapi.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.9/tests/dielectric/test_query_operators.py` & `emmet-api-0.52.0/tests/materials/dielectric/test_query_operators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from maggma.api import query_operator
-from emmet.api.routes.dielectric.query_operators import DielectricQuery
+from emmet.api.routes.materials.dielectric.query_operators import DielectricQuery
 
 from monty.tempfile import ScratchDir
 from monty.serialization import loadfn, dumpfn
 
 
 def test_dielectric_query_operator():
     op = DielectricQuery()
```

### Comparing `emmet-api-0.51.9/tests/elasticity/test_query_operators.py` & `emmet-api-0.52.0/tests/materials/elasticity/test_query_operators.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from emmet.api.routes.elasticity.query_operators import (
+from emmet.api.routes.materials.elasticity.query_operators import (
     BulkModulusQuery,
     ShearModulusQuery,
     PoissonQuery,
     ElasticityChemsysQuery,
 )
 
 from monty.tempfile import ScratchDir
```

### Comparing `emmet-api-0.51.9/tests/electrodes/test_query_operators.py` & `emmet-api-0.52.0/tests/materials/electrodes/test_query_operators.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from emmet.api.routes.electrodes.query_operators import (
+from emmet.api.routes.materials.electrodes.query_operators import (
     ElectrodeFormulaQuery,
     ElectrodesChemsysQuery,
     ElectrodeElementsQuery,
     VoltageStepQuery,
     InsertionVoltageStepQuery,
     WorkingIonQuery,
     ElectrodeMultiMaterialIDQuery,
```

### Comparing `emmet-api-0.51.9/tests/electrodes/test_utils.py` & `emmet-api-0.52.0/tests/materials/electrodes/test_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from emmet.api.routes.electrodes.utils import (
+from emmet.api.routes.materials.electrodes.utils import (
     electrodes_chemsys_to_criteria,
     electrodes_formula_to_criteria,
 )
 import pytest
 
 
 def test_electrodes_formula_to_criteria():
```

### Comparing `emmet-api-0.51.9/tests/electronic_structure/test_query_operators.py` & `emmet-api-0.52.0/tests/materials/electronic_structure/test_query_operators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from monty.tempfile import ScratchDir
 from monty.serialization import loadfn, dumpfn
 from pymatgen.electronic_structure.core import OrbitalType
 
-from emmet.api.routes.electronic_structure.query_operators import (
+from emmet.api.routes.materials.electronic_structure.query_operators import (
     ESSummaryDataQuery,
     BSDataQuery,
     DOSDataQuery,
     ObjectQuery,
 )
 from emmet.core.electronic_structure import (
     BSPathType,
```

### Comparing `emmet-api-0.51.9/tests/grain_boundary/test_query_operators.py` & `emmet-api-0.52.0/tests/materials/grain_boundary/test_query_operators.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from monty.tempfile import ScratchDir
 from monty.serialization import loadfn, dumpfn
 
-from emmet.api.routes.grain_boundary.query_operators import (
+from emmet.api.routes.materials.grain_boundary.query_operators import (
     GBStructureQuery,
     GBTaskIDQuery,
 )
 from emmet.core.grain_boundary import GBTypeEnum
 
 
 def test_grain_boundary_structure_query():
```

### Comparing `emmet-api-0.51.9/tests/magnetism/test_query_operators.py` & `emmet-api-0.52.0/tests/materials/magnetism/test_query_operators.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from emmet.api.routes.magnetism.query_operators import MagneticQuery
+from emmet.api.routes.materials.magnetism.query_operators import MagneticQuery
 
 from pymatgen.analysis.magnetism import Ordering
 
 from monty.tempfile import ScratchDir
 from monty.serialization import loadfn, dumpfn
```

### Comparing `emmet-api-0.51.9/tests/materials/test_query_operators.py` & `emmet-api-0.52.0/tests/materials/materials/test_query_operators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 
 from emmet.api.core.settings import MAPISettings
-from emmet.api.routes.materials.query_operators import (
+from emmet.api.routes.materials.materials.query_operators import (
     FormulaQuery,
     ChemsysQuery,
     ElementsQuery,
     DeprecationQuery,
     SymmetryQuery,
     MultiTaskIDQuery,
     MultiMaterialIDQuery,
```

### Comparing `emmet-api-0.51.9/tests/materials/test_utils.py` & `emmet-api-0.52.0/tests/materials/materials/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from emmet.api.routes.materials.utils import formula_to_criteria, chemsys_to_criteria
+from emmet.api.routes.materials.materials.utils import formula_to_criteria, chemsys_to_criteria
 import pytest
 
 
 def test_formula_to_criteria():
     # Regular formula
     assert formula_to_criteria("Cr2O3") == {
         "composition_reduced.Cr": 2.0,
```

### Comparing `emmet-api-0.51.9/tests/molecules/test_query_operators.py` & `emmet-api-0.52.0/tests/legacy/molecules/test_query_operators.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from monty.tempfile import ScratchDir
 from monty.serialization import loadfn, dumpfn
 
-from emmet.api.routes.molecules.query_operators import (
+from emmet.api.routes.legacy.jcesr.query_operators import (
     MoleculeBaseQuery,
     MoleculeElementsQuery,
     MoleculeFormulaQuery,
 )
 
 
 def test_molecule_elements_query():
```

### Comparing `emmet-api-0.51.9/tests/mpcomplete/test_query_operators.py` & `emmet-api-0.52.0/tests/materials/mpcomplete/test_query_operators.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from emmet.api.routes.mpcomplete.query_operator import (
+from emmet.api.routes.materials.mpcomplete.query_operator import (
     MPCompleteGetQuery,
     MPCompletePostQuery,
 )
 from emmet.api.core.settings import MAPISettings
 
 from pymatgen.core.structure import Structure
```

### Comparing `emmet-api-0.51.9/tests/mpcules/bonds/test_query_operators.py` & `emmet-api-0.52.0/tests/molecules/bonds/test_query_operators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from emmet.api.routes.mpcules.bonds.query_operators import (
+from emmet.api.routes.molecules.bonds.query_operators import (
     BondTypeLengthQuery
 )
 from monty.tempfile import ScratchDir
 from monty.serialization import loadfn, dumpfn
 
 
 def test_bond_type_length_query():
```

### Comparing `emmet-api-0.51.9/tests/mpcules/molecules/test_query_operators.py` & `emmet-api-0.52.0/tests/molecules/molecules/test_query_operators.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import os
 
 from emmet.api.core.settings import MAPISettings
-from emmet.api.routes.mpcules.molecules.query_operators import (
+from emmet.api.routes.molecules.molecules.query_operators import (
     FormulaQuery,
     ChemsysQuery,
     ElementsQuery,
     ChargeSpinQuery,
     DeprecationQuery,
     MultiTaskIDQuery,
     MultiMPculeIDQuery,
     FindMoleculeQuery,
-    FindMoleculeConnectivityQuery,
     CalcMethodQuery,
     HashQuery,
 )
 from monty.tempfile import ScratchDir
 from monty.serialization import loadfn, dumpfn
 
 from pymatgen.core.structure import Molecule
@@ -101,30 +100,30 @@
         assert new_op.query(task_ids="mpcule-149, mpcule-13") == {
             "criteria": {"task_ids": {"$in": ["mpcule-149", "mpcule-13"]}}
         }
 
 
 def test_multi_mpculeid_query():
     op = MultiMPculeIDQuery()
-    assert op.query(mpcule_ids="21d752f3018fd3c4eba7a9ce7a37b8c8-C1F1Mg1N1O1S2-1-2, 542d9adc3163002fe8dfe6d226875dde-C3H5Li2O3-0-2") == {
+    assert op.query(molecule_ids="21d752f3018fd3c4eba7a9ce7a37b8c8-C1F1Mg1N1O1S2-1-2, 542d9adc3163002fe8dfe6d226875dde-C3H5Li2O3-0-2") == {
         "criteria": {"molecule_id": {"$in": ["21d752f3018fd3c4eba7a9ce7a37b8c8-C1F1Mg1N1O1S2-1-2", "542d9adc3163002fe8dfe6d226875dde-C3H5Li2O3-0-2"]}}
     }
 
-    assert op.query(mpcule_ids="21d752f3018fd3c4eba7a9ce7a37b8c8-C1F1Mg1N1O1S2-1-2") == {
+    assert op.query(molecule_ids="21d752f3018fd3c4eba7a9ce7a37b8c8-C1F1Mg1N1O1S2-1-2") == {
         "criteria": {"molecule_id": "21d752f3018fd3c4eba7a9ce7a37b8c8-C1F1Mg1N1O1S2-1-2"}
     }
 
     with ScratchDir("."):
         dumpfn(op, "temp.json")
         new_op = loadfn("temp.json")
-        assert new_op.query(mpcule_ids="21d752f3018fd3c4eba7a9ce7a37b8c8-C1F1Mg1N1O1S2-1-2, 542d9adc3163002fe8dfe6d226875dde-C3H5Li2O3-0-2") == {
+        assert new_op.query(molecule_ids="21d752f3018fd3c4eba7a9ce7a37b8c8-C1F1Mg1N1O1S2-1-2, 542d9adc3163002fe8dfe6d226875dde-C3H5Li2O3-0-2") == {
            "criteria": {"molecule_id": {"$in": ["21d752f3018fd3c4eba7a9ce7a37b8c8-C1F1Mg1N1O1S2-1-2", "542d9adc3163002fe8dfe6d226875dde-C3H5Li2O3-0-2"]}}
         }
 
-        assert op.query(mpcule_ids="21d752f3018fd3c4eba7a9ce7a37b8c8-C1F1Mg1N1O1S2-1-2") == {
+        assert op.query(molecule_ids="21d752f3018fd3c4eba7a9ce7a37b8c8-C1F1Mg1N1O1S2-1-2") == {
             "criteria": {"molecule_id": "21d752f3018fd3c4eba7a9ce7a37b8c8-C1F1Mg1N1O1S2-1-2"}
         }
 
 
 def test_find_molecule_query():
     op = FindMoleculeQuery()
 
@@ -147,39 +146,14 @@
     docs = [{"molecule": mol.as_dict(), "molecule_id": "f9eff23899e37989eb800214ea1d54d4-C1F4Li1O3P1-0-1"}]
 
     pp = op.post_process(docs, query)[0]
     assert pp["molecule_id"] == "f9eff23899e37989eb800214ea1d54d4-C1F4Li1O3P1-0-1"
     assert pp["rmsd"] < 1e-15
 
 
-def test_find_molecule_connectivity_query():
-    op = FindMoleculeConnectivityQuery()
-
-    mol = Molecule.from_file(
-        os.path.join(MAPISettings().TEST_FILES, "test_molecule.xyz")
-    )
-
-    query = {
-        "criteria": {"composition": dict(mol.composition),
-                     "charge": int(mol.charge),
-                     "spin_multiplicity": int(mol.spin_multiplicity)
-                     }
-    }
-    assert (
-        op.query(
-            molecule=mol.as_dict(), charge=0, spin_multiplicity=1, _limit=1
-        )
-        == query
-    )
-
-    docs = [{"molecule": mol.as_dict(), "molecule_id": "f9eff23899e37989eb800214ea1d54d4-C1F4Li1O3P1-0-1"}]
-    pp = op.post_process(docs, query)[0]
-    assert pp["molecule_id"] == "f9eff23899e37989eb800214ea1d54d4-C1F4Li1O3P1-0-1"
-
-
 def test_calc_method_query():
     op = CalcMethodQuery()
 
     assert op.query(level_of_theory="wB97X-V/def2-TZVPPD/SMD", solvent="SOLVENT=THF", lot_solvent="wB97X-V/def2-TZVPPD/SMD(SOLVENT=THF)") == {
         "criteria": {
             "unique_levels_of_theory": "wB97X-V/def2-TZVPPD/SMD",
             "unique_lot_solvents": "wB97X-V/def2-TZVPPD/SMD(SOLVENT=THF)",
```

### Comparing `emmet-api-0.51.9/tests/mpcules/orbitals/test_query_operators.py` & `emmet-api-0.52.0/tests/molecules/orbitals/test_query_operators.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,127 +1,119 @@
-from emmet.api.routes.mpcules.orbitals.query_operators import (
+from emmet.api.routes.molecules.orbitals.query_operators import (
     NBOPopulationQuery,
     NBOLonePairQuery,
     NBOBondQuery,
     NBOInteractionQuery
 )
 from monty.tempfile import ScratchDir
 from monty.serialization import loadfn, dumpfn
 
 
 def test_nbo_population_query():
     op = NBOPopulationQuery()
     assert op.query(
-        open_shell=True,
-        electron_type="beta",
-        min_core_electron=10.0,
-        max_core_electron=11.0,
-        min_valence_electron=0.0,
-        max_valence_electron=2.0,
-        min_rydberg_electron=0.0,
-        max_rydberg_electron=1.0,
-        min_total_electron=11.0,
-        max_total_electron=12.0
+        electron_type_population="beta",
+        min_core_electrons=10.0,
+        max_core_electrons=11.0,
+        min_valence_electrons=0.0,
+        max_valence_electrons=2.0,
+        min_rydberg_electrons=0.0,
+        max_rydberg_electrons=1.0,
+        min_total_electrons=11.0,
+        max_total_electrons=12.0
     ) == {
         'criteria': {
-            'open_shell': True,
             'beta_population.core_electrons': {'$gte': 10.0, '$lte': 11.0},
             'beta_population.valence_electrons': {'$gte': 0.0, '$lte': 2.0},
             'beta_population.rydberg_electrons': {'$gte': 0.0, '$lte': 1.0},
             'beta_population.total_electrons': {'$gte': 11.0, '$lte': 12.0}
         }
     }
 
     with ScratchDir("."):
         dumpfn(op, "temp.json")
         new_op = loadfn("temp.json")
         assert new_op.query(
-            open_shell=True, 
-            electron_type="beta",
-            min_core_electron=10.0,
-            max_core_electron=11.0,
-            min_valence_electron=0.0,
-            max_valence_electron=2.0,
-            min_rydberg_electron=0.0,
-            max_rydberg_electron=1.0,
-            min_total_electron=11.0,
-            max_total_electron=12.0
+            electron_type_population="beta",
+            min_core_electrons=10.0,
+            max_core_electrons=11.0,
+            min_valence_electrons=0.0,
+            max_valence_electrons=2.0,
+            min_rydberg_electrons=0.0,
+            max_rydberg_electrons=1.0,
+            min_total_electrons=11.0,
+            max_total_electrons=12.0
         ) == {
             'criteria': {
-                'open_shell': True,
                 'beta_population.core_electrons': {'$gte': 10.0, '$lte': 11.0},
                 'beta_population.valence_electrons': {'$gte': 0.0, '$lte': 2.0},
                 'beta_population.rydberg_electrons': {'$gte': 0.0, '$lte': 1.0},
                 'beta_population.total_electrons': {'$gte': 11.0, '$lte': 12.0}
             }
         }
 
 
 def test_nbo_lone_pair_query():
     op = NBOLonePairQuery()
     assert op.query(
-        open_shell=True,
-        electron_type="alpha",
+        electron_type_lp="alpha",
         lp_type="LP",
         min_s_character=10.0,
         max_s_character=25.0,
         min_p_character=70.0,
         max_p_character=90.0,
         min_d_character=0.0,
         max_d_character=5.0,
         min_f_character=0.0,
         max_f_character=5.0,
-        min_occupancy=1.5,
-        max_occupancy=2.0
+        min_lp_occupancy=1.5,
+        max_lp_occupancy=2.0
     ) == {
         'criteria': {
-            'open_shell': True,
             'alpha_lone_pairs.s_character': {'$gte': 10.0, '$lte': 25.0},
             'alpha_lone_pairs.p_character': {'$gte': 70.0, '$lte': 90.0},
             'alpha_lone_pairs.d_character': {'$gte': 0.0, '$lte': 5.0},
             'alpha_lone_pairs.f_character': {'$gte': 0.0, '$lte': 5.0},
             'alpha_lone_pairs.occupancy': {'$gte': 1.5, '$lte': 2.0},
             'alpha_lone_pairs.type_code': 'LP'
         }
     }
 
     with ScratchDir("."):
         dumpfn(op, "temp.json")
         new_op = loadfn("temp.json")
         assert new_op.query(
-            open_shell=True,
-            electron_type="alpha",
+            electron_type_lp="alpha",
             lp_type="LP",
             min_s_character=10.0,
             max_s_character=25.0,
             min_p_character=70.0,
             max_p_character=90.0,
             min_d_character=0.0,
             max_d_character=5.0,
             min_f_character=0.0,
             max_f_character=5.0,
-            min_occupancy=1.5,
-            max_occupancy=2.0
+            min_lp_occupancy=1.5,
+            max_lp_occupancy=2.0
         ) == {
             'criteria': {
-                'open_shell': True,
                 'alpha_lone_pairs.s_character': {'$gte': 10.0, '$lte': 25.0},
                 'alpha_lone_pairs.p_character': {'$gte': 70.0, '$lte': 90.0},
                 'alpha_lone_pairs.d_character': {'$gte': 0.0, '$lte': 5.0},
                 'alpha_lone_pairs.f_character': {'$gte': 0.0, '$lte': 5.0},
                 'alpha_lone_pairs.occupancy': {'$gte': 1.5, '$lte': 2.0},
                 'alpha_lone_pairs.type_code': 'LP'
             }
         }
 
 
 def test_nbo_bond_query():
     op = NBOBondQuery()
     assert op.query(
-        open_shell=False,
+        electron_type_bond=None,
         bond_type="BD*",
         min_s_character_atom1=10.0,
         max_s_character_atom1=25.0,
         min_s_character_atom2=10.0,
         max_s_character_atom2=25.0,
         min_p_character_atom1=70.0,
         max_p_character_atom1=90.0,
@@ -135,19 +127,18 @@
         max_f_character_atom1=5.0,
         min_f_character_atom2=0.0,
         max_f_character_atom2=5.0,
         min_polarization_atom1=30.0,
         max_polarization_atom1=70.0,
         min_polarization_atom2=30.0,
         max_polarization_atom2=70.0,
-        min_occupancy=0.0,
-        max_occupancy=1.0
+        min_bond_occupancy=0.0,
+        max_bond_occupancy=1.0
     ) == {
         'criteria': {
-            'open_shell': False,
             'nbo_bonds.atom1_s_character': {'$gte': 10.0, '$lte': 25.0},
             'nbo_bonds.atom1_p_character': {'$gte': 70.0, '$lte': 90.0},
             'nbo_bonds.atom1_d_character': {'$gte': 0.0, '$lte': 5.0},
             'nbo_bonds.atom1_f_character': {'$gte': 0.0, '$lte': 5.0},
             'nbo_bonds.atom2_s_character': {'$gte': 10.0, '$lte': 25.0},
             'nbo_bonds.atom2_p_character': {'$gte': 70.0, '$lte': 90.0},
             'nbo_bonds.atom2_d_character': {'$gte': 0.0, '$lte': 5.0},
@@ -159,15 +150,15 @@
         }
     }
 
     with ScratchDir("."):
         dumpfn(op, "temp.json")
         new_op = loadfn("temp.json")
         assert new_op.query(
-            open_shell=False,
+            electron_type_bond=None,
             bond_type="BD*",
             min_s_character_atom1=10.0,
             max_s_character_atom1=25.0,
             min_s_character_atom2=10.0,
             max_s_character_atom2=25.0,
             min_p_character_atom1=70.0,
             max_p_character_atom1=90.0,
@@ -181,19 +172,18 @@
             max_f_character_atom1=5.0,
             min_f_character_atom2=0.0,
             max_f_character_atom2=5.0,
             min_polarization_atom1=30.0,
             max_polarization_atom1=70.0,
             min_polarization_atom2=30.0,
             max_polarization_atom2=70.0,
-            min_occupancy=0.0,
-            max_occupancy=1.0
+            min_bond_occupancy=0.0,
+            max_bond_occupancy=1.0
         ) == {
             'criteria': {
-                'open_shell': False,
                 'nbo_bonds.atom1_s_character': {'$gte': 10.0, '$lte': 25.0},
                 'nbo_bonds.atom1_p_character': {'$gte': 70.0, '$lte': 90.0},
                 'nbo_bonds.atom1_d_character': {'$gte': 0.0, '$lte': 5.0},
                 'nbo_bonds.atom1_f_character': {'$gte': 0.0, '$lte': 5.0},
                 'nbo_bonds.atom2_s_character': {'$gte': 10.0, '$lte': 25.0},
                 'nbo_bonds.atom2_p_character': {'$gte': 70.0, '$lte': 90.0},
                 'nbo_bonds.atom2_d_character': {'$gte': 0.0, '$lte': 5.0},
@@ -205,52 +195,48 @@
             }
         }
 
 
 def test_nbo_interaction_query():
     op = NBOInteractionQuery()
     assert op.query(
-        open_shell=True,
-        electron_type="alpha",
+        electron_type_interaction="alpha",
         donor_type="LP",
         acceptor_type="RY",
         min_perturbation_energy=0.1,
         max_perturbation_energy=3.0,
         min_energy_difference=2.0,
         max_energy_difference=15.0,
         min_fock_element=0.0,
         max_fock_element=10.0
     ) == {
         'criteria': {
-            'open_shell': True,
             'alpha_interactions.perturbation_energy': {'$gte': 0.1, '$lte': 3.0},
             'alpha_interactions.energy_difference': {'$gte': 2.0, '$lte': 15.0},
             'alpha_interactions.fock_element': {'$gte': 0.0, '$lte': 10.0},
             'alpha_interactions.donor_type': 'LP',
             'alpha_interactions.acceptor_type': 'RY'
         }
     }
 
     with ScratchDir("."):
         dumpfn(op, "temp.json")
         new_op = loadfn("temp.json")
         assert new_op.query(
-            open_shell=True,
-            electron_type="alpha",
+            electron_type_interaction="alpha",
             donor_type="LP",
             acceptor_type="RY",
             min_perturbation_energy=0.1,
             max_perturbation_energy=3.0,
             min_energy_difference=2.0,
             max_energy_difference=15.0,
             min_fock_element=0.0,
             max_fock_element=10.0
         ) == {
             'criteria': {
-                'open_shell': True,
                 'alpha_interactions.perturbation_energy': {'$gte': 0.1, '$lte': 3.0},
                 'alpha_interactions.energy_difference': {'$gte': 2.0, '$lte': 15.0},
                 'alpha_interactions.fock_element': {'$gte': 0.0, '$lte': 10.0},
                 'alpha_interactions.donor_type': 'LP',
                 'alpha_interactions.acceptor_type': 'RY'
             }
         }
```

### Comparing `emmet-api-0.51.9/tests/mpcules/redox/test_query_operators.py` & `emmet-api-0.52.0/tests/molecules/redox/test_query_operators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from emmet.api.routes.mpcules.redox.query_operators import (
+from emmet.api.routes.molecules.redox.query_operators import (
     RedoxPotentialQuery
 )
 from monty.tempfile import ScratchDir
 from monty.serialization import loadfn, dumpfn
 
 
 def test_redox_potential_query():
```

### Comparing `emmet-api-0.51.9/tests/mpcules/summary/test_query_operators.py` & `emmet-api-0.52.0/tests/molecules/summary/test_query_operators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from monty.tempfile import ScratchDir
 from monty.serialization import loadfn, dumpfn
 
-from emmet.api.routes.mpcules.summary.query_operators import (
+from emmet.api.routes.molecules.summary.query_operators import (
     MPculeIDsSearchQuery
 )
 
 
 def test_mpcules_ids_query():
     op = MPculeIDsSearchQuery()
```

### Comparing `emmet-api-0.51.9/tests/mpcules/tasks/test_query_operators.py` & `emmet-api-0.52.0/tests/molecules/tasks/test_query_operators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from emmet.api.routes.mpcules.tasks.query_operators import (
+from emmet.api.routes.molecules.tasks.query_operators import (
     MultipleTaskIDsQuery,
     # TrajectoryQuery,
     DeprecationQuery,
     # EntryQuery,
 )
 from emmet.api.core.settings import MAPISettings
```

### Comparing `emmet-api-0.51.9/tests/mpcules/thermo/test_query_operators.py` & `emmet-api-0.52.0/tests/molecules/thermo/test_query_operators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from emmet.api.routes.mpcules.thermo.query_operators import (
+from emmet.api.routes.molecules.thermo.query_operators import (
     ThermoCorrectionQuery
 )
 from monty.tempfile import ScratchDir
 from monty.serialization import loadfn, dumpfn
 
 
 def test_thermo_correction_query():
```

### Comparing `emmet-api-0.51.9/tests/oxidation_states/test_query_operators.py` & `emmet-api-0.52.0/tests/materials/oxidation_states/test_query_operators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from emmet.api.routes.oxidation_states.query_operators import PossibleOxiStateQuery
+from emmet.api.routes.materials.oxidation_states.query_operators import PossibleOxiStateQuery
 
 from monty.tempfile import ScratchDir
 from monty.serialization import loadfn, dumpfn
 
 
 def test_possible_oxi_state_query():
     op = PossibleOxiStateQuery()
```

### Comparing `emmet-api-0.51.9/tests/piezo/test_query_operators.py` & `emmet-api-0.52.0/tests/materials/piezo/test_query_operators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from emmet.api.routes.piezo.query_operators import PiezoelectricQuery
+from emmet.api.routes.materials.piezo.query_operators import PiezoelectricQuery
 
 from monty.tempfile import ScratchDir
 from monty.serialization import loadfn, dumpfn
 
 
 def test_piezo_query():
     op = PiezoelectricQuery()
```

### Comparing `emmet-api-0.51.9/tests/robocrys/test_query_operators.py` & `emmet-api-0.52.0/tests/materials/robocrys/test_query_operators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from emmet.api.routes.robocrys.query_operators import RoboTextSearchQuery
+from emmet.api.routes.materials.robocrys.query_operators import RoboTextSearchQuery
 from monty.tempfile import ScratchDir
 from monty.serialization import loadfn, dumpfn
 
 
 def test_robocrys_search_query():
     op = RoboTextSearchQuery()
```

### Comparing `emmet-api-0.51.9/tests/substrates/test_query_operators.py` & `emmet-api-0.52.0/tests/materials/substrates/test_query_operators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from emmet.api.routes.substrates.query_operators import (
+from emmet.api.routes.materials.substrates.query_operators import (
     SubstrateStructureQuery,
     EnergyAreaQuery,
 )
 
 
 from monty.tempfile import ScratchDir
 from monty.serialization import loadfn, dumpfn
```

### Comparing `emmet-api-0.51.9/tests/summary/test_query_operators.py` & `emmet-api-0.52.0/tests/materials/summary/test_query_operators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from monty.tempfile import ScratchDir
 from monty.serialization import loadfn, dumpfn
 
-from emmet.api.routes.summary.query_operators import (
+from emmet.api.routes.materials.summary.query_operators import (
     HasPropsQuery,
     MaterialIDsSearchQuery,
     SearchHasReconstructedQuery,
     SearchIsStableQuery,
     SearchMagneticQuery,
     SearchIsTheoreticalQuery,
     SearchStatsQuery,
```

### Comparing `emmet-api-0.51.9/tests/surface_properties/test_query_operators.py` & `emmet-api-0.52.0/tests/materials/surface_properties/test_query_operators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from emmet.api.routes.surface_properties.query_operators import ReconstructedQuery
+from emmet.api.routes.materials.surface_properties.query_operators import ReconstructedQuery
 
 
 from monty.tempfile import ScratchDir
 from monty.serialization import loadfn, dumpfn
 
 
 def test_reconstructed_operator():
```

### Comparing `emmet-api-0.51.9/tests/synthesis/test_adaptor_synpro.py` & `emmet-api-0.52.0/tests/materials/synthesis/test_adaptor_synpro.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from json import load
 
 from pymatgen.core import Composition
 
 from emmet.api.core.settings import MAPISettings
-from emmet.api.routes.synthesis.data_adaptor_synpro import (
+from emmet.api.routes.materials.synthesis.data_adaptor_synpro import (
     convert_value,
     convert_conditions,
     convert_one,
     get_material_formula,
 )
```

### Comparing `emmet-api-0.51.9/tests/synthesis/test_query_operators.py` & `emmet-api-0.52.0/tests/materials/synthesis/test_query_operators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from emmet.api.routes.synthesis.query_operators import SynthesisSearchQuery
+from emmet.api.routes.materials.synthesis.query_operators import SynthesisSearchQuery
 from emmet.core.synthesis import SynthesisTypeEnum, OperationTypeEnum
 
 from monty.tempfile import ScratchDir
 from monty.serialization import loadfn, dumpfn
 
 
 def test_synthesis_search_query():
```

### Comparing `emmet-api-0.51.9/tests/synthesis/test_utils.py` & `emmet-api-0.52.0/tests/materials/synthesis/test_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 from json import load
-from emmet.api.routes.synthesis.utils import (
+from emmet.api.routes.materials.synthesis.utils import (
     make_ellipsis,
     mask_paragraphs,
     mask_highlights,
 )
 from emmet.api.core.settings import MAPISettings
 from emmet.core.synthesis import SynthesisSearchResultModel
```

### Comparing `emmet-api-0.51.9/tests/tasks/test_query_operators.py` & `emmet-api-0.52.0/tests/materials/tasks/test_query_operators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from emmet.api.routes.tasks.query_operators import (
+from emmet.api.routes.materials.tasks.query_operators import (
     MultipleTaskIDsQuery,
     TrajectoryQuery,
     DeprecationQuery,
     EntryQuery,
 )
 from emmet.api.core.settings import MAPISettings
```

### Comparing `emmet-api-0.51.9/tests/tasks/test_utils.py` & `emmet-api-0.52.0/tests/materials/tasks/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from json import load
 
 from emmet.api.core.settings import MAPISettings
-from emmet.api.routes.tasks.utils import calcs_reversed_to_trajectory, task_to_entry
+from emmet.api.routes.materials.tasks.utils import calcs_reversed_to_trajectory, task_to_entry
 
 
 def test_calcs_reversed_to_trajectory():
     with open(
         os.path.join(MAPISettings().TEST_FILES, "calcs_reversed_mp_1031016.json")
     ) as file:
         calcs_reversed = load(file)
```

### Comparing `emmet-api-0.51.9/tests/xas/test_query_operators.py` & `emmet-api-0.52.0/tests/materials/xas/test_query_operators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from emmet.api.routes.xas.query_operators import XASQuery, XASTaskIDQuery
+from emmet.api.routes.materials.xas.query_operators import XASQuery, XASTaskIDQuery
 
 from monty.tempfile import ScratchDir
 from monty.serialization import loadfn, dumpfn
 
 from emmet.core.xas import Edge, Type
 from pymatgen.core.periodic_table import Element
```


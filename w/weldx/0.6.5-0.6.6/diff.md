# Comparing `tmp/weldx-0.6.5.tar.gz` & `tmp/weldx-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weldx-0.6.5.tar", last modified: Thu Apr  6 15:27:24 2023, max compression
+gzip compressed data, was "weldx-0.6.6.tar", last modified: Wed Apr 19 08:18:04 2023, max compression
```

## Comparing `weldx-0.6.5.tar` & `weldx-0.6.6.tar`

### file list

```diff
@@ -1,280 +1,280 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.081606 weldx-0.6.5/
--rw-r--r--   0 runner    (1001) docker     (123)    40717 2023-04-06 15:27:00.000000 weldx-0.6.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-06 15:27:00.000000 weldx-0.6.5/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-06 15:27:00.000000 weldx-0.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-06 15:27:00.000000 weldx-0.6.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-04-06 15:27:24.081606 weldx-0.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-04-06 15:27:00.000000 weldx-0.6.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-04-06 15:27:00.000000 weldx-0.6.5/RELEASE.md
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-06 15:27:00.000000 weldx-0.6.5/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-06 15:27:00.000000 weldx-0.6.5/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-04-06 15:27:00.000000 weldx-0.6.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 15:27:24.081606 weldx-0.6.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.049605 weldx-0.6.5/weldx/
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-06 15:27:23.000000 weldx-0.6.5/weldx/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.049605 weldx-0.6.5/weldx/asdf/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/asdf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.049605 weldx-0.6.5/weldx/asdf/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/asdf/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10850 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/asdf/cli/welding_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/asdf/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/asdf/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)    35535 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/asdf/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/asdf/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    23452 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/asdf/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    18813 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/asdf/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.049605 weldx-0.6.5/weldx/core/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34598 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/core/generic_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     8174 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/core/math_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/core/spatial_series.py
--rw-r--r--   0 runner    (1001) docker     (123)    16188 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/core/time_series.py
--rw-r--r--   0 runner    (1001) docker     (123)    92765 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.049605 weldx-0.6.5/weldx/manifests/
--rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/manifests/weldx-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/manifests/weldx-0.1.1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/manifests/weldx-0.1.2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    37433 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/measurement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.041604 weldx-0.6.5/weldx/schemas/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.041604 weldx-0.6.5/weldx/schemas/weldx.bam.de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.049605 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.041604 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/aws/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.053605 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/aws/design/
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/aws/design/base_metal-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/aws/design/connection-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/aws/design/joint_penetration-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/aws/design/sub_assembly-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/aws/design/weld_details-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/aws/design/weldment-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/aws/design/workpiece-0.1.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.053605 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/aws/process/
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/aws/process/arc_welding_process-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/aws/process/gas_component-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/aws/process/shielding_gas_for_procedure-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/aws/process/shielding_gas_type-0.1.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.053605 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/data_array-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/dataset-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/dimension-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/file-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/file-0.1.1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/generic_series-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/generic_series_free_dimension-0.1.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.053605 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/geometry/spatial_data-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/geometry/spatial_data-0.1.1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.057605 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/graph/di_edge-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/graph/di_graph-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/graph/di_node-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/mathematical_expression-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/media_file-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/time_series-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/time_series-0.1.1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.057605 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/transformations/
--rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/transformations/coordinate_system_hierarchy-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/transformations/local_coordinate_system-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/transformations/local_coordinate_system-0.1.1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/transformations/rotation-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/variable-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/variable-0.1.1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.057605 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/datamodels/
--rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/datamodels/multi_pass_weld-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/datamodels/multi_pass_weld-0.1.1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    25934 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/datamodels/single_pass_weld-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/datamodels/terms-0.1.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.057605 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/debug/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/debug/test_property_tag-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/debug/test_shape_validator-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/debug/test_unit_validator-0.1.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.057605 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/equipment/
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/equipment/measurement_equipment-0.1.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.057605 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/groove/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.061605 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/DHUGroove-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/DHVGroove-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/DUGroove-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/DVGroove-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/FFGroove-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/HUGroove-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/HVGroove-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/IGroove-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/UGroove-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/UVGroove-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/VGroove-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/VVGroove-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/groove/terms-0.1.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.061605 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/measurement/
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/measurement/error-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/measurement/measurement-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/measurement/measurement_chain-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/measurement/signal-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/measurement/signal_transformation-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/measurement/source-0.1.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.061605 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/process/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.061605 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/process/CLOOS/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/process/CLOOS/pulse-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/process/CLOOS/spray_arc-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/process/GMAW-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/process/generic-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/process/terms-0.1.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.061605 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/time/
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/time/datetimeindex-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/time/time-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/time/timedelta-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/time/timedeltaindex-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/time/timestamp-0.1.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.061605 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/units/
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/units/dimension-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/units/quantity-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/units/units-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/uuid-0.1.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.061605 weldx-0.6.5/weldx/tags/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.061605 weldx-0.6.5/weldx/tags/aws/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.065605 weldx-0.6.5/weldx/tags/aws/design/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/aws/design/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/aws/design/base_metal.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/aws/design/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/aws/design/joint_penetration.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/aws/design/sub_assembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/aws/design/weld_details.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/aws/design/weldment.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/aws/design/workpiece.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.065605 weldx-0.6.5/weldx/tags/aws/process/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/aws/process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/aws/process/arc_welding_process.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/aws/process/gas_component.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/aws/process/shielding_gas_for_procedure.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/aws/process/shielding_gas_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/base_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.065605 weldx-0.6.5/weldx/tags/core/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/core/data_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/core/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/core/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/core/generic_series.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.065605 weldx-0.6.5/weldx/tags/core/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/core/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/core/geometry/spatial_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/core/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/core/mathematical_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/core/media_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/core/time_series.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.065605 weldx-0.6.5/weldx/tags/core/transformations/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/core/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/core/transformations/coordinate_system_hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/core/transformations/local_coordinate_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/core/transformations/rotation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.069606 weldx-0.6.5/weldx/tags/debug/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/debug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/debug/test_property_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/debug/test_shape_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/debug/test_unit_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.069606 weldx-0.6.5/weldx/tags/equipment/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/equipment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/equipment/measurement_equipment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.069606 weldx-0.6.5/weldx/tags/groove/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/groove/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/groove/iso_9692_1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.069606 weldx-0.6.5/weldx/tags/measurement/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/measurement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/measurement/error.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/measurement/measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/measurement/measurement_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/measurement/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/measurement/signal_transformation.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/measurement/source.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.069606 weldx-0.6.5/weldx/tags/processes/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/processes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/processes/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.069606 weldx-0.6.5/weldx/tags/time/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/time/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/time/datetimeindex.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/time/time.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/time/timedelta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/time/timedeltaindex.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/time/timestamp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.069606 weldx-0.6.5/weldx/tags/units/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/units/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tags/units/pint_quantity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.073606 weldx-0.6.5/weldx/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tests/_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.077606 weldx-0.6.5/weldx/tests/asdf_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tests/asdf_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tests/asdf_tests/installable_quality_standard_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tests/asdf_tests/quality_standards_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tests/asdf_tests/test_asdf_aws_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tests/asdf_tests/test_asdf_base_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    29871 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tests/asdf_tests/test_asdf_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tests/asdf_tests/test_asdf_gmaw_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tests/asdf_tests/test_asdf_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tests/asdf_tests/test_asdf_groove.py
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tests/asdf_tests/test_asdf_measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tests/asdf_tests/test_asdf_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tests/asdf_tests/test_asdf_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tests/asdf_tests/test_asdf_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tests/asdf_tests/test_asdf_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tests/asdf_tests/test_media_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    23287 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tests/asdf_tests/test_weldx_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.077606 weldx-0.6.5/weldx/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tests/data/WelDX_notext.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.045604 weldx-0.6.5/weldx/tests/data/quality_standard/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.045604 weldx-0.6.5/weldx/tests/data/quality_standard/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.045604 weldx-0.6.5/weldx/tests/data/quality_standard/resources/test_organization/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.077606 weldx-0.6.5/weldx/tests/data/quality_standard/resources/test_organization/manifests/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tests/data/quality_standard/resources/test_organization/manifests/test_standard-1.0.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.077606 weldx-0.6.5/weldx/tests/data/quality_standard/resources/test_organization/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tests/data/quality_standard/resources/test_organization/schemas/alternative_measurement_equipment_schema-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    38638 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    99822 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    16672 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tests/test_measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)    27679 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tests/test_time.py
--rw-r--r--   0 runner    (1001) docker     (123)    20350 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tests/test_utility.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tests/test_visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tests/test_welding_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.077606 weldx-0.6.5/weldx/tests/transformations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tests/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tests/transformations/_util.py
--rw-r--r--   0 runner    (1001) docker     (123)   100131 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tests/transformations/test_cs_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    50176 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tests/transformations/test_local_cs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9428 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/tests/transformations/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    27811 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.077606 weldx-0.6.5/weldx/transformations/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    73288 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/transformations/cs_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    32437 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/transformations/local_cs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/transformations/rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/transformations/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/transformations/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.077606 weldx-0.6.5/weldx/util/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/util/external_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/util/media_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    13089 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/util/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    28462 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/util/xarray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.077606 weldx-0.6.5/weldx/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.081606 weldx-0.6.5/weldx/welding/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/welding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.081606 weldx-0.6.5/weldx/welding/groove/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/welding/groove/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64373 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/welding/groove/iso_9692_1.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/welding/processes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-06 15:27:00.000000 weldx-0.6.5/weldx/welding/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:27:24.049605 weldx-0.6.5/weldx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-04-06 15:27:23.000000 weldx-0.6.5/weldx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9946 2023-04-06 15:27:24.000000 weldx-0.6.5/weldx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 15:27:23.000000 weldx-0.6.5/weldx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-06 15:27:23.000000 weldx-0.6.5/weldx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-06 15:27:23.000000 weldx-0.6.5/weldx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-06 15:27:23.000000 weldx-0.6.5/weldx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.350632 weldx-0.6.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    41030 2023-04-19 08:17:45.000000 weldx-0.6.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-19 08:17:45.000000 weldx-0.6.6/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-19 08:17:45.000000 weldx-0.6.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-19 08:17:45.000000 weldx-0.6.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-04-19 08:18:04.354632 weldx-0.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-04-19 08:17:45.000000 weldx-0.6.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-04-19 08:17:45.000000 weldx-0.6.6/RELEASE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-19 08:17:45.000000 weldx-0.6.6/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-19 08:17:45.000000 weldx-0.6.6/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-04-19 08:17:45.000000 weldx-0.6.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 08:18:04.354632 weldx-0.6.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.326632 weldx-0.6.6/weldx/
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-19 08:18:04.000000 weldx-0.6.6/weldx/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.330632 weldx-0.6.6/weldx/asdf/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/asdf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.330632 weldx-0.6.6/weldx/asdf/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/asdf/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10850 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/asdf/cli/welding_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/asdf/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/asdf/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35535 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/asdf/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/asdf/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23452 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/asdf/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18813 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/asdf/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.330632 weldx-0.6.6/weldx/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34598 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/core/generic_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8174 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/core/math_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/core/spatial_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16188 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/core/time_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92765 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.330632 weldx-0.6.6/weldx/manifests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/manifests/weldx-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/manifests/weldx-0.1.1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/manifests/weldx-0.1.2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    37433 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/measurement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.322632 weldx-0.6.6/weldx/schemas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.322632 weldx-0.6.6/weldx/schemas/weldx.bam.de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.330632 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.322632 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/aws/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.330632 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/aws/design/
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/aws/design/base_metal-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/aws/design/connection-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/aws/design/joint_penetration-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/aws/design/sub_assembly-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/aws/design/weld_details-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/aws/design/weldment-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/aws/design/workpiece-0.1.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.330632 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/aws/process/
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/aws/process/arc_welding_process-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/aws/process/gas_component-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/aws/process/shielding_gas_for_procedure-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/aws/process/shielding_gas_type-0.1.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.334632 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/data_array-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/dataset-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/dimension-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/file-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/file-0.1.1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/generic_series-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/generic_series_free_dimension-0.1.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.334632 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/geometry/spatial_data-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/geometry/spatial_data-0.1.1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.334632 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/graph/di_edge-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/graph/di_graph-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/graph/di_node-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/mathematical_expression-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/media_file-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/time_series-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/time_series-0.1.1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.334632 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/transformations/coordinate_system_hierarchy-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/transformations/local_coordinate_system-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/transformations/local_coordinate_system-0.1.1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/transformations/rotation-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/variable-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/variable-0.1.1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.334632 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/datamodels/
+-rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/datamodels/multi_pass_weld-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/datamodels/multi_pass_weld-0.1.1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    25934 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/datamodels/single_pass_weld-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/datamodels/terms-0.1.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.334632 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/debug/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/debug/test_property_tag-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/debug/test_shape_validator-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/debug/test_unit_validator-0.1.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.334632 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/equipment/
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/equipment/measurement_equipment-0.1.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.334632 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/groove/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.338632 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/DHUGroove-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/DHVGroove-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/DUGroove-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/DVGroove-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/FFGroove-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/HUGroove-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/HVGroove-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/IGroove-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/UGroove-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/UVGroove-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/VGroove-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/VVGroove-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/groove/terms-0.1.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.338632 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/measurement/
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/measurement/error-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/measurement/measurement-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/measurement/measurement_chain-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/measurement/signal-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/measurement/signal_transformation-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/measurement/source-0.1.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.338632 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/process/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.338632 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/process/CLOOS/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/process/CLOOS/pulse-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/process/CLOOS/spray_arc-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/process/GMAW-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/process/generic-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/process/terms-0.1.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.338632 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/time/
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/time/datetimeindex-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/time/time-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/time/timedelta-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/time/timedeltaindex-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/time/timestamp-0.1.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.338632 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/units/
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/units/dimension-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/units/quantity-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/units/units-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/uuid-0.1.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.338632 weldx-0.6.6/weldx/tags/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.338632 weldx-0.6.6/weldx/tags/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.342632 weldx-0.6.6/weldx/tags/aws/design/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/aws/design/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/aws/design/base_metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/aws/design/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/aws/design/joint_penetration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/aws/design/sub_assembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/aws/design/weld_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/aws/design/weldment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/aws/design/workpiece.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.342632 weldx-0.6.6/weldx/tags/aws/process/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/aws/process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/aws/process/arc_welding_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/aws/process/gas_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/aws/process/shielding_gas_for_procedure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/aws/process/shielding_gas_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/base_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.342632 weldx-0.6.6/weldx/tags/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/core/data_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/core/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/core/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/core/generic_series.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.342632 weldx-0.6.6/weldx/tags/core/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/core/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/core/geometry/spatial_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/core/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/core/mathematical_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/core/media_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/core/time_series.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.342632 weldx-0.6.6/weldx/tags/core/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/core/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/core/transformations/coordinate_system_hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/core/transformations/local_coordinate_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/core/transformations/rotation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.342632 weldx-0.6.6/weldx/tags/debug/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/debug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/debug/test_property_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/debug/test_shape_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/debug/test_unit_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.342632 weldx-0.6.6/weldx/tags/equipment/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/equipment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/equipment/measurement_equipment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.342632 weldx-0.6.6/weldx/tags/groove/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/groove/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/groove/iso_9692_1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.346632 weldx-0.6.6/weldx/tags/measurement/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/measurement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/measurement/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/measurement/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/measurement/measurement_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/measurement/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/measurement/signal_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/measurement/source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.346632 weldx-0.6.6/weldx/tags/processes/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/processes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/processes/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.346632 weldx-0.6.6/weldx/tags/time/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/time/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/time/datetimeindex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/time/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/time/timedelta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/time/timedeltaindex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/time/timestamp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.346632 weldx-0.6.6/weldx/tags/units/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/units/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tags/units/pint_quantity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.346632 weldx-0.6.6/weldx/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tests/_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.350632 weldx-0.6.6/weldx/tests/asdf_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tests/asdf_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tests/asdf_tests/installable_quality_standard_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tests/asdf_tests/quality_standards_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tests/asdf_tests/test_asdf_aws_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tests/asdf_tests/test_asdf_base_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29871 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tests/asdf_tests/test_asdf_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tests/asdf_tests/test_asdf_gmaw_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tests/asdf_tests/test_asdf_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tests/asdf_tests/test_asdf_groove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tests/asdf_tests/test_asdf_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tests/asdf_tests/test_asdf_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tests/asdf_tests/test_asdf_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tests/asdf_tests/test_asdf_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tests/asdf_tests/test_asdf_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tests/asdf_tests/test_media_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23287 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tests/asdf_tests/test_weldx_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.350632 weldx-0.6.6/weldx/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tests/data/WelDX_notext.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.326632 weldx-0.6.6/weldx/tests/data/quality_standard/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.326632 weldx-0.6.6/weldx/tests/data/quality_standard/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.326632 weldx-0.6.6/weldx/tests/data/quality_standard/resources/test_organization/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.350632 weldx-0.6.6/weldx/tests/data/quality_standard/resources/test_organization/manifests/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tests/data/quality_standard/resources/test_organization/manifests/test_standard-1.0.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.350632 weldx-0.6.6/weldx/tests/data/quality_standard/resources/test_organization/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tests/data/quality_standard/resources/test_organization/schemas/alternative_measurement_equipment_schema-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38638 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99822 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16672 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tests/test_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27679 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tests/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20350 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tests/test_utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tests/test_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tests/test_welding_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.350632 weldx-0.6.6/weldx/tests/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tests/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tests/transformations/_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100131 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tests/transformations/test_cs_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50182 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tests/transformations/test_local_cs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9428 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/tests/transformations/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27811 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.350632 weldx-0.6.6/weldx/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73288 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/transformations/cs_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32466 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/transformations/local_cs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/transformations/rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/transformations/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/transformations/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.350632 weldx-0.6.6/weldx/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/util/external_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/util/media_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13089 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/util/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28495 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/util/xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.350632 weldx-0.6.6/weldx/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.350632 weldx-0.6.6/weldx/welding/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/welding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.350632 weldx-0.6.6/weldx/welding/groove/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/welding/groove/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64373 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/welding/groove/iso_9692_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/welding/processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-19 08:17:45.000000 weldx-0.6.6/weldx/welding/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:18:04.330632 weldx-0.6.6/weldx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-04-19 08:18:04.000000 weldx-0.6.6/weldx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9946 2023-04-19 08:18:04.000000 weldx-0.6.6/weldx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 08:18:04.000000 weldx-0.6.6/weldx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-19 08:18:04.000000 weldx-0.6.6/weldx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-19 08:18:04.000000 weldx-0.6.6/weldx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-19 08:18:04.000000 weldx-0.6.6/weldx.egg-info/top_level.txt
```

### Comparing `weldx-0.6.5/CHANGELOG.md` & `weldx-0.6.6/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,21 @@
 # Release Notes
 
+## 0.6.6 (19.04.2023)
+
+Version `0.6.6` is a compatibility release for `xarray>=2023.4.0` .
+
+### Fixes
+
+- explicitly keep reference time as xarray attribute in transformation and interpolation operations \[{pull}`868`\] .
+
+### Dependencies
+
+- compatibility with `xarray=2023.4.0` and `pandas=2` \[{pull}`868`\] .
+
 ## 0.6.5 (2023.04.06)
 
 Version `0.6.5` is a compatibility release to support new `asdf` and `xarray` and drops support for Python 3.8.
 Please see the new minimal version requirements below.
 
 ### Fixes
```

### Comparing `weldx-0.6.5/CITATION.cff` & `weldx-0.6.6/CITATION.cff`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # YAML 1.2
 ---
 title: weldx
-version: 0.6.5
-date-released: 2023-04-06
+version: 0.6.6
+date-released: 2023-04-19
 authors:
   - affiliation: "Bundesanstalt für Materialforschung und -prüfung (BAM)"
     email: cagtay.fabry@bam.de
     family-names: Fabry
     given-names: Cagtay
     orcid: "https://orcid.org/0000-0002-0788-8079"
   - affiliation: "Bundesanstalt für Materialforschung und -prüfung (BAM)"
```

### Comparing `weldx-0.6.5/LICENSE` & `weldx-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/PKG-INFO` & `weldx-0.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weldx
-Version: 0.6.5
+Version: 0.6.6
 Summary: Python API for the WelDX file format and standard
 Author-email: Cagtay Fabry <cagtay.fabry@bam.de>, Volker Hirthammer <volker.hirthammer@bam.de>, "Martin K. Scherer" <martin.scherer@bam.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2020, BAMWelDX
         All rights reserved.
```

### Comparing `weldx-0.6.5/README.md` & `weldx-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/RELEASE.md` & `weldx-0.6.6/RELEASE.md`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/conftest.py` & `weldx-0.6.6/conftest.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/pyproject.toml` & `weldx-0.6.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/__init__.py` & `weldx-0.6.6/weldx/__init__.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/asdf/cli/welding_schema.py` & `weldx-0.6.6/weldx/asdf/cli/welding_schema.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/asdf/constants.py` & `weldx-0.6.6/weldx/asdf/constants.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/asdf/extension.py` & `weldx-0.6.6/weldx/asdf/extension.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/asdf/file.py` & `weldx-0.6.6/weldx/asdf/file.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/asdf/types.py` & `weldx-0.6.6/weldx/asdf/types.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/asdf/util.py` & `weldx-0.6.6/weldx/asdf/util.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/asdf/validators.py` & `weldx-0.6.6/weldx/asdf/validators.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/config.py` & `weldx-0.6.6/weldx/config.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/constants.py` & `weldx-0.6.6/weldx/constants.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/core/generic_series.py` & `weldx-0.6.6/weldx/core/generic_series.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/core/math_expression.py` & `weldx-0.6.6/weldx/core/math_expression.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/core/spatial_series.py` & `weldx-0.6.6/weldx/core/spatial_series.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/core/time_series.py` & `weldx-0.6.6/weldx/core/time_series.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/geometry.py` & `weldx-0.6.6/weldx/geometry.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/manifests/weldx-0.1.0.yaml` & `weldx-0.6.6/weldx/manifests/weldx-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/manifests/weldx-0.1.1.yaml` & `weldx-0.6.6/weldx/manifests/weldx-0.1.1.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/manifests/weldx-0.1.2.yaml` & `weldx-0.6.6/weldx/manifests/weldx-0.1.2.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/measurement.py` & `weldx-0.6.6/weldx/measurement.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/aws/design/base_metal-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/aws/design/base_metal-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/aws/design/connection-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/aws/design/connection-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/aws/design/joint_penetration-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/aws/design/joint_penetration-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/aws/design/sub_assembly-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/aws/design/sub_assembly-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/aws/design/weld_details-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/aws/design/weld_details-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/aws/design/workpiece-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/aws/design/workpiece-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/aws/process/arc_welding_process-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/aws/process/arc_welding_process-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/aws/process/gas_component-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/aws/process/gas_component-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/aws/process/shielding_gas_for_procedure-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/aws/process/shielding_gas_for_procedure-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/aws/process/shielding_gas_type-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/aws/process/shielding_gas_type-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/data_array-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/data_array-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/dataset-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/dataset-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/dimension-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/dimension-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/file-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/file-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/file-0.1.1.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/file-0.1.1.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/generic_series-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/generic_series-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/generic_series_free_dimension-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/generic_series_free_dimension-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/geometry/spatial_data-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/geometry/spatial_data-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/geometry/spatial_data-0.1.1.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/geometry/spatial_data-0.1.1.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/graph/di_edge-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/graph/di_edge-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/graph/di_graph-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/graph/di_graph-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/graph/di_node-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/graph/di_node-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/mathematical_expression-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/mathematical_expression-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/media_file-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/media_file-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/time_series-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/time_series-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/time_series-0.1.1.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/time_series-0.1.1.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/transformations/coordinate_system_hierarchy-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/transformations/coordinate_system_hierarchy-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/transformations/local_coordinate_system-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/transformations/local_coordinate_system-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/transformations/local_coordinate_system-0.1.1.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/transformations/local_coordinate_system-0.1.1.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/transformations/rotation-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/transformations/rotation-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/variable-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/variable-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/core/variable-0.1.1.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/core/variable-0.1.1.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/datamodels/multi_pass_weld-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/datamodels/multi_pass_weld-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/datamodels/multi_pass_weld-0.1.1.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/datamodels/multi_pass_weld-0.1.1.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/datamodels/single_pass_weld-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/datamodels/single_pass_weld-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/datamodels/terms-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/datamodels/terms-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/debug/test_property_tag-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/debug/test_property_tag-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/debug/test_shape_validator-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/debug/test_shape_validator-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/debug/test_unit_validator-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/debug/test_unit_validator-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/equipment/measurement_equipment-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/equipment/measurement_equipment-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/DHUGroove-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/DHUGroove-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/DHVGroove-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/DHVGroove-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/DUGroove-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/DUGroove-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/DVGroove-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/DVGroove-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/FFGroove-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/FFGroove-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/HUGroove-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/HUGroove-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/HVGroove-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/HVGroove-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/IGroove-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/IGroove-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/UGroove-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/UGroove-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/UVGroove-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/UVGroove-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/VGroove-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/VGroove-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/VVGroove-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/groove/iso_9692_1_2013_12/VVGroove-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/groove/terms-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/groove/terms-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/measurement/error-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/measurement/error-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/measurement/measurement-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/measurement/measurement-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/measurement/measurement_chain-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/measurement/measurement_chain-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/measurement/signal-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/measurement/signal-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/measurement/signal_transformation-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/measurement/signal_transformation-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/measurement/source-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/measurement/source-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/process/CLOOS/spray_arc-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/process/CLOOS/spray_arc-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/process/GMAW-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/process/GMAW-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/process/terms-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/process/terms-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/time/datetimeindex-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/time/datetimeindex-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/time/time-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/time/time-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/time/timedelta-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/time/timedelta-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/time/timedeltaindex-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/time/timedeltaindex-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/time/timestamp-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/time/timestamp-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/units/dimension-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/units/dimension-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/units/quantity-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/units/quantity-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/schemas/weldx.bam.de/weldx/uuid-0.1.0.yaml` & `weldx-0.6.6/weldx/schemas/weldx.bam.de/weldx/uuid-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tags/aws/design/base_metal.py` & `weldx-0.6.6/weldx/tags/aws/design/base_metal.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tags/aws/design/connection.py` & `weldx-0.6.6/weldx/tags/aws/design/connection.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tags/aws/design/joint_penetration.py` & `weldx-0.6.6/weldx/tags/aws/design/joint_penetration.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tags/aws/design/sub_assembly.py` & `weldx-0.6.6/weldx/tags/aws/design/sub_assembly.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tags/aws/process/arc_welding_process.py` & `weldx-0.6.6/weldx/tags/aws/process/arc_welding_process.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tags/aws/process/shielding_gas_for_procedure.py` & `weldx-0.6.6/weldx/tags/aws/process/shielding_gas_for_procedure.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tags/aws/process/shielding_gas_type.py` & `weldx-0.6.6/weldx/tags/aws/process/shielding_gas_type.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tags/base_types.py` & `weldx-0.6.6/weldx/tags/base_types.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tags/core/common_types.py` & `weldx-0.6.6/weldx/tags/core/common_types.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tags/core/data_array.py` & `weldx-0.6.6/weldx/tags/core/data_array.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tags/core/dataset.py` & `weldx-0.6.6/weldx/tags/core/dataset.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tags/core/file.py` & `weldx-0.6.6/weldx/tags/core/file.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tags/core/generic_series.py` & `weldx-0.6.6/weldx/tags/core/generic_series.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tags/core/geometry/spatial_data.py` & `weldx-0.6.6/weldx/tags/core/geometry/spatial_data.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tags/core/graph.py` & `weldx-0.6.6/weldx/tags/core/graph.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tags/core/mathematical_expression.py` & `weldx-0.6.6/weldx/tags/core/mathematical_expression.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tags/core/media_file.py` & `weldx-0.6.6/weldx/tags/core/media_file.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tags/core/time_series.py` & `weldx-0.6.6/weldx/tags/core/time_series.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tags/core/transformations/coordinate_system_hierarchy.py` & `weldx-0.6.6/weldx/tags/core/transformations/coordinate_system_hierarchy.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tags/core/transformations/local_coordinate_system.py` & `weldx-0.6.6/weldx/tags/core/transformations/local_coordinate_system.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tags/core/transformations/rotation.py` & `weldx-0.6.6/weldx/tags/core/transformations/rotation.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tags/debug/test_property_tag.py` & `weldx-0.6.6/weldx/tags/debug/test_property_tag.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tags/debug/test_shape_validator.py` & `weldx-0.6.6/weldx/tags/debug/test_shape_validator.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tags/debug/test_unit_validator.py` & `weldx-0.6.6/weldx/tags/debug/test_unit_validator.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tags/groove/iso_9692_1.py` & `weldx-0.6.6/weldx/tags/groove/iso_9692_1.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tags/measurement/measurement_chain.py` & `weldx-0.6.6/weldx/tags/measurement/measurement_chain.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tags/processes/process.py` & `weldx-0.6.6/weldx/tags/processes/process.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tags/time/datetimeindex.py` & `weldx-0.6.6/weldx/tags/time/datetimeindex.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tags/time/time.py` & `weldx-0.6.6/weldx/tags/time/time.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tags/time/timedelta.py` & `weldx-0.6.6/weldx/tags/time/timedelta.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tags/time/timedeltaindex.py` & `weldx-0.6.6/weldx/tags/time/timedeltaindex.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tags/time/timestamp.py` & `weldx-0.6.6/weldx/tags/time/timestamp.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tags/units/pint_quantity.py` & `weldx-0.6.6/weldx/tags/units/pint_quantity.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tests/_helpers.py` & `weldx-0.6.6/weldx/tests/_helpers.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tests/asdf_tests/quality_standards_check.py` & `weldx-0.6.6/weldx/tests/asdf_tests/quality_standards_check.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tests/asdf_tests/test_asdf_aws_schema.py` & `weldx-0.6.6/weldx/tests/asdf_tests/test_asdf_aws_schema.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tests/asdf_tests/test_asdf_base_types.py` & `weldx-0.6.6/weldx/tests/asdf_tests/test_asdf_base_types.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tests/asdf_tests/test_asdf_core.py` & `weldx-0.6.6/weldx/tests/asdf_tests/test_asdf_core.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tests/asdf_tests/test_asdf_gmaw_process.py` & `weldx-0.6.6/weldx/tests/asdf_tests/test_asdf_gmaw_process.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tests/asdf_tests/test_asdf_graph.py` & `weldx-0.6.6/weldx/tests/asdf_tests/test_asdf_graph.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tests/asdf_tests/test_asdf_groove.py` & `weldx-0.6.6/weldx/tests/asdf_tests/test_asdf_groove.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tests/asdf_tests/test_asdf_measurement.py` & `weldx-0.6.6/weldx/tests/asdf_tests/test_asdf_measurement.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tests/asdf_tests/test_asdf_time.py` & `weldx-0.6.6/weldx/tests/asdf_tests/test_asdf_time.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tests/asdf_tests/test_asdf_types.py` & `weldx-0.6.6/weldx/tests/asdf_tests/test_asdf_types.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tests/asdf_tests/test_asdf_util.py` & `weldx-0.6.6/weldx/tests/asdf_tests/test_asdf_util.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tests/asdf_tests/test_asdf_validators.py` & `weldx-0.6.6/weldx/tests/asdf_tests/test_asdf_validators.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tests/asdf_tests/test_media_file.py` & `weldx-0.6.6/weldx/tests/asdf_tests/test_media_file.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tests/asdf_tests/test_weldx_file.py` & `weldx-0.6.6/weldx/tests/asdf_tests/test_weldx_file.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tests/conftest.py` & `weldx-0.6.6/weldx/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tests/data/WelDX_notext.svg` & `weldx-0.6.6/weldx/tests/data/WelDX_notext.svg`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tests/data/quality_standard/resources/test_organization/schemas/alternative_measurement_equipment_schema-1.0.0.yaml` & `weldx-0.6.6/weldx/tests/data/quality_standard/resources/test_organization/schemas/alternative_measurement_equipment_schema-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tests/test_config.py` & `weldx-0.6.6/weldx/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tests/test_core.py` & `weldx-0.6.6/weldx/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tests/test_geometry.py` & `weldx-0.6.6/weldx/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tests/test_measurement.py` & `weldx-0.6.6/weldx/tests/test_measurement.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tests/test_time.py` & `weldx-0.6.6/weldx/tests/test_time.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tests/test_utility.py` & `weldx-0.6.6/weldx/tests/test_utility.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tests/test_visualization.py` & `weldx-0.6.6/weldx/tests/test_visualization.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tests/test_welding_util.py` & `weldx-0.6.6/weldx/tests/test_welding_util.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tests/transformations/_util.py` & `weldx-0.6.6/weldx/tests/transformations/_util.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tests/transformations/test_cs_manager.py` & `weldx-0.6.6/weldx/tests/transformations/test_cs_manager.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/tests/transformations/test_local_cs.py` & `weldx-0.6.6/weldx/tests/transformations/test_local_cs.py`

 * *Files 0% similar despite different names*

```diff
@@ -623,18 +623,18 @@
     linearly in time.
 
     Parameters
     ----------
     seconds :
         The seconds (time delta) that should be interpolated
     lcs_ref_sec :
-        The seconds of the reference time, that will passed to the created LCS. If
+        The seconds of the reference time, that will be passed to the created LCS. If
         `None`, no reference time will be passed
     ref_sec :
-        The seconds of the reference time, that will passed to `interp_time`. If
+        The seconds of the reference time, that will be passed to `interp_time`. If
         `None`, no reference time will be passed
     time_dep_orientation :
         If `True` a time dependent orientation will be passed to the LCS.
         The orientation is a rotation around the x axis. The rotation angle is 0
         degrees at t=0 seconds and increases linearly to 90 degrees over the next
         4 seconds. Before and after this period, the angle is kept constant.
```

### Comparing `weldx-0.6.5/weldx/tests/transformations/test_util.py` & `weldx-0.6.6/weldx/tests/transformations/test_util.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/time.py` & `weldx-0.6.6/weldx/time.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/transformations/__init__.py` & `weldx-0.6.6/weldx/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/transformations/cs_manager.py` & `weldx-0.6.6/weldx/transformations/cs_manager.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/transformations/local_cs.py` & `weldx-0.6.6/weldx/transformations/local_cs.py`

 * *Files 0% similar despite different names*

```diff
@@ -356,14 +356,15 @@
         )
 
         orientation = xr.apply_ufunc(
             normalize,
             orientation,
             input_core_dims=[["c"]],
             output_core_dims=[["c"]],
+            keep_attrs=True,
         )
 
         # vectorize test if orthogonal
         if not ut.xr_is_orthogonal_matrix(orientation, dims=["c", "v"]):
             raise ValueError("Orientation vectors must be orthogonal")
 
         return orientation
```

### Comparing `weldx-0.6.5/weldx/transformations/rotation.py` & `weldx-0.6.6/weldx/transformations/rotation.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/transformations/util.py` & `weldx-0.6.6/weldx/transformations/util.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/types.py` & `weldx-0.6.6/weldx/types.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/util/external_file.py` & `weldx-0.6.6/weldx/util/external_file.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/util/media_file.py` & `weldx-0.6.6/weldx/util/media_file.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/util/util.py` & `weldx-0.6.6/weldx/util/util.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/util/xarray.py` & `weldx-0.6.6/weldx/util/xarray.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,14 +166,15 @@
 
     return xr.apply_ufunc(
         mul_func,
         a,
         b,
         input_core_dims=[dims_a, dims_b],
         output_core_dims=[dims_out],
+        keep_attrs=True,
         **apply_kwargs,
     )
 
 
 def xr_is_orthogonal_matrix(da: xr.DataArray, dims: list[str]) -> bool:
     """Check if  matrix along specific dimensions in a DataArray is orthogonal.
 
@@ -613,15 +614,15 @@
 
     if time is not None:
         if "time" not in dims:  # prepend to beginning if not already set
             dims = ["time"] + dims
         coords["time"] = time  # type: ignore[assignment]
 
     if "time" in coords:
-        coords["time"] = Time(coords["time"]).index
+        coords["time"] = Time(coords["time"]).as_data_array()
 
     coords = dict(add_coords, **coords)
 
     da = xr.DataArray(data=data, dims=dims, coords=coords).transpose(..., "c")
 
     return da.astype(float).weldx.time_ref_restore()
 
@@ -639,15 +640,15 @@
     Returns
     -------
     xarray.DataArray
 
     """
     if time is not None and np.array(data).ndim == 3:
         if isinstance(time, Time):
-            time = time.as_pandas_index()
+            time = time.as_data_array()
         da = xr.DataArray(
             data=data,
             dims=["time", "c", "v"],
             coords={"time": time, "c": ["x", "y", "z"], "v": [0, 1, 2]},
         )
     else:
         da = xr.DataArray(
```

### Comparing `weldx-0.6.5/weldx/visualization/__init__.py` & `weldx-0.6.6/weldx/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/welding/groove/iso_9692_1.py` & `weldx-0.6.6/weldx/welding/groove/iso_9692_1.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/welding/processes.py` & `weldx-0.6.6/weldx/welding/processes.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx/welding/util.py` & `weldx-0.6.6/weldx/welding/util.py`

 * *Files identical despite different names*

### Comparing `weldx-0.6.5/weldx.egg-info/PKG-INFO` & `weldx-0.6.6/weldx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weldx
-Version: 0.6.5
+Version: 0.6.6
 Summary: Python API for the WelDX file format and standard
 Author-email: Cagtay Fabry <cagtay.fabry@bam.de>, Volker Hirthammer <volker.hirthammer@bam.de>, "Martin K. Scherer" <martin.scherer@bam.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2020, BAMWelDX
         All rights reserved.
```

### Comparing `weldx-0.6.5/weldx.egg-info/SOURCES.txt` & `weldx-0.6.6/weldx.egg-info/SOURCES.txt`

 * *Files identical despite different names*


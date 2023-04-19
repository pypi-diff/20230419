# Comparing `tmp/qiskit-experiments-0.5.0.tar.gz` & `tmp/qiskit-experiments-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit-experiments-0.5.0.tar", last modified: Tue Mar 28 19:32:12 2023, max compression
+gzip compressed data, was "qiskit-experiments-0.5.1.tar", last modified: Wed Apr 19 01:39:00 2023, max compression
```

## Comparing `qiskit-experiments-0.5.0.tar` & `qiskit-experiments-0.5.1.tar`

### file list

```diff
@@ -1,209 +1,209 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:32:12.464128 qiskit-experiments-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-03-28 19:32:12.464128 qiskit-experiments-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:32:12.432125 qiskit-experiments-0.5.0/qiskit_experiments/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:32:12.436126 qiskit-experiments-0.5.0/qiskit_experiments/calibration_management/
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/calibration_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15632 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/calibration_management/base_calibration_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    16951 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/calibration_management/basis_gate_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/calibration_management/calibration_key_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/calibration_management/calibration_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    70393 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/calibration_management/calibrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/calibration_management/control_channel_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/calibration_management/parameter_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     7115 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/calibration_management/update_library.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:32:12.440126 qiskit-experiments-0.5.0/qiskit_experiments/curve_analysis/
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/curve_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17468 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/curve_analysis/base_curve_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    15107 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/curve_analysis/composite_curve_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    18942 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/curve_analysis/curve_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    22146 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/curve_analysis/curve_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    12185 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/curve_analysis/curve_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/curve_analysis/fit_function.py
--rw-r--r--   0 runner    (1001) docker     (123)    11532 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/curve_analysis/guess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:32:12.440126 qiskit-experiments-0.5.0/qiskit_experiments/curve_analysis/standard_analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/curve_analysis/standard_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/curve_analysis/standard_analysis/bloch_trajectory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/curve_analysis/standard_analysis/decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/curve_analysis/standard_analysis/error_amplification_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/curve_analysis/standard_analysis/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/curve_analysis/standard_analysis/oscillation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/curve_analysis/standard_analysis/resonance.py
--rw-r--r--   0 runner    (1001) docker     (123)    17350 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/curve_analysis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:32:12.440126 qiskit-experiments-0.5.0/qiskit_experiments/curve_analysis/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/curve_analysis/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12035 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/curve_analysis/visualization/base_drawer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/curve_analysis/visualization/curves.py
--rw-r--r--   0 runner    (1001) docker     (123)    16466 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/curve_analysis/visualization/fit_result_plotters.py
--rw-r--r--   0 runner    (1001) docker     (123)    15038 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/curve_analysis/visualization/mpl_drawer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/curve_analysis/visualization/style.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:32:12.440126 qiskit-experiments-0.5.0/qiskit_experiments/data_processing/
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/data_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/data_processing/data_action.py
--rw-r--r--   0 runner    (1001) docker     (123)    12779 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/data_processing/data_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/data_processing/discriminator.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/data_processing/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    42185 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/data_processing/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/data_processing/processor_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/data_processing/sklearn_discriminators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:32:12.444126 qiskit-experiments-0.5.0/qiskit_experiments/database_service/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/database_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/database_service/device_component.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/database_service/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/database_service/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:32:12.444126 qiskit-experiments-0.5.0/qiskit_experiments/framework/
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17743 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/framework/analysis_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/framework/analysis_result_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/framework/backend_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    15017 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/framework/backend_timing.py
--rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/framework/base_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    16475 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/framework/base_experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:32:12.448127 qiskit-experiments-0.5.0/qiskit_experiments/framework/composite/
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/framework/composite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/framework/composite/batch_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    15898 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/framework/composite/composite_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     8034 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/framework/composite/composite_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/framework/composite/parallel_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/framework/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)    84134 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/framework/experiment_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    23184 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/framework/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/framework/matplotlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     9473 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/framework/restless_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/framework/store_init_args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:32:12.448127 qiskit-experiments-0.5.0/qiskit_experiments/library/
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:32:12.448127 qiskit-experiments-0.5.0/qiskit_experiments/library/calibration/
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/calibration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/calibration/fine_amplitude.py
--rw-r--r--   0 runner    (1001) docker     (123)     8471 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/calibration/fine_drag_cal.py
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/calibration/fine_frequency_cal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/calibration/frequency_cal.py
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/calibration/half_angle_cal.py
--rw-r--r--   0 runner    (1001) docker     (123)    10951 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/calibration/rough_amplitude_cal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/calibration/rough_drag_cal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/calibration/rough_frequency.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:32:12.452127 qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/
--rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:32:12.452127 qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/analysis/correlated_readout_error_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/analysis/cr_hamiltonian_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/analysis/drag_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/analysis/fine_amplitude_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/analysis/local_readout_error_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/analysis/multi_state_discrimination_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/analysis/ramsey_xy_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/analysis/readout_angle_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/analysis/resonator_spectroscopy_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/analysis/t1_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/analysis/t2hahn_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/analysis/t2ramsey_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/analysis/tphi_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/analysis/zz_ramsey_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/correlated_readout_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    24596 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/cr_hamiltonian.py
--rw-r--r--   0 runner    (1001) docker     (123)     7927 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/drag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/ef_spectroscopy.py
--rw-r--r--   0 runner    (1001) docker     (123)    18587 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/fine_amplitude.py
--rw-r--r--   0 runner    (1001) docker     (123)    12364 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/fine_drag.py
--rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/fine_frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/half_angle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/local_readout_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/multi_state_discrimination.py
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/qubit_spectroscopy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/rabi.py
--rw-r--r--   0 runner    (1001) docker     (123)     9236 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/ramsey_xy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/readout_angle.py
--rw-r--r--   0 runner    (1001) docker     (123)    11665 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/resonator_spectroscopy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/spectroscopy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/t1.py
--rw-r--r--   0 runner    (1001) docker     (123)     7527 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/t2hahn.py
--rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/t2ramsey.py
--rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/tphi.py
--rw-r--r--   0 runner    (1001) docker     (123)    15761 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/zz_ramsey.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:32:12.456127 qiskit-experiments-0.5.0/qiskit_experiments/library/quantum_volume/
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/quantum_volume/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/quantum_volume/qv_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     7758 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/quantum_volume/qv_experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:32:12.456127 qiskit-experiments-0.5.0/qiskit_experiments/library/randomized_benchmarking/
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/randomized_benchmarking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20032 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/randomized_benchmarking/clifford_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:32:12.456127 qiskit-experiments-0.5.0/qiskit_experiments/library/randomized_benchmarking/data/
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/randomized_benchmarking/data/clifford_compose_1q.npz
--rw-r--r--   0 runner    (1001) docker     (123)   434028 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/randomized_benchmarking/data/clifford_compose_2q_sparse.npz
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/randomized_benchmarking/data/clifford_inverse_1q.npz
--rw-r--r--   0 runner    (1001) docker     (123)    19116 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/randomized_benchmarking/data/clifford_inverse_2q.npz
--rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/randomized_benchmarking/interleaved_rb_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/randomized_benchmarking/interleaved_rb_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    14888 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/randomized_benchmarking/rb_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/randomized_benchmarking/rb_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19508 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/randomized_benchmarking/standard_rb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:32:12.460127 qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:32:12.460127 qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/basis/
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/basis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7408 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/basis/base_basis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/basis/cache_method.py
--rw-r--r--   0 runner    (1001) docker     (123)    29737 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/basis/local_basis.py
--rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/basis/pauli_basis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:32:12.460127 qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/fitters/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/fitters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20672 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/fitters/cvxpy_lstsq.py
--rw-r--r--   0 runner    (1001) docker     (123)    10343 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/fitters/cvxpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7113 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/fitters/fitter_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    13316 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/fitters/lininv.py
--rw-r--r--   0 runner    (1001) docker     (123)    12083 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/fitters/lstsq_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/fitters/postprocess_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/fitters/scipy_lstsq.py
--rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/mit_qpt_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/mit_qst_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/mit_tomography_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/qpt_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/qpt_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/qst_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/qst_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    19670 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/tomography_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    13646 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/tomography_experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:32:12.464128 qiskit-experiments-0.5.0/qiskit_experiments/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/test/fake_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    20066 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/test/fake_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    31398 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/test/mock_iq_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    37323 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/test/mock_iq_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/test/noisy_delay_aer_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)    23891 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/test/pulse_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/test/t2hahn_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/test/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:32:12.464128 qiskit-experiments-0.5.0/qiskit_experiments/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:32:12.464128 qiskit-experiments-0.5.0/qiskit_experiments/visualization/drawers/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/visualization/drawers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23669 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/visualization/drawers/base_drawer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/visualization/drawers/legacy_curve_compat_drawer.py
--rw-r--r--   0 runner    (1001) docker     (123)    23317 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/visualization/drawers/mpl_drawer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:32:12.464128 qiskit-experiments-0.5.0/qiskit_experiments/visualization/plotters/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/visualization/plotters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25866 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/visualization/plotters/base_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/visualization/plotters/curve_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)    16098 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/visualization/plotters/iq_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/visualization/style.py
--rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/visualization/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8900 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/qiskit_experiments/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:32:12.436126 qiskit-experiments-0.5.0/qiskit_experiments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-03-28 19:32:12.000000 qiskit-experiments-0.5.0/qiskit_experiments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10175 2023-03-28 19:32:12.000000 qiskit-experiments-0.5.0/qiskit_experiments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 19:32:12.000000 qiskit-experiments-0.5.0/qiskit_experiments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 19:32:12.000000 qiskit-experiments-0.5.0/qiskit_experiments.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-28 19:32:12.000000 qiskit-experiments-0.5.0/qiskit_experiments.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-28 19:32:12.000000 qiskit-experiments-0.5.0/qiskit_experiments.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 19:32:12.464128 qiskit-experiments-0.5.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2542 2023-03-28 19:32:01.000000 qiskit-experiments-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:39:00.675049 qiskit-experiments-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-04-19 01:39:00.675049 qiskit-experiments-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:39:00.599048 qiskit-experiments-0.5.1/qiskit_experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:39:00.603048 qiskit-experiments-0.5.1/qiskit_experiments/calibration_management/
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/calibration_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15765 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/calibration_management/base_calibration_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17004 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/calibration_management/basis_gate_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/calibration_management/calibration_key_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/calibration_management/calibration_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70393 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/calibration_management/calibrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/calibration_management/control_channel_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/calibration_management/parameter_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7115 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/calibration_management/update_library.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:39:00.607048 qiskit-experiments-0.5.1/qiskit_experiments/curve_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/curve_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17468 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/curve_analysis/base_curve_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15107 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/curve_analysis/composite_curve_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18942 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/curve_analysis/curve_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22146 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/curve_analysis/curve_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12185 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/curve_analysis/curve_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/curve_analysis/fit_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11532 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/curve_analysis/guess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:39:00.611048 qiskit-experiments-0.5.1/qiskit_experiments/curve_analysis/standard_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/curve_analysis/standard_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/curve_analysis/standard_analysis/bloch_trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/curve_analysis/standard_analysis/decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/curve_analysis/standard_analysis/error_amplification_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/curve_analysis/standard_analysis/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/curve_analysis/standard_analysis/oscillation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/curve_analysis/standard_analysis/resonance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17350 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/curve_analysis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:39:00.615048 qiskit-experiments-0.5.1/qiskit_experiments/curve_analysis/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/curve_analysis/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12035 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/curve_analysis/visualization/base_drawer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/curve_analysis/visualization/curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16466 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/curve_analysis/visualization/fit_result_plotters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15036 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/curve_analysis/visualization/mpl_drawer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/curve_analysis/visualization/style.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:39:00.619048 qiskit-experiments-0.5.1/qiskit_experiments/data_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/data_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/data_processing/data_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12779 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/data_processing/data_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/data_processing/discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/data_processing/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42185 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/data_processing/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/data_processing/processor_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/data_processing/sklearn_discriminators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:39:00.619048 qiskit-experiments-0.5.1/qiskit_experiments/database_service/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/database_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/database_service/device_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/database_service/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/database_service/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:39:00.623048 qiskit-experiments-0.5.1/qiskit_experiments/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17743 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/framework/analysis_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/framework/analysis_result_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/framework/backend_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15017 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/framework/backend_timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/framework/base_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16475 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/framework/base_experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:39:00.627048 qiskit-experiments-0.5.1/qiskit_experiments/framework/composite/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/framework/composite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/framework/composite/batch_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15898 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/framework/composite/composite_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8034 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/framework/composite/composite_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/framework/composite/parallel_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/framework/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84134 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/framework/experiment_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23184 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/framework/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/framework/matplotlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9473 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/framework/restless_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/framework/store_init_args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:39:00.627048 qiskit-experiments-0.5.1/qiskit_experiments/library/
+-rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:39:00.631048 qiskit-experiments-0.5.1/qiskit_experiments/library/calibration/
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/calibration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/calibration/fine_amplitude.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8471 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/calibration/fine_drag_cal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/calibration/fine_frequency_cal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/calibration/frequency_cal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/calibration/half_angle_cal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11102 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/calibration/rough_amplitude_cal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/calibration/rough_drag_cal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/calibration/rough_frequency.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:39:00.639048 qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:39:00.647049 qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/analysis/correlated_readout_error_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/analysis/cr_hamiltonian_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/analysis/drag_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/analysis/fine_amplitude_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/analysis/local_readout_error_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/analysis/multi_state_discrimination_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/analysis/ramsey_xy_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/analysis/readout_angle_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/analysis/resonator_spectroscopy_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/analysis/t1_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/analysis/t2hahn_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/analysis/t2ramsey_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/analysis/tphi_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/analysis/zz_ramsey_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/correlated_readout_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24596 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/cr_hamiltonian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7927 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/drag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/ef_spectroscopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18587 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/fine_amplitude.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/fine_drag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/fine_frequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/half_angle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/local_readout_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/multi_state_discrimination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/qubit_spectroscopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/rabi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9236 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/ramsey_xy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/readout_angle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11665 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/resonator_spectroscopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/spectroscopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7527 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/t2hahn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/t2ramsey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/tphi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15761 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/zz_ramsey.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:39:00.651049 qiskit-experiments-0.5.1/qiskit_experiments/library/quantum_volume/
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/quantum_volume/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/quantum_volume/qv_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7758 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/quantum_volume/qv_experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:39:00.655049 qiskit-experiments-0.5.1/qiskit_experiments/library/randomized_benchmarking/
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/randomized_benchmarking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20032 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/randomized_benchmarking/clifford_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:39:00.655049 qiskit-experiments-0.5.1/qiskit_experiments/library/randomized_benchmarking/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/randomized_benchmarking/data/clifford_compose_1q.npz
+-rw-r--r--   0 runner    (1001) docker     (123)   434028 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/randomized_benchmarking/data/clifford_compose_2q_sparse.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/randomized_benchmarking/data/clifford_inverse_1q.npz
+-rw-r--r--   0 runner    (1001) docker     (123)    19116 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/randomized_benchmarking/data/clifford_inverse_2q.npz
+-rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/randomized_benchmarking/interleaved_rb_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/randomized_benchmarking/interleaved_rb_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14888 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/randomized_benchmarking/rb_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/randomized_benchmarking/rb_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19508 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/randomized_benchmarking/standard_rb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:39:00.659049 qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:39:00.663049 qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/basis/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/basis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7408 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/basis/base_basis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/basis/cache_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29737 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/basis/local_basis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/basis/pauli_basis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:39:00.667049 qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/fitters/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/fitters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20672 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/fitters/cvxpy_lstsq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10343 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/fitters/cvxpy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7113 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/fitters/fitter_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13316 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/fitters/lininv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12083 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/fitters/lstsq_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/fitters/postprocess_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/fitters/scipy_lstsq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/mit_qpt_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/mit_qst_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/mit_tomography_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/qpt_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/qpt_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/qst_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/qst_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19670 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/tomography_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13646 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/tomography_experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:39:00.667049 qiskit-experiments-0.5.1/qiskit_experiments/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/test/fake_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20066 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/test/fake_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31398 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/test/mock_iq_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37323 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/test/mock_iq_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/test/noisy_delay_aer_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23891 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/test/pulse_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/test/t2hahn_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/test/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:39:00.671049 qiskit-experiments-0.5.1/qiskit_experiments/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:39:00.671049 qiskit-experiments-0.5.1/qiskit_experiments/visualization/drawers/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/visualization/drawers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23669 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/visualization/drawers/base_drawer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/visualization/drawers/legacy_curve_compat_drawer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23317 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/visualization/drawers/mpl_drawer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:39:00.675049 qiskit-experiments-0.5.1/qiskit_experiments/visualization/plotters/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/visualization/plotters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25866 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/visualization/plotters/base_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/visualization/plotters/curve_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16098 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/visualization/plotters/iq_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/visualization/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/visualization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8900 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/qiskit_experiments/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:39:00.603048 qiskit-experiments-0.5.1/qiskit_experiments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-04-19 01:39:00.000000 qiskit-experiments-0.5.1/qiskit_experiments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10175 2023-04-19 01:39:00.000000 qiskit-experiments-0.5.1/qiskit_experiments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 01:39:00.000000 qiskit-experiments-0.5.1/qiskit_experiments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 01:39:00.000000 qiskit-experiments-0.5.1/qiskit_experiments.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-19 01:39:00.000000 qiskit-experiments-0.5.1/qiskit_experiments.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-19 01:39:00.000000 qiskit-experiments-0.5.1/qiskit_experiments.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 01:39:00.675049 qiskit-experiments-0.5.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2591 2023-04-19 01:38:51.000000 qiskit-experiments-0.5.1/setup.py
```

### Comparing `qiskit-experiments-0.5.0/LICENSE.txt` & `qiskit-experiments-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/PKG-INFO` & `qiskit-experiments-0.5.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-experiments
-Version: 0.5.0
+Version: 0.5.1
 Summary: Software for developing quantum computing programs
 Home-page: https://github.com/Qiskit/qiskit-experiments
 Author: Qiskit Development Team
 Author-email: hello@qiskit.org
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/Qiskit/qiskit-experiments/issues
 Project-URL: Documentation, https://qiskit.org/documentation/
@@ -35,15 +35,19 @@
         simple questions.
         For questions that are more suited for a forum we use the Qiskit tag in 
         [Stack Exchange](https://quantumcomputing.stackexchange.com/questions/tagged/qiskit).
         
         ## Authors and Citation
         
         Qiskit Experiments is the work of [many people](https://github.com/Qiskit/qiskit-experiments/graphs/contributors) who contribute
-        to the project at different levels. If you use Qiskit, please cite as per the included [BibTeX file](https://github.com/Qiskit/qiskit/blob/master/Qiskit.bib).
+        to the project at different levels. If you use Qiskit Experiments, please cite
+        the following references:
+        
+        - Qiskit, as per the [BibTeX file](https://github.com/Qiskit/qiskit-metapackage/blob/master/Qiskit.bib).
+        - Qiskit Experiments, as per the [DOI](https://doi.org/10.5281/zenodo.7737483).
         
         ## License
         
         [Apache License 2.0](LICENSE.txt)
         
         
 Keywords: qiskit sdk quantum
```

### Comparing `qiskit-experiments-0.5.0/README.md` & `qiskit-experiments-0.5.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -24,13 +24,17 @@
 simple questions.
 For questions that are more suited for a forum we use the Qiskit tag in 
 [Stack Exchange](https://quantumcomputing.stackexchange.com/questions/tagged/qiskit).
 
 ## Authors and Citation
 
 Qiskit Experiments is the work of [many people](https://github.com/Qiskit/qiskit-experiments/graphs/contributors) who contribute
-to the project at different levels. If you use Qiskit, please cite as per the included [BibTeX file](https://github.com/Qiskit/qiskit/blob/master/Qiskit.bib).
+to the project at different levels. If you use Qiskit Experiments, please cite
+the following references:
+
+- Qiskit, as per the [BibTeX file](https://github.com/Qiskit/qiskit-metapackage/blob/master/Qiskit.bib).
+- Qiskit Experiments, as per the [DOI](https://doi.org/10.5281/zenodo.7737483).
 
 ## License
 
 [Apache License 2.0](LICENSE.txt)
```

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/__init__.py` & `qiskit-experiments-0.5.1/qiskit_experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/calibration_management/__init__.py` & `qiskit-experiments-0.5.1/qiskit_experiments/calibration_management/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/calibration_management/base_calibration_experiment.py` & `qiskit-experiments-0.5.1/qiskit_experiments/calibration_management/base_calibration_experiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -312,18 +312,22 @@
 
         Returns:
             A quantum circuit that has the same number of qubits as the backend and where
             the physical qubits of the experiment have been properly mapped.
         """
         initial_layout = Layout.from_intlist(list(self.physical_qubits), *circuit.qregs)
 
+        coupling_map = self._backend_data.coupling_map
+        if coupling_map is not None:
+            coupling_map = CouplingMap(self._backend_data.coupling_map)
+
         layout = PassManager(
             [
                 SetLayout(initial_layout),
-                FullAncillaAllocation(CouplingMap(self._backend_data.coupling_map)),
+                FullAncillaAllocation(coupling_map),
                 EnlargeWithAncilla(),
                 ApplyLayout(),
             ]
         )
 
         return StagedPassManager(["layout"], layout=layout).run(circuit)
```

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/calibration_management/basis_gate_library.py` & `qiskit-experiments-0.5.1/qiskit_experiments/calibration_management/basis_gate_library.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,16 +216,17 @@
         """Setup the schedules.
 
         Args:
             basis_gates: The basis gates to generate.
             default_values: Default values for the parameters this dictionary can contain
                 the following keys: "duration", "amp", "β", and "σ". If "σ" is not provided
                 this library will take one fourth of the pulse duration as default value.
-            link_parameters: If set to True then the amplitude and DRAG parameters of the
-                X and Y gates will be linked as well as those of the SX and SY gates.
+            link_parameters: If set to ``True``, then the amplitude and DRAG parameters of the
+                :math:`X` and :math:`Y` gates will be linked as well as those of
+                the :math:`SX` and :math:`SY` gates.
         """
         self._link_parameters = link_parameters
 
         extra_kwargs = {"link_parameters": link_parameters}
 
         super().__init__(basis_gates, default_values, **extra_kwargs)
```

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/calibration_management/calibration_key_types.py` & `qiskit-experiments-0.5.1/qiskit_experiments/calibration_management/calibration_key_types.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/calibration_management/calibration_utils.py` & `qiskit-experiments-0.5.1/qiskit_experiments/calibration_management/calibration_utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/calibration_management/calibrations.py` & `qiskit-experiments-0.5.1/qiskit_experiments/calibration_management/calibrations.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/calibration_management/control_channel_map.py` & `qiskit-experiments-0.5.1/qiskit_experiments/calibration_management/control_channel_map.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/calibration_management/parameter_value.py` & `qiskit-experiments-0.5.1/qiskit_experiments/calibration_management/parameter_value.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/calibration_management/update_library.py` & `qiskit-experiments-0.5.1/qiskit_experiments/calibration_management/update_library.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/curve_analysis/__init__.py` & `qiskit-experiments-0.5.1/qiskit_experiments/curve_analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/curve_analysis/base_curve_analysis.py` & `qiskit-experiments-0.5.1/qiskit_experiments/curve_analysis/base_curve_analysis.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/curve_analysis/composite_curve_analysis.py` & `qiskit-experiments-0.5.1/qiskit_experiments/curve_analysis/composite_curve_analysis.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/curve_analysis/curve_analysis.py` & `qiskit-experiments-0.5.1/qiskit_experiments/curve_analysis/curve_analysis.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/curve_analysis/curve_data.py` & `qiskit-experiments-0.5.1/qiskit_experiments/curve_analysis/curve_data.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/curve_analysis/curve_fit.py` & `qiskit-experiments-0.5.1/qiskit_experiments/curve_analysis/curve_fit.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/curve_analysis/fit_function.py` & `qiskit-experiments-0.5.1/qiskit_experiments/curve_analysis/fit_function.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/curve_analysis/guess.py` & `qiskit-experiments-0.5.1/qiskit_experiments/curve_analysis/guess.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/curve_analysis/standard_analysis/__init__.py` & `qiskit-experiments-0.5.1/qiskit_experiments/curve_analysis/standard_analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/curve_analysis/standard_analysis/bloch_trajectory.py` & `qiskit-experiments-0.5.1/qiskit_experiments/curve_analysis/standard_analysis/bloch_trajectory.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/curve_analysis/standard_analysis/decay.py` & `qiskit-experiments-0.5.1/qiskit_experiments/curve_analysis/standard_analysis/decay.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/curve_analysis/standard_analysis/error_amplification_analysis.py` & `qiskit-experiments-0.5.1/qiskit_experiments/curve_analysis/standard_analysis/error_amplification_analysis.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/curve_analysis/standard_analysis/gaussian.py` & `qiskit-experiments-0.5.1/qiskit_experiments/curve_analysis/standard_analysis/gaussian.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/curve_analysis/standard_analysis/oscillation.py` & `qiskit-experiments-0.5.1/qiskit_experiments/curve_analysis/standard_analysis/oscillation.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/curve_analysis/standard_analysis/resonance.py` & `qiskit-experiments-0.5.1/qiskit_experiments/curve_analysis/standard_analysis/resonance.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/curve_analysis/utils.py` & `qiskit-experiments-0.5.1/qiskit_experiments/curve_analysis/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/curve_analysis/visualization/__init__.py` & `qiskit-experiments-0.5.1/qiskit_experiments/curve_analysis/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/curve_analysis/visualization/base_drawer.py` & `qiskit-experiments-0.5.1/qiskit_experiments/curve_analysis/visualization/base_drawer.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/curve_analysis/visualization/curves.py` & `qiskit-experiments-0.5.1/qiskit_experiments/curve_analysis/visualization/curves.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/curve_analysis/visualization/fit_result_plotters.py` & `qiskit-experiments-0.5.1/qiskit_experiments/curve_analysis/visualization/fit_result_plotters.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/curve_analysis/visualization/mpl_drawer.py` & `qiskit-experiments-0.5.1/qiskit_experiments/curve_analysis/visualization/mpl_drawer.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     "0.6",
     msg="Plotting and drawing of analysis figures has been replaced with the new"
     "`qiskit_experiments.visualization` module.",
 )
 class MplCurveDrawer(BaseCurveDrawer):
     """Curve drawer for MatplotLib backend."""
 
-    DefaultMarkers = MarkerStyle().filled_markers
+    DefaultMarkers = MarkerStyle.filled_markers
     DefaultColors = tab10.colors
 
     class PrefixFormatter(Formatter):
         """Matplotlib axis formatter to detach prefix.
 
         If a value is, e.g., x=1000.0 and the factor is 1000, then it will be shown
         as 1.0 in the ticks and its unit will be shown with the prefactor 'k'
```

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/curve_analysis/visualization/style.py` & `qiskit-experiments-0.5.1/qiskit_experiments/curve_analysis/visualization/style.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/data_processing/__init__.py` & `qiskit-experiments-0.5.1/qiskit_experiments/data_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/data_processing/data_action.py` & `qiskit-experiments-0.5.1/qiskit_experiments/data_processing/data_action.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/data_processing/data_processor.py` & `qiskit-experiments-0.5.1/qiskit_experiments/data_processing/data_processor.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/data_processing/discriminator.py` & `qiskit-experiments-0.5.1/qiskit_experiments/data_processing/discriminator.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/data_processing/exceptions.py` & `qiskit-experiments-0.5.1/qiskit_experiments/data_processing/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/data_processing/nodes.py` & `qiskit-experiments-0.5.1/qiskit_experiments/data_processing/nodes.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/data_processing/processor_library.py` & `qiskit-experiments-0.5.1/qiskit_experiments/data_processing/processor_library.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/data_processing/sklearn_discriminators.py` & `qiskit-experiments-0.5.1/qiskit_experiments/data_processing/sklearn_discriminators.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/database_service/__init__.py` & `qiskit-experiments-0.5.1/qiskit_experiments/database_service/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/database_service/device_component.py` & `qiskit-experiments-0.5.1/qiskit_experiments/database_service/device_component.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/database_service/exceptions.py` & `qiskit-experiments-0.5.1/qiskit_experiments/database_service/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/database_service/utils.py` & `qiskit-experiments-0.5.1/qiskit_experiments/database_service/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/exceptions.py` & `qiskit-experiments-0.5.1/qiskit_experiments/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/framework/__init__.py` & `qiskit-experiments-0.5.1/qiskit_experiments/framework/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/framework/analysis_result.py` & `qiskit-experiments-0.5.1/qiskit_experiments/framework/analysis_result.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/framework/analysis_result_data.py` & `qiskit-experiments-0.5.1/qiskit_experiments/framework/analysis_result_data.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/framework/backend_data.py` & `qiskit-experiments-0.5.1/qiskit_experiments/framework/backend_data.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/framework/backend_timing.py` & `qiskit-experiments-0.5.1/qiskit_experiments/framework/backend_timing.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/framework/base_analysis.py` & `qiskit-experiments-0.5.1/qiskit_experiments/framework/base_analysis.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/framework/base_experiment.py` & `qiskit-experiments-0.5.1/qiskit_experiments/framework/base_experiment.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/framework/composite/__init__.py` & `qiskit-experiments-0.5.1/qiskit_experiments/framework/composite/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/framework/composite/batch_experiment.py` & `qiskit-experiments-0.5.1/qiskit_experiments/framework/composite/batch_experiment.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/framework/composite/composite_analysis.py` & `qiskit-experiments-0.5.1/qiskit_experiments/framework/composite/composite_analysis.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/framework/composite/composite_experiment.py` & `qiskit-experiments-0.5.1/qiskit_experiments/framework/composite/composite_experiment.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/framework/composite/parallel_experiment.py` & `qiskit-experiments-0.5.1/qiskit_experiments/framework/composite/parallel_experiment.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/framework/configs.py` & `qiskit-experiments-0.5.1/qiskit_experiments/framework/configs.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/framework/experiment_data.py` & `qiskit-experiments-0.5.1/qiskit_experiments/framework/experiment_data.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/framework/json.py` & `qiskit-experiments-0.5.1/qiskit_experiments/framework/json.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/framework/matplotlib.py` & `qiskit-experiments-0.5.1/qiskit_experiments/framework/matplotlib.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/framework/restless_mixin.py` & `qiskit-experiments-0.5.1/qiskit_experiments/framework/restless_mixin.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/framework/store_init_args.py` & `qiskit-experiments-0.5.1/qiskit_experiments/framework/store_init_args.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/__init__.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,14 +119,15 @@
 See :doc:`/tutorials/calibrations` for examples.
 
 .. autosummary::
     :toctree: ../stubs/
     :template: autosummary/experiment.rst
 
     ~calibration.RoughFrequencyCal
+    ~calibration.RoughEFFrequencyCal
     ~calibration.FrequencyCal
     ~calibration.FineFrequencyCal
     ~calibration.RoughDragCal
     ~calibration.FineXDragCal
     ~calibration.FineSXDragCal
     ~calibration.FineDragCal
     ~calibration.FineAmplitudeCal
@@ -146,14 +147,15 @@
     RoughAmplitudeCal,
     RoughXSXAmplitudeCal,
     EFRoughXSXAmplitudeCal,
     FineAmplitudeCal,
     FineXAmplitudeCal,
     FineSXAmplitudeCal,
     RoughFrequencyCal,
+    RoughEFFrequencyCal,
     FrequencyCal,
     FineFrequencyCal,
     HalfAngleCal,
 )
 from .characterization import (
     T1,
     T2Hahn,
```

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/calibration/__init__.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/calibration/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 Calibrations management
 =======================
 
 See :mod:`.calibration_management`.
 """
 
-from .rough_frequency import RoughFrequencyCal
+from .rough_frequency import RoughFrequencyCal, RoughEFFrequencyCal
 from .rough_drag_cal import RoughDragCal
 from .rough_amplitude_cal import RoughAmplitudeCal, RoughXSXAmplitudeCal, EFRoughXSXAmplitudeCal
 from .fine_amplitude import FineAmplitudeCal, FineXAmplitudeCal, FineSXAmplitudeCal
 from .fine_drag_cal import FineDragCal, FineXDragCal, FineSXDragCal
 from .frequency_cal import FrequencyCal
 from .fine_frequency_cal import FineFrequencyCal
 from .half_angle_cal import HalfAngleCal
```

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/calibration/fine_amplitude.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/calibration/fine_amplitude.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/calibration/fine_drag_cal.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/calibration/fine_drag_cal.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/calibration/fine_frequency_cal.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/calibration/fine_frequency_cal.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/calibration/frequency_cal.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/calibration/frequency_cal.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/calibration/half_angle_cal.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/calibration/half_angle_cal.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/calibration/rough_amplitude_cal.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/calibration/rough_amplitude_cal.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,38 +216,41 @@
             AnglesSchedules(
                 target_angle=np.pi / 2, parameter="amp", schedule="sx", previous_value=None
             ),
         ]
 
 
 class EFRoughXSXAmplitudeCal(RoughAmplitudeCal):
-    """A rough amplitude calibration of x and sx gates on the 1<->2 transition."""
+    r"""A rough amplitude calibration of :math:`X` and :math:`SX` gates on the
+    :math:`|1\rangle` <-> :math:`|2\rangle` transition.
+    """
 
     __outcome__ = "rabi_rate_12"
 
     @qubit_deprecate()
     def __init__(
         self,
         physical_qubits: Sequence[int],
         calibrations: Calibrations,
         amplitudes: Iterable[float] = None,
         backend: Optional[Backend] = None,
         ef_pulse_label: str = "12",
     ):
-        r"""A rough amplitude calibration that updates both the sx and x pulses on 1<->2.
+        r"""A rough amplitude calibration that updates both the sx and x pulses on the
+        :math:`|1\rangle` <-> :math:`|2\rangle` transition.
 
         Args:
             physical_qubits: Sequence containing the index of the qubit
                 (technically a qutrit) to run on.
             calibrations: The calibrations instance that stores the pulse schedules.
             amplitudes: The amplitudes to scan.
             backend: Optional, the backend to run the experiment on.
             ef_pulse_label: A label that is post-pended to "x" and "sx" to obtain the name
                 of the pulses that drive a :math:`\pi` and :math:`\pi/2` rotation on
-                the 1<->2 transition.
+                the :math:`|1\rangle` <-> :math:`|2\rangle` transition.
         """
         super().__init__(
             physical_qubits,
             calibrations,
             schedule_name="x" + ef_pulse_label,
             amplitudes=amplitudes,
             backend=backend,
```

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/calibration/rough_drag_cal.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/calibration/rough_drag_cal.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 )
 from qiskit_experiments.calibration_management.update_library import BaseUpdater
 from qiskit_experiments.library.characterization.drag import RoughDrag
 from qiskit_experiments.warnings import qubit_deprecate
 
 
 class RoughDragCal(BaseCalibrationExperiment, RoughDrag):
-    """A calibration version of the Drag experiment.
+    """A calibration version of the :class:`.RoughDrag` experiment.
 
     # section: manual
         :ref:`DRAG Calibration`
 
     """
 
     @qubit_deprecate()
@@ -43,23 +43,23 @@
         backend: Optional[Backend] = None,
         schedule_name: str = "x",
         betas: Iterable[float] = None,
         cal_parameter_name: Optional[str] = "β",
         auto_update: bool = True,
         group: str = "default",
     ):
-        r"""see class :class:`RoughDrag` for details.
+        r"""see class :class:`.RoughDrag` for details.
 
         Args:
             physical_qubits: Sequence containing the qubit for which to run the
-                rough drag calibration.
+                rough DRAG calibration.
             calibrations: The calibrations instance with the schedules.
             backend: Optional, the backend to run the experiment on.
             schedule_name: The name of the schedule to calibrate. Defaults to "x".
-            betas: A list of drag parameter values to scan. If None is given 51 betas ranging
+            betas: A list of DRAG parameter values to scan. If None is given 51 betas ranging
                 from -5 to 5 will be scanned.
             cal_parameter_name: The name of the parameter in the schedule to update.
                 Defaults to "β".
             auto_update: Whether or not to automatically update the calibrations. By
                 default this variable is set to True.
             group: The group of calibration parameters to use. The default value is "default".
         """
```

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/calibration/rough_frequency.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/calibration/rough_frequency.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,27 +24,28 @@
 from qiskit_experiments.calibration_management.base_calibration_experiment import (
     BaseCalibrationExperiment,
 )
 from qiskit_experiments.warnings import qubit_deprecate
 
 
 class RoughFrequencyCal(BaseCalibrationExperiment, QubitSpectroscopy):
-    """A calibration experiment that runs QubitSpectroscopy."""
+    """A calibration experiment that runs :class:`.QubitSpectroscopy` to calibrate the qubit
+    transition frequency."""
 
     @qubit_deprecate()
     def __init__(
         self,
         physical_qubits: Sequence[int],
         calibrations: Calibrations,
         frequencies: Iterable[float],
         backend: Optional[Backend] = None,
         auto_update: bool = True,
         absolute: bool = True,
     ):
-        """See :class:`QubitSpectroscopy` for detailed documentation.
+        """See :class:`.QubitSpectroscopy` for detailed documentation.
 
         Args:
             physical_qubits: List with the qubit on which to run spectroscopy.
             calibrations: If calibrations is given then running the experiment may update the values
                 of the frequencies stored in calibrations.
             frequencies: The frequencies to scan in the experiment, in Hz.
             backend: Optional, the backend to run the experiment on.
@@ -69,47 +70,52 @@
 
     def _attach_calibrations(self, circuit: QuantumCircuit):
         """QubitSpectroscopy already has the schedules attached in the program circuits."""
         pass
 
 
 class RoughEFFrequencyCal(BaseCalibrationExperiment, EFSpectroscopy):
-    """A calibration experiment that runs QubitSpectroscopy."""
+    r"""A calibration experiment that runs :class:`.QubitSpectroscopy` for the
+    :math:`|1\rangle` <-> :math:`|2\rangle` transition.
+    """
 
     __updater__ = Frequency
 
     # pylint: disable=super-init-not-called
     def __init__(
         self,
         physical_qubits: Sequence[int],
         calibrations: Calibrations,
         frequencies: Iterable[float],
+        backend: Optional[Backend] = None,
         auto_update: bool = True,
         absolute: bool = True,
     ):
-        """See :class:`QubitSpectroscopy` for detailed documentation.
+        """See :class:`.QubitSpectroscopy` for detailed documentation.
 
         Args:
             physical_qubits: List containing the qubit on which to run spectroscopy.
             calibrations: If calibrations is given then running the experiment may update the values
                 of the frequencies stored in calibrations.
             frequencies: The frequencies to scan in the experiment, in Hz.
+            backend: Optional, the backend to run the experiment on.
             auto_update: If set to True, which is the default, then the experiment will
                 automatically update the frequency in the calibrations.
             absolute: Boolean to specify if the frequencies are absolute or relative to the
                 qubit frequency in the backend.
 
         Raises:
             QiskitError: If there are less than three frequency shifts.
 
         """
         super().__init__(
             calibrations,
             physical_qubits,
             frequencies,
+            backend,
             absolute,
             cal_parameter_name="f12",
             updater=Frequency,
             auto_update=auto_update,
         )
 
     def _attach_calibrations(self, circuit: QuantumCircuit):
```

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/__init__.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/analysis/__init__.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/analysis/correlated_readout_error_analysis.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/analysis/correlated_readout_error_analysis.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/analysis/cr_hamiltonian_analysis.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/analysis/cr_hamiltonian_analysis.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/analysis/drag_analysis.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/analysis/drag_analysis.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/analysis/fine_amplitude_analysis.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/analysis/fine_amplitude_analysis.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/analysis/local_readout_error_analysis.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/analysis/local_readout_error_analysis.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/analysis/multi_state_discrimination_analysis.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/analysis/multi_state_discrimination_analysis.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/analysis/ramsey_xy_analysis.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/analysis/ramsey_xy_analysis.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/analysis/readout_angle_analysis.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/analysis/readout_angle_analysis.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/analysis/resonator_spectroscopy_analysis.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/analysis/resonator_spectroscopy_analysis.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/analysis/t1_analysis.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/analysis/t1_analysis.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/analysis/t2hahn_analysis.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/analysis/t2hahn_analysis.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/analysis/t2ramsey_analysis.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/analysis/t2ramsey_analysis.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/analysis/tphi_analysis.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/analysis/tphi_analysis.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/analysis/zz_ramsey_analysis.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/analysis/zz_ramsey_analysis.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/correlated_readout_error.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/correlated_readout_error.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/cr_hamiltonian.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/cr_hamiltonian.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/drag.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/drag.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/ef_spectroscopy.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/ef_spectroscopy.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/fine_amplitude.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/fine_amplitude.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/fine_drag.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/fine_drag.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,42 +86,42 @@
         that the instantaneous Z-angle error induced by a single pulse is
 
         .. math::
 
             \bar\delta(t) = {\rm d}\beta\, \Omega^2_x(t)
 
 
-        We can integrate :math:`\bar{\delta}(t)`, i.e. the instantaneous Z-angle rotation error,
+        We can integrate :math:`\bar{\delta}(t)`, i.e. the instantaneous :math:`Z`-angle rotation error,
         to obtain the total rotation angle error per pulse, :math:`{\rm d}\theta`:
 
         .. math::
 
            {\rm d}\theta = \int\bar\delta(t){\rm d}t = {\rm d}\beta \int\Omega^2_x(t){\rm d}t
 
         If we assume a Gaussian pulse, i.e. :math:`\Omega_x(t)=A\exp[-t^2/(2\sigma^2)]`
         then the integral of :math:`\Omega_x^2(t)` in the equation above results in
         :math:`A^2\sigma\sqrt{\pi}`. Furthermore, the integral of :math:`\Omega_x(t)` is
         :math:`A\sigma\sqrt{\pi/2}=\theta_\text{target}`, where :math:`\theta_\text{target}`
         is the target rotation angle, i.e. the area under the pulse. This last point allows
         us to rewrite :math:`A^2\sigma\sqrt{\pi}` as
-        :math:`\theta^2_\text{target}/(2\sigma\sqrt{\pi})`. The total Z angle error per pulse
+        :math:`\theta^2_\text{target}/(2\sigma\sqrt{\pi})`. The total :math:`Z` angle error per pulse
         is therefore
 
         .. math::
 
            {\rm d}\theta=
             \int\bar\delta(t){\rm d}t={\rm d}\beta\,\frac{\theta^2_\text{target}}{2\sigma\sqrt{\pi}}
 
-        Here, :math:`{\rm d}\theta` is the Z angle error per pulse. The qubit population produced by
-        the gate sequence shown above is used to measure :math:`{\rm d}\theta`. Indeed, each
-        gate pair Rp - Rm will produce a small unwanted Z - rotation out of the ZX plane with a
-        magnitude :math:`2\,{\rm d}\theta`. The total rotation out of the ZX plane is then mapped
-        to a qubit population by the final Post gate. Inverting the relation above after cancelling
-        out the factor of two due to the Rp - Rm pulse pair yields the error in :math:`\beta` that
-        produced the rotation error :math:`{\rm d}\theta` as
+        Here, :math:`{\rm d}\theta` is the :math:`Z` angle error per pulse. The qubit population
+        produced by the gate sequence shown above is used to measure :math:`{\rm d}\theta`. Indeed,
+        each gate pair Rp - Rm will produce a small unwanted :math:`Z`-rotation out of the
+        :math:`ZX` plane with a magnitude :math:`2\,{\rm d}\theta`. The total rotation out of the
+        :math:`ZX` plane is then mapped to a qubit population by the final Post gate. Inverting the
+        relation above after cancelling out the factor of two due to the Rp - Rm pulse pair yields
+        the error in :math:`\beta` that produced the rotation error :math:`{\rm d}\theta` as
 
         .. math::
 
             {\rm d}\beta=\frac{\sqrt{\pi}\,{\rm d}\theta\sigma}{ \theta_\text{target}^2}.
 
         This is the correction formula in the FineDRAG Updater.
 
@@ -264,15 +264,15 @@
     @staticmethod
     def _pre_circuit() -> QuantumCircuit:
         """Return the quantum circuit done before the Rp - Rz - Rp - Rz gates."""
         return QuantumCircuit(1)
 
 
 class FineSXDrag(FineDrag):
-    """Class to fine characterize the DRAG parameter of an SX gate."""
+    """Class to fine characterize the DRAG parameter of an :math:`SX` gate."""
 
     @qubit_deprecate()
     def __init__(self, physical_qubits: Sequence[int], backend: Optional[Backend] = None):
         """Initialize the experiment."""
         super().__init__(physical_qubits, SXGate(), backend=backend)
 
     @classmethod
```

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/fine_frequency.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/fine_frequency.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/half_angle.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/half_angle.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/local_readout_error.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/local_readout_error.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/multi_state_discrimination.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/multi_state_discrimination.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/qubit_spectroscopy.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/qubit_spectroscopy.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/rabi.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/rabi.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 from qiskit_experiments.framework import BaseExperiment, Options
 from qiskit_experiments.framework.restless_mixin import RestlessMixin
 from qiskit_experiments.curve_analysis import ParameterRepr, OscillationAnalysis
 from qiskit_experiments.warnings import qubit_deprecate
 
 
 class Rabi(BaseExperiment, RestlessMixin):
-    """An experiment that scans a pulse amplitude to calibrate rotations between 0 and 1.
+    r"""An experiment that scans a pulse amplitude to calibrate rotations on the :math:`|0\rangle`
+    <-> :math:`|1\rangle` transition.
 
     # section: overview
 
         The circuits have a custom rabi gate with the pulse schedule attached to it
         through the calibrations. The circuits are of the form:
 
         .. parsed-literal::
@@ -181,24 +182,25 @@
         for run_opt in ["meas_level", "meas_return"]:
             if hasattr(self.run_options, run_opt):
                 metadata[run_opt] = getattr(self.run_options, run_opt)
         return metadata
 
 
 class EFRabi(Rabi):
-    """An experiment that scans the amplitude of a pulse inducing rotations between 1 and 2.
+    r"""An experiment that scans the amplitude of a pulse inducing rotations on the
+     :math:`|1\rangle` <-> :math:`|2\rangle` transition.
 
     # section: overview
 
         This experiment is a subclass of the :class:`Rabi` experiment but takes place between
         the first and second excited state. An initial X gate populates the first excited state.
-        The Rabi pulse is applied on the 1 <-> 2 transition (sometimes also labeled the e <-> f
-        transition). The necessary frequency shift (typically the qubit anharmonicity) is given
-        through the pulse schedule given at initialization. The schedule is then also stored in
-        the experiment options. The circuits are of the form:
+        The Rabi pulse is applied on the :math:`|1\rangle` <-> :math:`|2\rangle` transition
+        (sometimes also labeled the e <-> f transition). The necessary frequency shift (typically
+        the qubit anharmonicity) is given through the pulse schedule given at initialization. The
+        schedule is then also stored in the experiment options. The circuits are of the form:
 
         .. parsed-literal::
 
                        ┌───┐┌───────────┐ ░ ┌─┐
                   q_0: ┤ X ├┤ Rabi(amp) ├─░─┤M├
                        └───┘└───────────┘ ░ └╥┘
             measure: 1/══════════════════════╩═
```

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/ramsey_xy.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/ramsey_xy.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/readout_angle.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/readout_angle.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/resonator_spectroscopy.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/resonator_spectroscopy.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/spectroscopy.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/spectroscopy.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/t1.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/t1.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/t2hahn.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/t2hahn.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/t2ramsey.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/t2ramsey.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/tphi.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/tphi.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/characterization/zz_ramsey.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/characterization/zz_ramsey.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/quantum_volume/__init__.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/quantum_volume/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/quantum_volume/qv_analysis.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/quantum_volume/qv_analysis.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/quantum_volume/qv_experiment.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/quantum_volume/qv_experiment.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/randomized_benchmarking/__init__.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/randomized_benchmarking/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/randomized_benchmarking/clifford_utils.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/randomized_benchmarking/clifford_utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/randomized_benchmarking/data/clifford_compose_1q.npz` & `qiskit-experiments-0.5.1/qiskit_experiments/library/randomized_benchmarking/data/clifford_compose_1q.npz`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/randomized_benchmarking/data/clifford_compose_2q_sparse.npz` & `qiskit-experiments-0.5.1/qiskit_experiments/library/randomized_benchmarking/data/clifford_compose_2q_sparse.npz`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/randomized_benchmarking/data/clifford_inverse_2q.npz` & `qiskit-experiments-0.5.1/qiskit_experiments/library/randomized_benchmarking/data/clifford_inverse_2q.npz`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/randomized_benchmarking/interleaved_rb_analysis.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/randomized_benchmarking/interleaved_rb_analysis.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/randomized_benchmarking/interleaved_rb_experiment.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/randomized_benchmarking/interleaved_rb_experiment.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/randomized_benchmarking/rb_analysis.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/randomized_benchmarking/rb_analysis.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/randomized_benchmarking/rb_utils.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/randomized_benchmarking/rb_utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/randomized_benchmarking/standard_rb.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/randomized_benchmarking/standard_rb.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/__init__.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/basis/__init__.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/basis/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/basis/base_basis.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/basis/base_basis.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/basis/cache_method.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/basis/cache_method.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/basis/local_basis.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/basis/local_basis.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/basis/pauli_basis.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/basis/pauli_basis.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/fitters/__init__.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/fitters/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/fitters/cvxpy_lstsq.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/fitters/cvxpy_lstsq.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/fitters/cvxpy_utils.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/fitters/cvxpy_utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/fitters/fitter_data.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/fitters/fitter_data.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/fitters/lininv.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/fitters/lininv.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/fitters/lstsq_utils.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/fitters/lstsq_utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/fitters/postprocess_fit.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/fitters/postprocess_fit.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/fitters/scipy_lstsq.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/fitters/scipy_lstsq.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/mit_qpt_experiment.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/mit_qpt_experiment.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/mit_qst_experiment.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/mit_qst_experiment.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/mit_tomography_analysis.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/mit_tomography_analysis.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/qpt_analysis.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/qpt_analysis.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/qpt_experiment.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/qpt_experiment.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/qst_analysis.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/qst_analysis.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/qst_experiment.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/qst_experiment.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/tomography_analysis.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/tomography_analysis.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/library/tomography/tomography_experiment.py` & `qiskit-experiments-0.5.1/qiskit_experiments/library/tomography/tomography_experiment.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/test/__init__.py` & `qiskit-experiments-0.5.1/qiskit_experiments/test/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/test/fake_backend.py` & `qiskit-experiments-0.5.1/qiskit_experiments/test/fake_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/test/fake_service.py` & `qiskit-experiments-0.5.1/qiskit_experiments/test/fake_service.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/test/mock_iq_backend.py` & `qiskit-experiments-0.5.1/qiskit_experiments/test/mock_iq_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/test/mock_iq_helpers.py` & `qiskit-experiments-0.5.1/qiskit_experiments/test/mock_iq_helpers.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/test/noisy_delay_aer_simulator.py` & `qiskit-experiments-0.5.1/qiskit_experiments/test/noisy_delay_aer_simulator.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/test/pulse_backend.py` & `qiskit-experiments-0.5.1/qiskit_experiments/test/pulse_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/test/t2hahn_backend.py` & `qiskit-experiments-0.5.1/qiskit_experiments/test/t2hahn_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/test/utils.py` & `qiskit-experiments-0.5.1/qiskit_experiments/test/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/version.py` & `qiskit-experiments-0.5.1/qiskit_experiments/version.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/visualization/__init__.py` & `qiskit-experiments-0.5.1/qiskit_experiments/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/visualization/drawers/__init__.py` & `qiskit-experiments-0.5.1/qiskit_experiments/visualization/drawers/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/visualization/drawers/base_drawer.py` & `qiskit-experiments-0.5.1/qiskit_experiments/visualization/drawers/base_drawer.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/visualization/drawers/legacy_curve_compat_drawer.py` & `qiskit-experiments-0.5.1/qiskit_experiments/visualization/drawers/legacy_curve_compat_drawer.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/visualization/drawers/mpl_drawer.py` & `qiskit-experiments-0.5.1/qiskit_experiments/visualization/drawers/mpl_drawer.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/visualization/plotters/__init__.py` & `qiskit-experiments-0.5.1/qiskit_experiments/visualization/plotters/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/visualization/plotters/base_plotter.py` & `qiskit-experiments-0.5.1/qiskit_experiments/visualization/plotters/base_plotter.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/visualization/plotters/curve_plotter.py` & `qiskit-experiments-0.5.1/qiskit_experiments/visualization/plotters/curve_plotter.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/visualization/plotters/iq_plotter.py` & `qiskit-experiments-0.5.1/qiskit_experiments/visualization/plotters/iq_plotter.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/visualization/style.py` & `qiskit-experiments-0.5.1/qiskit_experiments/visualization/style.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/visualization/utils.py` & `qiskit-experiments-0.5.1/qiskit_experiments/visualization/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments/warnings.py` & `qiskit-experiments-0.5.1/qiskit_experiments/warnings.py`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments.egg-info/PKG-INFO` & `qiskit-experiments-0.5.1/qiskit_experiments.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-experiments
-Version: 0.5.0
+Version: 0.5.1
 Summary: Software for developing quantum computing programs
 Home-page: https://github.com/Qiskit/qiskit-experiments
 Author: Qiskit Development Team
 Author-email: hello@qiskit.org
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/Qiskit/qiskit-experiments/issues
 Project-URL: Documentation, https://qiskit.org/documentation/
@@ -35,15 +35,19 @@
         simple questions.
         For questions that are more suited for a forum we use the Qiskit tag in 
         [Stack Exchange](https://quantumcomputing.stackexchange.com/questions/tagged/qiskit).
         
         ## Authors and Citation
         
         Qiskit Experiments is the work of [many people](https://github.com/Qiskit/qiskit-experiments/graphs/contributors) who contribute
-        to the project at different levels. If you use Qiskit, please cite as per the included [BibTeX file](https://github.com/Qiskit/qiskit/blob/master/Qiskit.bib).
+        to the project at different levels. If you use Qiskit Experiments, please cite
+        the following references:
+        
+        - Qiskit, as per the [BibTeX file](https://github.com/Qiskit/qiskit-metapackage/blob/master/Qiskit.bib).
+        - Qiskit Experiments, as per the [DOI](https://doi.org/10.5281/zenodo.7737483).
         
         ## License
         
         [Apache License 2.0](LICENSE.txt)
         
         
 Keywords: qiskit sdk quantum
```

### Comparing `qiskit-experiments-0.5.0/qiskit_experiments.egg-info/SOURCES.txt` & `qiskit-experiments-0.5.1/qiskit_experiments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qiskit-experiments-0.5.0/setup.py` & `qiskit-experiments-0.5.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,33 +6,32 @@
 # obtain a copy of this license in the LICENSE.txt file in the root directory
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
-"The Qiskit Terra setup file."
+"The Qiskit Experiments setup file."
 
 import os
-import sys
 from setuptools import setup, find_packages
 
-with open("requirements.txt") as f:
+with open("requirements.txt", encoding="utf-8") as f:
     REQUIREMENTS = f.read().splitlines()
 
 
 version_path = os.path.abspath(
     os.path.join(os.path.join(os.path.dirname(__file__), "qiskit_experiments"), "VERSION.txt")
 )
-with open(version_path, "r") as fd:
+with open(version_path, "r", encoding="utf-8") as fd:
     version = fd.read().rstrip()
 
 # Read long description from README.
 README_PATH = os.path.join(os.path.abspath(os.path.dirname(__file__)), "README.md")
-with open(README_PATH) as readme_file:
+with open(README_PATH, encoding="utf-8") as readme_file:
     README = readme_file.read()
 
 setup(
     name="qiskit-experiments",
     version=version,
     description="Software for developing quantum computing programs",
     long_description=README,
```


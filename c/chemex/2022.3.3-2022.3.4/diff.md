# Comparing `tmp/chemex-2022.3.3.tar.gz` & `tmp/chemex-2022.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chemex-2022.3.3.tar", max compression
+gzip compressed data, was "chemex-2022.3.4.tar", max compression
```

## Comparing `chemex-2022.3.3.tar` & `chemex-2022.3.4.tar`

### file list

```diff
@@ -1,117 +1,117 @@
--rw-r--r--   0        0        0    34916 2023-04-19 08:05:00.033306 chemex-2022.3.3/LICENSE.md
--rw-r--r--   0        0        0     1046 2023-04-19 08:05:00.033306 chemex-2022.3.3/README.md
--rw-r--r--   0        0        0      326 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/__init__.py
--rw-r--r--   0        0        0      185 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/__main__.py
--rw-r--r--   0        0        0     2583 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/chemex.py
--rw-r--r--   0        0        0     5876 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/cli.py
--rw-r--r--   0        0        0        0 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/configuration/__init__.py
--rw-r--r--   0        0        0      447 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/configuration/base.py
--rw-r--r--   0        0        0     4619 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/configuration/conditions.py
--rw-r--r--   0        0        0     1491 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/configuration/data.py
--rw-r--r--   0        0        0     1418 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/configuration/experiment.py
--rw-r--r--   0        0        0     4588 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/configuration/methods.py
--rw-r--r--   0        0        0     1971 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/configuration/parameters.py
--rw-r--r--   0        0        0        0 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/containers/__init__.py
--rw-r--r--   0        0        0     3158 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/containers/data.py
--rw-r--r--   0        0        0     1497 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/containers/dataset.py
--rw-r--r--   0        0        0     5406 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/containers/experiment.py
--rw-r--r--   0        0        0     4238 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/containers/experiments.py
--rw-r--r--   0        0        0     3840 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/containers/profile.py
--rw-r--r--   0        0        0        0 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/experiments/__init__.py
--rw-r--r--   0        0        0     4379 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/experiments/builder.py
--rw-r--r--   0        0        0        0 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/experiments/catalog/__init__.py
--rw-r--r--   0        0        0     3678 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/experiments/catalog/cest_13c.py
--rw-r--r--   0        0        0     3588 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/experiments/catalog/cest_15n.py
--rw-r--r--   0        0        0     4060 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/experiments/catalog/cest_15n_cw.py
--rw-r--r--   0        0        0     4353 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/experiments/catalog/cest_15n_tr.py
--rw-r--r--   0        0        0     3682 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/experiments/catalog/cest_1hn_ap.py
--rw-r--r--   0        0        0     4771 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/experiments/catalog/cest_1hn_ip_ap.py
--rw-r--r--   0        0        0     4084 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/experiments/catalog/cest_ch3_1h_ip_ap.py
--rw-r--r--   0        0        0     5188 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/experiments/catalog/coscest_13c.py
--rw-r--r--   0        0        0     5472 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/experiments/catalog/coscest_1hn_ip_ap.py
--rw-r--r--   0        0        0     4782 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/experiments/catalog/cpmg_13c_ip.py
--rw-r--r--   0        0        0     5174 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/experiments/catalog/cpmg_13co_ap.py
--rw-r--r--   0        0        0     4864 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/experiments/catalog/cpmg_15n_ip.py
--rw-r--r--   0        0        0     5702 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/experiments/catalog/cpmg_15n_ip_0013.py
--rw-r--r--   0        0        0     5456 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/experiments/catalog/cpmg_15n_tr.py
--rw-r--r--   0        0        0     7561 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/experiments/catalog/cpmg_15n_tr_0013.py
--rw-r--r--   0        0        0     5192 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/experiments/catalog/cpmg_1hn_ap.py
--rw-r--r--   0        0        0     7764 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/experiments/catalog/cpmg_1hn_ap_0013.py
--rw-r--r--   0        0        0     5016 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/experiments/catalog/cpmg_ch3_13c_h2c.py
--rw-r--r--   0        0        0     5869 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/experiments/catalog/cpmg_ch3_1h_dq.py
--rw-r--r--   0        0        0     6696 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/experiments/catalog/cpmg_ch3_1h_sq.py
--rw-r--r--   0        0        0     5871 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/experiments/catalog/cpmg_ch3_1h_tq.py
--rw-r--r--   0        0        0     7400 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/experiments/catalog/cpmg_ch3_1h_tq_diff.py
--rw-r--r--   0        0        0     4292 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/experiments/catalog/cpmg_ch3_mq.py
--rw-r--r--   0        0        0     4916 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/experiments/catalog/cpmg_chd2_1h_ap.py
--rw-r--r--   0        0        0     5290 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/experiments/catalog/cpmg_hn_dq_zq.py
--rw-r--r--   0        0        0     4412 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/experiments/catalog/dcest_13c.py
--rw-r--r--   0        0        0     4643 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/experiments/catalog/dcest_15n.py
--rw-r--r--   0        0        0     3330 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/experiments/catalog/relaxation_hznz.py
--rw-r--r--   0        0        0     2991 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/experiments/catalog/relaxation_nz.py
--rw-r--r--   0        0        0     2921 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/experiments/catalog/shift_15n_sq.py
--rw-r--r--   0        0        0     3283 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/experiments/catalog/shift_15n_sqmq.py
--rw-r--r--   0        0        0     3235 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/experiments/factories.py
--rw-r--r--   0        0        0      970 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/experiments/loader.py
--rw-r--r--   0        0        0     2671 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/filterers.py
--rw-r--r--   0        0        0     7125 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/messages.py
--rw-r--r--   0        0        0        0 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/models/__init__.py
--rw-r--r--   0        0        0     2753 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/models/constraints.py
--rw-r--r--   0        0        0     1071 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/models/factory.py
--rw-r--r--   0        0        0        0 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/models/kinetic/__init__.py
--rw-r--r--   0        0        0      575 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/models/kinetic/settings_1st.py
--rw-r--r--   0        0        0     1241 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/models/kinetic/settings_2st.py
--rw-r--r--   0        0        0     2954 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/models/kinetic/settings_2st_a_a2.py
--rw-r--r--   0        0        0     2958 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/models/kinetic/settings_2st_a_a3.py
--rw-r--r--   0        0        0     2966 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/models/kinetic/settings_2st_a_a4.py
--rw-r--r--   0        0        0     2722 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/models/kinetic/settings_2st_binding.py
--rw-r--r--   0        0        0     2878 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/models/kinetic/settings_2st_eyring.py
--rw-r--r--   0        0        0     1985 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/models/kinetic/settings_2st_hd.py
--rw-r--r--   0        0        0     1278 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/models/kinetic/settings_2st_rs.py
--rw-r--r--   0        0        0     4590 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/models/kinetic/settings_3st_a_a2_a3.py
--rw-r--r--   0        0        0     4298 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/models/kinetic/settings_3st_a_a2_a4.py
--rw-r--r--   0        0        0     5043 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/models/kinetic/settings_3st_double_binding.py
--rw-r--r--   0        0        0     4463 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/models/kinetic/settings_3st_eyring.py
--rw-r--r--   0        0        0     4079 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/models/kinetic/settings_3st_induced_fit.py
--rw-r--r--   0        0        0     3994 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/models/kinetic/settings_4st_hd.py
--rw-r--r--   0        0        0     4768 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/models/kinetic/settings_nst.py
--rw-r--r--   0        0        0      945 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/models/loader.py
--rw-r--r--   0        0        0     1384 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/models/model.py
--rw-r--r--   0        0        0        0 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/nmr/__init__.py
--rw-r--r--   0        0        0    10952 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/nmr/basis.py
--rw-r--r--   0        0        0     6309 2023-04-19 08:05:00.033306 chemex-2022.3.3/chemex/nmr/constants.py
--rw-r--r--   0        0        0     9538 2023-04-19 08:05:00.037305 chemex-2022.3.3/chemex/nmr/liouvillian.py
--rw-r--r--   0        0        0     8795 2023-04-19 08:05:00.037305 chemex-2022.3.3/chemex/nmr/rates.py
--rw-r--r--   0        0        0    13135 2023-04-19 08:05:00.037305 chemex-2022.3.3/chemex/nmr/spectrometer.py
--rw-r--r--   0        0        0        0 2023-04-19 08:05:00.037305 chemex-2022.3.3/chemex/optimize/__init__.py
--rw-r--r--   0        0        0     5309 2023-04-19 08:05:00.037305 chemex-2022.3.3/chemex/optimize/fitting.py
--rw-r--r--   0        0        0     8679 2023-04-19 08:05:00.037305 chemex-2022.3.3/chemex/optimize/gridding.py
--rw-r--r--   0        0        0     2946 2023-04-19 08:05:00.037305 chemex-2022.3.3/chemex/optimize/grouping.py
--rw-r--r--   0        0        0     5459 2023-04-19 08:05:00.037305 chemex-2022.3.3/chemex/optimize/helper.py
--rw-r--r--   0        0        0     2763 2023-04-19 08:05:00.037305 chemex-2022.3.3/chemex/optimize/minimizer.py
--rw-r--r--   0        0        0        0 2023-04-19 08:05:00.037305 chemex-2022.3.3/chemex/parameters/__init__.py
--rw-r--r--   0        0        0    12804 2023-04-19 08:05:00.037305 chemex-2022.3.3/chemex/parameters/database.py
--rw-r--r--   0        0        0     3236 2023-04-19 08:05:00.037305 chemex-2022.3.3/chemex/parameters/factory.py
--rw-r--r--   0        0        0     4659 2023-04-19 08:05:00.037305 chemex-2022.3.3/chemex/parameters/name.py
--rw-r--r--   0        0        0     3937 2023-04-19 08:05:00.037305 chemex-2022.3.3/chemex/parameters/setting.py
--rw-r--r--   0        0        0    12612 2023-04-19 08:05:00.037305 chemex-2022.3.3/chemex/parameters/spin_system.py
--rw-r--r--   0        0        0     9618 2023-04-19 08:05:00.037305 chemex-2022.3.3/chemex/parameters/spins.py
--rw-r--r--   0        0        0      901 2023-04-19 08:05:00.037305 chemex-2022.3.3/chemex/parameters/userfunctions.py
--rw-r--r--   0        0        0      316 2023-04-19 08:05:00.037305 chemex-2022.3.3/chemex/plotters/__init__.py
--rw-r--r--   0        0        0     7907 2023-04-19 08:05:00.037305 chemex-2022.3.3/chemex/plotters/cest.py
--rw-r--r--   0        0        0     6634 2023-04-19 08:05:00.037305 chemex-2022.3.3/chemex/plotters/cpmg.py
--rw-r--r--   0        0        0     2376 2023-04-19 08:05:00.037305 chemex-2022.3.3/chemex/plotters/plot.py
--rw-r--r--   0        0        0      329 2023-04-19 08:05:00.037305 chemex-2022.3.3/chemex/plotters/plotter.py
--rw-r--r--   0        0        0     3706 2023-04-19 08:05:00.037305 chemex-2022.3.3/chemex/plotters/relaxation.py
--rw-r--r--   0        0        0     1674 2023-04-19 08:05:00.037305 chemex-2022.3.3/chemex/plotters/shift.py
--rw-r--r--   0        0        0        0 2023-04-19 08:05:00.037305 chemex-2022.3.3/chemex/printers/__init__.py
--rw-r--r--   0        0        0     1785 2023-04-19 08:05:00.037305 chemex-2022.3.3/chemex/printers/data.py
--rw-r--r--   0        0        0     4510 2023-04-19 08:05:00.037305 chemex-2022.3.3/chemex/printers/parameters.py
--rw-r--r--   0        0        0     2679 2023-04-19 08:05:00.037305 chemex-2022.3.3/chemex/printers/plot.py
--rw-r--r--   0        0        0     2929 2023-04-19 08:05:00.037305 chemex-2022.3.3/chemex/toml.py
--rw-r--r--   0        0        0       98 2023-04-19 08:05:00.037305 chemex-2022.3.3/chemex/tools/__init__.py
--rw-r--r--   0        0        0     9332 2023-04-19 08:05:00.037305 chemex-2022.3.3/chemex/tools/pick_cest.py
--rw-r--r--   0        0        0     1819 2023-04-19 08:05:00.037305 chemex-2022.3.3/chemex/tools/plot_param.py
--rw-r--r--   0        0        0     2667 2023-04-19 08:05:00.037305 chemex-2022.3.3/chemex/uncertainty.py
--rw-r--r--   0        0        0     1056 2023-04-19 08:05:00.193307 chemex-2022.3.3/pyproject.toml
--rw-r--r--   0        0        0     2135 1970-01-01 00:00:00.000000 chemex-2022.3.3/PKG-INFO
+-rw-r--r--   0        0        0    34916 2023-04-19 20:10:31.302739 chemex-2022.3.4/LICENSE.md
+-rw-r--r--   0        0        0     1046 2023-04-19 20:10:31.302739 chemex-2022.3.4/README.md
+-rw-r--r--   0        0        0      326 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/__init__.py
+-rw-r--r--   0        0        0      185 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/__main__.py
+-rw-r--r--   0        0        0     2583 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/chemex.py
+-rw-r--r--   0        0        0     5876 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/cli.py
+-rw-r--r--   0        0        0        0 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/configuration/__init__.py
+-rw-r--r--   0        0        0      447 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/configuration/base.py
+-rw-r--r--   0        0        0     4619 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/configuration/conditions.py
+-rw-r--r--   0        0        0     1491 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/configuration/data.py
+-rw-r--r--   0        0        0     1418 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/configuration/experiment.py
+-rw-r--r--   0        0        0     4588 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/configuration/methods.py
+-rw-r--r--   0        0        0     1971 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/configuration/parameters.py
+-rw-r--r--   0        0        0        0 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/containers/__init__.py
+-rw-r--r--   0        0        0     3158 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/containers/data.py
+-rw-r--r--   0        0        0     1497 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/containers/dataset.py
+-rw-r--r--   0        0        0     5406 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/containers/experiment.py
+-rw-r--r--   0        0        0     4238 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/containers/experiments.py
+-rw-r--r--   0        0        0     3840 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/containers/profile.py
+-rw-r--r--   0        0        0        0 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/__init__.py
+-rw-r--r--   0        0        0     4379 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/builder.py
+-rw-r--r--   0        0        0        0 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/__init__.py
+-rw-r--r--   0        0        0     3678 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/cest_13c.py
+-rw-r--r--   0        0        0     3588 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/cest_15n.py
+-rw-r--r--   0        0        0     4060 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/cest_15n_cw.py
+-rw-r--r--   0        0        0     4353 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/cest_15n_tr.py
+-rw-r--r--   0        0        0     3682 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/cest_1hn_ap.py
+-rw-r--r--   0        0        0     4771 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/cest_1hn_ip_ap.py
+-rw-r--r--   0        0        0     4084 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/cest_ch3_1h_ip_ap.py
+-rw-r--r--   0        0        0     5188 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/coscest_13c.py
+-rw-r--r--   0        0        0     5472 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/coscest_1hn_ip_ap.py
+-rw-r--r--   0        0        0     4782 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/cpmg_13c_ip.py
+-rw-r--r--   0        0        0     5174 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/cpmg_13co_ap.py
+-rw-r--r--   0        0        0     4864 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/cpmg_15n_ip.py
+-rw-r--r--   0        0        0     5702 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/cpmg_15n_ip_0013.py
+-rw-r--r--   0        0        0     5456 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/cpmg_15n_tr.py
+-rw-r--r--   0        0        0     7561 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/cpmg_15n_tr_0013.py
+-rw-r--r--   0        0        0     5192 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/cpmg_1hn_ap.py
+-rw-r--r--   0        0        0     7764 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/cpmg_1hn_ap_0013.py
+-rw-r--r--   0        0        0     5016 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/cpmg_ch3_13c_h2c.py
+-rw-r--r--   0        0        0     5869 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/cpmg_ch3_1h_dq.py
+-rw-r--r--   0        0        0     6696 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/cpmg_ch3_1h_sq.py
+-rw-r--r--   0        0        0     5871 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/cpmg_ch3_1h_tq.py
+-rw-r--r--   0        0        0     7400 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/cpmg_ch3_1h_tq_diff.py
+-rw-r--r--   0        0        0     4292 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/cpmg_ch3_mq.py
+-rw-r--r--   0        0        0     4916 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/experiments/catalog/cpmg_chd2_1h_ap.py
+-rw-r--r--   0        0        0     5290 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/experiments/catalog/cpmg_hn_dq_zq.py
+-rw-r--r--   0        0        0     4412 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/experiments/catalog/dcest_13c.py
+-rw-r--r--   0        0        0     4643 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/experiments/catalog/dcest_15n.py
+-rw-r--r--   0        0        0     3330 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/experiments/catalog/relaxation_hznz.py
+-rw-r--r--   0        0        0     2991 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/experiments/catalog/relaxation_nz.py
+-rw-r--r--   0        0        0     2921 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/experiments/catalog/shift_15n_sq.py
+-rw-r--r--   0        0        0     3283 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/experiments/catalog/shift_15n_sqmq.py
+-rw-r--r--   0        0        0     3235 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/experiments/factories.py
+-rw-r--r--   0        0        0      970 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/experiments/loader.py
+-rw-r--r--   0        0        0     2671 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/filterers.py
+-rw-r--r--   0        0        0     7125 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/messages.py
+-rw-r--r--   0        0        0        0 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/models/__init__.py
+-rw-r--r--   0        0        0     2753 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/models/constraints.py
+-rw-r--r--   0        0        0     1071 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/models/factory.py
+-rw-r--r--   0        0        0        0 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/models/kinetic/__init__.py
+-rw-r--r--   0        0        0      575 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/models/kinetic/settings_1st.py
+-rw-r--r--   0        0        0     1241 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/models/kinetic/settings_2st.py
+-rw-r--r--   0        0        0     2954 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/models/kinetic/settings_2st_a_a2.py
+-rw-r--r--   0        0        0     2958 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/models/kinetic/settings_2st_a_a3.py
+-rw-r--r--   0        0        0     2966 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/models/kinetic/settings_2st_a_a4.py
+-rw-r--r--   0        0        0     2722 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/models/kinetic/settings_2st_binding.py
+-rw-r--r--   0        0        0     2878 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/models/kinetic/settings_2st_eyring.py
+-rw-r--r--   0        0        0     1985 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/models/kinetic/settings_2st_hd.py
+-rw-r--r--   0        0        0     1278 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/models/kinetic/settings_2st_rs.py
+-rw-r--r--   0        0        0     4590 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/models/kinetic/settings_3st_a_a2_a3.py
+-rw-r--r--   0        0        0     4298 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/models/kinetic/settings_3st_a_a2_a4.py
+-rw-r--r--   0        0        0     5043 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/models/kinetic/settings_3st_double_binding.py
+-rw-r--r--   0        0        0     4463 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/models/kinetic/settings_3st_eyring.py
+-rw-r--r--   0        0        0     4079 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/models/kinetic/settings_3st_induced_fit.py
+-rw-r--r--   0        0        0     3994 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/models/kinetic/settings_4st_hd.py
+-rw-r--r--   0        0        0     4768 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/models/kinetic/settings_nst.py
+-rw-r--r--   0        0        0      945 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/models/loader.py
+-rw-r--r--   0        0        0     1384 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/models/model.py
+-rw-r--r--   0        0        0        0 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/nmr/__init__.py
+-rw-r--r--   0        0        0    10952 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/nmr/basis.py
+-rw-r--r--   0        0        0     6309 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/nmr/constants.py
+-rw-r--r--   0        0        0     9538 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/nmr/liouvillian.py
+-rw-r--r--   0        0        0     8795 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/nmr/rates.py
+-rw-r--r--   0        0        0    13135 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/nmr/spectrometer.py
+-rw-r--r--   0        0        0        0 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/optimize/__init__.py
+-rw-r--r--   0        0        0     5309 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/optimize/fitting.py
+-rw-r--r--   0        0        0     8679 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/optimize/gridding.py
+-rw-r--r--   0        0        0     2946 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/optimize/grouping.py
+-rw-r--r--   0        0        0     5459 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/optimize/helper.py
+-rw-r--r--   0        0        0     2763 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/optimize/minimizer.py
+-rw-r--r--   0        0        0        0 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/parameters/__init__.py
+-rw-r--r--   0        0        0    12804 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/parameters/database.py
+-rw-r--r--   0        0        0     3236 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/parameters/factory.py
+-rw-r--r--   0        0        0     4659 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/parameters/name.py
+-rw-r--r--   0        0        0     3937 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/parameters/setting.py
+-rw-r--r--   0        0        0    12623 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/parameters/spin_system.py
+-rw-r--r--   0        0        0     9618 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/parameters/spins.py
+-rw-r--r--   0        0        0      901 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/parameters/userfunctions.py
+-rw-r--r--   0        0        0      316 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/plotters/__init__.py
+-rw-r--r--   0        0        0     7907 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/plotters/cest.py
+-rw-r--r--   0        0        0     6634 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/plotters/cpmg.py
+-rw-r--r--   0        0        0     2376 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/plotters/plot.py
+-rw-r--r--   0        0        0      329 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/plotters/plotter.py
+-rw-r--r--   0        0        0     3706 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/plotters/relaxation.py
+-rw-r--r--   0        0        0     1674 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/plotters/shift.py
+-rw-r--r--   0        0        0        0 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/printers/__init__.py
+-rw-r--r--   0        0        0     1785 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/printers/data.py
+-rw-r--r--   0        0        0     4510 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/printers/parameters.py
+-rw-r--r--   0        0        0     2679 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/printers/plot.py
+-rw-r--r--   0        0        0     2929 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/toml.py
+-rw-r--r--   0        0        0       98 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/tools/__init__.py
+-rw-r--r--   0        0        0     9332 2023-04-19 20:10:31.310739 chemex-2022.3.4/chemex/tools/pick_cest.py
+-rw-r--r--   0        0        0     1819 2023-04-19 20:10:31.310739 chemex-2022.3.4/chemex/tools/plot_param.py
+-rw-r--r--   0        0        0     2667 2023-04-19 20:10:31.310739 chemex-2022.3.4/chemex/uncertainty.py
+-rw-r--r--   0        0        0     1056 2023-04-19 20:10:31.542741 chemex-2022.3.4/pyproject.toml
+-rw-r--r--   0        0        0     2135 1970-01-01 00:00:00.000000 chemex-2022.3.4/PKG-INFO
```

### Comparing `chemex-2022.3.3/LICENSE.md` & `chemex-2022.3.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/README.md` & `chemex-2022.3.4/README.md`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/chemex.py` & `chemex-2022.3.4/chemex/chemex.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/cli.py` & `chemex-2022.3.4/chemex/cli.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/configuration/conditions.py` & `chemex-2022.3.4/chemex/configuration/conditions.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/configuration/data.py` & `chemex-2022.3.4/chemex/configuration/data.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/configuration/experiment.py` & `chemex-2022.3.4/chemex/configuration/experiment.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/configuration/methods.py` & `chemex-2022.3.4/chemex/configuration/methods.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/configuration/parameters.py` & `chemex-2022.3.4/chemex/configuration/parameters.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/containers/data.py` & `chemex-2022.3.4/chemex/containers/data.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/containers/dataset.py` & `chemex-2022.3.4/chemex/containers/dataset.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/containers/experiment.py` & `chemex-2022.3.4/chemex/containers/experiment.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/containers/experiments.py` & `chemex-2022.3.4/chemex/containers/experiments.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/containers/profile.py` & `chemex-2022.3.4/chemex/containers/profile.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/experiments/builder.py` & `chemex-2022.3.4/chemex/experiments/builder.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/experiments/catalog/cest_13c.py` & `chemex-2022.3.4/chemex/experiments/catalog/cest_13c.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/experiments/catalog/cest_15n.py` & `chemex-2022.3.4/chemex/experiments/catalog/cest_15n.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/experiments/catalog/cest_15n_cw.py` & `chemex-2022.3.4/chemex/experiments/catalog/cest_15n_cw.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/experiments/catalog/cest_15n_tr.py` & `chemex-2022.3.4/chemex/experiments/catalog/cest_15n_tr.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/experiments/catalog/cest_1hn_ap.py` & `chemex-2022.3.4/chemex/experiments/catalog/cest_1hn_ap.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/experiments/catalog/cest_1hn_ip_ap.py` & `chemex-2022.3.4/chemex/experiments/catalog/cest_1hn_ip_ap.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/experiments/catalog/cest_ch3_1h_ip_ap.py` & `chemex-2022.3.4/chemex/experiments/catalog/cest_ch3_1h_ip_ap.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/experiments/catalog/coscest_13c.py` & `chemex-2022.3.4/chemex/experiments/catalog/coscest_13c.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/experiments/catalog/coscest_1hn_ip_ap.py` & `chemex-2022.3.4/chemex/experiments/catalog/coscest_1hn_ip_ap.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/experiments/catalog/cpmg_13c_ip.py` & `chemex-2022.3.4/chemex/experiments/catalog/cpmg_13c_ip.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/experiments/catalog/cpmg_13co_ap.py` & `chemex-2022.3.4/chemex/experiments/catalog/cpmg_13co_ap.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/experiments/catalog/cpmg_15n_ip.py` & `chemex-2022.3.4/chemex/experiments/catalog/cpmg_15n_ip.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/experiments/catalog/cpmg_15n_ip_0013.py` & `chemex-2022.3.4/chemex/experiments/catalog/cpmg_15n_ip_0013.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/experiments/catalog/cpmg_15n_tr.py` & `chemex-2022.3.4/chemex/experiments/catalog/cpmg_15n_tr.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/experiments/catalog/cpmg_15n_tr_0013.py` & `chemex-2022.3.4/chemex/experiments/catalog/cpmg_15n_tr_0013.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/experiments/catalog/cpmg_1hn_ap.py` & `chemex-2022.3.4/chemex/experiments/catalog/cpmg_1hn_ap.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/experiments/catalog/cpmg_1hn_ap_0013.py` & `chemex-2022.3.4/chemex/experiments/catalog/cpmg_1hn_ap_0013.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/experiments/catalog/cpmg_ch3_13c_h2c.py` & `chemex-2022.3.4/chemex/experiments/catalog/cpmg_ch3_13c_h2c.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/experiments/catalog/cpmg_ch3_1h_dq.py` & `chemex-2022.3.4/chemex/experiments/catalog/cpmg_ch3_1h_dq.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/experiments/catalog/cpmg_ch3_1h_sq.py` & `chemex-2022.3.4/chemex/experiments/catalog/cpmg_ch3_1h_sq.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/experiments/catalog/cpmg_ch3_1h_tq.py` & `chemex-2022.3.4/chemex/experiments/catalog/cpmg_ch3_1h_tq.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/experiments/catalog/cpmg_ch3_1h_tq_diff.py` & `chemex-2022.3.4/chemex/experiments/catalog/cpmg_ch3_1h_tq_diff.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/experiments/catalog/cpmg_ch3_mq.py` & `chemex-2022.3.4/chemex/experiments/catalog/cpmg_ch3_mq.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/experiments/catalog/cpmg_chd2_1h_ap.py` & `chemex-2022.3.4/chemex/experiments/catalog/cpmg_chd2_1h_ap.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/experiments/catalog/cpmg_hn_dq_zq.py` & `chemex-2022.3.4/chemex/experiments/catalog/cpmg_hn_dq_zq.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/experiments/catalog/dcest_13c.py` & `chemex-2022.3.4/chemex/experiments/catalog/dcest_13c.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/experiments/catalog/dcest_15n.py` & `chemex-2022.3.4/chemex/experiments/catalog/dcest_15n.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/experiments/catalog/relaxation_hznz.py` & `chemex-2022.3.4/chemex/experiments/catalog/relaxation_hznz.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/experiments/catalog/relaxation_nz.py` & `chemex-2022.3.4/chemex/experiments/catalog/relaxation_nz.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/experiments/catalog/shift_15n_sq.py` & `chemex-2022.3.4/chemex/experiments/catalog/shift_15n_sq.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/experiments/catalog/shift_15n_sqmq.py` & `chemex-2022.3.4/chemex/experiments/catalog/shift_15n_sqmq.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/experiments/factories.py` & `chemex-2022.3.4/chemex/experiments/factories.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/experiments/loader.py` & `chemex-2022.3.4/chemex/experiments/loader.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/filterers.py` & `chemex-2022.3.4/chemex/filterers.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/messages.py` & `chemex-2022.3.4/chemex/messages.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/models/constraints.py` & `chemex-2022.3.4/chemex/models/constraints.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/models/factory.py` & `chemex-2022.3.4/chemex/models/factory.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/models/kinetic/settings_1st.py` & `chemex-2022.3.4/chemex/models/kinetic/settings_1st.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/models/kinetic/settings_2st.py` & `chemex-2022.3.4/chemex/models/kinetic/settings_2st.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/models/kinetic/settings_2st_a_a2.py` & `chemex-2022.3.4/chemex/models/kinetic/settings_2st_a_a2.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/models/kinetic/settings_2st_a_a3.py` & `chemex-2022.3.4/chemex/models/kinetic/settings_2st_a_a3.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/models/kinetic/settings_2st_a_a4.py` & `chemex-2022.3.4/chemex/models/kinetic/settings_2st_a_a4.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/models/kinetic/settings_2st_binding.py` & `chemex-2022.3.4/chemex/models/kinetic/settings_2st_binding.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/models/kinetic/settings_2st_eyring.py` & `chemex-2022.3.4/chemex/models/kinetic/settings_2st_eyring.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/models/kinetic/settings_2st_hd.py` & `chemex-2022.3.4/chemex/models/kinetic/settings_2st_hd.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/models/kinetic/settings_2st_rs.py` & `chemex-2022.3.4/chemex/models/kinetic/settings_2st_rs.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/models/kinetic/settings_3st_a_a2_a3.py` & `chemex-2022.3.4/chemex/models/kinetic/settings_3st_a_a2_a3.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/models/kinetic/settings_3st_a_a2_a4.py` & `chemex-2022.3.4/chemex/models/kinetic/settings_3st_a_a2_a4.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/models/kinetic/settings_3st_double_binding.py` & `chemex-2022.3.4/chemex/models/kinetic/settings_3st_double_binding.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/models/kinetic/settings_3st_eyring.py` & `chemex-2022.3.4/chemex/models/kinetic/settings_3st_eyring.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/models/kinetic/settings_3st_induced_fit.py` & `chemex-2022.3.4/chemex/models/kinetic/settings_3st_induced_fit.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/models/kinetic/settings_4st_hd.py` & `chemex-2022.3.4/chemex/models/kinetic/settings_4st_hd.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/models/kinetic/settings_nst.py` & `chemex-2022.3.4/chemex/models/kinetic/settings_nst.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/models/loader.py` & `chemex-2022.3.4/chemex/models/loader.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/models/model.py` & `chemex-2022.3.4/chemex/models/model.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/nmr/basis.py` & `chemex-2022.3.4/chemex/nmr/basis.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/nmr/constants.py` & `chemex-2022.3.4/chemex/nmr/constants.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/nmr/liouvillian.py` & `chemex-2022.3.4/chemex/nmr/liouvillian.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/nmr/rates.py` & `chemex-2022.3.4/chemex/nmr/rates.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/nmr/spectrometer.py` & `chemex-2022.3.4/chemex/nmr/spectrometer.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/optimize/fitting.py` & `chemex-2022.3.4/chemex/optimize/fitting.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/optimize/gridding.py` & `chemex-2022.3.4/chemex/optimize/gridding.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/optimize/grouping.py` & `chemex-2022.3.4/chemex/optimize/grouping.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/optimize/helper.py` & `chemex-2022.3.4/chemex/optimize/helper.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/optimize/minimizer.py` & `chemex-2022.3.4/chemex/optimize/minimizer.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/parameters/database.py` & `chemex-2022.3.4/chemex/parameters/database.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/parameters/factory.py` & `chemex-2022.3.4/chemex/parameters/factory.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/parameters/name.py` & `chemex-2022.3.4/chemex/parameters/name.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/parameters/setting.py` & `chemex-2022.3.4/chemex/parameters/setting.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/parameters/spin_system.py` & `chemex-2022.3.4/chemex/parameters/spin_system.py`

 * *Files 1% similar despite different names*

```diff
@@ -299,15 +299,15 @@
             return selection.lower() in ("all", "*")
         return any(item.match(self) for item in selection)
 
     def correct(self, basis: Basis) -> SpinSystem:
         spins = []
         last_spin = Spin("")
         for letter, atom in basis.atoms.items():
-            spin = self.spins.get(letter, last_spin)
+            spin = Spin(self.spins.get(letter, last_spin).name)
             if not spin.atom.name.startswith(atom.upper()):
                 spin.atom = Atom(f"{atom}{spin.atom.name[1:]}")
             last_spin = spin
             spins.append(spin)
         return SpinSystem(self._spins2name(spins))
 
     def build_sub_spin_system(
```

### Comparing `chemex-2022.3.3/chemex/parameters/spins.py` & `chemex-2022.3.4/chemex/parameters/spins.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/parameters/userfunctions.py` & `chemex-2022.3.4/chemex/parameters/userfunctions.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/plotters/cest.py` & `chemex-2022.3.4/chemex/plotters/cest.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/plotters/cpmg.py` & `chemex-2022.3.4/chemex/plotters/cpmg.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/plotters/plot.py` & `chemex-2022.3.4/chemex/plotters/plot.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/plotters/relaxation.py` & `chemex-2022.3.4/chemex/plotters/relaxation.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/plotters/shift.py` & `chemex-2022.3.4/chemex/plotters/shift.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/printers/data.py` & `chemex-2022.3.4/chemex/printers/data.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/printers/parameters.py` & `chemex-2022.3.4/chemex/printers/parameters.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/printers/plot.py` & `chemex-2022.3.4/chemex/printers/plot.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/toml.py` & `chemex-2022.3.4/chemex/toml.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/tools/pick_cest.py` & `chemex-2022.3.4/chemex/tools/pick_cest.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/tools/plot_param.py` & `chemex-2022.3.4/chemex/tools/plot_param.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/chemex/uncertainty.py` & `chemex-2022.3.4/chemex/uncertainty.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.3/pyproject.toml` & `chemex-2022.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chemex"
-version = "2022.3.3"
+version = "2022.3.4"
 description = "ChemEx is an analysis program for chemical exchange detected by NMR"
 authors = ["Guillaume Bouvignies <gbouvignies@gmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/gbouvignies/chemex"
 homepage = "http://gbouvignies.github.io/ChemEx/"
 classifiers = [
```

### Comparing `chemex-2022.3.3/PKG-INFO` & `chemex-2022.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chemex
-Version: 2022.3.3
+Version: 2022.3.4
 Summary: ChemEx is an analysis program for chemical exchange detected by NMR
 Home-page: http://gbouvignies.github.io/ChemEx/
 License: GPL-3.0-only
 Author: Guillaume Bouvignies
 Author-email: gbouvignies@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Intended Audience :: Science/Research
```


# Comparing `tmp/chemex-2022.3.1.tar.gz` & `tmp/chemex-2022.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chemex-2022.3.1.tar", max compression
+gzip compressed data, was "chemex-2022.3.2.tar", max compression
```

## Comparing `chemex-2022.3.1.tar` & `chemex-2022.3.2.tar`

### file list

```diff
@@ -1,117 +1,117 @@
--rw-r--r--   0        0        0    34916 2023-04-14 11:37:01.941999 chemex-2022.3.1/LICENSE.md
--rw-r--r--   0        0        0     1046 2023-04-14 11:37:01.941999 chemex-2022.3.1/README.md
--rw-r--r--   0        0        0      326 2023-04-14 11:37:01.941999 chemex-2022.3.1/chemex/__init__.py
--rw-r--r--   0        0        0      185 2023-04-14 11:37:01.941999 chemex-2022.3.1/chemex/__main__.py
--rw-r--r--   0        0        0     2583 2023-04-14 11:37:01.941999 chemex-2022.3.1/chemex/chemex.py
--rw-r--r--   0        0        0     5876 2023-04-14 11:37:01.941999 chemex-2022.3.1/chemex/cli.py
--rw-r--r--   0        0        0        0 2023-04-14 11:37:01.941999 chemex-2022.3.1/chemex/configuration/__init__.py
--rw-r--r--   0        0        0      447 2023-04-14 11:37:01.941999 chemex-2022.3.1/chemex/configuration/base.py
--rw-r--r--   0        0        0     4619 2023-04-14 11:37:01.941999 chemex-2022.3.1/chemex/configuration/conditions.py
--rw-r--r--   0        0        0     1491 2023-04-14 11:37:01.941999 chemex-2022.3.1/chemex/configuration/data.py
--rw-r--r--   0        0        0     1418 2023-04-14 11:37:01.941999 chemex-2022.3.1/chemex/configuration/experiment.py
--rw-r--r--   0        0        0     4588 2023-04-14 11:37:01.941999 chemex-2022.3.1/chemex/configuration/methods.py
--rw-r--r--   0        0        0     1971 2023-04-14 11:37:01.941999 chemex-2022.3.1/chemex/configuration/parameters.py
--rw-r--r--   0        0        0        0 2023-04-14 11:37:01.941999 chemex-2022.3.1/chemex/containers/__init__.py
--rw-r--r--   0        0        0     3158 2023-04-14 11:37:01.941999 chemex-2022.3.1/chemex/containers/data.py
--rw-r--r--   0        0        0     1497 2023-04-14 11:37:01.941999 chemex-2022.3.1/chemex/containers/dataset.py
--rw-r--r--   0        0        0     5406 2023-04-14 11:37:01.941999 chemex-2022.3.1/chemex/containers/experiment.py
--rw-r--r--   0        0        0     4238 2023-04-14 11:37:01.941999 chemex-2022.3.1/chemex/containers/experiments.py
--rw-r--r--   0        0        0     3840 2023-04-14 11:37:01.941999 chemex-2022.3.1/chemex/containers/profile.py
--rw-r--r--   0        0        0        0 2023-04-14 11:37:01.941999 chemex-2022.3.1/chemex/experiments/__init__.py
--rw-r--r--   0        0        0     4379 2023-04-14 11:37:01.941999 chemex-2022.3.1/chemex/experiments/builder.py
--rw-r--r--   0        0        0        0 2023-04-14 11:37:01.941999 chemex-2022.3.1/chemex/experiments/catalog/__init__.py
--rw-r--r--   0        0        0     3678 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/cest_13c.py
--rw-r--r--   0        0        0     3588 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/cest_15n.py
--rw-r--r--   0        0        0     4060 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/cest_15n_cw.py
--rw-r--r--   0        0        0     4353 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/cest_15n_tr.py
--rw-r--r--   0        0        0     3682 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/cest_1hn_ap.py
--rw-r--r--   0        0        0     4771 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/cest_1hn_ip_ap.py
--rw-r--r--   0        0        0     4084 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/cest_ch3_1h_ip_ap.py
--rw-r--r--   0        0        0     5188 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/coscest_13c.py
--rw-r--r--   0        0        0     5472 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/coscest_1hn_ip_ap.py
--rw-r--r--   0        0        0     4782 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/cpmg_13c_ip.py
--rw-r--r--   0        0        0     5174 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/cpmg_13co_ap.py
--rw-r--r--   0        0        0     4864 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/cpmg_15n_ip.py
--rw-r--r--   0        0        0     5702 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/cpmg_15n_ip_0013.py
--rw-r--r--   0        0        0     5456 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/cpmg_15n_tr.py
--rw-r--r--   0        0        0     7561 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/cpmg_15n_tr_0013.py
--rw-r--r--   0        0        0     4965 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/cpmg_1hn_ap.py
--rw-r--r--   0        0        0     7340 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/cpmg_1hn_ap_0013.py
--rw-r--r--   0        0        0     5016 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/cpmg_ch3_13c_h2c.py
--rw-r--r--   0        0        0     5869 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/cpmg_ch3_1h_dq.py
--rw-r--r--   0        0        0     6696 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/cpmg_ch3_1h_sq.py
--rw-r--r--   0        0        0     5871 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/cpmg_ch3_1h_tq.py
--rw-r--r--   0        0        0     7400 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/cpmg_ch3_1h_tq_diff.py
--rw-r--r--   0        0        0     4292 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/cpmg_ch3_mq.py
--rw-r--r--   0        0        0     4916 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/cpmg_chd2_1h_ap.py
--rw-r--r--   0        0        0     5290 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/cpmg_hn_dq_zq.py
--rw-r--r--   0        0        0     4412 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/dcest_13c.py
--rw-r--r--   0        0        0     4643 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/dcest_15n.py
--rw-r--r--   0        0        0     3330 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/relaxation_hznz.py
--rw-r--r--   0        0        0     2991 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/relaxation_nz.py
--rw-r--r--   0        0        0     2921 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/shift_15n_sq.py
--rw-r--r--   0        0        0     3283 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/shift_15n_sqmq.py
--rw-r--r--   0        0        0     3235 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/factories.py
--rw-r--r--   0        0        0      970 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/loader.py
--rw-r--r--   0        0        0     2671 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/filterers.py
--rw-r--r--   0        0        0     7125 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/messages.py
--rw-r--r--   0        0        0        0 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/models/__init__.py
--rw-r--r--   0        0        0     2753 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/models/constraints.py
--rw-r--r--   0        0        0     1071 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/models/factory.py
--rw-r--r--   0        0        0        0 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/models/kinetic/__init__.py
--rw-r--r--   0        0        0      575 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/models/kinetic/settings_1st.py
--rw-r--r--   0        0        0     1241 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/models/kinetic/settings_2st.py
--rw-r--r--   0        0        0     2954 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/models/kinetic/settings_2st_a_a2.py
--rw-r--r--   0        0        0     2958 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/models/kinetic/settings_2st_a_a3.py
--rw-r--r--   0        0        0     2966 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/models/kinetic/settings_2st_a_a4.py
--rw-r--r--   0        0        0     2722 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/models/kinetic/settings_2st_binding.py
--rw-r--r--   0        0        0     2878 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/models/kinetic/settings_2st_eyring.py
--rw-r--r--   0        0        0     1985 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/models/kinetic/settings_2st_hd.py
--rw-r--r--   0        0        0     1278 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/models/kinetic/settings_2st_rs.py
--rw-r--r--   0        0        0     4590 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/models/kinetic/settings_3st_a_a2_a3.py
--rw-r--r--   0        0        0     4298 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/models/kinetic/settings_3st_a_a2_a4.py
--rw-r--r--   0        0        0     5043 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/models/kinetic/settings_3st_double_binding.py
--rw-r--r--   0        0        0     4463 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/models/kinetic/settings_3st_eyring.py
--rw-r--r--   0        0        0     4079 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/models/kinetic/settings_3st_induced_fit.py
--rw-r--r--   0        0        0     3994 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/models/kinetic/settings_4st_hd.py
--rw-r--r--   0        0        0     4768 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/models/kinetic/settings_nst.py
--rw-r--r--   0        0        0      945 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/models/loader.py
--rw-r--r--   0        0        0     1396 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/models/model.py
--rw-r--r--   0        0        0        0 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/nmr/__init__.py
--rw-r--r--   0        0        0    10952 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/nmr/basis.py
--rw-r--r--   0        0        0     6309 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/nmr/constants.py
--rw-r--r--   0        0        0     9538 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/nmr/liouvillian.py
--rw-r--r--   0        0        0     8795 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/nmr/rates.py
--rw-r--r--   0        0        0    13135 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/nmr/spectrometer.py
--rw-r--r--   0        0        0        0 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/optimize/__init__.py
--rw-r--r--   0        0        0     5309 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/optimize/fitting.py
--rw-r--r--   0        0        0     8679 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/optimize/gridding.py
--rw-r--r--   0        0        0     2946 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/optimize/grouping.py
--rw-r--r--   0        0        0     5459 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/optimize/helper.py
--rw-r--r--   0        0        0     2763 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/optimize/minimizer.py
--rw-r--r--   0        0        0        0 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/parameters/__init__.py
--rw-r--r--   0        0        0    12772 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/parameters/database.py
--rw-r--r--   0        0        0     3236 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/parameters/factory.py
--rw-r--r--   0        0        0     4659 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/parameters/name.py
--rw-r--r--   0        0        0     3937 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/parameters/setting.py
--rw-r--r--   0        0        0    12664 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/parameters/spin_system.py
--rw-r--r--   0        0        0     9618 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/parameters/spins.py
--rw-r--r--   0        0        0      901 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/parameters/userfunctions.py
--rw-r--r--   0        0        0      316 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/plotters/__init__.py
--rw-r--r--   0        0        0     7907 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/plotters/cest.py
--rw-r--r--   0        0        0     6634 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/plotters/cpmg.py
--rw-r--r--   0        0        0     2376 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/plotters/plot.py
--rw-r--r--   0        0        0      329 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/plotters/plotter.py
--rw-r--r--   0        0        0     3706 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/plotters/relaxation.py
--rw-r--r--   0        0        0     1674 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/plotters/shift.py
--rw-r--r--   0        0        0        0 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/printers/__init__.py
--rw-r--r--   0        0        0     1785 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/printers/data.py
--rw-r--r--   0        0        0     4510 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/printers/parameters.py
--rw-r--r--   0        0        0     2679 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/printers/plot.py
--rw-r--r--   0        0        0     2929 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/toml.py
--rw-r--r--   0        0        0       98 2023-04-14 11:37:01.949999 chemex-2022.3.1/chemex/tools/__init__.py
--rw-r--r--   0        0        0     9332 2023-04-14 11:37:01.949999 chemex-2022.3.1/chemex/tools/pick_cest.py
--rw-r--r--   0        0        0     1819 2023-04-14 11:37:01.949999 chemex-2022.3.1/chemex/tools/plot_param.py
--rw-r--r--   0        0        0     2667 2023-04-14 11:37:01.949999 chemex-2022.3.1/chemex/uncertainty.py
--rw-r--r--   0        0        0     1057 2023-04-14 11:37:02.122002 chemex-2022.3.1/pyproject.toml
--rw-r--r--   0        0        0     2085 1970-01-01 00:00:00.000000 chemex-2022.3.1/PKG-INFO
+-rw-r--r--   0        0        0    34916 2023-04-18 22:38:41.117631 chemex-2022.3.2/LICENSE.md
+-rw-r--r--   0        0        0     1046 2023-04-18 22:38:41.117631 chemex-2022.3.2/README.md
+-rw-r--r--   0        0        0      326 2023-04-18 22:38:41.117631 chemex-2022.3.2/chemex/__init__.py
+-rw-r--r--   0        0        0      185 2023-04-18 22:38:41.117631 chemex-2022.3.2/chemex/__main__.py
+-rw-r--r--   0        0        0     2583 2023-04-18 22:38:41.117631 chemex-2022.3.2/chemex/chemex.py
+-rw-r--r--   0        0        0     5876 2023-04-18 22:38:41.117631 chemex-2022.3.2/chemex/cli.py
+-rw-r--r--   0        0        0        0 2023-04-18 22:38:41.117631 chemex-2022.3.2/chemex/configuration/__init__.py
+-rw-r--r--   0        0        0      447 2023-04-18 22:38:41.117631 chemex-2022.3.2/chemex/configuration/base.py
+-rw-r--r--   0        0        0     4619 2023-04-18 22:38:41.117631 chemex-2022.3.2/chemex/configuration/conditions.py
+-rw-r--r--   0        0        0     1491 2023-04-18 22:38:41.117631 chemex-2022.3.2/chemex/configuration/data.py
+-rw-r--r--   0        0        0     1418 2023-04-18 22:38:41.117631 chemex-2022.3.2/chemex/configuration/experiment.py
+-rw-r--r--   0        0        0     4588 2023-04-18 22:38:41.117631 chemex-2022.3.2/chemex/configuration/methods.py
+-rw-r--r--   0        0        0     1971 2023-04-18 22:38:41.117631 chemex-2022.3.2/chemex/configuration/parameters.py
+-rw-r--r--   0        0        0        0 2023-04-18 22:38:41.117631 chemex-2022.3.2/chemex/containers/__init__.py
+-rw-r--r--   0        0        0     3158 2023-04-18 22:38:41.117631 chemex-2022.3.2/chemex/containers/data.py
+-rw-r--r--   0        0        0     1497 2023-04-18 22:38:41.117631 chemex-2022.3.2/chemex/containers/dataset.py
+-rw-r--r--   0        0        0     5406 2023-04-18 22:38:41.117631 chemex-2022.3.2/chemex/containers/experiment.py
+-rw-r--r--   0        0        0     4238 2023-04-18 22:38:41.117631 chemex-2022.3.2/chemex/containers/experiments.py
+-rw-r--r--   0        0        0     3840 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/containers/profile.py
+-rw-r--r--   0        0        0        0 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/experiments/__init__.py
+-rw-r--r--   0        0        0     4379 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/experiments/builder.py
+-rw-r--r--   0        0        0        0 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/experiments/catalog/__init__.py
+-rw-r--r--   0        0        0     3678 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/experiments/catalog/cest_13c.py
+-rw-r--r--   0        0        0     3588 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/experiments/catalog/cest_15n.py
+-rw-r--r--   0        0        0     4060 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/experiments/catalog/cest_15n_cw.py
+-rw-r--r--   0        0        0     4353 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/experiments/catalog/cest_15n_tr.py
+-rw-r--r--   0        0        0     3682 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/experiments/catalog/cest_1hn_ap.py
+-rw-r--r--   0        0        0     4771 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/experiments/catalog/cest_1hn_ip_ap.py
+-rw-r--r--   0        0        0     4084 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/experiments/catalog/cest_ch3_1h_ip_ap.py
+-rw-r--r--   0        0        0     5188 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/experiments/catalog/coscest_13c.py
+-rw-r--r--   0        0        0     5472 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/experiments/catalog/coscest_1hn_ip_ap.py
+-rw-r--r--   0        0        0     4782 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/experiments/catalog/cpmg_13c_ip.py
+-rw-r--r--   0        0        0     5174 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/experiments/catalog/cpmg_13co_ap.py
+-rw-r--r--   0        0        0     4864 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/experiments/catalog/cpmg_15n_ip.py
+-rw-r--r--   0        0        0     5702 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/experiments/catalog/cpmg_15n_ip_0013.py
+-rw-r--r--   0        0        0     5456 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/experiments/catalog/cpmg_15n_tr.py
+-rw-r--r--   0        0        0     7561 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/experiments/catalog/cpmg_15n_tr_0013.py
+-rw-r--r--   0        0        0     5192 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/experiments/catalog/cpmg_1hn_ap.py
+-rw-r--r--   0        0        0     7764 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/experiments/catalog/cpmg_1hn_ap_0013.py
+-rw-r--r--   0        0        0     5016 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/experiments/catalog/cpmg_ch3_13c_h2c.py
+-rw-r--r--   0        0        0     5869 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/experiments/catalog/cpmg_ch3_1h_dq.py
+-rw-r--r--   0        0        0     6696 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/experiments/catalog/cpmg_ch3_1h_sq.py
+-rw-r--r--   0        0        0     5871 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/experiments/catalog/cpmg_ch3_1h_tq.py
+-rw-r--r--   0        0        0     7400 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/experiments/catalog/cpmg_ch3_1h_tq_diff.py
+-rw-r--r--   0        0        0     4292 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/experiments/catalog/cpmg_ch3_mq.py
+-rw-r--r--   0        0        0     4916 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/experiments/catalog/cpmg_chd2_1h_ap.py
+-rw-r--r--   0        0        0     5290 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/experiments/catalog/cpmg_hn_dq_zq.py
+-rw-r--r--   0        0        0     4412 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/experiments/catalog/dcest_13c.py
+-rw-r--r--   0        0        0     4643 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/experiments/catalog/dcest_15n.py
+-rw-r--r--   0        0        0     3330 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/experiments/catalog/relaxation_hznz.py
+-rw-r--r--   0        0        0     2991 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/experiments/catalog/relaxation_nz.py
+-rw-r--r--   0        0        0     2921 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/experiments/catalog/shift_15n_sq.py
+-rw-r--r--   0        0        0     3283 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/experiments/catalog/shift_15n_sqmq.py
+-rw-r--r--   0        0        0     3235 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/experiments/factories.py
+-rw-r--r--   0        0        0      970 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/experiments/loader.py
+-rw-r--r--   0        0        0     2671 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/filterers.py
+-rw-r--r--   0        0        0     7125 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/messages.py
+-rw-r--r--   0        0        0        0 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/models/__init__.py
+-rw-r--r--   0        0        0     2753 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/models/constraints.py
+-rw-r--r--   0        0        0     1071 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/models/factory.py
+-rw-r--r--   0        0        0        0 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/models/kinetic/__init__.py
+-rw-r--r--   0        0        0      575 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/models/kinetic/settings_1st.py
+-rw-r--r--   0        0        0     1241 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/models/kinetic/settings_2st.py
+-rw-r--r--   0        0        0     2954 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/models/kinetic/settings_2st_a_a2.py
+-rw-r--r--   0        0        0     2958 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/models/kinetic/settings_2st_a_a3.py
+-rw-r--r--   0        0        0     2966 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/models/kinetic/settings_2st_a_a4.py
+-rw-r--r--   0        0        0     2722 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/models/kinetic/settings_2st_binding.py
+-rw-r--r--   0        0        0     2878 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/models/kinetic/settings_2st_eyring.py
+-rw-r--r--   0        0        0     1985 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/models/kinetic/settings_2st_hd.py
+-rw-r--r--   0        0        0     1278 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/models/kinetic/settings_2st_rs.py
+-rw-r--r--   0        0        0     4590 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/models/kinetic/settings_3st_a_a2_a3.py
+-rw-r--r--   0        0        0     4298 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/models/kinetic/settings_3st_a_a2_a4.py
+-rw-r--r--   0        0        0     5043 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/models/kinetic/settings_3st_double_binding.py
+-rw-r--r--   0        0        0     4463 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/models/kinetic/settings_3st_eyring.py
+-rw-r--r--   0        0        0     4079 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/models/kinetic/settings_3st_induced_fit.py
+-rw-r--r--   0        0        0     3994 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/models/kinetic/settings_4st_hd.py
+-rw-r--r--   0        0        0     4768 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/models/kinetic/settings_nst.py
+-rw-r--r--   0        0        0      945 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/models/loader.py
+-rw-r--r--   0        0        0     1384 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/models/model.py
+-rw-r--r--   0        0        0        0 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/nmr/__init__.py
+-rw-r--r--   0        0        0    10952 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/nmr/basis.py
+-rw-r--r--   0        0        0     6309 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/nmr/constants.py
+-rw-r--r--   0        0        0     9538 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/nmr/liouvillian.py
+-rw-r--r--   0        0        0     8795 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/nmr/rates.py
+-rw-r--r--   0        0        0    13135 2023-04-18 22:38:41.121631 chemex-2022.3.2/chemex/nmr/spectrometer.py
+-rw-r--r--   0        0        0        0 2023-04-18 22:38:41.125631 chemex-2022.3.2/chemex/optimize/__init__.py
+-rw-r--r--   0        0        0     5309 2023-04-18 22:38:41.125631 chemex-2022.3.2/chemex/optimize/fitting.py
+-rw-r--r--   0        0        0     8679 2023-04-18 22:38:41.125631 chemex-2022.3.2/chemex/optimize/gridding.py
+-rw-r--r--   0        0        0     2946 2023-04-18 22:38:41.125631 chemex-2022.3.2/chemex/optimize/grouping.py
+-rw-r--r--   0        0        0     5459 2023-04-18 22:38:41.125631 chemex-2022.3.2/chemex/optimize/helper.py
+-rw-r--r--   0        0        0     2763 2023-04-18 22:38:41.125631 chemex-2022.3.2/chemex/optimize/minimizer.py
+-rw-r--r--   0        0        0        0 2023-04-18 22:38:41.125631 chemex-2022.3.2/chemex/parameters/__init__.py
+-rw-r--r--   0        0        0    12804 2023-04-18 22:38:41.125631 chemex-2022.3.2/chemex/parameters/database.py
+-rw-r--r--   0        0        0     3236 2023-04-18 22:38:41.125631 chemex-2022.3.2/chemex/parameters/factory.py
+-rw-r--r--   0        0        0     4659 2023-04-18 22:38:41.125631 chemex-2022.3.2/chemex/parameters/name.py
+-rw-r--r--   0        0        0     3937 2023-04-18 22:38:41.125631 chemex-2022.3.2/chemex/parameters/setting.py
+-rw-r--r--   0        0        0    12612 2023-04-18 22:38:41.125631 chemex-2022.3.2/chemex/parameters/spin_system.py
+-rw-r--r--   0        0        0     9618 2023-04-18 22:38:41.125631 chemex-2022.3.2/chemex/parameters/spins.py
+-rw-r--r--   0        0        0      901 2023-04-18 22:38:41.125631 chemex-2022.3.2/chemex/parameters/userfunctions.py
+-rw-r--r--   0        0        0      316 2023-04-18 22:38:41.125631 chemex-2022.3.2/chemex/plotters/__init__.py
+-rw-r--r--   0        0        0     7907 2023-04-18 22:38:41.125631 chemex-2022.3.2/chemex/plotters/cest.py
+-rw-r--r--   0        0        0     6634 2023-04-18 22:38:41.125631 chemex-2022.3.2/chemex/plotters/cpmg.py
+-rw-r--r--   0        0        0     2376 2023-04-18 22:38:41.125631 chemex-2022.3.2/chemex/plotters/plot.py
+-rw-r--r--   0        0        0      329 2023-04-18 22:38:41.125631 chemex-2022.3.2/chemex/plotters/plotter.py
+-rw-r--r--   0        0        0     3706 2023-04-18 22:38:41.125631 chemex-2022.3.2/chemex/plotters/relaxation.py
+-rw-r--r--   0        0        0     1674 2023-04-18 22:38:41.125631 chemex-2022.3.2/chemex/plotters/shift.py
+-rw-r--r--   0        0        0        0 2023-04-18 22:38:41.125631 chemex-2022.3.2/chemex/printers/__init__.py
+-rw-r--r--   0        0        0     1785 2023-04-18 22:38:41.125631 chemex-2022.3.2/chemex/printers/data.py
+-rw-r--r--   0        0        0     4510 2023-04-18 22:38:41.125631 chemex-2022.3.2/chemex/printers/parameters.py
+-rw-r--r--   0        0        0     2679 2023-04-18 22:38:41.125631 chemex-2022.3.2/chemex/printers/plot.py
+-rw-r--r--   0        0        0     2929 2023-04-18 22:38:41.125631 chemex-2022.3.2/chemex/toml.py
+-rw-r--r--   0        0        0       98 2023-04-18 22:38:41.125631 chemex-2022.3.2/chemex/tools/__init__.py
+-rw-r--r--   0        0        0     9332 2023-04-18 22:38:41.125631 chemex-2022.3.2/chemex/tools/pick_cest.py
+-rw-r--r--   0        0        0     1819 2023-04-18 22:38:41.125631 chemex-2022.3.2/chemex/tools/plot_param.py
+-rw-r--r--   0        0        0     2667 2023-04-18 22:38:41.125631 chemex-2022.3.2/chemex/uncertainty.py
+-rw-r--r--   0        0        0     1057 2023-04-18 22:38:41.321632 chemex-2022.3.2/pyproject.toml
+-rw-r--r--   0        0        0     2085 1970-01-01 00:00:00.000000 chemex-2022.3.2/PKG-INFO
```

### Comparing `chemex-2022.3.1/LICENSE.md` & `chemex-2022.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/README.md` & `chemex-2022.3.2/README.md`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/chemex.py` & `chemex-2022.3.2/chemex/chemex.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/cli.py` & `chemex-2022.3.2/chemex/cli.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/configuration/conditions.py` & `chemex-2022.3.2/chemex/configuration/conditions.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/configuration/data.py` & `chemex-2022.3.2/chemex/configuration/data.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/configuration/experiment.py` & `chemex-2022.3.2/chemex/configuration/experiment.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/configuration/methods.py` & `chemex-2022.3.2/chemex/configuration/methods.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/configuration/parameters.py` & `chemex-2022.3.2/chemex/configuration/parameters.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/containers/data.py` & `chemex-2022.3.2/chemex/containers/data.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/containers/dataset.py` & `chemex-2022.3.2/chemex/containers/dataset.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/containers/experiment.py` & `chemex-2022.3.2/chemex/containers/experiment.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/containers/experiments.py` & `chemex-2022.3.2/chemex/containers/experiments.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/containers/profile.py` & `chemex-2022.3.2/chemex/containers/profile.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/experiments/builder.py` & `chemex-2022.3.2/chemex/experiments/builder.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/experiments/catalog/cest_13c.py` & `chemex-2022.3.2/chemex/experiments/catalog/cest_13c.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/experiments/catalog/cest_15n.py` & `chemex-2022.3.2/chemex/experiments/catalog/cest_15n.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/experiments/catalog/cest_15n_cw.py` & `chemex-2022.3.2/chemex/experiments/catalog/cest_15n_cw.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/experiments/catalog/cest_15n_tr.py` & `chemex-2022.3.2/chemex/experiments/catalog/cest_15n_tr.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/experiments/catalog/cest_1hn_ap.py` & `chemex-2022.3.2/chemex/experiments/catalog/cest_1hn_ap.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/experiments/catalog/cest_1hn_ip_ap.py` & `chemex-2022.3.2/chemex/experiments/catalog/cest_1hn_ip_ap.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/experiments/catalog/cest_ch3_1h_ip_ap.py` & `chemex-2022.3.2/chemex/experiments/catalog/cest_ch3_1h_ip_ap.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/experiments/catalog/coscest_13c.py` & `chemex-2022.3.2/chemex/experiments/catalog/coscest_13c.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/experiments/catalog/coscest_1hn_ip_ap.py` & `chemex-2022.3.2/chemex/experiments/catalog/coscest_1hn_ip_ap.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/experiments/catalog/cpmg_13c_ip.py` & `chemex-2022.3.2/chemex/experiments/catalog/cpmg_13c_ip.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/experiments/catalog/cpmg_13co_ap.py` & `chemex-2022.3.2/chemex/experiments/catalog/cpmg_13co_ap.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/experiments/catalog/cpmg_15n_ip.py` & `chemex-2022.3.2/chemex/experiments/catalog/cpmg_15n_ip.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/experiments/catalog/cpmg_15n_ip_0013.py` & `chemex-2022.3.2/chemex/experiments/catalog/cpmg_15n_ip_0013.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/experiments/catalog/cpmg_15n_tr.py` & `chemex-2022.3.2/chemex/experiments/catalog/cpmg_15n_tr.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/experiments/catalog/cpmg_15n_tr_0013.py` & `chemex-2022.3.2/chemex/experiments/catalog/cpmg_15n_tr_0013.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/experiments/catalog/cpmg_1hn_ap.py` & `chemex-2022.3.2/chemex/experiments/catalog/cpmg_1hn_ap.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,16 @@
 
 
 class Cpmg1HnApSettings(CpmgSettings):
     name: Literal["cpmg_1hn_ap"]
     time_t2: float
     carrier: float
     pw90: float
-    time_equil: float = 0.0
+    time_equil_1: float = 0.0
+    time_equil_2: float = 0.0
     observed_state: Literal["a", "b", "c", "d"] = "a"
 
     @property
     def t_neg(self) -> float:
         return -2.0 * self.pw90 / np.pi
 
     @property
@@ -58,15 +59,14 @@
         state = self.experiment.observed_state
         return ToBeFitted(rates=[f"r2_i_{state}"], model_free=[f"tauc_{state}"])
 
 
 def build_spectrometer(
     config: Cpmg1HnApConfig, spin_system: SpinSystem
 ) -> Spectrometer:
-
     settings = config.experiment
     conditions = config.conditions
 
     basis = Basis(type="ixyzsz", spin_system="hn")
     liouvillian = LiouvillianIS(spin_system, basis, conditions)
     spectrometer = Spectrometer(liouvillian)
 
@@ -86,41 +86,48 @@
         tau_cps = {
             ncyc: self.settings.time_t2 / (4.0 * ncyc) - self.settings.pw90
             for ncyc in ncycs_no_ref
         }
         # An ncyc of -1 corresponds to the experiment without the CPMG
         # refocusisng pulses
         tau_cps[-1.0] = 0.5 * self.settings.time_t2
-        delays = [self.settings.t_neg, self.settings.time_equil, *tau_cps.values()]
+        delays = [
+            self.settings.t_neg,
+            self.settings.time_equil_1,
+            self.settings.time_equil_2,
+            *tau_cps.values(),
+        ]
         return tau_cps, delays
 
     def calculate(self, spectrometer: Spectrometer, data: Data) -> np.ndarray:
-
         ncycs = data.metadata
 
         # Calculation of the spectrometers corresponding to all the delays
         tau_cps, all_delays = self._get_delays(ncycs)
         delays = dict(zip(all_delays, spectrometer.delays(all_delays)))
         d_neg = delays[self.settings.t_neg]
-        d_eq = delays[self.settings.time_equil]
+        d_eq_1 = delays[self.settings.time_equil_1]
+        d_eq_2 = delays[self.settings.time_equil_2]
         d_cp = {ncyc: delays[delay] for ncyc, delay in tau_cps.items()}
 
         # Calculation of the spectrometers corresponding to all the pulses
         p90 = spectrometer.p90_i
         p180 = spectrometer.p180_i
         p180pmx = 0.5 * (p180[0] + p180[2])  # +/- phase cycling
 
         # Getting the starting magnetization
         start = spectrometer.get_start_magnetization(terms=self.settings.start)
 
         # Calculating the instensities as a function of ncyc
-        part1 = d_neg @ p90[0] @ start
-        part2 = d_eq @ p90[0] @ d_neg
+        part1 = d_neg @ p90[0] @ d_eq_1 @ start
+        part2 = d_eq_2 @ p90[0] @ d_neg
         intensities = {
-            0.0: spectrometer.detect(d_eq @ p90[0] @ p180pmx @ p90[0] @ start),
+            0.0: spectrometer.detect(
+                d_eq_2 @ p90[0] @ p180pmx @ p90[0] @ d_eq_1 @ start
+            ),
             -1.0: spectrometer.detect(part2 @ d_cp[-1] @ p180pmx @ d_cp[-1] @ part1),
         }
         for ncyc in set(ncycs) - {0.0, -1.0}:
             echo = d_cp[ncyc] @ p180[1] @ d_cp[ncyc]
             cpmg = matrix_power(echo, int(ncyc))
             intensities[ncyc] = spectrometer.detect(
                 part2 @ cpmg @ p180pmx @ cpmg @ part1
```

### Comparing `chemex-2022.3.1/chemex/experiments/catalog/cpmg_1hn_ap_0013.py` & `chemex-2022.3.2/chemex/experiments/catalog/cpmg_1hn_ap_0013.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,14 +40,16 @@
     ncyc_max: int
     taua: float = 2.38e-3
     ipap_flg: bool = False
     eburp_flg: bool = False
     reburp_flg: bool = False
     pw_eburp: float = 1.4e-3
     pw_reburp: float = 1.52e-3
+    time_equil_1: float = 0.0
+    time_equil_2: float = 0.0
     observed_state: Literal["a", "b", "c", "d"] = "a"
 
     @property
     def t_neg(self) -> float:
         return -2.0 * self.pw90 / np.pi
 
     @property
@@ -103,14 +105,16 @@
         }
         deltas[0.0] = self.settings.pw90 * self.settings.ncyc_max
         delays = [
             self.settings.taua,
             self.settings.t_neg,
             self.settings.pw_eburp,
             0.5 * self.settings.pw_reburp,
+            self.settings.time_equil_1,
+            self.settings.time_equil_2,
             *tau_cps.values(),
             *deltas.values(),
         ]
         return tau_cps, deltas, delays
 
     def _get_phases(self, ncyc: NDArrayFloat) -> tuple[NDArrayInt, NDArrayInt]:
         cp_phases1 = np.array(
@@ -136,14 +140,16 @@
         # Calculation of the spectrometers corresponding to all the delays
         tau_cps, deltas, all_delays = self._get_delays(ncycs)
         delays = dict(zip(all_delays, spectrometer.delays(all_delays)))
         d_neg = delays[self.settings.t_neg]
         d_taua = delays[self.settings.taua]
         d_eburp = delays[self.settings.pw_eburp]
         d_reburp = delays[0.5 * self.settings.pw_reburp]
+        d_eq_1 = delays[self.settings.time_equil_1]
+        d_eq_2 = delays[self.settings.time_equil_2]
         d_delta = {ncyc: delays[delay] for ncyc, delay in deltas.items()}
         d_cp = {ncyc: delays[delay] for ncyc, delay in tau_cps.items()}
 
         # Calculation of the spectrometers corresponding to all the pulses
         p90 = spectrometer.p90_i
         p180 = spectrometer.p180_i
         pp90_i = spectrometer.perfect90_i
@@ -165,23 +171,32 @@
         elif self.settings.reburp_flg:
             pp180pmy = spectrometer.perfect180_i[[1, 3]]
             middle = d_reburp @ pp180pmy @ d_reburp
         else:
             middle = p180[[1, 3]]
 
         # Calculating the intensities as a function of ncyc
-        centre = {0.0: d_delta[0] @ p90[0] @ middle @ p90[0]}
+        centre = {0.0: d_eq_2 @ d_delta[0] @ p90[0] @ middle @ p90[0] @ d_eq_1}
 
         for ncyc in set(ncycs) - {0.0}:
             phases1, phases2 = self._get_phases(ncyc)
             echo = d_cp[ncyc] @ p180 @ d_cp[ncyc]
             cpmg1 = reduce(np.matmul, echo[phases1.T])
             cpmg2 = reduce(np.matmul, echo[phases2.T])
             centre[ncyc] = (
-                d_delta[ncyc] @ p90[0] @ d_neg @ cpmg2 @ middle @ cpmg1 @ d_neg @ p90[0]
+                d_eq_2
+                @ d_delta[ncyc]
+                @ p90[0]
+                @ d_neg
+                @ cpmg2
+                @ middle
+                @ cpmg1
+                @ d_neg
+                @ p90[0]
+                @ d_eq_1
             )
 
         intst = {
             ncyc: spectrometer.detect(inept @ zfilter @ centre[ncyc] @ start)
             for ncyc in set(ncycs)
         }
```

### Comparing `chemex-2022.3.1/chemex/experiments/catalog/cpmg_ch3_13c_h2c.py` & `chemex-2022.3.2/chemex/experiments/catalog/cpmg_ch3_13c_h2c.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/experiments/catalog/cpmg_ch3_1h_dq.py` & `chemex-2022.3.2/chemex/experiments/catalog/cpmg_ch3_1h_dq.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/experiments/catalog/cpmg_ch3_1h_sq.py` & `chemex-2022.3.2/chemex/experiments/catalog/cpmg_ch3_1h_sq.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/experiments/catalog/cpmg_ch3_1h_tq.py` & `chemex-2022.3.2/chemex/experiments/catalog/cpmg_ch3_1h_tq.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/experiments/catalog/cpmg_ch3_1h_tq_diff.py` & `chemex-2022.3.2/chemex/experiments/catalog/cpmg_ch3_1h_tq_diff.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/experiments/catalog/cpmg_ch3_mq.py` & `chemex-2022.3.2/chemex/experiments/catalog/cpmg_ch3_mq.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/experiments/catalog/cpmg_chd2_1h_ap.py` & `chemex-2022.3.2/chemex/experiments/catalog/cpmg_chd2_1h_ap.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/experiments/catalog/cpmg_hn_dq_zq.py` & `chemex-2022.3.2/chemex/experiments/catalog/cpmg_hn_dq_zq.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/experiments/catalog/dcest_13c.py` & `chemex-2022.3.2/chemex/experiments/catalog/dcest_13c.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/experiments/catalog/dcest_15n.py` & `chemex-2022.3.2/chemex/experiments/catalog/dcest_15n.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/experiments/catalog/relaxation_hznz.py` & `chemex-2022.3.2/chemex/experiments/catalog/relaxation_hznz.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/experiments/catalog/relaxation_nz.py` & `chemex-2022.3.2/chemex/experiments/catalog/relaxation_nz.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/experiments/catalog/shift_15n_sq.py` & `chemex-2022.3.2/chemex/experiments/catalog/shift_15n_sq.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/experiments/catalog/shift_15n_sqmq.py` & `chemex-2022.3.2/chemex/experiments/catalog/shift_15n_sqmq.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/experiments/factories.py` & `chemex-2022.3.2/chemex/experiments/factories.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/experiments/loader.py` & `chemex-2022.3.2/chemex/experiments/loader.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/filterers.py` & `chemex-2022.3.2/chemex/filterers.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/messages.py` & `chemex-2022.3.2/chemex/messages.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/models/constraints.py` & `chemex-2022.3.2/chemex/models/constraints.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/models/factory.py` & `chemex-2022.3.2/chemex/models/factory.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/models/kinetic/settings_1st.py` & `chemex-2022.3.2/chemex/models/kinetic/settings_1st.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/models/kinetic/settings_2st.py` & `chemex-2022.3.2/chemex/models/kinetic/settings_2st.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/models/kinetic/settings_2st_a_a2.py` & `chemex-2022.3.2/chemex/models/kinetic/settings_2st_a_a2.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/models/kinetic/settings_2st_a_a3.py` & `chemex-2022.3.2/chemex/models/kinetic/settings_2st_a_a3.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/models/kinetic/settings_2st_a_a4.py` & `chemex-2022.3.2/chemex/models/kinetic/settings_2st_a_a4.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/models/kinetic/settings_2st_binding.py` & `chemex-2022.3.2/chemex/models/kinetic/settings_2st_binding.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/models/kinetic/settings_2st_eyring.py` & `chemex-2022.3.2/chemex/models/kinetic/settings_2st_eyring.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/models/kinetic/settings_2st_hd.py` & `chemex-2022.3.2/chemex/models/kinetic/settings_2st_hd.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/models/kinetic/settings_2st_rs.py` & `chemex-2022.3.2/chemex/models/kinetic/settings_2st_rs.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/models/kinetic/settings_3st_a_a2_a3.py` & `chemex-2022.3.2/chemex/models/kinetic/settings_3st_a_a2_a3.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/models/kinetic/settings_3st_a_a2_a4.py` & `chemex-2022.3.2/chemex/models/kinetic/settings_3st_a_a2_a4.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/models/kinetic/settings_3st_double_binding.py` & `chemex-2022.3.2/chemex/models/kinetic/settings_3st_double_binding.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/models/kinetic/settings_3st_eyring.py` & `chemex-2022.3.2/chemex/models/kinetic/settings_3st_eyring.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/models/kinetic/settings_3st_induced_fit.py` & `chemex-2022.3.2/chemex/models/kinetic/settings_3st_induced_fit.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/models/kinetic/settings_4st_hd.py` & `chemex-2022.3.2/chemex/models/kinetic/settings_4st_hd.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/models/kinetic/settings_nst.py` & `chemex-2022.3.2/chemex/models/kinetic/settings_nst.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/models/loader.py` & `chemex-2022.3.2/chemex/models/loader.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/models/model.py` & `chemex-2022.3.2/chemex/models/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,50 +4,50 @@
 from string import ascii_lowercase
 
 from chemex.models.factory import model_factory
 
 
 @dataclass
 class _Model:
-    __name: str = "2st"
-    __states: str = "ab"
-    __model_free: bool = False
-    __temp_coef: bool = False
+    _name: str = "2st"
+    _states: str = "ab"
+    _model_free: bool = False
+    _temp_coef: bool = False
 
     @staticmethod
     def validate_model_name(name: str) -> str:
         if name not in model_factory.set:
             print("Warning: The 'model' option should either be:")
             for model_name in sorted(model_factory.set):
                 print(f"    - '{model_name}'")
             print("Set to the default value: '2st'.")
             return "2st"
         return name
 
     def set_model(self, name: str) -> None:
         kinetic_model_name, *ext = name.split(".")
-        self.__name = self.validate_model_name(kinetic_model_name)
+        self._name = self.validate_model_name(kinetic_model_name)
         state_nb = int(kinetic_model_name[0])
-        self.__states = ascii_lowercase[:state_nb]
-        self.__model_free = "mf" in ext if ext else False
-        self.__temp_coef = "tc" in ext if ext else False
+        self._states = ascii_lowercase[:state_nb]
+        self._model_free = "mf" in ext if ext else False
+        self._temp_coef = "tc" in ext if ext else False
 
     @property
     def name(self) -> str:
-        return self.__name
+        return self._name
 
     @property
     def states(self) -> str:
-        return self.__states
+        return self._states
 
     @property
     def model_free(self) -> bool:
-        return self.__model_free
+        return self._model_free
 
     @property
     def temp_coef(self) -> bool:
-        return self.__temp_coef
+        return self._temp_coef
 
 
 model = _Model()
 
 set_model = model.set_model
```

### Comparing `chemex-2022.3.1/chemex/nmr/basis.py` & `chemex-2022.3.2/chemex/nmr/basis.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/nmr/constants.py` & `chemex-2022.3.2/chemex/nmr/constants.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/nmr/liouvillian.py` & `chemex-2022.3.2/chemex/nmr/liouvillian.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/nmr/rates.py` & `chemex-2022.3.2/chemex/nmr/rates.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/nmr/spectrometer.py` & `chemex-2022.3.2/chemex/nmr/spectrometer.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/optimize/fitting.py` & `chemex-2022.3.2/chemex/optimize/fitting.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/optimize/gridding.py` & `chemex-2022.3.2/chemex/optimize/gridding.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/optimize/grouping.py` & `chemex-2022.3.2/chemex/optimize/grouping.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/optimize/helper.py` & `chemex-2022.3.2/chemex/optimize/helper.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/optimize/minimizer.py` & `chemex-2022.3.2/chemex/optimize/minimizer.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/parameters/database.py` & `chemex-2022.3.2/chemex/parameters/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,14 +158,15 @@
             ids_modified.update(matching_ids)
 
         return self._count_per_section(ids_modified)
 
     def fix_all(self) -> None:
         for parameter in self._parameters.values():
             parameter.vary = False
+            parameter.expr = ""
 
     def _get_ids_left(self, expression: str) -> set[str]:
         return self.get_matching_ids(ParamName.from_section(expression))
 
     def _get_ids_right(self, expression: str) -> dict[str, set[str]]:
         ids_right = {}
         for match in _RE_PARAM_NAME.finditer(expression):
```

### Comparing `chemex-2022.3.1/chemex/parameters/factory.py` & `chemex-2022.3.2/chemex/parameters/factory.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/parameters/name.py` & `chemex-2022.3.2/chemex/parameters/name.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/parameters/setting.py` & `chemex-2022.3.2/chemex/parameters/setting.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/parameters/spin_system.py` & `chemex-2022.3.2/chemex/parameters/spin_system.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,23 +117,23 @@
 @total_ordering
 class Group:
     NO_NUMBER: int = -100000000
 
     def __init__(self, name: str) -> None:
         self.symbol, self.number, self.suffix = self.parse_group(name.strip().upper())
         self.symbol = AAA_TO_A.get(self.symbol, self.symbol)
-        self.name = self.get_name()
         self.search_keys: set = {self} if self else set()
 
     def parse_group(self, name: str) -> tuple[str, int, str]:
         if found := search("[0-9]+", name.strip().upper()):
             return name[: found.start()], int(found.group()), name[found.end() :]
         return name, self.NO_NUMBER, ""
 
-    def get_name(self) -> str:
+    @property
+    def name(self) -> str:
         number = "" if self.number == self.NO_NUMBER else self.number
         return f"{self.symbol}{number}{self.suffix}"
 
     def match(self, other: Group) -> bool:
         symbol = other.symbol == self.symbol or not self.symbol
         number = other.number == self.number or self.number == self.NO_NUMBER
         suffix = other.suffix == self.suffix or not self.suffix
@@ -161,15 +161,14 @@
 
 @total_ordering
 class Spin:
     def __init__(self, name: str, group_for_completion: Group | None = None) -> None:
         self.group, self.atom = self.split_group_atom(name.strip().upper())
         if not self.group and group_for_completion:
             self.group = group_for_completion
-        self.name = self.get_name()
         self.search_keys = self.group.search_keys | self.atom.search_keys
 
     @staticmethod
     def split_group_atom(name: str) -> tuple[Group, Atom]:
         if name == "?":
             return Group(""), Atom("")
         found_digit = search("[0-9]", name)
@@ -178,15 +177,16 @@
         if not found_atom:
             if name in STANDARD_ATOM_NAMES:
                 return Group(""), Atom(name)
             return Group(name), Atom("")
         atom_index = first_digit + found_atom.start()
         return Group(name[:atom_index]), Atom(name[atom_index:])
 
-    def get_name(self) -> str:
+    @property
+    def name(self) -> str:
         return f"{self.group}{self.atom}"
 
     def match(self, other: Spin):
         return self.group.match(other.group) and self.atom.match(other.atom)
 
     def __lt__(self, other: Spin) -> bool:
         self_tuple = (self.atom.nucleus.name, self.group, self.atom)
```

### Comparing `chemex-2022.3.1/chemex/parameters/spins.py` & `chemex-2022.3.2/chemex/parameters/spins.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/parameters/userfunctions.py` & `chemex-2022.3.2/chemex/parameters/userfunctions.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/plotters/cest.py` & `chemex-2022.3.2/chemex/plotters/cest.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/plotters/cpmg.py` & `chemex-2022.3.2/chemex/plotters/cpmg.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/plotters/plot.py` & `chemex-2022.3.2/chemex/plotters/plot.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/plotters/relaxation.py` & `chemex-2022.3.2/chemex/plotters/relaxation.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/plotters/shift.py` & `chemex-2022.3.2/chemex/plotters/shift.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/printers/data.py` & `chemex-2022.3.2/chemex/printers/data.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/printers/parameters.py` & `chemex-2022.3.2/chemex/printers/parameters.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/printers/plot.py` & `chemex-2022.3.2/chemex/printers/plot.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/toml.py` & `chemex-2022.3.2/chemex/toml.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/tools/pick_cest.py` & `chemex-2022.3.2/chemex/tools/pick_cest.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/tools/plot_param.py` & `chemex-2022.3.2/chemex/tools/plot_param.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/chemex/uncertainty.py` & `chemex-2022.3.2/chemex/uncertainty.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.1/pyproject.toml` & `chemex-2022.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chemex"
-version = "2022.3.1"
+version = "2022.3.2"
 description = "ChemEx is an analysis program for chemical exchange detected by NMR"
 authors = ["Guillaume Bouvignies <gbouvignies@gmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/gbouvignies/chemex"
 homepage = "http://gbouvignies.github.io/ChemEx/"
 classifiers = [
```

### Comparing `chemex-2022.3.1/PKG-INFO` & `chemex-2022.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chemex
-Version: 2022.3.1
+Version: 2022.3.2
 Summary: ChemEx is an analysis program for chemical exchange detected by NMR
 Home-page: http://gbouvignies.github.io/ChemEx/
 License: GPL-3.0-only
 Author: Guillaume Bouvignies
 Author-email: gbouvignies@gmail.com
 Requires-Python: >=3.9,<3.11
 Classifier: Intended Audience :: Science/Research
```


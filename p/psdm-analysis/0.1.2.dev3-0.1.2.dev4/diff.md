# Comparing `tmp/psdm-analysis-0.1.2.dev3.tar.gz` & `tmp/psdm-analysis-0.1.2.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psdm-analysis-0.1.2.dev3.tar", max compression
+gzip compressed data, was "psdm-analysis-0.1.2.dev4.tar", max compression
```

## Comparing `psdm-analysis-0.1.2.dev3.tar` & `psdm-analysis-0.1.2.dev4.tar`

### file list

```diff
@@ -1,62 +1,63 @@
--rw-r--r--   0        0        0     1581 2023-01-31 09:55:39.404671 psdm-analysis-0.1.2.dev3/LICENSE
--rw-r--r--   0        0        0      373 2023-02-06 12:47:42.418947 psdm-analysis-0.1.2.dev3/README.md
--rw-r--r--   0        0        0        0 2023-01-31 09:55:39.404953 psdm-analysis-0.1.2.dev3/psdm_analysis/__init__.py
--rw-r--r--   0        0        0        0 2022-10-31 07:56:26.279000 psdm-analysis-0.1.2.dev3/psdm_analysis/analysis/__init__.py
--rw-r--r--   0        0        0      601 2022-10-31 07:56:26.279000 psdm-analysis-0.1.2.dev3/psdm_analysis/analysis/calc.py
--rw-r--r--   0        0        0     1200 2023-03-10 10:05:58.780408 psdm-analysis-0.1.2.dev3/psdm_analysis/analysis/grid.py
--rw-r--r--   0        0        0        0 2022-10-31 07:56:26.279000 psdm-analysis-0.1.2.dev3/psdm_analysis/io/__init__.py
--rw-r--r--   0        0        0     2790 2023-03-15 13:03:26.349577 psdm-analysis-0.1.2.dev3/psdm_analysis/io/utils.py
--rw-r--r--   0        0        0        0 2022-10-31 07:56:26.280000 psdm-analysis-0.1.2.dev3/psdm_analysis/models/__init__.py
--rw-r--r--   0        0        0     7232 2023-03-15 13:03:30.029189 psdm-analysis-0.1.2.dev3/psdm_analysis/models/entity.py
--rw-r--r--   0        0        0     5922 2023-03-09 08:16:57.841881 psdm-analysis-0.1.2.dev3/psdm_analysis/models/grid_with_results.py
--rw-r--r--   0        0        0        0 2022-10-31 07:56:26.280000 psdm-analysis-0.1.2.dev3/psdm_analysis/models/input/__init__.py
--rw-r--r--   0        0        0        0 2022-10-31 07:56:26.281000 psdm-analysis-0.1.2.dev3/psdm_analysis/models/input/connector/__init__.py
--rw-r--r--   0        0        0     2126 2023-03-10 10:57:43.319027 psdm-analysis-0.1.2.dev3/psdm_analysis/models/input/connector/lines.py
--rw-r--r--   0        0        0      578 2023-03-10 10:57:43.310448 psdm-analysis-0.1.2.dev3/psdm_analysis/models/input/connector/switches.py
--rw-r--r--   0        0        0     2447 2023-03-10 08:30:28.809992 psdm-analysis-0.1.2.dev3/psdm_analysis/models/input/connector/transformer.py
--rw-r--r--   0        0        0        0 2022-10-31 07:56:26.281000 psdm-analysis-0.1.2.dev3/psdm_analysis/models/input/container/__init__.py
--rw-r--r--   0        0        0     3925 2023-03-15 13:03:26.349736 psdm-analysis-0.1.2.dev3/psdm_analysis/models/input/container/grid_container.py
--rw-r--r--   0        0        0     3471 2023-03-15 13:03:26.353051 psdm-analysis-0.1.2.dev3/psdm_analysis/models/input/container/mixins.py
--rw-r--r--   0        0        0     6113 2023-03-10 12:50:34.862218 psdm-analysis-0.1.2.dev3/psdm_analysis/models/input/container/participants_container.py
--rw-r--r--   0        0        0     1884 2023-03-10 10:05:58.775987 psdm-analysis-0.1.2.dev3/psdm_analysis/models/input/enums.py
--rw-r--r--   0        0        0     1129 2023-03-09 10:52:57.686227 psdm-analysis-0.1.2.dev3/psdm_analysis/models/input/node.py
--rw-r--r--   0        0        0        0 2022-10-31 07:56:26.282000 psdm-analysis-0.1.2.dev3/psdm_analysis/models/input/participant/__init__.py
--rw-r--r--   0        0        0     1402 2023-03-10 09:59:49.646961 psdm-analysis-0.1.2.dev3/psdm_analysis/models/input/participant/bm.py
--rw-r--r--   0        0        0     3131 2023-02-13 16:22:32.837449 psdm-analysis-0.1.2.dev3/psdm_analysis/models/input/participant/charging.py
--rw-r--r--   0        0        0      654 2023-03-07 14:13:45.241862 psdm-analysis-0.1.2.dev3/psdm_analysis/models/input/participant/em.py
--rw-r--r--   0        0        0      936 2023-03-07 14:13:52.999849 psdm-analysis-0.1.2.dev3/psdm_analysis/models/input/participant/evcs.py
--rw-r--r--   0        0        0      971 2023-03-10 09:59:49.649913 psdm-analysis-0.1.2.dev3/psdm_analysis/models/input/participant/evs.py
--rw-r--r--   0        0        0      527 2023-03-07 14:14:05.804367 psdm-analysis-0.1.2.dev3/psdm_analysis/models/input/participant/fixed_feed_in.py
--rw-r--r--   0        0        0      806 2023-03-10 09:59:49.640692 psdm-analysis-0.1.2.dev3/psdm_analysis/models/input/participant/hp.py
--rw-r--r--   0        0        0      953 2023-03-07 14:14:17.158339 psdm-analysis-0.1.2.dev3/psdm_analysis/models/input/participant/load.py
--rw-r--r--   0        0        0     1032 2023-03-10 12:50:34.867015 psdm-analysis-0.1.2.dev3/psdm_analysis/models/input/participant/participant.py
--rw-r--r--   0        0        0     1320 2023-03-07 14:14:27.737375 psdm-analysis-0.1.2.dev3/psdm_analysis/models/input/participant/pv.py
--rw-r--r--   0        0        0     1541 2023-03-10 09:59:49.643881 psdm-analysis-0.1.2.dev3/psdm_analysis/models/input/participant/storage.py
--rw-r--r--   0        0        0     1143 2023-03-10 09:39:46.024226 psdm-analysis-0.1.2.dev3/psdm_analysis/models/input/participant/wec.py
--rw-r--r--   0        0        0     2887 2023-02-05 09:44:03.774951 psdm-analysis-0.1.2.dev3/psdm_analysis/models/primary_data.py
--rw-r--r--   0        0        0        0 2022-10-31 07:56:26.283000 psdm-analysis-0.1.2.dev3/psdm_analysis/models/result/__init__.py
--rw-r--r--   0        0        0     2243 2023-01-02 10:54:15.863000 psdm-analysis-0.1.2.dev3/psdm_analysis/models/result/flex_option.py
--rw-r--r--   0        0        0        0 2022-12-12 11:44:36.942000 psdm-analysis-0.1.2.dev3/psdm_analysis/models/result/grid/__init__.py
--rw-r--r--   0        0        0     2271 2023-03-07 14:09:10.191710 psdm-analysis-0.1.2.dev3/psdm_analysis/models/result/grid/enhanced_node.py
--rw-r--r--   0        0        0     3640 2023-03-15 13:03:26.368243 psdm-analysis-0.1.2.dev3/psdm_analysis/models/result/grid/node.py
--rw-r--r--   0        0        0        0 2022-11-07 09:58:45.661000 psdm-analysis-0.1.2.dev3/psdm_analysis/models/result/participant/__init__.py
--rw-r--r--   0        0        0     3645 2023-03-09 08:16:57.850633 psdm-analysis-0.1.2.dev3/psdm_analysis/models/result/participant/dict.py
--rw-r--r--   0        0        0     3170 2023-02-13 16:22:32.848887 psdm-analysis-0.1.2.dev3/psdm_analysis/models/result/participant/flex_options.py
--rw-r--r--   0        0        0     6179 2023-03-09 08:16:57.870452 psdm-analysis-0.1.2.dev3/psdm_analysis/models/result/participant/participant.py
--rw-r--r--   0        0        0     9604 2023-03-09 08:16:57.883582 psdm-analysis-0.1.2.dev3/psdm_analysis/models/result/participant/participants_res_container.py
--rw-r--r--   0        0        0     5741 2023-03-09 08:21:54.119152 psdm-analysis-0.1.2.dev3/psdm_analysis/models/result/power.py
--rw-r--r--   0        0        0     2096 2023-03-15 13:04:31.048733 psdm-analysis-0.1.2.dev3/psdm_analysis/models/result/res_container.py
--rw-r--r--   0        0        0        0 2022-10-31 07:56:26.284000 psdm-analysis-0.1.2.dev3/psdm_analysis/plots/__init__.py
--rw-r--r--   0        0        0        0 2022-10-31 07:56:26.284000 psdm-analysis-0.1.2.dev3/psdm_analysis/plots/results/__init__.py
--rw-r--r--   0        0        0     2431 2023-02-05 09:37:19.218355 psdm-analysis-0.1.2.dev3/psdm_analysis/plots/results/bar_plot.py
--rw-r--r--   0        0        0     3461 2023-02-21 11:37:43.193646 psdm-analysis-0.1.2.dev3/psdm_analysis/plots/results/flex_plot.py
--rw-r--r--   0        0        0     1096 2023-02-21 11:47:22.103016 psdm-analysis-0.1.2.dev3/psdm_analysis/plots/results/line_plot.py
--rw-r--r--   0        0        0     1083 2023-02-13 14:56:08.018673 psdm-analysis-0.1.2.dev3/psdm_analysis/plots/results/nodes.py
--rw-r--r--   0        0        0    11946 2023-03-07 14:09:10.271592 psdm-analysis-0.1.2.dev3/psdm_analysis/plots/results/power_plot.py
--rw-r--r--   0        0        0     4105 2023-03-13 15:22:36.170856 psdm-analysis-0.1.2.dev3/psdm_analysis/plots/utils.py
--rw-r--r--   0        0        0        0 2022-11-03 09:12:48.266000 psdm-analysis-0.1.2.dev3/psdm_analysis/processing/__init__.py
--rw-r--r--   0        0        0     1213 2023-02-01 12:19:09.699932 psdm-analysis-0.1.2.dev3/psdm_analysis/processing/dataframe.py
--rw-r--r--   0        0        0     2103 2023-03-09 08:23:16.593280 psdm-analysis-0.1.2.dev3/psdm_analysis/processing/series.py
--rw-r--r--   0        0        0      650 2023-03-15 13:05:34.534695 psdm-analysis-0.1.2.dev3/pyproject.toml
--rw-r--r--   0        0        0     1616 1970-01-01 00:00:00.000000 psdm-analysis-0.1.2.dev3/setup.py
--rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 psdm-analysis-0.1.2.dev3/PKG-INFO
+-rw-r--r--   0        0        0     1581 2023-01-31 09:55:39.404671 psdm-analysis-0.1.2.dev4/LICENSE
+-rw-r--r--   0        0        0      373 2023-04-19 12:49:15.037328 psdm-analysis-0.1.2.dev4/README.md
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.038177 psdm-analysis-0.1.2.dev4/psdm_analysis/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.038287 psdm-analysis-0.1.2.dev4/psdm_analysis/analysis/__init__.py
+-rw-r--r--   0        0        0      601 2023-04-19 12:49:15.038571 psdm-analysis-0.1.2.dev4/psdm_analysis/analysis/calc.py
+-rw-r--r--   0        0        0     1200 2023-04-19 12:49:15.038918 psdm-analysis-0.1.2.dev4/psdm_analysis/analysis/grid.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.038964 psdm-analysis-0.1.2.dev4/psdm_analysis/io/__init__.py
+-rw-r--r--   0        0        0     2842 2023-04-19 12:49:15.039092 psdm-analysis-0.1.2.dev4/psdm_analysis/io/utils.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.039122 psdm-analysis-0.1.2.dev4/psdm_analysis/models/__init__.py
+-rw-r--r--   0        0        0     7232 2023-04-19 12:49:15.039262 psdm-analysis-0.1.2.dev4/psdm_analysis/models/entity.py
+-rw-r--r--   0        0        0     5988 2023-04-19 12:49:15.039392 psdm-analysis-0.1.2.dev4/psdm_analysis/models/grid_with_results.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.039422 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.039466 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/connector/__init__.py
+-rw-r--r--   0        0        0     2126 2023-04-19 12:49:15.039712 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/connector/lines.py
+-rw-r--r--   0        0        0      578 2023-04-19 12:49:15.039922 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/connector/switches.py
+-rw-r--r--   0        0        0     2455 2023-04-19 12:49:15.040033 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/connector/transformer.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.040065 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/container/__init__.py
+-rw-r--r--   0        0        0     3925 2023-04-19 12:49:15.040286 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/container/grid_container.py
+-rw-r--r--   0        0        0     3456 2023-04-19 12:49:15.040383 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/container/mixins.py
+-rw-r--r--   0        0        0     6113 2023-04-19 12:49:15.040661 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/container/participants_container.py
+-rw-r--r--   0        0        0     1884 2023-04-19 12:49:15.040834 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/enums.py
+-rw-r--r--   0        0        0     1129 2023-04-19 12:49:15.041071 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/node.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.041104 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/__init__.py
+-rw-r--r--   0        0        0     1368 2023-04-19 12:49:15.041213 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/bm.py
+-rw-r--r--   0        0        0     3138 2023-04-19 12:49:15.041309 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/charging.py
+-rw-r--r--   0        0        0      654 2023-04-19 12:49:15.041628 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/em.py
+-rw-r--r--   0        0        0      936 2023-04-19 12:49:15.041802 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/evcs.py
+-rw-r--r--   0        0        0      965 2023-04-19 12:49:15.041899 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/evs.py
+-rw-r--r--   0        0        0      527 2023-04-19 12:49:15.042031 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/fixed_feed_in.py
+-rw-r--r--   0        0        0      814 2023-04-19 12:49:15.042128 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/hp.py
+-rw-r--r--   0        0        0      953 2023-04-19 12:49:15.042385 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/load.py
+-rw-r--r--   0        0        0     1032 2023-04-19 12:49:15.042559 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/participant.py
+-rw-r--r--   0        0        0     1320 2023-04-19 12:49:15.042694 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/pv.py
+-rw-r--r--   0        0        0     1527 2023-04-19 12:49:15.042799 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/storage.py
+-rw-r--r--   0        0        0     1113 2023-04-19 12:49:15.042895 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/wec.py
+-rw-r--r--   0        0        0     2887 2023-04-19 12:49:15.043116 psdm-analysis-0.1.2.dev4/psdm_analysis/models/primary_data.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.043156 psdm-analysis-0.1.2.dev4/psdm_analysis/models/result/__init__.py
+-rw-r--r--   0        0        0     2243 2023-04-19 12:49:15.043509 psdm-analysis-0.1.2.dev4/psdm_analysis/models/result/flex_option.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.043543 psdm-analysis-0.1.2.dev4/psdm_analysis/models/result/grid/__init__.py
+-rw-r--r--   0        0        0     2314 2023-04-19 12:49:15.043655 psdm-analysis-0.1.2.dev4/psdm_analysis/models/result/grid/enhanced_node.py
+-rw-r--r--   0        0        0     3670 2023-04-19 12:49:15.043790 psdm-analysis-0.1.2.dev4/psdm_analysis/models/result/grid/node.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.043823 psdm-analysis-0.1.2.dev4/psdm_analysis/models/result/participant/__init__.py
+-rw-r--r--   0        0        0     3645 2023-04-19 12:49:15.043937 psdm-analysis-0.1.2.dev4/psdm_analysis/models/result/participant/dict.py
+-rw-r--r--   0        0        0     3170 2023-04-19 12:49:15.044163 psdm-analysis-0.1.2.dev4/psdm_analysis/models/result/participant/flex_options.py
+-rw-r--r--   0        0        0     6261 2023-04-19 12:49:15.044315 psdm-analysis-0.1.2.dev4/psdm_analysis/models/result/participant/participant.py
+-rw-r--r--   0        0        0     9664 2023-04-19 12:49:15.044458 psdm-analysis-0.1.2.dev4/psdm_analysis/models/result/participant/participants_res_container.py
+-rw-r--r--   0        0        0     5776 2023-04-19 12:49:15.044578 psdm-analysis-0.1.2.dev4/psdm_analysis/models/result/power.py
+-rw-r--r--   0        0        0     2340 2023-04-19 12:49:15.044687 psdm-analysis-0.1.2.dev4/psdm_analysis/models/result/res_container.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.044717 psdm-analysis-0.1.2.dev4/psdm_analysis/plots/__init__.py
+-rw-r--r--   0        0        0     1349 2023-04-19 12:49:15.044823 psdm-analysis-0.1.2.dev4/psdm_analysis/plots/grid.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.044851 psdm-analysis-0.1.2.dev4/psdm_analysis/plots/results/__init__.py
+-rw-r--r--   0        0        0     2431 2023-04-19 12:49:15.045086 psdm-analysis-0.1.2.dev4/psdm_analysis/plots/results/bar_plot.py
+-rw-r--r--   0        0        0     3461 2023-04-19 12:49:15.045391 psdm-analysis-0.1.2.dev4/psdm_analysis/plots/results/flex_plot.py
+-rw-r--r--   0        0        0     1096 2023-04-19 12:49:15.045589 psdm-analysis-0.1.2.dev4/psdm_analysis/plots/results/line_plot.py
+-rw-r--r--   0        0        0     1083 2023-04-19 12:49:15.045811 psdm-analysis-0.1.2.dev4/psdm_analysis/plots/results/nodes.py
+-rw-r--r--   0        0        0    11954 2023-04-19 12:49:15.045955 psdm-analysis-0.1.2.dev4/psdm_analysis/plots/results/power_plot.py
+-rw-r--r--   0        0        0     4096 2023-04-19 12:49:15.046076 psdm-analysis-0.1.2.dev4/psdm_analysis/plots/utils.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.046127 psdm-analysis-0.1.2.dev4/psdm_analysis/processing/__init__.py
+-rw-r--r--   0        0        0     1217 2023-04-19 12:49:15.046231 psdm-analysis-0.1.2.dev4/psdm_analysis/processing/dataframe.py
+-rw-r--r--   0        0        0     2174 2023-04-19 12:49:15.046324 psdm-analysis-0.1.2.dev4/psdm_analysis/processing/series.py
+-rw-r--r--   0        0        0      668 2023-04-19 12:50:52.147307 psdm-analysis-0.1.2.dev4/pyproject.toml
+-rw-r--r--   0        0        0     1636 1970-01-01 00:00:00.000000 psdm-analysis-0.1.2.dev4/setup.py
+-rw-r--r--   0        0        0      997 1970-01-01 00:00:00.000000 psdm-analysis-0.1.2.dev4/PKG-INFO
```

### Comparing `psdm-analysis-0.1.2.dev3/LICENSE` & `psdm-analysis-0.1.2.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev3/psdm_analysis/analysis/calc.py` & `psdm-analysis-0.1.2.dev4/psdm_analysis/analysis/calc.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev3/psdm_analysis/analysis/grid.py` & `psdm-analysis-0.1.2.dev4/psdm_analysis/analysis/grid.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev3/psdm_analysis/io/utils.py` & `psdm-analysis-0.1.2.dev4/psdm_analysis/io/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 from datetime import datetime
 from pathlib import Path
+from typing import Optional
 
 import pandas as pd
 from pandas import DataFrame
 from pandas.core.groupby import DataFrameGroupBy
 
 ROOT_DIR = os.path.abspath(__file__ + "/../../../")
 
@@ -61,20 +62,20 @@
     data = read_csv(simulation_data_path, file_name, delimiter)
 
     if "uuid" in data.columns:
         data = data.drop(columns=["uuid"])
     return data.groupby(by="input_model")
 
 
-def check_filter(filter_start: datetime, filter_end: datetime):
+def check_filter(filter_start: Optional[datetime], filter_end: Optional[datetime]):
     if (filter_start or filter_end) and not (filter_start and filter_end):
         raise ValueError(
             "Both start and end of the filter must be provided if one is provided."
         )
-    if filter_start and filter_end and filter_start > filter_end:
+    if (filter_start and filter_end) and (filter_start > filter_end):
         raise ValueError("Filter start must be before end.")
 
 
 def df_to_csv(df: DataFrame, path: str, file_name: str, delimiter: str):
     full_path = get_file_path(path, file_name)
     df = df.replace(True, "true")
     df = df.replace(False, "false")
```

### Comparing `psdm-analysis-0.1.2.dev3/psdm_analysis/models/entity.py` & `psdm-analysis-0.1.2.dev4/psdm_analysis/models/entity.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev3/psdm_analysis/models/grid_with_results.py` & `psdm-analysis-0.1.2.dev4/psdm_analysis/models/grid_with_results.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 from dataclasses import dataclass
 from datetime import datetime
-from typing import List
+from typing import List, Optional, Tuple
 
 from psdm_analysis.io.utils import check_filter
 from psdm_analysis.models.input.container.grid_container import GridContainer
 from psdm_analysis.models.input.container.participants_container import (
     SystemParticipantsContainer,
 )
 from psdm_analysis.models.input.enums import RawGridElementsEnum, SystemParticipantsEnum
@@ -27,19 +27,19 @@
     def from_csv(
         cls,
         name: str,
         grid_path: str,
         grid_delimiter: str,
         result_path: str,
         result_delimiter: str,
-        primary_data_delimiter: str = None,
-        simulation_end: datetime = None,
+        primary_data_delimiter: Optional[str] = None,
+        simulation_end: Optional[datetime] = None,
         from_agg_results: bool = False,
-        filter_start: datetime = None,
-        filter_end: datetime = None,
+        filter_start: Optional[datetime] = None,
+        filter_end: Optional[datetime] = None,
     ) -> "GridWithResults":
         check_filter(filter_start, filter_end)
 
         if not primary_data_delimiter:
             primary_data_delimiter = grid_delimiter
 
         grid = GridContainer.from_csv(
@@ -123,15 +123,15 @@
                     + "within the participant results of the"
                     + str(type(participant_results))
                 )
         return ParticipantsResult(participant, res)
 
     def em_results(
         self,
-    ) -> [(SystemParticipantsContainer, ParticipantsResultContainer)]:
+    ) -> List[Tuple[SystemParticipantsContainer, ParticipantsResultContainer]]:
         uuid_to_connected_asset = self.grid.participants.ems.uuid_to_connected_assets()
         return [
             (
                 self.grid.participants.subset(connected_assets + [em_uuid]),
                 self.results.participants.subset(connected_assets + [em_uuid]),
             )
             for (em_uuid, connected_assets) in uuid_to_connected_asset.items()
```

### Comparing `psdm-analysis-0.1.2.dev3/psdm_analysis/models/input/connector/lines.py` & `psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/connector/lines.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev3/psdm_analysis/models/input/connector/switches.py` & `psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/connector/switches.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev3/psdm_analysis/models/input/connector/transformer.py` & `psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/connector/transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,26 +84,26 @@
         return self.data["tap_min"]
 
     @property
     def tap_max(self):
         return self.data["tap_max"]
 
     @staticmethod
-    def entity_attributes() -> [str]:
+    def entity_attributes() -> list[str]:
         return [
             "node_a",
             "node_b",
             "parallel_devices",
             "type_id",
             "tap_pos",
             "auto_tap",
         ]
 
     @staticmethod
-    def type_attributes() -> [str]:
+    def type_attributes() -> list[str]:
         return [
             "r_sc",
             "x_sc",
             "g_m",
             "b_m",
             "s_rated",
             "v_rated_a",
```

### Comparing `psdm-analysis-0.1.2.dev3/psdm_analysis/models/input/container/grid_container.py` & `psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/container/grid_container.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev3/psdm_analysis/models/input/container/mixins.py` & `psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/container/mixins.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import logging
 from abc import ABC, abstractmethod
 
-from psdm_analysis.io import utils
 from psdm_analysis.io.utils import df_to_csv
 from psdm_analysis.models.entity import Entities
 from psdm_analysis.models.input.enums import EntitiesEnum
 from psdm_analysis.models.input.participant.participant import SystemParticipants
 
 
 class ContainerMixin(ABC):
@@ -59,15 +58,15 @@
             type_data.drop_duplicates(),
             path,
             self.get_enum().get_type_file_name(),
             delimiter,
         )
 
     @classmethod
-    def attributes(cls, include_type_attrs: bool = True) -> [str]:
+    def attributes(cls, include_type_attrs: bool = True) -> list[str]:
         base_attributes = []
         # check if cls is a subclass of SystemParticipants
         if issubclass(cls, SystemParticipants):
             base_attributes += SystemParticipants.attributes()
         elif issubclass(cls, Entities):
             base_attributes += Entities.attributes()
         else:
@@ -79,19 +78,19 @@
             all_entity_attributes + cls.type_attributes()
             if include_type_attrs
             else all_entity_attributes
         )
 
     @staticmethod
     @abstractmethod
-    def entity_attributes() -> [str]:
+    def entity_attributes() -> list[str]:
         pass
 
     @staticmethod
-    def type_attributes() -> [str]:
+    def type_attributes() -> list[str]:
         return ["type_uuid", "type_id"]
 
 
 class SpTypeMixin(HasTypeMixin):
     @property
     def capex(self):
         return self.data["capex"]
@@ -106,18 +105,18 @@
 
     @property
     def cos_phi_rated(self):
         return self.data["cos_phi_rated"]
 
     @staticmethod
     @abstractmethod
-    def entity_attributes() -> [str]:
+    def entity_attributes() -> list[str]:
         pass
 
     @staticmethod
-    def type_attributes() -> [str]:
+    def type_attributes() -> list[str]:
         return HasTypeMixin.type_attributes() + [
             "capex",
             "opex",
             "s_rated",
             "cos_phi_rated",
         ]
```

### Comparing `psdm-analysis-0.1.2.dev3/psdm_analysis/models/input/container/participants_container.py` & `psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/container/participants_container.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev3/psdm_analysis/models/input/enums.py` & `psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/enums.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev3/psdm_analysis/models/input/node.py` & `psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/node.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev3/psdm_analysis/models/input/participant/bm.py` & `psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/bm.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from dataclasses import dataclass
-from typing import List
 
-from psdm_analysis.models.input.container.mixins import HasTypeMixin, SpTypeMixin
+from psdm_analysis.models.input.container.mixins import SpTypeMixin
 from psdm_analysis.models.input.enums import SystemParticipantsEnum
 from psdm_analysis.models.input.participant.participant import SystemParticipants
 
 
 @dataclass(frozen=True)
 class BiomassPlants(SystemParticipants, SpTypeMixin):
     @staticmethod
@@ -29,23 +28,23 @@
         return self.data["active_power_gradient"]
 
     @property
     def eta_conv(self):
         return self.data["eta_conv"]
 
     @staticmethod
-    def entity_attributes() -> List[str]:
+    def entity_attributes() -> list[str]:
         return SystemParticipants.attributes() + [
             "type",
             "market_reaction",
             "cost_controlled",
             "feed_in_tariff",
             "type_id",
             "active_power_gradient",
         ]
 
     @staticmethod
-    def type_attributes() -> [str]:
+    def type_attributes() -> list[str]:
         return SpTypeMixin.type_attributes() + [
             "active_power_gradient",
             "eta_conv",
         ]
```

### Comparing `psdm-analysis-0.1.2.dev3/psdm_analysis/models/input/participant/charging.py` & `psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/charging.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         return common_type
 
     regex = r"\(.*\)$"
     match = re.search(regex, type_str)
     if match:
         power, current_type = match.group().strip("()").split("|")
         current_type = CurrentType[current_type]
-        return ChargingPointType(type_str, power, current_type, set())
+        return ChargingPointType(type_str, float(power), current_type, set())
     else:
         raise ValueError(f"Can not determine power of {type_str}!")
 
 
 def parse_evcs_type_info(type_str: str):
     evcs_type = parse_evcs_type(type_str)
     return pd.Series(evcs_type.__dict__)
```

### Comparing `psdm-analysis-0.1.2.dev3/psdm_analysis/models/input/participant/em.py` & `psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/em.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev3/psdm_analysis/models/input/participant/evcs.py` & `psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/evcs.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev3/psdm_analysis/models/input/participant/evs.py` & `psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/evs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from dataclasses import dataclass
 
-from psdm_analysis.models.input.container.mixins import HasTypeMixin, SpTypeMixin
+from psdm_analysis.models.input.container.mixins import SpTypeMixin
 from psdm_analysis.models.input.enums import SystemParticipantsEnum
 from psdm_analysis.models.input.participant.participant import (
     SystemParticipantsWithCapacity,
 )
 
 
 @dataclass(frozen=True)
@@ -22,16 +22,16 @@
         return self.data["e_storage"]
 
     @property
     def e_cons(self):
         return self.data["e_cons"]
 
     @staticmethod
-    def entity_attributes() -> [str]:
+    def entity_attributes() -> list[str]:
         return []
 
     @staticmethod
-    def type_attributes() -> [str]:
+    def type_attributes() -> list[str]:
         return SpTypeMixin.type_attributes() + [
             "e_storage",
             "e_cons",
         ]
```

### Comparing `psdm-analysis-0.1.2.dev3/psdm_analysis/models/input/participant/fixed_feed_in.py` & `psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/fixed_feed_in.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev3/psdm_analysis/models/input/participant/hp.py` & `psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/hp.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,13 +16,13 @@
         return self.data["thermal_bus"]
 
     @property
     def p_thermal(self):
         return self.data["p_thermal"]
 
     @staticmethod
-    def entity_attributes() -> [str]:
+    def entity_attributes() -> list[str]:
         return ["thermal_bus"]
 
     @staticmethod
-    def type_attributes() -> [str]:
+    def type_attributes() -> list[str]:
         return SpTypeMixin.type_attributes() + ["p_thermal"]
```

### Comparing `psdm-analysis-0.1.2.dev3/psdm_analysis/models/input/participant/load.py` & `psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/load.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev3/psdm_analysis/models/input/participant/participant.py` & `psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/participant.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev3/psdm_analysis/models/input/participant/pv.py` & `psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/pv.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev3/psdm_analysis/models/input/participant/storage.py` & `psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pandas import Series
 
-from psdm_analysis.models.input.container.mixins import HasTypeMixin, SpTypeMixin
+from psdm_analysis.models.input.container.mixins import SpTypeMixin
 from psdm_analysis.models.input.enums import SystemParticipantsEnum
 from psdm_analysis.models.input.participant.participant import (
     SystemParticipantsWithCapacity,
 )
 
 
 class Storages(SystemParticipantsWithCapacity, SpTypeMixin):
```

### Comparing `psdm-analysis-0.1.2.dev3/psdm_analysis/models/input/participant/wec.py` & `psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/wec.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from dataclasses import dataclass
-from typing import List
 
-from psdm_analysis.models.input.container.mixins import HasTypeMixin, SpTypeMixin
+from psdm_analysis.models.input.container.mixins import SpTypeMixin
 from psdm_analysis.models.input.enums import SystemParticipantsEnum
 from psdm_analysis.models.input.participant.participant import SystemParticipants
 
 
 @dataclass(frozen=True)
 class WindEnergyConverters(SpTypeMixin, SystemParticipants):
     @staticmethod
@@ -25,18 +24,18 @@
         return self.data["rotor_area"]
 
     @property
     def hub_height(self):
         return self.data["hub_height"]
 
     @staticmethod
-    def entity_attributes() -> [str]:
+    def entity_attributes() -> list[str]:
         return ["market_reaction"]
 
     @staticmethod
-    def type_attributes() -> [str]:
+    def type_attributes() -> list[str]:
         return SpTypeMixin.type_attributes() + [
             "cp_characteristic",
             "eta_conv",
             "rotor_area",
             "hub_height",
         ]
```

### Comparing `psdm-analysis-0.1.2.dev3/psdm_analysis/models/primary_data.py` & `psdm-analysis-0.1.2.dev4/psdm_analysis/models/primary_data.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev3/psdm_analysis/models/result/flex_option.py` & `psdm-analysis-0.1.2.dev4/psdm_analysis/models/result/flex_option.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev3/psdm_analysis/models/result/grid/enhanced_node.py` & `psdm-analysis-0.1.2.dev4/psdm_analysis/models/result/grid/enhanced_node.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,17 @@
     def from_node_result(
         cls, node_res: NodeResult, p: Series, q: Series = None
     ) -> "EnhancedNodeResult":
         return cls(
             RawGridElementsEnum.NODE,
             node_res.name,
             node_res.input_model,
-            pd.concat([node_res.data, p.rename("p"), q.rename("q")], axis=1),
+            pd.concat(
+                [node_res.data, p.rename("p"), q.rename("q")], axis=1
+            ).sort_index(),
         )
 
     @property
     def p(self) -> Series:
         return self.data["p"]
 
     @property
```

### Comparing `psdm-analysis-0.1.2.dev3/psdm_analysis/models/result/grid/node.py` & `psdm-analysis-0.1.2.dev4/psdm_analysis/models/result/grid/node.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 from dataclasses import dataclass
 from datetime import datetime
-from typing import List
+from typing import List, Optional
 
 import pandas as pd
 from pandas import DataFrame, Series
 
 from psdm_analysis.io.utils import (
     check_filter,
     csv_to_grpd_df,
@@ -61,16 +61,16 @@
 
     @classmethod
     def from_csv(
         cls,
         simulation_data_path: str,
         delimiter: str,
         simulation_end: datetime,
-        filter_start: datetime = None,
-        filter_end: datetime = None,
+        filter_start: Optional[datetime] = None,
+        filter_end: Optional[datetime] = None,
     ):
         check_filter(filter_start, filter_end)
         file_path = get_file_path(simulation_data_path, "node_res.csv")
         if file_path.exists():
             node_data = csv_to_grpd_df("node_res.csv", simulation_data_path, delimiter)
             if not node_data:
                 return cls.create_empty(RawGridElementsEnum.NODE)
```

### Comparing `psdm-analysis-0.1.2.dev3/psdm_analysis/models/result/participant/dict.py` & `psdm-analysis-0.1.2.dev4/psdm_analysis/models/result/participant/dict.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev3/psdm_analysis/models/result/participant/flex_options.py` & `psdm-analysis-0.1.2.dev4/psdm_analysis/models/result/participant/flex_options.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev3/psdm_analysis/models/result/participant/participant.py` & `psdm-analysis-0.1.2.dev4/psdm_analysis/models/result/participant/participant.py`

 * *Files 5% similar despite different names*

```diff
@@ -100,31 +100,35 @@
             {uuid: self.entities[uuid] for uuid in self.entities.keys() & uuids},
         )
 
     @property
     def p(self):
         if not self.entities.values():
             return None
-        return pd.DataFrame(
-            {p_uuid: res.p for p_uuid, res in self.entities.items()}
-        ).fillna(method="ffill")
+        return (
+            pd.DataFrame({p_uuid: res.p for p_uuid, res in self.entities.items()})
+            .fillna(method="ffill")
+            .sort_index()
+        )
 
     def sum(self) -> PQResult:
         return PQResult.sum(list(self.entities.values()))
 
     def p_sum(self) -> Series:
         if not self.entities:
             return Series(dtype=float)
         return self.p.fillna(method="ffill").sum(axis=1).rename("p_sum")
 
     @property
     def q(self):
-        return pd.DataFrame(
-            {p_uuid: res.q for p_uuid, res in self.entities.items()}
-        ).fillna(method="ffill")
+        return (
+            pd.DataFrame({p_uuid: res.q for p_uuid, res in self.entities.items()})
+            .fillna(method="ffill")
+            .sort_index()
+        )
 
     def q_sum(self):
         if not self.entities:
             return Series(dtype=float)
         return self.q.fillna(method="ffill").sum(axis=1).rename("q_sum")
 
     def energy(self):
```

### Comparing `psdm-analysis-0.1.2.dev3/psdm_analysis/models/result/participant/participants_res_container.py` & `psdm-analysis-0.1.2.dev4/psdm_analysis/models/result/participant/participants_res_container.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import concurrent.futures
 from dataclasses import dataclass
 from datetime import datetime
 from functools import partial
+from typing import Optional
 
 import pandas as pd
 from pandas import DataFrame, Series
 
 from psdm_analysis.io.utils import check_filter
 from psdm_analysis.models.input.enums import SystemParticipantsEnum
 from psdm_analysis.models.result.participant.flex_options import FlexOptionsResult
@@ -44,16 +45,16 @@
     @classmethod
     def from_csv(
         cls,
         simulation_data_path: str,
         delimiter: str,
         simulation_end: datetime,
         from_agg_results: bool = False,
-        filter_start: datetime = None,
-        filter_end: datetime = None,
+        filter_start: Optional[datetime] = None,
+        filter_end: Optional[datetime] = None,
     ):
         check_filter(filter_start, filter_end)
         with concurrent.futures.ProcessPoolExecutor() as executor:
             # warning: Breakpoints in the underlying method might not work when started from ipynb
             pa_from_csv_for_participant = partial(
                 ParticipantsResultContainer.from_csv_for_participant,
                 simulation_data_path,
@@ -120,15 +121,15 @@
                 delimiter,
                 simulation_end,
                 from_agg_results,
             )
 
     def to_list(
         self, include_em: bool = True, include_flex=True, include_empty=True
-    ) -> [ParticipantsResult]:
+    ) -> list[ParticipantsResult]:
         optional = []
         if include_em:
             optional.append(self.ems)
         if include_flex:
             optional.append(self.flex)
         required_participants = [
             self.loads,
@@ -216,22 +217,22 @@
         self, include_empty: bool = True
     ) -> dict[SystemParticipantsEnum, ParticipantsResult]:
         if include_empty:
             return {res.entity_type: res for res in self.to_list()}
         else:
             return {res.entity_type: res for res in self.to_list() if res.entities}
 
-    def energies(self) -> {SystemParticipantsEnum, float}:
+    def energies(self) -> dict[SystemParticipantsEnum, float]:
         return {
             sp_type: res.energy()
             for sp_type, res in self.to_dict(include_empty=False).items()
             if sp_type != SystemParticipantsEnum.FLEX_OPTIONS
         }
 
-    def load_and_generation_energies(self) -> {SystemParticipantsEnum, float}:
+    def load_and_generation_energies(self) -> dict[SystemParticipantsEnum, float]:
         return {
             sp_type: res.load_and_generation()
             for sp_type, res in self.to_dict(include_empty=False).items()
         }
 
     def sum(self) -> PQResult:
         participant_res = []
```

### Comparing `psdm-analysis-0.1.2.dev3/psdm_analysis/models/result/power.py` & `psdm-analysis-0.1.2.dev4/psdm_analysis/models/result/power.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import dataclasses
 import os
 import re
 from dataclasses import dataclass
 from functools import reduce
-from typing import List, Union
+from typing import List, Tuple, Union
 
 import pandas as pd
 from pandas import Series
 
 from psdm_analysis.io.utils import get_absolute_path
 from psdm_analysis.models.entity import ResultEntities
 from psdm_analysis.models.input.enums import EntitiesEnum, SystemParticipantsEnum
@@ -97,15 +97,15 @@
         if len(results) == 1:
             return results[0]
         return reduce(lambda a, b: a + b, results)
 
     def energy(self) -> float:
         return duration_weighted_sum(self.p)
 
-    def load_and_generation(self) -> (float, float):
+    def load_and_generation(self) -> Tuple[float, float]:
         return load_and_generation(self.p)
 
     def divide_load_generation(self):
         load, generation = divide_positive_negative(self.data)
         return dataclasses.replace(self, data=load), dataclasses.replace(
             self, data=generation
         )
@@ -149,15 +149,17 @@
             "PQResult - Sum",
             "PQResult - Sum",
             summed_data,
         )
 
     @staticmethod
     # todo: find a way for parallel calculation
-    def sum_with_soc(results: [(float, "PQWithSocResult")]) -> "PQWithSocResult":
+    def sum_with_soc(
+        results: list[Tuple[float, "PQWithSocResult"]]
+    ) -> "PQWithSocResult":
         if len(results) == 0:
             return PQWithSocResult.create_empty(
                 SystemParticipantsEnum.PARTICIPANTS_SUM, "", ""
             )
         if len(results) == 1:
             return results[0][1]
         this_capacity, agg = results[0]
```

### Comparing `psdm-analysis-0.1.2.dev3/psdm_analysis/models/result/res_container.py` & `psdm-analysis-0.1.2.dev4/psdm_analysis/models/result/res_container.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from dataclasses import dataclass
 from datetime import datetime
-from typing import Set
+from typing import Optional, Set
 
 from psdm_analysis.io.utils import check_filter
 from psdm_analysis.models.result.grid.node import NodesResult
 from psdm_analysis.models.result.participant.participants_res_container import (
     ParticipantsResultContainer,
 )
 
@@ -16,38 +16,42 @@
     participants: ParticipantsResultContainer
 
     def __len__(self):
         return len(self.nodes) + len(self.participants)
 
     # todo: implement slicing
     def __getitem__(self, slice_val):
-        pass
+        raise NotImplementedError
 
     @classmethod
     def from_csv(
         cls,
         name: str,
         simulation_data_path: str,
         delimiter: str,
-        simulation_end: datetime = None,
+        simulation_end: Optional[datetime] = None,
         from_agg_results: bool = True,
-        filter_start: datetime = None,
-        filter_end: datetime = None,
+        filter_start: Optional[datetime] = None,
+        filter_end: Optional[datetime] = None,
     ):
         check_filter(filter_start, filter_end)
         # todo: load async
         nodes = NodesResult.from_csv(
             simulation_data_path,
             delimiter,
             simulation_end,
             filter_start=filter_start,
             filter_end=filter_end,
         )
 
         if simulation_end is None:
+            if len(nodes.entities) == 0:
+                raise ValueError(
+                    "Can't determine simulation end time. No node results to base it on."
+                )
             some_node_res = next(iter(nodes.entities.values()))
             simulation_end = some_node_res.data.index.max()
 
         participants = ParticipantsResultContainer.from_csv(
             simulation_data_path,
             delimiter,
             simulation_end,
```

### Comparing `psdm-analysis-0.1.2.dev3/psdm_analysis/plots/results/bar_plot.py` & `psdm-analysis-0.1.2.dev4/psdm_analysis/plots/results/bar_plot.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev3/psdm_analysis/plots/results/flex_plot.py` & `psdm-analysis-0.1.2.dev4/psdm_analysis/plots/results/flex_plot.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev3/psdm_analysis/plots/results/line_plot.py` & `psdm-analysis-0.1.2.dev4/psdm_analysis/plots/results/line_plot.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev3/psdm_analysis/plots/results/nodes.py` & `psdm-analysis-0.1.2.dev4/psdm_analysis/plots/results/nodes.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev3/psdm_analysis/plots/results/power_plot.py` & `psdm-analysis-0.1.2.dev4/psdm_analysis/plots/results/power_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,18 +213,18 @@
             for pq_result in pq_results
         ]
     legend_with_distinct_labels(ax)
 
 
 def ax_plot_stacked_pq(
     ax: Axes,
-    results: [PQResult],
+    results: list[PQResult],
     resolution: str,
     hourly_mean: bool = False,
-    plot_kwargs: [dict] = None,
+    plot_kwargs: list[dict] = None,
 ):
     residual_load, residual_generation = results[0].divide_load_generation()
 
     plot_partial = partial(
         ax_plot_active_power,
         ax=ax,
         resolution=resolution,
```

### Comparing `psdm-analysis-0.1.2.dev3/psdm_analysis/plots/utils.py` & `psdm-analysis-0.1.2.dev4/psdm_analysis/plots/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,16 +34,16 @@
 UNKNOWN_COLOR = GREY
 FLEX_MAX = BLUE
 FLEX_MIN = GREEN
 FLEX_REF = YELLOW
 
 
 def set_style(style: str = "whitegrid", context: str = "notebook"):
-    sns.set_style("whitegrid")
-    sns.set_context("notebook")
+    sns.set_style(style)
+    sns.set_context(context)
 
 
 def get_label_and_color(sp_type: EntitiesEnum):
     if sp_type == SystemParticipantsEnum.LOAD:
         return "Load", LOAD_COLOR
     elif sp_type == SystemParticipantsEnum.PHOTOVOLTAIC_POWER_PLANT:
         return "PV", PV_COLOR
```

### Comparing `psdm-analysis-0.1.2.dev3/psdm_analysis/processing/dataframe.py` & `psdm-analysis-0.1.2.dev4/psdm_analysis/processing/dataframe.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     positive = df.copy()
     positive[positive < 0] = 0
     negative = df.copy()
     negative[negative > 0] = 0
     return positive, negative
 
 
-def join_dataframes(dfs: [DataFrame]):
+def join_dataframes(dfs: list[DataFrame]):
     return pd.concat(dfs)
 
 
 def filter_data_for_time_interval(
     data: DataFrame, start: datetime, end: datetime
 ) -> DataFrame:
     if data.empty:
```

### Comparing `psdm-analysis-0.1.2.dev3/psdm_analysis/processing/series.py` & `psdm-analysis-0.1.2.dev4/psdm_analysis/processing/series.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,15 @@
+from typing import Tuple
+
 import pandas as pd
 from pandas import DataFrame, Series
 
 
 def duration_weighted_series(series: Series):
+    series.sort_index(inplace=True)
     values = series[:-1].reset_index(drop=True)
     time = (
         (series.index[1::] - series.index[:-1])
         .to_series()
         .apply(lambda x: x.total_seconds() / 3600)
         .reset_index(drop=True)
     )
@@ -29,27 +32,27 @@
         .join(that.rename("other"), how="outer")
         .fillna(method="ffill")
         .sum(axis=1)
         .rename(name)
     )
 
 
-def join_series(series: [Series]) -> DataFrame:
+def join_series(series: list[Series]) -> DataFrame:
     first_series = series[0]
     df = first_series.rename(first_series.name).to_frame()
     for series in series[1:]:
         df = df.join(series.rename(series.name), how="outer").fillna(method="ffill")
     return df
 
 
 def hourly_mean_resample(series: Series) -> Series:
     return series.resample("60s").ffill().resample("1h").mean()
 
 
-def load_and_generation(p_ts: Series) -> (float, float):
+def load_and_generation(p_ts: Series) -> Tuple[float, float]:
     weighted_series = duration_weighted_series(p_ts)
     load_filter = weighted_series["values"] > 0
     weighted_load = weighted_series[load_filter]
     weighted_generation = weighted_series[~load_filter]
     return (
         weighted_series_sum(weighted_load),
         weighted_series_sum(weighted_generation),
```

### Comparing `psdm-analysis-0.1.2.dev3/pyproject.toml` & `psdm-analysis-0.1.2.dev4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "psdm-analysis"
-version = "0.1.2.dev3"
+version = "0.1.2.dev4"
 description = ""
 authors = ["Thomas Oberliessen <thomas.oberliessen@googlemail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">3.8.1, <3.12"
-pandas = "^1.4.1"
+python = ">3.10, <3.12"
+pandas = "2.0.0"
 jupyter = "^1.0.0"
 matplotlib = "^3.6.0"
 seaborn = "^0.12.1"
 plotly = "^5.6.0"
 requests = "^2.27.1"
 numpy = "^1.24.1"
 scipy = "^1.10.0"
+pyarrow = "^11.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 flake8 = "^6.0.0"
 flake8-black = "^0.3.6"
 flake8-isort = "^6.0.0"
 pre-commit = "^2.21.0"
```

### Comparing `psdm-analysis-0.1.2.dev3/setup.py` & `psdm-analysis-0.1.2.dev4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,31 +20,32 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['jupyter>=1.0.0,<2.0.0',
  'matplotlib>=3.6.0,<4.0.0',
  'numpy>=1.24.1,<2.0.0',
- 'pandas>=1.4.1,<2.0.0',
+ 'pandas==2.0.0',
  'plotly>=5.6.0,<6.0.0',
+ 'pyarrow>=11.0.0,<12.0.0',
  'requests>=2.27.1,<3.0.0',
  'scipy>=1.10.0,<2.0.0',
  'seaborn>=0.12.1,<0.13.0']
 
 setup_kwargs = {
     'name': 'psdm-analysis',
-    'version': '0.1.2.dev3',
+    'version': '0.1.2.dev4',
     'description': '',
     'long_description': '# psdm-analysis\n\nThe psdm-analysis tool is meant to parse the [Power System Data Model (PSDM)](https://github.com/ie3-institute/PowerSystemDataModel) as well as provide calculation and plotting utilities to analyze the respective data.\n\nIt is currently under development and therefore highly unstable. So if you want to use it, expect it to change quite frequently for now.',
     'author': 'Thomas Oberliessen',
     'author_email': 'thomas.oberliessen@googlemail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>3.8.1,<3.12',
+    'python_requires': '>3.10,<3.12',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `psdm-analysis-0.1.2.dev3/PKG-INFO` & `psdm-analysis-0.1.2.dev4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: psdm-analysis
-Version: 0.1.2.dev3
+Version: 0.1.2.dev4
 Summary: 
 Author: Thomas Oberliessen
 Author-email: thomas.oberliessen@googlemail.com
-Requires-Python: >3.8.1,<3.12
+Requires-Python: >3.10,<3.12
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: jupyter (>=1.0.0,<2.0.0)
 Requires-Dist: matplotlib (>=3.6.0,<4.0.0)
 Requires-Dist: numpy (>=1.24.1,<2.0.0)
-Requires-Dist: pandas (>=1.4.1,<2.0.0)
+Requires-Dist: pandas (==2.0.0)
 Requires-Dist: plotly (>=5.6.0,<6.0.0)
+Requires-Dist: pyarrow (>=11.0.0,<12.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Requires-Dist: scipy (>=1.10.0,<2.0.0)
 Requires-Dist: seaborn (>=0.12.1,<0.13.0)
 Description-Content-Type: text/markdown
 
 # psdm-analysis
```


# Comparing `tmp/dramkit-0.5.28.tar.gz` & `tmp/dramkit-0.5.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dramkit-0.5.28.tar", last modified: Fri Mar 31 14:20:40 2023, max compression
+gzip compressed data, was "dramkit-0.5.29.tar", last modified: Wed Apr 19 02:58:09 2023, max compression
```

## Comparing `dramkit-0.5.28.tar` & `dramkit-0.5.29.tar`

### file list

```diff
@@ -1,181 +1,187 @@
-drwxrwxrwx   0        0        0        0 2023-03-31 14:20:40.526026 dramkit-0.5.28/
--rw-rw-rw-   0        0        0     1072 2023-02-25 10:45:19.000000 dramkit-0.5.28/LICENSE
--rw-rw-rw-   0        0        0     1095 2023-03-31 14:20:40.525026 dramkit-0.5.28/PKG-INFO
--rw-rw-rw-   0        0        0      795 2022-05-06 14:18:52.000000 dramkit-0.5.28/README.md
-drwxrwxrwx   0        0        0        0 2023-03-31 14:20:39.913027 dramkit-0.5.28/dramkit/
--rw-rw-rw-   0        0        0     1000 2023-03-29 07:47:32.000000 dramkit-0.5.28/dramkit/__init__.py
--rw-rw-rw-   0        0        0      662 2023-03-31 14:19:56.000000 dramkit-0.5.28/dramkit/_pkg_info.py
-drwxrwxrwx   0        0        0        0 2023-03-31 14:20:40.111045 dramkit-0.5.28/dramkit/_tmp/
--rw-rw-rw-   0        0        0     6600 2021-12-24 09:25:22.000000 dramkit-0.5.28/dramkit/_tmp/CRR.py
--rw-rw-rw-   0        0        0     1844 2022-08-02 09:50:33.000000 dramkit-0.5.28/dramkit/_tmp/CtrlPreTS.py
--rw-rw-rw-   0        0        0      515 2022-01-09 09:11:34.000000 dramkit-0.5.28/dramkit/_tmp/NPairSum.py
--rw-rw-rw-   0        0        0     3672 2021-12-24 09:25:22.000000 dramkit-0.5.28/dramkit/_tmp/PIDtest.py
--rw-rw-rw-   0        0        0     2316 2021-12-24 09:25:22.000000 dramkit-0.5.28/dramkit/_tmp/PIDtest2.py
--rw-rw-rw-   0        0        0     6152 2021-12-24 09:25:22.000000 dramkit-0.5.28/dramkit/_tmp/VMD.py
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.28/dramkit/_tmp/__init__.py
--rw-rw-rw-   0        0        0     2182 2021-12-24 09:25:22.000000 dramkit-0.5.28/dramkit/_tmp/cca_test.py
--rw-rw-rw-   0        0        0     1768 2021-12-24 09:25:22.000000 dramkit-0.5.28/dramkit/_tmp/dtw_test.py
--rw-rw-rw-   0        0        0    10656 2021-12-24 09:25:22.000000 dramkit-0.5.28/dramkit/_tmp/explore.py
--rw-rw-rw-   0        0        0     2857 2021-12-24 09:25:22.000000 dramkit-0.5.28/dramkit/_tmp/gini.py
--rw-rw-rw-   0        0        0      899 2021-12-24 09:25:22.000000 dramkit-0.5.28/dramkit/_tmp/merge_sort.py
--rw-rw-rw-   0        0        0      910 2021-12-24 09:25:22.000000 dramkit-0.5.28/dramkit/_tmp/mouse_move.py
--rw-rw-rw-   0        0        0     1600 2021-12-24 09:25:22.000000 dramkit-0.5.28/dramkit/_tmp/mpc_test1.py
--rw-rw-rw-   0        0        0     7521 2021-12-24 09:25:22.000000 dramkit-0.5.28/dramkit/_tmp/options_Implied_volatility.py
--rw-rw-rw-   0        0        0      501 2021-12-24 09:25:22.000000 dramkit-0.5.28/dramkit/_tmp/pf_test.py
--rw-rw-rw-   0        0        0     4142 2021-12-24 09:25:22.000000 dramkit-0.5.28/dramkit/_tmp/plot_test.py
--rw-rw-rw-   0        0        0     1567 2022-05-06 11:02:39.000000 dramkit-0.5.28/dramkit/_tmp/plot_test2.py
--rw-rw-rw-   0        0        0     2618 2022-07-06 06:24:15.000000 dramkit-0.5.28/dramkit/_tmp/simple_smooth.py
--rw-rw-rw-   0        0        0     1057 2023-03-17 03:20:46.000000 dramkit-0.5.28/dramkit/_tmp/test_async_washs.py
--rw-rw-rw-   0        0        0      747 2021-12-24 09:25:22.000000 dramkit-0.5.28/dramkit/_tmp/test_backtrader.py
--rw-rw-rw-   0        0        0     1917 2023-02-16 09:04:46.000000 dramkit-0.5.28/dramkit/_tmp/test_chatgpt_v1.py
--rw-rw-rw-   0        0        0      657 2021-12-24 09:25:22.000000 dramkit-0.5.28/dramkit/_tmp/test_code.py
--rw-rw-rw-   0        0        0     3629 2022-04-13 14:32:40.000000 dramkit-0.5.28/dramkit/_tmp/test_find_peaks.py
--rw-rw-rw-   0        0        0      585 2023-01-29 09:46:43.000000 dramkit-0.5.28/dramkit/_tmp/test_get_var_name.py
--rw-rw-rw-   0        0        0     1263 2022-06-22 06:15:28.000000 dramkit-0.5.28/dramkit/_tmp/test_grading.py
--rw-rw-rw-   0        0        0     2193 2021-12-24 09:25:22.000000 dramkit-0.5.28/dramkit/_tmp/test_lr.py
--rw-rw-rw-   0        0        0     1154 2023-01-13 09:20:58.000000 dramkit-0.5.28/dramkit/_tmp/test_maxsort.py
--rw-rw-rw-   0        0        0      318 2022-01-26 13:43:15.000000 dramkit-0.5.28/dramkit/_tmp/test_ocr.py
--rw-rw-rw-   0        0        0     1791 2022-04-22 14:45:04.000000 dramkit-0.5.28/dramkit/_tmp/test_pywechat.py
--rw-rw-rw-   0        0        0     3046 2022-09-12 10:04:35.000000 dramkit-0.5.28/dramkit/_tmp/test_tree.py
--rw-rw-rw-   0        0        0     1154 2023-03-08 08:28:22.000000 dramkit-0.5.28/dramkit/_tmp/test_tree2.py
--rw-rw-rw-   0        0        0     1590 2022-09-06 13:36:18.000000 dramkit-0.5.28/dramkit/_tmp/test_wechat_work.py
--rw-rw-rw-   0        0        0     4876 2021-12-24 09:25:22.000000 dramkit-0.5.28/dramkit/_tmp/tfDNNCls_test.py
--rw-rw-rw-   0        0        0     2832 2021-12-24 09:25:22.000000 dramkit-0.5.28/dramkit/_tmp/tmp.py
--rw-rw-rw-   0        0        0     1323 2023-03-28 09:21:10.000000 dramkit-0.5.28/dramkit/_tmp/tmp_args.py
--rw-rw-rw-   0        0        0     5409 2021-12-24 09:25:22.000000 dramkit-0.5.28/dramkit/_tmp/transformer_pytorch.py
--rw-rw-rw-   0        0        0     4675 2022-07-06 06:13:38.000000 dramkit-0.5.28/dramkit/_tmp/utils_SignalDec.py
--rw-rw-rw-   0        0        0    10430 2022-05-06 10:45:29.000000 dramkit-0.5.28/dramkit/_tmp/utils_TimeSeries.py
--rw-rw-rw-   0        0        0     3190 2022-05-06 10:38:49.000000 dramkit-0.5.28/dramkit/_tmp/utils_lottery.py
--rw-rw-rw-   0        0        0     3295 2021-12-24 09:25:22.000000 dramkit-0.5.28/dramkit/_tmp/utils_rl.py
--rw-rw-rw-   0        0        0     2178 2021-12-24 09:25:22.000000 dramkit-0.5.28/dramkit/_tmp/utils_rl2.py
--rw-rw-rw-   0        0        0     4310 2021-12-24 09:25:22.000000 dramkit-0.5.28/dramkit/_tmp/utils_rl3.py
--rw-rw-rw-   0        0        0     4703 2021-12-24 09:25:22.000000 dramkit-0.5.28/dramkit/_tmp/utils_rl4.py
--rw-rw-rw-   0        0        0    10517 2021-12-24 09:25:22.000000 dramkit-0.5.28/dramkit/_tmp/utils_rl5.py
--rw-rw-rw-   0        0        0    10095 2021-12-24 09:25:22.000000 dramkit-0.5.28/dramkit/_tmp/utils_rl6.py
--rw-rw-rw-   0        0        0     5426 2021-12-24 09:25:22.000000 dramkit-0.5.28/dramkit/_tmp/utils_rl7.py
--rw-rw-rw-   0        0        0     2959 2021-12-24 09:25:22.000000 dramkit-0.5.28/dramkit/_tmp/utils_sem.py
-drwxrwxrwx   0        0        0        0 2023-03-31 14:20:40.126027 dramkit-0.5.28/dramkit/backpacks/
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.28/dramkit/backpacks/__init__.py
--rw-rw-rw-   0        0        0     7101 2022-05-01 13:07:37.000000 dramkit-0.5.28/dramkit/backpacks/backpack01_float_dy.py
--rw-rw-rw-   0        0        0     6771 2022-05-01 13:50:22.000000 dramkit-0.5.28/dramkit/backpacks/backpack01_int_dy.py
-drwxrwxrwx   0        0        0        0 2023-03-31 14:20:40.183026 dramkit-0.5.28/dramkit/chncal/
--rw-rw-rw-   0        0        0      730 2023-03-29 14:37:50.000000 dramkit-0.5.28/dramkit/chncal/__init__.py
--rw-rw-rw-   0        0        0    21004 2023-03-29 14:37:50.000000 dramkit-0.5.28/dramkit/chncal/apis.py
--rw-rw-rw-   0        0        0    69806 2023-03-29 14:37:50.000000 dramkit-0.5.28/dramkit/chncal/constants.py
--rw-rw-rw-   0        0        0     8480 2023-03-29 14:37:50.000000 dramkit-0.5.28/dramkit/chncal/constants_fate.py
--rw-rw-rw-   0        0        0  9509384 2023-03-29 14:37:50.000000 dramkit-0.5.28/dramkit/chncal/constants_hko.py
--rw-rw-rw-   0        0        0  3940532 2023-03-29 14:37:50.000000 dramkit-0.5.28/dramkit/chncal/constants_trade_dates.py
--rw-rw-rw-   0        0        0     2501 2023-03-29 14:37:50.000000 dramkit-0.5.28/dramkit/chncal/constants_wuxing.py
--rw-rw-rw-   0        0        0     8342 2023-03-29 14:37:50.000000 dramkit-0.5.28/dramkit/chncal/constants_zodiac_marry.py
--rw-rw-rw-   0        0        0     4570 2023-03-29 14:37:50.000000 dramkit-0.5.28/dramkit/chncal/solar_terms.py
--rw-rw-rw-   0        0        0     4477 2023-03-16 01:34:08.000000 dramkit-0.5.28/dramkit/cryptotools.py
--rw-rw-rw-   0        0        0    30707 2023-02-16 08:17:46.000000 dramkit-0.5.28/dramkit/datetimetools.py
-drwxrwxrwx   0        0        0        0 2023-03-31 14:20:40.257027 dramkit-0.5.28/dramkit/datsci/
--rw-rw-rw-   0        0        0       65 2022-05-06 02:08:55.000000 dramkit-0.5.28/dramkit/datsci/__init__.py
--rw-rw-rw-   0        0        0     2865 2023-03-22 07:56:05.000000 dramkit-0.5.28/dramkit/datsci/_utils_ann.py
--rw-rw-rw-   0        0        0     2090 2022-05-05 14:04:35.000000 dramkit-0.5.28/dramkit/datsci/activate_funcs.py
--rw-rw-rw-   0        0        0    19078 2023-03-22 07:56:56.000000 dramkit-0.5.28/dramkit/datsci/ahp.py
--rw-rw-rw-   0        0        0     2992 2023-03-22 07:58:04.000000 dramkit-0.5.28/dramkit/datsci/ahp_sim_ri.py
--rw-rw-rw-   0        0        0    10071 2022-05-19 06:37:13.000000 dramkit-0.5.28/dramkit/datsci/apriori.py
--rw-rw-rw-   0        0        0     4362 2022-05-06 06:17:24.000000 dramkit-0.5.28/dramkit/datsci/curvature.py
--rw-rw-rw-   0        0        0     6966 2023-03-22 07:59:58.000000 dramkit-0.5.28/dramkit/datsci/elm_cls.py
--rw-rw-rw-   0        0        0     8216 2023-03-22 08:00:46.000000 dramkit-0.5.28/dramkit/datsci/elm_reg.py
--rw-rw-rw-   0        0        0     3697 2022-06-25 18:21:15.000000 dramkit-0.5.28/dramkit/datsci/entropy_weight.py
--rw-rw-rw-   0        0        0    50059 2023-03-22 08:02:24.000000 dramkit-0.5.28/dramkit/datsci/find_maxmin.py
--rw-rw-rw-   0        0        0     7229 2023-03-22 08:06:26.000000 dramkit-0.5.28/dramkit/datsci/freq_item_set.py
--rw-rw-rw-   0        0        0     6219 2023-03-22 07:59:12.000000 dramkit-0.5.28/dramkit/datsci/lr.py
--rw-rw-rw-   0        0        0    19065 2022-12-12 03:02:35.000000 dramkit-0.5.28/dramkit/datsci/preprocess.py
--rw-rw-rw-   0        0        0    41389 2023-03-23 13:45:46.000000 dramkit-0.5.28/dramkit/datsci/stats.py
--rw-rw-rw-   0        0        0    36092 2023-03-22 08:04:05.000000 dramkit-0.5.28/dramkit/datsci/time_series.py
--rw-rw-rw-   0        0        0     3451 2022-06-25 18:24:48.000000 dramkit-0.5.28/dramkit/datsci/topsis.py
--rw-rw-rw-   0        0        0    23324 2022-10-17 06:00:47.000000 dramkit-0.5.28/dramkit/datsci/utils_lgb.py
--rw-rw-rw-   0        0        0     6843 2022-09-09 05:44:56.000000 dramkit-0.5.28/dramkit/datsci/utils_ml.py
-drwxrwxrwx   0        0        0        0 2023-03-31 14:20:40.285030 dramkit-0.5.28/dramkit/find_addends/
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.28/dramkit/find_addends/__init__.py
--rw-rw-rw-   0        0        0     3433 2023-03-22 08:18:35.000000 dramkit-0.5.28/dramkit/find_addends/find_addends_backpack01float.py
--rw-rw-rw-   0        0        0     2149 2022-05-01 08:15:22.000000 dramkit-0.5.28/dramkit/find_addends/find_addends_backpack01int.py
--rw-rw-rw-   0        0        0    12658 2023-03-22 08:17:39.000000 dramkit-0.5.28/dramkit/find_addends/find_addends_bigfirst.py
--rw-rw-rw-   0        0        0     4500 2023-03-22 08:17:06.000000 dramkit-0.5.28/dramkit/find_addends/find_addends_recu.py
--rw-rw-rw-   0        0        0     9576 2023-03-22 08:16:00.000000 dramkit-0.5.28/dramkit/find_addends/find_addends_smlfirst.py
--rw-rw-rw-   0        0        0     3988 2022-04-30 16:29:18.000000 dramkit-0.5.28/dramkit/find_addends/find_addends_utils.py
--rw-rw-rw-   0        0        0   106664 2023-03-28 10:22:45.000000 dramkit-0.5.28/dramkit/gentools.py
--rw-rw-rw-   0        0        0      735 2022-08-04 06:40:11.000000 dramkit-0.5.28/dramkit/install_check.py
--rw-rw-rw-   0        0        0    63935 2023-03-31 06:52:14.000000 dramkit-0.5.28/dramkit/iotools.py
-drwxrwxrwx   0        0        0        0 2023-03-31 14:20:40.306029 dramkit-0.5.28/dramkit/logtools/
--rw-rw-rw-   0        0        0       25 2021-12-25 16:04:07.000000 dramkit-0.5.28/dramkit/logtools/__init__.py
--rw-rw-rw-   0        0        0     2566 2023-02-08 04:11:46.000000 dramkit-0.5.28/dramkit/logtools/logger_general.py
--rw-rw-rw-   0        0        0     3597 2023-02-07 03:04:57.000000 dramkit-0.5.28/dramkit/logtools/logger_rotating.py
--rw-rw-rw-   0        0        0     2880 2023-02-07 03:04:39.000000 dramkit-0.5.28/dramkit/logtools/logger_timedrotating.py
--rw-rw-rw-   0        0        0     4214 2023-02-28 10:31:30.000000 dramkit-0.5.28/dramkit/logtools/utils_logger.py
-drwxrwxrwx   0        0        0        0 2023-03-31 14:20:40.325026 dramkit-0.5.28/dramkit/openai/
--rw-rw-rw-   0        0        0      134 2023-03-06 15:44:45.000000 dramkit-0.5.28/dramkit/openai/__init__.py
--rw-rw-rw-   0        0        0     5619 2023-03-31 13:34:27.000000 dramkit-0.5.28/dramkit/openai/aiedu_chat.py
--rw-rw-rw-   0        0        0    14142 2023-03-31 07:06:12.000000 dramkit-0.5.28/dramkit/openai/openai_chat.py
--rw-rw-rw-   0        0        0     1497 2023-03-15 02:00:55.000000 dramkit-0.5.28/dramkit/openai/openai_chat_hs.py
-drwxrwxrwx   0        0        0        0 2023-03-31 14:20:40.376026 dramkit-0.5.28/dramkit/optimizer/
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.28/dramkit/optimizer/__init__.py
--rw-rw-rw-   0        0        0     9712 2023-03-22 08:26:32.000000 dramkit-0.5.28/dramkit/optimizer/alo.py
--rw-rw-rw-   0        0        0     3141 2022-05-02 02:31:44.000000 dramkit-0.5.28/dramkit/optimizer/base_funcs.py
--rw-rw-rw-   0        0        0     7428 2023-03-22 08:35:00.000000 dramkit-0.5.28/dramkit/optimizer/boa.py
--rw-rw-rw-   0        0        0     8863 2023-03-22 08:34:30.000000 dramkit-0.5.28/dramkit/optimizer/cs.py
--rw-rw-rw-   0        0        0    13415 2023-03-22 08:33:50.000000 dramkit-0.5.28/dramkit/optimizer/ga.py
--rw-rw-rw-   0        0        0     8701 2023-03-22 08:33:17.000000 dramkit-0.5.28/dramkit/optimizer/gwo.py
--rw-rw-rw-   0        0        0     9311 2023-03-22 08:32:10.000000 dramkit-0.5.28/dramkit/optimizer/hcpsoboa.py
--rw-rw-rw-   0        0        0     9929 2023-03-22 08:31:27.000000 dramkit-0.5.28/dramkit/optimizer/hho.py
--rw-rw-rw-   0        0        0     8817 2023-03-22 08:30:38.000000 dramkit-0.5.28/dramkit/optimizer/hpsoboa.py
--rw-rw-rw-   0        0        0     8889 2023-03-22 08:29:43.000000 dramkit-0.5.28/dramkit/optimizer/pso.py
--rw-rw-rw-   0        0        0     5222 2022-05-02 02:18:28.000000 dramkit-0.5.28/dramkit/optimizer/utils_heuristic.py
--rw-rw-rw-   0        0        0     7334 2023-03-22 08:27:35.000000 dramkit-0.5.28/dramkit/optimizer/woa.py
-drwxrwxrwx   0        0        0        0 2023-03-31 14:20:40.403027 dramkit-0.5.28/dramkit/other/
--rw-rw-rw-   0        0        0     3679 2023-03-29 08:50:48.000000 dramkit-0.5.28/dramkit/other/_Linux_notes.py
--rw-rw-rw-   0        0        0     2804 2023-03-29 05:41:02.000000 dramkit-0.5.28/dramkit/other/_Python_notes.py
--rw-rw-rw-   0        0        0       70 2023-02-07 06:10:30.000000 dramkit-0.5.28/dramkit/other/_Vim_notes.py
--rw-rw-rw-   0        0        0      164 2022-08-25 01:46:27.000000 dramkit-0.5.28/dramkit/other/__init__.py
--rw-rw-rw-   0        0        0     7988 2022-10-27 06:38:44.000000 dramkit-0.5.28/dramkit/other/langconv.py
--rw-rw-rw-   0        0        0     8353 2022-12-10 15:26:10.000000 dramkit-0.5.28/dramkit/other/othertools.py
--rw-rw-rw-   0        0        0     1804 2023-03-22 08:36:51.000000 dramkit-0.5.28/dramkit/other/replace_endblank.py
--rw-rw-rw-   0        0        0   143066 2022-08-25 01:37:20.000000 dramkit-0.5.28/dramkit/other/zh_wiki.py
-drwxrwxrwx   0        0        0        0 2023-03-31 14:20:40.426026 dramkit-0.5.28/dramkit/plottools/
--rw-rw-rw-   0        0        0      112 2022-05-04 14:50:04.000000 dramkit-0.5.28/dramkit/plottools/__init__.py
--rw-rw-rw-   0        0        0     4400 2022-01-09 07:36:22.000000 dramkit-0.5.28/dramkit/plottools/plot_barline.py
--rw-rw-rw-   0        0        0    48494 2023-03-22 08:37:45.000000 dramkit-0.5.28/dramkit/plottools/plot_common.py
--rw-rw-rw-   0        0        0     9033 2022-06-25 18:36:48.000000 dramkit-0.5.28/dramkit/plottools/plot_histdist.py
--rw-rw-rw-   0        0        0     2145 2023-03-04 13:10:35.000000 dramkit-0.5.28/dramkit/plottools/plot_scatter.py
--rw-rw-rw-   0        0        0     5120 2023-03-21 14:27:12.000000 dramkit-0.5.28/dramkit/plottools/utils_plot.py
-drwxrwxrwx   0        0        0        0 2023-03-31 14:20:40.436026 dramkit-0.5.28/dramkit/pystyles/
--rw-rw-rw-   0        0        0       25 2021-12-25 16:04:07.000000 dramkit-0.5.28/dramkit/pystyles/__init__.py
--rw-rw-rw-   0        0        0     8021 2022-04-30 13:24:37.000000 dramkit-0.5.28/dramkit/pystyles/dramkit_style.py
-drwxrwxrwx   0        0        0        0 2023-03-31 14:20:40.460026 dramkit-0.5.28/dramkit/sorts/
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.28/dramkit/sorts/__init__.py
--rw-rw-rw-   0        0        0     1302 2022-01-09 08:45:28.000000 dramkit-0.5.28/dramkit/sorts/bubble_sort.py
--rw-rw-rw-   0        0        0     1426 2022-01-09 08:51:55.000000 dramkit-0.5.28/dramkit/sorts/bucket_sort.py
--rw-rw-rw-   0        0        0     4742 2022-01-09 08:10:56.000000 dramkit-0.5.28/dramkit/sorts/insert_sort.py
--rw-rw-rw-   0        0        0     4833 2022-01-09 09:23:30.000000 dramkit-0.5.28/dramkit/sorts/insert_sort_bin.py
--rw-rw-rw-   0        0        0     1339 2022-01-09 08:55:14.000000 dramkit-0.5.28/dramkit/sorts/quick_sort.py
-drwxrwxrwx   0        0        0        0 2023-03-31 14:20:40.475028 dramkit-0.5.28/dramkit/speedup/
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.28/dramkit/speedup/__init__.py
--rw-rw-rw-   0        0        0     3607 2023-03-22 08:41:09.000000 dramkit-0.5.28/dramkit/speedup/multi_process.py
--rw-rw-rw-   0        0        0     5545 2023-03-22 08:42:20.000000 dramkit-0.5.28/dramkit/speedup/multi_thread.py
-drwxrwxrwx   0        0        0        0 2023-03-31 14:20:40.505026 dramkit-0.5.28/dramkit/sqltools/
--rw-rw-rw-   0        0        0     2495 2023-02-23 05:15:08.000000 dramkit-0.5.28/dramkit/sqltools/_Hive_notes.py
--rw-rw-rw-   0        0        0    29959 2023-02-22 23:49:38.000000 dramkit-0.5.28/dramkit/sqltools/_MySQL_notes.py
--rw-rw-rw-   0        0        0     6849 2023-03-07 09:26:53.000000 dramkit-0.5.28/dramkit/sqltools/_Oracle_notes.py
--rw-rw-rw-   0        0        0       58 2022-09-29 03:34:58.000000 dramkit-0.5.28/dramkit/sqltools/__init__.py
--rw-rw-rw-   0        0        0    19770 2023-02-15 09:03:04.000000 dramkit-0.5.28/dramkit/sqltools/cxoracle.py
--rw-rw-rw-   0        0        0    25908 2023-02-24 11:31:13.000000 dramkit-0.5.28/dramkit/sqltools/py_hive.py
--rw-rw-rw-   0        0        0    50395 2023-02-24 11:32:46.000000 dramkit-0.5.28/dramkit/sqltools/py_mysql.py
--rw-rw-rw-   0        0        0    18391 2023-03-22 02:56:24.000000 dramkit-0.5.28/dramkit/sqltools/sql_alchemy.py
-drwxrwxrwx   0        0        0        0 2023-03-31 14:20:40.514026 dramkit-0.5.28/dramkit/webtools/
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.28/dramkit/webtools/__init__.py
--rw-rw-rw-   0        0        0     5337 2022-06-25 18:37:55.000000 dramkit-0.5.28/dramkit/webtools/utils_html.py
-drwxrwxrwx   0        0        0        0 2023-03-31 14:20:40.522038 dramkit-0.5.28/dramkit/wechat/
--rw-rw-rw-   0        0        0       58 2022-09-06 14:04:57.000000 dramkit-0.5.28/dramkit/wechat/__init__.py
--rw-rw-rw-   0        0        0     7473 2022-10-28 03:03:37.000000 dramkit-0.5.28/dramkit/wechat/qywechat.py
-drwxrwxrwx   0        0        0        0 2023-03-31 14:20:39.930040 dramkit-0.5.28/dramkit.egg-info/
--rw-rw-rw-   0        0        0     1095 2023-03-31 14:20:36.000000 dramkit-0.5.28/dramkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4651 2023-03-31 14:20:38.000000 dramkit-0.5.28/dramkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-31 14:20:36.000000 dramkit-0.5.28/dramkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-03-31 14:20:36.000000 dramkit-0.5.28/dramkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-03-31 14:20:36.000000 dramkit-0.5.28/dramkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-31 14:20:40.526026 dramkit-0.5.28/setup.cfg
--rw-rw-rw-   0        0        0     1868 2023-03-29 07:39:44.000000 dramkit-0.5.28/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 02:58:09.879306 dramkit-0.5.29/
+-rw-rw-rw-   0        0        0     1072 2023-02-25 10:45:19.000000 dramkit-0.5.29/LICENSE
+-rw-rw-rw-   0        0        0     1095 2023-04-19 02:58:09.878269 dramkit-0.5.29/PKG-INFO
+-rw-rw-rw-   0        0        0      795 2022-05-06 14:18:52.000000 dramkit-0.5.29/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 02:58:09.439229 dramkit-0.5.29/dramkit/
+-rw-rw-rw-   0        0        0     1011 2023-04-12 07:16:11.000000 dramkit-0.5.29/dramkit/__init__.py
+-rw-rw-rw-   0        0        0      662 2023-04-19 02:57:32.000000 dramkit-0.5.29/dramkit/_pkg_info.py
+drwxrwxrwx   0        0        0        0 2023-04-19 02:58:09.574242 dramkit-0.5.29/dramkit/_tmp/
+-rw-rw-rw-   0        0        0     6600 2021-12-24 09:25:22.000000 dramkit-0.5.29/dramkit/_tmp/CRR.py
+-rw-rw-rw-   0        0        0     1844 2022-08-02 09:50:33.000000 dramkit-0.5.29/dramkit/_tmp/CtrlPreTS.py
+-rw-rw-rw-   0        0        0      515 2022-01-09 09:11:34.000000 dramkit-0.5.29/dramkit/_tmp/NPairSum.py
+-rw-rw-rw-   0        0        0     3672 2021-12-24 09:25:22.000000 dramkit-0.5.29/dramkit/_tmp/PIDtest.py
+-rw-rw-rw-   0        0        0     2316 2021-12-24 09:25:22.000000 dramkit-0.5.29/dramkit/_tmp/PIDtest2.py
+-rw-rw-rw-   0        0        0     6152 2021-12-24 09:25:22.000000 dramkit-0.5.29/dramkit/_tmp/VMD.py
+-rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.29/dramkit/_tmp/__init__.py
+-rw-rw-rw-   0        0        0     2182 2021-12-24 09:25:22.000000 dramkit-0.5.29/dramkit/_tmp/cca_test.py
+-rw-rw-rw-   0        0        0     1768 2021-12-24 09:25:22.000000 dramkit-0.5.29/dramkit/_tmp/dtw_test.py
+-rw-rw-rw-   0        0        0    10656 2021-12-24 09:25:22.000000 dramkit-0.5.29/dramkit/_tmp/explore.py
+-rw-rw-rw-   0        0        0     2857 2021-12-24 09:25:22.000000 dramkit-0.5.29/dramkit/_tmp/gini.py
+-rw-rw-rw-   0        0        0      899 2021-12-24 09:25:22.000000 dramkit-0.5.29/dramkit/_tmp/merge_sort.py
+-rw-rw-rw-   0        0        0      910 2021-12-24 09:25:22.000000 dramkit-0.5.29/dramkit/_tmp/mouse_move.py
+-rw-rw-rw-   0        0        0     1600 2021-12-24 09:25:22.000000 dramkit-0.5.29/dramkit/_tmp/mpc_test1.py
+-rw-rw-rw-   0        0        0     7521 2021-12-24 09:25:22.000000 dramkit-0.5.29/dramkit/_tmp/options_Implied_volatility.py
+-rw-rw-rw-   0        0        0      501 2021-12-24 09:25:22.000000 dramkit-0.5.29/dramkit/_tmp/pf_test.py
+-rw-rw-rw-   0        0        0     4142 2021-12-24 09:25:22.000000 dramkit-0.5.29/dramkit/_tmp/plot_test.py
+-rw-rw-rw-   0        0        0     1567 2022-05-06 11:02:39.000000 dramkit-0.5.29/dramkit/_tmp/plot_test2.py
+-rw-rw-rw-   0        0        0     2618 2022-07-06 06:24:15.000000 dramkit-0.5.29/dramkit/_tmp/simple_smooth.py
+-rw-rw-rw-   0        0        0     1057 2023-03-17 03:20:46.000000 dramkit-0.5.29/dramkit/_tmp/test_async_washs.py
+-rw-rw-rw-   0        0        0     1720 2023-04-03 01:16:22.000000 dramkit-0.5.29/dramkit/_tmp/test_await_timeout.py
+-rw-rw-rw-   0        0        0      747 2021-12-24 09:25:22.000000 dramkit-0.5.29/dramkit/_tmp/test_backtrader.py
+-rw-rw-rw-   0        0        0     1917 2023-02-16 09:04:46.000000 dramkit-0.5.29/dramkit/_tmp/test_chatgpt_v1.py
+-rw-rw-rw-   0        0        0      657 2021-12-24 09:25:22.000000 dramkit-0.5.29/dramkit/_tmp/test_code.py
+-rw-rw-rw-   0        0        0     3629 2022-04-13 14:32:40.000000 dramkit-0.5.29/dramkit/_tmp/test_find_peaks.py
+-rw-rw-rw-   0        0        0      585 2023-01-29 09:46:43.000000 dramkit-0.5.29/dramkit/_tmp/test_get_var_name.py
+-rw-rw-rw-   0        0        0     1263 2022-06-22 06:15:28.000000 dramkit-0.5.29/dramkit/_tmp/test_grading.py
+-rw-rw-rw-   0        0        0     2193 2021-12-24 09:25:22.000000 dramkit-0.5.29/dramkit/_tmp/test_lr.py
+-rw-rw-rw-   0        0        0     1154 2023-01-13 09:20:58.000000 dramkit-0.5.29/dramkit/_tmp/test_maxsort.py
+-rw-rw-rw-   0        0        0      466 2023-04-06 07:48:43.000000 dramkit-0.5.29/dramkit/_tmp/test_multiprocessing.py
+-rw-rw-rw-   0        0        0      318 2022-01-26 13:43:15.000000 dramkit-0.5.29/dramkit/_tmp/test_ocr.py
+-rw-rw-rw-   0        0        0     1791 2022-04-22 14:45:04.000000 dramkit-0.5.29/dramkit/_tmp/test_pywechat.py
+-rw-rw-rw-   0        0        0     3046 2022-09-12 10:04:35.000000 dramkit-0.5.29/dramkit/_tmp/test_tree.py
+-rw-rw-rw-   0        0        0     1154 2023-03-08 08:28:22.000000 dramkit-0.5.29/dramkit/_tmp/test_tree2.py
+-rw-rw-rw-   0        0        0     1590 2022-09-06 13:36:18.000000 dramkit-0.5.29/dramkit/_tmp/test_wechat_work.py
+-rw-rw-rw-   0        0        0     4876 2021-12-24 09:25:22.000000 dramkit-0.5.29/dramkit/_tmp/tfDNNCls_test.py
+-rw-rw-rw-   0        0        0     2832 2021-12-24 09:25:22.000000 dramkit-0.5.29/dramkit/_tmp/tmp.py
+-rw-rw-rw-   0        0        0     1323 2023-03-28 09:21:10.000000 dramkit-0.5.29/dramkit/_tmp/tmp_args.py
+-rw-rw-rw-   0        0        0     5409 2021-12-24 09:25:22.000000 dramkit-0.5.29/dramkit/_tmp/transformer_pytorch.py
+-rw-rw-rw-   0        0        0     4675 2022-07-06 06:13:38.000000 dramkit-0.5.29/dramkit/_tmp/utils_SignalDec.py
+-rw-rw-rw-   0        0        0    10430 2022-05-06 10:45:29.000000 dramkit-0.5.29/dramkit/_tmp/utils_TimeSeries.py
+-rw-rw-rw-   0        0        0     3190 2022-05-06 10:38:49.000000 dramkit-0.5.29/dramkit/_tmp/utils_lottery.py
+-rw-rw-rw-   0        0        0     3295 2021-12-24 09:25:22.000000 dramkit-0.5.29/dramkit/_tmp/utils_rl.py
+-rw-rw-rw-   0        0        0     2178 2021-12-24 09:25:22.000000 dramkit-0.5.29/dramkit/_tmp/utils_rl2.py
+-rw-rw-rw-   0        0        0     4310 2021-12-24 09:25:22.000000 dramkit-0.5.29/dramkit/_tmp/utils_rl3.py
+-rw-rw-rw-   0        0        0     4703 2021-12-24 09:25:22.000000 dramkit-0.5.29/dramkit/_tmp/utils_rl4.py
+-rw-rw-rw-   0        0        0    10517 2021-12-24 09:25:22.000000 dramkit-0.5.29/dramkit/_tmp/utils_rl5.py
+-rw-rw-rw-   0        0        0    10095 2021-12-24 09:25:22.000000 dramkit-0.5.29/dramkit/_tmp/utils_rl6.py
+-rw-rw-rw-   0        0        0     5426 2021-12-24 09:25:22.000000 dramkit-0.5.29/dramkit/_tmp/utils_rl7.py
+-rw-rw-rw-   0        0        0     2959 2021-12-24 09:25:22.000000 dramkit-0.5.29/dramkit/_tmp/utils_sem.py
+drwxrwxrwx   0        0        0        0 2023-04-19 02:58:09.584263 dramkit-0.5.29/dramkit/backpacks/
+-rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.29/dramkit/backpacks/__init__.py
+-rw-rw-rw-   0        0        0     7101 2022-05-01 13:07:37.000000 dramkit-0.5.29/dramkit/backpacks/backpack01_float_dy.py
+-rw-rw-rw-   0        0        0     6771 2022-05-01 13:50:22.000000 dramkit-0.5.29/dramkit/backpacks/backpack01_int_dy.py
+drwxrwxrwx   0        0        0        0 2023-04-19 02:58:09.627246 dramkit-0.5.29/dramkit/chncal/
+-rw-rw-rw-   0        0        0      730 2023-04-16 13:47:23.000000 dramkit-0.5.29/dramkit/chncal/__init__.py
+-rw-rw-rw-   0        0        0    21004 2023-04-16 13:47:23.000000 dramkit-0.5.29/dramkit/chncal/apis.py
+-rw-rw-rw-   0        0        0    69806 2023-04-16 13:47:23.000000 dramkit-0.5.29/dramkit/chncal/constants.py
+-rw-rw-rw-   0        0        0     8480 2023-04-16 13:47:23.000000 dramkit-0.5.29/dramkit/chncal/constants_fate.py
+-rw-rw-rw-   0        0        0  9509384 2023-04-16 13:47:23.000000 dramkit-0.5.29/dramkit/chncal/constants_hko.py
+-rw-rw-rw-   0        0        0  3947993 2023-04-16 13:47:23.000000 dramkit-0.5.29/dramkit/chncal/constants_trade_dates.py
+-rw-rw-rw-   0        0        0     2501 2023-04-16 13:47:23.000000 dramkit-0.5.29/dramkit/chncal/constants_wuxing.py
+-rw-rw-rw-   0        0        0     8342 2023-04-16 13:47:23.000000 dramkit-0.5.29/dramkit/chncal/constants_zodiac_marry.py
+-rw-rw-rw-   0        0        0     4570 2023-04-16 13:47:23.000000 dramkit-0.5.29/dramkit/chncal/solar_terms.py
+-rw-rw-rw-   0        0        0     4477 2023-03-16 01:34:08.000000 dramkit-0.5.29/dramkit/cryptotools.py
+-rw-rw-rw-   0        0        0    33510 2023-04-19 02:53:20.000000 dramkit-0.5.29/dramkit/datetimetools.py
+drwxrwxrwx   0        0        0        0 2023-04-19 02:58:09.676250 dramkit-0.5.29/dramkit/datsci/
+-rw-rw-rw-   0        0        0       65 2022-05-06 02:08:55.000000 dramkit-0.5.29/dramkit/datsci/__init__.py
+-rw-rw-rw-   0        0        0     2865 2023-03-22 07:56:05.000000 dramkit-0.5.29/dramkit/datsci/_utils_ann.py
+-rw-rw-rw-   0        0        0     2090 2022-05-05 14:04:35.000000 dramkit-0.5.29/dramkit/datsci/activate_funcs.py
+-rw-rw-rw-   0        0        0    19078 2023-03-22 07:56:56.000000 dramkit-0.5.29/dramkit/datsci/ahp.py
+-rw-rw-rw-   0        0        0     2992 2023-03-22 07:58:04.000000 dramkit-0.5.29/dramkit/datsci/ahp_sim_ri.py
+-rw-rw-rw-   0        0        0    10071 2022-05-19 06:37:13.000000 dramkit-0.5.29/dramkit/datsci/apriori.py
+-rw-rw-rw-   0        0        0     4362 2022-05-06 06:17:24.000000 dramkit-0.5.29/dramkit/datsci/curvature.py
+-rw-rw-rw-   0        0        0     6966 2023-03-22 07:59:58.000000 dramkit-0.5.29/dramkit/datsci/elm_cls.py
+-rw-rw-rw-   0        0        0     8216 2023-03-22 08:00:46.000000 dramkit-0.5.29/dramkit/datsci/elm_reg.py
+-rw-rw-rw-   0        0        0     3697 2022-06-25 18:21:15.000000 dramkit-0.5.29/dramkit/datsci/entropy_weight.py
+-rw-rw-rw-   0        0        0    50059 2023-03-22 08:02:24.000000 dramkit-0.5.29/dramkit/datsci/find_maxmin.py
+-rw-rw-rw-   0        0        0     7229 2023-03-22 08:06:26.000000 dramkit-0.5.29/dramkit/datsci/freq_item_set.py
+-rw-rw-rw-   0        0        0     6219 2023-03-22 07:59:12.000000 dramkit-0.5.29/dramkit/datsci/lr.py
+-rw-rw-rw-   0        0        0    19065 2022-12-12 03:02:35.000000 dramkit-0.5.29/dramkit/datsci/preprocess.py
+-rw-rw-rw-   0        0        0    41389 2023-03-23 13:45:46.000000 dramkit-0.5.29/dramkit/datsci/stats.py
+-rw-rw-rw-   0        0        0    36092 2023-03-22 08:04:05.000000 dramkit-0.5.29/dramkit/datsci/time_series.py
+-rw-rw-rw-   0        0        0     3451 2022-06-25 18:24:48.000000 dramkit-0.5.29/dramkit/datsci/topsis.py
+-rw-rw-rw-   0        0        0    23324 2022-10-17 06:00:47.000000 dramkit-0.5.29/dramkit/datsci/utils_lgb.py
+-rw-rw-rw-   0        0        0     6843 2022-09-09 05:44:56.000000 dramkit-0.5.29/dramkit/datsci/utils_ml.py
+drwxrwxrwx   0        0        0        0 2023-04-19 02:58:09.695251 dramkit-0.5.29/dramkit/find_addends/
+-rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.29/dramkit/find_addends/__init__.py
+-rw-rw-rw-   0        0        0     3433 2023-03-22 08:18:35.000000 dramkit-0.5.29/dramkit/find_addends/find_addends_backpack01float.py
+-rw-rw-rw-   0        0        0     2149 2022-05-01 08:15:22.000000 dramkit-0.5.29/dramkit/find_addends/find_addends_backpack01int.py
+-rw-rw-rw-   0        0        0    12658 2023-03-22 08:17:39.000000 dramkit-0.5.29/dramkit/find_addends/find_addends_bigfirst.py
+-rw-rw-rw-   0        0        0     4500 2023-03-22 08:17:06.000000 dramkit-0.5.29/dramkit/find_addends/find_addends_recu.py
+-rw-rw-rw-   0        0        0     9576 2023-03-22 08:16:00.000000 dramkit-0.5.29/dramkit/find_addends/find_addends_smlfirst.py
+-rw-rw-rw-   0        0        0     3988 2022-04-30 16:29:18.000000 dramkit-0.5.29/dramkit/find_addends/find_addends_utils.py
+-rw-rw-rw-   0        0        0   109159 2023-04-12 08:39:09.000000 dramkit-0.5.29/dramkit/gentools.py
+-rw-rw-rw-   0        0        0      735 2022-08-04 06:40:11.000000 dramkit-0.5.29/dramkit/install_check.py
+-rw-rw-rw-   0        0        0    67031 2023-04-12 07:15:28.000000 dramkit-0.5.29/dramkit/iotools.py
+drwxrwxrwx   0        0        0        0 2023-04-19 02:58:09.708268 dramkit-0.5.29/dramkit/logtools/
+-rw-rw-rw-   0        0        0       25 2021-12-25 16:04:07.000000 dramkit-0.5.29/dramkit/logtools/__init__.py
+-rw-rw-rw-   0        0        0     2566 2023-02-08 04:11:46.000000 dramkit-0.5.29/dramkit/logtools/logger_general.py
+-rw-rw-rw-   0        0        0     3597 2023-02-07 03:04:57.000000 dramkit-0.5.29/dramkit/logtools/logger_rotating.py
+-rw-rw-rw-   0        0        0     2880 2023-02-07 03:04:39.000000 dramkit-0.5.29/dramkit/logtools/logger_timedrotating.py
+-rw-rw-rw-   0        0        0     4214 2023-02-28 10:31:30.000000 dramkit-0.5.29/dramkit/logtools/utils_logger.py
+drwxrwxrwx   0        0        0        0 2023-04-19 02:58:09.720270 dramkit-0.5.29/dramkit/openai/
+-rw-rw-rw-   0        0        0      134 2023-03-06 15:44:45.000000 dramkit-0.5.29/dramkit/openai/__init__.py
+-rw-rw-rw-   0        0        0     5619 2023-03-31 13:34:27.000000 dramkit-0.5.29/dramkit/openai/aiedu_chat.py
+-rw-rw-rw-   0        0        0    14142 2023-03-31 07:06:12.000000 dramkit-0.5.29/dramkit/openai/openai_chat.py
+-rw-rw-rw-   0        0        0     1497 2023-03-15 02:00:55.000000 dramkit-0.5.29/dramkit/openai/openai_chat_hs.py
+drwxrwxrwx   0        0        0        0 2023-04-19 02:58:09.753257 dramkit-0.5.29/dramkit/optimizer/
+-rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.29/dramkit/optimizer/__init__.py
+-rw-rw-rw-   0        0        0     9712 2023-03-22 08:26:32.000000 dramkit-0.5.29/dramkit/optimizer/alo.py
+-rw-rw-rw-   0        0        0     3141 2022-05-02 02:31:44.000000 dramkit-0.5.29/dramkit/optimizer/base_funcs.py
+-rw-rw-rw-   0        0        0     7428 2023-03-22 08:35:00.000000 dramkit-0.5.29/dramkit/optimizer/boa.py
+-rw-rw-rw-   0        0        0     8863 2023-03-22 08:34:30.000000 dramkit-0.5.29/dramkit/optimizer/cs.py
+-rw-rw-rw-   0        0        0    13415 2023-03-22 08:33:50.000000 dramkit-0.5.29/dramkit/optimizer/ga.py
+-rw-rw-rw-   0        0        0     8701 2023-03-22 08:33:17.000000 dramkit-0.5.29/dramkit/optimizer/gwo.py
+-rw-rw-rw-   0        0        0     9311 2023-03-22 08:32:10.000000 dramkit-0.5.29/dramkit/optimizer/hcpsoboa.py
+-rw-rw-rw-   0        0        0     9929 2023-03-22 08:31:27.000000 dramkit-0.5.29/dramkit/optimizer/hho.py
+-rw-rw-rw-   0        0        0     8817 2023-03-22 08:30:38.000000 dramkit-0.5.29/dramkit/optimizer/hpsoboa.py
+-rw-rw-rw-   0        0        0     8889 2023-03-22 08:29:43.000000 dramkit-0.5.29/dramkit/optimizer/pso.py
+-rw-rw-rw-   0        0        0     5222 2022-05-02 02:18:28.000000 dramkit-0.5.29/dramkit/optimizer/utils_heuristic.py
+-rw-rw-rw-   0        0        0     7334 2023-03-22 08:27:35.000000 dramkit-0.5.29/dramkit/optimizer/woa.py
+drwxrwxrwx   0        0        0        0 2023-04-19 02:58:09.778260 dramkit-0.5.29/dramkit/other/
+-rw-rw-rw-   0        0        0     3720 2023-04-06 06:30:27.000000 dramkit-0.5.29/dramkit/other/_Linux_notes.py
+-rw-rw-rw-   0        0        0     2804 2023-03-29 05:41:02.000000 dramkit-0.5.29/dramkit/other/_Python_notes.py
+-rw-rw-rw-   0        0        0       70 2023-02-07 06:10:30.000000 dramkit-0.5.29/dramkit/other/_Vim_notes.py
+-rw-rw-rw-   0        0        0      164 2022-08-25 01:46:27.000000 dramkit-0.5.29/dramkit/other/__init__.py
+-rw-rw-rw-   0        0        0     7988 2022-10-27 06:38:44.000000 dramkit-0.5.29/dramkit/other/langconv.py
+-rw-rw-rw-   0        0        0     8353 2022-12-10 15:26:10.000000 dramkit-0.5.29/dramkit/other/othertools.py
+-rw-rw-rw-   0        0        0     1804 2023-03-22 08:36:51.000000 dramkit-0.5.29/dramkit/other/replace_endblank.py
+-rw-rw-rw-   0        0        0   143066 2022-08-25 01:37:20.000000 dramkit-0.5.29/dramkit/other/zh_wiki.py
+drwxrwxrwx   0        0        0        0 2023-04-19 02:58:09.795275 dramkit-0.5.29/dramkit/plottools/
+-rw-rw-rw-   0        0        0      112 2022-05-04 14:50:04.000000 dramkit-0.5.29/dramkit/plottools/__init__.py
+-rw-rw-rw-   0        0        0     4400 2022-01-09 07:36:22.000000 dramkit-0.5.29/dramkit/plottools/plot_barline.py
+-rw-rw-rw-   0        0        0    48494 2023-03-22 08:37:45.000000 dramkit-0.5.29/dramkit/plottools/plot_common.py
+-rw-rw-rw-   0        0        0     9033 2022-06-25 18:36:48.000000 dramkit-0.5.29/dramkit/plottools/plot_histdist.py
+-rw-rw-rw-   0        0        0     2145 2023-03-04 13:10:35.000000 dramkit-0.5.29/dramkit/plottools/plot_scatter.py
+-rw-rw-rw-   0        0        0     5120 2023-03-21 14:27:12.000000 dramkit-0.5.29/dramkit/plottools/utils_plot.py
+drwxrwxrwx   0        0        0        0 2023-04-19 02:58:09.802270 dramkit-0.5.29/dramkit/pystyles/
+-rw-rw-rw-   0        0        0       25 2021-12-25 16:04:07.000000 dramkit-0.5.29/dramkit/pystyles/__init__.py
+-rw-rw-rw-   0        0        0     8021 2022-04-30 13:24:37.000000 dramkit-0.5.29/dramkit/pystyles/dramkit_style.py
+drwxrwxrwx   0        0        0        0 2023-04-19 02:58:09.819263 dramkit-0.5.29/dramkit/sorts/
+-rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.29/dramkit/sorts/__init__.py
+-rw-rw-rw-   0        0        0     1302 2022-01-09 08:45:28.000000 dramkit-0.5.29/dramkit/sorts/bubble_sort.py
+-rw-rw-rw-   0        0        0     1426 2022-01-09 08:51:55.000000 dramkit-0.5.29/dramkit/sorts/bucket_sort.py
+-rw-rw-rw-   0        0        0     4742 2022-01-09 08:10:56.000000 dramkit-0.5.29/dramkit/sorts/insert_sort.py
+-rw-rw-rw-   0        0        0     4833 2022-01-09 09:23:30.000000 dramkit-0.5.29/dramkit/sorts/insert_sort_bin.py
+-rw-rw-rw-   0        0        0     1339 2022-01-09 08:55:14.000000 dramkit-0.5.29/dramkit/sorts/quick_sort.py
+drwxrwxrwx   0        0        0        0 2023-04-19 02:58:09.836280 dramkit-0.5.29/dramkit/speedup/
+-rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.29/dramkit/speedup/__init__.py
+-rw-rw-rw-   0        0        0     1231 2023-04-14 13:02:46.000000 dramkit-0.5.29/dramkit/speedup/_mp_test1.py
+-rw-rw-rw-   0        0        0      886 2023-04-14 13:17:44.000000 dramkit-0.5.29/dramkit/speedup/_mp_test2.py
+-rw-rw-rw-   0        0        0      684 2023-04-14 13:14:44.000000 dramkit-0.5.29/dramkit/speedup/_mp_test3.py
+-rw-rw-rw-   0        0        0     3384 2023-04-14 13:25:51.000000 dramkit-0.5.29/dramkit/speedup/iotools_tmp.py
+-rw-rw-rw-   0        0        0     3754 2023-04-12 08:17:22.000000 dramkit-0.5.29/dramkit/speedup/multi_process_concurrent.py
+-rw-rw-rw-   0        0        0     7888 2023-04-07 08:59:34.000000 dramkit-0.5.29/dramkit/speedup/multi_thread.py
+drwxrwxrwx   0        0        0        0 2023-04-19 02:58:09.858267 dramkit-0.5.29/dramkit/sqltools/
+-rw-rw-rw-   0        0        0     2495 2023-02-23 05:15:08.000000 dramkit-0.5.29/dramkit/sqltools/_Hive_notes.py
+-rw-rw-rw-   0        0        0    30416 2023-04-11 01:33:28.000000 dramkit-0.5.29/dramkit/sqltools/_MySQL_notes.py
+-rw-rw-rw-   0        0        0     6849 2023-03-07 09:26:53.000000 dramkit-0.5.29/dramkit/sqltools/_Oracle_notes.py
+-rw-rw-rw-   0        0        0       58 2022-09-29 03:34:58.000000 dramkit-0.5.29/dramkit/sqltools/__init__.py
+-rw-rw-rw-   0        0        0    19770 2023-02-15 09:03:04.000000 dramkit-0.5.29/dramkit/sqltools/cxoracle.py
+-rw-rw-rw-   0        0        0    25908 2023-02-24 11:31:13.000000 dramkit-0.5.29/dramkit/sqltools/py_hive.py
+-rw-rw-rw-   0        0        0    50395 2023-02-24 11:32:46.000000 dramkit-0.5.29/dramkit/sqltools/py_mysql.py
+-rw-rw-rw-   0        0        0    18391 2023-03-22 02:56:24.000000 dramkit-0.5.29/dramkit/sqltools/sql_alchemy.py
+drwxrwxrwx   0        0        0        0 2023-04-19 02:58:09.868282 dramkit-0.5.29/dramkit/webtools/
+-rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.29/dramkit/webtools/__init__.py
+-rw-rw-rw-   0        0        0     5337 2022-06-25 18:37:55.000000 dramkit-0.5.29/dramkit/webtools/utils_html.py
+drwxrwxrwx   0        0        0        0 2023-04-19 02:58:09.876268 dramkit-0.5.29/dramkit/wechat/
+-rw-rw-rw-   0        0        0       58 2022-09-06 14:04:57.000000 dramkit-0.5.29/dramkit/wechat/__init__.py
+-rw-rw-rw-   0        0        0     7473 2022-10-28 03:03:37.000000 dramkit-0.5.29/dramkit/wechat/qywechat.py
+drwxrwxrwx   0        0        0        0 2023-04-19 02:58:09.452231 dramkit-0.5.29/dramkit.egg-info/
+-rw-rw-rw-   0        0        0     1095 2023-04-19 02:58:05.000000 dramkit-0.5.29/dramkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4852 2023-04-19 02:58:08.000000 dramkit-0.5.29/dramkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 02:58:05.000000 dramkit-0.5.29/dramkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-04-19 02:58:05.000000 dramkit-0.5.29/dramkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-19 02:58:05.000000 dramkit-0.5.29/dramkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 02:58:09.879306 dramkit-0.5.29/setup.cfg
+-rw-rw-rw-   0        0        0     1868 2023-03-29 07:39:44.000000 dramkit-0.5.29/setup.py
```

### Comparing `dramkit-0.5.28/LICENSE` & `dramkit-0.5.29/LICENSE`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/PKG-INFO` & `dramkit-0.5.29/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dramkit
-Version: 0.5.28
+Version: 0.5.29
 Summary: DramKit is a toolbox.
 Home-page: https://github.com/Genlovy-Hoo/dramkit/
 Author: Genlovy Hoo, YueYong Hu
 Author-email: genlovhyy@163.com
 License: MIT
 Platform: any
 Description-Content-Type: text/markdown
```

### Comparing `dramkit-0.5.28/README.md` & `dramkit-0.5.29/README.md`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/__init__.py` & `dramkit-0.5.29/dramkit/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -24,9 +24,9 @@
 from . import gentools
 from . import iotools
 from . import cryptotools
 from . import datetimetools as dttools
 from .datsci import find_maxmin
 from .openai import openai_chat, aiedu_chat
 from .other import othertools
-from .speedup import multi_thread, multi_process
+from .speedup import multi_thread, multi_process_concurrent
 from .sqltools import py_mysql
```

### Comparing `dramkit-0.5.28/dramkit/_pkg_info.py` & `dramkit-0.5.29/dramkit/_pkg_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 pkg_info = {
     '__pkgname__': 'dramkit',
-    '__version__': '0.5.28',
+    '__version__': '0.5.29',
     '__license__': 'MIT',
     '__url__': 'https://github.com/Genlovy-Hoo/dramkit/',
     '__urls__':
         {'pypi': 'https://pypi.org/project/dramkit/',
          'github': 'https://github.com/Genlovy-Hoo/dramkit/',
 		 'document': 'http://www.glhyy.cn/dramkit/doc/html/index.html'
         },
```

### Comparing `dramkit-0.5.28/dramkit/_tmp/CRR.py` & `dramkit-0.5.29/dramkit/_tmp/CRR.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/_tmp/CtrlPreTS.py` & `dramkit-0.5.29/dramkit/_tmp/CtrlPreTS.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/_tmp/NPairSum.py` & `dramkit-0.5.29/dramkit/_tmp/NPairSum.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/_tmp/PIDtest.py` & `dramkit-0.5.29/dramkit/_tmp/PIDtest.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/_tmp/PIDtest2.py` & `dramkit-0.5.29/dramkit/_tmp/PIDtest2.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/_tmp/VMD.py` & `dramkit-0.5.29/dramkit/_tmp/VMD.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/_tmp/cca_test.py` & `dramkit-0.5.29/dramkit/_tmp/cca_test.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/_tmp/dtw_test.py` & `dramkit-0.5.29/dramkit/_tmp/dtw_test.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/_tmp/explore.py` & `dramkit-0.5.29/dramkit/_tmp/explore.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/_tmp/gini.py` & `dramkit-0.5.29/dramkit/_tmp/gini.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/_tmp/merge_sort.py` & `dramkit-0.5.29/dramkit/_tmp/merge_sort.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/_tmp/mouse_move.py` & `dramkit-0.5.29/dramkit/_tmp/mouse_move.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/_tmp/mpc_test1.py` & `dramkit-0.5.29/dramkit/_tmp/mpc_test1.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/_tmp/options_Implied_volatility.py` & `dramkit-0.5.29/dramkit/_tmp/options_Implied_volatility.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/_tmp/plot_test.py` & `dramkit-0.5.29/dramkit/_tmp/plot_test.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/_tmp/plot_test2.py` & `dramkit-0.5.29/dramkit/_tmp/plot_test2.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/_tmp/simple_smooth.py` & `dramkit-0.5.29/dramkit/_tmp/simple_smooth.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/_tmp/test_async_washs.py` & `dramkit-0.5.29/dramkit/_tmp/test_async_washs.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/_tmp/test_backtrader.py` & `dramkit-0.5.29/dramkit/_tmp/test_backtrader.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/_tmp/test_chatgpt_v1.py` & `dramkit-0.5.29/dramkit/_tmp/test_chatgpt_v1.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/_tmp/test_code.py` & `dramkit-0.5.29/dramkit/_tmp/test_code.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/_tmp/test_find_peaks.py` & `dramkit-0.5.29/dramkit/_tmp/test_find_peaks.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/_tmp/test_get_var_name.py` & `dramkit-0.5.29/dramkit/_tmp/test_get_var_name.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/_tmp/test_grading.py` & `dramkit-0.5.29/dramkit/_tmp/test_grading.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/_tmp/test_lr.py` & `dramkit-0.5.29/dramkit/_tmp/test_lr.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/_tmp/test_maxsort.py` & `dramkit-0.5.29/dramkit/_tmp/test_maxsort.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/_tmp/test_pywechat.py` & `dramkit-0.5.29/dramkit/_tmp/test_pywechat.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/_tmp/test_tree.py` & `dramkit-0.5.29/dramkit/_tmp/test_tree.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/_tmp/test_tree2.py` & `dramkit-0.5.29/dramkit/_tmp/test_tree2.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/_tmp/test_wechat_work.py` & `dramkit-0.5.29/dramkit/_tmp/test_wechat_work.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/_tmp/tfDNNCls_test.py` & `dramkit-0.5.29/dramkit/_tmp/tfDNNCls_test.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/_tmp/tmp.py` & `dramkit-0.5.29/dramkit/_tmp/tmp.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/_tmp/tmp_args.py` & `dramkit-0.5.29/dramkit/_tmp/tmp_args.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/_tmp/transformer_pytorch.py` & `dramkit-0.5.29/dramkit/_tmp/transformer_pytorch.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/_tmp/utils_SignalDec.py` & `dramkit-0.5.29/dramkit/_tmp/utils_SignalDec.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/_tmp/utils_TimeSeries.py` & `dramkit-0.5.29/dramkit/_tmp/utils_TimeSeries.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/_tmp/utils_lottery.py` & `dramkit-0.5.29/dramkit/_tmp/utils_lottery.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/_tmp/utils_rl.py` & `dramkit-0.5.29/dramkit/_tmp/utils_rl.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/_tmp/utils_rl2.py` & `dramkit-0.5.29/dramkit/_tmp/utils_rl2.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/_tmp/utils_rl3.py` & `dramkit-0.5.29/dramkit/_tmp/utils_rl3.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/_tmp/utils_rl4.py` & `dramkit-0.5.29/dramkit/_tmp/utils_rl4.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/_tmp/utils_rl5.py` & `dramkit-0.5.29/dramkit/_tmp/utils_rl5.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/_tmp/utils_rl6.py` & `dramkit-0.5.29/dramkit/_tmp/utils_rl6.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/_tmp/utils_rl7.py` & `dramkit-0.5.29/dramkit/_tmp/utils_rl7.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/_tmp/utils_sem.py` & `dramkit-0.5.29/dramkit/_tmp/utils_sem.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/backpacks/backpack01_float_dy.py` & `dramkit-0.5.29/dramkit/backpacks/backpack01_float_dy.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/backpacks/backpack01_int_dy.py` & `dramkit-0.5.29/dramkit/backpacks/backpack01_int_dy.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/chncal/__init__.py` & `dramkit-0.5.29/dramkit/chncal/__init__.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/chncal/apis.py` & `dramkit-0.5.29/dramkit/chncal/apis.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/chncal/constants.py` & `dramkit-0.5.29/dramkit/chncal/constants.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/chncal/constants_fate.py` & `dramkit-0.5.29/dramkit/chncal/constants_fate.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/chncal/constants_hko.py` & `dramkit-0.5.29/dramkit/chncal/constants_hko.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/chncal/constants_trade_dates.py` & `dramkit-0.5.29/dramkit/chncal/constants_trade_dates.py`

 * *Files 0% similar despite different names*

```diff
@@ -6050,14 +6050,32 @@
     ("CFFEX", datetime.date(year=2023, month=3, day=23)): 1,
     ("CFFEX", datetime.date(year=2023, month=3, day=24)): 1,
     ("CFFEX", datetime.date(year=2023, month=3, day=25)): 0,
     ("CFFEX", datetime.date(year=2023, month=3, day=26)): 0,
     ("CFFEX", datetime.date(year=2023, month=3, day=27)): 1,
     ("CFFEX", datetime.date(year=2023, month=3, day=28)): 1,
     ("CFFEX", datetime.date(year=2023, month=3, day=29)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=30)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=31)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=1)): 0,
+    ("CFFEX", datetime.date(year=2023, month=4, day=2)): 0,
+    ("CFFEX", datetime.date(year=2023, month=4, day=3)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=4)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=5)): 0,
+    ("CFFEX", datetime.date(year=2023, month=4, day=6)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=7)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=8)): 0,
+    ("CFFEX", datetime.date(year=2023, month=4, day=9)): 0,
+    ("CFFEX", datetime.date(year=2023, month=4, day=10)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=11)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=12)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=13)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=14)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=15)): 0,
+    ("CFFEX", datetime.date(year=2023, month=4, day=16)): 0,
     ("CZCE", datetime.date(year=1990, month=10, day=12)): 1,
     ("CZCE", datetime.date(year=1990, month=10, day=13)): 0,
     ("CZCE", datetime.date(year=1990, month=10, day=14)): 0,
     ("CZCE", datetime.date(year=1990, month=10, day=15)): 1,
     ("CZCE", datetime.date(year=1990, month=10, day=16)): 1,
     ("CZCE", datetime.date(year=1990, month=10, day=17)): 1,
     ("CZCE", datetime.date(year=1990, month=10, day=18)): 1,
@@ -17906,14 +17924,32 @@
     ("CZCE", datetime.date(year=2023, month=3, day=23)): 1,
     ("CZCE", datetime.date(year=2023, month=3, day=24)): 1,
     ("CZCE", datetime.date(year=2023, month=3, day=25)): 0,
     ("CZCE", datetime.date(year=2023, month=3, day=26)): 0,
     ("CZCE", datetime.date(year=2023, month=3, day=27)): 1,
     ("CZCE", datetime.date(year=2023, month=3, day=28)): 1,
     ("CZCE", datetime.date(year=2023, month=3, day=29)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=30)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=31)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=1)): 0,
+    ("CZCE", datetime.date(year=2023, month=4, day=2)): 0,
+    ("CZCE", datetime.date(year=2023, month=4, day=3)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=4)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=5)): 0,
+    ("CZCE", datetime.date(year=2023, month=4, day=6)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=7)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=8)): 0,
+    ("CZCE", datetime.date(year=2023, month=4, day=9)): 0,
+    ("CZCE", datetime.date(year=2023, month=4, day=10)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=11)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=12)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=13)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=14)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=15)): 0,
+    ("CZCE", datetime.date(year=2023, month=4, day=16)): 0,
     ("DCE", datetime.date(year=1993, month=3, day=1)): 1,
     ("DCE", datetime.date(year=1993, month=3, day=2)): 1,
     ("DCE", datetime.date(year=1993, month=3, day=3)): 1,
     ("DCE", datetime.date(year=1993, month=3, day=4)): 1,
     ("DCE", datetime.date(year=1993, month=3, day=5)): 1,
     ("DCE", datetime.date(year=1993, month=3, day=6)): 0,
     ("DCE", datetime.date(year=1993, month=3, day=7)): 0,
@@ -28891,14 +28927,32 @@
     ("DCE", datetime.date(year=2023, month=3, day=23)): 1,
     ("DCE", datetime.date(year=2023, month=3, day=24)): 1,
     ("DCE", datetime.date(year=2023, month=3, day=25)): 0,
     ("DCE", datetime.date(year=2023, month=3, day=26)): 0,
     ("DCE", datetime.date(year=2023, month=3, day=27)): 1,
     ("DCE", datetime.date(year=2023, month=3, day=28)): 1,
     ("DCE", datetime.date(year=2023, month=3, day=29)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=30)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=31)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=1)): 0,
+    ("DCE", datetime.date(year=2023, month=4, day=2)): 0,
+    ("DCE", datetime.date(year=2023, month=4, day=3)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=4)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=5)): 0,
+    ("DCE", datetime.date(year=2023, month=4, day=6)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=7)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=8)): 0,
+    ("DCE", datetime.date(year=2023, month=4, day=9)): 0,
+    ("DCE", datetime.date(year=2023, month=4, day=10)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=11)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=12)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=13)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=14)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=15)): 0,
+    ("DCE", datetime.date(year=2023, month=4, day=16)): 0,
     ("INE", datetime.date(year=2017, month=5, day=23)): 1,
     ("INE", datetime.date(year=2017, month=5, day=24)): 1,
     ("INE", datetime.date(year=2017, month=5, day=25)): 1,
     ("INE", datetime.date(year=2017, month=5, day=26)): 1,
     ("INE", datetime.date(year=2017, month=5, day=27)): 0,
     ("INE", datetime.date(year=2017, month=5, day=28)): 0,
     ("INE", datetime.date(year=2017, month=5, day=29)): 0,
@@ -31027,14 +31081,32 @@
     ("INE", datetime.date(year=2023, month=3, day=23)): 1,
     ("INE", datetime.date(year=2023, month=3, day=24)): 1,
     ("INE", datetime.date(year=2023, month=3, day=25)): 0,
     ("INE", datetime.date(year=2023, month=3, day=26)): 0,
     ("INE", datetime.date(year=2023, month=3, day=27)): 1,
     ("INE", datetime.date(year=2023, month=3, day=28)): 1,
     ("INE", datetime.date(year=2023, month=3, day=29)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=30)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=31)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=1)): 0,
+    ("INE", datetime.date(year=2023, month=4, day=2)): 0,
+    ("INE", datetime.date(year=2023, month=4, day=3)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=4)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=5)): 0,
+    ("INE", datetime.date(year=2023, month=4, day=6)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=7)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=8)): 0,
+    ("INE", datetime.date(year=2023, month=4, day=9)): 0,
+    ("INE", datetime.date(year=2023, month=4, day=10)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=11)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=12)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=13)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=14)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=15)): 0,
+    ("INE", datetime.date(year=2023, month=4, day=16)): 0,
     ("SHFE", datetime.date(year=1991, month=5, day=28)): 1,
     ("SHFE", datetime.date(year=1991, month=5, day=29)): 1,
     ("SHFE", datetime.date(year=1991, month=5, day=30)): 1,
     ("SHFE", datetime.date(year=1991, month=5, day=31)): 1,
     ("SHFE", datetime.date(year=1991, month=6, day=1)): 0,
     ("SHFE", datetime.date(year=1991, month=6, day=2)): 0,
     ("SHFE", datetime.date(year=1991, month=6, day=3)): 1,
@@ -42655,14 +42727,32 @@
     ("SHFE", datetime.date(year=2023, month=3, day=23)): 1,
     ("SHFE", datetime.date(year=2023, month=3, day=24)): 1,
     ("SHFE", datetime.date(year=2023, month=3, day=25)): 0,
     ("SHFE", datetime.date(year=2023, month=3, day=26)): 0,
     ("SHFE", datetime.date(year=2023, month=3, day=27)): 1,
     ("SHFE", datetime.date(year=2023, month=3, day=28)): 1,
     ("SHFE", datetime.date(year=2023, month=3, day=29)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=30)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=31)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=1)): 0,
+    ("SHFE", datetime.date(year=2023, month=4, day=2)): 0,
+    ("SHFE", datetime.date(year=2023, month=4, day=3)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=4)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=5)): 0,
+    ("SHFE", datetime.date(year=2023, month=4, day=6)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=7)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=8)): 0,
+    ("SHFE", datetime.date(year=2023, month=4, day=9)): 0,
+    ("SHFE", datetime.date(year=2023, month=4, day=10)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=11)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=12)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=13)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=14)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=15)): 0,
+    ("SHFE", datetime.date(year=2023, month=4, day=16)): 0,
     ("SSE", datetime.date(year=1990, month=12, day=19)): 1,
     ("SSE", datetime.date(year=1990, month=12, day=20)): 1,
     ("SSE", datetime.date(year=1990, month=12, day=21)): 1,
     ("SSE", datetime.date(year=1990, month=12, day=22)): 0,
     ("SSE", datetime.date(year=1990, month=12, day=23)): 0,
     ("SSE", datetime.date(year=1990, month=12, day=24)): 1,
     ("SSE", datetime.date(year=1990, month=12, day=25)): 1,
@@ -54444,14 +54534,32 @@
     ("SSE", datetime.date(year=2023, month=3, day=23)): 1,
     ("SSE", datetime.date(year=2023, month=3, day=24)): 1,
     ("SSE", datetime.date(year=2023, month=3, day=25)): 0,
     ("SSE", datetime.date(year=2023, month=3, day=26)): 0,
     ("SSE", datetime.date(year=2023, month=3, day=27)): 1,
     ("SSE", datetime.date(year=2023, month=3, day=28)): 1,
     ("SSE", datetime.date(year=2023, month=3, day=29)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=30)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=31)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=1)): 0,
+    ("SSE", datetime.date(year=2023, month=4, day=2)): 0,
+    ("SSE", datetime.date(year=2023, month=4, day=3)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=4)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=5)): 0,
+    ("SSE", datetime.date(year=2023, month=4, day=6)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=7)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=8)): 0,
+    ("SSE", datetime.date(year=2023, month=4, day=9)): 0,
+    ("SSE", datetime.date(year=2023, month=4, day=10)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=11)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=12)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=13)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=14)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=15)): 0,
+    ("SSE", datetime.date(year=2023, month=4, day=16)): 0,
     ("SZSE", datetime.date(year=1991, month=7, day=3)): 1,
     ("SZSE", datetime.date(year=1991, month=7, day=4)): 1,
     ("SZSE", datetime.date(year=1991, month=7, day=5)): 1,
     ("SZSE", datetime.date(year=1991, month=7, day=6)): 0,
     ("SZSE", datetime.date(year=1991, month=7, day=7)): 0,
     ("SZSE", datetime.date(year=1991, month=7, day=8)): 1,
     ("SZSE", datetime.date(year=1991, month=7, day=9)): 1,
@@ -66037,8 +66145,26 @@
     ("SZSE", datetime.date(year=2023, month=3, day=23)): 1,
     ("SZSE", datetime.date(year=2023, month=3, day=24)): 1,
     ("SZSE", datetime.date(year=2023, month=3, day=25)): 0,
     ("SZSE", datetime.date(year=2023, month=3, day=26)): 0,
     ("SZSE", datetime.date(year=2023, month=3, day=27)): 1,
     ("SZSE", datetime.date(year=2023, month=3, day=28)): 1,
     ("SZSE", datetime.date(year=2023, month=3, day=29)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=30)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=31)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=1)): 0,
+    ("SZSE", datetime.date(year=2023, month=4, day=2)): 0,
+    ("SZSE", datetime.date(year=2023, month=4, day=3)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=4)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=5)): 0,
+    ("SZSE", datetime.date(year=2023, month=4, day=6)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=7)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=8)): 0,
+    ("SZSE", datetime.date(year=2023, month=4, day=9)): 0,
+    ("SZSE", datetime.date(year=2023, month=4, day=10)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=11)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=12)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=13)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=14)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=15)): 0,
+    ("SZSE", datetime.date(year=2023, month=4, day=16)): 0,
 }
```

### Comparing `dramkit-0.5.28/dramkit/chncal/constants_wuxing.py` & `dramkit-0.5.29/dramkit/chncal/constants_wuxing.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/chncal/constants_zodiac_marry.py` & `dramkit-0.5.29/dramkit/chncal/constants_zodiac_marry.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/chncal/solar_terms.py` & `dramkit-0.5.29/dramkit/chncal/solar_terms.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/cryptotools.py` & `dramkit-0.5.29/dramkit/cryptotools.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/datetimetools.py` & `dramkit-0.5.29/dramkit/datetimetools.py`

 * *Files 5% similar despite different names*

```diff
@@ -426,14 +426,16 @@
             return pd.to_datetime(x)
 
 
 def copy_format(to_tm, from_tm):
     '''
     复制日期时间格式
     '''
+    if pd.isna(from_tm):
+        return to_tm
     input_type = type(to_tm).__name__
     types1 = ['datetime', 'date', 'Timestamp', 'struct_time']
     types2 = ['str', 'int', 'float']
     types3 = ['ndarray', 'Series', 'list', 'tuple']
     assert input_type in types1+types2+types3
     if input_type == type(from_tm).__name__ and input_type in types1:
         return to_tm
@@ -553,24 +555,108 @@
 
 def get_quarter(dt=None, joiner='Q'):
     '''获取日期所在季度'''
     if pd.isnull(dt):
         dt = datetime.datetime.now()
     t = x2datetime(dt)
     y, q = t.year, t.quarter
+    if not joiner:
+        return (y, q)
     return joiner.join([str(y), str(q)])
 
 
+def get_quarter_start_end_by_yq(y, q, joiner='-'):
+    m1 = {1: '01', 2: '04', 3: '07', 4: '10'}[q]
+    d1 = '01'
+    m2 = {1: '03', 2: '06', 3: '09', 4: '12'}[q]
+    d2 = {3: '31', 6: '30', 9: '30', 12: '31'}[int(m2)]
+    start = joiner.join([str(y), m1, d1])
+    end = joiner.join([str(y), m2, d2])
+    return start, end
+
+
+def get_quarter_start_end_by_date(date=None):
+    '''获取date日期所在季度的起始日期'''
+    y, q = get_quarter(date, None)
+    return copy_format(get_quarter_start_end_by_yq(y, q),
+                       date)
+
+
 def today_quarter(joiner='Q'):
     '''获取今日所在季度'''
     t = pd.to_datetime(datetime.datetime.now())
     y, q = t.year, t.quarter
+    if not joiner:
+        return (y, q)
     return joiner.join([str(y), str(q)])
 
 
+def get_2part_next(part1, part2, step, n=1):
+    '''
+    Example
+    -------
+    >>> get_2part_next(2023, 2, 4, 2) # 2023Q2往后推2个季度
+    (2023, 4)
+    >>> get_2part_next(2023, 4, 4, 5) # 2023Q4往后推5个季度
+    (2025, 1)
+    >>> get_2part_next(2023, 4, 12, 8) # 202304往后推8个月
+    (2023, 12)
+    >>> get_2part_next(2023, 9, 12, 10) # 202309往后推10个月
+    (2024, 7)
+    >>> get_2part_next(2023, 2, 4, -2) # 2023Q2往前推2个季度
+    (2022, 4)
+    >>> get_2part_next(2023, 4, 4, -5) # 2023Q4往前推5个季度
+    (2022, 3)
+    >>> get_2part_next(2023, 4, 12, -8) # 202304往前推8个月
+    (2022, 4)
+    >>> get_2part_next(2023, 9, 12, -10) # 202309往前推10个月
+    (2022, 11)
+    '''
+    assert all([isinstance(x, int) for x in [part1, part2, step, n]])
+    if n == 0:
+        p1new, p2new = part1, part2
+    elif n > 0:
+        p1add = n // step + int((part2 + n % step) > step)
+        p1new = part1 + p1add
+        p2new = part2 + (n % step)
+        if p2new > step:
+            p2new = p2new - step
+    else:
+        n = abs(n)
+        p1add = -(n // step) - int((part2 - n % step) <= 0)
+        p1new = part1 + p1add
+        p2new = part2 - (n % step)
+        if p2new <= 0:
+            p2new = step + p2new
+    return (p1new, p2new)
+
+
+def get_pre_quarter(date=None, n=1, joiner='Q'):
+    '''
+    | 获取date前第n个季度
+    | 如:
+    | get_pre_quarter("20230418") -> "2023Q1"
+    | get_pre_quarter("20230418", 2) -> "2022Q4"
+    | get_pre_quarter("20230418", 3) -> "2022Q3"
+    | get_pre_quarter("20230418", 4) -> "2022Q2"
+    | get_pre_quarter("20230418", 5) -> "2022Q1"
+    | get_pre_quarter("20230418", 6) -> "2021Q4"
+    | get_pre_quarter("20230418", 7) -> "2021Q3"
+    | get_pre_quarter("20230418", 8) -> "2021Q2"
+    '''
+    if pd.isnull(date):
+        date = datetime.datetime.now()
+    t = x2datetime(date)
+    y, q = t.year, t.quarter
+    ynew, qnew = get_2part_next(y, q, 4, -n)
+    if not joiner:
+        return (ynew, qnew)
+    return joiner.join([str(ynew), str(qnew)])
+
+
 def get_dayofweek(date=None):
     '''返回date属于星期几（1-7）'''
     if pd.isnull(date):
         date = datetime.date.today()
     return x2datetime(date).weekday() + 1
```

### Comparing `dramkit-0.5.28/dramkit/datsci/_utils_ann.py` & `dramkit-0.5.29/dramkit/datsci/_utils_ann.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/datsci/activate_funcs.py` & `dramkit-0.5.29/dramkit/datsci/activate_funcs.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/datsci/ahp.py` & `dramkit-0.5.29/dramkit/datsci/ahp.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/datsci/ahp_sim_ri.py` & `dramkit-0.5.29/dramkit/datsci/ahp_sim_ri.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/datsci/apriori.py` & `dramkit-0.5.29/dramkit/datsci/apriori.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/datsci/curvature.py` & `dramkit-0.5.29/dramkit/datsci/curvature.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/datsci/elm_cls.py` & `dramkit-0.5.29/dramkit/datsci/elm_cls.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/datsci/elm_reg.py` & `dramkit-0.5.29/dramkit/datsci/elm_reg.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/datsci/entropy_weight.py` & `dramkit-0.5.29/dramkit/datsci/entropy_weight.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/datsci/find_maxmin.py` & `dramkit-0.5.29/dramkit/datsci/find_maxmin.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/datsci/freq_item_set.py` & `dramkit-0.5.29/dramkit/datsci/freq_item_set.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/datsci/lr.py` & `dramkit-0.5.29/dramkit/datsci/lr.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/datsci/preprocess.py` & `dramkit-0.5.29/dramkit/datsci/preprocess.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/datsci/stats.py` & `dramkit-0.5.29/dramkit/datsci/stats.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/datsci/time_series.py` & `dramkit-0.5.29/dramkit/datsci/time_series.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/datsci/topsis.py` & `dramkit-0.5.29/dramkit/datsci/topsis.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/datsci/utils_lgb.py` & `dramkit-0.5.29/dramkit/datsci/utils_lgb.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/datsci/utils_ml.py` & `dramkit-0.5.29/dramkit/datsci/utils_ml.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/find_addends/find_addends_backpack01float.py` & `dramkit-0.5.29/dramkit/find_addends/find_addends_backpack01float.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/find_addends/find_addends_backpack01int.py` & `dramkit-0.5.29/dramkit/find_addends/find_addends_backpack01int.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/find_addends/find_addends_bigfirst.py` & `dramkit-0.5.29/dramkit/find_addends/find_addends_bigfirst.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/find_addends/find_addends_recu.py` & `dramkit-0.5.29/dramkit/find_addends/find_addends_recu.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/find_addends/find_addends_smlfirst.py` & `dramkit-0.5.29/dramkit/find_addends/find_addends_smlfirst.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/find_addends/find_addends_utils.py` & `dramkit-0.5.29/dramkit/find_addends/find_addends_utils.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/gentools.py` & `dramkit-0.5.29/dramkit/gentools.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,28 +207,100 @@
 
 
 class StructureObject(object):
     def __init__(self, *args, **kwargs):
         raise DeprecatedError('`StructureObject`已弃用，请调用`GenObject`!')
         
         
-def run_func_with_timeout(func, args, timeout=10):
+def run_func_with_timeout_thread(func, *args,
+                                 timeout=10,
+                                 logger_error=False,
+                                 logger_timeout=None,
+                                 timeout_show_str=None,
+                                 kill_when_timeout=True,
+                                 **kwargs):
     '''
     | 限定时间(timeout秒)执行函数func，若限定时间内未执行完毕，返回None
     | args为tuple或list，为func函数接受的参数列表
+    
+    | 注：在线程中强制结束函数可能导致未知错误，
+    | 比如文件资源打开了但是强制结束时不能关闭
     '''
-    task = SingleThread(func, args, False) # 创建线程
+    # 创建线程
+    task = SingleThread(func, args, kwargs,
+                        logger=logger_error,
+                        # daemon=True
+                        )
     task.start() # 启动线程
     task.join(timeout=timeout) # 最大执行时间
-
-    # 若超时后，线程依旧运行，则强制结束
+    # 超时处理
     if task.is_alive():
-        task.stop_thread()
-
+        if not isnull(timeout_show_str):
+            logger_show(timeout_show_str, logger_timeout, 'warn')
+        # 强制结束
+        if kill_when_timeout:
+            task.stop_thread()
+            # task.join()
     return task.get_result()
+
+
+def with_timeout_thread(timeout=30,
+                        logger_error=None,
+                        logger_timeout=None,
+                        timeout_show_str=None,
+                        kill_when_timeout=True):
+    '''
+    | 作为装饰器在指定时间timeout(秒)内运行函数，超时则结束运行
+    | 通过控制线程实现
+
+    Examples
+    --------
+    .. code-block:: python
+        :linenos:
+
+        import os
+        import pandas as pd
+        from dramkit.gentools import tmprint
+        
+        df1 = pd.DataFrame([[1, 2], [3, 4]])
+        df2 = pd.DataFrame([[5, 6], [7, 8]])
+        df1.to_excel('df.xlsx')
+        TIMEOUT = 3
+        
+        @with_timeout_thread(TIMEOUT,
+                             logger_error=False
+                             )
+        def func(x):
+            with open('df.xlsx') as f:
+                tmprint('sleeping...')
+                time.sleep(5)
+            df2.to_excel('df.xlsx')
+            return x
+        
+        def test():
+            res = func('test')
+            print('res:', res)
+            os.remove('df.xlsx')
+            return res
+            
+    >>> res = test()
+    '''
+    def transfunc(func):
+        @wraps(func)
+        def timeouter(*args, **kwargs):
+            '''尝试在指定时间内运行func，超时则结束运行'''
+            return run_func_with_timeout_thread(
+                    func, *args, timeout=timeout, 
+                    logger_error=logger_error,
+                    logger_timeout=logger_timeout,
+                    timeout_show_str=timeout_show_str,
+                    kill_when_timeout=kill_when_timeout,
+                    **kwargs)
+        return timeouter
+    return transfunc
         
         
 def try_repeat_run(n_max_run=3, logger=None, sleep_seconds=0,
                    force_rep=False):
     '''
     | 作为装饰器尝试多次运行指定函数
     | 使用场景：第一次运行可能出错，需要再次运行(比如取数据时第一次可能连接超时，需要再取一次)
```

### Comparing `dramkit-0.5.28/dramkit/install_check.py` & `dramkit-0.5.29/dramkit/install_check.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/iotools.py` & `dramkit-0.5.29/dramkit/iotools.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,40 +8,42 @@
 import yaml
 import pickle
 import shutil
 import logging
 import zipfile
 import socket
 import inspect
+import platform
 import requests
 import traceback
 import subprocess
 import py_compile
 import pandas as pd
 from tqdm import tqdm
 from pathlib import Path
 from urllib.request import urlopen
 from dramkit.gentools import (isnull,
                               check_list_arg,
                               get_update_kwargs,
                               cut_range_to_subs,
                               get_tmp_col,
                               merge_df,
-                              update_df)
+                              update_df,
+                              run_func_with_timeout_thread)
 from dramkit.logtools.utils_logger import (logger_show,
                                            close_log_file)
 from dramkit.datetimetools import timestamp2str
-from dramkit.speedup.multi_thread import SingleThread
-from dramkit.speedup.multi_process import multi_process_concurrent
+from dramkit.speedup.multi_process_concurrent import multi_process_concurrent
 
+_WINDOWS_SYSTEM = 'windows' in platform.system().lower()
 
-SP = ' '
-CR = '\r'
-LF = '\n'
-CRLF = CR + LF
+_SP = ' '
+_CR = '\r'
+_LF = '\n'
+_CRLF = _CR + _LF
 
 
 class GetInputTimeoutError(Exception):
     pass
 
 
 def _echo(string):
@@ -65,27 +67,27 @@
     _echo(hint_str)
     begin = time.monotonic()
     end = begin + timeout
     line = ''
     while time.monotonic() < end:
         if msvcrt.kbhit():
             c = msvcrt.getwche()
-            if c in (CR, LF):
-                _echo(CRLF)
+            if c in (_CR, _LF):
+                _echo(_CRLF)
                 return line
             if c == '\003':
                 raise KeyboardInterrupt
             if c == '\b':
                 line = line[:-1]
-                cover = SP * len(hint_str + line + SP)
-                _echo(''.join([CR, cover, CR, hint_str, line]))
+                cover = _SP * len(hint_str + line + _SP)
+                _echo(''.join([_CR, cover, _CR, hint_str, line]))
             else:
                 line += c
         time.sleep(0.05)
-    _echo(CRLF)
+    _echo(_CRLF)
     raise GetInputTimeoutError
     
     
 def get_input_timeout_notwin(timeout=10, hint_str=None):
     '''
     | 非windows下设置在等待时间内获取input
     | https://pypi.org/project/inputimeout/
@@ -95,83 +97,50 @@
     hint_str = _check_hint_str(timeout, hint_str)
     _echo(hint_str)
     sel = selectors.DefaultSelector()
     sel.register(sys.stdin, selectors.EVENT_READ)
     events = sel.select(timeout)
     if events:
         key, _ = events[0]
-        return key.fileobj.readline().rstrip(LF)
+        return key.fileobj.readline().rstrip(_LF)
     else:
-        _echo(LF)
+        _echo(_LF)
         termios.tcflush(sys.stdin, termios.TCIFLUSH)
         raise GetInputTimeoutError
     
     
 def get_input_timeout(timeout=10, hint_str=None, logger=None):
     try:
-        if 'win' in sys.platform.lower():
+        if _WINDOWS_SYSTEM:
             res = get_input_timeout_win(timeout=timeout, hint_str=hint_str)
         else:
             res = get_input_timeout_notwin(timeout=timeout, hint_str=hint_str)
     except GetInputTimeoutError:
         logger_show('超时未接收到输入，返回None！', logger, 'warn')
         res = None
     return res
 
+
 def get_input_with_timeout(timeout=10, hint_str=None,
                            logger=None):
-    if 'win' in sys.platform.lower():
-        return _get_input_with_timeout0(timeout=timeout,
-               hint_str=hint_str, logger=logger)
-    else:
-        return _get_input_with_timeout(timeout=timeout,
-               hint_str=hint_str, logger=logger)
-
-
-def _get_input_with_timeout(timeout=10, hint_str=None,
-                            logger=None):
-    '''
-    | 通过input函数获取输入
-    | 若等待时间超过timeout秒没接收到输入，则返回None
-    | hint_str为input函数提示信息
-    | 参考：https://baijiahao.baidu.com/s?id=1757161895383507904&wfr=spider&for=pc
-    '''
-    hint_str = _check_hint_str(timeout, hint_str)
-    try:
-        res = get_input_timeout(timeout=timeout, hint_str=hint_str)
-    except GetInputTimeoutError:
-        logger_show('超时未接收到输入，返回None！', logger, 'warn')
-        res = None
-    return res
-
-
-def _get_input_with_timeout0(timeout=10, hint_str=None,
-                             logger=None):
     '''
     | 通过input函数获取输入
     | 若等待时间超过timeout秒没接收到输入，则返回None
     | hint_str为input函数提示信息
     | 参考：https://zhuanlan.zhihu.com/p/367634630
     '''
     def _get_input(hint_str):
         str_input = input(hint_str)
-        return str_input
-    
+        return str_input    
     hint_str = _check_hint_str(timeout, hint_str)
-
-    task = SingleThread(_get_input, (hint_str,), False) # 创建线程
-    task.start() # 启动线程
-    task.join(timeout=timeout) # 最大执行时间
-
-    # 若超时后，线程依旧运行，则强制结束
-    if task.is_alive():
-        logger_show('超时未接收到输入，返回None！', logger, 'warn')
-        task.stop_thread()
-
-    return task.get_result()
+    return run_func_with_timeout_thread(
+            _get_input, hint_str, timeout=timeout,
+            timeout_show_str='超时未接收到输入，返回None！',
+            logger_error=False, logger_timeout=logger,
+            kill_when_timeout=True)
 
 
 def get_input_multi_line(end_word='end', end_char='',
                          hint_str=None, hint_lineno=True):
     '''
     | input读取多行输入（包括回车换行符也会被保留）
     | end_word设置结束词，当在一行里面输入完整结束词，则表示输入完毕
@@ -269,30 +238,24 @@
     :returns: `dict` - 返回读取数据
     '''
 
     if not os.path.exists(fpath):
         logger_show('文件不存在，返回None：{}'.format(fpath),
                     logger, 'warn')
         return None
-
-    try:
-        with open(fpath, 'r', encoding=encoding) as f:
-            data_json = json.load(f)
-    except:
+                
+    for en in [encoding, 'utf-8', 'gbk', None]:
         try:
-            with open(fpath, 'r', encoding='utf-8') as f:
+            with open(fpath, 'r', encoding=en) as f:
                 data_json = json.load(f)
+            break
         except:
-            try:
-                with open(fpath, 'r', encoding='gbk') as f:
-                    data_json = json.load(f)
-            except:
-                logger_show('读取%s出错，请检查文件（如编码或文件末尾多余字符等问题）！'%fpath,
-                            logger, 'error')
-                raise
+            logger_show('读取%s出错，请检查文件（如编码或文件末尾多余字符等问题）！'%fpath,
+                        logger, 'error')
+            raise
 
     return data_json
 
 
 def write_json(data, fpath, encoding=None, mode='w', **kwargs):
     '''
     把data写入json格式文件
@@ -461,55 +424,131 @@
     if ftype in ['dta']:
         ftype = 'stata'
     if ftype in ['pk', 'pkl']:
         ftype = 'pickle'
     return ftype
 
 
+def _drop_unname_cols(df):
+    _cols = [x for x in df.columns if 'unnamed:' in str(x).lower()]
+    if len(_cols) > 0:
+        df = df.drop(_cols, axis=1)
+    return df
+
+
 def df2file_pd(df, fpath, ftype=None, **kwargs):
     '''pandas.DataFrame写入文件'''
     ftype = _get_pd_ftype(fpath, ftype)
     exec('df.to_{}(fpath, **kwargs)'.format(ftype))
 
 
+def _pd_load_df_check(fpath, ftype, logger):
+    if not os.path.exists(fpath):
+        logger_show('文件不存在，返回None：{}!'.format(fpath),
+                    logger, 'warn')
+        return None
+    ftype = _get_pd_ftype(fpath, ftype)
+    allows = [x.split('_')[-1] for x in dir(pd) if x.startswith('read_')]
+    if ftype not in allows:
+        logger_show('不支持的文件类型: `{}`！'.format(ftype))
+        raise
+    read_func = eval('pd.read_{}'.format(ftype))
+    return read_func
+
+
+def _process_df_pd_big(read_func, fpath,
+                       chunksize=100000,
+                       read_kwargs={},
+                       del_unname_cols=True,
+                       process_func=None,
+                       process_args=(),
+                       process_kwargs={},
+                       return_df=True):
+    df_iter = read_func(fpath, chunksize=chunksize,
+                        **read_kwargs)
+    res = []
+    for tmp in df_iter:
+        if del_unname_cols:
+            tmp = _drop_unname_cols(tmp)
+        if not isnull(process_func):
+            tmp = process_func(tmp, *process_args, **process_kwargs)
+        res.append(tmp)
+    if return_df:
+        res = pd.concat(res, axis=0)
+    return res
+
+
+def process_df_pd_big(fpath: str,
+                      ftype: str = None,
+                      chunksize : int = 100000,
+                      del_unname_cols: bool = True,
+                      logger: logging.Logger = None,
+                      read_kwargs: dict = {},
+                      process_func=None,
+                      process_args: tuple = (),
+                      process_kwargs: dict = {},
+                      return_df: bool = True):
+    '''用pandas读取大数据文件并分批处理，返回处理后的结果'''
+    read_func = _pd_load_df_check(fpath, ftype, logger)
+    if isnull(read_func):
+        return None
+    res = _process_df_pd_big(read_func, fpath,
+                             chunksize=chunksize,
+                             read_kwargs=read_kwargs,
+                             del_unname_cols=del_unname_cols,
+                             process_func=process_func,
+                             process_args=process_args,
+                             process_kwargs=process_kwargs,
+                             return_df=return_df)
+    return res
+
+
 def load_df_pd(fpath: str,
                ftype: str = None,
                del_unname_cols: bool = True,
                encoding: str = None,
                logger: logging.Logger = None,
                **kwargs):
     '''用pandas读取文件，返回DataFrame'''
     
-    ftype = _get_pd_ftype(fpath, ftype)
-    allows = [x.split('_')[-1] for x in dir(pd) if x.startswith('read_')]
-    if ftype not in allows:
-        logger_show('不支持的文件类型: `{}`！'.format(ftype))
-        raise
-        
-    read_func = eval('pd.read_{}'.format(ftype))  
-    
-    if not os.path.exists(fpath):
-        logger_show('文件不存在，返回None：{}!'.format(fpath),
-                    logger, 'warn')
+    read_func = _pd_load_df_check(fpath, ftype, logger)
+    if isnull(read_func):
         return None
+    
+    _big = False
+    if 'chunksize' in kwargs and not isnull(kwargs['chunksize']):
+        _big = True
+        chunksize, kwargs = get_update_kwargs(
+            'chunksize', None, kwargs, func_update=False)
 
     data = None
-    for encoding in [encoding, 'utf-8', 'gbk']:
+    for en in [encoding, 'utf-8', 'gbk']:
         try:
-            data = read_func(fpath, encoding=encoding, **kwargs)
+            if not _big:
+                data = read_func(fpath, encoding=en, **kwargs)
+            else:
+                kwargs.update({'encoding': en})
+                data = _process_df_pd_big(read_func, fpath,
+                                          chunksize=chunksize,
+                                          del_unname_cols=False,
+                                          read_kwargs=kwargs)
             break
         except:
             pass
     if isnull(data):
-        data = read_func(fpath, **kwargs)
+        if not _big:
+            data = read_func(fpath, **kwargs)
+        else:
+            data = _process_df_pd_big(read_func, fpath,
+                                      chunksize=chunksize,
+                                      del_unname_cols=False,
+                                      read_kwargs=kwargs)
 
     if del_unname_cols:
-        del_cols = [x for x in data.columns if 'unnamed:' in str(x).lower()]
-        if len(del_cols) > 0:
-            data.drop(del_cols, axis=1, inplace=True)
+        data = _drop_unname_cols(data)
 
     return data
 
 
 def load_csv(fpath, del_unname_cols=True, encoding=None,
              logger=None, **kwargs):
     '''
@@ -718,14 +757,49 @@
     for k in range(len(subs)):
         i0, i1 = subs[k]
         path_ = add_ext_to_filename(fpath, '_%s'%(k+1))
         df_ = df.iloc[i0:i1, :].copy()
         df2file_pd(df_, path_, **kwargs_tofile)
         
         
+def get_fpath_ext_num(fpath):
+    '''
+    | 给定路径fpath，若不存在，则返回fpath，若存在则返回带数字在后缀的路径
+    | 比如fpath=xxx.y存在，则返回xxx_1.y，xxx_1.y也存在，则返回xxx_2.y
+    '''
+    if not os.path.exists(fpath):
+        return fpath
+    k = 1
+    res = add_ext_to_filename(fpath, '_%s'%k)
+    while os.path.exists(res):
+        res = add_ext_to_filename(fpath, '_{}'.format(k+1))
+        k += 1
+    return res
+        
+        
+def cut_bigdffile_by_maxline(fpath, max_line=100000,
+                             kwargs_loaddf={},
+                             kwargs_tofile={'index': None}):
+    def _df2file(df, fpath, **kwargs):
+        fpath_ = get_fpath_ext_num(fpath)
+        df2file_pd(df, fpath_, ftype=None, **kwargs)
+        return fpath_
+    fpaths = process_df_pd_big(fpath,
+                      ftype=None,
+                      chunksize=max_line,
+                      del_unname_cols=True,
+                      logger=None,
+                      read_kwargs=kwargs_loaddf,
+                      process_func=_df2file,
+                      process_args=(fpath,),
+                      process_kwargs=kwargs_tofile,
+                      return_df=False)
+    return fpaths
+        
+        
 def cut_dffile_by_year(fpath, tcol=None,
                        name_last_year=False,
                        kwargs_loaddf={},
                        kwargs_tofile={'index': None},
                        kwargs_exists_merge={},
                        logger=None):
     '''
@@ -1840,14 +1914,19 @@
     reqs_version = df_pip[df_pip['pkg'].isin(reqs)].copy()
     reqs_version.sort_values('pkg', ascending=True, inplace=True)
     reqs_str = '\n'.join(reqs)
     reqs_version_str = '\n'.join(['=='.join(x) for x in reqs_version.values])
     return (reqs, reqs_version), (reqs_str, reqs_version_str), (pkgs, df)
 
 
+def get_filedir(fpath):
+    '''获取fpath路径所在文件夹路径'''
+    return os.path.split(fpath)[0]
+
+
 def get_filename(fpath, with_ext=True):
     '''获取文件名（去除前缀路径），with_ext为False则返回不带后缀'''
     if with_ext:
         return os.path.basename(fpath)
     else:
         return os.path.basename(os.path.splitext(fpath)[0])
```

### Comparing `dramkit-0.5.28/dramkit/logtools/logger_general.py` & `dramkit-0.5.29/dramkit/logtools/logger_general.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/logtools/logger_rotating.py` & `dramkit-0.5.29/dramkit/logtools/logger_rotating.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/logtools/logger_timedrotating.py` & `dramkit-0.5.29/dramkit/logtools/logger_timedrotating.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/logtools/utils_logger.py` & `dramkit-0.5.29/dramkit/logtools/utils_logger.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/openai/aiedu_chat.py` & `dramkit-0.5.29/dramkit/openai/aiedu_chat.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/openai/openai_chat.py` & `dramkit-0.5.29/dramkit/openai/openai_chat.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/openai/openai_chat_hs.py` & `dramkit-0.5.29/dramkit/openai/openai_chat_hs.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/optimizer/alo.py` & `dramkit-0.5.29/dramkit/optimizer/alo.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/optimizer/base_funcs.py` & `dramkit-0.5.29/dramkit/optimizer/base_funcs.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/optimizer/boa.py` & `dramkit-0.5.29/dramkit/optimizer/boa.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/optimizer/cs.py` & `dramkit-0.5.29/dramkit/optimizer/cs.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/optimizer/ga.py` & `dramkit-0.5.29/dramkit/optimizer/ga.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/optimizer/gwo.py` & `dramkit-0.5.29/dramkit/optimizer/gwo.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/optimizer/hcpsoboa.py` & `dramkit-0.5.29/dramkit/optimizer/hcpsoboa.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/optimizer/hho.py` & `dramkit-0.5.29/dramkit/optimizer/hho.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/optimizer/hpsoboa.py` & `dramkit-0.5.29/dramkit/optimizer/hpsoboa.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/optimizer/pso.py` & `dramkit-0.5.29/dramkit/optimizer/pso.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/optimizer/utils_heuristic.py` & `dramkit-0.5.29/dramkit/optimizer/utils_heuristic.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/optimizer/woa.py` & `dramkit-0.5.29/dramkit/optimizer/woa.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/other/_Linux_notes.py` & `dramkit-0.5.29/dramkit/other/_Linux_notes.py`

 * *Files 4% similar despite different names*

```diff
@@ -123,8 +123,11 @@
 nvm -v
 nvm install 18
 node -v
 npm -v
 
 npm install -g pnpm # npm安装pnpm
 
+# unzip解压覆盖
+unzip -o xxx.zip
+
 # '''
```

### Comparing `dramkit-0.5.28/dramkit/other/_Python_notes.py` & `dramkit-0.5.29/dramkit/other/_Python_notes.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/other/langconv.py` & `dramkit-0.5.29/dramkit/other/langconv.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/other/othertools.py` & `dramkit-0.5.29/dramkit/other/othertools.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/other/replace_endblank.py` & `dramkit-0.5.29/dramkit/other/replace_endblank.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/other/zh_wiki.py` & `dramkit-0.5.29/dramkit/other/zh_wiki.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/plottools/plot_barline.py` & `dramkit-0.5.29/dramkit/plottools/plot_barline.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/plottools/plot_common.py` & `dramkit-0.5.29/dramkit/plottools/plot_common.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/plottools/plot_histdist.py` & `dramkit-0.5.29/dramkit/plottools/plot_histdist.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/plottools/plot_scatter.py` & `dramkit-0.5.29/dramkit/plottools/plot_scatter.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/plottools/utils_plot.py` & `dramkit-0.5.29/dramkit/plottools/utils_plot.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/pystyles/dramkit_style.py` & `dramkit-0.5.29/dramkit/pystyles/dramkit_style.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/sorts/bubble_sort.py` & `dramkit-0.5.29/dramkit/sorts/bubble_sort.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/sorts/bucket_sort.py` & `dramkit-0.5.29/dramkit/sorts/bucket_sort.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/sorts/insert_sort.py` & `dramkit-0.5.29/dramkit/sorts/insert_sort.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/sorts/insert_sort_bin.py` & `dramkit-0.5.29/dramkit/sorts/insert_sort_bin.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/sorts/quick_sort.py` & `dramkit-0.5.29/dramkit/sorts/quick_sort.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/speedup/multi_process.py` & `dramkit-0.5.29/dramkit/speedup/multi_process_concurrent.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 # -*- coding: utf-8 -*-
 
 import time
-from concurrent.futures import as_completed
-from concurrent.futures import ProcessPoolExecutor
+import platform
+from concurrent.futures import (as_completed,
+                                ProcessPoolExecutor)
+from dramkit.gentools import tmprint, print_used_time
 
+_WINDOWS_SYSTEM = 'windows' in platform.system().lower()
 
+#%%
+@print_used_time
 def multi_process_concurrent(func, args_list,
                              keep_order=True,
                              multi_line=None):
     '''
     多进程，同一个函数执行多次
 
     Parameters
@@ -22,15 +27,15 @@
 
         .. caution:: 
             若keep_order为True，则func的格式应转化为：
 
             | def func(args):
             |     return f(\*args)
     multi_line : int, None
-        最大线程数，默认等于len(args_list)
+        最大进程数，默认等于len(args_list)
 
     Returns
     -------
     results : list
         每个元素对应func以args_list的元素为输入的返回结果
 
     Note
@@ -69,38 +74,40 @@
 
 
 def _func_test_win_new(args):
     return _func_test_win(*args)
 
 #%%
 if __name__ == '__main__':
-    import platform
-
+    from dramkit import TimeRecoder
 
     def func(idx, sleep_tm):
         '''注：若此目标函数定义在__name__ == '__main__'之后，则在windows下会报错'''
         print('task id:', idx)
         time.sleep(sleep_tm)
         print('task id: {}; slept: {}s.'.format(idx, sleep_tm))
         return [idx, sleep_tm]
 
     def func_new(args):
         return func(*args)
 
     args_list = [[1, 2], [3, 4], [4, 5], [2, 3]]
+    args_list = [[1, 20], [3, 40], [4, 50], [2, 30]]
 
 
-    print('multi-process, concurrent............................')
-    strt_tm = time.monotonic()
-    if platform.system() == 'Windows':
+    # '''
+    tmprint('multi-process, concurrent...................')
+    tr = TimeRecoder()
+    if _WINDOWS_SYSTEM:
         results_Order = multi_process_concurrent(_func_test_win_new, args_list,
                                                  keep_order=True)
         results_noOrder = multi_process_concurrent(_func_test_win, args_list,
                                                    keep_order=False)
         results_Order2 = multi_process_concurrent(_func_test_win_new, args_list,
                                                   keep_order=True, multi_line=2)
     else:
         results_Order = multi_process_concurrent(func_new, args_list,
                                                  keep_order=True)
         results_noOrder = multi_process_concurrent(func, args_list,
                                                    keep_order=False)
-    print('total used time: {tm}s.'.format(tm=round(time.monotonic() - strt_tm,6)))
+    tr.used()
+    # '''
```

### Comparing `dramkit-0.5.28/dramkit/sqltools/_Hive_notes.py` & `dramkit-0.5.29/dramkit/sqltools/_Hive_notes.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/sqltools/_MySQL_notes.py` & `dramkit-0.5.29/dramkit/sqltools/_MySQL_notes.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,22 @@
 -- 查看安装文件目录
 SHOW VARIABLES LIKE "basedir";
 SELECT @@basedir;
 
 -- （windows）mysql57开启bin log，在配置文件my.ini中[mysqld]下添加内容：log-bin=mysql-bin
 -- （windows）mysql8关闭bin log，在配置文件my.ini中[mysqld]下添加内容：skip-log-bin
 
+-- 2006 MySQL server has gone解决
+show global status like 'uptime'; /*查看mysql的运行时长*/
+show global variables like '%timeout'; /*查看超时设置*/
+set global wait_timeout=3600*48; /*设置连接超时*/
+show global status like 'com_kill'; /*查看连接进程被kill*/
+show global variables like 'max_allowed_packet'; /*查看查询结果大小限制*/
+set global max_allowed_packet=1024*1024*16; /*修改查询结果大小限制*/
+
 -- Ubuntu设置MySql局域网可以访问
 -- 1. 编辑 /etc/mysql/mysql.conf.d/mysqld.cnf
 -- 把里面的bind-address = 127.0.0.1
 -- 改成  # bind-address = 127.0.0.1 进行屏蔽
 -- 2：
 mysql -uroot -ppassword /*登录*/
 use mysql;
```

### Comparing `dramkit-0.5.28/dramkit/sqltools/_Oracle_notes.py` & `dramkit-0.5.29/dramkit/sqltools/_Oracle_notes.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/sqltools/cxoracle.py` & `dramkit-0.5.29/dramkit/sqltools/cxoracle.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/sqltools/py_hive.py` & `dramkit-0.5.29/dramkit/sqltools/py_hive.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/sqltools/py_mysql.py` & `dramkit-0.5.29/dramkit/sqltools/py_mysql.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/sqltools/sql_alchemy.py` & `dramkit-0.5.29/dramkit/sqltools/sql_alchemy.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/webtools/utils_html.py` & `dramkit-0.5.29/dramkit/webtools/utils_html.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit/wechat/qywechat.py` & `dramkit-0.5.29/dramkit/wechat/qywechat.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.28/dramkit.egg-info/PKG-INFO` & `dramkit-0.5.29/dramkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dramkit
-Version: 0.5.28
+Version: 0.5.29
 Summary: DramKit is a toolbox.
 Home-page: https://github.com/Genlovy-Hoo/dramkit/
 Author: Genlovy Hoo, YueYong Hu
 Author-email: genlovhyy@163.com
 License: MIT
 Platform: any
 Description-Content-Type: text/markdown
```

### Comparing `dramkit-0.5.28/dramkit.egg-info/SOURCES.txt` & `dramkit-0.5.29/dramkit.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -29,22 +29,24 @@
 dramkit/_tmp/mpc_test1.py
 dramkit/_tmp/options_Implied_volatility.py
 dramkit/_tmp/pf_test.py
 dramkit/_tmp/plot_test.py
 dramkit/_tmp/plot_test2.py
 dramkit/_tmp/simple_smooth.py
 dramkit/_tmp/test_async_washs.py
+dramkit/_tmp/test_await_timeout.py
 dramkit/_tmp/test_backtrader.py
 dramkit/_tmp/test_chatgpt_v1.py
 dramkit/_tmp/test_code.py
 dramkit/_tmp/test_find_peaks.py
 dramkit/_tmp/test_get_var_name.py
 dramkit/_tmp/test_grading.py
 dramkit/_tmp/test_lr.py
 dramkit/_tmp/test_maxsort.py
+dramkit/_tmp/test_multiprocessing.py
 dramkit/_tmp/test_ocr.py
 dramkit/_tmp/test_pywechat.py
 dramkit/_tmp/test_tree.py
 dramkit/_tmp/test_tree2.py
 dramkit/_tmp/test_wechat_work.py
 dramkit/_tmp/tfDNNCls_test.py
 dramkit/_tmp/tmp.py
@@ -140,15 +142,19 @@
 dramkit/sorts/__init__.py
 dramkit/sorts/bubble_sort.py
 dramkit/sorts/bucket_sort.py
 dramkit/sorts/insert_sort.py
 dramkit/sorts/insert_sort_bin.py
 dramkit/sorts/quick_sort.py
 dramkit/speedup/__init__.py
-dramkit/speedup/multi_process.py
+dramkit/speedup/_mp_test1.py
+dramkit/speedup/_mp_test2.py
+dramkit/speedup/_mp_test3.py
+dramkit/speedup/iotools_tmp.py
+dramkit/speedup/multi_process_concurrent.py
 dramkit/speedup/multi_thread.py
 dramkit/sqltools/_Hive_notes.py
 dramkit/sqltools/_MySQL_notes.py
 dramkit/sqltools/_Oracle_notes.py
 dramkit/sqltools/__init__.py
 dramkit/sqltools/cxoracle.py
 dramkit/sqltools/py_hive.py
```

### Comparing `dramkit-0.5.28/setup.py` & `dramkit-0.5.29/setup.py`

 * *Files identical despite different names*


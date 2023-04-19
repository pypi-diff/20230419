# Comparing `tmp/retentioneering-3.0.0b1.tar.gz` & `tmp/retentioneering-3.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retentioneering-3.0.0b1.tar", max compression
+gzip compressed data, was "retentioneering-3.0.0b2.tar", max compression
```

## Comparing `retentioneering-3.0.0b1.tar` & `retentioneering-3.0.0b2.tar`

### file list

```diff
@@ -1,123 +1,128 @@
--rw-r--r--   0        0        0     7341 2022-09-06 07:58:30.273796 retentioneering-3.0.0b1/LICENSE
--rw-r--r--   0        0        0     2065 2023-03-22 12:06:39.614862 retentioneering-3.0.0b1/pyproject.toml
--rw-r--r--   0        0        0      347 2023-03-22 12:06:27.631508 retentioneering-3.0.0b1/retentioneering/__init__.py
--rw-r--r--   0        0        0       84 2023-01-16 14:26:06.541078 retentioneering-3.0.0b1/retentioneering/backend/__init__.py
--rw-r--r--   0        0        0      113 2023-01-16 14:26:06.541078 retentioneering-3.0.0b1/retentioneering/backend/callback/__init__.py
--rw-r--r--   0        0        0      487 2023-01-16 14:26:06.541078 retentioneering-3.0.0b1/retentioneering/backend/callback/list_dataprocessors.py
--rw-r--r--   0        0        0     5290 2023-01-16 14:26:06.541078 retentioneering-3.0.0b1/retentioneering/backend/callback/mock_list_dataprocessor.py
--rw-r--r--   0        0        0     1097 2023-01-16 14:26:06.541078 retentioneering-3.0.0b1/retentioneering/backend/jupiter_server.py
--rw-r--r--   0        0        0     5293 2023-03-14 09:18:13.137154 retentioneering-3.0.0b1/retentioneering/backend/server_manager.py
--rw-r--r--   0        0        0       59 2023-03-07 11:03:25.184838 retentioneering-3.0.0b1/retentioneering/constants/__init__.py
--rw-r--r--   0        0        0      345 2023-03-07 11:03:25.184838 retentioneering-3.0.0b1/retentioneering/constants/constants.py
--rw-r--r--   0        0        0       42 2023-01-16 14:26:06.541078 retentioneering-3.0.0b1/retentioneering/data_processor/__init__.py
--rw-r--r--   0        0        0     2190 2023-03-07 11:03:25.184838 retentioneering-3.0.0b1/retentioneering/data_processor/data_processor.py
--rw-r--r--   0        0        0     1744 2023-03-07 11:03:25.184838 retentioneering-3.0.0b1/retentioneering/data_processor/registry.py
--rw-r--r--   0        0        0      841 2023-01-16 14:26:06.541078 retentioneering-3.0.0b1/retentioneering/data_processors_lib/__init__.py
--rw-r--r--   0        0        0     4892 2023-03-22 12:06:27.631508 retentioneering-3.0.0b1/retentioneering/data_processors_lib/collapse_loops.py
--rw-r--r--   0        0        0     3546 2023-03-22 12:06:27.631508 retentioneering-3.0.0b1/retentioneering/data_processors_lib/delete_users_by_path_length.py
--rw-r--r--   0        0        0     2342 2023-03-22 12:06:27.631508 retentioneering-3.0.0b1/retentioneering/data_processors_lib/filter_events.py
--rw-r--r--   0        0        0     3332 2023-03-22 12:06:27.631508 retentioneering-3.0.0b1/retentioneering/data_processors_lib/group_events.py
--rw-r--r--   0        0        0     4696 2023-03-22 12:06:27.631508 retentioneering-3.0.0b1/retentioneering/data_processors_lib/lost_users.py
--rw-r--r--   0        0        0     4055 2023-03-22 12:06:27.631508 retentioneering-3.0.0b1/retentioneering/data_processors_lib/negative_target.py
--rw-r--r--   0        0        0     3173 2023-03-22 12:06:27.631508 retentioneering-3.0.0b1/retentioneering/data_processors_lib/new_users.py
--rw-r--r--   0        0        0     3962 2023-03-22 12:06:27.631508 retentioneering-3.0.0b1/retentioneering/data_processors_lib/positive_target.py
--rw-r--r--   0        0        0     1760 2023-03-17 11:02:30.068802 retentioneering-3.0.0b1/retentioneering/data_processors_lib/rename.py
--rw-r--r--   0        0        0     8627 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/data_processors_lib/split_sessions.py
--rw-r--r--   0        0        0     2437 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/data_processors_lib/start_end_events.py
--rw-r--r--   0        0        0     6571 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/data_processors_lib/truncate_path.py
--rw-r--r--   0        0        0     5760 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/data_processors_lib/truncated_events.py
--rw-r--r--   0        0        0       56 2023-01-16 14:26:06.544412 retentioneering-3.0.0b1/retentioneering/datasets/__init__.py
--rw-r--r--   0        0        0        0 2023-01-16 14:26:06.544412 retentioneering-3.0.0b1/retentioneering/datasets/data/__init__.py
--rw-r--r--   0        0        0  1903381 2023-01-16 14:26:06.551078 retentioneering-3.0.0b1/retentioneering/datasets/data/ab_test_demo.csv
--rw-r--r--   0        0        0  1467900 2023-03-07 11:03:25.188171 retentioneering-3.0.0b1/retentioneering/datasets/data/simple-onlineshop.csv
--rw-r--r--   0        0        0     1352 2023-03-07 11:03:25.188171 retentioneering-3.0.0b1/retentioneering/datasets/load.py
--rw-r--r--   0        0        0       31 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/edgelist/__init__.py
--rw-r--r--   0        0        0     4222 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/edgelist/edgelist.py
--rw-r--r--   0        0        0      486 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/eventstream/__init__.py
--rw-r--r--   0        0        0    41037 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/eventstream/eventstream.py
--rw-r--r--   0        0        0      719 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/eventstream/helpers/__init__.py
--rw-r--r--   0        0        0     1574 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/eventstream/helpers/collapse_loops_helper.py
--rw-r--r--   0        0        0     1434 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/eventstream/helpers/delete_users_by_path_length_helper.py
--rw-r--r--   0        0        0     1137 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/eventstream/helpers/filter_helper.py
--rw-r--r--   0        0        0     1454 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/eventstream/helpers/group_helper.py
--rw-r--r--   0        0        0     1381 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/eventstream/helpers/lost_users_helper.py
--rw-r--r--   0        0        0     1410 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/eventstream/helpers/negative_target.py
--rw-r--r--   0        0        0     1196 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/eventstream/helpers/new_users_helper.py
--rw-r--r--   0        0        0     1409 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/eventstream/helpers/positive_target.py
--rw-r--r--   0        0        0      692 2023-03-14 09:18:13.137154 retentioneering-3.0.0b1/retentioneering/eventstream/helpers/rename_helper.py
--rw-r--r--   0        0        0     1882 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/eventstream/helpers/split_session_helper.py
--rw-r--r--   0        0        0     1009 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/eventstream/helpers/start_end_helper.py
--rw-r--r--   0        0        0     1670 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/eventstream/helpers/truncate_path_helper.py
--rw-r--r--   0        0        0     1517 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/eventstream/helpers/truncated_events_helper.py
--rw-r--r--   0        0        0     4157 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/eventstream/schema.py
--rw-r--r--   0        0        0     2389 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/eventstream/types.py
--rw-r--r--   0        0        0        0 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/exceptions/__init__.py
--rw-r--r--   0        0        0       45 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/exceptions/base.py
--rw-r--r--   0        0        0     1242 2023-03-07 11:03:25.191505 retentioneering-3.0.0b1/retentioneering/exceptions/server.py
--rw-r--r--   0        0        0      306 2023-03-07 11:03:25.191505 retentioneering-3.0.0b1/retentioneering/exceptions/widget.py
--rw-r--r--   0        0        0       81 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/graph/__init__.py
--rw-r--r--   0        0        0     4073 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/graph/nodes.py
--rw-r--r--   0        0        0    13921 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/graph/p_graph.py
--rw-r--r--   0        0        0       31 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/nodelist/__init__.py
--rw-r--r--   0        0        0     1071 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/nodelist/nodelist.py
--rw-r--r--   0        0        0       38 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/params_model/__init__.py
--rw-r--r--   0        0        0    10064 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/params_model/params_model.py
--rw-r--r--   0        0        0      952 2023-03-07 11:03:25.191505 retentioneering-3.0.0b1/retentioneering/params_model/registry.py
--rw-r--r--   0        0        0        0 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/preprocessor/__init__.py
--rw-r--r--   0        0        0       41 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/templates/__init__.py
--rw-r--r--   0        0        0       33 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/templates/p_graph/__init__.py
--rw-r--r--   0        0        0     1704 2023-03-07 11:03:25.191505 retentioneering-3.0.0b1/retentioneering/templates/p_graph/p_graph.html
--rw-r--r--   0        0        0      700 2023-03-07 11:03:25.191505 retentioneering-3.0.0b1/retentioneering/templates/p_graph/show.py
--rw-r--r--   0        0        0       42 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/templates/transition_graph/__init__.py
--rw-r--r--   0        0        0       22 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/templates/transition_graph/body.html
--rw-r--r--   0        0        0      713 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/templates/transition_graph/full.html
--rw-r--r--   0        0        0      894 2023-03-07 11:03:25.191505 retentioneering-3.0.0b1/retentioneering/templates/transition_graph/init_template.py
--rw-r--r--   0        0        0     1507 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/templates/transition_graph/inner_iframe.html
--rw-r--r--   0        0        0     1143 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/templates/transition_graph/show.py
--rw-r--r--   0        0        0        0 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/tooling/__init__.py
--rw-r--r--   0        0        0       31 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/tooling/clusters/__init__.py
--rw-r--r--   0        0        0    33379 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/tooling/clusters/clusters.py
--rw-r--r--   0        0        0     2039 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/tooling/clusters/segments.py
--rw-r--r--   0        0        0     3166 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/tooling/clusters/userlist.py
--rw-r--r--   0        0        0       29 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/tooling/cohorts/__init__.py
--rw-r--r--   0        0        0    12952 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/tooling/cohorts/cohorts.py
--rw-r--r--   0        0        0       39 2023-03-07 11:03:25.191505 retentioneering-3.0.0b1/retentioneering/tooling/constants/__init__.py
--rw-r--r--   0        0        0      240 2023-03-07 11:03:25.191505 retentioneering-3.0.0b1/retentioneering/tooling/constants/constants.py
--rw-r--r--   0        0        0       31 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/tooling/describe/__init__.py
--rw-r--r--   0        0        0     4560 2023-03-14 09:18:13.140487 retentioneering-3.0.0b1/retentioneering/tooling/describe/describe.py
--rw-r--r--   0        0        0       44 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/tooling/describe_events/__init__.py
--rw-r--r--   0        0        0     4828 2023-03-14 09:18:13.140487 retentioneering-3.0.0b1/retentioneering/tooling/describe_events/describe_events.py
--rw-r--r--   0        0        0       53 2023-01-16 14:26:06.557745 retentioneering-3.0.0b1/retentioneering/tooling/event_timestamp_hist/__init__.py
--rw-r--r--   0        0        0     5552 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/tooling/event_timestamp_hist/event_timestamp_hist.py
--rw-r--r--   0        0        0       27 2023-01-16 14:26:06.561078 retentioneering-3.0.0b1/retentioneering/tooling/funnel/__init__.py
--rw-r--r--   0        0        0    12195 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/tooling/funnel/funnel.py
--rw-r--r--   0        0        0       43 2023-03-07 11:03:25.191505 retentioneering-3.0.0b1/retentioneering/tooling/mixins/__init__.py
--rw-r--r--   0        0        0     1427 2023-03-07 11:03:25.191505 retentioneering-3.0.0b1/retentioneering/tooling/mixins/ended_events.py
--rw-r--r--   0        0        0       67 2023-01-16 14:26:06.561078 retentioneering-3.0.0b1/retentioneering/tooling/stattests/__init__.py
--rw-r--r--   0        0        0      167 2023-01-16 14:26:06.561078 retentioneering-3.0.0b1/retentioneering/tooling/stattests/constants.py
--rw-r--r--   0        0        0    11911 2023-03-22 12:06:27.634842 retentioneering-3.0.0b1/retentioneering/tooling/stattests/stattests.py
--rw-r--r--   0        0        0       36 2023-01-16 14:26:06.561078 retentioneering-3.0.0b1/retentioneering/tooling/step_matrix/__init__.py
--rw-r--r--   0        0        0    21475 2023-03-22 12:06:27.638175 retentioneering-3.0.0b1/retentioneering/tooling/step_matrix/step_matrix.py
--rw-r--r--   0        0        0       36 2023-01-16 14:26:06.561078 retentioneering-3.0.0b1/retentioneering/tooling/step_sankey/__init__.py
--rw-r--r--   0        0        0    24468 2023-03-22 12:06:27.638175 retentioneering-3.0.0b1/retentioneering/tooling/step_sankey/step_sankey.py
--rw-r--r--   0        0        0      110 2023-03-07 11:03:25.191505 retentioneering-3.0.0b1/retentioneering/tooling/timedelta_hist/__init__.py
--rw-r--r--   0        0        0      186 2023-03-07 11:03:25.191505 retentioneering-3.0.0b1/retentioneering/tooling/timedelta_hist/constants.py
--rw-r--r--   0        0        0    13335 2023-03-22 12:06:27.638175 retentioneering-3.0.0b1/retentioneering/tooling/timedelta_hist/timedelta_hist.py
--rw-r--r--   0        0        0       46 2023-03-22 12:06:27.638175 retentioneering-3.0.0b1/retentioneering/tooling/transition_graph/__init__.py
--rw-r--r--   0        0        0    32526 2023-03-22 12:06:27.638175 retentioneering-3.0.0b1/retentioneering/tooling/transition_graph/transition_graph.py
--rw-r--r--   0        0        0       48 2023-03-07 11:03:25.191505 retentioneering-3.0.0b1/retentioneering/tooling/transition_matrix/__init__.py
--rw-r--r--   0        0        0     3264 2023-03-22 12:06:27.638175 retentioneering-3.0.0b1/retentioneering/tooling/transition_matrix/transition_matrix.py
--rw-r--r--   0        0        0        0 2023-03-07 11:03:25.191505 retentioneering-3.0.0b1/retentioneering/tooling/typing/__init__.py
--rw-r--r--   0        0        0      171 2023-03-07 11:03:25.191505 retentioneering-3.0.0b1/retentioneering/tooling/typing/transition_graph/__init__.py
--rw-r--r--   0        0        0     1327 2023-03-22 12:06:27.638175 retentioneering-3.0.0b1/retentioneering/tooling/typing/transition_graph/graph_types.py
--rw-r--r--   0        0        0       49 2023-01-16 14:26:06.561078 retentioneering-3.0.0b1/retentioneering/tooling/user_lifetime_hist/__init__.py
--rw-r--r--   0        0        0     6525 2023-03-22 12:06:27.638175 retentioneering-3.0.0b1/retentioneering/tooling/user_lifetime_hist/user_lifetime_hist.py
--rw-r--r--   0        0        0      458 2023-01-16 14:26:06.561078 retentioneering-3.0.0b1/retentioneering/utils/__init__.py
--rw-r--r--   0        0        0      122 2023-03-07 11:03:25.191505 retentioneering-3.0.0b1/retentioneering/utils/dict.py
--rw-r--r--   0        0        0      465 2023-01-16 14:26:06.561078 retentioneering-3.0.0b1/retentioneering/utils/list.py
--rw-r--r--   0        0        0      444 2023-01-16 14:26:06.561078 retentioneering-3.0.0b1/retentioneering/utils/pandas.py
--rw-r--r--   0        0        0      986 2023-03-07 11:03:25.191505 retentioneering-3.0.0b1/retentioneering/utils/registry.py
--rw-r--r--   0        0        0      269 2023-01-16 14:26:06.561078 retentioneering-3.0.0b1/retentioneering/utils/singleton.py
--rw-r--r--   0        0        0       77 2023-03-07 11:03:25.191505 retentioneering-3.0.0b1/retentioneering/widget/__init__.py
--rw-r--r--   0        0        0     7265 2023-03-07 16:29:54.477842 retentioneering-3.0.0b1/retentioneering/widget/widgets.py
--rw-r--r--   0        0        0     1283 1970-01-01 00:00:00.000000 retentioneering-3.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0     7341 2022-09-06 07:58:30.273796 retentioneering-3.0.0b2/LICENSE
+-rw-r--r--   0        0        0     1947 2023-04-19 10:57:10.934033 retentioneering-3.0.0b2/pyproject.toml
+-rw-r--r--   0        0        0      375 2023-04-19 10:56:29.220603 retentioneering-3.0.0b2/retentioneering/__init__.py
+-rw-r--r--   0        0        0       84 2023-01-16 14:26:06.541078 retentioneering-3.0.0b2/retentioneering/backend/__init__.py
+-rw-r--r--   0        0        0      113 2023-01-16 14:26:06.541078 retentioneering-3.0.0b2/retentioneering/backend/callback/__init__.py
+-rw-r--r--   0        0        0      490 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/backend/callback/list_dataprocessors.py
+-rw-r--r--   0        0        0     5220 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/backend/callback/mock_list_dataprocessor.py
+-rw-r--r--   0        0        0     1097 2023-01-16 14:26:06.541078 retentioneering-3.0.0b2/retentioneering/backend/jupiter_server.py
+-rw-r--r--   0        0        0     5293 2023-04-03 06:56:53.875728 retentioneering-3.0.0b2/retentioneering/backend/server_manager.py
+-rw-r--r--   0        0        0      149 2023-04-17 15:56:20.806436 retentioneering-3.0.0b2/retentioneering/backend/tracker/__init__.py
+-rw-r--r--   0        0        0     1675 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/backend/tracker/connector.py
+-rw-r--r--   0        0        0     2036 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/backend/tracker/hwid.py
+-rw-r--r--   0        0        0     2381 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/backend/tracker/tracker.py
+-rw-r--r--   0        0        0     1162 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/backend/tracker/tracking_info.py
+-rw-r--r--   0        0        0       59 2023-03-07 11:03:25.184838 retentioneering-3.0.0b2/retentioneering/constants/__init__.py
+-rw-r--r--   0        0        0      345 2023-03-07 11:03:25.184838 retentioneering-3.0.0b2/retentioneering/constants/constants.py
+-rw-r--r--   0        0        0       42 2023-01-16 14:26:06.541078 retentioneering-3.0.0b2/retentioneering/data_processor/__init__.py
+-rw-r--r--   0        0        0     2190 2023-03-07 11:03:25.184838 retentioneering-3.0.0b2/retentioneering/data_processor/data_processor.py
+-rw-r--r--   0        0        0     1744 2023-03-07 11:03:25.184838 retentioneering-3.0.0b2/retentioneering/data_processor/registry.py
+-rw-r--r--   0        0        0      843 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/data_processors_lib/__init__.py
+-rw-r--r--   0        0        0     3887 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/data_processors_lib/add_negative_events.py
+-rw-r--r--   0        0        0     3794 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/data_processors_lib/add_positive_events.py
+-rw-r--r--   0        0        0     2449 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/data_processors_lib/add_start_end_events.py
+-rw-r--r--   0        0        0     4781 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/data_processors_lib/collapse_loops.py
+-rw-r--r--   0        0        0     3517 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/data_processors_lib/drop_paths.py
+-rw-r--r--   0        0        0     2342 2023-04-03 06:56:53.879061 retentioneering-3.0.0b2/retentioneering/data_processors_lib/filter_events.py
+-rw-r--r--   0        0        0     3332 2023-04-03 06:56:53.879061 retentioneering-3.0.0b2/retentioneering/data_processors_lib/group_events.py
+-rw-r--r--   0        0        0     5454 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/data_processors_lib/label_cropped_paths.py
+-rw-r--r--   0        0        0     4633 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/data_processors_lib/label_lost_users.py
+-rw-r--r--   0        0        0     3186 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/data_processors_lib/label_new_users.py
+-rw-r--r--   0        0        0     1760 2023-03-17 11:02:30.068802 retentioneering-3.0.0b2/retentioneering/data_processors_lib/rename.py
+-rw-r--r--   0        0        0     8492 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/data_processors_lib/split_sessions.py
+-rw-r--r--   0        0        0     6575 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/data_processors_lib/truncate_paths.py
+-rw-r--r--   0        0        0       56 2023-01-16 14:26:06.544412 retentioneering-3.0.0b2/retentioneering/datasets/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-16 14:26:06.544412 retentioneering-3.0.0b2/retentioneering/datasets/data/__init__.py
+-rw-r--r--   0        0        0  1903381 2023-01-16 14:26:06.551078 retentioneering-3.0.0b2/retentioneering/datasets/data/ab_test_demo.csv
+-rw-r--r--   0        0        0  1467900 2023-03-07 11:03:25.188171 retentioneering-3.0.0b2/retentioneering/datasets/data/simple-onlineshop.csv
+-rw-r--r--   0        0        0     1352 2023-03-07 11:03:25.188171 retentioneering-3.0.0b2/retentioneering/datasets/load.py
+-rw-r--r--   0        0        0       31 2023-01-16 14:26:06.557745 retentioneering-3.0.0b2/retentioneering/edgelist/__init__.py
+-rw-r--r--   0        0        0     4222 2023-04-03 06:56:53.879061 retentioneering-3.0.0b2/retentioneering/edgelist/edgelist.py
+-rw-r--r--   0        0        0      486 2023-01-16 14:26:06.557745 retentioneering-3.0.0b2/retentioneering/eventstream/__init__.py
+-rw-r--r--   0        0        0    42992 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/eventstream/eventstream.py
+-rw-r--r--   0        0        0      792 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/eventstream/helpers/__init__.py
+-rw-r--r--   0        0        0     1476 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/eventstream/helpers/add_negative_events_helper.py
+-rw-r--r--   0        0        0     1475 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/eventstream/helpers/add_positive_events_helper.py
+-rw-r--r--   0        0        0     1129 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/eventstream/helpers/add_start_end_events_helper.py
+-rw-r--r--   0        0        0     1539 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/eventstream/helpers/collapse_loops_helper.py
+-rw-r--r--   0        0        0     1373 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/eventstream/helpers/drop_paths_helper.py
+-rw-r--r--   0        0        0     1239 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/eventstream/helpers/filter_events_helper.py
+-rw-r--r--   0        0        0     1556 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/eventstream/helpers/group_events_helper.py
+-rw-r--r--   0        0        0     1557 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/eventstream/helpers/label_cropped_paths_helper.py
+-rw-r--r--   0        0        0     1513 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/eventstream/helpers/label_lost_users_helper.py
+-rw-r--r--   0        0        0     1336 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/eventstream/helpers/label_new_users_helper.py
+-rw-r--r--   0        0        0      781 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/eventstream/helpers/rename_helper.py
+-rw-r--r--   0        0        0     1946 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/eventstream/helpers/split_sessions_helper.py
+-rw-r--r--   0        0        0     1803 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/eventstream/helpers/truncate_paths_helper.py
+-rw-r--r--   0        0        0     4157 2023-04-03 06:56:53.879061 retentioneering-3.0.0b2/retentioneering/eventstream/schema.py
+-rw-r--r--   0        0        0     2389 2023-04-03 06:56:53.879061 retentioneering-3.0.0b2/retentioneering/eventstream/types.py
+-rw-r--r--   0        0        0        0 2023-01-16 14:26:06.557745 retentioneering-3.0.0b2/retentioneering/exceptions/__init__.py
+-rw-r--r--   0        0        0       45 2023-01-16 14:26:06.557745 retentioneering-3.0.0b2/retentioneering/exceptions/base.py
+-rw-r--r--   0        0        0     1242 2023-03-22 12:39:29.884664 retentioneering-3.0.0b2/retentioneering/exceptions/server.py
+-rw-r--r--   0        0        0      306 2023-03-07 11:03:25.191505 retentioneering-3.0.0b2/retentioneering/exceptions/widget.py
+-rw-r--r--   0        0        0       31 2023-01-16 14:26:06.557745 retentioneering-3.0.0b2/retentioneering/nodelist/__init__.py
+-rw-r--r--   0        0        0     1071 2023-04-03 06:56:53.879061 retentioneering-3.0.0b2/retentioneering/nodelist/nodelist.py
+-rw-r--r--   0        0        0       38 2023-01-16 14:26:06.557745 retentioneering-3.0.0b2/retentioneering/params_model/__init__.py
+-rw-r--r--   0        0        0    11842 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/params_model/params_model.py
+-rw-r--r--   0        0        0      952 2023-03-07 11:03:25.191505 retentioneering-3.0.0b2/retentioneering/params_model/registry.py
+-rw-r--r--   0        0        0      105 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/preprocessing_graph/__init__.py
+-rw-r--r--   0        0        0     4223 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/preprocessing_graph/nodes.py
+-rw-r--r--   0        0        0    14182 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/preprocessing_graph/preprocessing_graph.py
+-rw-r--r--   0        0        0        0 2023-01-16 14:26:06.557745 retentioneering-3.0.0b2/retentioneering/preprocessor/__init__.py
+-rw-r--r--   0        0        0       65 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/templates/__init__.py
+-rw-r--r--   0        0        0       45 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/templates/preprocessing_graph/__init__.py
+-rw-r--r--   0        0        0     1704 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/templates/preprocessing_graph/preprocessing_graph.html
+-rw-r--r--   0        0        0      736 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/templates/preprocessing_graph/show.py
+-rw-r--r--   0        0        0       42 2023-01-16 14:26:06.557745 retentioneering-3.0.0b2/retentioneering/templates/transition_graph/__init__.py
+-rw-r--r--   0        0        0       22 2023-01-16 14:26:06.557745 retentioneering-3.0.0b2/retentioneering/templates/transition_graph/body.html
+-rw-r--r--   0        0        0      713 2023-01-16 14:26:06.557745 retentioneering-3.0.0b2/retentioneering/templates/transition_graph/full.html
+-rw-r--r--   0        0        0      894 2023-04-17 15:56:16.596442 retentioneering-3.0.0b2/retentioneering/templates/transition_graph/init_template.py
+-rw-r--r--   0        0        0     1507 2023-01-16 14:26:06.557745 retentioneering-3.0.0b2/retentioneering/templates/transition_graph/inner_iframe.html
+-rw-r--r--   0        0        0     1143 2023-01-16 14:26:06.557745 retentioneering-3.0.0b2/retentioneering/templates/transition_graph/show.py
+-rw-r--r--   0        0        0      382 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/tooling/__init__.py
+-rw-r--r--   0        0        0       33 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/tooling/_describe/__init__.py
+-rw-r--r--   0        0        0     4543 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/tooling/_describe/_describe.py
+-rw-r--r--   0        0        0       46 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/tooling/_describe_events/__init__.py
+-rw-r--r--   0        0        0     4750 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/tooling/_describe_events/_describe_events.py
+-rw-r--r--   0        0        0       50 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/tooling/_transition_matrix/__init__.py
+-rw-r--r--   0        0        0     1319 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/tooling/_transition_matrix/_transition_matrix.py
+-rw-r--r--   0        0        0       31 2023-01-16 14:26:06.557745 retentioneering-3.0.0b2/retentioneering/tooling/clusters/__init__.py
+-rw-r--r--   0        0        0    33471 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/tooling/clusters/clusters.py
+-rw-r--r--   0        0        0     2039 2023-01-16 14:26:06.557745 retentioneering-3.0.0b2/retentioneering/tooling/clusters/segments.py
+-rw-r--r--   0        0        0     3166 2023-01-16 14:26:06.557745 retentioneering-3.0.0b2/retentioneering/tooling/clusters/userlist.py
+-rw-r--r--   0        0        0       29 2023-01-16 14:26:06.557745 retentioneering-3.0.0b2/retentioneering/tooling/cohorts/__init__.py
+-rw-r--r--   0        0        0    13160 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/tooling/cohorts/cohorts.py
+-rw-r--r--   0        0        0       39 2023-03-07 11:03:25.191505 retentioneering-3.0.0b2/retentioneering/tooling/constants/__init__.py
+-rw-r--r--   0        0        0      240 2023-03-07 11:03:25.191505 retentioneering-3.0.0b2/retentioneering/tooling/constants/constants.py
+-rw-r--r--   0        0        0       53 2023-01-16 14:26:06.557745 retentioneering-3.0.0b2/retentioneering/tooling/event_timestamp_hist/__init__.py
+-rw-r--r--   0        0        0     5596 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/tooling/event_timestamp_hist/event_timestamp_hist.py
+-rw-r--r--   0        0        0       27 2023-01-16 14:26:06.561078 retentioneering-3.0.0b2/retentioneering/tooling/funnel/__init__.py
+-rw-r--r--   0        0        0    12195 2023-04-03 06:56:53.882394 retentioneering-3.0.0b2/retentioneering/tooling/funnel/funnel.py
+-rw-r--r--   0        0        0       43 2023-03-07 11:03:25.191505 retentioneering-3.0.0b2/retentioneering/tooling/mixins/__init__.py
+-rw-r--r--   0        0        0     1516 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/tooling/mixins/ended_events.py
+-rw-r--r--   0        0        0       71 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/tooling/stattests/__init__.py
+-rw-r--r--   0        0        0      171 2023-04-17 15:56:20.809770 retentioneering-3.0.0b2/retentioneering/tooling/stattests/constants.py
+-rw-r--r--   0        0        0    11923 2023-04-17 15:56:20.813103 retentioneering-3.0.0b2/retentioneering/tooling/stattests/stattests.py
+-rw-r--r--   0        0        0       36 2023-01-16 14:26:06.561078 retentioneering-3.0.0b2/retentioneering/tooling/step_matrix/__init__.py
+-rw-r--r--   0        0        0    21738 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/tooling/step_matrix/step_matrix.py
+-rw-r--r--   0        0        0       36 2023-01-16 14:26:06.561078 retentioneering-3.0.0b2/retentioneering/tooling/step_sankey/__init__.py
+-rw-r--r--   0        0        0    24641 2023-04-17 15:56:20.813103 retentioneering-3.0.0b2/retentioneering/tooling/step_sankey/step_sankey.py
+-rw-r--r--   0        0        0      110 2023-03-07 11:03:25.191505 retentioneering-3.0.0b2/retentioneering/tooling/timedelta_hist/__init__.py
+-rw-r--r--   0        0        0      186 2023-03-07 11:03:25.191505 retentioneering-3.0.0b2/retentioneering/tooling/timedelta_hist/constants.py
+-rw-r--r--   0        0        0    13318 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/tooling/timedelta_hist/timedelta_hist.py
+-rw-r--r--   0        0        0       46 2023-04-03 06:56:53.882394 retentioneering-3.0.0b2/retentioneering/tooling/transition_graph/__init__.py
+-rw-r--r--   0        0        0    35854 2023-04-17 15:56:20.813103 retentioneering-3.0.0b2/retentioneering/tooling/transition_graph/transition_graph.py
+-rw-r--r--   0        0        0        0 2023-03-07 11:03:25.191505 retentioneering-3.0.0b2/retentioneering/tooling/typing/__init__.py
+-rw-r--r--   0        0        0      171 2023-03-07 11:03:25.191505 retentioneering-3.0.0b2/retentioneering/tooling/typing/transition_graph/__init__.py
+-rw-r--r--   0        0        0     1327 2023-04-03 06:56:53.882394 retentioneering-3.0.0b2/retentioneering/tooling/typing/transition_graph/graph_types.py
+-rw-r--r--   0        0        0       49 2023-01-16 14:26:06.561078 retentioneering-3.0.0b2/retentioneering/tooling/user_lifetime_hist/__init__.py
+-rw-r--r--   0        0        0     6555 2023-04-19 10:56:35.553951 retentioneering-3.0.0b2/retentioneering/tooling/user_lifetime_hist/user_lifetime_hist.py
+-rw-r--r--   0        0        0      458 2023-01-16 14:26:06.561078 retentioneering-3.0.0b2/retentioneering/utils/__init__.py
+-rw-r--r--   0        0        0      122 2023-03-07 11:03:25.191505 retentioneering-3.0.0b2/retentioneering/utils/dict.py
+-rw-r--r--   0        0        0      465 2023-01-16 14:26:06.561078 retentioneering-3.0.0b2/retentioneering/utils/list.py
+-rw-r--r--   0        0        0      444 2023-01-16 14:26:06.561078 retentioneering-3.0.0b2/retentioneering/utils/pandas.py
+-rw-r--r--   0        0        0      986 2023-03-07 11:03:25.191505 retentioneering-3.0.0b2/retentioneering/utils/registry.py
+-rw-r--r--   0        0        0      269 2023-01-16 14:26:06.561078 retentioneering-3.0.0b2/retentioneering/utils/singleton.py
+-rw-r--r--   0        0        0       77 2023-03-07 11:03:25.191505 retentioneering-3.0.0b2/retentioneering/widget/__init__.py
+-rw-r--r--   0        0        0     7265 2023-03-22 12:39:29.887997 retentioneering-3.0.0b2/retentioneering/widget/widgets.py
+-rw-r--r--   0        0        0      988 1970-01-01 00:00:00.000000 retentioneering-3.0.0b2/PKG-INFO
```

### Comparing `retentioneering-3.0.0b1/LICENSE` & `retentioneering-3.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b1/pyproject.toml` & `retentioneering-3.0.0b2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 [tool.poetry]
 name = "retentioneering"
-version = "3.0.0b1"
-license = "Retentioneering Software Non-Exclusive License (License)"
-description = "Product analytics and marketing optimization framework based on deep user trajectories analysis"
-authors = ["Retentioneering User Trajectory Analysis Lab <retentioneering@gmail.com>"]
-repository = "https://github.com/retentioneering/retentioneering-tools"
+version = "3.0.0b2"
+description = "universal framework for data processing"
+authors = ["Retentioneering User Trajectory Analysis Lab <you@example.com>"]
 packages = [
     { include = "retentioneering"}
 ]
 
 [[tool.poetry.source]]
 name = "main"
 url = "https://pypi.python.org/simple"
@@ -24,22 +22,25 @@
 pydantic = "^1.10.2"
 networkx = "^2.8.6"
 plotly = "^5.10.0"
 seaborn = "^0.12.1"
 umap-learn = "^0.5.3"
 statsmodels = "^0.13.5"
 scipy = ">=1.3,<1.9"
+ipywidgets = "8.0.4"
 
 [tool.poetry.dev-dependencies]
 pre-commit = "^2.20.0"
 poetry = "^1.2.1"
 pytest = "^7.1.3"
 tox-poetry = "^0.4.1"
 mypy = "^0.971"
 
+[tool.poetry.group.dev.dependencies]
+types-requests = "^2.28.11.16"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
```

### Comparing `retentioneering-3.0.0b1/retentioneering/backend/callback/mock_list_dataprocessor.py` & `retentioneering-3.0.0b2/retentioneering/backend/callback/mock_list_dataprocessor.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
             {
                 "name": "full_collapse",
                 "widget": "bool",
                 "default": True,
                 "optional": False,
             },
             {
-                "name": "timestamp_aggregation_type",
+                "name": "time_agg",
                 "widget": "enum",
                 "default": "max",
                 "optional": False,
                 "params": ["max", "min", "mean"],
             },
         ],
     },
@@ -58,18 +58,18 @@
                 "name": "min_cjm",
                 "widget": "int",
                 "optional": False,
             },
         ],
     },
     {
-        "name": "LostUsersEvents",
+        "name": "LabelLostUsers",
         "params": [
             {
-                "name": "lost_cutoff",
+                "name": "timeout",
                 "widget": "tuple",
                 "optional": True,
                 "params": [
                     {
                         "widget": "float",
                     },
                     {
@@ -82,58 +82,58 @@
                 "name": "lost_users_list",
                 "widget": "list_of_string",
                 "optional": True,
             },
         ],
     },
     {
-        "name": "NegativeTarget",
+        "name": "AddNegativeEvents",
         "params": [
             {
-                "name": "negative_target_events",
+                "name": "targets",
                 "widget": "list_of_string",
                 "optional": False,
             },
             {
                 "name": "negative_function",
                 "widget": "callable",
                 "optional": True,
             },
         ],
     },
     {
-        "name": "NewUsersEvents",
+        "name": "LabelNewUsers",
         "params": [
             {
                 "name": "new_users_list",
                 "widget": "list_of_string",
                 "optional": False,
             },
         ],
     },
     {
-        "name": "PositiveTarget",
+        "name": "AddPositiveEvents",
         "params": [
             {
-                "name": "positive_target_events",
+                "name": "targets",
                 "widget": "list_of_string",
                 "optional": False,
             },
             {
                 "name": "positive_function",
                 "widget": "callable",
                 "optional": False,
             },
         ],
     },
     {
         "name": "SplitSessions",
         "params": [
             {
-                "name": "session_cutoff",
+                "name": "timeout",
                 "widget": "tuple",
                 "optional": False,
                 "params": [
                     {
                         "widget": "float",
                     },
                     {
@@ -151,36 +151,36 @@
                 "name": "session_col",
                 "widget": "string",
                 "optional": True,
             },
         ],
     },
     {
-        "name": "StartEndEvents",
+        "name": "AddStartEndEvents",
         "params": [],
     },
     {
-        "name": "TruncatedEvents",
+        "name": "LabelCroppedPaths",
         "params": [
             {
-                "name": "left_truncated_cutoff",
+                "name": "left_cutoff",
                 "widget": "tuple",
                 "optional": False,
                 "params": [
                     {
                         "widget": "float",
                     },
                     {
                         "widget": "enum",
                         "params": ["Y", "M", "W", "D", "h", "m", "s", "ms", "us", "μs", "ns", "ps", "fs", "as"],
                     },
                 ],
             },
             {
-                "name": "right_truncated_cutoff",
+                "name": "right_cutoff",
                 "widget": "tuple",
                 "optional": False,
                 "params": [
                     {
                         "widget": "float",
                     },
                     {
```

### Comparing `retentioneering-3.0.0b1/retentioneering/backend/jupiter_server.py` & `retentioneering-3.0.0b2/retentioneering/backend/jupiter_server.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b1/retentioneering/backend/server_manager.py` & `retentioneering-3.0.0b2/retentioneering/backend/server_manager.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b1/retentioneering/data_processor/data_processor.py` & `retentioneering-3.0.0b2/retentioneering/data_processor/data_processor.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b1/retentioneering/data_processor/registry.py` & `retentioneering-3.0.0b2/retentioneering/data_processor/registry.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b1/retentioneering/data_processors_lib/__init__.py` & `retentioneering-3.0.0b2/retentioneering/data_processors_lib/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,13 @@
+from .add_negative_events import AddNegativeEvents, AddNegativeEventsParams
+from .add_positive_events import AddPositiveEvents, AddPositiveEventsParams
+from .add_start_end_events import AddStartEndEvents, AddStartEndEventsParams
 from .collapse_loops import CollapseLoops, CollapseLoopsParams
-from .delete_users_by_path_length import (
-    DeleteUsersByPathLength,
-    DeleteUsersByPathLengthParams,
-)
+from .drop_paths import DropPaths, DropPathsParams
 from .filter_events import FilterEvents, FilterEventsParams
 from .group_events import GroupEvents, GroupEventsParams
-from .lost_users import LostUsersEvents, LostUsersParams
-from .negative_target import NegativeTarget, NegativeTargetParams
-from .new_users import NewUsersEvents, NewUsersParams
-from .positive_target import PositiveTarget, PositiveTargetParams
+from .label_cropped_paths import LabelCroppedPaths, LabelCroppedPathsParams
+from .label_lost_users import LabelLostUsers, LabelLostUsersParams
+from .label_new_users import LabelNewUsers, LabelNewUsersParams
 from .rename import RenameParams, RenameProcessor
 from .split_sessions import SplitSessions, SplitSessionsParams
-from .start_end_events import StartEndEvents, StartEndEventsParams
-from .truncate_path import TruncatePath, TruncatePathParams
-from .truncated_events import TruncatedEvents, TruncatedEventsParams
+from .truncate_paths import TruncatePaths, TruncatePathsParams
```

### Comparing `retentioneering-3.0.0b1/retentioneering/data_processors_lib/collapse_loops.py` & `retentioneering-3.0.0b2/retentioneering/data_processors_lib/collapse_loops.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,39 +10,39 @@
 
 
 class CollapseLoopsParams(ParamsModel):
     """
     A class with parameters for :py:class:`.CollapseLoops` class.
     """
 
-    suffix: Optional[Literal["loop", "count"]] = "loop"
-    timestamp_aggregation_type: Literal["max", "min", "mean"] = "max"
+    suffix: Optional[Literal["loop", "count"]]
+    time_agg: Literal["max", "min", "mean"] = "max"
 
 
 class CollapseLoops(DataProcessor):
     """
     Find ``loops`` and create new synthetic events in the paths of all users having such sequences.
 
     A ``loop`` - is a sequence of repetitive events.
     For example *"event1 -> event1"*
 
     Parameters
     ----------
-    suffix : {"loop", "count", None}, default "loop"
+    suffix : {"loop", "count"}, optional
+
+        - If ``None``, event_name will be event_name without any changes.\n
+        For example *"event1 - event1 - event1"* --> event1.
 
         - If ``loop``, event_name will be event_name_loop.\n
         For example *"event1 - event1 - event1"* --> event1_loop.
 
         - If ``count``, event_name will be event_name_loop_{number of events}.\n
         For example *"event1 - event1 - event1"* --> event1_loop_3.
 
-        - If ``None``, event_name will be event_name without any changes.\n
-        For example *"event1 - event1 - event1"* --> event1.
-
-    timestamp_aggregation_type : {"max", "min", "mean"}, default "max"
+    time_agg : {"max", "min", "mean"}, default "max"
         Aggregation method to calculate timestamp values for new groups.
 
     Returns
     -------
     Eventstream
         Eventstream with:
 
@@ -79,29 +79,29 @@
 
         user_col = eventstream.schema.user_id
         time_col = eventstream.schema.event_timestamp
         type_col = eventstream.schema.event_type
         event_col = eventstream.schema.event_name
 
         suffix = self.params.suffix
-        timestamp_aggregation_type = self.params.timestamp_aggregation_type
+        time_agg = self.params.time_agg
         df = eventstream.to_dataframe(copy=True)
         df["ref"] = df[eventstream.schema.event_id]
 
         df["grp"] = df[event_col] != df.groupby(user_col)[event_col].shift(1)
         # Столбец в котором считается порядковый номер по группам одинаковых событий
         df["cumgroup"] = df.groupby(user_col)["grp"].cumsum()
         df["count"] = df.groupby([user_col, "cumgroup"]).cumcount() + 1
         df["collapsed"] = df.groupby([user_col, "cumgroup", event_col])["count"].transform(max)
         df["collapsed"] = df["collapsed"].apply(lambda x: False if x == 1 else True)
 
         loops = (
             df[df["collapsed"] == 1]
             .groupby([user_col, "cumgroup", event_col])
-            .agg({time_col: timestamp_aggregation_type, "count": "max"})
+            .agg({time_col: time_agg, "count": "max"})
             .reset_index()
         )
 
         if suffix == "loop":
             loops[event_col] = loops[event_col].map(str) + "_loop"
         elif suffix == "count":
             loops[event_col] = loops[event_col].map(str) + "_loop_" + loops["count"].map(str)
```

### Comparing `retentioneering-3.0.0b1/retentioneering/data_processors_lib/delete_users_by_path_length.py` & `retentioneering-3.0.0b2/retentioneering/data_processors_lib/drop_paths.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,96 +7,96 @@
 from retentioneering.constants import DATETIME_UNITS
 from retentioneering.data_processor import DataProcessor
 from retentioneering.eventstream.types import EventstreamType
 from retentioneering.params_model import ParamsModel
 from retentioneering.widget.widgets import ReteTimeWidget
 
 
-class DeleteUsersByPathLengthParams(ParamsModel):
+class DropPathsParams(ParamsModel):
     """
-    A class with parameters for :py:class:`.DeleteUsersByPathLength` class.
+    A class with parameters for :py:class:`.DropPaths` class.
     """
 
-    events_num: Optional[int]
-    cutoff: Optional[Tuple[float, DATETIME_UNITS]]
+    min_steps: Optional[int]
+    min_time: Optional[Tuple[float, DATETIME_UNITS]]
 
     _widgets = {
-        "cutoff": ReteTimeWidget(),
+        "min_time": ReteTimeWidget(),
     }
 
 
-class DeleteUsersByPathLength(DataProcessor):
+class DropPaths(DataProcessor):
     """
     Filter user paths based on the path length, removing the paths that are shorter than the
-    specified number of events or cut_off.
+    specified number of events or time.
 
     Parameters
     ----------
-    events_num : int, optional
-        Minimum user path length
+    min_steps : int, optional
+        Minimum user path length measured in the number of events.
 
-    cutoff : Tuple(float, :numpy_link:`DATETIME_UNITS<>`), optional
+    min_time : Tuple(float, :numpy_link:`DATETIME_UNITS<>`), optional
         Minimum user path length and its unit of measure.
 
     Returns
     -------
     Eventstream
         ``Eventstream`` with events that should be deleted from input ``eventstream`` marked ``_deleted=True``.
 
     Raises
     ------
     ValueError
-        If both of ``events_num`` and ``cutoff`` are empty or both are given.
+        If both of ``min_steps`` and ``min_time`` are empty or both are given.
 
     See Also
     --------
     .TimedeltaHist : Plot the distribution of the time deltas between two events.
     .UserLifetimeHist : Plot the distribution of user lifetimes.
 
     Notes
     -----
     See :doc:`Data processors user guide</user_guides/dataprocessors>` for the details.
     """
 
-    params: DeleteUsersByPathLengthParams
+    params: DropPathsParams
 
-    def __init__(self, params: DeleteUsersByPathLengthParams):
+    def __init__(self, params: DropPathsParams):
         super().__init__(params=params)
 
     def apply(self, eventstream: EventstreamType) -> EventstreamType:
         from retentioneering.eventstream.eventstream import Eventstream
 
         user_col = eventstream.schema.user_id
         time_col = eventstream.schema.event_timestamp
 
-        cutoff, cutoff_unit = None, None
-        events_num = self.params.events_num
+        min_time, time_unit = None, None
+        min_steps = self.params.min_steps
 
-        if self.params.cutoff:
-            cutoff, cutoff_unit = self.params.cutoff
+        if self.params.min_time:
+            min_time, time_unit = self.params.min_time
 
-        if events_num and cutoff:
-            raise ValueError("Events_num and cutoff parameters cannot be used simultaneously!")
+        if min_steps and min_time:
+            raise ValueError("min_steps and min_time parameters cannot be used simultaneously!")
 
-        if not events_num and not cutoff:
-            raise ValueError("Either events_num or cutoff must be specified!")
+        if not min_steps and not min_time:
+            raise ValueError("Either min_steps or min_time must be specified!")
 
         events = eventstream.to_dataframe(copy=True)
 
-        if cutoff and cutoff_unit:
+        if min_time and time_unit:
             userpath = (
                 events.groupby(user_col)[time_col]
                 .agg([np.min, np.max])
                 .rename(columns={"amin": "start", "amax": "end"})
             )
-            mask_ = (userpath["end"] - userpath["start"]) / np.timedelta64(1, cutoff_unit) < cutoff  # type: ignore
+            mask_ = (userpath["end"] - userpath["start"]) / np.timedelta64(1, time_unit) < min_time  # type: ignore
 
         else:
             userpath = events.groupby([user_col])[[time_col]].nunique().rename(columns={time_col: "length"})
-            mask_ = userpath["length"] < events_num
+            mask_ = userpath["length"] < min_steps
 
         users_to_delete = userpath[mask_].index
         events = events[events[user_col].isin(users_to_delete)]
         events["ref"] = events.loc[:, eventstream.schema.event_id]
 
         eventstream = Eventstream(
             raw_data_schema=eventstream.schema.to_raw_data_schema(),
```

### Comparing `retentioneering-3.0.0b1/retentioneering/data_processors_lib/filter_events.py` & `retentioneering-3.0.0b2/retentioneering/data_processors_lib/filter_events.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b1/retentioneering/data_processors_lib/group_events.py` & `retentioneering-3.0.0b2/retentioneering/data_processors_lib/group_events.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b1/retentioneering/data_processors_lib/lost_users.py` & `retentioneering-3.0.0b2/retentioneering/data_processors_lib/label_lost_users.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,41 +8,41 @@
 from retentioneering.constants import DATETIME_UNITS
 from retentioneering.data_processor import DataProcessor
 from retentioneering.eventstream.types import EventstreamType
 from retentioneering.params_model import ParamsModel
 from retentioneering.widget.widgets import ListOfInt, ReteTimeWidget
 
 
-class LostUsersParams(ParamsModel):
+class LabelLostUsersParams(ParamsModel):
     """
-    A class with parameters for :py:class:`.LostUsersEvents` class.
+    A class with parameters for :py:class:`.LabelLostUsers` class.
     """
 
-    lost_cutoff: Optional[Tuple[float, DATETIME_UNITS]]
+    timeout: Optional[Tuple[float, DATETIME_UNITS]]
     lost_users_list: Optional[Union[List[int], List[str]]]
 
     _widgets = {
-        "lost_cutoff": ReteTimeWidget(),
+        "timeout": ReteTimeWidget(),
         "lost_users_list": ListOfInt(),
     }
 
 
-class LostUsersEvents(DataProcessor):
+class LabelLostUsers(DataProcessor):
     """
     Create one of synthetic events in each user's path:
     ``lost_user`` or ``absent_user``.
 
 
     Parameters
     ----------
     Only one of parameters could be used at the same time
-    lost_cutoff : Tuple(float, :numpy_link:`DATETIME_UNITS<>`), optional
+    timeout : Tuple(float, :numpy_link:`DATETIME_UNITS<>`), optional
         Threshold value and its unit of measure.
         Calculate timedelta between the last event in each user's path and the last event in the whole eventstream.
-        For users with timedelta greater or equal to selected ``lost_cutoff``, a new synthetic event - ``lost_user``
+        For users with timedelta greater or equal to selected ``timeout``, a new synthetic event - ``lost_user``
         will be added.
         For other users paths a new synthetic event - ``absent_user`` will be added.
 
     lost_users_list : list of int or list of str, optional
         If the `list of user_ids` is given new synthetic event - ``lost_user`` will be added to each user from the list.
         For other user's paths will be added new synthetic event - ``absent_user``.
 
@@ -58,56 +58,56 @@
         +-----------------+-----------------+------------------+
         | absent_user     | absent_user     | last_event       |
         +-----------------+-----------------+------------------+
 
     Raises
     ------
     ValueError
-        Raised when both ``lost_cutoff`` and ``lost_users_list`` are either empty or given.
+        Raised when both ``timeout`` and ``lost_users_list`` are either empty or given.
 
     Notes
     -----
     See :doc:`Data processors user guide</user_guides/dataprocessors>` for the details.
     """
 
-    params: LostUsersParams
+    params: LabelLostUsersParams
 
-    def __init__(self, params: LostUsersParams):
+    def __init__(self, params: LabelLostUsersParams):
         super().__init__(params=params)
 
     def apply(self, eventstream: EventstreamType) -> EventstreamType:
         from retentioneering.eventstream.eventstream import Eventstream
 
         user_col = eventstream.schema.user_id
         time_col = eventstream.schema.event_timestamp
         type_col = eventstream.schema.event_type
         event_col = eventstream.schema.event_name
 
-        lost_cutoff, lost_cutoff_unit = None, None
+        timeout, timeout_unit = None, None
         lost_users_list = self.params.lost_users_list
         data_lost = pd.DataFrame()
 
-        if self.params.lost_cutoff:
-            lost_cutoff, lost_cutoff_unit = self.params.lost_cutoff
+        if self.params.timeout:
+            timeout, timeout_unit = self.params.timeout
 
-        if lost_cutoff and lost_users_list:
-            raise ValueError("lost_cutoff and lost_users_list parameters cannot be used simultaneously!")
+        if timeout and lost_users_list:
+            raise ValueError("timeout and lost_users_list parameters cannot be used simultaneously!")
 
-        if not lost_cutoff and not lost_users_list:
-            raise ValueError("Either lost_cutoff or lost_users_list must be specified!")
+        if not timeout and not lost_users_list:
+            raise ValueError("Either timeout or lost_users_list must be specified!")
 
         df = eventstream.to_dataframe(copy=True)
 
-        if lost_cutoff and lost_cutoff_unit:
+        if timeout and timeout_unit:
             data_lost = df.groupby(user_col, as_index=False).last()
             data_lost["diff_end_to_end"] = data_lost[time_col].max() - data_lost[time_col]
 
-            data_lost["diff_end_to_end"] /= np.timedelta64(1, lost_cutoff_unit)  # type: ignore
+            data_lost["diff_end_to_end"] /= np.timedelta64(1, timeout_unit)  # type: ignore
 
-            data_lost[type_col] = np.where(data_lost["diff_end_to_end"] < lost_cutoff, "absent_user", "lost_user")
+            data_lost[type_col] = np.where(data_lost["diff_end_to_end"] < timeout, "absent_user", "lost_user")
             data_lost[event_col] = data_lost[type_col]
             data_lost["ref"] = None
             del data_lost["diff_end_to_end"]
 
         if lost_users_list:
             data_lost = df.groupby(user_col, as_index=False).last()
             data_lost[type_col] = np.where(data_lost["user_id"].isin(lost_users_list), "lost_user", "absent_user")
```

### Comparing `retentioneering-3.0.0b1/retentioneering/data_processors_lib/negative_target.py` & `retentioneering-3.0.0b2/retentioneering/data_processors_lib/add_negative_events.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,103 +9,101 @@
 from retentioneering.eventstream.types import EventstreamType
 from retentioneering.params_model import ParamsModel
 from retentioneering.widget.widgets import ListOfString, ReteFunction
 
 EventstreamFilter = Callable[[pd.DataFrame, EventstreamSchema], Any]
 
 
-def _default_func(eventstream: EventstreamType, negative_target_events: List[str]) -> pd.DataFrame:
+def _default_func(eventstream: EventstreamType, targets: List[str]) -> pd.DataFrame:
     """
-    Filters rows with target events from the input eventstream.
+    Filter rows with target events from the input eventstream.
 
     Parameters
     ----------
     eventstream : Eventstream
         Source eventstream or output from previous nodes.
 
-    negative_target_events : list of str
+    targets : list of str
         Each event from that list is associated with the bad result (scenario)
         of user's behaviour (experience) in the product.
         If there are several target events in user path - the event with minimum timestamp is taken.
 
     Returns
     -------
     pd.DataFrame
-        Filtered DataFrame with negative_target_events and its timestamps.
+        Filtered DataFrame with targets and its timestamps.
     """
     user_col = eventstream.schema.user_id
     time_col = eventstream.schema.event_timestamp
     event_col = eventstream.schema.event_name
     df = eventstream.to_dataframe()
 
-    negative_events_index = (
-        df[df[event_col].isin(negative_target_events)].groupby(user_col)[time_col].idxmin()  # type: ignore
-    )
+    targets_index = df[df[event_col].isin(targets)].groupby(user_col)[time_col].idxmin()  # type: ignore
 
-    return df.loc[negative_events_index]  # type: ignore
+    return df.loc[targets_index]  # type: ignore
 
 
-class NegativeTargetParams(ParamsModel):
+class AddNegativeEventsParams(ParamsModel):
     """
-    A class with parameters for :py:class:`.NegativeTarget` class.
+    A class with parameters for :py:class:`.AddNegativeEvents` class.
     """
 
-    negative_target_events: List[str]
+    targets: List[str]
     func: Callable = _default_func
 
-    _widgets = {"func": ReteFunction(), "negative_target_events": ListOfString()}
+    _widgets = {"func": ReteFunction(), "targets": ListOfString()}
 
 
-class NegativeTarget(DataProcessor):
+class AddNegativeEvents(DataProcessor):
     """
     Create new synthetic events in paths of all users having the specified event(s):
     ``negative_target_RAW_EVENT_NAME``.
 
     Parameters
     ----------
-    negative_target_events : list of str
+    targets : list of str
         Define the list of events that we consider negative.
         If there are several target events in the user path, the event with the minimum timestamp is taken.
 
     func : Callable, default _default_func_negative
         Filter rows with target events from the input eventstream.
 
     Returns
     -------
     Eventstream
         ``Eventstream`` with new synthetic events only added to the users who fit the conditions.
 
         +--------------------------------+-----------------+-----------------------------+
         | **event_name**                 | **event_type**  | **timestamp**               |
         +--------------------------------+-----------------+-----------------------------+
-        | negative_target_RAW_EVENT_NAME | negative_target | min(negative_target_events) |
+        | negative_target_RAW_EVENT_NAME | negative_target | min(targets)                |
         +--------------------------------+-----------------+-----------------------------+
 
     Notes
     -----
     See :doc:`Data processors user guide</user_guides/dataprocessors>` for the details.
 
 
     """
 
-    params: NegativeTargetParams
+    params: AddNegativeEventsParams
 
-    def __init__(self, params: NegativeTargetParams):
+    def __init__(self, params: AddNegativeEventsParams):
         super().__init__(params=params)
 
     def apply(self, eventstream: EventstreamType) -> EventstreamType:
         from retentioneering.eventstream.eventstream import Eventstream
 
         type_col = eventstream.schema.event_type
         event_col = eventstream.schema.event_name
 
         func = self.params.func
-        negative_target_events = self.params.negative_target_events
+        targets = self.params.targets
 
-        negative_targets = func(eventstream, negative_target_events)
+        negative_targets = func(eventstream, targets)
         negative_targets[type_col] = "negative_target"
         negative_targets[event_col] = "negative_target_" + negative_targets[event_col]
         negative_targets["ref"] = None
 
         eventstream = Eventstream(
             raw_data_schema=eventstream.schema.to_raw_data_schema(),
             raw_data=negative_targets,
```

### Comparing `retentioneering-3.0.0b1/retentioneering/data_processors_lib/new_users.py` & `retentioneering-3.0.0b2/retentioneering/data_processors_lib/label_new_users.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 
 from retentioneering.data_processor import DataProcessor
 from retentioneering.eventstream.types import EventstreamType
 from retentioneering.params_model import ParamsModel
 from retentioneering.widget.widgets import ListOfIntNewUsers
 
 
-class NewUsersParams(ParamsModel):
+class LabelNewUsersParams(ParamsModel):
     """
-    A class with parameters for :py:class:`.NewUsersEvents` class.
+    A class with parameters for :py:class:`.LabelNewUsers` class.
     """
 
     new_users_list: Union[List[int], List[str], Literal["all"]]
     _widgets = {"new_users_list": ListOfIntNewUsers()}
 
 
-class NewUsersEvents(DataProcessor):
+class LabelNewUsers(DataProcessor):
     """
     Create a new synthetic event for each user:
     ``new_user`` or ``existing_user``.
 
     Parameters
     ----------
     new_users_list : list of int or list of str or `all`
@@ -48,17 +48,17 @@
 
     Notes
     -----
     See :doc:`Data processors user guide</user_guides/dataprocessors>` for the details.
 
     """
 
-    params: NewUsersParams
+    params: LabelNewUsersParams
 
-    def __init__(self, params: NewUsersParams):
+    def __init__(self, params: LabelNewUsersParams):
         super().__init__(params=params)
 
     def apply(self, eventstream: EventstreamType) -> EventstreamType:
         from retentioneering.eventstream.eventstream import Eventstream
 
         events: DataFrame = eventstream.to_dataframe(copy=True)
         user_col = eventstream.schema.user_id
```

### Comparing `retentioneering-3.0.0b1/retentioneering/data_processors_lib/positive_target.py` & `retentioneering-3.0.0b2/retentioneering/data_processors_lib/add_positive_events.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,101 +6,99 @@
 
 from retentioneering.data_processor import DataProcessor
 from retentioneering.eventstream.types import EventstreamType
 from retentioneering.params_model import ParamsModel
 from retentioneering.widget.widgets import ListOfString, ReteFunction
 
 
-def _default_func(eventstream: EventstreamType, positive_target_events: list[str]) -> pd.DataFrame:
+def _default_func(eventstream: EventstreamType, targets: list[str]) -> pd.DataFrame:
     """
-    Filters rows with target events from the input eventstream.
+    Filter rows with target events from the input eventstream.
 
     Parameters
     ----------
     eventstream : Eventstream
         Source eventstream or output from previous nodes.
 
-    positive_target_events : list of str
+    targets : list of str
         Condition for eventstream filtering.
         Each event from that list is associated with a conversion goal of the user behaviour in the product.
         If there are several target events in user path - the event with minimum timestamp is taken.
 
     Returns
     -------
     pd.DataFrame
-        Filtered DataFrame with positive_target_events and its timestamps.
+        Filtered DataFrame with targets and its timestamps.
     """
     user_col = eventstream.schema.user_id
     time_col = eventstream.schema.event_timestamp
     event_col = eventstream.schema.event_name
     df = eventstream.to_dataframe()
 
-    positive_events_index = (
-        df[df[event_col].isin(positive_target_events)].groupby(user_col)[time_col].idxmin()  # type: ignore
-    )
+    targets_index = df[df[event_col].isin(targets)].groupby(user_col)[time_col].idxmin()  # type: ignore
 
-    return df.loc[positive_events_index]  # type: ignore
+    return df.loc[targets_index]  # type: ignore
 
 
-class PositiveTargetParams(ParamsModel):
+class AddPositiveEventsParams(ParamsModel):
     """
-    A class with parameters for :py:class:`.PositiveTarget` class.
+    A class with parameters for :py:class:`.AddPositiveEvents` class.
     """
 
-    positive_target_events: List[str]
+    targets: List[str]
     func: Callable = _default_func
 
-    _widgets = {"func": ReteFunction(), "positive_target_events": ListOfString()}
+    _widgets = {"func": ReteFunction(), "targets": ListOfString()}
 
 
-class PositiveTarget(DataProcessor):
+class AddPositiveEvents(DataProcessor):
     """
     Create new synthetic events in paths of all users having the specified events:
     ``positive_target_RAW_EVENT_NAME``
 
     Parameters
     ----------
-    positive_target_events : list of str
+    targets : list of str
         Define the list of events we consider positive.
         If there are several target events in a user path, the event with the minimum timestamp is taken.
 
     func : Callable, default _default_func
         Filter rows with target events from the input eventstream.
 
     Returns
     -------
     Eventstream
         ``Eventstream`` with new synthetic events only added to users who fit the conditions.
 
         +--------------------------------+-----------------+-----------------------------+
         | **event_name**                 | **event_type**  | **timestamp**               |
         +--------------------------------+-----------------+-----------------------------+
-        | positive_target_RAW_EVENT_NAME | positive_target | min(positive_target_events) |
+        | positive_target_RAW_EVENT_NAME | positive_target | min(targets)                |
         +--------------------------------+-----------------+-----------------------------+
 
     Notes
     -----
     See :doc:`Data processors user guide</user_guides/dataprocessors>` for the details.
     """
 
-    params: PositiveTargetParams
+    params: AddPositiveEventsParams
 
-    def __init__(self, params: PositiveTargetParams):
+    def __init__(self, params: AddPositiveEventsParams):
         super().__init__(params=params)
 
     def apply(self, eventstream: EventstreamType) -> EventstreamType:
         from retentioneering.eventstream.eventstream import Eventstream
 
         type_col = eventstream.schema.event_type
         event_col = eventstream.schema.event_name
 
         func: Callable[[EventstreamType, list[str]], pd.DataFrame] = self.params.func
-        positive_target_events = self.params.positive_target_events
+        targets = self.params.targets
 
-        positive_targets = func(eventstream, positive_target_events)
+        positive_targets = func(eventstream, targets)
         positive_targets[type_col] = "positive_target"
         positive_targets[event_col] = "positive_target_" + positive_targets[event_col]
         positive_targets["ref"] = None
 
         eventstream = Eventstream(
             raw_data_schema=eventstream.schema.to_raw_data_schema(),
             raw_data=positive_targets,
```

### Comparing `retentioneering-3.0.0b1/retentioneering/data_processors_lib/rename.py` & `retentioneering-3.0.0b2/retentioneering/data_processors_lib/rename.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b1/retentioneering/data_processors_lib/split_sessions.py` & `retentioneering-3.0.0b2/retentioneering/data_processors_lib/split_sessions.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,48 +15,48 @@
 
 class SplitSessionsParams(ParamsModel):
     """
     A class with parameters for :py:class:`.SplitSessions` class.
 
     """
 
-    session_cutoff: Tuple[float, DATETIME_UNITS]
+    timeout: Tuple[float, DATETIME_UNITS]
     mark_truncated: bool = False
     session_col: str = "session_id"
 
-    _widgets = {"session_cutoff": ReteTimeWidget()}
+    _widgets = {"timeout": ReteTimeWidget()}
 
 
 class SplitSessions(DataProcessor):
     """
     Create new synthetic events, that divide users' paths on sessions:
-    ``session_start`` (or ``session_start_truncated``) and ``session_end`` (or ``session_end_truncated``).
+    ``session_start`` (or ``session_start_cropped``) and ``session_end`` (or ``session_end_cropped``).
     Also create a new column that contains session number for each event in input eventstream.
     Session number will take the form: ``{user_id}_{session_number through one user path}``.
 
     Parameters
     ----------
-    session_cutoff : Tuple(float, :numpy_link:`DATETIME_UNITS<>`)
+    timeout : Tuple(float, :numpy_link:`DATETIME_UNITS<>`)
         Threshold value and its unit of measure.
         ``session_start`` and ``session_end`` events are always placed before the first and after the last event
         in each user's path.
         Because user can have more than one session, it calculates timedelta between every two consecutive events in
         each user's path.
-        If the calculated timedelta is more than selected session_cutoff,
+        If the calculated timedelta is more than selected timeout,
         new synthetic events - ``session_start`` and ``session_end`` are created inside the user path,
         marking session starting and ending points.
 
     mark_truncated : bool, default False
         If ``True`` - calculates timedelta between:
 
         - first event in each user's path and first event in the whole eventstream.
         - last event in each user's path and last event in the whole eventstream.
 
-        For users with timedelta less than selected ``session_cutoff``,
-        a new synthetic event - ``session_start_truncated`` or ``session_end_truncated`` will be added.
+        For users with timedelta less than selected ``timeout``,
+        a new synthetic event - ``session_start_cropped`` or ``session_end_cropped`` will be added.
 
     session_col : str, default "session_id"
         The name of the ``session_col``.
 
     Returns
     -------
     Eventstream
@@ -65,21 +65,21 @@
         +-----------------------------+----------------------------+-----------------+
         | **event_name**              | **event_type**             | **timestamp**   |
         +-----------------------------+----------------------------+-----------------+
         | session_start               | session_start              | first_event     |
         +-----------------------------+----------------------------+-----------------+
         | session_end                 | session_end                | last_event      |
         +-----------------------------+----------------------------+-----------------+
-        | session_start_truncated     | session_start_truncated    | first_event     |
+        | session_start_cropped       | session_start_cropped      | first_event     |
         +-----------------------------+----------------------------+-----------------+
-        | session_end_truncated       | session_end_truncated      | last_event      |
+        | session_end_cropped         | session_end_cropped        | last_event      |
         +-----------------------------+----------------------------+-----------------+
 
         If the delta between timestamps of two consecutive events
-        (raw_event_n and raw_event_n+1) is greater than the selected ``session_cutoff``
+        (raw_event_n and raw_event_n+1) is greater than the selected ``timeout``
         the user will have more than one session:
 
         +--------------+-------------------+------------------+-------------------+------------------+
         |  **user_id** | **event_name**    | **event_type**   | **timestamp**     | **session_col**  |
         +--------------+-------------------+------------------+-------------------+------------------+
         |     1        | session_start     | session_start    | first_event       |     1_0          |
         +--------------+-------------------+------------------+-------------------+------------------+
@@ -112,27 +112,27 @@
         from retentioneering.eventstream.eventstream import Eventstream
 
         user_col = eventstream.schema.user_id
         time_col = eventstream.schema.event_timestamp
         type_col = eventstream.schema.event_type
         event_col = eventstream.schema.event_name
         session_col = self.params.session_col
-        session_cutoff, session_cutoff_unit = self.params.session_cutoff
+        timeout, timeout_unit = self.params.timeout
         mark_truncated = self.params.mark_truncated
 
         df = eventstream.to_dataframe(copy=True)
         df["ref"] = df[eventstream.schema.event_id]
 
         df["prev_timedelta"] = df[time_col] - df.groupby(user_col)[time_col].shift(1)
         df["next_timedelta"] = df.groupby(user_col)[time_col].shift(-1) - df[time_col]
-        df["prev_timedelta"] /= np.timedelta64(1, session_cutoff_unit)  # type: ignore
-        df["next_timedelta"] /= np.timedelta64(1, session_cutoff_unit)  # type: ignore
+        df["prev_timedelta"] /= np.timedelta64(1, timeout_unit)  # type: ignore
+        df["next_timedelta"] /= np.timedelta64(1, timeout_unit)  # type: ignore
 
-        session_starts_mask = (df["prev_timedelta"] > session_cutoff) | (df["prev_timedelta"].isnull())
-        session_ends_mask = (df["next_timedelta"] > session_cutoff) | (df["next_timedelta"].isnull())
+        session_starts_mask = (df["prev_timedelta"] > timeout) | (df["prev_timedelta"].isnull())
+        session_ends_mask = (df["next_timedelta"] > timeout) | (df["next_timedelta"].isnull())
 
         df["is_session_start"] = session_starts_mask
         df[session_col] = df.groupby(user_col)["is_session_start"].transform(np.cumsum)
         df[session_col] = df[user_col].astype(str) + "_" + df[session_col].astype(str)
 
         session_starts = df[session_starts_mask].copy()
         session_ends = df[session_ends_mask].copy()
@@ -146,25 +146,25 @@
         session_ends["ref"] = None
 
         df = df.drop(["prev_timedelta", "next_timedelta", "is_session_start"], axis=1)
 
         if mark_truncated:
             dataset_start = df[time_col].min()
             dataset_end = df[time_col].max()
-            start_to_start = (session_starts[time_col] - dataset_start) / np.timedelta64(1, session_cutoff_unit)
-            end_to_end = (dataset_end - session_ends[time_col]) / np.timedelta64(1, session_cutoff_unit)
+            start_to_start = (session_starts[time_col] - dataset_start) / np.timedelta64(1, timeout_unit)
+            end_to_end = (dataset_end - session_ends[time_col]) / np.timedelta64(1, timeout_unit)
 
-            session_starts_truncated = session_starts[start_to_start < session_cutoff].reset_index()
-            session_ends_truncated = session_ends[end_to_end < session_cutoff].reset_index()
+            session_starts_truncated = session_starts[start_to_start < timeout].reset_index()
+            session_ends_truncated = session_ends[end_to_end < timeout].reset_index()
 
-            session_starts_truncated[event_col] = "session_start_truncated"
-            session_starts_truncated[type_col] = "session_start_truncated"
+            session_starts_truncated[event_col] = "session_start_cropped"
+            session_starts_truncated[type_col] = "session_start_cropped"
 
-            session_ends_truncated[event_col] = "session_end_truncated"
-            session_ends_truncated[type_col] = "session_end_truncated"
+            session_ends_truncated[event_col] = "session_end_cropped"
+            session_ends_truncated[type_col] = "session_end_cropped"
 
             session_starts = pd.concat([session_starts, session_starts_truncated])
             session_ends = pd.concat([session_ends, session_ends_truncated])
 
         df = pd.concat([df, session_starts, session_ends])
 
         raw_data_schema = eventstream.schema.to_raw_data_schema()
```

### Comparing `retentioneering-3.0.0b1/retentioneering/data_processors_lib/start_end_events.py` & `retentioneering-3.0.0b2/retentioneering/data_processors_lib/add_start_end_events.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 from pandas import DataFrame
 
 from retentioneering.data_processor import DataProcessor
 from retentioneering.eventstream.types import EventstreamType
 from retentioneering.params_model import ParamsModel
 
 
-class StartEndEventsParams(ParamsModel):
+class AddStartEndEventsParams(ParamsModel):
     pass
 
 
-class StartEndEvents(DataProcessor):
+class AddStartEndEvents(DataProcessor):
     """
     Create two synthetic events in each user's path:
     ``path_start`` and ``path_end``.
 
     Returns
     -------
     Eventstream
@@ -31,17 +31,17 @@
         +----------------+----------------+----------------+
 
     Notes
     -----
     See :doc:`Data processors user guide</user_guides/dataprocessors>` for the details.
     """
 
-    params: StartEndEventsParams
+    params: AddStartEndEventsParams
 
-    def __init__(self, params: StartEndEventsParams) -> None:
+    def __init__(self, params: AddStartEndEventsParams) -> None:
         super().__init__(params=params)
 
     def apply(self, eventstream: EventstreamType) -> EventstreamType:
         from retentioneering.eventstream.eventstream import Eventstream
 
         events: DataFrame = eventstream.to_dataframe(copy=True)
         user_col = eventstream.schema.user_id
```

### Comparing `retentioneering-3.0.0b1/retentioneering/data_processors_lib/truncate_path.py` & `retentioneering-3.0.0b2/retentioneering/data_processors_lib/truncate_paths.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 import pandas as pd
 
 from retentioneering.data_processor import DataProcessor
 from retentioneering.eventstream.types import EventstreamType
 from retentioneering.params_model import ParamsModel
 
 
-class TruncatePathParams(ParamsModel):
+class TruncatePathsParams(ParamsModel):
     """
     A class with parameters for :py:class:`.TruncatePath` class.
     """
 
     drop_before: Optional[str]
     drop_after: Optional[str]
     occurrence_before: Literal["first", "last"] = "first"
     occurrence_after: Literal["first", "last"] = "first"
     shift_before: int = 0
     shift_after: int = 0
 
 
-class TruncatePath(DataProcessor):
+class TruncatePaths(DataProcessor):
     """
     Remove events that will be deleted from each user's path
     based on the specified event and selected parameters.
 
     Parameters
     ----------
     drop_before : str, optional
@@ -59,17 +59,17 @@
     ``Step`` - is the group of events in the user path with the same timestamp.
     If the user path doesn't contain events from ``drop_before`` and ``drop_after`` parameters, then its
     path does not change.
 
     See :doc:`Data processors user guide</user_guides/dataprocessors>` for the details.
     """
 
-    params: TruncatePathParams
+    params: TruncatePathsParams
 
-    def __init__(self, params: TruncatePathParams):
+    def __init__(self, params: TruncatePathsParams):
         super().__init__(params=params)
 
     def apply(self, eventstream: EventstreamType) -> EventstreamType:
         from retentioneering.eventstream.eventstream import Eventstream
 
         user_col = eventstream.schema.user_id
         time_col = eventstream.schema.event_timestamp
```

### Comparing `retentioneering-3.0.0b1/retentioneering/datasets/data/ab_test_demo.csv` & `retentioneering-3.0.0b2/retentioneering/datasets/data/ab_test_demo.csv`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b1/retentioneering/datasets/data/simple-onlineshop.csv` & `retentioneering-3.0.0b2/retentioneering/datasets/data/simple-onlineshop.csv`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b1/retentioneering/datasets/load.py` & `retentioneering-3.0.0b2/retentioneering/datasets/load.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b1/retentioneering/edgelist/edgelist.py` & `retentioneering-3.0.0b2/retentioneering/edgelist/edgelist.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b1/retentioneering/eventstream/eventstream.py` & `retentioneering-3.0.0b2/retentioneering/eventstream/eventstream.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,115 +1,120 @@
 # flake8: noqa
 from __future__ import annotations
 
 import uuid
+import warnings
 from collections.abc import Collection
 from typing import Any, Callable, List, Literal, MutableMapping, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
 
+from retentioneering.backend.tracker import track
 from retentioneering.constants import DATETIME_UNITS
 from retentioneering.eventstream.schema import EventstreamSchema, RawDataSchema
 from retentioneering.eventstream.types import (
     EventstreamType,
     RawDataCustomColSchema,
     RawDataSchemaType,
     Relation,
 )
-from retentioneering.graph import PGraph
-from retentioneering.tooling.clusters import Clusters
-from retentioneering.tooling.cohorts import Cohorts
+from retentioneering.preprocessing_graph import PreprocessingGraph
+from retentioneering.tooling import (
+    Clusters,
+    Cohorts,
+    EventTimestampHist,
+    Funnel,
+    StatTests,
+    StepMatrix,
+    StepSankey,
+    TimedeltaHist,
+    TransitionGraph,
+    UserLifetimeHist,
+)
+from retentioneering.tooling._describe import _Describe
+from retentioneering.tooling._describe_events import _DescribeEvents
+from retentioneering.tooling._transition_matrix import _TransitionMatrix
 from retentioneering.tooling.constants import BINS_ESTIMATORS
-from retentioneering.tooling.describe import Describe
-from retentioneering.tooling.describe_events import DescribeEvents
-from retentioneering.tooling.event_timestamp_hist import EventTimestampHist
-from retentioneering.tooling.funnel import Funnel
-from retentioneering.tooling.stattests import TEST_NAMES, StatTests
-from retentioneering.tooling.step_matrix import StepMatrix
-from retentioneering.tooling.step_sankey import StepSankey
-from retentioneering.tooling.timedelta_hist import (
+from retentioneering.tooling.stattests.constants import STATTEST_NAMES
+from retentioneering.tooling.timedelta_hist.constants import (
     AGGREGATION_NAMES,
     EVENTSTREAM_GLOBAL_EVENTS,
-    TimedeltaHist,
 )
-from retentioneering.tooling.transition_graph import TransitionGraph
-from retentioneering.tooling.transition_matrix import TransitionMatrix
 from retentioneering.tooling.typing.transition_graph import NormType, Threshold
-from retentioneering.tooling.user_lifetime_hist import UserLifetimeHist
 from retentioneering.utils import get_merged_col
 from retentioneering.utils.list import find_index
 
 from .helpers import (
+    AddNegativeEventsHelperMixin,
+    AddPositiveEventsHelperMixin,
+    AddStartEndEventsHelperMixin,
     CollapseLoopsHelperMixin,
-    DeleteUsersByPathLengthHelperMixin,
-    FilterHelperMixin,
-    GroupHelperMixin,
-    LostUsersHelperMixin,
-    NegativeTargetHelperMixin,
-    NewUsersHelperMixin,
-    PositiveTargetHelperMixin,
+    DropPathsHelperMixin,
+    FilterEventsHelperMixin,
+    GroupEventsHelperMixin,
+    LabelCroppedPathsHelperMixin,
+    LabelLostUsersHelperMixin,
+    LabelNewUsersHelperMixin,
     RenameHelperMixin,
     SplitSessionsHelperMixin,
-    StartEndHelperMixin,
-    TruncatedEventsHelperMixin,
-    TruncatePathHelperMixin,
+    TruncatePathsHelperMixin,
 )
 
 IndexOrder = List[Optional[str]]
 FeatureType = Literal["tfidf", "count", "frequency", "binary", "time", "time_fraction", "external"]
 NgramRange = Tuple[int, int]
 Method = Literal["kmeans", "gmm"]
 
 
 DEFAULT_INDEX_ORDER: IndexOrder = [
     "profile",
     "path_start",
     "new_user",
     "existing_user",
-    "truncated_left",
+    "cropped_left",
     "session_start",
-    "session_start_truncated",
+    "session_start_cropped",
     "group_alias",
     "raw",
     "raw_sleep",
     None,
     "synthetic",
     "synthetic_sleep",
     "positive_target",
     "negative_target",
-    "session_end_truncated",
+    "session_end_cropped",
     "session_end",
     "session_sleep",
-    "truncated_right",
+    "cropped_right",
     "absent_user",
     "lost_user",
     "path_end",
 ]
 
 RAW_COL_PREFIX = "raw_"
 DELETE_COL_NAME = "_deleted"
 
 
-# TODO проработать резервирование колонок
+# @TODO: проработать резервирование колонок
 
 
 class Eventstream(
     CollapseLoopsHelperMixin,
-    DeleteUsersByPathLengthHelperMixin,
-    FilterHelperMixin,
-    GroupHelperMixin,
-    LostUsersHelperMixin,
-    NegativeTargetHelperMixin,
-    NewUsersHelperMixin,
-    PositiveTargetHelperMixin,
+    DropPathsHelperMixin,
+    FilterEventsHelperMixin,
+    GroupEventsHelperMixin,
+    LabelLostUsersHelperMixin,
+    AddNegativeEventsHelperMixin,
+    LabelNewUsersHelperMixin,
+    AddPositiveEventsHelperMixin,
     SplitSessionsHelperMixin,
-    StartEndHelperMixin,
-    TruncatedEventsHelperMixin,
-    TruncatePathHelperMixin,
+    AddStartEndEventsHelperMixin,
+    LabelCroppedPathsHelperMixin,
+    TruncatePathsHelperMixin,
     RenameHelperMixin,
     EventstreamType,
 ):
     """
     Collection of tools for storing and processing clickstream data.
 
     Parameters
@@ -151,25 +156,25 @@
 
 
     """
 
     schema: EventstreamSchema
     index_order: IndexOrder
     relations: List[Relation]
+    preprocessiong_graph: PreprocessingGraph | None = None
+
     __raw_data_schema: RawDataSchemaType
     __events: pd.DataFrame | pd.Series[Any]
     __clusters: Clusters | None = None
     __funnel: Funnel | None = None
     __cohorts: Cohorts | None = None
     __step_matrix: StepMatrix | None = None
     __sankey: StepSankey | None = None
     __stattests: StatTests | None = None
-    __transition_graph: TransitionGraph | None = None
-    __p_graph: PGraph | None = None
-    __transition_matrix: TransitionMatrix | None = None
+    __transition_graph: TransitionGraph
     __timedelta_hist: TimedeltaHist | None = None
     __user_lifetime_hist: UserLifetimeHist | None = None
     __event_timestamp_hist: EventTimestampHist | None = None
 
     def __init__(
         self,
         raw_data: pd.DataFrame | pd.Series[Any],
@@ -182,14 +187,15 @@
         index_order: Optional[IndexOrder] = None,
         relations: Optional[List[Relation]] = None,
         user_sample_size: Optional[int | float] = None,
         user_sample_seed: Optional[int] = None,
     ) -> None:
         self.__clusters = None
         self.__funnel = None
+
         self.schema = schema if schema else EventstreamSchema()
 
         if not raw_data_schema:
             raw_data_schema = RawDataSchema()
             if "event_type" in raw_data.columns:
                 raw_data_schema.event_type = "event_type"
         elif isinstance(raw_data_schema, dict):
@@ -203,15 +209,17 @@
         else:
             self.index_order = index_order
         if not relations:
             self.relations = []
         else:
             self.relations = relations
         self.__events = self.__prepare_events(raw_data) if prepare else raw_data
+        self.__events = self.__required_cleanup(events=self.__events)
         self.index_events()
+        self.preprocessiong_graph = None
 
     def copy(self) -> Eventstream:
         """
         Make a copy of current ``eventstream``.
 
         Returns
         -------
@@ -489,14 +497,27 @@
 
         self.__events[DELETE_COL_NAME] = self.__events[DELETE_COL_NAME] | merged[f"{DELETE_COL_NAME}_y"] == True
 
     def __get_not_deleted_events(self) -> pd.DataFrame | pd.Series[Any]:
         events = self.__events
         return events[events[DELETE_COL_NAME] == False]
 
+    def __required_cleanup(self, events: pd.DataFrame | pd.Series[Any]) -> pd.DataFrame | pd.Series[Any]:
+        income_size = len(events)
+        events.dropna(  # type: ignore
+            subset=[self.schema.event_name, self.schema.event_timestamp, self.schema.user_id], inplace=True
+        )
+        size_after_cleanup = len(events)
+        if (removed_rows := income_size - size_after_cleanup) > 0:
+            warnings.warn(
+                "Removed %s rows because they have empty %s or %s or %s"
+                % (removed_rows, self.schema.event_name, self.schema.event_timestamp, self.schema.user_id)
+            )
+        return events
+
     def __prepare_events(self, raw_data: pd.DataFrame | pd.Series[Any]) -> pd.DataFrame | pd.Series[Any]:
         events = raw_data.copy()
         # add "raw_" prefix for raw cols
         events.rename(lambda col: f"raw_{col}", axis="columns", inplace=True)
 
         events[DELETE_COL_NAME] = False
         events[self.schema.event_id] = [uuid.uuid4() for x in range(len(events))]
@@ -652,15 +673,15 @@
         self,
         max_steps: int = 20,
         weight_col: Optional[str] = None,
         precision: int = 2,
         targets: Optional[list[str] | str] = None,
         accumulated: Optional[Union[Literal["both", "only"], None]] = None,
         sorting: Optional[list[str]] = None,
-        thresh: float = 0,
+        threshold: float = 0,
         centered: Optional[dict] = None,
         groups: Optional[Tuple[list, list]] = None,
         show_plot: bool = True,
     ) -> StepMatrix:
         """
         Show a heatmap visualization of the step matrix.
 
@@ -681,31 +702,30 @@
             eventstream=self,
             max_steps=max_steps,
             weight_col=weight_col,
             precision=precision,
             targets=targets,
             accumulated=accumulated,
             sorting=sorting,
-            thresh=thresh,
+            threshold=threshold,
             centered=centered,
             groups=groups,
         )
 
         self.__step_matrix.fit()
         if show_plot:
-            figure = self.__step_matrix.plot()
-            figure.show()
+            self.__step_matrix.plot()
         return self.__step_matrix
 
     def step_sankey(
         self,
         max_steps: int = 10,
-        thresh: Union[int, float] = 0.05,
+        threshold: Union[int, float] = 0.05,
         sorting: list | None = None,
-        target: Union[list[str], str] | None = None,
+        targets: Union[list[str], str] | None = None,
         autosize: bool = True,
         width: int | None = None,
         height: int | None = None,
         show_plot: bool = True,
     ) -> StepSankey:
         """
         Show a Sankey diagram visualizing the user paths in stepwise manner.
@@ -722,17 +742,17 @@
         StepSankey
             A ``StepSankey`` class instance fitted to the given parameters.
 
         """
         self.__sankey = StepSankey(
             eventstream=self,
             max_steps=max_steps,
-            thresh=thresh,
+            threshold=threshold,
             sorting=sorting,
-            target=target,
+            targets=targets,
             autosize=autosize,
             width=width,
             height=height,
         )
 
         self.__sankey.fit()
         if show_plot:
@@ -744,15 +764,16 @@
         self,
         cohort_start_unit: DATETIME_UNITS,
         cohort_period: Tuple[int, DATETIME_UNITS],
         average: bool = True,
         cut_bottom: int = 0,
         cut_right: int = 0,
         cut_diagonal: int = 0,
-        figsize: Tuple[float, float] = (10, 10),
+        width: float = 5.0,
+        height: float = 5.0,
         show_plot: bool = True,
     ) -> Cohorts:
         """
         Show a heatmap visualization of the user appearance grouped by cohorts.
 
         Parameters
         ----------
@@ -775,20 +796,20 @@
             cut_bottom=cut_bottom,
             cut_right=cut_right,
             cut_diagonal=cut_diagonal,
         )
 
         self.__cohorts.fit()
         if show_plot:
-            self.__cohorts.heatmap(figsize)
+            self.__cohorts.heatmap(width=width, height=height)
         return self.__cohorts
 
     def stattests(
         self,
-        test: TEST_NAMES,
+        test: STATTEST_NAMES,
         groups: Tuple[list[str | int], list[str | int]],
         func: Callable,
         group_names: Tuple[str, str] = ("group_1", "group_2"),
         alpha: float = 0.05,
     ) -> StatTests:
         """
         Determine the statistical difference between the metric values in two user groups.
@@ -810,23 +831,24 @@
         self.__stattests.display_results()
         return self.__stattests
 
     def timedelta_hist(
         self,
         raw_events_only: bool = False,
         event_pair: Optional[list[str | Literal[EVENTSTREAM_GLOBAL_EVENTS]]] = None,
-        only_adjacent_event_pairs: bool = True,
-        weight_col: str = "user_id",
-        aggregation: Optional[AGGREGATION_NAMES] = None,
+        adjacent_events_only: bool = True,
+        weight_col: str | None = None,
+        time_agg: Optional[AGGREGATION_NAMES] = None,
         timedelta_unit: DATETIME_UNITS = "s",
         log_scale: bool | tuple[bool, bool] | None = None,
         lower_cutoff_quantile: Optional[float] = None,
         upper_cutoff_quantile: Optional[float] = None,
         bins: int | Literal[BINS_ESTIMATORS] = 20,
-        figsize: tuple[float, float] = (12.0, 7.0),
+        width: float = 6.0,
+        height: float = 4.5,
         show_plot: bool = True,
     ) -> TimedeltaHist:
         """
         Plot the distribution of the time deltas between two events. Support various
         distribution types, such as distribution of time for adjacent consecutive events, or
         for a pair of pre-defined events, or median transition time from event to event per user/session.
 
@@ -843,23 +865,24 @@
             A ``TimedeltaHist`` class instance fitted with given parameters.
 
         """
         self.__timedelta_hist = TimedeltaHist(
             eventstream=self,
             raw_events_only=raw_events_only,
             event_pair=event_pair,
-            only_adjacent_event_pairs=only_adjacent_event_pairs,
-            aggregation=aggregation,
+            adjacent_events_only=adjacent_events_only,
+            time_agg=time_agg,
             weight_col=weight_col,
             timedelta_unit=timedelta_unit,
             log_scale=log_scale,
             lower_cutoff_quantile=lower_cutoff_quantile,
             upper_cutoff_quantile=upper_cutoff_quantile,
             bins=bins,
-            figsize=figsize,
+            width=width,
+            height=height,
         )
 
         self.__timedelta_hist.fit()
         if show_plot:
             self.__timedelta_hist.plot()
 
         return self.__timedelta_hist
@@ -867,15 +890,16 @@
     def user_lifetime_hist(
         self,
         timedelta_unit: DATETIME_UNITS = "s",
         log_scale: bool | tuple[bool, bool] | None = None,
         lower_cutoff_quantile: Optional[float] = None,
         upper_cutoff_quantile: Optional[float] = None,
         bins: int | Literal[BINS_ESTIMATORS] = 20,
-        figsize: tuple[float, float] = (12.0, 7.0),
+        width: float = 6.0,
+        height: float = 4.5,
         show_plot: bool = True,
     ) -> UserLifetimeHist:
         """
         Plot the distribution of user lifetimes. A ``users lifetime`` is the timedelta between the first and the last
         events of the user.
 
         Parameters
@@ -895,29 +919,31 @@
         self.__user_lifetime_hist = UserLifetimeHist(
             eventstream=self,
             timedelta_unit=timedelta_unit,
             log_scale=log_scale,
             lower_cutoff_quantile=lower_cutoff_quantile,
             upper_cutoff_quantile=upper_cutoff_quantile,
             bins=bins,
-            figsize=figsize,
+            width=width,
+            height=height,
         )
         self.__user_lifetime_hist.fit()
         if show_plot:
             self.__user_lifetime_hist.plot()
         return self.__user_lifetime_hist
 
     def event_timestamp_hist(
         self,
         event_list: list[str] | None = None,
         raw_events_only: bool = False,
         lower_cutoff_quantile: Optional[float] = None,
         upper_cutoff_quantile: Optional[float] = None,
         bins: int | Literal[BINS_ESTIMATORS] = 20,
-        figsize: tuple[float, float] = (12.0, 7.0),
+        width: float = 6.0,
+        height: float = 4.5,
         show_plot: bool = True,
     ) -> EventTimestampHist:
         """
         Plot distribution of events over time. Can be useful for detecting time-based anomalies, and visualising
         general timespan of the eventstream.
 
         Parameters
@@ -936,15 +962,16 @@
         self.__event_timestamp_hist = EventTimestampHist(
             eventstream=self,
             event_list=event_list,
             raw_events_only=raw_events_only,
             lower_cutoff_quantile=lower_cutoff_quantile,
             upper_cutoff_quantile=upper_cutoff_quantile,
             bins=bins,
-            figsize=figsize,
+            width=width,
+            height=height,
         )
 
         self.__event_timestamp_hist.fit()
         if show_plot:
             self.__event_timestamp_hist.plot()
         return self.__event_timestamp_hist
 
@@ -982,16 +1009,16 @@
         - All ``float`` values are rounded to 2.
         - All ``datetime`` values are rounded to seconds.
 
         See :ref:`Eventstream user guide<eventstream_describe>` for the details.
 
 
         """
-        describer = Describe(eventstream=self, session_col=session_col, raw_events_only=raw_events_only)
-        return describer._describe()
+        describer = _Describe(eventstream=self, session_col=session_col, raw_events_only=raw_events_only)
+        return describer._values()
 
     def describe_events(
         self, session_col: str = "session_id", raw_events_only: bool = False, event_list: list[str] | None = None
     ) -> pd.DataFrame:
         """
         Display general information on eventstream events. If ``session_col`` is present in eventstream, also
         output session statistics.
@@ -1051,86 +1078,115 @@
         -----
         - All ``float`` values are rounded to 2.
         - All ``datetime`` values are rounded to seconds.
 
         See :ref:`Eventstream user guide<eventstream_describe_events>` for the details.
 
         """
-        describer = DescribeEvents(
+        describer = _DescribeEvents(
             eventstream=self, session_col=session_col, event_list=event_list, raw_events_only=raw_events_only
         )
-        return describer._describe()
+        return describer._values()
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "transition_graph", "event_custom_name": "transition_graph_helper"},
+        allowed_params=[
+            "edges_norm_type",
+            "targets",
+            "nodes_threshold",
+            "edges_threshold",
+            "nodes_weight_col",
+            "edges_weight_col",
+            "custom_weight_cols",
+            "width",
+            "height",
+        ],
+    )
     def transition_graph(
         self,
-        graph_settings: dict[str, Any] | None = None,
         edges_norm_type: NormType = None,
         targets: MutableMapping[str, str | None] | None = None,
         nodes_threshold: Threshold | None = None,
         edges_threshold: Threshold | None = None,
         nodes_weight_col: str | None = None,
         edges_weight_col: str | None = None,
         custom_weight_cols: list[str] | None = None,
         width: int = 960,
         height: int = 900,
+        show_weights: bool = True,
+        show_percents: bool = False,
+        show_nodes_names: bool = True,
+        show_all_edges_for_targets: bool = True,
+        show_nodes_without_links: bool = False,
     ) -> TransitionGraph:
         """
 
         Parameters
         ----------
         See parameters' description
-            :py:class:`.TransitionGraph`
+            :py:meth:`.TransitionGraph.plot`
 
         Returns
         -------
         TransitionGraph
             Rendered IFrame graph.
 
         """
-        self.__transition_graph = TransitionGraph(
-            eventstream=self,
-            graph_settings=graph_settings,
-            edges_norm_type=edges_norm_type,
+        self.__transition_graph = TransitionGraph(eventstream=self)
+        self.__transition_graph.plot(
             targets=targets,
+            edges_norm_type=edges_norm_type,
+            edges_weight_col=edges_weight_col,
             nodes_threshold=nodes_threshold,
             edges_threshold=edges_threshold,
             nodes_weight_col=nodes_weight_col,
-            edges_weight_col=edges_weight_col,
             custom_weight_cols=custom_weight_cols,
-        )
-        self.__transition_graph.plot_graph(
-            targets=targets,
             width=width,
             height=height,
-            edges_norm_type=edges_norm_type,
+            show_weights=show_weights,
+            show_percents=show_percents,
+            show_nodes_names=show_nodes_names,
+            show_all_edges_for_targets=show_all_edges_for_targets,
+            show_nodes_without_links=show_nodes_without_links,
         )
         return self.__transition_graph
 
-    def processing_graph(self) -> PGraph:
-        if self.__p_graph is None:
-            self.__p_graph = PGraph(source_stream=self)
-        self.__p_graph.display()
-        return self.__p_graph
-
-    def transition_matrix(self, weight_col: str | None = None, norm_type: NormType = None) -> TransitionMatrix:
+    def preprocessing_graph(self) -> PreprocessingGraph:
+        """
+        Display the preprocessing GUI tool.
         """
-        Display transition weights as a matrix for each unique pair of events.
-        The calculation logic is the same that is used for edge weights calculation of transition graph.
+        if self.preprocessiong_graph is None:
+            self.preprocessiong_graph = PreprocessingGraph(source_stream=self)
+        self.preprocessiong_graph.display()
+        return self.preprocessiong_graph
+
+    @track(  # type: ignore
+        tracking_info={"event_name": "transition_matrix", "event_custom_name": "transition_matrix_helper"},
+        allowed_params=["weight_col", "norm_type"],
+    )
+    def transition_matrix(self, weight_col: str | None = None, norm_type: NormType = None) -> pd.DataFrame:
+        """
+        Get transition weights as a matrix for each unique pair of events. The calculation logic is the same
+        that is used for edge weights calculation of transition graph.
 
         Parameters
         ----------
-        See parameters' description
-            :py:meth:`.TransitionMatrix.values`
 
+        weight_col : str, optional
+            Weighting column for the transition weights calculation.
+            See :ref:`transition graph user guide <transition_graph_weights>` for the details.
+
+        norm_type : {"full", "node", None}, default None
+            Normalization type. See :ref:`transition graph user guide <transition_graph_weights>` for the details.
 
         Returns
         -------
-        TransitionMatrix
-            Display ``(i, j)``-th matrix value relates to the weight of i → j transition.
+        pd.DataFrame
+            Transition matrix. ``(i, j)``-th matrix value relates to the weight of i → j transition.
 
+        Notes
+        -----
+        See :ref:`transition graph user guide <transition_graph_transition_matrix>` for the details.
         """
-        if self.__transition_matrix is None:
-            self.__transition_matrix = TransitionMatrix(
-                eventstream=self,
-            )
-        self.__transition_matrix.display(weight_col=weight_col, norm_type=norm_type)
-        return self.__transition_matrix
+
+        matrix = _TransitionMatrix(eventstream=self)
+        return matrix._values(weight_col=weight_col, norm_type=norm_type)
```

### Comparing `retentioneering-3.0.0b1/retentioneering/eventstream/helpers/__init__.py` & `retentioneering-3.0.0b2/retentioneering/eventstream/helpers/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+from .add_negative_events_helper import AddNegativeEventsHelperMixin
+from .add_positive_events_helper import AddPositiveEventsHelperMixin
+from .add_start_end_events_helper import AddStartEndEventsHelperMixin
 from .collapse_loops_helper import CollapseLoopsHelperMixin
-from .delete_users_by_path_length_helper import DeleteUsersByPathLengthHelperMixin
-from .filter_helper import FilterHelperMixin
-from .group_helper import GroupHelperMixin
-from .lost_users_helper import LostUsersHelperMixin
-from .negative_target import NegativeTargetHelperMixin
-from .new_users_helper import NewUsersHelperMixin
-from .positive_target import PositiveTargetHelperMixin
+from .drop_paths_helper import DropPathsHelperMixin
+from .filter_events_helper import FilterEventsHelperMixin
+from .group_events_helper import GroupEventsHelperMixin
+from .label_cropped_paths_helper import LabelCroppedPathsHelperMixin
+from .label_lost_users_helper import LabelLostUsersHelperMixin
+from .label_new_users_helper import LabelNewUsersHelperMixin
 from .rename_helper import RenameHelperMixin
-from .split_session_helper import SplitSessionsHelperMixin
-from .start_end_helper import StartEndHelperMixin
-from .truncate_path_helper import TruncatePathHelperMixin
-from .truncated_events_helper import TruncatedEventsHelperMixin
+from .split_sessions_helper import SplitSessionsHelperMixin
+from .truncate_paths_helper import TruncatePathsHelperMixin
```

### Comparing `retentioneering-3.0.0b1/retentioneering/eventstream/helpers/collapse_loops_helper.py` & `retentioneering-3.0.0b2/retentioneering/eventstream/helpers/label_new_users_helper.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,54 +1,44 @@
 from __future__ import annotations
 
-from typing import Literal, Union
+from typing import List, Literal, Union
 
 from ..types import EventstreamType
 
 
-class CollapseLoopsHelperMixin:
-    def collapse_loops(
-        self,
-        suffix: Union[Literal["loop", "count"], None] = "loop",
-        timestamp_aggregation_type: Literal["max", "min", "mean"] = "max",
-    ) -> EventstreamType:
+class LabelNewUsersHelperMixin:
+    def label_new_users(self, new_users_list: Union[List[int], Literal["all"]]) -> EventstreamType:
         """
-        A method of ``Eventstream`` class that finds ``loops`` and creates new synthetic events
-        in paths of all users having such sequences.
-
-        A ``loop`` - is a sequence of repetitive events.
-        For example *"event1 -> event1"*
+        A method of ``Eventstream`` class that creates one
+        of the synthetic events in each user's path: ``new_user`` or ``existing_user`` .
 
         Parameters
         ----------
         See parameters description
-            :py:class:`.CollapseLoops`
+            :py:class:`.LabelNewUsers`
 
         Returns
         -------
         Eventstream
-             Input ``eventstream`` with ``loops`` replaced by new synthetic events.
+             Input ``eventstream`` with new synthetic events.
 
 
         """
-
         # avoid circular import
         from retentioneering.data_processors_lib import (
-            CollapseLoops,
-            CollapseLoopsParams,
+            LabelNewUsers,
+            LabelNewUsersParams,
+        )
+        from retentioneering.preprocessing_graph.nodes import EventsNode
+        from retentioneering.preprocessing_graph.preprocessing_graph import (
+            PreprocessingGraph,
         )
-        from retentioneering.graph.nodes import EventsNode
-        from retentioneering.graph.p_graph import PGraph
 
-        p = PGraph(source_stream=self)  # type: ignore
+        p = PreprocessingGraph(source_stream=self)  # type: ignore
 
         node = EventsNode(
-            processor=CollapseLoops(
-                params=CollapseLoopsParams(
-                    suffix=suffix, timestamp_aggregation_type=timestamp_aggregation_type  # type: ignore
-                )
-            )
+            processor=LabelNewUsers(params=LabelNewUsersParams(new_users_list=new_users_list))  # type: ignore
         )
         p.add_node(node=node, parents=[p.root])
         result = p.combine(node)
         del p
         return result
```

### Comparing `retentioneering-3.0.0b1/retentioneering/eventstream/helpers/delete_users_by_path_length_helper.py` & `retentioneering-3.0.0b2/retentioneering/eventstream/helpers/label_lost_users_helper.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,49 +1,52 @@
 from __future__ import annotations
 
-from typing import Tuple
+from typing import List, Optional, Tuple
 
 from retentioneering.constants import DATETIME_UNITS
 
 from ..types import EventstreamType
 
 
-class DeleteUsersByPathLengthHelperMixin:
-    def delete_users(
-        self, events_num: int | None = None, cutoff: Tuple[float, DATETIME_UNITS] | None = None
+class LabelLostUsersHelperMixin:
+    def label_lost_users(
+        self, timeout: Optional[Tuple[float, DATETIME_UNITS]] = None, lost_users_list: Optional[List[int]] = None
     ) -> EventstreamType:
         """
-        A method of ``Eventstream`` class that deletes users' paths that are shorter than the specified
-        number of events or cut_off.
+        A method of ``Eventstream`` class that creates one
+        of the synthetic events in each user's path: ``lost_user`` or ``absent_user`` .
 
         Parameters
         ----------
         See parameters description
-            :py:class:`.DeleteUsersByPathLength`
+            :py:class:`.LabelLostUsers`
 
         Returns
         -------
         Eventstream
-             Input ``eventstream`` without the deleted short users' paths.
+             Input ``eventstream`` with new synthetic events.
+
 
 
         """
 
         # avoid circular import
         from retentioneering.data_processors_lib import (
-            DeleteUsersByPathLength,
-            DeleteUsersByPathLengthParams,
+            LabelLostUsers,
+            LabelLostUsersParams,
+        )
+        from retentioneering.preprocessing_graph.nodes import EventsNode
+        from retentioneering.preprocessing_graph.preprocessing_graph import (
+            PreprocessingGraph,
         )
-        from retentioneering.graph.nodes import EventsNode
-        from retentioneering.graph.p_graph import PGraph
 
-        p = PGraph(source_stream=self)  # type: ignore
+        p = PreprocessingGraph(source_stream=self)  # type: ignore
 
         node = EventsNode(
-            processor=DeleteUsersByPathLength(
-                params=DeleteUsersByPathLengthParams(events_num=events_num, cutoff=cutoff)  # type: ignore
+            processor=LabelLostUsers(
+                params=LabelLostUsersParams(timeout=timeout, lost_users_list=lost_users_list)  # type: ignore
             )
         )
         p.add_node(node=node, parents=[p.root])
         result = p.combine(node)
         del p
         return result
```

### Comparing `retentioneering-3.0.0b1/retentioneering/eventstream/helpers/filter_helper.py` & `retentioneering-3.0.0b2/retentioneering/eventstream/helpers/filter_events_helper.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from typing import Any, Callable
 
 from pandas import DataFrame
 
 from ..types import EventstreamSchemaType, EventstreamType
 
 
-class FilterHelperMixin:
-    def filter(self, func: Callable[[DataFrame, EventstreamSchemaType], Any]) -> EventstreamType:
+class FilterEventsHelperMixin:
+    def filter_events(self, func: Callable[[DataFrame, EventstreamSchemaType], Any]) -> EventstreamType:
         """
         A method of ``Eventstream`` class that filters input ``eventstream`` based on custom conditions.
 
         Parameters
         ----------
         See parameters description
             :py:class:`.FilterEvents`
@@ -22,17 +22,19 @@
         Eventstream
             The filtered ``eventstream``.
 
 
         """
         # avoid circular import
         from retentioneering.data_processors_lib import FilterEvents, FilterEventsParams
-        from retentioneering.graph.nodes import EventsNode
-        from retentioneering.graph.p_graph import PGraph
+        from retentioneering.preprocessing_graph.nodes import EventsNode
+        from retentioneering.preprocessing_graph.preprocessing_graph import (
+            PreprocessingGraph,
+        )
 
-        p = PGraph(source_stream=self)  # type: ignore
+        p = PreprocessingGraph(source_stream=self)  # type: ignore
 
         node = EventsNode(processor=FilterEvents(params=FilterEventsParams(func=func)))  # type: ignore
         p.add_node(node=node, parents=[p.root])
         result = p.combine(node)
         del p
         return result
```

### Comparing `retentioneering-3.0.0b1/retentioneering/eventstream/helpers/group_helper.py` & `retentioneering-3.0.0b2/retentioneering/eventstream/helpers/group_events_helper.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import pandas as pd
 
 from ..types import EventstreamSchemaType, EventstreamType
 
 EventstreamFilter = Callable[[pd.DataFrame, EventstreamSchemaType], Any]
 
 
-class GroupHelperMixin:
-    def group(
+class GroupEventsHelperMixin:
+    def group_events(
         self,
         event_name: str,
         func: EventstreamFilter,
         event_type: str | None = "group_alias",
     ) -> EventstreamType:
         """
         A method of ``Eventstream`` class that filters and replaces raw events with new synthetic events,
@@ -32,18 +32,20 @@
 
 
 
         """
 
         # avoid circular import
         from retentioneering.data_processors_lib import GroupEvents, GroupEventsParams
-        from retentioneering.graph.nodes import EventsNode
-        from retentioneering.graph.p_graph import PGraph
+        from retentioneering.preprocessing_graph.nodes import EventsNode
+        from retentioneering.preprocessing_graph.preprocessing_graph import (
+            PreprocessingGraph,
+        )
 
-        p = PGraph(source_stream=self)  # type: ignore
+        p = PreprocessingGraph(source_stream=self)  # type: ignore
 
         node = EventsNode(
             processor=GroupEvents(
                 params=GroupEventsParams(event_name=event_name, func=func, event_type=event_type)  # type: ignore
             )
         )
         p.add_node(node=node, parents=[p.root])
```

### Comparing `retentioneering-3.0.0b1/retentioneering/eventstream/helpers/lost_users_helper.py` & `retentioneering-3.0.0b2/retentioneering/eventstream/helpers/label_cropped_paths_helper.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,51 @@
 from __future__ import annotations
 
-from typing import List, Optional, Tuple
+from typing import Optional, Tuple
 
 from retentioneering.constants import DATETIME_UNITS
 
 from ..types import EventstreamType
 
 
-class LostUsersHelperMixin:
-    def lost_users(
-        self, lost_cutoff: Optional[Tuple[float, DATETIME_UNITS]] = None, lost_users_list: Optional[List[int]] = None
+class LabelCroppedPathsHelperMixin:
+    def label_cropped_paths(
+        self,
+        left_cutoff: Optional[Tuple[float, DATETIME_UNITS]],
+        right_cutoff: Optional[Tuple[float, DATETIME_UNITS]],
     ) -> EventstreamType:
         """
-        A method of ``Eventstream`` class that creates one
-        of the synthetic events in each user's path: ``lost_user`` or ``absent_user`` .
+        A method of ``Eventstream`` class that creates new synthetic event(s) for each user based
+        on the timeout threshold: ``cropped_left`` and ``cropped_right``.
+
 
         Parameters
         ----------
         See parameters description
-            :py:class:`.LostUsersEvents`
+            :py:class:`.LabelCroppedPaths`
 
         Returns
         -------
         Eventstream
-             Input ``eventstream`` with new synthetic events.
-
+            Input ``eventstream`` with new synthetic events.
 
 
         """
-
         # avoid circular import
-        from retentioneering.data_processors_lib import LostUsersEvents, LostUsersParams
-        from retentioneering.graph.nodes import EventsNode
-        from retentioneering.graph.p_graph import PGraph
-
-        p = PGraph(source_stream=self)  # type: ignore
-
-        node = EventsNode(
-            processor=LostUsersEvents(
-                params=LostUsersParams(lost_cutoff=lost_cutoff, lost_users_list=lost_users_list)  # type: ignore
-            )
+        from retentioneering.data_processors_lib import (
+            LabelCroppedPaths,
+            LabelCroppedPathsParams,
+        )
+        from retentioneering.preprocessing_graph.nodes import EventsNode
+        from retentioneering.preprocessing_graph.preprocessing_graph import (
+            PreprocessingGraph,
         )
+
+        p = PreprocessingGraph(source_stream=self)  # type: ignore
+
+        params = dict(left_cutoff=left_cutoff, right_cutoff=right_cutoff)
+
+        node = EventsNode(processor=LabelCroppedPaths(params=LabelCroppedPathsParams(**params)))  # type: ignore
         p.add_node(node=node, parents=[p.root])
         result = p.combine(node)
         del p
         return result
```

### Comparing `retentioneering-3.0.0b1/retentioneering/eventstream/helpers/negative_target.py` & `retentioneering-3.0.0b2/retentioneering/eventstream/helpers/add_negative_events_helper.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 from __future__ import annotations
 
 from typing import Callable, List, Optional
 
 from ..types import EventstreamType
 
 
-class NegativeTargetHelperMixin:
-    def negative_target(self, negative_target_events: List[str], func: Optional[Callable] = None) -> EventstreamType:
+class AddNegativeEventsHelperMixin:
+    def add_negative_events(self, targets: List[str], func: Optional[Callable] = None) -> EventstreamType:
         """
         A method of ``Eventstream`` class that creates new synthetic
         events in paths of all users having the specified events - ``negative_target_RAW_EVENT_NAME``.
 
         Parameters
         ----------
         See parameters description
-            :py:class:`.NegativeTarget`
+            :py:class:`.AddNegativeEvents`
 
 
         Returns
         -------
         Eventstream
             Input ``eventstream`` with new synthetic events.
 
 
 
         """
         # avoid circular import
         from retentioneering.data_processors_lib import (
-            NegativeTarget,
-            NegativeTargetParams,
+            AddNegativeEvents,
+            AddNegativeEventsParams,
+        )
+        from retentioneering.preprocessing_graph.nodes import EventsNode
+        from retentioneering.preprocessing_graph.preprocessing_graph import (
+            PreprocessingGraph,
         )
-        from retentioneering.graph.nodes import EventsNode
-        from retentioneering.graph.p_graph import PGraph
 
-        p = PGraph(source_stream=self)  # type: ignore
+        p = PreprocessingGraph(source_stream=self)  # type: ignore
 
-        params: dict[str, list[str] | Callable] = {"negative_target_events": negative_target_events}
+        params: dict[str, list[str] | Callable] = {"targets": targets}
         if func:
             params["func"] = func
 
-        node = EventsNode(processor=NegativeTarget(params=NegativeTargetParams(**params)))  # type: ignore
+        node = EventsNode(processor=AddNegativeEvents(params=AddNegativeEventsParams(**params)))  # type: ignore
         p.add_node(node=node, parents=[p.root])
         result = p.combine(node)
         del p
         return result
```

### Comparing `retentioneering-3.0.0b1/retentioneering/eventstream/helpers/new_users_helper.py` & `retentioneering-3.0.0b2/retentioneering/eventstream/helpers/drop_paths_helper.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,46 @@
 from __future__ import annotations
 
-from typing import List, Literal, Union
+from typing import Tuple
+
+from retentioneering.constants import DATETIME_UNITS
 
 from ..types import EventstreamType
 
 
-class NewUsersHelperMixin:
-    def add_new_users(self, new_users_list: Union[List[int], Literal["all"]]) -> EventstreamType:
+class DropPathsHelperMixin:
+    def drop_paths(
+        self, min_steps: int | None = None, min_time: Tuple[float, DATETIME_UNITS] | None = None
+    ) -> EventstreamType:
         """
-        A method of ``Eventstream`` class that creates one
-        of the synthetic events in each user's path: ``new_user`` or ``existing_user`` .
+        A method of ``Eventstream`` class that deletes users' paths that are shorter than the specified
+        number of events or cut_off.
 
         Parameters
         ----------
         See parameters description
-            :py:class:`.NewUsersEvents`
+            :py:class:`.DropPaths`
 
         Returns
         -------
         Eventstream
-             Input ``eventstream`` with new synthetic events.
+             Input ``eventstream`` without the deleted short users' paths.
 
 
         """
+
         # avoid circular import
-        from retentioneering.data_processors_lib import NewUsersEvents, NewUsersParams
-        from retentioneering.graph.nodes import EventsNode
-        from retentioneering.graph.p_graph import PGraph
+        from retentioneering.data_processors_lib import DropPaths, DropPathsParams
+        from retentioneering.preprocessing_graph.nodes import EventsNode
+        from retentioneering.preprocessing_graph.preprocessing_graph import (
+            PreprocessingGraph,
+        )
 
-        p = PGraph(source_stream=self)  # type: ignore
+        p = PreprocessingGraph(source_stream=self)  # type: ignore
 
         node = EventsNode(
-            processor=NewUsersEvents(params=NewUsersParams(new_users_list=new_users_list))  # type: ignore
+            processor=DropPaths(params=DropPathsParams(min_steps=min_steps, min_time=min_time))  # type: ignore
         )
         p.add_node(node=node, parents=[p.root])
         result = p.combine(node)
         del p
         return result
```

### Comparing `retentioneering-3.0.0b1/retentioneering/eventstream/helpers/positive_target.py` & `retentioneering-3.0.0b2/retentioneering/eventstream/helpers/add_positive_events_helper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 from __future__ import annotations
 
 from typing import Callable, List, Optional
 
 from ..types import EventstreamType
 
 
-class PositiveTargetHelperMixin:
-    def positive_target(self, positive_target_events: List[str], func: Optional[Callable] = None) -> EventstreamType:
+class AddPositiveEventsHelperMixin:
+    def add_positive_events(self, targets: List[str], func: Optional[Callable] = None) -> EventstreamType:
         """
         A method of ``Eventstream`` class that creates new synthetic
         events in paths of all users having the specified events - ``positive_target_RAW_EVENT_NAME``.
 
         Parameters
         ----------
         See parameters description
-            :py:class:`.PositiveTarget`
+            :py:class:`.AddPositiveEvents`
 
         Returns
         -------
         Eventstream
             Input ``eventstream`` with new synthetic events.
 
 
 
         """
         # avoid circular import
         from retentioneering.data_processors_lib import (
-            PositiveTarget,
-            PositiveTargetParams,
+            AddPositiveEvents,
+            AddPositiveEventsParams,
+        )
+        from retentioneering.preprocessing_graph.nodes import EventsNode
+        from retentioneering.preprocessing_graph.preprocessing_graph import (
+            PreprocessingGraph,
         )
-        from retentioneering.graph.nodes import EventsNode
-        from retentioneering.graph.p_graph import PGraph
 
-        p = PGraph(source_stream=self)  # type: ignore
+        p = PreprocessingGraph(source_stream=self)  # type: ignore
 
-        params: dict[str, list[str] | Callable] = {"positive_target_events": positive_target_events}
+        params: dict[str, list[str] | Callable] = {"targets": targets}
         if func:
             params["func"] = func
 
-        node = EventsNode(processor=PositiveTarget(params=PositiveTargetParams(**params)))  # type: ignore
+        node = EventsNode(processor=AddPositiveEvents(params=AddPositiveEventsParams(**params)))  # type: ignore
         p.add_node(node=node, parents=[p.root])
         result = p.combine(node)
         del p
         return result
```

### Comparing `retentioneering-3.0.0b1/retentioneering/eventstream/helpers/split_session_helper.py` & `retentioneering-3.0.0b2/retentioneering/eventstream/helpers/split_sessions_helper.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 
 from ..types import EventstreamType
 
 
 class SplitSessionsHelperMixin:
     def split_sessions(
         self,
-        session_cutoff: Tuple[float, DATETIME_UNITS],
+        timeout: Tuple[float, DATETIME_UNITS],
         session_col: str = "session_id",
         mark_truncated: Optional[bool] = False,
     ) -> EventstreamType:
         """
         A method of ``Eventstream`` class that creates new synthetic events in each user's path:
-        ``session_start`` (or ``session_start_truncated``) and ``session_end`` (or ``session_end_truncated``).
+        ``session_start`` (or ``session_start_cropped``) and ``session_end`` (or ``session_end_cropped``).
         The created events divide users' paths on sessions.
         Also creates a new column that contains session number for each event in the input eventstream
         Session number will take the form: ``{user_id}_{session_number through one user path}``.
         The created events and column are added to the input eventstream.
 
         Parameters
         ----------
@@ -35,17 +35,19 @@
         """
 
         # avoid circular import
         from retentioneering.data_processors_lib import (
             SplitSessions,
             SplitSessionsParams,
         )
-        from retentioneering.graph.nodes import EventsNode
-        from retentioneering.graph.p_graph import PGraph
+        from retentioneering.preprocessing_graph.nodes import EventsNode
+        from retentioneering.preprocessing_graph.preprocessing_graph import (
+            PreprocessingGraph,
+        )
 
-        p = PGraph(source_stream=self)  # type: ignore
-        params = dict(session_cutoff=session_cutoff, session_col=session_col, mark_truncated=mark_truncated)
+        p = PreprocessingGraph(source_stream=self)  # type: ignore
+        params = dict(timeout=timeout, session_col=session_col, mark_truncated=mark_truncated)
         node = EventsNode(processor=SplitSessions(params=SplitSessionsParams(**params)))  # type: ignore
         p.add_node(node=node, parents=[p.root])
         result = p.combine(node)
         del p
         return result
```

### Comparing `retentioneering-3.0.0b1/retentioneering/eventstream/helpers/start_end_helper.py` & `retentioneering-3.0.0b2/retentioneering/eventstream/helpers/add_start_end_events_helper.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 from __future__ import annotations
 
 from ..types import EventstreamType
 
 
-class StartEndHelperMixin:
-    def add_start_end(self) -> EventstreamType:
+class AddStartEndEventsHelperMixin:
+    def add_start_end_events(self) -> EventstreamType:
         """
         A method of ``Eventstream`` class that creates
         two synthetic events in each user's path: ``path_start`` and ``path_end``.
 
         Returns
         -------
         Eventstream
-            Input ``eventstream`` with added synthetic events. See details :py:class:`.StartEndEvents`.
+            Input ``eventstream`` with added synthetic events. See details :py:class:`.AddStartEndEvents`.
 
 
         """
         # avoid circular import
         from retentioneering.data_processors_lib import (
-            StartEndEvents,
-            StartEndEventsParams,
+            AddStartEndEvents,
+            AddStartEndEventsParams,
+        )
+        from retentioneering.preprocessing_graph.nodes import EventsNode
+        from retentioneering.preprocessing_graph.preprocessing_graph import (
+            PreprocessingGraph,
         )
-        from retentioneering.graph.nodes import EventsNode
-        from retentioneering.graph.p_graph import PGraph
 
-        p = PGraph(source_stream=self)  # type: ignore
+        p = PreprocessingGraph(source_stream=self)  # type: ignore
 
-        node = EventsNode(processor=StartEndEvents(params=StartEndEventsParams(**{})))
+        node = EventsNode(processor=AddStartEndEvents(params=AddStartEndEventsParams(**{})))
         p.add_node(node=node, parents=[p.root])
         result = p.combine(node)
         del p
         return result
```

### Comparing `retentioneering-3.0.0b1/retentioneering/eventstream/helpers/truncate_path_helper.py` & `retentioneering-3.0.0b2/retentioneering/eventstream/helpers/truncate_paths_helper.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 from typing import Literal, Optional
 
 from ..types import EventstreamType
 
 
-class TruncatePathHelperMixin:
-    def truncate_path(
+class TruncatePathsHelperMixin:
+    def truncate_paths(
         self,
         drop_before: Optional[str] = None,
         drop_after: Optional[str] = None,
         occurrence_before: Literal["first", "last"] = "first",
         occurrence_after: Literal["first", "last"] = "first",
         shift_before: int = 0,
         shift_after: int = 0,
@@ -19,36 +19,41 @@
         A method of ``Eventstream`` class that truncates each user's path based on the
         specified event(s) and selected parameters.
 
 
         Parameters
         ----------
         See parameters description
-            :py:class:`.TruncatePath`
+            :py:class:`.TruncatePaths`
 
         Returns
         -------
         Eventstream
              Input ``eventstream`` with truncated paths.
 
 
         """
         # avoid circular import
-        from retentioneering.data_processors_lib import TruncatePath, TruncatePathParams
-        from retentioneering.graph.nodes import EventsNode
-        from retentioneering.graph.p_graph import PGraph
+        from retentioneering.data_processors_lib import (
+            TruncatePaths,
+            TruncatePathsParams,
+        )
+        from retentioneering.preprocessing_graph.nodes import EventsNode
+        from retentioneering.preprocessing_graph.preprocessing_graph import (
+            PreprocessingGraph,
+        )
 
-        p = PGraph(source_stream=self)  # type: ignore
+        p = PreprocessingGraph(source_stream=self)  # type: ignore
         params = {
             "drop_before": drop_before,
             "drop_after": drop_after,
             "occurrence_before": occurrence_before,
             "occurrence_after": occurrence_after,
             "shift_before": shift_before,
             "shift_after": shift_after,
         }
 
-        node = EventsNode(processor=TruncatePath(params=TruncatePathParams(**params)))  # type: ignore
+        node = EventsNode(processor=TruncatePaths(params=TruncatePathsParams(**params)))  # type: ignore
         p.add_node(node=node, parents=[p.root])
         result = p.combine(node)
         del p
         return result
```

### Comparing `retentioneering-3.0.0b1/retentioneering/eventstream/schema.py` & `retentioneering-3.0.0b2/retentioneering/eventstream/schema.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b1/retentioneering/eventstream/types.py` & `retentioneering-3.0.0b2/retentioneering/eventstream/types.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b1/retentioneering/exceptions/server.py` & `retentioneering-3.0.0b2/retentioneering/exceptions/server.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b1/retentioneering/graph/nodes.py` & `retentioneering-3.0.0b2/retentioneering/preprocessing_graph/nodes.py`

 * *Files 11% similar despite different names*

```diff
@@ -42,25 +42,25 @@
         super().__init__()
         self.events = source
         self.description = description
 
 
 class EventsNode(BaseNode):
     """
-    Class for regular nodes of a preprocessing graph.
+    Class for regular nodes of a PreprocessingGraph.
 
     Notes
     -----
     See :doc:`Preprocessing user guide</user_guides/preprocessing>` for the details.
 
     See Also
     --------
-    .PGraph.add_node : Add a node to Pgraph.
-    .PGraph.combine : Run calculations of Preprocessing Graph.
-    .MergeNode
+    .PreprocessingGraph.add_node : Add a node to PreprocessingGraph.
+    .PreprocessingGraph.combine : Run calculations of PreprocessingGraph.
+    .MergeNode : Merging nodes of a PreprocessingGraph.
 
     """
 
     processor: DataProcessor
     events: Optional[EventstreamType]
     description: Optional[str]
 
@@ -72,25 +72,25 @@
 
     def calc_events(self, parent: EventstreamType) -> None:
         self.events = self.processor.apply(parent)
 
 
 class MergeNode(BaseNode):
     """
-    Class for merging nodes of a preprocessing graph.
+    Class for merging nodes of a PreprocessingGraph.
 
     Notes
     -----
     See :doc:`Preprocessing user guide</user_guides/preprocessing>` for the details.
 
     See Also
     --------
-    .PGraph.add_node : Add a node to Pgraph.
-    .PGraph.combine : Run calculations of Preprocessing Graph.
-    .EventsNode
+    .PreprocessingGraph.add_node : Add a node to PreprocessingGraph.
+    .PreprocessingGraph.combine : Run calculations of PreprocessingGraph.
+    .EventsNode : Regular nodes of a PreprocessingGraph.
 
     """
 
     events: Optional[EventstreamType]
     description: Optional[str]
 
     def __init__(self, description: Optional[str] = None) -> None:
```

### Comparing `retentioneering-3.0.0b1/retentioneering/graph/p_graph.py` & `retentioneering-3.0.0b2/retentioneering/preprocessing_graph/preprocessing_graph.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 from pydantic import ValidationError
 
 from retentioneering.backend import JupyterServer, ServerManager
 from retentioneering.backend.callback import list_dataprocessor, list_dataprocessor_mock
 from retentioneering.eventstream.types import EventstreamType
 from retentioneering.exceptions.server import ServerErrorWithResponse
 from retentioneering.exceptions.widget import WidgetParseError
-from retentioneering.graph.nodes import (
+from retentioneering.preprocessing_graph.nodes import (
     EventsNode,
     MergeNode,
     Node,
     SourceNode,
     build_node,
 )
-from retentioneering.templates import PGraphRenderer
+from retentioneering.templates import PreprocessingGraphRenderer
 
 
 class NodeData(TypedDict):
     name: str
     pk: str
     description: Optional[str]
     processor: Optional[dict]
@@ -52,15 +52,15 @@
 class CreateNodeErrorDesc(TypedDict):
     type: Literal["node_error"]
     node_pk: str
     msg: Optional[str]
     fields_errors: List[FieldErrorDesc]
 
 
-class PGraph:
+class PreprocessingGraph:
     """
     Collection of methods for preprocessing graph construction and calculation.
 
     Parameters
     ----------
     source_stream : EventstreamType
         Source eventstream.
@@ -81,15 +81,15 @@
         self.root = SourceNode(source=source_stream)
         self.combine_result = None
         self._ngraph = networkx.DiGraph()
         self._ngraph.add_node(self.root)
 
     def add_node(self, node: Node, parents: List[Node]) -> None:
         """
-        Add node to ``PGraph`` instance.
+        Add node to ``PreprocessingGraph`` instance.
 
         Parameters
         ----------
         node : Node
             An instance of either ``EventsNode`` or ``MergeNode``.
         parents : list of Nodes
 
@@ -98,17 +98,17 @@
 
         Returns
         -------
         None
 
         See Also
         --------
-        PGraph.combine : Adding a node doesn't cause graph recalculation.
-        .EventsNode
-        .MergeNode
+        PreprocessingGraph.combine : Start PreprocessingGraph recalculation.
+        .EventsNode : Regular nodes of a preprocessing graph.
+        .MergeNode : Merge nodes of a preprocessing graph.
 
         """
         self.__valiate_already_exists(node)
         self.__validate_not_found(parents)
 
         if node.events is not None:
             self.__validate_schema(node.events)
@@ -172,14 +172,18 @@
         Show parents of the specified ``node``.
 
         Parameters
         ----------
         node : Node
             Instance of one of the classes SourceNode, EventsNode or MergeNode.
 
+        Returns
+        -------
+        list of Nodes
+
         """
         self.__validate_not_found([node])
         parents: List[Node] = []
 
         for parent in self._ngraph.predecessors(node):
             parents.append(parent)
         return parents
@@ -208,40 +212,40 @@
     def __validate_not_found(self, nodes: List[Node]) -> None:
         for node in nodes:
             if node not in self._ngraph.nodes:
                 raise ValueError("node not found!")
 
     def display(self, width: int = 960, height: int = 900) -> DisplayHandle:
         """
-        Show constructed ``PGraph``.
+        Show constructed ``PreprocessingGraph``.
 
         """
         if not self.__server_manager:
             self.__server_manager = ServerManager()
 
         if not self.__server:
             self.__server = self.__server_manager.create_server()
             self.__server.register_action("list-dataprocessor-mock", list_dataprocessor_mock)
             self.__server.register_action("list-dataprocessor", list_dataprocessor)
             self.__server.register_action("set-graph", self._set_graph_handler)
             self.__server.register_action("get-graph", self.export)
             self.__server.register_action("combine", self._combine_handler)
 
-        render = PGraphRenderer()
+        render = PreprocessingGraphRenderer()
         return display(
             HTML(
                 render.show(
                     server_id=self.__server.pk, env=self.__server_manager.check_env(), width=width, height=height
                 )
             )
         )
 
     def export(self, payload: dict[str, Any]) -> dict:
         """
-        Show ``PGraph`` as a dict.
+        Show ``PreprocessingGraph`` as a dict.
 
         Parameters
         ----------
         payload : dict
 
         Returns
         -------
@@ -263,24 +267,25 @@
 
     def _combine_handler(self, payload: CombineHandlerPayload) -> None:
         node = self._find_node(payload["node_pk"])
         if not node:
             raise ServerErrorWithResponse(message="node not found!", type="unexpected_error")
         self.combine_result = self.combine(node)
 
-    def _set_graph_handler(self, payload: Payload) -> None:
+    def _set_graph_handler(self, payload: Payload) -> dict:
         current_graph = self._ngraph
         current_root = self.root
 
         def restore_graph() -> None:
             self._ngraph = current_graph
             self.root = current_root
 
         try:
             self._set_graph(payload=payload)
+            return self.export({})
         except ServerErrorWithResponse as err:
             restore_graph()
             raise err
         except Exception as err:
             restore_graph()
             raise ServerErrorWithResponse(message=str(err), type="unexpected_error")
```

### Comparing `retentioneering-3.0.0b1/retentioneering/nodelist/nodelist.py` & `retentioneering-3.0.0b2/retentioneering/nodelist/nodelist.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b1/retentioneering/params_model/params_model.py` & `retentioneering-3.0.0b2/retentioneering/params_model/params_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -86,23 +86,25 @@
                 params_schema["required"].append(field_name)
 
             if field_type_classname == "Callable" or field_type_classname_legacy == "Callable":
                 params_schema["properties"][field_name] = {
                     "title": field_name.title(),
                     "type": "callable",
                 }
+            params_schema["properties"][field_name]["default"] = field.default
+
         properties: dict[str, dict] = params_schema.get("properties", {})
         required: list[str] = params_schema.get("required", [])
         optionals = {name: name not in required for name in properties.keys()}
         definitions = params_schema.get("definitions", {})
         widgets = {}
         custom_widgets = cls._widgets
         for name, params in properties.items():
             custom_widget: dict[str, Any] | None = None
-            default = params.get("default")
+            default = params.get("default", None)
             if name in custom_widgets:  # type: ignore
                 custom_widget = cls._parse_custom_widget(name=name, optional=optionals[name])
 
             if "$ref" in params or "allOf" in params:
                 widget: dict[str, Any] = cls._parse_schema_definition(
                     params=params, definitions=definitions, default=default, optional=optionals[name]
                 )
@@ -115,30 +117,69 @@
                     params, definitions, default=default, optional=optionals[name]
                 )
             else:
                 widget = cls._parse_simple_widget(name, params, optional=optionals[name], default=default)
 
             if custom_widget:
                 custom_widget_data = {
-                    "default": widget.get("default", None),
+                    "default": cls._get_serialized_default_value(
+                        field_name=name,
+                        widget_type=custom_widget.get("widget", None),
+                        field_default=default,
+                        widget_default=custom_widget.get("default", None),
+                    ),
                     "optional": widget.get("optional", False),
                     "name": widget["name"] if "name" not in custom_widget else None,
                 }
                 if isinstance(custom_widget_data["name"], str):
                     custom_widget_data["name"] = custom_widget_data["name"].lower().replace(" ", "_")
 
                 custom_widget.update(clear_dict(custom_widget_data))
                 widgets[name] = custom_widget
             elif widget:
+                widget["default"] = cls._get_serialized_default_value(
+                    field_name=name,
+                    widget_type=widget.get("widget", None),
+                    field_default=default,
+                    widget_default=widget.get("default", None),
+                )
                 widgets[name] = widget
             else:
                 raise ValueError("Not created widget")
         return widgets  # type: ignore
 
     @classmethod
+    def _get_serialized_default_value(
+        cls, field_name: str, widget_type: Optional[str] = None, field_default: Any = None, widget_default: Any = None
+    ) -> Any:
+        widget = WIDGET_MAPPING.get(widget_type, None) if widget_type else None
+        default = widget_default if field_default is None else field_default
+
+        # если дефолтного значения нет - значит его не нужно сериализовывать
+        if default is None:
+            return default
+
+        serialize: None | Callable = None
+
+        if field_name in cls._widgets:
+            custom_widget = cls._widgets[field_name]  # type: ignore
+            if isinstance(custom_widget, dict):
+                serialize = custom_widget.get("_serialize", None)
+            elif hasattr(custom_widget, "_serialize"):
+                serialize = custom_widget._serialize
+
+        if widget and hasattr(widget, "_serialize"):
+            serialize = widget._serialize  # type: ignore
+
+        if serialize is not None:
+            return serialize(default)
+
+        return default
+
+    @classmethod
     def _parse_schema_definition(
         cls,
         params: dict[str, dict[str, Any]] | Any,
         definitions: dict[str, Any],
         default: Any | None = None,
         optional: bool = True,
     ) -> dict[str, Any]:
@@ -198,15 +239,15 @@
         widget_type = params.get("type")
         if widget_type == "array":
             widget_type = "enum"
         try:
             items = params.get("items", [{}])[-1]
         except KeyError:
             items = params.get("items", [{}])
-        widget_params = dict(optional=optional, name=name, widget=widget_type)
+        widget_params = dict(optional=optional, name=name, widget=widget_type, default=default)
 
         if "enum" in items and widget_type != "enum":
             widget_type = "enum"
             widget_params["params"] = items["enum"]  # type: ignore
 
         return widget_params
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `retentioneering-3.0.0b1/retentioneering/params_model/registry.py` & `retentioneering-3.0.0b2/retentioneering/params_model/registry.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b1/retentioneering/templates/p_graph/p_graph.html` & `retentioneering-3.0.0b2/retentioneering/templates/preprocessing_graph/preprocessing_graph.html`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b1/retentioneering/templates/p_graph/show.py` & `retentioneering-3.0.0b2/retentioneering/templates/preprocessing_graph/show.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import uuid
 
 from jinja2 import Environment, FileSystemLoader, PackageLoader, Template
 
 
-class PGraphRenderer:
+class PreprocessingGraphRenderer:
     __template: Template
     __environment: Environment
 
     def __init__(self) -> None:
         self.__environment = Environment(
-            loader=PackageLoader(package_name="retentioneering", package_path="templates/p_graph"),
+            loader=PackageLoader(package_name="retentioneering", package_path="templates/preprocessing_graph"),
         )
-        self.__template = self.__environment.get_template("p_graph.html")
+        self.__template = self.__environment.get_template("preprocessing_graph.html")
 
     def show(self, server_id: str, env: str, width: int, height: int) -> str:
         return self.__template.render(
             server_id=server_id,
             env=env,
             block_id=str(uuid.uuid4()),
             width=width,
```

### Comparing `retentioneering-3.0.0b1/retentioneering/templates/transition_graph/full.html` & `retentioneering-3.0.0b2/retentioneering/templates/transition_graph/full.html`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b1/retentioneering/templates/transition_graph/init_template.py` & `retentioneering-3.0.0b2/retentioneering/templates/transition_graph/init_template.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b1/retentioneering/templates/transition_graph/inner_iframe.html` & `retentioneering-3.0.0b2/retentioneering/templates/transition_graph/inner_iframe.html`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b1/retentioneering/templates/transition_graph/show.py` & `retentioneering-3.0.0b2/retentioneering/templates/transition_graph/show.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b1/retentioneering/tooling/clusters/clusters.py` & `retentioneering-3.0.0b2/retentioneering/tooling/clusters/clusters.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,101 +57,101 @@
         self.__is_fitted: bool = False
 
         self._method: Method | None = None
         self._n_clusters: int | None = None
         self._user_clusters: pd.Series | None = None
         self._feature_type: FeatureType | None = None
         self._ngram_range: NgramRange | None = None
-        self._vector: pd.DataFrame | None = None
+        self._X: pd.DataFrame | None = None
 
     # public API
 
     def fit(
         self,
         method: Method,
         n_clusters: int,
         feature_type: FeatureType | None = None,
         ngram_range: NgramRange | None = None,
-        vector: pd.DataFrame | None = None,
+        X: pd.DataFrame | None = None,
     ) -> Clusters:
         """
         Prepare features and compute clusters for the input eventstream data.
 
         Parameters
         ----------
         method : {"kmeans", "gmm"}
             - ``kmeans`` stands for the classic K-means algorithm.
               See details in :sklearn_kmeans:`sklearn documentation<>`.
             - ``gmm`` stands for Gaussian mixture model. See details in :sklearn_gmm:`sklearn documentation<>`.
 
         n_clusters : int
             The expected number of clusters to be passed to a clustering algorithm.
-        feature_type : {"tfidf", "count", "frequency", "binary", "markov", "time", "time_fraction"}, default None
+        feature_type : {"tfidf", "count", "frequency", "binary", "markov", "time", "time_fraction"}, optional
             See :py:func:`extract_features`.
         ngram_range : Tuple(int, int), optional
             See :py:func:`extract_features`.
-        vector : pd.DataFrame, optional
+        X : pd.DataFrame, optional
             ``pd.DataFrame`` representing a custom vectorization of the user paths. The index corresponds to user_ids,
             the columns are vectorized values of the path.
 
         Returns
         -------
         Clusters
             A fitted ``Clusters`` instance.
 
 
         """
 
-        self._method, self._n_clusters, self._feature_type, self._ngram_range, self._vector = self.__validate_input(
-            method, n_clusters, feature_type, ngram_range, vector
+        self._method, self._n_clusters, self._feature_type, self._ngram_range, self._X = self.__validate_input(
+            method, n_clusters, feature_type, ngram_range, X
         )
 
         self.__features, self.__cluster_result = self._prepare_clusters()
         self._user_clusters = self.__cluster_result.copy()
 
         self.__segments = Segments(
             eventstream=self.__eventstream,
             segments_df=self.__cluster_result.to_frame("segment").reset_index(),
         )
 
         self.__is_fitted = True
 
         return self
 
-    def event_dist(
+    def diff(
         self,
-        cluster_id1: int,
-        cluster_id2: int | None = None,
-        top_n: int = 8,
+        cluster_id1: int | str,
+        cluster_id2: int | str | None = None,
+        top_n_events: int = 8,
         weight_col: str | None = None,
         targets: list[str] | None = None,
     ) -> go.Figure:
         """
-        Plots a bar plot illustrating the distribution of ``top_n`` events in cluster ``cluster_id1``
+        Plots a bar plot illustrating the distribution of ``top_n_events`` in cluster ``cluster_id1``
         compared with the entire dataset or the cluster ``cluster_id2`` if specified.
         Should be used after :py:func:`fit` or :py:func:`set_clusters`.
 
 
         Parameters
         ----------
-        cluster_id1 : int
+        cluster_id1 : int or str
             ID of the cluster to compare.
-        cluster_id2 : int, optional
+        cluster_id2 : int or str, optional
             ID of the second cluster to compare with the first
             cluster. If ``None``, then compares with the entire dataset.
-        top_n : int, default 8
+        top_n_events : int, default 8
             Number of top events.
         weight_col : str, optional
             If ``None``, distribution will be compared based on event occurrences in
             datasets. If ``weight_col`` is specified, percentages of users
             (column name specified by parameter ``weight_col``) who have particular
             events will be plotted.
-        targets : list of str, optional
+        targets : str or list of str, optional
             List of event names always to include for comparison, regardless
-            of the parameter top_n value. Target events will appear in the same
+            of the parameter top_n_events value. Target events will appear in the same
             order as specified.
 
 
 
         Returns
         -------
         matplotlib.axes.Axes
@@ -161,27 +161,30 @@
             raise RuntimeError("Clusters are not defined. Consider to run 'fit()' or `set_clusters()` methods.")
 
         cluster1 = self.filter_cluster(cluster_id1).to_dataframe()
 
         if targets is None:
             targets = []
 
+        if isinstance(targets, str):
+            targets = [targets]
+
         if weight_col is not None:
             cluster1 = cluster1.drop_duplicates(subset=[self.event_col, weight_col])
             top_cluster = cluster1[self.event_col].value_counts() / cluster1[weight_col].nunique()
 
         else:
             top_cluster = cluster1[self.event_col].value_counts(normalize=True)
 
         # add zero events for missing targets
         for event in set(targets) - set(top_cluster.index):  # type: ignore
             top_cluster.loc[event] = 0
 
-        # create events order: top_n non-target events + targets:
-        events_to_keep = top_cluster[lambda x: ~x.index.isin(targets)].iloc[:top_n].index.tolist()  # type: ignore
+        # create events order: top_n_events (non-target) + targets:
+        events_to_keep = top_cluster[lambda x: ~x.index.isin(targets)].iloc[:top_n_events].index.tolist()  # type: ignore
         target_separator_position = len(events_to_keep)
         events_to_keep += list(targets)
         top_cluster = top_cluster.loc[events_to_keep].reset_index()  # type: ignore
 
         if cluster_id2 is None:
             cluster2 = self.__eventstream.to_dataframe()
         else:
@@ -195,25 +198,25 @@
             # get events distribution from cluster 2:
             top_all = cluster2[self.event_col].value_counts(normalize=True)
 
         # make sure top_all has all events from cluster 1
         for event in set(top_cluster["index"]) - set(top_all.index):
             top_all.loc[event] = 0
 
-        # keep only top_n events from cluster1
+        # keep only top_n_events from cluster1
         top_all = top_all.loc[top_cluster["index"]].reset_index()  # type: ignore
 
         top_all.columns = [self.event_col, "freq"]  # type: ignore
         top_cluster.columns = [self.event_col, "freq"]  # type: ignore
 
         top_all["hue"] = "all" if cluster_id2 is None else f"cluster {cluster_id2}"
         top_cluster["hue"] = f"cluster {cluster_id1}"
 
         total_size = self.__eventstream.to_dataframe()[self.user_col].nunique()
-        figure = self._plot_event_dist(
+        figure = self._plot_diff(
             top_all.append(top_cluster, ignore_index=True, sort=False),
             cl1=cluster_id1,
             sizes=[
                 cluster1[self.user_col].nunique() / total_size,
                 cluster2[self.user_col].nunique() / total_size,
             ],
             weight_col=weight_col,
@@ -227,15 +230,15 @@
     def plot(self, targets: list[str] | list[list[str]] | None = None) -> go.Figure:
         """
         Plot a bar plot illustrating the cluster sizes and the conversion rates of
         the ``target`` events within the clusters. Should be used after :py:func:`fit` or :py:func:`set_clusters`.
 
         Parameters
         ----------
-        targets : list of str (optional, default None)
+        targets : list of str, optional
             Represents the list of the target events
 
         """
         if not self.__is_fitted:
             raise RuntimeError("Clusters are not defined. Consider to run 'fit()' or `set_clusters()` methods.")
 
         target_names, targets_bool = self._prepare_targets(targets)  # type: ignore
@@ -433,33 +436,33 @@
 
         return cast(pd.DataFrame, vec_data)
 
     def projection(
         self,
         method: PlotProjectionMethod = "tsne",
         targets: list[str] | None = None,
-        plot_type: Literal["targets", "clusters"] = "clusters",
+        color_type: Literal["targets", "clusters"] = "clusters",
         **kwargs: Any,
     ) -> go.Figure:
         """
         Show the clusters' projection on a plane, applying dimension reduction techniques.
         Should be used after :py:func:`fit` or :py:func:`set_clusters`.
 
         Parameters
         ----------
         method : {'umap', 'tsne'}, default 'tsne'
             Type of manifold transformation.
-        plot_type : {'targets', 'clusters'}, default 'clusters'
+        color_type : {'targets', 'clusters'}, default 'clusters'
             Type of color-coding used for projection visualization:
 
             - ``clusters`` colors trajectories with different colors depending on cluster number.
             - ``targets`` colors trajectories based on reach to any event provided in 'targets' parameter.
               Must provide ``targets`` parameter in this case.
 
-        targets : list or tuple of str, optional
+        targets : str or list of str, optional
             Vector of event_names as str. If user reaches any of the specified events, the dot corresponding
             to this user will be highlighted as converted on the resulting projection plot.
 
         **kwargs : optional
             Parameters for :sklearn_tsne:`sklearn.manifold.TSNE()<>` and :umap:`umap.UMAP()<>`.
 
         Returns
@@ -470,40 +473,43 @@
 
         if self.__features is None or self.__is_fitted is False:
             raise RuntimeError("Clusters and features must be defined. Consider to run 'fit()' method.")
 
         if targets is None:
             targets = []
 
-        if plot_type == "clusters":
+        if isinstance(targets, str):
+            targets = [targets]
+
+        if color_type == "clusters":
             if self.__cluster_result is not None:
                 targets_mapping = self.__cluster_result.values
                 legend_title = "cluster number:"
             else:
                 raise RuntimeError("Clusters are not defined. Consider to run 'fit()' or `set_clusters()` methods.")
 
-        elif plot_type == "targets":
+        elif color_type == "targets":
             if (not targets) and (len(targets) < 1):
                 raise ValueError(
-                    "When plot_type='targets' is set, 'targets' must be defined as list of target event names"
+                    "When color_type='targets' is set, 'targets' must be defined as list of target event names"
                 )
             else:
                 targets = [list(pd.core.common.flatten(targets))]  # type: ignore
                 legend_title = "conversion to (" + " | ".join(targets[0]).strip(" | ") + "):"  # type: ignore
                 # @TODO: fix 'groupby + apply' inefficient combination. Vladimir Kukushkin
                 targets_mapping = (
                     self.__eventstream.to_dataframe()
                     .groupby(self.user_col)[self.event_col]
                     .apply(lambda x: bool(set(*targets) & set(x)))
                     .to_frame()
                     .sort_index()[self.event_col]
                     .values
                 )
         else:
-            raise ValueError("Unexpected plot type: %s. Allowed values: clusters, targets" % plot_type)
+            raise ValueError("Unexpected plot type: %s. Allowed values: clusters, targets" % color_type)
 
         features = self.__features
 
         if method == "tsne":
             projection: pd.DataFrame = self._learn_tsne(features, **kwargs)
         elif method == "umap":
             projection = self._learn_umap(features, **kwargs)
@@ -523,54 +529,54 @@
     # inner functions
     def __validate_input(
         self,
         method: Method,
         n_clusters: int,
         feature_type: FeatureType | None = None,
         ngram_range: NgramRange | None = None,
-        vector: pd.DataFrame | None = None,
+        X: pd.DataFrame | None = None,
     ) -> tuple[Method | None, int | None, FeatureType | None, NgramRange | None, pd.DataFrame | None]:
         _method = method or self._method
         _n_clusters = n_clusters or self._n_clusters
         _user_clusters = None
 
-        if vector is not None:
-            if not isinstance(vector, pd.DataFrame):  # type: ignore
+        if X is not None:
+            if not isinstance(X, pd.DataFrame):  # type: ignore
                 raise ValueError("Vector is not a DataFrame!")
-            if np.all(np.all(vector.dtypes == "float") and vector.isna().sum().sum() != 0):
+            if np.all(np.all(X.dtypes == "float") and X.isna().sum().sum() != 0):
                 raise ValueError(
                     "Vector is wrong formatted! NaN should be replaced with 0 and all dtypes must be float!"
                 )
             if feature_type:
                 raise ValueError("Both 'vector' and 'feature_type' are defined. 'feature_type' will be ignored.")
             if ngram_range:
                 raise ValueError("Both 'vector' and 'ngram_range' are defined. 'ngram_range' will be ignored.")
 
-            _vector = vector
+            _X = X
             _feature_type = None
             _ngram_range = None
         else:
             _feature_type = feature_type or self._feature_type
             _ngram_range = ngram_range or self._ngram_range
-            _vector = vector or self._vector
+            _X = X or self._X
 
             if _feature_type is None:
                 raise ValueError("'feature_type' must be defined for fitting.")
 
             if _ngram_range is None:
                 raise ValueError("'ngram_range' must be defined for fitting.")
 
-        return _method, _n_clusters, _feature_type, _ngram_range, _vector
+        return _method, _n_clusters, _feature_type, _ngram_range, _X
 
     def _prepare_clusters(self) -> tuple[pd.DataFrame, pd.Series]:
         features = pd.DataFrame()
         user_clusters = pd.Series(dtype=np.int64)
 
-        if self._vector is not None:
-            features = self._vector.copy()
+        if self._X is not None:
+            features = self._X.copy()
         else:
             if self._feature_type is not None and self._ngram_range is not None:
                 features = self.extract_features(self._feature_type, self._ngram_range)
 
         if self._n_clusters is not None:
             if self._method == "kmeans":
                 cluster_result = self._kmeans(features=features, n_clusters=self._n_clusters)
@@ -793,23 +799,23 @@
                 )
 
         else:
             targets_bool = [np.array([False] * len(self.__cluster_result))]
             target_names = [" "]
         return target_names, targets_bool
 
-    def _plot_event_dist(
+    def _plot_diff(
         self,
         bars: pd.DataFrame,
-        cl1: int,
+        cl1: int | str,
         sizes: list[float],
         weight_col: str | None,
         target_pos: int,
         targets: list[str],
-        cl2: int | None,
+        cl2: int | str | None,
     ) -> go.Figure:
         event_col = self.__eventstream.schema.event_name
 
         fig_x_size = round(2 + (bars.shape[0] // 2) ** 0.8)
         rcParams["figure.figsize"] = fig_x_size, 6
 
         bar = sns.barplot(
```

### Comparing `retentioneering-3.0.0b1/retentioneering/tooling/clusters/segments.py` & `retentioneering-3.0.0b2/retentioneering/tooling/clusters/segments.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b1/retentioneering/tooling/clusters/userlist.py` & `retentioneering-3.0.0b2/retentioneering/tooling/clusters/userlist.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b1/retentioneering/tooling/cohorts/cohorts.py` & `retentioneering-3.0.0b2/retentioneering/tooling/cohorts/cohorts.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 from typing import Literal, Tuple
 
+import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import seaborn as sns
 
 from retentioneering.constants import DATETIME_UNITS, DATETIME_UNITS_LIST
 from retentioneering.eventstream.types import EventstreamType
@@ -213,81 +214,84 @@
         )
         user_retention.index = user_retention.index.astype(str)
         if self.average:
             user_retention.loc["Average"] = user_retention.mean()
 
         self._cohort_matrix_result = user_retention
 
-    def heatmap(self, figsize: Tuple[float, float] = (10, 10)) -> sns.heatmap:
+    def heatmap(self, width: float = 5.0, height: float = 5.0) -> matplotlib.axes.Axes:
         """
         Builds a heatmap based on the calculated cohort matrix values.
         Should be used after :py:func:`fit`.
 
         Parameters
         ----------
-        figsize: Tuple[float, float], default (10, 10)
-            Is a tuple of the width and height of the figure in inches.
+        width : float, default 5.0
+            Width of the figure in inches.
+        height : float, default 5.0
+            Height of the figure in inches.
+
 
         Returns
         -------
-        sns.heatmap
+        matplotlib.axes.Axes
         """
 
         df = self._cohort_matrix_result
-
-        figure = plt.figure(figsize=figsize)
-        sns.heatmap(df, annot=True, fmt=".1%", linewidths=1, linecolor="gray")
-        return figure
+        figsize = (width, height)
+        figure, ax = plt.subplots(figsize=figsize)
+        sns.heatmap(df, annot=True, fmt=".1%", linewidths=1, linecolor="gray", ax=ax)
+        return ax
 
     def lineplot(
-        self,
-        show_plot: Literal["cohorts", "average", "all"] = "cohorts",
-        figsize: Tuple[float, float] = (10, 10),
-    ) -> sns.lineplot:
+        self, show_plot: Literal["cohorts", "average", "all"] = "cohorts", width: float = 7.0, height: float = 5.0
+    ) -> matplotlib.axes.Axes:
         """
         Create a chart representing each cohort dynamics over time.
         Should be used after :py:func:`fit`.
 
         Parameters
         ----------
         show_plot: 'cohorts', 'average' or 'all'
             - if ``cohorts`` - shows a lineplot for each cohort,
             - if ``average`` - shows a lineplot only for the average values over all the cohorts,
             - if ``all`` - shows a lineplot for each cohort and also for their average values.
-        figsize: Tuple[float, float], default (10, 10)
-            Is a tuple of the width and height of the figure in inches.
+        width : float, default 7.0
+            Width of the figure in inches.
+        height : float, default 5.0
+            Height of the figure in inches.
 
         Returns
         -------
-        sns.lineplot
+        matplotlib.axes.Axes
 
         """
         if show_plot not in ["cohorts", "average", "all"]:
             raise ValueError("show_plot parameter should be 'cohorts', 'average' or 'all'!")
-
+        figsize = (width, height)
         df_matrix = self._cohort_matrix_result
         df_wo_average = df_matrix[df_matrix.index != "Average"]  # type: ignore
         if show_plot in ["all", "average"] and "Average" not in df_matrix.index:  # type: ignore
             df_matrix.loc["Average"] = df_matrix.mean()  # type: ignore
         df_average = df_matrix[df_matrix.index == "Average"]  # type: ignore
-        figure = plt.figure(figsize=figsize)
+        figure, ax = plt.subplots(figsize=figsize)
         if show_plot == "all":
-            sns.lineplot(df_wo_average.T, lw=1.5)
-            sns.lineplot(df_average.T, lw=2.5, palette=["red"], marker="X", markersize=8, alpha=0.6)
+            sns.lineplot(df_wo_average.T, lw=1.5, ax=ax)
+            sns.lineplot(df_average.T, lw=2.5, palette=["red"], marker="X", markersize=8, alpha=0.6, ax=ax)
 
         if show_plot == "average":
-            sns.lineplot(df_average.T, lw=2.5, palette=["red"], marker="X", markersize=8, alpha=0.6)
+            sns.lineplot(df_average.T, lw=2.5, palette=["red"], marker="X", markersize=8, alpha=0.6, ax=ax)
 
         if show_plot == "cohorts":
-            sns.lineplot(df_wo_average.T, lw=1.5)
+            sns.lineplot(df_wo_average.T, lw=1.5, ax=ax)
 
-        plt.legend(loc="upper left", bbox_to_anchor=(1, 1))
-        plt.xlabel("Period from the start of observation")
-        plt.ylabel("Share of active users")
-        return figure
+        ax.legend(loc="upper left", bbox_to_anchor=(1, 1))
+        ax.set_xlabel("Period from the start of observation")
+        ax.set_ylabel("Share of active users")
+        return ax
 
     @property
     def values(self) -> pd.DataFrame:
         """
         Returns a pd.DataFrame representing the calculated cohort matrix values.
         Should be used after :py:func:`fit`.
```

### Comparing `retentioneering-3.0.0b1/retentioneering/tooling/describe/describe.py` & `retentioneering-3.0.0b2/retentioneering/tooling/_describe/_describe.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import numpy as np
 import pandas as pd
 from numpy import timedelta64
 
 from retentioneering.eventstream.types import EventstreamType
 
 
-class Describe:
-    OUT_COLS = ["value"]
-    INDEX_NAMES = ["category", "metric"]
+class _Describe:
+    OUT_COLS = ("value",)
+    INDEX_NAMES = ("category", "metric")
     TIME_ROUND_UNIT = "s"
 
     def __init__(
         self, eventstream: EventstreamType, session_col: str = "session_id", raw_events_only: bool = False
     ) -> None:
         self.__eventstream = eventstream
         self.user_col = self.__eventstream.schema.user_id
@@ -35,19 +35,19 @@
 
         if raw_events_only:
             self.df = self.df[self.df[self.type_col].isin(["raw"])]
 
     def _calc_statistics(self, agg_col: str) -> list[np.timedelta64 | int | float]:
         df_agg = self.df.groupby(agg_col).agg({self.time_col: ["min", "max"], self.event_col: ["count"]}).reset_index()
         time_diff_user = df_agg[(self.time_col, "max")] - df_agg[(self.time_col, "min")]
-        mean_time_agg_col = time_diff_user.mean().round(Describe.TIME_ROUND_UNIT)  # type: ignore
-        median_time_agg_col = time_diff_user.median().round(Describe.TIME_ROUND_UNIT)  # type: ignore
-        std_time_agg_col = time_diff_user.std().round(Describe.TIME_ROUND_UNIT)  # type: ignore
-        min_length_time_agg_col = time_diff_user.min().round(Describe.TIME_ROUND_UNIT)  # type: ignore
-        max_length_time_agg_col = time_diff_user.max().round(Describe.TIME_ROUND_UNIT)  # type: ignore
+        mean_time_agg_col = time_diff_user.mean().round(self.TIME_ROUND_UNIT)  # type: ignore
+        median_time_agg_col = time_diff_user.median().round(self.TIME_ROUND_UNIT)  # type: ignore
+        std_time_agg_col = time_diff_user.std().round(self.TIME_ROUND_UNIT)  # type: ignore
+        min_length_time_agg_col = time_diff_user.min().round(self.TIME_ROUND_UNIT)  # type: ignore
+        max_length_time_agg_col = time_diff_user.max().round(self.TIME_ROUND_UNIT)  # type: ignore
 
         event_count_agg_col = df_agg[(self.event_col, "count")]
         mean_event_agg_col = round(event_count_agg_col.mean(), 2)  # type: ignore
         median_event_agg_col = event_count_agg_col.median()
         std_event_agg_col = round(event_count_agg_col.std(), 2)  # type: ignore
         min_event_length_agg_col = event_count_agg_col.min()
         max_event_length_agg_col = event_count_agg_col.max()
@@ -66,36 +66,39 @@
         ]
         return values_time_events  # type: ignore
 
     def _output_df_construction(
         self, values_overall: list[timedelta64 | int | float], values_time_events: list[timedelta64 | int | float]
     ) -> pd.DataFrame:
         overall_index = pd.MultiIndex.from_product(self.overall_stats, names=self.INDEX_NAMES)
-        time_events_index = pd.MultiIndex.from_product(self.time_events_stats, names=Describe.INDEX_NAMES)
+        time_events_index = pd.MultiIndex.from_product(self.time_events_stats, names=self.INDEX_NAMES)
 
-        df_overall = pd.DataFrame(data=values_overall, index=overall_index, columns=Describe.OUT_COLS)
-        df_time_events = pd.DataFrame(data=values_time_events, index=time_events_index, columns=Describe.OUT_COLS)
+        df_overall = pd.DataFrame(data=values_overall, index=overall_index, columns=self.OUT_COLS)
+        df_time_events = pd.DataFrame(data=values_time_events, index=time_events_index, columns=self.OUT_COLS)
 
         return pd.concat([df_overall, df_time_events])
 
-    def _describe(self) -> pd.DataFrame:
+    def _values(self) -> pd.DataFrame:
         max_time = self.df[self.time_col].max()
         min_time = self.df[self.time_col].min()
 
         values_overall = [
             self.df[self.user_col].nunique(),
             self.df[self.event_col].nunique(),
-            min_time.round(Describe.TIME_ROUND_UNIT),
-            max_time.round(Describe.TIME_ROUND_UNIT),
-            (max_time - min_time).round(Describe.TIME_ROUND_UNIT),
+            min_time.round(self.TIME_ROUND_UNIT),
+            max_time.round(self.TIME_ROUND_UNIT),
+            (max_time - min_time).round(self.TIME_ROUND_UNIT),
         ]
 
         values_time_events = self._calc_statistics(self.user_col)
 
         if self.has_session_col:
             self.time_events_stats[0] += ["session_length_time", "session_length_steps"]
             self.overall_stats[1].insert(2, "unique_sessions")
 
             values_overall.insert(2, self.df[self.session_col].nunique())
             values_time_events += self._calc_statistics(self.session_col)
 
         return self._output_df_construction(values_overall, values_time_events)  # type: ignore
+
+
+__all__ = ("_Describe",)
```

### Comparing `retentioneering-3.0.0b1/retentioneering/tooling/describe_events/describe_events.py` & `retentioneering-3.0.0b2/retentioneering/tooling/_describe_events/_describe_events.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import pandas as pd
 
 from retentioneering.eventstream.types import EventstreamType
 
 
-class DescribeEvents:
+class _DescribeEvents:
     TIME_ROUND_UNIT = "s"
     STATS_ORDER = ["mean", "std", "median", "min", "max"]
     UNIQUE_SESS = ("basic_statistics", "unique_sessions")
     SHARE_SESS = ("basic_statistics", "unique_sessions_shared")
 
     def __init__(
         self,
@@ -50,22 +50,22 @@
             df.groupby([self.event_col, agg_col])
             .agg(time_to_FO=(f"__event_{prefix}_timedelta", "first"), steps_to_FO=(f"__event_{prefix}_idx", "first"))
             .reset_index()
         )
         df_agg_event.columns = [self.event_col, self.user_col, first_time, first_event]  # type: ignore
         df_agg_event[first_time] = df_agg_event[first_time].dt.total_seconds()
         df_agg_event = df_agg_event.groupby([self.event_col])[[first_time, first_event]].agg(
-            DescribeEvents.STATS_ORDER  # type: ignore
+            self.STATS_ORDER  # type: ignore
         )
         df_agg_event[(first_event, "mean")] = df_agg_event[(first_event, "mean")].round(2)
         df_agg_event[(first_event, "std")] = df_agg_event[(first_event, "std")].round(2)
 
-        for stat in DescribeEvents.STATS_ORDER:
+        for stat in self.STATS_ORDER:
             mult_ind = (first_time, stat)
-            df_agg_event[mult_ind] = pd.to_timedelta(df_agg_event[mult_ind], unit="s").round(DescribeEvents.TIME_ROUND_UNIT)  # type: ignore
+            df_agg_event[mult_ind] = pd.to_timedelta(df_agg_event[mult_ind], unit="s").round(self.TIME_ROUND_UNIT)  # type: ignore
 
         return df_agg_event
 
     def _create_basic_info_df(self, df: pd.DataFrame) -> pd.DataFrame:
         basic_info = df.groupby("event").agg(
             number_of_occurrences=("event_id", "count"), unique_users=("user_id", "nunique")
         )
@@ -74,22 +74,20 @@
             basic_info["number_of_occurrences"] / self.total_events_base
         ).round(2)
         basic_info["unique_users_shared"] = (basic_info["unique_users"] / self.unique_users_base).round(2)
 
         basic_info.columns = pd.MultiIndex.from_product([["basic_statistics"], basic_info.columns])
 
         if self.has_session_col:
-            basic_info[DescribeEvents.UNIQUE_SESS] = self.df.groupby("event")[self.session_col].agg("nunique")
-            basic_info[DescribeEvents.SHARE_SESS] = (
-                basic_info[DescribeEvents.UNIQUE_SESS] / self.total_sessions_base
-            ).round(2)
+            basic_info[self.UNIQUE_SESS] = self.df.groupby("event")[self.session_col].agg("nunique")
+            basic_info[self.SHARE_SESS] = (basic_info[self.UNIQUE_SESS] / self.total_sessions_base).round(2)
 
         return basic_info
 
-    def _describe(self) -> pd.DataFrame:
+    def _values(self) -> pd.DataFrame:
         df = self._agg_min_time(df=self.df, agg_col=self.user_col, prefix="user")
 
         if self.has_session_col:
             df = self._agg_min_time(df=df, agg_col=self.session_col, prefix="session")
 
         if self.event_list:
             df = df[df[self.event_col].isin(self.event_list)]
@@ -99,9 +97,12 @@
 
         if self.has_session_col:
             df_agg_sess = self._agg_time_events(df=df, agg_col=self.session_col, prefix="session")
             df_agg_event = df_agg_event.merge(df_agg_sess, left_index=True, right_index=True)
 
         res = basic_info.merge(df_agg_event, left_index=True, right_index=True)
         if self.has_session_col:
-            res.insert(2, DescribeEvents.UNIQUE_SESS, res.pop(DescribeEvents.UNIQUE_SESS))  # type: ignore
+            res.insert(2, self.UNIQUE_SESS, res.pop(self.UNIQUE_SESS))  # type: ignore
         return res
+
+
+__all__ = ("_DescribeEvents",)
```

### Comparing `retentioneering-3.0.0b1/retentioneering/tooling/event_timestamp_hist/event_timestamp_hist.py` & `retentioneering-3.0.0b2/retentioneering/tooling/event_timestamp_hist/event_timestamp_hist.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,16 +28,18 @@
     lower_cutoff_quantile : float, optional
         Specify time distance quantile as the lower boundary. The values below the boundary are truncated.
     upper_cutoff_quantile : float, optional
         Specify time distance quantile as the upper boundary. The values above the boundary are truncated.
     bins : int or str, default 20
         Generic bin parameter that can be the name of a reference rule or
         the number of bins. Passed to :numpy_bins_link:`numpy.histogram_bin_edges<>`.
-    figsize : tuple of float, default (12.0, 7.0)
-        Width, height in inches.
+    width : float, default 6.0
+        Width in inches.
+    height : float, default 4.5
+        Height in inches.
 
 
     See Also
     --------
     .TimedeltaHist : Plot the distribution of the time deltas between two events.
     .UserLifetimeHist : Plot the distribution of user lifetimes.
     .Eventstream.describe : Show general eventstream statistics.
@@ -52,15 +54,16 @@
         self,
         eventstream: EventstreamType,
         raw_events_only: bool = False,
         event_list: list[str] | None = None,
         lower_cutoff_quantile: Optional[float] = None,
         upper_cutoff_quantile: Optional[float] = None,
         bins: int | Literal[BINS_ESTIMATORS] = 20,
-        figsize: tuple[float, float] = (12.0, 7.0),
+        width: float = 6.0,
+        height: float = 4.5,
     ) -> None:
         self.__eventstream = eventstream
         self.user_col = self.__eventstream.schema.user_id
         self.event_col = self.__eventstream.schema.event_name
         self.time_col = self.__eventstream.schema.event_timestamp
 
         self.event_list = event_list
@@ -76,15 +79,15 @@
                 raise ValueError("upper_cutoff_quantile should be a fraction between 0 and 1.")
         self.upper_cutoff_quantile = upper_cutoff_quantile
 
         if lower_cutoff_quantile is not None and upper_cutoff_quantile is not None:
             if lower_cutoff_quantile > upper_cutoff_quantile:
                 warnings.warn("lower_cutoff_quantile exceeds upper_cutoff_quantile; no data passed to the histogram")
         self.bins = bins
-        self.figsize = figsize
+        self.figsize = (width, height)
         self.bins_to_show: np.ndarray = np.array([])
         self.values_to_plot: np.ndarray = np.array([])
 
     def _remove_cutoff_values(self, series: pd.Series) -> pd.Series:
         idx = [True] * len(series)
         if self.upper_cutoff_quantile is not None:
             idx &= series <= series.quantile(self.upper_cutoff_quantile)
```

### Comparing `retentioneering-3.0.0b1/retentioneering/tooling/funnel/funnel.py` & `retentioneering-3.0.0b2/retentioneering/tooling/funnel/funnel.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b1/retentioneering/tooling/mixins/ended_events.py` & `retentioneering-3.0.0b2/retentioneering/tooling/mixins/ended_events.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,28 +5,29 @@
 
 
 class EndedEventsMixin:
     def __init__(self) -> None:
         pass
 
     @staticmethod
-    def _add_ended_events(data: pd.DataFrame, schema: EventstreamSchemaType) -> pd.DataFrame:
+    def _add_ended_events(data: pd.DataFrame, schema: EventstreamSchemaType, weight_col: str) -> pd.DataFrame:
         """
         Adds artificial ``ENDED`` event in the end of a path. If a path already
         contains ``path_end`` event, it will be replaced with ``ENDED`` event.
         Otherwise, ``ENDED`` event will be placed into the end of the path.
+        Path is identified by the weight_col parameter which can be user_id, session_id, etc.
         """
         data[schema.event_name] = data[schema.event_name].str.replace("path_end", "ENDED")
-        users_with_ended = data[data[schema.event_name] == "ENDED"][schema.user_id].unique()
+        ids_with_ended = data[data[schema.event_name] == "ENDED"][weight_col].unique()
 
-        paths_with_ended = data[data[schema.user_id].isin(users_with_ended)]
-        paths_without_ended = data[~data[schema.user_id].isin(users_with_ended)]
+        paths_with_ended = data[data[weight_col].isin(ids_with_ended)]
+        paths_without_ended = data[~data[weight_col].isin(ids_with_ended)]
 
         additional_ended_events = (
-            paths_without_ended.groupby(schema.user_id, as_index=False)
+            paths_without_ended.groupby(weight_col, as_index=False)
             .last()
             .assign(
                 **{
                     schema.event_name: "ENDED",
                     schema.event_index: lambda df_: df_[schema.event_index]
                     + (np.where(df_[schema.event_name] == "ENDED", 0.5, 0)),
                 }
```

### Comparing `retentioneering-3.0.0b1/retentioneering/tooling/stattests/stattests.py` & `retentioneering-3.0.0b2/retentioneering/tooling/stattests/stattests.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import seaborn as sns
 from scipy.stats import chi2_contingency, fisher_exact, ks_2samp, mannwhitneyu
 from scipy.stats.contingency import crosstab
 from statsmodels.stats.power import TTestIndPower
 from statsmodels.stats.weightstats import ttest_ind, ztest
 
 from retentioneering.eventstream.types import EventstreamType
-from retentioneering.tooling.stattests.constants import TEST_NAMES
+from retentioneering.tooling.stattests.constants import STATTEST_NAMES
 
 
 def _cohend(d1: list, d2: list) -> float:
     n1, n2 = len(d1), len(d2)
     s1, s2 = np.var(d1, ddof=1), np.var(d2, ddof=1)
     s = float(math.sqrt(((n1 - 1) * s1 + (n2 - 1) * s2) / (n1 + n2 - 2)))
     u1, u2 = float(np.mean(d1)), float(np.mean(d2))
@@ -68,15 +68,15 @@
     See :doc:`StatTests user guide</user_guides/stattests>` for the details.
 
     """
 
     def __init__(
         self,
         eventstream: EventstreamType,
-        test: TEST_NAMES,
+        test: STATTEST_NAMES,
         groups: Tuple[list[str | int], list[str | int]],
         func: Callable,
         group_names: Tuple[str, str] = ("group_1", "group_2"),
         alpha: float = 0.05,
     ) -> None:
         self.__eventstream = eventstream
         self.output_template_numerical = "{0} (mean ± SD): {1:.3f} ± {2:.3f}, n = {3}"
@@ -148,15 +148,15 @@
             if self.test == "chi2_contingency":
                 freq_table = self._get_freq_table(data_max, data_min)
                 p_val = chi2_contingency(freq_table)[1]
             elif self.test == "fisher_exact":
                 freq_table = self._get_freq_table(data_max, data_min)
                 p_val = fisher_exact(freq_table, alternative="greater")[1]
         else:
-            raise ValueError("The argument test is not supported. Supported tests are: {}".format(*TEST_NAMES))  # type: ignore
+            raise ValueError("The argument test is not supported. Supported tests are: {}".format(*STATTEST_NAMES))  # type: ignore
         return p_val, power  # type: ignore
 
     def _get_sorted_test_results(self) -> Tuple[float, float, str, str]:
         p_val_norm, power_norm = self._get_test_results(self.g1_data, self.g2_data)
         p_val_rev, power_rev = self._get_test_results(self.g2_data, self.g1_data)
         if p_val_norm < p_val_rev:
             p_val = p_val_norm
@@ -250,23 +250,23 @@
             )
             print(
                 self.output_template_numerical.format(
                     values["group_two_name"], values["group_two_mean"], values["group_two_SD"], values["group_two_size"]
                 )
             )
             print(
-                "'{0}' is greater than '{1}' with P-value: {2:.5f}".format(
+                "'{0}' is greater than '{1}' with p-value: {2:.5f}".format(
                     values["greatest_group_name"], values["least_group_name"], values["p_val"]
                 )
             )
             print("power of the test: {0:.2f}%".format(100 * values["power_estimated"]))
         elif self.test in ["chi2_contingency", "fisher_exact"]:
             print(self.output_template_categorical.format(values["group_one_name"], values["group_one_size"]))
             print(self.output_template_categorical.format(values["group_two_name"], values["group_two_size"]))
-            print("Group difference test with P-value: {:.5f}".format(values["p_val"]))
+            print("Group difference test with p-value: {:.5f}".format(values["p_val"]))
         else:
             raise ValueError("Wrong test passed")
 
     @property
     def params(self) -> dict:
         """
         Returns the parameters used for the last fitting.
```

### Comparing `retentioneering-3.0.0b1/retentioneering/tooling/step_matrix/step_matrix.py` & `retentioneering-3.0.0b2/retentioneering/tooling/step_matrix/step_matrix.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         - If ``both``, show step values and accumulated values.
         - If ``only``, show targets only as accumulated.
     sorting : list of str, optional
         - If list of event names specified - lines in the heatmap will be shown in
           the passed order.
         - If ``None`` - rows will be ordered according to i`th value (first row,
           where 1st element is max; second row, where second element is max; etc)
-    thresh : float, default=0
+    threshold : float, default=0
         Used to remove rare events. Aggregates all rows where all values are
         less than the specified threshold.
     centered : dict, optional
         Parameter used to align user paths at a specific event at a specific step.
         Has to contain three keys:
         - ``event``: str, name of event to align.
         - ``left_gap``: int, number of events to include before specified event.
@@ -83,15 +83,15 @@
         of user_id`s. Two separate step_matrices M1 and M2 will be calculated
         for users from g_1 and g_2, respectively. Resulting matrix will be the matrix
         M = M1-M2.
 
     Notes
     -----
     During step matrix calculation an artificial ``ENDED`` event is created. If a path already
-    contains ``path_end`` event (See :py:class:`.StartEndEvents`), it
+    contains ``path_end`` event (See :py:class:`.AddStartEndEvents`), it
     will be temporarily replaced with ``ENDED`` (within step matrix only). Otherwise, ``ENDED``
     event will be explicitly added to the end of each path.
 
     Event ``ENDED`` is cumulated so that the values in its row are summed up from
     the first step to the last. ``ENDED`` row is always placed at the last line of step matrix.
     This design guarantees that the sum of any step matrix's column is 1
     (0 for a differential step matrix).
@@ -102,25 +102,26 @@
     --------
     .Eventstream.step_matrix : Call StepMatrix tool as an eventstream method.
     .StepSankey : A class for the visualization of user paths in stepwise manner using Sankey diagram.
     .CollapseLoops : Find loops and create new synthetic events in the paths of all users having such sequences.
     """
 
     __eventstream: EventstreamType
+    ENDED_EVENT = "ENDED"
 
     def __init__(
         self,
         eventstream: EventstreamType,
         max_steps: int = 20,
         weight_col: Optional[str] = None,
         precision: int = 2,
         targets: Optional[list[str] | str] = None,
         accumulated: Optional[Union[Literal["both", "only"], None]] = None,
         sorting: Optional[list[str]] = None,
-        thresh: float = 0,
+        threshold: float = 0,
         centered: Optional[dict] = None,
         groups: Optional[Tuple[list, list]] = None,
     ) -> None:
         self.__eventstream = eventstream
         self.user_col = self.__eventstream.schema.user_id
         self.event_col = self.__eventstream.schema.event_name
         self.time_col = self.__eventstream.schema.event_timestamp
@@ -128,15 +129,15 @@
         self.data = self.__eventstream.to_dataframe()
         self.max_steps = max_steps
         self.weight_col = weight_col or self.__eventstream.schema.user_id
         self.precision = precision
         self.targets = targets
         self.accumulated = accumulated
         self.sorting = sorting
-        self.thresh = thresh
+        self.threshold = threshold
         self.centered: CenteredParams | None = CenteredParams(**centered) if centered else None
         self.groups = groups
 
         self.result_data: pd.DataFrame = pd.DataFrame()
         self.result_targets: pd.DataFrame | None = None
         self.fraction_title: str | None = None
         self.targets_list: list[list[str]] | None = None
@@ -212,16 +213,16 @@
         agg.columns = ["event_rank", "event_name", "freq"]  # type: ignore
         piv = agg.pivot(index="event_name", columns="event_rank", values="freq").fillna(0)
         # add missing cols if number of events < max_steps:
         piv = self._pad_cols(piv)
         piv.columns.name = None
         piv.index.name = None
         # MAKE TERMINATED STATE ACCUMULATED:
-        if "ENDED" in piv.index:
-            piv.loc["ENDED"] = piv.loc["ENDED"].cumsum().fillna(0)
+        if self.ENDED_EVENT in piv.index:
+            piv.loc[self.ENDED_EVENT] = piv.loc[self.ENDED_EVENT].cumsum().fillna(0)
         return piv
 
     def _process_targets(self, data: pd.DataFrame) -> tuple[pd.DataFrame | None, list[list[str]] | None]:
         if self.targets is None:
             return None, None
 
         # format targets to list of lists. E.g. [['a', 'b'], 'c'] -> [['a', 'b'], ['c']]
@@ -247,32 +248,34 @@
         # if target is not present in dataset add zeros:
         for i in targets_flatten:
             if i not in piv_targets.index:
                 piv_targets.loc[i] = 0
         piv_targets = piv_targets.loc[targets_flatten].copy()
         piv_targets.columns.name = None
         piv_targets.index.name = None
+        ACC_INDEX = "ACC_"
+
         if self.accumulated == "only":
-            piv_targets.index = map(lambda x: "ACC_" + x, piv_targets.index)  # type: ignore
+            piv_targets.index = map(lambda x: ACC_INDEX + x, piv_targets.index)  # type: ignore
             for i in piv_targets.index:
                 piv_targets.loc[i] = piv_targets.loc[i].cumsum().fillna(0)
 
             # change names is targets list:
             for target in targets:
                 for j, item in enumerate(target):
-                    target[j] = "ACC_" + item
+                    target[j] = ACC_INDEX + item
         if self.accumulated == "both":
             for i in piv_targets.index:
-                piv_targets.loc["ACC_" + i] = piv_targets.loc[i].cumsum().fillna(0)  # type: ignore
+                piv_targets.loc[ACC_INDEX + i] = piv_targets.loc[i].cumsum().fillna(0)  # type: ignore
 
             # add accumulated targets to the list:
             targets_not_acc = deepcopy(targets)
             for target in targets:
                 for j, item in enumerate(target):
-                    target[j] = "ACC_" + item
+                    target[j] = ACC_INDEX + item
             targets = targets_not_acc + targets
         return piv_targets, targets
 
     def _center_matrix(self, data: pd.DataFrame) -> tuple[pd.DataFrame, str]:
         if self.centered is None:
             return pd.DataFrame(), ""
 
@@ -301,17 +304,17 @@
         return data, fraction_title
 
     @staticmethod
     def _sort_matrix(step_matrix: pd.DataFrame) -> pd.DataFrame:
         x = step_matrix.copy()
         order = []
         for i in x.columns:
-            new_r = x[i].idxmax()
+            new_r = x[i].idxmax()  # type: ignore
             order.append(new_r)
-            x = x.drop(new_r)
+            x = x.drop(new_r)  # type: ignore
             if x.shape[0] == 0:
                 break
         order.extend(list(set(step_matrix.index) - set(order)))
         return step_matrix.loc[order]
 
     def _render_plot(
         self,
@@ -386,26 +389,26 @@
             sns.mpl.pyplot.yticks(rotation=0)
             # add vertical lines for central step-matrix
             if self.centered is not None:
                 centered_position = self.centered.left_gap
                 axs.vlines(
                     [centered_position - 0.02, centered_position + 0.98], *axs.get_ylim(), colors="Black", linewidth=0.7
                 )
-        return figure
+        return axs
 
     def fit(self) -> None:
         """
         Calculates the step matrix internal values with the defined parameters.
         Applying ``fit`` method is necessary for the following usage
         of any visualization or descriptive ``StepMatrix`` methods.
 
         """
         weight_col = self.weight_col or self.user_col
         data = self.__eventstream.to_dataframe()
-        data = self._add_ended_events(data, self.__eventstream.schema)
+        data = self._add_ended_events(data=data, schema=self.__eventstream.schema, weight_col=self.weight_col)
         data["event_rank"] = data.groupby(weight_col).cumcount() + 1
 
         # BY HERE WE NEED TO OBTAIN FINAL DIFF piv and piv_targets before sorting, thresholding and plotting:
 
         if self.groups:
             data_pos = data[data[weight_col].isin(self.groups[0])].copy()
             if len(data_pos) == 0:
@@ -425,29 +428,30 @@
                 piv_targets = piv_targets_pos - piv_targets_neg
             else:
                 piv_targets = None
 
         else:
             piv, piv_targets, fraction_title, targets_plot = self._step_matrix_values(data=data)
 
-        thresh_index = "THRESHOLDED_"
-        if self.thresh != 0:
+        threshold_index = "THRESHOLDED_"
+
+        if self.threshold != 0:
             # find if there are any rows to threshold:
-            thresholded = piv.loc[(piv.abs() < self.thresh).all(axis=1) & (piv.index != "ENDED")].copy()
+            thresholded = piv.loc[(piv.abs() < self.threshold).all(axis=1) & (piv.index != self.ENDED_EVENT)].copy()
             if len(thresholded) > 0:
-                piv = piv.loc[(piv.abs() >= self.thresh).any(axis=1) | (piv.index == "ENDED")].copy()
-                thresh_index = f"THRESHOLDED_{len(thresholded)}"
-                piv.loc[thresh_index] = thresholded.sum()
+                piv = piv.loc[(piv.abs() >= self.threshold).any(axis=1) | (piv.index == self.ENDED_EVENT)].copy()
+                threshold_index = f"{threshold_index}{len(thresholded)}"
+                piv.loc[threshold_index] = thresholded.sum()
 
         if self.sorting is None:
             piv = self._sort_matrix(piv)
 
             keep_in_the_end = []
-            keep_in_the_end.append("ENDED") if ("ENDED" in piv.index) else None
-            keep_in_the_end.append(thresh_index) if (thresh_index in piv.index) else None
+            keep_in_the_end.append(self.ENDED_EVENT) if (self.ENDED_EVENT in piv.index) else None
+            keep_in_the_end.append(threshold_index) if (threshold_index in piv.index) else None
 
             events_order = [*(i for i in piv.index if i not in keep_in_the_end), *keep_in_the_end]
             piv = piv.loc[events_order]
 
         else:
             if {*self.sorting} != {*piv.index}:
                 raise ValueError(
@@ -464,26 +468,26 @@
                 piv_targets.columns = [f"{int(i) - window - 1}" for i in piv_targets.columns]  # type: ignore
 
         self.result_data = piv
         self.result_targets = piv_targets
         self.fraction_title = fraction_title
         self.targets_list = targets_plot
 
-    def plot(self) -> sns.heatmap:
+    def plot(self) -> matplotlib.axes.Axes:
         """
         Create a heatmap plot based on the calculated step matrix values.
         Should be used after :py:func:`fit`.
 
         Returns
         -------
-        sns.heatmap
+        matplotlib.axes.Axes
 
         """
-        figure = self._render_plot(self.result_data, self.result_targets, self.targets_list, self.fraction_title)
-        return figure
+        axes = self._render_plot(self.result_data, self.result_targets, self.targets_list, self.fraction_title)
+        return axes
 
     @property
     def values(self) -> tuple[pd.DataFrame, pd.DataFrame | None]:
         """
         Returns the calculated step matrix as a pd.DataFrame.
         Should be used after :py:func:`fit`.
 
@@ -505,11 +509,11 @@
         return {
             "max_steps": self.max_steps,
             "weight_col": self.weight_col,
             "precision": self.precision,
             "targets": self.targets,
             "accumulated": self.accumulated,
             "sorting": self.sorting,
-            "thresh": self.thresh,
+            "threshold": self.threshold,
             "centered": self.centered,
             "groups": self.groups,
         }
```

### Comparing `retentioneering-3.0.0b1/retentioneering/tooling/step_sankey/step_sankey.py` & `retentioneering-3.0.0b2/retentioneering/tooling/step_sankey/step_sankey.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,28 +16,28 @@
     A class for the visualization of user paths in stepwise manner using Sankey diagram.
 
     Parameters
     ----------
     eventstream : EventstreamType
     max_steps : int, default 10
         Maximum number of steps in trajectories to include. Should be > 1.
-    thresh : float | int, default 0.05
+    threshold : float | int, default 0.05
         Used to remove rare events from the plot. An event is collapsed to ``thresholded_N`` artificial event if
-        its maximum frequency across all the steps is less than or equal to ``thresh``. The frequency is set
-        with respect to ``thresh`` type:
+        its maximum frequency across all the steps is less than or equal to ``threshold``. The frequency is set
+        with respect to ``threshold`` type:
 
         - If ``int`` - the frequency is the number of unique users who had given event at given step.
         - If ``float`` - percentage of users: the same as for ``int``, but divided by the number of unique users.
 
         The events which are prohibited for collapsing could be enlisted in ``target`` parameter.
     sorting : list of str, optional
         Define the order of the events visualized at each step. The events that are not represented in the list
         will follow after the events from the list.
-    target : list of str, optional
-        Contain events that are prohibited for collapsing with ``thresh`` parameter.
+    targets : str or list of str, optional
+        Contain events that are prohibited for collapsing with ``threshold`` parameter.
     autosize : bool, default True
         Plotly autosize parameter. See :plotly_autosize:`plotly documentation<>`.
     width : int, optional
         Plot's width (in px). See :plotly_width:`plotly documentation<>`.
     height : int, optional
         Plot's height (in px). See :plotly_height:`plotly documentation<>`.
 
@@ -58,31 +58,31 @@
 
     """
 
     def __init__(
         self,
         eventstream: EventstreamType,
         max_steps: int = 10,
-        thresh: Union[int, float] = 0.05,
+        threshold: Union[int, float] = 0.05,
         sorting: list | None = None,
-        target: Union[list[str], str] | None = None,
+        targets: Union[list[str], str] | None = None,
         autosize: bool = True,
         width: int | None = None,
         height: int | None = None,
     ) -> None:
         self.__eventstream = eventstream
         self.user_col = self.__eventstream.schema.user_id
         self.event_col = self.__eventstream.schema.event_name
         self.time_col = self.__eventstream.schema.event_timestamp
         self.event_index_col = self.__eventstream.schema.event_index
 
         self.max_steps = max_steps
-        self.thresh = thresh
+        self.threshold = threshold
         self.sorting = sorting
-        self.target = target
+        self.targets = targets
         self.autosize = autosize
         self.width = width
         self.height = height
 
         self.data_grp_nodes: pd.DataFrame = pd.DataFrame()
         self.data: pd.DataFrame = pd.DataFrame()
         self.data_grp_links: pd.DataFrame = pd.DataFrame()
@@ -239,48 +239,52 @@
         )
         repeats = pd.DataFrame({self.user_col: np.repeat(pad[self.user_col], pad["repeat_number"])})
         padded_end_events = pd.merge(repeats, data[data[self.event_col] == "ENDED"], on=self.user_col)
         result = pd.concat([data, padded_end_events]).sort_values([self.user_col, self.event_index_col])
         return result
 
     def _prepare_data(self, data: pd.DataFrame) -> pd.DataFrame:
-        data = self._add_ended_events(data, self.__eventstream.schema)
+        data = self._add_ended_events(
+            data=data, schema=self.__eventstream.schema, weight_col=self.__eventstream.schema.user_id
+        )
         data = self._pad_end_events(data)
         # NOTE set new columns using declared functions
         data[self.time_col] = pd.to_datetime(data[self.time_col])
         data["step"] = data.groupby(self.user_col)[self.event_index_col].rank(method="first").astype(int)
         data = data.sort_values(by=["step", self.time_col]).reset_index(drop=True)
         data = self._get_next_event_and_timedelta(data)
 
         # NOTE threshold
         data["event_users"] = data.groupby(by=["step", self.event_col])[self.user_col].transform("nunique")
         data["total_users"] = data.loc[data["step"] == 1, self.user_col].nunique()
         data["perc"] = data["event_users"] / data["total_users"]
 
-        if self.thresh is not None:
-            if isinstance(self.thresh, float):
+        if self.threshold is not None:
+            if isinstance(self.threshold, float):
                 column_to_compare = "perc"
             else:
-                # assume that self.thresh must be of int type here
+                # assume that self.threshold must be of int type here
                 column_to_compare = "event_users"
 
             events_to_keep = ["ENDED"]
-            if self.target is not None:
-                events_to_keep += self.target
+            if self.targets is not None:
+                events_to_keep += self.targets
 
-            thresh_events = (
+            threshold_events = (
                 data.loc[data["step"] <= self.max_steps, :]
                 .groupby(by=self.event_col, as_index=False)[column_to_compare]
                 .max()
                 .loc[
-                    lambda df_: (df_[column_to_compare] <= self.thresh) & (~df_[self.event_col].isin(events_to_keep))
+                    lambda df_: (df_[column_to_compare] <= self.threshold) & (~df_[self.event_col].isin(events_to_keep))
                 ]  # type: ignore
                 .loc[:, self.event_col]
             )
-            data.loc[data[self.event_col].isin(thresh_events), self.event_col] = f"thresholded_{len(thresh_events)}"
+            data.loc[
+                data[self.event_col].isin(threshold_events), self.event_col
+            ] = f"thresholded_{len(threshold_events)}"
 
             # NOTE rearrange the data taking into account recently added thresholded events
             data["step"] = data.groupby(self.user_col)[self.event_index_col].rank(method="first").astype(int)
             data = self._get_next_event_and_timedelta(data)
 
         # NOTE use max_steps for filtering data
         data = data.loc[data["step"] <= self.max_steps, :]
@@ -583,14 +587,14 @@
         """
         Returns the parameters used for the last fitting.
         Should be used after :py:func:`fit`.
 
         """
         return {
             "max_steps": self.max_steps,
-            "thresh": self.thresh,
+            "threshold": self.threshold,
             "sorting": self.sorting,
-            "target": self.target,
+            "targets": self.targets,
             "autosize": self.autosize,
             "width": self.width,
             "height": self.height,
         }
```

### Comparing `retentioneering-3.0.0b1/retentioneering/tooling/timedelta_hist/timedelta_hist.py` & `retentioneering-3.0.0b2/retentioneering/tooling/timedelta_hist/timedelta_hist.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,30 +37,32 @@
         Examples: ('login', 'purchase'); ['start', 'cabinet']
 
         Besides the generic eventstream events, ``event_pair`` can accept special ``eventstream_start`` and
         ``eventstream_end`` events which denote the first and the last event in the entire eventstream correspondingly.
 
         Note that the sequence of events and ``weight_col`` is important.
 
-    only_adjacent_event_pairs : bool, default True
+    adjacent_events_only : bool, default True
         Is used only when ``event_pair`` is not ``None``; specifies whether events need to be
         adjacent to be included.
 
-        For example, if ``event_pair=("login", "purchase")`` and ``only_adjacent_event_pairs=False``,
+        For example, if ``event_pair=("login", "purchase")`` and ``adjacent_events_only=False``,
         then the sequence ("login", "main", "trading", "purchase") will contain a valid pair
-        (which is not the case with only_adjacent_event_pairs=True).
+        (which is not the case with ``adjacent_events_only=True``).
 
-    weight_col : str, default 'user_id'
+    weight_col : str, default None
         Specify a unit of observation, inside which time differences will be computed.
+        By default, the values from ``user_id`` column in :py:class:`.EventstreamSchema` is taken.
+
         For example:
 
         - If ``user_id`` - time deltas will be computed only for events inside each user path.
         - If ``session_id`` - the same, but inside each session.
 
-    aggregation : {None, "mean", "median"}, default None
+    time_agg : {None, "mean", "median"}, default None
         Specify the aggregation policy for the time distances. Aggregate based on passed ``weight_col``.
 
         - If ``None`` - no aggregation;
         - ``mean`` and ``median`` plot distributions of ``weight_col`` unit mean or unit ``median`` timedeltas.
 
         For example, if session id is specified in ``weight_col``, one observation per
         session (for example, session median) will be provided for the histogram.
@@ -75,27 +77,29 @@
     lower_cutoff_quantile : float, optional
         Specify time distance quantile as the lower boundary. The values below the boundary are truncated.
     upper_cutoff_quantile : float, optional
         Specify time distance quantile as the upper boundary. The values above the boundary are truncated.
     bins : int or {"auto", "fd", "doane", "scott", "stone", "rice", "sturges", "sqrt"}, default 20
         Generic bin parameter that can be the name of a reference rule or
         the number of bins. Passed to :numpy_bins_link:`numpy.histogram_bin_edges<>`.
-    figsize : tuple of float, default (6.0, 4.5)
-        Width, height in inches.
+    width : float, default 6.0
+        Width in inches.
+    height : float, default 4.5
+        Height in inches.
 
     See Also
     --------
     .UserLifetimeHist : Plot the distribution of user lifetimes.
     .EventTimestampHist : Plot the distribution of events over time.
     .Eventstream.describe : Show general eventstream statistics.
     .Eventstream.describe_events : Show general eventstream events statistics.
-    .StartEndEvents : Create new synthetic events ``path_start`` and ``path_end`` to each user trajectory.
+    .AddStartEndEvents : Create new synthetic events ``path_start`` and ``path_end`` to each user trajectory.
     .SplitSessions : Create new synthetic events, that divide users’ paths on sessions.
-    .TruncatedEvents : Create new synthetic event(s) for each user based on the timeout threshold.
-    .DeleteUsersByPathLength : Filter user paths based on the path length, removing the paths that are shorter than the
+    .LabelCroppedPaths : Create new synthetic event(s) for each user based on the timeout threshold.
+    .DropPaths : Filter user paths based on the path length, removing the paths that are shorter than the
                                 specified number of events or cut_off.
 
 
     Notes
     -----
     See :ref:`Eventstream user guide<eventstream_timedelta_hist>` for the details.
     """
@@ -104,58 +108,56 @@
     EVENTSTREAM_END = "eventstream_end"
 
     def __init__(
         self,
         eventstream: EventstreamType,
         raw_events_only: bool = False,
         event_pair: Optional[list[str | EVENTSTREAM_GLOBAL_EVENTS]] = None,
-        only_adjacent_event_pairs: bool = True,
-        weight_col: str = "user_id",
-        aggregation: Optional[AGGREGATION_NAMES] = None,
+        adjacent_events_only: bool = True,
+        weight_col: str | None = None,
+        time_agg: Optional[AGGREGATION_NAMES] = None,
         timedelta_unit: DATETIME_UNITS = "s",
         log_scale: bool | tuple[bool, bool] | None = None,
         lower_cutoff_quantile: Optional[float] = None,
         upper_cutoff_quantile: Optional[float] = None,
         bins: int | Literal[BINS_ESTIMATORS] = 20,
-        figsize: tuple[float, float] = (6.0, 4.5),
+        width: float = 6.0,
+        height: float = 4.5,
     ) -> None:
         self.__eventstream = eventstream
         self.user_col = self.__eventstream.schema.user_id
         self.event_col = self.__eventstream.schema.event_name
         self.time_col = self.__eventstream.schema.event_timestamp
         self.type_col = self.__eventstream.schema.event_type
         self.raw_events_only = raw_events_only
 
-        self.data: pd.DataFrame = eventstream.to_dataframe(copy=True)
-        if raw_events_only:
-            self.data = self.data[self.data[self.type_col].isin(["raw"])]
         if event_pair is not None:
             if type(event_pair) not in (list, tuple):
                 raise TypeError("event_pair should be a tuple or a list of length 2.")
             if len(event_pair) != 2:
                 raise ValueError("event_pair should be a tuple or a list of length 2.")
 
-            if set(event_pair) == {TimedeltaHist.EVENTSTREAM_START, TimedeltaHist.EVENTSTREAM_END}:
+            if set(event_pair) == {self.EVENTSTREAM_START, self.EVENTSTREAM_END}:
                 raise ValueError(
-                    f"event_pair = ['{TimedeltaHist.EVENTSTREAM_START}', '{TimedeltaHist.EVENTSTREAM_END}'] "
+                    f"event_pair = ['{self.EVENTSTREAM_START}', '{self.EVENTSTREAM_END}'] "
                     f"is invalid. Only one event of these two events can be a member of the event_pair."
                 )
-            if set(event_pair) in [{TimedeltaHist.EVENTSTREAM_START}, {TimedeltaHist.EVENTSTREAM_END}]:
+            if set(event_pair) in [{self.EVENTSTREAM_START}, {self.EVENTSTREAM_END}]:
                 raise ValueError(
-                    f"event_pair = ['{TimedeltaHist.EVENTSTREAM_START}', '{TimedeltaHist.EVENTSTREAM_END}'] and "
-                    f"event_pair = ['{TimedeltaHist.EVENTSTREAM_START}', '{TimedeltaHist.EVENTSTREAM_END}'] "
-                    f"are invalid. Events '{TimedeltaHist.EVENTSTREAM_START}' "
-                    f"and '{TimedeltaHist.EVENTSTREAM_END}' couldn't be doubled."
+                    f"event_pair = ['{self.EVENTSTREAM_START}', '{self.EVENTSTREAM_END}'] and "
+                    f"event_pair = ['{self.EVENTSTREAM_START}', '{self.EVENTSTREAM_END}'] "
+                    f"are invalid. Events '{self.EVENTSTREAM_START}' "
+                    f"and '{self.EVENTSTREAM_END}' couldn't be doubled."
                 )
 
         self.event_pair = event_pair
-        self.only_adjacent_event_pairs = only_adjacent_event_pairs
-        self.weight_col = weight_col
+        self.adjacent_events_only = adjacent_events_only
+        self.weight_col = weight_col or self.__eventstream.schema.user_id
 
-        self.aggregation = aggregation
+        self.time_agg = time_agg
         self.timedelta_unit = timedelta_unit
         if lower_cutoff_quantile is not None:
             if not 0 < lower_cutoff_quantile < 1:
                 raise ValueError("lower_cutoff_quantile should be a fraction between 0 and 1.")
         self.lower_cutoff_quantile = lower_cutoff_quantile
         if upper_cutoff_quantile is not None:
             if not 0 < upper_cutoff_quantile < 1:
@@ -169,34 +171,34 @@
             if isinstance(log_scale, bool):
                 self.log_scale = (log_scale, False)
             else:
                 self.log_scale = log_scale
         else:
             self.log_scale = (False, False)
         self.bins = bins
-        self.figsize = figsize
+        self.figsize = (width, height)
         self.bins_to_show: np.ndarray = np.array([])
         self.values_to_plot: np.ndarray = np.array([])
 
     def _prepare_time_diff(self, data: pd.DataFrame) -> pd.DataFrame:
-        if not self.only_adjacent_event_pairs:
+        if not self.adjacent_events_only:
             data = data[data[self.event_col].isin(self.event_pair)]  # type: ignore
 
         weight_col_group = data.groupby([self.weight_col])
         with pd.option_context("mode.chained_assignment", None):
             data["time_passed"] = weight_col_group[self.time_col].diff() / np.timedelta64(1, self.timedelta_unit)  # type: ignore
             if self.event_pair:
                 data["prev_event"] = weight_col_group[self.event_col].shift()
                 data = data[(data[self.event_col] == self.event_pair[1]) & (data["prev_event"] == self.event_pair[0])]
 
         return data.dropna(subset="time_passed")  # type: ignore
 
     def _aggregate_data(self, data: pd.DataFrame) -> pd.DataFrame:
-        if self.aggregation is not None:
-            data = data.groupby(self.weight_col)["time_passed"].agg(self.aggregation).reset_index()
+        if self.time_agg is not None:
+            data = data.groupby(self.weight_col)["time_passed"].agg(self.time_agg).reset_index()
         return data
 
     def _remove_cutoff_values(self, series: pd.Series) -> pd.Series:
         idx = [True] * len(series)
         if self.upper_cutoff_quantile is not None:
             idx &= series <= series.quantile(self.upper_cutoff_quantile)
         if self.lower_cutoff_quantile is not None:
@@ -223,15 +225,20 @@
         """
         Calculate values and bins for the histplot.
 
         Returns
         -------
         None
         """
-        data = self.data.sort_values([self.weight_col, self.time_col])
+
+        data = self.__eventstream.to_dataframe(copy=True)
+
+        if self.raw_events_only:
+            data = data[data[self.type_col].isin(["raw"])]
+        data = data.sort_values([self.weight_col, self.time_col])
 
         if self.event_pair is not None and set([self.EVENTSTREAM_START, self.EVENTSTREAM_END]).intersection(
             self.event_pair
         ):
             data = self._prepare_global_events_diff(data)
 
         data = self._prepare_time_diff(data)
@@ -275,11 +282,11 @@
         """
 
         plt.subplots(figsize=self.figsize)
 
         hist = sns.histplot(self.values_to_plot, bins=self.bins, log_scale=self.log_scale)
         hist.set_title(
             f"Timedelta histogram, event pair - {self.event_pair}, weight column - {self.weight_col}"
-            f"{', group - ' + self.aggregation if self.aggregation is not None else ''}"
+            f"{', group - ' + self.time_agg if self.time_agg is not None else ''}"
         )
         hist.set_xlabel(f"Time units: {self.timedelta_unit}")
         return hist
```

### Comparing `retentioneering-3.0.0b1/retentioneering/tooling/transition_graph/transition_graph.py` & `retentioneering-3.0.0b2/retentioneering/tooling/transition_graph/transition_graph.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from typing import Any, Dict, List, MutableMapping, MutableSequence, Union, cast
 
 import networkx as nx
 import pandas as pd
 from IPython.core.display import HTML, display
 
 from retentioneering.backend import ServerManager
+from retentioneering.backend.tracker import track
 from retentioneering.edgelist import Edgelist
 from retentioneering.eventstream.types import EventstreamType
 from retentioneering.nodelist import Nodelist
 from retentioneering.templates.transition_graph import TransitionGraphRenderer
 from retentioneering.tooling.typing.transition_graph import (
     GraphSettings,
     LayoutNode,
@@ -37,57 +38,22 @@
     A class that holds methods for transition graph visualization.
 
     Parameters
     ----------
     eventstream: EventstreamType
         Source eventstream.
 
-    edges_norm_type: {"full", "node", None}, default None
-        Type of normalization that is used to calculate weights for graph nodes and edges. See
-        :ref:`Transition graph user guide <transition_graph_weights>` for the details.
-
-    weights: dict, optional
-        Weighting columns for nodes and edges. See :ref:`Transition graph user guide <transition_graph_weights>`
-        for the details.
-
-        - Possible keys: "nodes", "edges".
-        - Possible values: "event_id", user column (typically "user_id") or custom columns.
-
-        If ``None``, {'nodes': 'event_id', 'edges': 'event_id'} dict is used.
-
-    thresholds: dict, optional
-        Threshold values for hiding nodes and edges from the canvas.
-
-        - Possible keys: "nodes", "edges".
-        - Possible values: dict with weighting columns as dict keys and threshold values as dict values.
-
-        Example: {'nodes': {'event_id': 0.03}, 'edges': {'event_id': 0.03, user_id: 0.05}}
-
-        If ``None``, all the threshold values are set to 0.
-
-    targets: dict, optional
-        Events mapping that defines which nodes and edges should be colored for better visualization.
-
-        - Possible keys: "positive" (green), "negative" (red), "source" (orange).
-        - Possible values: list of events of a given type.
-
-    graph_settings: dict, optional
-        Visual boolean settings related to :ref:`Settings block <transition_graph_visual_settings>`
-        in the control of transition graph interface.
-
-        Possible keys:
-        - show_weights,
-        - show_percents,
-        - show_nodes_names,
-        - show_all_edges_for_targets,
-        - show_nodes_without_links.
 
     See Also
     --------
     .Eventstream.transition_graph : Call TransitionGraph tool as an eventstream method.
+    .Eventstream.transition_matrix : Matrix representation of transition graph.
+    .EventstreamSchema : Schema of eventstream columns, that could be used as weights.
+    .TransitionGraph.plot : Interactive transition graph visualization.
+
 
     Notes
     -----
     See :doc:`transition graph user guide</user_guides/transition_graph>` for the details.
 
     """
 
@@ -124,82 +90,42 @@
             if not all(map(lambda x: x is None or 0 <= x <= 1, value.values())):
                 raise ValueError(
                     f"For normalization type {self.edges_norm_type} all thresholds must be between 0 and 1 or None"
                 )
 
         return True
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "transition_graph", "event_custom_name": "transition_graph_init"},
+    )
     def __init__(
         self,
         eventstream: EventstreamType,  # graph: dict,  # preprocessed graph
-        graph_settings: GraphSettings | dict[str, Any] | None = None,
-        edges_norm_type: NormType = None,
-        targets: MutableMapping[str, str | None] | None = None,
-        nodes_threshold: Threshold | None = None,
-        edges_threshold: Threshold | None = None,
-        nodes_weight_col: str | None = None,
-        edges_weight_col: str | None = None,
-        custom_weight_cols: list[str] | None = None,
     ) -> None:
         from retentioneering.eventstream.eventstream import Eventstream
 
-        if graph_settings is None:
-            graph_settings = {}  # type: ignore
-        if nodes_threshold is None:
-            nodes_threshold = {"user_id": 0.0, "event_id": 0.0}
-        self.nodes_thresholds = nodes_threshold
-
-        if edges_threshold is None:
-            edges_threshold = {"user_id": 0.0, "event_id": 0.0}
-        self.edges_thresholds = edges_threshold
-
-        self.nodelist_default_col = eventstream.schema.event_id
-        self.edgelist_default_col = eventstream.schema.event_id
-
-        self.targets = targets if targets else {"positive": None, "negative": None, "source": None}
         sm = ServerManager()
         self.env = sm.check_env()
         self.server = sm.create_server()
 
         self.server.register_action("save-nodelist", lambda n: self._on_nodelist_updated(n))
         self.server.register_action("save-layout", lambda n: self._on_layout_request(n))
         self.server.register_action("save-graph-settings", lambda n: self._on_graph_settings_request(n))
         self.server.register_action("recalculate", lambda n: self._on_recalc_request(n))
 
         self.eventstream: Eventstream = eventstream  # type: ignore
 
         self.event_col = self.eventstream.schema.event_name
         self.event_time_col = self.eventstream.schema.event_timestamp
         self.user_col = self.eventstream.schema.user_id
-        self.id_col = self.eventstream.schema.event_id
-        self.weight_cols = self._define_weight_cols(custom_weight_cols)
-
-        self.nodes_weight_col = nodes_weight_col if nodes_weight_col else eventstream.schema.event_id
-        self.edges_weight_col = edges_weight_col if edges_weight_col else eventstream.schema.event_id
 
         self.spring_layout_config = {"k": 0.1, "iterations": 300, "nx_threshold": 1e-4}
 
         self.layout: pd.DataFrame | None = None
-        self.graph_settings = graph_settings
-
-        self.edges_norm_type: NormType | None = edges_norm_type
-
-        self.nodelist: Nodelist = Nodelist(
-            weight_cols=self.weight_cols,
-            time_col=self.event_time_col,
-            event_col=self.event_col,
-        )
-
-        self.nodelist.calculate_nodelist(data=self.eventstream.to_dataframe())
-        self.edgelist: Edgelist = Edgelist(eventstream=self.eventstream)
-        self.edgelist.calculate_edgelist(
-            weight_cols=self.weight_cols,
-            norm_type=self.edges_norm_type,
-        )
-
+        self.graph_settings: GraphSettings | dict[str, Any] = {}
         self.render: TransitionGraphRenderer = TransitionGraphRenderer()
 
     def _define_weight_cols(self, custom_weight_cols: list[str] | None) -> list[str]:
         weight_cols = [
             self.eventstream.schema.event_id,
             self.eventstream.schema.user_id,
         ]
@@ -614,105 +540,187 @@
     @staticmethod
     def generateId(size: int = 6, chars: str = string.ascii_uppercase + string.digits) -> str:
         return "el" + "".join(random.choice(chars) for _ in range(size))
 
     def _edges_norm_type_to_json_value(self, edges_norm_type: NormType) -> str:
         return "none" if edges_norm_type is None else str(edges_norm_type).lower()
 
-    def plot_graph(
+    @track(  # type: ignore
+        tracking_info={"event_name": "transition_graph", "event_custom_name": "transition_graph_plot_graph"},
+        allowed_params=[
+            "edges_norm_type",
+            "targets",
+            "nodes_threshold",
+            "edges_threshold",
+            "nodes_weight_col",
+            "edges_weight_col",
+            "custom_weight_cols",
+        ],
+    )
+    def plot(
         self,
         targets: MutableMapping[str, str | None] | None = None,
         edges_norm_type: NormType | None = None,
+        nodes_threshold: Threshold | None = None,
+        edges_threshold: Threshold | None = None,
+        nodes_weight_col: str | None = None,
+        edges_weight_col: str | None = None,
+        custom_weight_cols: list[str] | None = None,
         width: int = 960,
         height: int = 900,
-        weight_template: str | None = None,
-        show_weights: bool | None = None,
-        show_percents: bool | None = None,
-        show_nodes_names: bool | None = None,
-        show_all_edges_for_targets: bool | None = None,
-        show_nodes_without_links: bool | None = None,
+        show_weights: bool = True,
+        show_percents: bool = False,
+        show_nodes_names: bool = True,
+        show_all_edges_for_targets: bool = True,
+        show_nodes_without_links: bool = False,
     ) -> None:
         """
         Create interactive transition graph visualization with callback to sourcing eventstream.
 
         Parameters
         ----------
         edges_norm_type: {"full", "node", None}, default None
-            Type of normalization that is used to calculate weights for graph nodes and edges. See
-            :ref:`Transition graph user guide <transition_graph_weights>` for the details.
+            Type of normalization that is used to calculate weights for graph edges.
+            Based on ``edges_weight_col`` parameter the weight values are calculated.
+
+            - If ``None``, normalization is not used, the absolute values are taken.
+            - If ``full``, normalization across the whole eventstream.
+            - If ``node``, normalization across each node (or outgoing transitions from each node).
+
+            See :ref:`Transition graph user guide <transition_graph_weights>` for the details.
+
+        edges_weight_col: str, optional
+            A column name from the :py:class:`.EventstreamSchema` which values will control the final
+            edges' weights and displayed width as well.
+
+            For each edge is calculated:
 
-        weights: dict, optional
-            Weighting columns for nodes and edges. See :ref:`Transition graph user guide <transition_graph_weights>`
-            for the details.
+            - If ``None`` or ``event_id`` - the number of transitions.
+            - If ``user_id`` - the number of unique users.
+            - If ``session_id`` - the number of unique sessions.
+            - If ``custom_col`` - the number of unique values in selected column.
 
-            - Possible keys: "nodes", "edges".
-            - Possible values: "event_id", user column (typically "user_id") or custom columns.
+            See :ref:`Transition graph user guide <transition_graph_weights>` for the details.
 
-            If ``None``, {'nodes': 'event_id', 'edges': 'event_id'} dict is used.
+        edges_threshold: dict, optional
+            Threshold mapping that defines the minimal weights for edges displayed on the canvas.
 
-        thresholds: dict, optional
-            Threshold values for hiding nodes and edges from the canvas.
+            - Keys should be of type str and contain the weight column names (the values from the
+              :py:class:`.EventstreamSchema`).
+            - Values of the dict are the thresholds for the edges that will be displayed.
 
-            - Possible keys: "nodes", "edges".
-            - Possible values: dict with weighting columns as dict keys and threshold values as dict values.
+            Support multiple weighting columns. In that case, logical OR will be applied.
+            Edges with value less than at least one of thresholds will be hidden.
+            Example: {'event_id': 100, user_id: 50}.
 
-            Example: {'nodes': {'event_id': 0.03}, 'edges': {'event_id': 0.03, user_id: 0.05}}
+            See :ref:`Transition graph user guide<transition_graph_thresholds>` for the details.
 
-            If ``None``, all the threshold values are set to 0.
+        nodes_weight_col: str, optional
+            A column name from the :py:class:`.EventstreamSchema` which values control the final
+            nodes' weights and displayed diameter as well.
+
+            For each node is calculated:
+
+            - If ``None`` or ``event_id`` - the number of events.
+            - If ``user_id`` - the number of unique users.
+            - If ``session_id`` - the number of unique sessions.
+            - If ``custom_col`` - the number of unique values in selected column.
+
+            See :ref:`Transition graph user guide <transition_graph_weights>` for the details.
+
+        nodes_threshold: dict, optional
+            Threshold mapping that defines the minimal weights for nodes displayed on the canvas.
+
+            - Keys should be of type str and contain the weight column names (the values from the
+              :py:class:`.EventstreamSchema`).
+            - Values of the dict are the thresholds for the nodes that will be displayed.
+              They should be of type int or float.
+
+            Support multiple weighting columns. In that case, logical OR will be applied.
+            Nodes with value less than at least one of thresholds will be hidden.
+            Example: {'event_id': 100, user_id: 50}.
+
+            See :ref:`Transition graph user guide<transition_graph_thresholds>` for the details.
 
         targets: dict, optional
             Events mapping that defines which nodes and edges should be colored for better visualization.
 
             - Possible keys: "positive" (green), "negative" (red), "source" (orange).
             - Possible values: list of events of a given type.
 
-        width : int, default 960
+            See :ref:`Transition graph user guide<transition_graph_targets>` for the details.
+
+        custom_weight_cols: list of str, optional
+            Custom columns from the :py:class:`.EventstreamSchema` that can be selected in ``edges_weight_col``
+            and ``nodes_weight_col`` parameters. If ``session_col=session_id`` exists,
+            it is added by default to this list.
+        width: int, default 960
             Width of plot in pixels.
-        height : int, default 960
+        height: int, default 960
             Height of plot in pixels.
-        weight_template : str, optional
-        show_weights : bool, optional
-        show_percents : bool, optional
-        show_nodes_names : bool, optional
-        show_all_edges_for_targets : bool, optional
-        show_nodes_without_links : bool, optional
+        show_weights: bool, default True
+            Hide/display the edge weight labels. By default, weights are shown.
+        show_percents: bool, default False
+            Display edge weights as percents. Available only if an edge normalization type is chosen.
+            By default, weights are displayed in fractions.
+        show_nodes_names: bool, default True
+            Hide/display the node names. By default, names are shown.
+        show_all_edges_for_targets: bool, default True
+            This displaying option allows to ignore the threshold filters and always display
+            any edge connected to a target node. By default, all such edges are shown.
+        show_nodes_without_links: bool, default False
+            Setting a threshold filter might remove all the edges connected to a node.
+            Such isolated nodes might be considered as useless. This displaying option
+            hides them in the canvas as well.
+        @TODO: add show_edge_info_on_hover Ticket: https://retentioneering.atlassian.net/browse/PLAT-776. dpanina.
 
         Returns
         -------
             Rendered IFrame graph.
 
         Notes
         -----
-        To get the definition of ``show_*`` visual parameters see
-        :ref:`Settings block <transition_graph_visual_settings>` in the control of transition graph interface.
+        1. If all the edges connected to a node are hidden, the node becomes hidden as well.
+           In order to avoid it - use ``show_nodes_without_links=True`` parameter in code or in the interface.
+        2. The thresholds may use their own weighting columns both for nodes and for edges independently
+           of weighting columns defined in ``edges_weight_col`` and ``nodes_weight_col`` arguments.
 
+        See :doc:`TransitionGraph user guide </user_guides/transition_graph>` for the details.
         """
-        if targets:
-            self.targets = targets
-        self.edges_norm_type = edges_norm_type
+        if not edges_norm_type and show_percents:
+            raise ValueError("If show_percents=True, edges_norm_type should be 'full' or 'node'!")
 
-        settings = self._apply_settings(
-            show_weights=show_weights,
-            show_percents=show_percents,
-            show_nodes_names=show_nodes_names,
-            show_all_edges_for_targets=show_all_edges_for_targets,
-            show_nodes_without_links=show_nodes_without_links,
+        self.__prepare_graph_for_plot(
+            edges_weight_col=edges_weight_col,
+            edges_threshold=edges_threshold,
+            edges_norm_type=edges_norm_type,
+            nodes_weight_col=nodes_weight_col,
+            nodes_threshold=nodes_threshold,
+            targets=targets,
+            custom_weight_cols=custom_weight_cols,
         )
 
         norm_nodes_threshold = (
             self.nodes_thresholds if self.nodes_thresholds else self._get_norm_node_threshold(self.nodes_thresholds)
         )
         norm_links_threshold = (
             self.edges_thresholds if self.edges_thresholds else self._get_norm_link_threshold(self.edges_thresholds)
         )
 
-        self.edgelist.calculate_edgelist(weight_cols=self.weight_cols, norm_type=self.edges_norm_type)
         node_params = self._make_node_params(targets)
         cols = self.__get_nodelist_cols()
 
+        settings = self._apply_settings(
+            show_weights=show_weights,
+            show_percents=show_percents,
+            show_nodes_names=show_nodes_names,
+            show_all_edges_for_targets=show_all_edges_for_targets,
+            show_nodes_without_links=show_nodes_without_links,
+        )
+
         nodes, links = self._make_template_data(
             node_params=node_params,
             width=width,
             height=height,
         )
 
         shown_nodes_col = self.nodes_weight_col
@@ -738,15 +746,15 @@
                 show_weights=self._get_option("show_weights", settings),
                 show_percents=self._get_option("show_percents", settings),
                 show_nodes_names=self._get_option("show_nodes_names", settings),
                 show_all_edges_for_targets=self._get_option("show_all_edges_for_targets", settings),
                 show_nodes_without_links=self._get_option("show_nodes_without_links", settings),
                 nodes_threshold=self._to_js_val(norm_nodes_threshold),
                 links_threshold=self._to_js_val(norm_links_threshold),
-                weight_template=weight_template if weight_template is not None else "undefined",
+                weight_template="undefined",
             )
         )
 
         graph_body = self.render.body()
 
         graph_script_src = (
             "https://static.server.retentioneering.com/viztools/transition-graph/v3/transition-graph.umd.js?id="
@@ -804,11 +812,51 @@
                 graph_script_src=graph_script_src,
                 init_graph_js=init_graph_js,
                 template=html_template,
             )
         )
         display(HTML(html))
 
+    def __prepare_graph_for_plot(
+        self,
+        edges_weight_col: str | None = None,
+        edges_threshold: Threshold | None = None,
+        nodes_weight_col: str | None = None,
+        nodes_threshold: Threshold | None = None,
+        edges_norm_type: NormType | None = None,
+        targets: MutableMapping[str, str | None] | None = None,
+        custom_weight_cols: list[str] | None = None,
+    ) -> None:
+        if targets:
+            self.targets = targets
+        self.edges_norm_type = edges_norm_type
+        if nodes_threshold is None:
+            nodes_threshold = {"user_id": 0.0, "event_id": 0.0}
+        self.nodes_thresholds = nodes_threshold
+        if edges_threshold is None:
+            edges_threshold = {"user_id": 0.0, "event_id": 0.0}
+        self.edges_thresholds = edges_threshold
+        self.nodelist_default_col = self.eventstream.schema.event_id
+        self.edgelist_default_col = self.eventstream.schema.event_id
+        self.targets = targets if targets else {"positive": None, "negative": None, "source": None}
+        self.weight_cols = self._define_weight_cols(custom_weight_cols)
+        self.nodes_weight_col = nodes_weight_col if nodes_weight_col else self.eventstream.schema.event_id
+        self.edges_weight_col = edges_weight_col if edges_weight_col else self.eventstream.schema.event_id
+
+        self.edges_weight_col = self.eventstream.schema.event_id
+        self.edges_norm_type: NormType | None = edges_norm_type
+        self.nodelist: Nodelist = Nodelist(
+            weight_cols=self.weight_cols,
+            time_col=self.event_time_col,
+            event_col=self.event_col,
+        )
+        self.nodelist.calculate_nodelist(data=self.eventstream.to_dataframe())
+        self.edgelist: Edgelist = Edgelist(eventstream=self.eventstream)
+        self.edgelist.calculate_edgelist(
+            weight_cols=self.weight_cols,
+            norm_type=self.edges_norm_type,
+        )
+
     def _get_option(self, name: str, settings: dict[str, Any]) -> str:
         if name in settings:
             return self._to_json(settings[name])
         return "undefined"
```

### Comparing `retentioneering-3.0.0b1/retentioneering/tooling/typing/transition_graph/graph_types.py` & `retentioneering-3.0.0b2/retentioneering/tooling/typing/transition_graph/graph_types.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b1/retentioneering/tooling/user_lifetime_hist/user_lifetime_hist.py` & `retentioneering-3.0.0b2/retentioneering/tooling/user_lifetime_hist/user_lifetime_hist.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,26 +32,28 @@
     lower_cutoff_quantile : float, optional
         Specify time distance quantile as the lower boundary. The values below the boundary are truncated.
     upper_cutoff_quantile : float, optional
         Specify time distance quantile as the upper boundary. The values above the boundary are truncated.
     bins : int or str, default 20
         Generic bin parameter that can be the name of a reference rule or
         the number of bins. Passed to :numpy_bins_link:`numpy.histogram_bin_edges<>`.
-    figsize : tuple of float, default (12.0, 7.0)
-        Width, height in inches.
+    width : float, default 6.0
+        Width in inches.
+    height : float, default 4.5
+        Height in inches.
 
 
 
     See Also
     --------
     .EventTimestampHist : Plot the distribution of events over time.
     .TimedeltaHist : Plot the distribution of the time deltas between two events.
     .Eventstream.describe : Show general eventstream statistics.
     .Eventstream.describe_events : Show general eventstream events statistics.
-    .DeleteUsersByPathLength : Filter user paths based on the path length, removing the paths that are shorter than the
+    .DropPaths : Filter user paths based on the path length, removing the paths that are shorter than the
                                specified number of events or cut_off.
 
     Notes
     -----
     See :ref:`Eventstream user guide<eventstream_user_lifetime>` for the details.
 
     """
@@ -60,15 +62,16 @@
         self,
         eventstream: EventstreamType,
         timedelta_unit: DATETIME_UNITS = "s",
         log_scale: bool | tuple[bool, bool] | None = None,
         lower_cutoff_quantile: Optional[float] = None,
         upper_cutoff_quantile: Optional[float] = None,
         bins: int | Literal[BINS_ESTIMATORS] = 20,
-        figsize: tuple[float, float] = (12.0, 7.0),
+        width: float = 6.0,
+        height: float = 4.5,
     ) -> None:
         self.__eventstream = eventstream
         self.user_col = self.__eventstream.schema.user_id
         self.event_col = self.__eventstream.schema.event_name
         self.time_col = self.__eventstream.schema.event_timestamp
         self.timedelta_unit = timedelta_unit
         if lower_cutoff_quantile is not None:
@@ -88,15 +91,15 @@
                 self.log_scale = (log_scale, False)
             else:
                 self.log_scale = log_scale
         else:
             self.log_scale = (False, False)
 
         self.bins = bins
-        self.figsize = figsize
+        self.figsize = (width, height)
         self.bins_to_show: np.ndarray = np.array([])
         self.values_to_plot: np.ndarray = np.array([])
 
     def _remove_cutoff_values(self, series: pd.Series) -> pd.Series:
         idx = [True] * len(series)
         if self.upper_cutoff_quantile is not None:
             idx &= series <= series.quantile(self.upper_cutoff_quantile)
```

### Comparing `retentioneering-3.0.0b1/retentioneering/utils/registry.py` & `retentioneering-3.0.0b2/retentioneering/utils/registry.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0b1/retentioneering/widget/widgets.py` & `retentioneering-3.0.0b2/retentioneering/widget/widgets.py`

 * *Files identical despite different names*


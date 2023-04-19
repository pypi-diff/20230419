# Comparing `tmp/dg-commons-0.0.6.tar.gz` & `tmp/dg-commons-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dg-commons-0.0.6.tar", last modified: Wed Oct 20 13:17:02 2021, max compression
+gzip compressed data, was "dg-commons-0.0.8.tar", last modified: Tue Nov 23 17:11:33 2021, max compression
```

## Comparing `dg-commons-0.0.6.tar` & `dg-commons-0.0.8.tar`

### file list

```diff
@@ -1,77 +1,81 @@
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2021-10-20 13:17:02.128692 dg-commons-0.0.6/
--rw-rw-r--   0 ale       (1000) ale       (1000)    35149 2021-10-13 07:29:33.000000 dg-commons-0.0.6/LICENSE
--rw-rw-r--   0 ale       (1000) ale       (1000)       47 2021-10-13 13:29:06.000000 dg-commons-0.0.6/MANIFEST.in
--rw-rw-r--   0 ale       (1000) ale       (1000)      972 2021-10-20 13:17:02.128692 dg-commons-0.0.6/PKG-INFO
--rw-rw-r--   0 ale       (1000) ale       (1000)      500 2021-10-13 13:57:46.000000 dg-commons-0.0.6/README.md
--rw-rw-r--   0 ale       (1000) ale       (1000)       38 2021-10-20 13:17:02.128692 dg-commons-0.0.6/setup.cfg
--rw-rw-r--   0 ale       (1000) ale       (1000)     1475 2021-10-20 13:10:00.000000 dg-commons-0.0.6/setup.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2021-10-20 13:17:02.120692 dg-commons-0.0.6/src/
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2021-10-20 13:17:02.120692 dg-commons-0.0.6/src/dg_commons/
--rw-rw-r--   0 ale       (1000) ale       (1000)      264 2021-10-20 13:15:48.000000 dg-commons-0.0.6/src/dg_commons/__init__.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2021-10-20 13:17:02.124692 dg-commons-0.0.6/src/dg_commons/controllers/
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2021-10-13 13:29:06.000000 dg-commons-0.0.6/src/dg_commons/controllers/__init__.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     2158 2021-10-20 13:10:00.000000 dg-commons-0.0.6/src/dg_commons/controllers/pid.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     3885 2021-10-18 10:09:09.000000 dg-commons-0.0.6/src/dg_commons/controllers/pure_pursuit.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     6530 2021-10-20 13:10:00.000000 dg-commons-0.0.6/src/dg_commons/controllers/speed.py
--rw-rw-r--   0 ale       (1000) ale       (1000)      803 2021-10-20 13:10:00.000000 dg-commons-0.0.6/src/dg_commons/controllers/steer.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2021-10-20 13:17:02.124692 dg-commons-0.0.6/src/dg_commons/dynamics/
--rw-rw-r--   0 ale       (1000) ale       (1000)       31 2021-10-13 13:29:06.000000 dg-commons-0.0.6/src/dg_commons/dynamics/__init__.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     3677 2021-10-20 13:10:00.000000 dg-commons-0.0.6/src/dg_commons/dynamics/bicycle_dynamic.py
--rw-rw-r--   0 ale       (1000) ale       (1000)      471 2021-10-13 13:29:06.000000 dg-commons-0.0.6/src/dg_commons/game_types.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     2128 2021-10-13 13:29:06.000000 dg-commons-0.0.6/src/dg_commons/geo.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2021-10-20 13:17:02.124692 dg-commons-0.0.6/src/dg_commons/maps/
--rw-rw-r--   0 ale       (1000) ale       (1000)       21 2021-10-13 13:29:06.000000 dg-commons-0.0.6/src/dg_commons/maps/__init__.py
--rw-rw-r--   0 ale       (1000) ale       (1000)    10123 2021-10-20 13:10:00.000000 dg-commons-0.0.6/src/dg_commons/maps/lanes.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2021-10-20 13:17:02.124692 dg-commons-0.0.6/src/dg_commons/planning/
--rw-rw-r--   0 ale       (1000) ale       (1000)      112 2021-10-13 13:29:06.000000 dg-commons-0.0.6/src/dg_commons/planning/__init__.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     3225 2021-10-20 13:10:00.000000 dg-commons-0.0.6/src/dg_commons/planning/commands_sampler.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     1306 2021-10-20 13:10:00.000000 dg-commons-0.0.6/src/dg_commons/planning/goals.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     4665 2021-10-20 13:10:00.000000 dg-commons-0.0.6/src/dg_commons/planning/motion_primitives.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     2884 2021-10-13 13:29:06.000000 dg-commons-0.0.6/src/dg_commons/planning/trajectory.py
--rw-rw-r--   0 ale       (1000) ale       (1000)      813 2021-10-20 13:10:00.000000 dg-commons-0.0.6/src/dg_commons/planning/trajectory_generator_abc.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2021-10-20 13:17:02.124692 dg-commons-0.0.6/src/dg_commons/seq/
--rw-rw-r--   0 ale       (1000) ale       (1000)       46 2021-10-13 13:29:06.000000 dg-commons-0.0.6/src/dg_commons/seq/__init__.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     1512 2021-10-13 13:29:06.000000 dg-commons-0.0.6/src/dg_commons/seq/seq_op.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     6933 2021-10-13 13:29:06.000000 dg-commons-0.0.6/src/dg_commons/seq/sequence.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2021-10-20 13:17:02.124692 dg-commons-0.0.6/src/dg_commons/sim/
--rw-rw-r--   0 ale       (1000) ale       (1000)      220 2021-10-13 13:29:06.000000 dg-commons-0.0.6/src/dg_commons/sim/__init__.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2021-10-20 13:17:02.128692 dg-commons-0.0.6/src/dg_commons/sim/agents/
--rw-rw-r--   0 ale       (1000) ale       (1000)       21 2021-10-13 13:29:06.000000 dg-commons-0.0.6/src/dg_commons/sim/agents/__init__.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     2174 2021-10-13 13:29:06.000000 dg-commons-0.0.6/src/dg_commons/sim/agents/agent.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     4508 2021-10-13 13:29:06.000000 dg-commons-0.0.6/src/dg_commons/sim/agents/lane_follower.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     5106 2021-10-20 13:10:00.000000 dg-commons-0.0.6/src/dg_commons/sim/collision.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     2751 2021-10-20 13:10:00.000000 dg-commons-0.0.6/src/dg_commons/sim/collision_structures.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     6862 2021-10-20 13:10:00.000000 dg-commons-0.0.6/src/dg_commons/sim/collision_utils.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     4842 2021-10-20 13:10:00.000000 dg-commons-0.0.6/src/dg_commons/sim/collision_visualisation.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2021-10-20 13:17:02.128692 dg-commons-0.0.6/src/dg_commons/sim/models/
--rw-rw-r--   0 ale       (1000) ale       (1000)       74 2021-10-20 13:10:00.000000 dg-commons-0.0.6/src/dg_commons/sim/models/__init__.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     1541 2021-10-13 13:29:06.000000 dg-commons-0.0.6/src/dg_commons/sim/models/model_structures.py
--rw-rw-r--   0 ale       (1000) ale       (1000)      969 2021-10-20 13:10:00.000000 dg-commons-0.0.6/src/dg_commons/sim/models/model_utils.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     9682 2021-10-20 13:10:00.000000 dg-commons-0.0.6/src/dg_commons/sim/models/pedestrian.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     1110 2021-10-13 13:29:06.000000 dg-commons-0.0.6/src/dg_commons/sim/models/pedestrian_utils.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     1432 2021-10-13 13:29:06.000000 dg-commons-0.0.6/src/dg_commons/sim/models/tires.py
--rw-rw-r--   0 ale       (1000) ale       (1000)      904 2021-10-13 13:29:06.000000 dg-commons-0.0.6/src/dg_commons/sim/models/utils.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     9868 2021-10-13 13:29:06.000000 dg-commons-0.0.6/src/dg_commons/sim/models/vehicle.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     9087 2021-10-13 13:29:06.000000 dg-commons-0.0.6/src/dg_commons/sim/models/vehicle_dynamic.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     2616 2021-10-13 13:29:06.000000 dg-commons-0.0.6/src/dg_commons/sim/models/vehicle_ligths.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     7060 2021-10-20 13:10:00.000000 dg-commons-0.0.6/src/dg_commons/sim/models/vehicle_structures.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     2265 2021-10-20 13:10:00.000000 dg-commons-0.0.6/src/dg_commons/sim/models/vehicle_utils.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2021-10-20 13:17:02.128692 dg-commons-0.0.6/src/dg_commons/sim/scenarios/
--rw-rw-r--   0 ale       (1000) ale       (1000)       21 2021-10-13 13:29:06.000000 dg-commons-0.0.6/src/dg_commons/sim/scenarios/__init__.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     5234 2021-10-13 13:29:06.000000 dg-commons-0.0.6/src/dg_commons/sim/scenarios/agent_from_commonroad.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     1930 2021-10-20 13:10:00.000000 dg-commons-0.0.6/src/dg_commons/sim/scenarios/factory.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     1607 2021-10-20 13:10:00.000000 dg-commons-0.0.6/src/dg_commons/sim/scenarios/utils.py
--rw-rw-r--   0 ale       (1000) ale       (1000)      576 2021-10-13 13:29:06.000000 dg-commons-0.0.6/src/dg_commons/sim/sim_types.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     6997 2021-10-20 13:10:00.000000 dg-commons-0.0.6/src/dg_commons/sim/simulator.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     7888 2021-10-13 13:29:06.000000 dg-commons-0.0.6/src/dg_commons/sim/simulator_animation.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     5247 2021-10-13 13:29:06.000000 dg-commons-0.0.6/src/dg_commons/sim/simulator_structures.py
--rw-rw-r--   0 ale       (1000) ale       (1000)    10223 2021-10-13 13:29:06.000000 dg-commons-0.0.6/src/dg_commons/sim/simulator_visualisation.py
--rw-rw-r--   0 ale       (1000) ale       (1000)      578 2021-10-20 13:10:00.000000 dg-commons-0.0.6/src/dg_commons/time.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     1764 2021-10-20 13:10:00.000000 dg-commons-0.0.6/src/dg_commons/utils_toolz.py
--rw-rw-r--   0 ale       (1000) ale       (1000)      191 2021-10-17 12:50:11.000000 dg-commons-0.0.6/src/dg_commons/utils_types.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2021-10-20 13:17:02.124692 dg-commons-0.0.6/src/dg_commons.egg-info/
--rw-rw-r--   0 ale       (1000) ale       (1000)      972 2021-10-20 13:17:02.000000 dg-commons-0.0.6/src/dg_commons.egg-info/PKG-INFO
--rw-rw-r--   0 ale       (1000) ale       (1000)     2227 2021-10-20 13:17:02.000000 dg-commons-0.0.6/src/dg_commons.egg-info/SOURCES.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)        1 2021-10-20 13:17:02.000000 dg-commons-0.0.6/src/dg_commons.egg-info/dependency_links.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)      155 2021-10-20 13:17:02.000000 dg-commons-0.0.6/src/dg_commons.egg-info/requires.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)       28 2021-10-20 13:17:02.000000 dg-commons-0.0.6/src/dg_commons.egg-info/top_level.txt
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2021-11-23 17:11:33.609321 dg-commons-0.0.8/
+-rw-rw-r--   0 ale       (1000) ale       (1000)    35149 2021-10-13 07:29:33.000000 dg-commons-0.0.8/LICENSE
+-rw-rw-r--   0 ale       (1000) ale       (1000)       47 2021-10-13 13:29:06.000000 dg-commons-0.0.8/MANIFEST.in
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2044 2021-11-23 17:11:33.609321 dg-commons-0.0.8/PKG-INFO
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1572 2021-11-06 08:38:54.000000 dg-commons-0.0.8/README.md
+-rw-rw-r--   0 ale       (1000) ale       (1000)       38 2021-11-23 17:11:33.609321 dg-commons-0.0.8/setup.cfg
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1666 2021-11-19 18:55:06.000000 dg-commons-0.0.8/setup.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2021-11-23 17:11:33.597321 dg-commons-0.0.8/src/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2021-11-23 17:11:33.601321 dg-commons-0.0.8/src/dg_commons/
+-rw-rw-r--   0 ale       (1000) ale       (1000)      306 2021-11-23 17:11:29.000000 dg-commons-0.0.8/src/dg_commons/__init__.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2021-11-23 17:11:33.601321 dg-commons-0.0.8/src/dg_commons/controllers/
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2021-10-13 13:29:06.000000 dg-commons-0.0.8/src/dg_commons/controllers/__init__.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2158 2021-10-20 13:10:00.000000 dg-commons-0.0.8/src/dg_commons/controllers/pid.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     3885 2021-10-18 10:09:09.000000 dg-commons-0.0.8/src/dg_commons/controllers/pure_pursuit.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     6530 2021-10-20 13:10:00.000000 dg-commons-0.0.8/src/dg_commons/controllers/speed.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      803 2021-10-20 13:10:00.000000 dg-commons-0.0.8/src/dg_commons/controllers/steer.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2021-11-23 17:11:33.601321 dg-commons-0.0.8/src/dg_commons/dynamics/
+-rw-rw-r--   0 ale       (1000) ale       (1000)       31 2021-10-13 13:29:06.000000 dg-commons-0.0.8/src/dg_commons/dynamics/__init__.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     3677 2021-10-20 13:10:00.000000 dg-commons-0.0.8/src/dg_commons/dynamics/bicycle_dynamic.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      471 2021-10-13 13:29:06.000000 dg-commons-0.0.8/src/dg_commons/game_types.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2553 2021-11-22 16:16:59.000000 dg-commons-0.0.8/src/dg_commons/geo.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2021-11-23 17:11:33.601321 dg-commons-0.0.8/src/dg_commons/maps/
+-rw-rw-r--   0 ale       (1000) ale       (1000)       21 2021-10-13 13:29:06.000000 dg-commons-0.0.8/src/dg_commons/maps/__init__.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)    10123 2021-10-20 13:10:00.000000 dg-commons-0.0.8/src/dg_commons/maps/lanes.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1361 2021-11-21 20:02:37.000000 dg-commons-0.0.8/src/dg_commons/maps/road_bounds.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     6192 2021-11-22 16:16:59.000000 dg-commons-0.0.8/src/dg_commons/maps/shapely_viz.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2021-11-23 17:11:33.605321 dg-commons-0.0.8/src/dg_commons/planning/
+-rw-rw-r--   0 ale       (1000) ale       (1000)      112 2021-10-13 13:29:06.000000 dg-commons-0.0.8/src/dg_commons/planning/__init__.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     3225 2021-10-20 13:10:00.000000 dg-commons-0.0.8/src/dg_commons/planning/commands_sampler.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1306 2021-10-20 13:10:00.000000 dg-commons-0.0.8/src/dg_commons/planning/goals.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     4665 2021-10-20 13:10:00.000000 dg-commons-0.0.8/src/dg_commons/planning/motion_primitives.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2884 2021-10-13 13:29:06.000000 dg-commons-0.0.8/src/dg_commons/planning/trajectory.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      813 2021-10-20 13:10:00.000000 dg-commons-0.0.8/src/dg_commons/planning/trajectory_generator_abc.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2021-11-23 17:11:33.605321 dg-commons-0.0.8/src/dg_commons/seq/
+-rw-rw-r--   0 ale       (1000) ale       (1000)       46 2021-10-13 13:29:06.000000 dg-commons-0.0.8/src/dg_commons/seq/__init__.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1512 2021-10-13 13:29:06.000000 dg-commons-0.0.8/src/dg_commons/seq/seq_op.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     6933 2021-10-13 13:29:06.000000 dg-commons-0.0.8/src/dg_commons/seq/sequence.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2021-11-23 17:11:33.605321 dg-commons-0.0.8/src/dg_commons/sim/
+-rw-rw-r--   0 ale       (1000) ale       (1000)      220 2021-10-13 13:29:06.000000 dg-commons-0.0.8/src/dg_commons/sim/__init__.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2021-11-23 17:11:33.605321 dg-commons-0.0.8/src/dg_commons/sim/agents/
+-rw-rw-r--   0 ale       (1000) ale       (1000)       21 2021-10-13 13:29:06.000000 dg-commons-0.0.8/src/dg_commons/sim/agents/__init__.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2174 2021-10-13 13:29:06.000000 dg-commons-0.0.8/src/dg_commons/sim/agents/agent.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     4508 2021-10-13 13:29:06.000000 dg-commons-0.0.8/src/dg_commons/sim/agents/lane_follower.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     7394 2021-11-23 16:47:40.000000 dg-commons-0.0.8/src/dg_commons/sim/collision.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2751 2021-10-20 13:10:00.000000 dg-commons-0.0.8/src/dg_commons/sim/collision_structures.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     6905 2021-11-23 16:01:30.000000 dg-commons-0.0.8/src/dg_commons/sim/collision_utils.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     4842 2021-10-20 13:10:00.000000 dg-commons-0.0.8/src/dg_commons/sim/collision_visualisation.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2021-11-23 17:11:33.609321 dg-commons-0.0.8/src/dg_commons/sim/models/
+-rw-rw-r--   0 ale       (1000) ale       (1000)       74 2021-10-20 13:10:00.000000 dg-commons-0.0.8/src/dg_commons/sim/models/__init__.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1949 2021-11-23 16:47:40.000000 dg-commons-0.0.8/src/dg_commons/sim/models/model_structures.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      969 2021-10-20 13:10:00.000000 dg-commons-0.0.8/src/dg_commons/sim/models/model_utils.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1039 2021-11-23 16:45:04.000000 dg-commons-0.0.8/src/dg_commons/sim/models/obstacles.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     9682 2021-10-20 13:10:00.000000 dg-commons-0.0.8/src/dg_commons/sim/models/pedestrian.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1110 2021-10-13 13:29:06.000000 dg-commons-0.0.8/src/dg_commons/sim/models/pedestrian_utils.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1432 2021-10-13 13:29:06.000000 dg-commons-0.0.8/src/dg_commons/sim/models/tires.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      904 2021-10-13 13:29:06.000000 dg-commons-0.0.8/src/dg_commons/sim/models/utils.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     9959 2021-11-19 17:29:11.000000 dg-commons-0.0.8/src/dg_commons/sim/models/vehicle.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     9087 2021-10-13 13:29:06.000000 dg-commons-0.0.8/src/dg_commons/sim/models/vehicle_dynamic.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2692 2021-10-26 14:28:02.000000 dg-commons-0.0.8/src/dg_commons/sim/models/vehicle_ligths.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     7122 2021-11-06 08:57:37.000000 dg-commons-0.0.8/src/dg_commons/sim/models/vehicle_structures.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2265 2021-10-20 13:10:00.000000 dg-commons-0.0.8/src/dg_commons/sim/models/vehicle_utils.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2021-11-23 17:11:33.609321 dg-commons-0.0.8/src/dg_commons/sim/scenarios/
+-rw-rw-r--   0 ale       (1000) ale       (1000)       21 2021-10-13 13:29:06.000000 dg-commons-0.0.8/src/dg_commons/sim/scenarios/__init__.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     5448 2021-10-28 14:36:31.000000 dg-commons-0.0.8/src/dg_commons/sim/scenarios/agent_from_commonroad.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2004 2021-11-21 20:44:39.000000 dg-commons-0.0.8/src/dg_commons/sim/scenarios/factory.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1551 2021-11-23 16:30:41.000000 dg-commons-0.0.8/src/dg_commons/sim/scenarios/structures.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1607 2021-10-20 13:10:00.000000 dg-commons-0.0.8/src/dg_commons/sim/scenarios/utils.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      576 2021-10-13 13:29:06.000000 dg-commons-0.0.8/src/dg_commons/sim/sim_types.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     8645 2021-11-23 16:47:41.000000 dg-commons-0.0.8/src/dg_commons/sim/simulator.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     8354 2021-10-28 10:34:19.000000 dg-commons-0.0.8/src/dg_commons/sim/simulator_animation.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     5247 2021-10-13 13:29:06.000000 dg-commons-0.0.8/src/dg_commons/sim/simulator_structures.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)    10600 2021-11-23 16:47:41.000000 dg-commons-0.0.8/src/dg_commons/sim/simulator_visualisation.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      578 2021-10-20 13:10:00.000000 dg-commons-0.0.8/src/dg_commons/time.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1764 2021-10-20 13:10:00.000000 dg-commons-0.0.8/src/dg_commons/utils_toolz.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      191 2021-10-17 12:50:11.000000 dg-commons-0.0.8/src/dg_commons/utils_types.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2021-11-23 17:11:33.601321 dg-commons-0.0.8/src/dg_commons.egg-info/
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2044 2021-11-23 17:11:33.000000 dg-commons-0.0.8/src/dg_commons.egg-info/PKG-INFO
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2379 2021-11-23 17:11:33.000000 dg-commons-0.0.8/src/dg_commons.egg-info/SOURCES.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        1 2021-11-23 17:11:33.000000 dg-commons-0.0.8/src/dg_commons.egg-info/dependency_links.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)      177 2021-11-23 17:11:33.000000 dg-commons-0.0.8/src/dg_commons.egg-info/requires.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)       28 2021-11-23 17:11:33.000000 dg-commons-0.0.8/src/dg_commons.egg-info/top_level.txt
```

### Comparing `dg-commons-0.0.6/LICENSE` & `dg-commons-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dg-commons-0.0.6/setup.py` & `dg-commons-0.0.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-import pathlib
+import distutils.text_file
+from pathlib import Path
+from typing import List
 
 from setuptools import setup, find_packages
 
 
 def get_version(filename):
     import ast
 
@@ -15,43 +17,40 @@
         else:
             raise ValueError("No version found in %r." % filename)
     if version is None:
         raise ValueError(filename)
     return version
 
 
-install_requires = [
-    "frozendict>=2.0.6",
-    "cytoolz>=0.11.0",
-    "cachetools~=4.2.1",
-    "numpy>=1.21.2",
-    "scipy>=1.7.1",
-    "matplotlib==3.4.3",
-    "shapely>=1.7.0",
-    "PyGeometry-z6>=2.0",
-    "zuper-commons-z6>=6.1.5",
-]
+def _parse_requirements(filename: str) -> List[str]:
+    """Return requirements from requirements file."""
+    return distutils.text_file.TextFile(filename=str(Path(__file__).with_name(filename))).readlines()
+
+
+install_requires = _parse_requirements("requirements.txt")
+extra_requires = {"all": _parse_requirements("requirements-extra.txt")}
 
 module = "dg_commons"
 package = "dg-commons"
 src = "src"
 
 version = get_version(filename=f"src/{module}/__init__.py")
 
 setup(
     name=package,
     author="Alessandro Zanardi",
     author_email="azanardi@ethz.ch",
     url="https://github.com/idsc-frazzoli/dg-commons",
     description="Common tools and utilities related to Driving Games",
-    long_description=(pathlib.Path(__file__).parent / "README.md").read_text(),
+    long_description=(Path(__file__).with_name("README.md")).read_text(),
     long_description_content_type="text/markdown",
     package_dir={"": src},
     packages=find_packages("src"),
     version=version,
     python_requires=">=3.8",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     ],
     install_requires=install_requires,
+    extra_requires=extra_requires,
 )
```

### Comparing `dg-commons-0.0.6/src/dg_commons/controllers/pid.py` & `dg-commons-0.0.8/src/dg_commons/controllers/pid.py`

 * *Files identical despite different names*

### Comparing `dg-commons-0.0.6/src/dg_commons/controllers/pure_pursuit.py` & `dg-commons-0.0.8/src/dg_commons/controllers/pure_pursuit.py`

 * *Files identical despite different names*

### Comparing `dg-commons-0.0.6/src/dg_commons/controllers/speed.py` & `dg-commons-0.0.8/src/dg_commons/controllers/speed.py`

 * *Files identical despite different names*

### Comparing `dg-commons-0.0.6/src/dg_commons/controllers/steer.py` & `dg-commons-0.0.8/src/dg_commons/controllers/steer.py`

 * *Files identical despite different names*

### Comparing `dg-commons-0.0.6/src/dg_commons/dynamics/bicycle_dynamic.py` & `dg-commons-0.0.8/src/dg_commons/dynamics/bicycle_dynamic.py`

 * *Files identical despite different names*

### Comparing `dg-commons-0.0.6/src/dg_commons/geo.py` & `dg-commons-0.0.8/src/dg_commons/geo.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,17 +6,19 @@
     translation_from_SE2,
     SE2,
     T2value,
     translation_angle_from_SE2,
     SE2_from_translation_angle,
     linear_angular_from_se2,
 )
+from shapely.affinity import affine_transform
+from shapely.geometry.base import BaseGeometry
 
 """
-This structures and operations are are taken from duckietown_world with minor modifications
+Some of these structures and operations are are taken from `duckietown-world` with minor modifications
 """
 
 
 def norm_between_SE2value(p0: SE2value, p1: SE2value, ord=None) -> float:
     t0 = translation_from_SE2(p0)
     t1 = translation_from_SE2(p1)
     return np.linalg.norm(t0 - t1, ord=ord)
@@ -70,7 +72,13 @@
         """From a matrix"""
         translation, angle = translation_angle_from_SE2(q)
         return SE2Transform(translation, angle)
 
     def as_SE2(self) -> SE2value:
         M = SE2_from_translation_angle(self.p, self.theta)
         return M
+
+
+def apply_SE2_to_shapely_geo(shapely_geometry: BaseGeometry, se2_value: SE2value) -> BaseGeometry:
+    """Apply SE2 transform to shapely geometry"""
+    coeffs = [se2_value[0, 0], se2_value[1, 0], se2_value[0, 1], se2_value[1, 1], se2_value[0, 2], se2_value[1, 2]]
+    return affine_transform(shapely_geometry, coeffs)
```

### Comparing `dg-commons-0.0.6/src/dg_commons/maps/lanes.py` & `dg-commons-0.0.8/src/dg_commons/maps/lanes.py`

 * *Files identical despite different names*

### Comparing `dg-commons-0.0.6/src/dg_commons/planning/commands_sampler.py` & `dg-commons-0.0.8/src/dg_commons/planning/commands_sampler.py`

 * *Files identical despite different names*

### Comparing `dg-commons-0.0.6/src/dg_commons/planning/goals.py` & `dg-commons-0.0.8/src/dg_commons/planning/goals.py`

 * *Files identical despite different names*

### Comparing `dg-commons-0.0.6/src/dg_commons/planning/motion_primitives.py` & `dg-commons-0.0.8/src/dg_commons/planning/motion_primitives.py`

 * *Files identical despite different names*

### Comparing `dg-commons-0.0.6/src/dg_commons/planning/trajectory.py` & `dg-commons-0.0.8/src/dg_commons/planning/trajectory.py`

 * *Files identical despite different names*

### Comparing `dg-commons-0.0.6/src/dg_commons/planning/trajectory_generator_abc.py` & `dg-commons-0.0.8/src/dg_commons/planning/trajectory_generator_abc.py`

 * *Files identical despite different names*

### Comparing `dg-commons-0.0.6/src/dg_commons/seq/seq_op.py` & `dg-commons-0.0.8/src/dg_commons/seq/seq_op.py`

 * *Files identical despite different names*

### Comparing `dg-commons-0.0.6/src/dg_commons/seq/sequence.py` & `dg-commons-0.0.8/src/dg_commons/seq/sequence.py`

 * *Files identical despite different names*

### Comparing `dg-commons-0.0.6/src/dg_commons/sim/agents/agent.py` & `dg-commons-0.0.8/src/dg_commons/sim/agents/agent.py`

 * *Files identical despite different names*

### Comparing `dg-commons-0.0.6/src/dg_commons/sim/agents/lane_follower.py` & `dg-commons-0.0.8/src/dg_commons/sim/agents/lane_follower.py`

 * *Files identical despite different names*

### Comparing `dg-commons-0.0.6/src/dg_commons/sim/collision.py` & `dg-commons-0.0.8/src/dg_commons/sim/collision.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 from typing import List, Optional, Tuple
 
 import numpy as np
 from geometry import translation_angle_from_SE2
 from shapely.geometry import Polygon
+from shapely.geometry.base import BaseGeometry
 
 from dg_commons import PlayerName
-from dg_commons.sim import ImpactLocation, CollisionReport, logger, SimModel
+from dg_commons.sim import ImpactLocation, CollisionReport, logger, SimModel, SimTime
 from dg_commons.sim.collision_structures import CollisionReportPlayer
 from dg_commons.sim.collision_utils import (
     compute_impact_geometry,
     velocity_after_collision,
     kinetic_energy,
     compute_impulse_response,
     rot_velocity_after_collision,
     velocity_of_P_given_A,
     CollisionException,
     chek_who_is_at_fault,
 )
+from dg_commons.sim.models.obstacles import StaticObstacle
 from dg_commons.sim.simulator import SimContext
 
 
-def impact_locations_from_polygons(a_model: SimModel, b_model: SimModel) -> List[Tuple[ImpactLocation, Polygon]]:
+def impact_locations_from_polygons(a_model: SimModel, b_shape: BaseGeometry) -> List[Tuple[ImpactLocation, Polygon]]:
     """
     Checks the impact locations of A based on its mesh and the footprint of B
     :return:
     """
     locations: List[Tuple[ImpactLocation, Polygon]] = []
     a_mesh = a_model.get_mesh()
-    b_shape = b_model.get_footprint()
     for loc, loc_shape in a_mesh.items():
         if b_shape.intersects(loc_shape):
             locations.append((loc, loc_shape))
     if not locations:
         raise CollisionException(f"Detected a collision but unable to find the impact location for model {a_model}")
     return locations
 
@@ -65,22 +66,22 @@
         return None
 
     # Update state of the model, it has collided
     a_model.has_collided = True
     b_model.has_collided = True
 
     # Compute collision locations
-    a_locations = impact_locations_from_polygons(a_model, b_model)
-    b_locations = impact_locations_from_polygons(b_model, a_model)
+    a_locations = impact_locations_from_polygons(a_model, b_shape)
+    b_locations = impact_locations_from_polygons(b_model, a_shape)
 
     # Check who is at fault
     who_is_at_fault = chek_who_is_at_fault(
         {a: a_model.get_pose(), b: b_model.get_pose()},
         impact_point=impact_point,
-        lanelet_network=sim_context.scenario.lanelet_network,
+        lanelet_network=sim_context.dg_scenario.lanelet_network,
     )
     a_fault, b_fault = who_is_at_fault[a], who_is_at_fault[b]
 
     # Compute impulse resolution
     a_geom = a_model.get_geometry()
     b_geom = b_model.get_geometry()
     j_n = compute_impulse_response(
@@ -116,7 +117,65 @@
     )
     return CollisionReport(
         players={a: a_report, b: b_report},
         impact_point=impact_point,
         impact_normal=impact_normal,
         at_time=sim_context.time,
     )
+
+
+def resolve_collision_with_environment(
+    a: PlayerName, a_model: SimModel, b_obstacle: StaticObstacle, time: SimTime
+) -> Optional[CollisionReport]:
+    a_shape = a_model.get_footprint()
+    b_shape = b_obstacle.shape
+    # Compute collision geometry
+    impact_normal, impact_point = compute_impact_geometry(a_shape, b_shape)
+    a_cog = translation_angle_from_SE2(a_model.get_pose())[0]
+    r_ap = np.array(impact_point.coords[0]) - np.array(a_cog)
+    a_vel, a_omega = a_model.get_velocity(in_model_frame=False)
+    a_vel_atP = velocity_of_P_given_A(a_vel, a_omega, r_ap)
+    rel_velocity_atP = a_vel_atP
+
+    if np.dot(rel_velocity_atP, impact_normal) < 0:
+        logger.debug(f"Not solving the collision,  since they are already separating")
+        return None
+
+    # Update state of the model, it has collided
+    a_model.has_collided = True
+
+    # Compute collision locations
+    a_locations = impact_locations_from_polygons(a_model, b_shape)
+
+    # If you collide with the environment it is your fault
+    a_fault = True
+
+    # Compute impulse resolution
+    a_geom = a_model.get_geometry()
+    b_geom = b_obstacle.geometry
+    r_bp = np.array([1, 1])  # irrelevant since it will disappear divided by infinity
+    j_n = compute_impulse_response(
+        n=impact_normal, vel_ab=rel_velocity_atP, r_ap=r_ap, r_bp=r_bp, a_geom=a_geom, b_geom=b_geom
+    )
+    # Apply impulse to models
+    a_vel_after = velocity_after_collision(impact_normal, a_vel, a_geom.m, j_n)
+    a_omega_after = rot_velocity_after_collision(r_ap, impact_normal, a_omega, a_geom.Iz, j_n)
+    a_model.set_velocity(a_vel_after, a_omega_after, in_model_frame=False)
+
+    # Log reports
+    a_kenergy_delta = kinetic_energy(a_vel_after, a_geom.m) - kinetic_energy(a_vel, a_geom.m)
+    # todo rotational energy
+    a_report = CollisionReportPlayer(
+        locations=a_locations,
+        at_fault=a_fault,
+        footprint=a_shape,
+        velocity=(a_vel, a_omega),
+        velocity_after=(a_vel_after, a_omega_after),
+        energy_delta=a_kenergy_delta,
+    )
+
+    return CollisionReport(
+        players={a: a_report},
+        impact_point=impact_point,
+        impact_normal=impact_normal,
+        at_time=time,
+    )
```

### Comparing `dg-commons-0.0.6/src/dg_commons/sim/collision_structures.py` & `dg-commons-0.0.8/src/dg_commons/sim/collision_structures.py`

 * *Files identical despite different names*

### Comparing `dg-commons-0.0.6/src/dg_commons/sim/collision_utils.py` & `dg-commons-0.0.8/src/dg_commons/sim/collision_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from math import pi
 from typing import List, Tuple, Mapping, Dict
 
 import numpy as np
 from commonroad.scenario.lanelet import LaneletNetwork
 from geometry import T2value, SO2value, SO2_from_angle, SE2value
 from shapely.geometry import Polygon, Point, LineString
+from shapely.geometry.base import BaseGeometry
 from toolz import remove
 
 from dg_commons.maps.lanes import DgLanelet, DgLanePose
 from dg_commons import X, PlayerName
 from dg_commons.sim.models.model_structures import ModelGeometry
 
 
@@ -22,29 +23,29 @@
 
 def velocity_of_P_given_A(vel: T2value, omega: float, vec_ap: T2value) -> T2value:
     """Compute velocity of point P given velocity at A, rotational velocity of the rigid body and vector AP"""
     # rotate by 90 to be equivalent to cross product omega x r_ap
     return vel + omega * (_rot90 @ vec_ap)
 
 
-def _find_intersection_points(a_shape: Polygon, b_shape: Polygon) -> List[Tuple[float, float]]:
+def _find_intersection_points(a_shape: Polygon, b_shape: BaseGeometry) -> List[Tuple[float, float]]:
     int_shape = a_shape.intersection(b_shape)
     points = list(int_shape.exterior.coords[:-1])
 
     def is_contained_in_aorb(p) -> bool:
         shapely_point = Point(p).buffer(1.0e-9)
         return a_shape.contains(shapely_point) or b_shape.contains(shapely_point)
 
     points = list(remove(is_contained_in_aorb, points))
     if not len(points) == 2:
         from matplotlib import pyplot as plt
 
         plt.figure()
         plt.plot(*a_shape.exterior.xy, "b")
-        plt.plot(*b_shape.exterior.xy, "r")
+        plt.plot(*b_shape.xy, "r")
         for p in points:
             plt.plot(*p, "o")
         plt.savefig(f"coll_debug{time.time()}.png")
         raise CollisionException(f"At the moment collisions with {len(points)} intersecting points are not supported")
     return points
 
 
@@ -52,15 +53,15 @@
     """returns the impact point angle wrt to the vehicle"""
     # Direction of Force (DOF) -> vector that goes from car center to impact point
     abs_angle_dof = np.arctan2(impact_point.y - state.y, impact_point.x - state.x)
     car_heading: float = state.theta
     return abs_angle_dof - car_heading
 
 
-def compute_impact_geometry(a: Polygon, b: Polygon) -> (np.ndarray, Point):
+def compute_impact_geometry(a: Polygon, b: BaseGeometry) -> (np.ndarray, Point):
     """
     This computes the normal of impact between vehicles a and b
     :param a: Polygon object
     :param b: Polygon object
     :return: normal of impact and the impact point
     """
     assert not a.touches(b)
@@ -80,19 +81,19 @@
 def compute_impulse_response(
     n: np.ndarray, vel_ab: np.ndarray, r_ap: np.ndarray, r_bp: np.ndarray, a_geom: ModelGeometry, b_geom: ModelGeometry
 ) -> float:
     """
     The impulse J is defined in terms of force F and time period ∆t
     J = F*∆t = ma*∆t = m *∆v/∆t *∆t = m*∆v
     :param n:             Vector onto which to project rel_v (normally, n or t)
-    :param vel_ab:           Relative velocity between a and b
+    :param vel_ab:          Relative velocity between a and b
     :param r_ap:            Vector from CG of a to collision point P
     :param r_bp:            Vector from CG of b to collision point P
-    :param a_geom:          Geometry of vehicle a
-    :param b_geom:          Geometry of vehicle b
+    :param a_geom:          Geometry of model a
+    :param b_geom:          Geometry of model b
     :return:
     """
     # Restitution coefficient -> represents the "bounciness" of the vehicle
     e = min(a_geom.e, b_geom.e)
     j = -(1 + e) * np.dot(vel_ab, n)
     rot_part = (np.cross(r_ap, n) ** 2 / a_geom.Iz) + (np.cross(r_bp, n) ** 2 / b_geom.Iz)
     j /= 1 / a_geom.m + 1 / b_geom.m + rot_part
```

### Comparing `dg-commons-0.0.6/src/dg_commons/sim/collision_visualisation.py` & `dg-commons-0.0.8/src/dg_commons/sim/collision_visualisation.py`

 * *Files identical despite different names*

### Comparing `dg-commons-0.0.6/src/dg_commons/sim/models/model_structures.py` & `dg-commons-0.0.8/src/dg_commons/sim/models/model_structures.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
+from math import inf
 from typing import Tuple, Sequence, NewType
 
 from dg_commons import Color
 
 __all__ = [
     "ModelType",
     "CAR",
     "MOTORCYCLE",
     "BICYCLE",
     "PEDESTRIAN",
+    "TRUCK",
     "ModelGeometry",
     "ModelParameters",
     "TwoWheelsTypes",
     "FourWheelsTypes",
 ]
 
 ModelType = NewType("ModelType", str)
@@ -41,14 +43,24 @@
     @property
     @abstractmethod
     def outline(self) -> Sequence[Tuple[float, float]]:
         pass
 
 
 @dataclass(frozen=True, unsafe_hash=True)
+class StaticModelGeometry(ModelGeometry):
+    def outline(self) -> Sequence[Tuple[float, float]]:
+        raise NotImplementedError("Outline method for static model geometry is not implemented")
+
+    @staticmethod
+    def default() -> "StaticModelGeometry":
+        return StaticModelGeometry(m=inf, Iz=inf, e=0.4, color="black")
+
+
+@dataclass(frozen=True, unsafe_hash=True)
 class ModelParameters:
     vx_limits: Tuple[float, float]
     """ Minimum and Maximum velocities [m/s] """
     acc_limits: Tuple[float, float]
     """ Minimum and Maximum acceleration [m/s^2] """
 
     def __post_init__(self):
```

### Comparing `dg-commons-0.0.6/src/dg_commons/sim/models/model_utils.py` & `dg-commons-0.0.8/src/dg_commons/sim/models/model_utils.py`

 * *Files identical despite different names*

### Comparing `dg-commons-0.0.6/src/dg_commons/sim/models/pedestrian.py` & `dg-commons-0.0.8/src/dg_commons/sim/models/pedestrian.py`

 * *Files identical despite different names*

### Comparing `dg-commons-0.0.6/src/dg_commons/sim/models/pedestrian_utils.py` & `dg-commons-0.0.8/src/dg_commons/sim/models/pedestrian_utils.py`

 * *Files identical despite different names*

### Comparing `dg-commons-0.0.6/src/dg_commons/sim/models/tires.py` & `dg-commons-0.0.8/src/dg_commons/sim/models/tires.py`

 * *Files identical despite different names*

### Comparing `dg-commons-0.0.6/src/dg_commons/sim/models/utils.py` & `dg-commons-0.0.8/src/dg_commons/sim/models/utils.py`

 * *Files identical despite different names*

### Comparing `dg-commons-0.0.6/src/dg_commons/sim/models/vehicle.py` & `dg-commons-0.0.8/src/dg_commons/sim/models/vehicle.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,20 +17,21 @@
 from dg_commons.sim.models.vehicle_structures import VehicleGeometry
 from dg_commons.sim.models.vehicle_utils import steering_constraint, VehicleParameters
 from dg_commons.sim.simulator_structures import SimModel
 
 
 @dataclass(unsafe_hash=True, eq=True, order=True)
 class VehicleCommands:
+    # todo add horn
     acc: float
     """ Acceleration [m/s^2] """
     ddelta: float
     """ Steering rate [rad/s] (delta derivative) """
     lights: LightsCmd = NO_LIGHTS
-    # todo add horn
+    """ Lights for the car, indicators"""
     idx = frozendict({"acc": 0, "ddelta": 1})
     """ Dictionary to get correct values from numpy arrays"""
 
     @classmethod
     def get_n_commands(cls) -> int:
         return len(cls.idx)
 
@@ -215,15 +216,15 @@
         assert footprint.is_valid
         return footprint
 
     def get_mesh(self) -> Mapping[ImpactLocation, Polygon]:
         footprint = self.get_footprint()
         vertices = footprint.exterior.coords[:-1]
         cxy = footprint.centroid.coords[0]
-        # maybe we can use triangulate from shapely
+        # fixme maybe we can use triangulate from shapely inferring the side from the relative angle
         impact_locations: Mapping[ImpactLocation, Polygon] = {
             IMPACT_RIGHT: Polygon([cxy, vertices[0], vertices[3], cxy]),
             IMPACT_LEFT: Polygon([cxy, vertices[1], vertices[2], cxy]),
             IMPACT_BACK: Polygon([cxy, vertices[0], vertices[1], cxy]),
             IMPACT_FRONT: Polygon([cxy, vertices[2], vertices[3], cxy]),
         }
         for shape in impact_locations.values():
```

### Comparing `dg-commons-0.0.6/src/dg_commons/sim/models/vehicle_dynamic.py` & `dg-commons-0.0.8/src/dg_commons/sim/models/vehicle_dynamic.py`

 * *Files identical despite different names*

### Comparing `dg-commons-0.0.6/src/dg_commons/sim/models/vehicle_ligths.py` & `dg-commons-0.0.8/src/dg_commons/sim/models/vehicle_ligths.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,18 @@
     "NO_LIGHTS",
     "LIGHTS_HEADLIGHTS",
     "LIGHTS_TURN_LEFT",
     "LIGHTS_TURN_RIGHT",
     "LIGHTS_HAZARD",
     "LightsValues",
     "LightsColors",
+    "lightscmd2phases",
+    "get_phased_lights",
+    "red",
+    "red_more",
 ]
 
 LightsCmd = NewType("LightsCmd", str)
 """ The type of light commands. """
 NO_LIGHTS = LightsCmd("none")
 """ Lights are off. """
 LIGHTS_HEADLIGHTS = LightsCmd("headlights")
```

### Comparing `dg-commons-0.0.6/src/dg_commons/sim/models/vehicle_structures.py` & `dg-commons-0.0.8/src/dg_commons/sim/models/vehicle_structures.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from dataclasses import dataclass
 from functools import cached_property
-from typing import Tuple, List, Optional, Mapping
+from typing import Tuple, List, Mapping
 
 import numpy as np
 from geometry import SE2_from_xytheta
 from shapely.geometry import Polygon
 from zuper_commons.types import ZValueError
 
 from dg_commons import Color
@@ -42,59 +42,72 @@
     c_rr_r: float
     """ Rolling Resistance coefficient rear """
     h_cog: float = 0.7
     """ Height of the CoG [m] """
 
     # todo fix default rotational inertia
     @classmethod
-    def default_car(cls, color: Optional[Color] = None) -> "VehicleGeometry":
-        color = "royalblue" if color is None else color
+    def default_car(
+        cls,
+        color: Color = "royalblue",
+        m=1500.0,
+        Iz=1300,
+        w_half=0.9,
+        lf=1.7,
+        lr=1.7,
+    ) -> "VehicleGeometry":
         return VehicleGeometry(
             vehicle_type=CAR,
-            m=1500.0,
-            Iz=1300,
-            w_half=0.9,
-            lf=1.7,
-            lr=1.7,
+            m=m,
+            Iz=Iz,
+            w_half=w_half,
+            lf=lf,
+            lr=lr,
             c_drag=0.3756,
             a_drag=2,
             e=0.5,
             c_rr_f=0.003,
             c_rr_r=0.003,
             color=color,
         )
 
     @classmethod
-    def default_bicycle(cls, color: Optional[Color] = None) -> "VehicleGeometry":
-        color = "saddlebrown" if color is None else color
+    def default_bicycle(
+        cls,
+        color: Color = "saddlebrown",
+        m=85.0,
+        Iz=90,
+        w_half=0.25,
+        lf=1.0,
+        lr=1.0,
+    ) -> "VehicleGeometry":
         return VehicleGeometry(
             vehicle_type=BICYCLE,
-            m=85.0,
-            Iz=90,
-            w_half=0.25,
-            lf=1.0,
-            lr=1.0,
+            m=m,
+            Iz=Iz,
+            w_half=w_half,
+            lf=lf,
+            lr=lr,
             c_drag=0.01,
             a_drag=0.2,
             e=0.35,
             c_rr_f=0.003,
             c_rr_r=0.003,
             color=color,
         )
 
     @classmethod
-    def default_truck(cls, color: Optional[Color] = None) -> "VehicleGeometry":
-        color = "darkgreen" if color is None else color
+    def default_truck(cls, color: Color = "darkgreen", m=8000.0, Iz=6300, w_half=1.2, lf=4, lr=4) -> "VehicleGeometry":
         return VehicleGeometry(
             vehicle_type=TRUCK,
-            m=8000.0,
-            Iz=6300,
-            w_half=1.2,
-            lf=4,
-            lr=4,
+            m=m,
+            Iz=Iz,
+            w_half=w_half,
+            lf=lf,
+            lr=lr,
             c_drag=0.3756,
             a_drag=4,
             e=0.5,
             c_rr_f=0.03,
             c_rr_r=0.03,
             color=color,
         )
```

### Comparing `dg-commons-0.0.6/src/dg_commons/sim/models/vehicle_utils.py` & `dg-commons-0.0.8/src/dg_commons/sim/models/vehicle_utils.py`

 * *Files identical despite different names*

### Comparing `dg-commons-0.0.6/src/dg_commons/sim/scenarios/agent_from_commonroad.py` & `dg-commons-0.0.8/src/dg_commons/sim/scenarios/agent_from_commonroad.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,24 +82,29 @@
     beta = 1.6
     area = length * width
     mass = alpha * area ** beta
     inertia = mass * (length + width) / 6
     return mass, inertia
 
 
-def dglane_from_position(p: T2value, network: LaneletNetwork):
+def dglane_from_position(
+    p: T2value, network: LaneletNetwork, init_lane_selection: int = 0, succ_lane_selection: int = 0
+) -> DgLanelet:
     """Gets the first merged lane from the current position"""
+    # todo add possibility to select the number of the lane successor (0 by default)
     lane_id = network.find_lanelet_by_position(
         [
             p,
         ]
     )
     assert len(lane_id[0]) > 0, p
-    lane = network.find_lanelet_by_id(lane_id[0][0])
-    merged_lane = Lanelet.all_lanelets_by_merging_successors_from_lanelet(lanelet=lane, network=network)[0][0]
+    lane = network.find_lanelet_by_id(lane_id[0][init_lane_selection])
+    merged_lane = Lanelet.all_lanelets_by_merging_successors_from_lanelet(lanelet=lane, network=network)[0][
+        succ_lane_selection
+    ]
     return DgLanelet.from_commonroad_lanelet(merged_lane)
 
 
 def infer_lane_from_dyn_obs(dyn_obs: DynamicObstacle, network: LaneletNetwork) -> DgLanelet:
     """Tries to find a lane corresponding to the trajectory, if no lane is found it creates one from the trajectory"""
     init_position = dyn_obs.initial_state.position
     end_position = dyn_obs.prediction.trajectory.state_list[-1].position
```

### Comparing `dg-commons-0.0.6/src/dg_commons/sim/scenarios/factory.py` & `dg-commons-0.0.8/src/dg_commons/sim/scenarios/factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Optional
 
 from dg_commons import PlayerName
 from dg_commons.sim import logger, SimLog, SimParameters
 from dg_commons.sim.scenarios import load_commonroad_scenario
 from dg_commons.sim.scenarios.agent_from_commonroad import model_agent_from_dynamic_obstacle, NotSupportedConversion
+from dg_commons.sim.scenarios.structures import DgScenario
 from dg_commons.sim.simulator import SimContext
 
 
 def get_scenario_commonroad_replica(
     scenario_name: str,
     scenarios_dir: Optional[str] = None,
     sim_param: Optional[SimParameters] = None,
@@ -36,13 +37,13 @@
             players.update({playername: agent})
             models.update({playername: model})
         except NotSupportedConversion as e:
             logger.warn("Unable to convert commonroad dynamic obstacle due to " + e.args[0] + " skipping...")
     logger.info(f"Managed to load {len(players)}")
     sim_param = SimParameters() if sim_param is None else sim_param
     return SimContext(
-        scenario=scenario,
+        dg_scenario=DgScenario(scenario),
         models=models,
         players=players,
         log=SimLog(),
         param=sim_param,
     )
```

### Comparing `dg-commons-0.0.6/src/dg_commons/sim/scenarios/utils.py` & `dg-commons-0.0.8/src/dg_commons/sim/scenarios/utils.py`

 * *Files identical despite different names*

### Comparing `dg-commons-0.0.6/src/dg_commons/sim/sim_types.py` & `dg-commons-0.0.8/src/dg_commons/sim/sim_types.py`

 * *Files identical despite different names*

### Comparing `dg-commons-0.0.6/src/dg_commons/sim/simulator.py` & `dg-commons-0.0.8/src/dg_commons/sim/simulator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,54 @@
 from dataclasses import dataclass, field
 from decimal import Decimal
 from itertools import combinations
 from typing import Mapping, Optional, List, Dict
 
-from commonroad.scenario.scenario import Scenario
-
 from dg_commons import PlayerName, U
 from dg_commons.sim import SimTime, CollisionReport, logger
 from dg_commons.sim.agents.agent import Agent, TAgent
 from dg_commons.sim.collision_utils import CollisionException
+from dg_commons.sim.scenarios.structures import DgScenario
 from dg_commons.sim.simulator_structures import *
 from dg_commons.time import time_function
 
 
 @dataclass
 class SimContext:
     """The simulation context that keeps track of everything, handle with care as it is passed around by reference and
     it is a mutable object"""
 
-    scenario: Scenario
+    dg_scenario: DgScenario
     models: Mapping[PlayerName, SimModel]
     players: Mapping[PlayerName, TAgent]
     param: SimParameters
     log: SimLog = field(default_factory=SimLog)
     time: SimTime = SimTime(0)
     seed: int = 0
     sim_terminated: bool = False
     collision_reports: List[CollisionReport] = field(default_factory=list)
     first_collision_ts: SimTime = SimTime("Infinity")
 
     def __post_init__(self):
         assert self.models.keys() == self.players.keys()
-        assert isinstance(self.scenario, Scenario), self.scenario
+        assert isinstance(self.dg_scenario, DgScenario), self.dg_scenario
         for pname in self.models.keys():
             assert issubclass(type(self.models[pname]), SimModel)
             assert issubclass(type(self.players[pname]), Agent)
 
 
 class Simulator:
     """
     A simulator has a loop made of 3 main steps:
         - A pre-update function creating the observations for the agents
         - An update function which asks the agents the commands and applies them to the dynamics of each model
         - A post-update function that checks the new states of all the models and resolves collisions
     """
 
-    # fixme check if this is okay once you have multple simulators running together
+    # fixme check if this is okay once you have multiple simulators running together
     last_observations: Optional[SimObservations] = SimObservations(players={}, time=Decimal(0))
     last_get_commands_ts: SimTime = SimTime("-Infinity")
     last_commands: Dict[PlayerName, U] = {}
     simlogger: Dict[PlayerName, PlayerLogger] = {}
 
     @time_function
     def run(self, sim_context: SimContext):
@@ -100,15 +99,16 @@
             self.last_get_commands_ts = t
         return
 
     def post_update(self, sim_context: SimContext):
         """
         Here all the operations that happen after we have stepped the simulation, e.g. collision checking
         """
-        collision_detected = self._check_collisions(sim_context)
+        collision_enviroment = self._check_collisions_with_environment(sim_context)
+        collision_players = self._check_collisions_among_players(sim_context)
         # after all the computations advance simulation time
         sim_context.time += sim_context.param.dt
         self._maybe_terminate_simulation(sim_context)
         return
 
     @staticmethod
     def _maybe_terminate_simulation(sim_context: SimContext):
@@ -116,27 +116,55 @@
         termination_condition: bool = (
             sim_context.time > sim_context.param.max_sim_time
             or sim_context.time > sim_context.first_collision_ts + sim_context.param.sim_time_after_collision
         )
         sim_context.sim_terminated = termination_condition
 
     @staticmethod
-    def _check_collisions(sim_context: SimContext) -> bool:
+    def _check_collisions_with_environment(sim_context: SimContext) -> bool:
+        """Check collisions of the players with the environment"""
+        from dg_commons.sim.collision import resolve_collision_with_environment  # import here to avoid circular imports
+
+        env_obstacles = sim_context.dg_scenario.strtree_obstacles
+        collision = False
+        for p, p_model in sim_context.models.items():
+            p_shape = p_model.get_footprint()
+            items = env_obstacles.query_items(p_shape)
+            for idx in items:
+                candidate = sim_context.dg_scenario.static_obstacles[idx]
+                if p_shape.intersects(candidate.shape):
+                    try:
+                        report: Optional[CollisionReport] = resolve_collision_with_environment(
+                            p, p_model, candidate, sim_context.time
+                        )
+                    except CollisionException as e:
+                        logger.warn(f"Failed to resolve collision of {p} with environment because:\n{e.args}")
+                        report = None
+                    if report is not None:
+                        logger.info(f"Player {p} collided with the environment")
+                        collision = True
+                        sim_context.collision_reports.append(report)
+                        if sim_context.time < sim_context.first_collision_ts:
+                            sim_context.first_collision_ts = sim_context.time
+        return collision
+
+    @staticmethod
+    def _check_collisions_among_players(sim_context: SimContext) -> bool:
         """
         This checks only collision location at the current step, tunneling effects and similar are ignored
         :param sim_context:
         :return: True if at least one collision happened, False otherwise
         """
+        from dg_commons.sim.collision import resolve_collision  # import here to avoid circular imports
+
         collision = False
         for p1, p2 in combinations(sim_context.models, 2):
             a_shape = sim_context.models[p1].get_footprint()
             b_shape = sim_context.models[p2].get_footprint()
             if a_shape.intersects(b_shape):
-                from dg_commons.sim.collision import resolve_collision  # import here to avoid circular imports
-
                 try:
                     report: Optional[CollisionReport] = resolve_collision(p1, p2, sim_context)
                 except CollisionException as e:
                     logger.warn(f"Failed to resolve collision between {p1} and {p2} because:\n{e.args}")
                     report = None
                 if report is not None:
                     logger.info(f"Detected a collision between {p1} and {p2}")
```

### Comparing `dg-commons-0.0.6/src/dg_commons/sim/simulator_animation.py` & `dg-commons-0.0.8/src/dg_commons/sim/simulator_animation.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,24 +2,32 @@
 from itertools import chain
 from typing import Mapping, List, Union, Optional, Sequence
 
 from matplotlib import pyplot as plt
 from matplotlib.animation import FuncAnimation
 from matplotlib.axes import Axes
 from toolz.sandbox import unzip
+from zuper_commons.types import ZValueError
 
-from dg_commons import Timestamp
-from dg_commons.time import time_function
 from dg_commons import PlayerName, X
+from dg_commons import Timestamp
 from dg_commons.sim import logger
 from dg_commons.sim.models.vehicle import VehicleCommands
-from dg_commons.sim.models.vehicle_ligths import lightscmd2phases, get_phased_lights, red, red_more, LightsColors
+from dg_commons.sim.models.vehicle_ligths import (
+    lightscmd2phases,
+    get_phased_lights,
+    red,
+    red_more,
+    LightsColors,
+    LightsCmd,
+)
 from dg_commons.sim.simulator import SimContext
 from dg_commons.sim.simulator_structures import LogEntry
 from dg_commons.sim.simulator_visualisation import SimRenderer, approximate_bounding_box_players, ZOrders
+from dg_commons.time import time_function
 
 
 @time_function
 def create_animation(
     file_path: str,
     sim_context: SimContext,
     figsize: Optional[Union[list, tuple]] = None,
@@ -69,15 +77,15 @@
         )
 
     def init_plot():
         ax.clear()
         with sim_viz.plot_arena(ax=ax):
             init_log_entry: Mapping[PlayerName, LogEntry] = sim_context.log.at_interp(time_begin)
             for pname, plog in init_log_entry.items():
-                lights_colors: LightsColors = _get_lights_colors_from_cmds(init_log_entry[pname].commands, t=0)
+                lights_colors: LightsColors = get_lights_colors_from_cmds(init_log_entry[pname].commands, t=0)
                 states[pname], actions[pname] = sim_viz.plot_player(
                     ax=ax,
                     state=plog.state,
                     lights_colors=lights_colors,
                     player_name=pname,
                     alpha=0.7,
                     plot_wheels=plot_wheels,
@@ -105,15 +113,15 @@
         return _get_list()
 
     def update_plot(frame: int = 0):
         t: float = frame * dt / 1000.0
         logger.info(f"Plotting t = {t}\r")
         log_at_t: Mapping[PlayerName, LogEntry] = sim_context.log.at_interp(t)
         for pname, box_handle in states.items():
-            lights_colors: LightsColors = _get_lights_colors_from_cmds(log_at_t[pname].commands, t=t)
+            lights_colors: LightsColors = get_lights_colors_from_cmds(log_at_t[pname].commands, t=t)
             states[pname], actions[pname] = sim_viz.plot_player(
                 ax=ax,
                 player_name=pname,
                 state=log_at_t[pname].state,
                 lights_colors=lights_colors,
                 vehicle_poly=box_handle,
                 lights_patches=actions[pname],
@@ -158,41 +166,51 @@
         fps=fps,
         # extra_args=["-g", "1", "-keyint_min", str(interval_seconds)]
     )
     logger.info("Animation saved...")
     ax.clear()
 
 
-def adjust_axes_limits(ax: Axes, plot_limits: Union[str, Sequence[Sequence[float]]], players_states: Sequence[X]):
+def adjust_axes_limits(
+    ax: Axes, plot_limits: Union[str, Sequence[Sequence[float]]], players_states: Optional[Sequence[X]] = None
+):
     if plot_limits is None:
         ax.autoscale()
     elif plot_limits == "auto":
+        if plot_limits is None:
+            raise ZValueError('Plotting with "auto" option requires players positions')
         players_limits = approximate_bounding_box_players(obj_list=players_states)
         if players_limits is not None:
             ax.axis(
                 xmin=players_limits[0][0],
                 xmax=players_limits[0][1],
                 ymin=players_limits[1][0],
                 ymax=players_limits[1][1],
             )
         else:
             ax.autoscale()
     else:
-        ax.xlim(plot_limits[0][0], plot_limits[0][1])
-        ax.ylim(plot_limits[1][0], plot_limits[1][1])
+        # plotlimits are expected to be seq of seq of floats
+        ax.set_xlim(plot_limits[0][0], plot_limits[0][1])
+        ax.set_ylim(plot_limits[1][0], plot_limits[1][1])
     return
 
 
-def _get_lights_colors_from_cmds(cmds: VehicleCommands, t: Timestamp) -> LightsColors:
+def get_lights_colors_from_cmds(cmds: VehicleCommands, t: Timestamp) -> LightsColors:
     """Note that braking lights are out of the agent's control"""
     try:
-        phases = lightscmd2phases[cmds.lights]
-        lights_colors = get_phased_lights(phases, float(t))
-        if cmds.acc < 0:  # and cmds == NO_LIGHTS:
-            if lights_colors.back_left == red:
-                lights_colors.back_left = red_more
-            if lights_colors.back_right == red:
-                lights_colors.back_right = red_more
+        lights_colors = lights_colors_from_lights_cmd(cmds.lights, cmds.acc, t)
     except AttributeError:
         # in case the model commands does not have lights command
         lights_colors = None
     return lights_colors
+
+
+def lights_colors_from_lights_cmd(lights_cmd: LightsCmd, acc: float, t: Timestamp) -> LightsColors:
+    phases = lightscmd2phases[lights_cmd]
+    lights_colors = get_phased_lights(phases, float(t))
+    if acc < 0:  # and cmds == NO_LIGHTS:
+        if lights_colors.back_left == red:
+            lights_colors.back_left = red_more
+        if lights_colors.back_right == red:
+            lights_colors.back_right = red_more
+    return lights_colors
```

### Comparing `dg-commons-0.0.6/src/dg_commons/sim/simulator_structures.py` & `dg-commons-0.0.8/src/dg_commons/sim/simulator_structures.py`

 * *Files identical despite different names*

### Comparing `dg-commons-0.0.6/src/dg_commons/sim/simulator_visualisation.py` & `dg-commons-0.0.8/src/dg_commons/sim/simulator_visualisation.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,23 +9,24 @@
 from decorator import contextmanager
 from geometry import SE2_from_xytheta, SE2value
 from matplotlib.axes import Axes
 from matplotlib.collections import LineCollection, PathCollection
 from matplotlib.lines import Line2D
 from matplotlib.patches import Polygon, Circle
 
+from dg_commons import Color
 from dg_commons import PlayerName, X, U
+from dg_commons.maps.shapely_viz import ShapelyViz
 from dg_commons.planning.trajectory import Trajectory
 from dg_commons.sim.models.pedestrian import PedestrianState, PedestrianGeometry
 from dg_commons.sim.models.vehicle import VehicleState, VehicleGeometry
 from dg_commons.sim.models.vehicle_ligths import LightsColors
 from dg_commons.sim.simulator import SimContext
-from dg_commons import Color
 
-__all__ = ["SimRenderer"]
+__all__ = ["SimRenderer", "plot_vehicle", "plot_pedestrian", "plot_trajectories"]
 
 
 class SimRendererABC(Generic[X, U], ABC):
     """An artist that can draw the game."""
 
     @abstractmethod
     def plot_arena(self, ax: Axes):
@@ -51,22 +52,25 @@
 
 class SimRenderer(SimRendererABC):
     """Visualization for the trajectory games"""
 
     def __init__(self, sim_context: SimContext, ax: Axes = None, *args, **kwargs):
         self.sim_context = sim_context
         self.commonroad_renderer: MPRenderer = MPRenderer(ax=ax, *args, **kwargs)
+        self.shapely_viz = ShapelyViz(ax=self.commonroad_renderer.ax)
 
     @contextmanager
     def plot_arena(self, ax: Axes):
-        # planning_problem_set.draw(rnd)
-        self.sim_context.scenario.lanelet_network.draw(
-            self.commonroad_renderer, draw_params={"traffic_light": {"draw_traffic_lights": False}}
-        )
-        self.commonroad_renderer.render()
+        if self.sim_context.dg_scenario.scenario:
+            self.sim_context.dg_scenario.lanelet_network.draw(
+                self.commonroad_renderer, draw_params={"traffic_light": {"draw_traffic_lights": False}}
+            )
+            self.commonroad_renderer.render()
+        for s_obstacle in self.sim_context.dg_scenario.static_obstacles.values():
+            self.shapely_viz.add_shape(s_obstacle.shape, color=s_obstacle.geometry.color)
         yield
 
     def plot_player(
         self,
         ax: Axes,
         player_name: PlayerName,
         state: X,
```

### Comparing `dg-commons-0.0.6/src/dg_commons/time.py` & `dg-commons-0.0.8/src/dg_commons/time.py`

 * *Files identical despite different names*

### Comparing `dg-commons-0.0.6/src/dg_commons/utils_toolz.py` & `dg-commons-0.0.8/src/dg_commons/utils_toolz.py`

 * *Files identical despite different names*

### Comparing `dg-commons-0.0.6/src/dg_commons.egg-info/SOURCES.txt` & `dg-commons-0.0.8/src/dg_commons.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 src/dg_commons/controllers/pure_pursuit.py
 src/dg_commons/controllers/speed.py
 src/dg_commons/controllers/steer.py
 src/dg_commons/dynamics/__init__.py
 src/dg_commons/dynamics/bicycle_dynamic.py
 src/dg_commons/maps/__init__.py
 src/dg_commons/maps/lanes.py
+src/dg_commons/maps/road_bounds.py
+src/dg_commons/maps/shapely_viz.py
 src/dg_commons/planning/__init__.py
 src/dg_commons/planning/commands_sampler.py
 src/dg_commons/planning/goals.py
 src/dg_commons/planning/motion_primitives.py
 src/dg_commons/planning/trajectory.py
 src/dg_commons/planning/trajectory_generator_abc.py
 src/dg_commons/seq/__init__.py
@@ -43,20 +45,22 @@
 src/dg_commons/sim/simulator_visualisation.py
 src/dg_commons/sim/agents/__init__.py
 src/dg_commons/sim/agents/agent.py
 src/dg_commons/sim/agents/lane_follower.py
 src/dg_commons/sim/models/__init__.py
 src/dg_commons/sim/models/model_structures.py
 src/dg_commons/sim/models/model_utils.py
+src/dg_commons/sim/models/obstacles.py
 src/dg_commons/sim/models/pedestrian.py
 src/dg_commons/sim/models/pedestrian_utils.py
 src/dg_commons/sim/models/tires.py
 src/dg_commons/sim/models/utils.py
 src/dg_commons/sim/models/vehicle.py
 src/dg_commons/sim/models/vehicle_dynamic.py
 src/dg_commons/sim/models/vehicle_ligths.py
 src/dg_commons/sim/models/vehicle_structures.py
 src/dg_commons/sim/models/vehicle_utils.py
 src/dg_commons/sim/scenarios/__init__.py
 src/dg_commons/sim/scenarios/agent_from_commonroad.py
 src/dg_commons/sim/scenarios/factory.py
+src/dg_commons/sim/scenarios/structures.py
 src/dg_commons/sim/scenarios/utils.py
```


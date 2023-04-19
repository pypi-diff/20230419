# Comparing `tmp/rlcard-1.1.0.tar.gz` & `tmp/rlcard-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rlcard-1.1.0.tar", last modified: Fri Jan 13 21:25:22 2023, max compression
+gzip compressed data, was "dist/rlcard-1.2.0.tar", last modified: Wed Apr 19 16:43:47 2023, max compression
```

## Comparing `rlcard-1.1.0.tar` & `rlcard-1.2.0.tar`

### file list

```diff
@@ -1,197 +1,198 @@
-drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-01-13 21:25:22.510221 rlcard-1.1.0/
--rw-r--r--   0 songyihuang   (501) staff       (20)    21901 2023-01-13 21:25:22.509955 rlcard-1.1.0/PKG-INFO
--rw-r--r--   0 songyihuang   (501) staff       (20)    19200 2023-01-13 21:15:03.000000 rlcard-1.1.0/README.md
-drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-01-13 21:25:22.454905 rlcard-1.1.0/rlcard/
--rw-r--r--   0 songyihuang   (501) staff       (20)       68 2023-01-13 21:25:17.000000 rlcard-1.1.0/rlcard/__init__.py
-drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-01-13 21:25:22.457906 rlcard-1.1.0/rlcard/agents/
--rw-r--r--   0 songyihuang   (501) staff       (20)      955 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/__init__.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     7692 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/cfr_agent.py
-drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-01-13 21:25:22.459724 rlcard-1.1.0/rlcard/agents/dmc_agent/
--rw-r--r--   0 songyihuang   (501) staff       (20)       32 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/dmc_agent/__init__.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     6916 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/dmc_agent/file_writer.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     4823 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/dmc_agent/model.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     1549 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/dmc_agent/pettingzoo_model.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     4551 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/dmc_agent/pettingzoo_utils.py
--rw-r--r--   0 songyihuang   (501) staff       (20)    13606 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/dmc_agent/trainer.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     5681 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/dmc_agent/utils.py
--rw-r--r--   0 songyihuang   (501) staff       (20)    16224 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/dqn_agent.py
-drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-01-13 21:25:22.461201 rlcard-1.1.0/rlcard/agents/human_agents/
--rw-r--r--   0 songyihuang   (501) staff       (20)        0 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/human_agents/__init__.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     2391 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/human_agents/blackjack_human_agent.py
-drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-01-13 21:25:22.461643 rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/
--rw-r--r--   0 songyihuang   (501) staff       (20)        0 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/__init__.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     2305 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gin_rummy_human_agent.py
-drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-01-13 21:25:22.462091 rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_cards/
--rw-r--r--   0 songyihuang   (501) staff       (20)        0 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_cards/__init__.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     7581 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_cards/card_image.py
-drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-01-13 21:25:22.469951 rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/
--rw-r--r--   0 songyihuang   (501) staff       (20)        0 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/__init__.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     1846 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/canvas_item.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     2185 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/configurations.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     3603 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/env_thread.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     1250 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/game_app.py
--rw-r--r--   0 songyihuang   (501) staff       (20)    15888 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/game_canvas.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     2017 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/game_canvas_debug.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     9991 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/game_canvas_getter.py
--rw-r--r--   0 songyihuang   (501) staff       (20)    15591 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/game_canvas_post_doing_action.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     4462 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/game_canvas_query.py
--rw-r--r--   0 songyihuang   (501) staff       (20)    13965 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/game_canvas_updater.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     4110 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/game_frame.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     2804 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/handling_tap.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     3514 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/handling_tap_discard_pile.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     3292 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/handling_tap_held_pile.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     1041 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/handling_tap_player_pane.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     2654 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/handling_tap_stock_pile.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     3374 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/handling_tap_to_arrange_held_pile.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     4159 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/info_messaging.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     1519 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/menu_bar.py
--rw-r--r--   0 songyihuang   (501) staff       (20)      228 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/player_type.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     7565 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/preferences_window.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     6579 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/starting_new_game.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     6673 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/status_messaging.py
--rw-r--r--   0 songyihuang   (501) staff       (20)    11181 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/utils.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     2363 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/utils_extra.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     2671 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/human_agents/leduc_holdem_human_agent.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     2508 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/human_agents/limit_holdem_human_agent.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     2464 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/human_agents/nolimit_holdem_human_agent.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     2849 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/human_agents/uno_human_agent.py
--rw-r--r--   0 songyihuang   (501) staff       (20)    14852 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/nfsp_agent.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     1295 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/pettingzoo_agents.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     1593 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/agents/random_agent.py
-drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-01-13 21:25:22.473769 rlcard-1.1.0/rlcard/envs/
--rw-r--r--   0 songyihuang   (501) staff       (20)      927 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/envs/__init__.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     3195 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/envs/blackjack.py
--rw-r--r--   0 songyihuang   (501) staff       (20)    12028 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/envs/bridge.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     7475 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/envs/doudizhu.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     8525 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/envs/env.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     4334 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/envs/gin_rummy.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     3725 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/envs/leducholdem.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     3691 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/envs/limitholdem.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     4046 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/envs/mahjong.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     4040 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/envs/nolimitholdem.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     2685 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/envs/registration.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     2570 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/envs/uno.py
-drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-01-13 21:25:22.474247 rlcard-1.1.0/rlcard/games/
--rw-r--r--   0 songyihuang   (501) staff       (20)        0 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/__init__.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     1713 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/base.py
-drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-01-13 21:25:22.476364 rlcard-1.1.0/rlcard/games/blackjack/
--rw-r--r--   0 songyihuang   (501) staff       (20)      267 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/blackjack/__init__.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     1181 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/blackjack/dealer.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     7288 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/blackjack/game.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     2580 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/blackjack/judger.py
--rw-r--r--   0 songyihuang   (501) staff       (20)      442 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/blackjack/player.py
-drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-01-13 21:25:22.478940 rlcard-1.1.0/rlcard/games/bridge/
--rw-r--r--   0 songyihuang   (501) staff       (20)       56 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/bridge/__init__.py
--rw-r--r--   0 songyihuang   (501) staff       (20)      989 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/bridge/dealer.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     3257 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/bridge/game.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     3173 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/bridge/judger.py
--rw-r--r--   0 songyihuang   (501) staff       (20)      763 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/bridge/player.py
--rw-r--r--   0 songyihuang   (501) staff       (20)    11301 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/bridge/round.py
-drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-01-13 21:25:22.481144 rlcard-1.1.0/rlcard/games/bridge/utils/
--rw-r--r--   0 songyihuang   (501) staff       (20)        0 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/bridge/utils/__init__.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     4024 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/bridge/utils/action_event.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     1046 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/bridge/utils/bridge_card.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     2504 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/bridge/utils/move.py
--rw-r--r--   0 songyihuang   (501) staff       (20)      785 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/bridge/utils/tray.py
--rw-r--r--   0 songyihuang   (501) staff       (20)      369 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/bridge/utils/utils.py
-drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-01-13 21:25:22.486206 rlcard-1.1.0/rlcard/games/doudizhu/
--rw-r--r--   0 songyihuang   (501) staff       (20)      322 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/doudizhu/__init__.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     2557 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/doudizhu/dealer.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     5272 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/doudizhu/game.py
--rw-r--r--   0 songyihuang   (501) staff       (20)   225279 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/doudizhu/jsondata.zip
--rw-r--r--   0 songyihuang   (501) staff       (20)    14671 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/doudizhu/judger.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     4202 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/doudizhu/player.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     4492 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/doudizhu/round.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     8323 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/doudizhu/utils.py
-drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-01-13 21:25:22.488853 rlcard-1.1.0/rlcard/games/gin_rummy/
--rw-r--r--   0 songyihuang   (501) staff       (20)       61 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/gin_rummy/__init__.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     1049 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/gin_rummy/dealer.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     5581 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/gin_rummy/game.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     7278 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/gin_rummy/judge.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     5396 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/gin_rummy/player.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     9935 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/gin_rummy/round.py
-drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-01-13 21:25:22.491662 rlcard-1.1.0/rlcard/games/gin_rummy/utils/
--rw-r--r--   0 songyihuang   (501) staff       (20)        1 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/gin_rummy/utils/__init__.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     4304 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/gin_rummy/utils/action_event.py
--rw-r--r--   0 songyihuang   (501) staff       (20)      231 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/gin_rummy/utils/gin_rummy_error.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     5655 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/gin_rummy/utils/melding.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     4951 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/gin_rummy/utils/move.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     3114 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/gin_rummy/utils/scorers.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     8748 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/gin_rummy/utils/settings.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     2037 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/gin_rummy/utils/thinker.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     3232 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/gin_rummy/utils/utils.py
-drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-01-13 21:25:22.493737 rlcard-1.1.0/rlcard/games/leducholdem/
--rw-r--r--   0 songyihuang   (501) staff       (20)      352 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/leducholdem/__init__.py
--rw-r--r--   0 songyihuang   (501) staff       (20)       55 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/leducholdem/card2index.json
--rw-r--r--   0 songyihuang   (501) staff       (20)      407 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/leducholdem/dealer.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     6657 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/leducholdem/game.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     2122 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/leducholdem/judger.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     1142 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/leducholdem/player.py
--rw-r--r--   0 songyihuang   (501) staff       (20)      672 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/leducholdem/round.py
-drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-01-13 21:25:22.495804 rlcard-1.1.0/rlcard/games/limitholdem/
--rw-r--r--   0 songyihuang   (501) staff       (20)      409 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/limitholdem/__init__.py
--rw-r--r--   0 songyihuang   (501) staff       (20)      511 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/limitholdem/card2index.json
--rw-r--r--   0 songyihuang   (501) staff       (20)      482 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/limitholdem/dealer.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     8157 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/limitholdem/game.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     4761 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/limitholdem/judger.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     1192 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/limitholdem/player.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     4360 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/limitholdem/round.py
--rw-r--r--   0 songyihuang   (501) staff       (20)    22693 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/limitholdem/utils.py
-drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-01-13 21:25:22.498077 rlcard-1.1.0/rlcard/games/mahjong/
--rw-r--r--   0 songyihuang   (501) staff       (20)      370 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/mahjong/__init__.py
--rw-r--r--   0 songyihuang   (501) staff       (20)      815 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/mahjong/card.py
--rw-r--r--   0 songyihuang   (501) staff       (20)      850 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/mahjong/dealer.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     4567 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/mahjong/game.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     9338 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/mahjong/judger.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     1983 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/mahjong/player.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     4630 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/mahjong/round.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     2166 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/mahjong/utils.py
-drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-01-13 21:25:22.499922 rlcard-1.1.0/rlcard/games/nolimitholdem/
--rw-r--r--   0 songyihuang   (501) staff       (20)      424 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/nolimitholdem/__init__.py
--rw-r--r--   0 songyihuang   (501) staff       (20)       90 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/nolimitholdem/dealer.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     8999 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/nolimitholdem/game.py
--rw-r--r--   0 songyihuang   (501) staff       (20)       90 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/nolimitholdem/judger.py
--rw-r--r--   0 songyihuang   (501) staff       (20)      603 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/nolimitholdem/player.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     5758 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/nolimitholdem/round.py
-drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-01-13 21:25:22.502456 rlcard-1.1.0/rlcard/games/uno/
--rw-r--r--   0 songyihuang   (501) staff       (20)      272 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/uno/__init__.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     2299 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/uno/card.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     1040 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/uno/dealer.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     4618 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/uno/game.py
-drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-01-13 21:25:22.502723 rlcard-1.1.0/rlcard/games/uno/jsondata/
--rw-r--r--   0 songyihuang   (501) staff       (20)      770 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/uno/jsondata/action_space.json
--rw-r--r--   0 songyihuang   (501) staff       (20)      521 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/uno/judger.py
--rw-r--r--   0 songyihuang   (501) staff       (20)      404 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/uno/player.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     8139 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/uno/round.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     3483 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/games/uno/utils.py
-drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-01-13 21:25:22.506470 rlcard-1.1.0/rlcard/models/
--rw-r--r--   0 songyihuang   (501) staff       (20)      971 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/models/__init__.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     1681 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/models/bridge_rule_models.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     6313 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/models/doudizhu_rule_models.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     5072 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/models/gin_rummy_rule_models.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     3919 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/models/leducholdem_rule_models.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     6315 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/models/limitholdem_rule_models.py
--rw-r--r--   0 songyihuang   (501) staff       (20)      462 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/models/model.py
-drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-01-13 21:25:22.453680 rlcard-1.1.0/rlcard/models/pretrained/
-drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-01-13 21:25:22.507717 rlcard-1.1.0/rlcard/models/pretrained/leduc_holdem_cfr/
--rw-r--r--   0 songyihuang   (501) staff       (20)    31694 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/models/pretrained/leduc_holdem_cfr/average_policy.pkl
--rw-r--r--   0 songyihuang   (501) staff       (20)        5 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/models/pretrained/leduc_holdem_cfr/iteration.pkl
--rw-r--r--   0 songyihuang   (501) staff       (20)    31696 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/models/pretrained/leduc_holdem_cfr/policy.pkl
--rw-r--r--   0 songyihuang   (501) staff       (20)    31694 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/models/pretrained/leduc_holdem_cfr/regrets.pkl
--rw-r--r--   0 songyihuang   (501) staff       (20)      906 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/models/pretrained_models.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     2134 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/models/registration.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     3204 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/models/uno_rule_models.py
-drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-01-13 21:25:22.509324 rlcard-1.1.0/rlcard/utils/
--rw-r--r--   0 songyihuang   (501) staff       (20)      149 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/utils/__init__.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     1949 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/utils/logger.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     2473 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/utils/pettingzoo_utils.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     4721 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/utils/seeding.py
--rw-r--r--   0 songyihuang   (501) staff       (20)     7617 2023-01-13 21:15:03.000000 rlcard-1.1.0/rlcard/utils/utils.py
-drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-01-13 21:25:22.456390 rlcard-1.1.0/rlcard.egg-info/
--rw-r--r--   0 songyihuang   (501) staff       (20)    21901 2023-01-13 21:25:22.000000 rlcard-1.1.0/rlcard.egg-info/PKG-INFO
--rw-r--r--   0 songyihuang   (501) staff       (20)     7036 2023-01-13 21:25:22.000000 rlcard-1.1.0/rlcard.egg-info/SOURCES.txt
--rw-r--r--   0 songyihuang   (501) staff       (20)        1 2023-01-13 21:25:22.000000 rlcard-1.1.0/rlcard.egg-info/dependency_links.txt
--rw-r--r--   0 songyihuang   (501) staff       (20)       67 2023-01-13 21:25:22.000000 rlcard-1.1.0/rlcard.egg-info/requires.txt
--rw-r--r--   0 songyihuang   (501) staff       (20)        7 2023-01-13 21:25:22.000000 rlcard-1.1.0/rlcard.egg-info/top_level.txt
--rw-r--r--   0 songyihuang   (501) staff       (20)       38 2023-01-13 21:25:22.510319 rlcard-1.1.0/setup.cfg
--rw-r--r--   0 songyihuang   (501) staff       (20)     1781 2023-01-13 21:15:03.000000 rlcard-1.1.0/setup.py
+drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-04-19 16:43:47.693724 rlcard-1.2.0/
+-rw-r--r--   0 songyihuang   (501) staff       (20)     1075 2023-04-19 16:33:04.000000 rlcard-1.2.0/LICENSE.md
+-rw-r--r--   0 songyihuang   (501) staff       (20)    24279 2023-04-19 16:43:47.693436 rlcard-1.2.0/PKG-INFO
+-rw-r--r--   0 songyihuang   (501) staff       (20)    23558 2023-04-19 16:33:04.000000 rlcard-1.2.0/README.md
+drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-04-19 16:43:47.635734 rlcard-1.2.0/rlcard/
+-rw-r--r--   0 songyihuang   (501) staff       (20)       68 2023-04-19 16:33:56.000000 rlcard-1.2.0/rlcard/__init__.py
+drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-04-19 16:43:47.639075 rlcard-1.2.0/rlcard/agents/
+-rw-r--r--   0 songyihuang   (501) staff       (20)      955 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/__init__.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     7692 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/cfr_agent.py
+drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-04-19 16:43:47.641118 rlcard-1.2.0/rlcard/agents/dmc_agent/
+-rw-r--r--   0 songyihuang   (501) staff       (20)       32 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/dmc_agent/__init__.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     6916 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/dmc_agent/file_writer.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     4823 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/dmc_agent/model.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     1549 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/dmc_agent/pettingzoo_model.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     4551 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/dmc_agent/pettingzoo_utils.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)    13606 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/dmc_agent/trainer.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     5681 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/dmc_agent/utils.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)    21493 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/dqn_agent.py
+drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-04-19 16:43:47.642779 rlcard-1.2.0/rlcard/agents/human_agents/
+-rw-r--r--   0 songyihuang   (501) staff       (20)        0 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/human_agents/__init__.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     2391 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/human_agents/blackjack_human_agent.py
+drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-04-19 16:43:47.643295 rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/
+-rw-r--r--   0 songyihuang   (501) staff       (20)        0 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/__init__.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     2305 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gin_rummy_human_agent.py
+drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-04-19 16:43:47.643842 rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_cards/
+-rw-r--r--   0 songyihuang   (501) staff       (20)        0 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_cards/__init__.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     7581 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_cards/card_image.py
+drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-04-19 16:43:47.652461 rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/
+-rw-r--r--   0 songyihuang   (501) staff       (20)        0 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/__init__.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     1846 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/canvas_item.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     2185 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/configurations.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     3603 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/env_thread.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     1250 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/game_app.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)    15888 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/game_canvas.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     2017 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/game_canvas_debug.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     9991 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/game_canvas_getter.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)    15591 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/game_canvas_post_doing_action.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     4462 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/game_canvas_query.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)    13965 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/game_canvas_updater.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     4110 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/game_frame.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     2804 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/handling_tap.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     3514 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/handling_tap_discard_pile.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     3292 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/handling_tap_held_pile.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     1041 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/handling_tap_player_pane.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     2654 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/handling_tap_stock_pile.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     3374 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/handling_tap_to_arrange_held_pile.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     4159 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/info_messaging.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     1519 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/menu_bar.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)      233 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/player_type.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     7565 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/preferences_window.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     6579 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/starting_new_game.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     6673 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/status_messaging.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)    11181 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/utils.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     2363 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/utils_extra.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     2671 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/human_agents/leduc_holdem_human_agent.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     2508 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/human_agents/limit_holdem_human_agent.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     2464 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/human_agents/nolimit_holdem_human_agent.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     2849 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/human_agents/uno_human_agent.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)    20071 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/nfsp_agent.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     1295 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/pettingzoo_agents.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     1593 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/agents/random_agent.py
+drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-04-19 16:43:47.657764 rlcard-1.2.0/rlcard/envs/
+-rw-r--r--   0 songyihuang   (501) staff       (20)      927 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/envs/__init__.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     3195 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/envs/blackjack.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)    12028 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/envs/bridge.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     7475 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/envs/doudizhu.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     8525 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/envs/env.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     4334 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/envs/gin_rummy.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     3725 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/envs/leducholdem.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     3691 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/envs/limitholdem.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     4046 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/envs/mahjong.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     4040 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/envs/nolimitholdem.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     2685 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/envs/registration.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     2570 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/envs/uno.py
+drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-04-19 16:43:47.658564 rlcard-1.2.0/rlcard/games/
+-rw-r--r--   0 songyihuang   (501) staff       (20)        0 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/__init__.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     1713 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/base.py
+drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-04-19 16:43:47.660815 rlcard-1.2.0/rlcard/games/blackjack/
+-rw-r--r--   0 songyihuang   (501) staff       (20)      267 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/blackjack/__init__.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     1181 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/blackjack/dealer.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     7288 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/blackjack/game.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     2580 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/blackjack/judger.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)      442 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/blackjack/player.py
+drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-04-19 16:43:47.663871 rlcard-1.2.0/rlcard/games/bridge/
+-rw-r--r--   0 songyihuang   (501) staff       (20)       56 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/bridge/__init__.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)      989 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/bridge/dealer.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     3257 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/bridge/game.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     3173 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/bridge/judger.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)      763 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/bridge/player.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)    11301 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/bridge/round.py
+drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-04-19 16:43:47.667032 rlcard-1.2.0/rlcard/games/bridge/utils/
+-rw-r--r--   0 songyihuang   (501) staff       (20)        0 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/bridge/utils/__init__.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     4024 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/bridge/utils/action_event.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     1046 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/bridge/utils/bridge_card.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     2504 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/bridge/utils/move.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)      785 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/bridge/utils/tray.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)      369 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/bridge/utils/utils.py
+drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-04-19 16:43:47.670851 rlcard-1.2.0/rlcard/games/doudizhu/
+-rw-r--r--   0 songyihuang   (501) staff       (20)      322 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/doudizhu/__init__.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     2557 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/doudizhu/dealer.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     5272 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/doudizhu/game.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)   225279 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/doudizhu/jsondata.zip
+-rw-r--r--   0 songyihuang   (501) staff       (20)    14671 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/doudizhu/judger.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     4202 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/doudizhu/player.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     4492 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/doudizhu/round.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     8323 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/doudizhu/utils.py
+drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-04-19 16:43:47.673039 rlcard-1.2.0/rlcard/games/gin_rummy/
+-rw-r--r--   0 songyihuang   (501) staff       (20)       61 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/gin_rummy/__init__.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     1049 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/gin_rummy/dealer.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     5597 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/gin_rummy/game.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     7278 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/gin_rummy/judge.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     5396 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/gin_rummy/player.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     9935 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/gin_rummy/round.py
+drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-04-19 16:43:47.675627 rlcard-1.2.0/rlcard/games/gin_rummy/utils/
+-rw-r--r--   0 songyihuang   (501) staff       (20)        1 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/gin_rummy/utils/__init__.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     4304 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/gin_rummy/utils/action_event.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)      231 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/gin_rummy/utils/gin_rummy_error.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     5655 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/gin_rummy/utils/melding.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     4951 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/gin_rummy/utils/move.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     3114 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/gin_rummy/utils/scorers.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     8758 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/gin_rummy/utils/settings.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     2037 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/gin_rummy/utils/thinker.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     3232 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/gin_rummy/utils/utils.py
+drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-04-19 16:43:47.677651 rlcard-1.2.0/rlcard/games/leducholdem/
+-rw-r--r--   0 songyihuang   (501) staff       (20)      352 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/leducholdem/__init__.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)       55 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/leducholdem/card2index.json
+-rw-r--r--   0 songyihuang   (501) staff       (20)      407 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/leducholdem/dealer.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     6657 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/leducholdem/game.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     2122 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/leducholdem/judger.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     1142 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/leducholdem/player.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)      672 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/leducholdem/round.py
+drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-04-19 16:43:47.679880 rlcard-1.2.0/rlcard/games/limitholdem/
+-rw-r--r--   0 songyihuang   (501) staff       (20)      409 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/limitholdem/__init__.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)      511 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/limitholdem/card2index.json
+-rw-r--r--   0 songyihuang   (501) staff       (20)      482 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/limitholdem/dealer.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     8157 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/limitholdem/game.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     4761 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/limitholdem/judger.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     1192 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/limitholdem/player.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     4360 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/limitholdem/round.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)    22693 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/limitholdem/utils.py
+drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-04-19 16:43:47.682851 rlcard-1.2.0/rlcard/games/mahjong/
+-rw-r--r--   0 songyihuang   (501) staff       (20)      370 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/mahjong/__init__.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)      815 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/mahjong/card.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)      850 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/mahjong/dealer.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     4567 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/mahjong/game.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     9338 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/mahjong/judger.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     1983 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/mahjong/player.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     4630 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/mahjong/round.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     2166 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/mahjong/utils.py
+drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-04-19 16:43:47.684757 rlcard-1.2.0/rlcard/games/nolimitholdem/
+-rw-r--r--   0 songyihuang   (501) staff       (20)      424 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/nolimitholdem/__init__.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)       90 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/nolimitholdem/dealer.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     8999 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/nolimitholdem/game.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)       90 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/nolimitholdem/judger.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)      603 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/nolimitholdem/player.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     5758 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/nolimitholdem/round.py
+drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-04-19 16:43:47.687131 rlcard-1.2.0/rlcard/games/uno/
+-rw-r--r--   0 songyihuang   (501) staff       (20)      272 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/uno/__init__.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     2299 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/uno/card.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     1040 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/uno/dealer.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     4618 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/uno/game.py
+drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-04-19 16:43:47.687428 rlcard-1.2.0/rlcard/games/uno/jsondata/
+-rw-r--r--   0 songyihuang   (501) staff       (20)      770 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/uno/jsondata/action_space.json
+-rw-r--r--   0 songyihuang   (501) staff       (20)      521 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/uno/judger.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)      404 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/uno/player.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     8228 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/uno/round.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     3483 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/games/uno/utils.py
+drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-04-19 16:43:47.690282 rlcard-1.2.0/rlcard/models/
+-rw-r--r--   0 songyihuang   (501) staff       (20)      971 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/models/__init__.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     1681 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/models/bridge_rule_models.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     6313 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/models/doudizhu_rule_models.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     5072 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/models/gin_rummy_rule_models.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     3919 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/models/leducholdem_rule_models.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     6315 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/models/limitholdem_rule_models.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)      462 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/models/model.py
+drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-04-19 16:43:47.634358 rlcard-1.2.0/rlcard/models/pretrained/
+drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-04-19 16:43:47.691521 rlcard-1.2.0/rlcard/models/pretrained/leduc_holdem_cfr/
+-rw-r--r--   0 songyihuang   (501) staff       (20)    31694 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/models/pretrained/leduc_holdem_cfr/average_policy.pkl
+-rw-r--r--   0 songyihuang   (501) staff       (20)        5 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/models/pretrained/leduc_holdem_cfr/iteration.pkl
+-rw-r--r--   0 songyihuang   (501) staff       (20)    31696 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/models/pretrained/leduc_holdem_cfr/policy.pkl
+-rw-r--r--   0 songyihuang   (501) staff       (20)    31694 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/models/pretrained/leduc_holdem_cfr/regrets.pkl
+-rw-r--r--   0 songyihuang   (501) staff       (20)      906 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/models/pretrained_models.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     2134 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/models/registration.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     3204 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/models/uno_rule_models.py
+drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-04-19 16:43:47.692975 rlcard-1.2.0/rlcard/utils/
+-rw-r--r--   0 songyihuang   (501) staff       (20)      149 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/utils/__init__.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     1949 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/utils/logger.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     2476 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/utils/pettingzoo_utils.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     4721 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/utils/seeding.py
+-rw-r--r--   0 songyihuang   (501) staff       (20)     7617 2023-04-19 16:33:04.000000 rlcard-1.2.0/rlcard/utils/utils.py
+drwxr-xr-x   0 songyihuang   (501) staff       (20)        0 2023-04-19 16:43:47.637236 rlcard-1.2.0/rlcard.egg-info/
+-rw-r--r--   0 songyihuang   (501) staff       (20)    24279 2023-04-19 16:43:47.000000 rlcard-1.2.0/rlcard.egg-info/PKG-INFO
+-rw-r--r--   0 songyihuang   (501) staff       (20)     7047 2023-04-19 16:43:47.000000 rlcard-1.2.0/rlcard.egg-info/SOURCES.txt
+-rw-r--r--   0 songyihuang   (501) staff       (20)        1 2023-04-19 16:43:47.000000 rlcard-1.2.0/rlcard.egg-info/dependency_links.txt
+-rw-r--r--   0 songyihuang   (501) staff       (20)       67 2023-04-19 16:43:47.000000 rlcard-1.2.0/rlcard.egg-info/requires.txt
+-rw-r--r--   0 songyihuang   (501) staff       (20)        7 2023-04-19 16:43:47.000000 rlcard-1.2.0/rlcard.egg-info/top_level.txt
+-rw-r--r--   0 songyihuang   (501) staff       (20)       38 2023-04-19 16:43:47.693814 rlcard-1.2.0/setup.cfg
+-rw-r--r--   0 songyihuang   (501) staff       (20)     1831 2023-04-19 16:33:04.000000 rlcard-1.2.0/setup.py
```

### Comparing `rlcard-1.1.0/PKG-INFO` & `rlcard-1.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,270 +1,310 @@
 Metadata-Version: 2.1
 Name: rlcard
-Version: 1.1.0
+Version: 1.2.0
 Summary: A Toolkit for Reinforcement Learning in Card Games
 Home-page: https://github.com/datamllab/rlcard
 Author: Data Analytics at Texas A&M (DATA) Lab
 Author-email: daochen.zha@tamu.edu
-License: UNKNOWN
-Description: # RLCard: A Toolkit for Reinforcement Learning in Card Games
-        <img width="500" src="https://dczha.com/files/rlcard/logo.jpg" alt="Logo" />
-        
-        [![Testing](https://github.com/datamllab/rlcard/actions/workflows/python-package.yml/badge.svg)](https://github.com/datamllab/rlcard/actions/workflows/python-package.yml)
-        [![PyPI version](https://badge.fury.io/py/rlcard.svg)](https://badge.fury.io/py/rlcard)
-        [![Coverage Status](https://coveralls.io/repos/github/datamllab/rlcard/badge.svg)](https://coveralls.io/github/datamllab/rlcard?branch=master)
-        [![Downloads](https://pepy.tech/badge/rlcard)](https://pepy.tech/project/rlcard)
-        [![Downloads](https://pepy.tech/badge/rlcard/month)](https://pepy.tech/project/rlcard)
-        [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-        
-        [中文文档](README.zh-CN.md)
-        
-        RLCard is a toolkit for Reinforcement Learning (RL) in card games. It supports multiple card environments with easy-to-use interfaces for implementing various reinforcement learning and searching algorithms. The goal of RLCard is to bridge reinforcement learning and imperfect information games. RLCard is developed by [DATA Lab](http://faculty.cs.tamu.edu/xiahu/) at Rice and Texas A&M University, and community contributors.
-        
-        *   Official Website: [https://www.rlcard.org](https://www.rlcard.org)
-        *   Tutorial in Jupyter Notebook: [https://github.com/datamllab/rlcard-tutorial](https://github.com/datamllab/rlcard-tutorial)
-        *   Paper: [https://arxiv.org/abs/1910.04376](https://arxiv.org/abs/1910.04376)
-        *   GUI: [RLCard-Showdown](https://github.com/datamllab/rlcard-showdown)
-        *   Dou Dizhu Demo: [Demo](https://douzero.org/)
-        *   Resources: [Awesome-Game-AI](https://github.com/datamllab/awesome-game-ai)
-        *   Related Project: [DouZero Project](https://github.com/kwai/DouZero)
-        *   Zhihu: https://zhuanlan.zhihu.com/p/526723604
-        
-        **Community:**
-        *  **Slack**: Discuss in our [#rlcard-project](https://join.slack.com/t/rlcard/shared_invite/zt-rkvktsaq-xkMwz8BfKupCM6zGhO01xg) slack channel.
-        *  **QQ Group**: Join our QQ group to discuss. Password: rlcardqqgroup
-        	*  Group 1: 665647450
-        	*  Group 2: 117349516
-        
-        **News:**
-        *   We have updated the tutorials in Jupyter Notebook to help you walk through RLCard! Please check [RLCard Tutorial](https://github.com/datamllab/rlcard-tutorial).
-        *   All the algorithms can suppport [PettingZoo](https://github.com/PettingZoo-Team/PettingZoo) now. Please check [here](examples/pettingzoo). Thanks the contribtuion from [Yifei Cheng](https://github.com/ycheng517).
-        *   Please follow [DouZero](https://github.com/kwai/DouZero), a strong Dou Dizhu AI and the [ICML 2021 paper](https://arxiv.org/abs/2106.06135). An online demo is available [here](https://douzero.org/). The algorithm is also integrated in RLCard. See [Training DMC on Dou Dizhu](docs/toy-examples.md#training-dmc-on-dou-dizhu).
-        *   Our package is used in [PettingZoo](https://github.com/PettingZoo-Team/PettingZoo). Please check it out!
-        *   We have released RLCard-Showdown, GUI demo for RLCard. Please check out [here](https://github.com/datamllab/rlcard-showdown)!
-        *   Jupyter Notebook tutorial available! We add some examples in R to call Python interfaces of RLCard with reticulate. See [here](docs/toy-examples-r.md)
-        *   Thanks for the contribution of [@Clarit7](https://github.com/Clarit7) for supporting different number of players in Blackjack. We call for contributions for gradually making the games more configurable. See [here](CONTRIBUTING.md#making-configurable-environments) for more details.
-        *   Thanks for the contribution of [@Clarit7](https://github.com/Clarit7) for the Blackjack and Limit Hold'em human interface.
-        *   Now RLCard supports environment local seeding and multiprocessing. Thanks for the testing scripts provided by [@weepingwillowben](https://github.com/weepingwillowben).
-        *   Human interface of NoLimit Holdem available. The action space of NoLimit Holdem has been abstracted. Thanks for the contribution of [@AdrianP-](https://github.com/AdrianP-).
-        *   New game Gin Rummy and human GUI available. Thanks for the contribution of [@billh0420](https://github.com/billh0420).
-        *   PyTorch implementation available. Thanks for the contribution of [@mjudell](https://github.com/mjudell).
-        
-        ## Cite this work
-        If you find this repo useful, you may cite:
-        
-        Zha, Daochen, et al. "RLCard: A Platform for Reinforcement Learning in Card Games." IJCAI. 2020.
-        ```bibtex
-        @inproceedings{zha2020rlcard,
-          title={RLCard: A Platform for Reinforcement Learning in Card Games},
-          author={Zha, Daochen and Lai, Kwei-Herng and Huang, Songyi and Cao, Yuanpu and Reddy, Keerthana and Vargas, Juan and Nguyen, Alex and Wei, Ruzhe and Guo, Junyu and Hu, Xia},
-          booktitle={IJCAI},
-          year={2020}
-        }
-        ```
-        
-        ## Installation
-        Make sure that you have **Python 3.6+** and **pip** installed. We recommend installing the stable version of `rlcard` with `pip`:
-        
-        ```
-        pip3 install rlcard
-        ```
-        The default installation will only include the card environments. To use PyTorch implementation of the training algorithms, run
-        ```
-        pip3 install rlcard[torch]
-        ```
-        If you are in China and the above command is too slow, you can use the mirror provided by Tsinghua University:
-        ```
-        pip3 install rlcard -i https://pypi.tuna.tsinghua.edu.cn/simple
-        ```
-        Alternatively, you can clone the latest version with (if you are in China and Github is slow, you can use the mirror in [Gitee](https://gitee.com/daochenzha/rlcard)):
-        ```
-        git clone https://github.com/datamllab/rlcard.git
-        ```
-        or only clone one branch to make it faster:
-        ```
-        git clone -b master --single-branch --depth=1 https://github.com/datamllab/rlcard.git
-        ```
-        Then install with
-        ```
-        cd rlcard
-        pip3 install -e .
-        pip3 install -e .[torch]
-        ```
-        
-        We also provide [**conda** installation method](https://anaconda.org/toubun/rlcard):
-        
-        ```
-        conda install -c toubun rlcard
-        ```
-        
-        Conda installation only provides the card environments, you need to manually install Pytorch on your demands.
-        
-        ## Examples
-        A **short example** is as below.
-        
-        ```python
-        import rlcard
-        from rlcard.agents import RandomAgent
-        
-        env = rlcard.make('blackjack')
-        env.set_agents([RandomAgent(num_actions=env.num_actions)])
-        
-        print(env.num_actions) # 2
-        print(env.num_players) # 1
-        print(env.state_shape) # [[2]]
-        print(env.action_shape) # [None]
-        
-        trajectories, payoffs = env.run()
-        ```
-        
-        RLCard can be flexibly connected to various algorithms. See the following examples:
-        
-        *   [Playing with random agents](docs/toy-examples.md#playing-with-random-agents)
-        *   [Deep-Q learning on Blackjack](docs/toy-examples.md#deep-q-learning-on-blackjack)
-        *   [Training CFR (chance sampling) on Leduc Hold'em](docs/toy-examples.md#training-cfr-on-leduc-holdem)
-        *   [Having fun with pretrained Leduc model](docs/toy-examples.md#having-fun-with-pretrained-leduc-model)
-        *   [Training DMC on Dou Dizhu](docs/toy-examples.md#training-dmc-on-dou-dizhu)
-        *   [Evaluating Agents](docs/toy-examples.md#evaluating-agents)
-        *   [Training Agents on PettingZoo](examples/pettingzoo)
-        
-        ## Demo
-        Run `examples/human/leduc_holdem_human.py` to play with the pre-trained Leduc Hold'em model. Leduc Hold'em is a simplified version of Texas Hold'em. Rules can be found [here](docs/games.md#leduc-holdem).
-        
-        ```
-        >> Leduc Hold'em pre-trained model
-        
-        >> Start a new game!
-        >> Agent 1 chooses raise
-        
-        =============== Community Card ===============
-        ┌─────────┐
-        │░░░░░░░░░│
-        │░░░░░░░░░│
-        │░░░░░░░░░│
-        │░░░░░░░░░│
-        │░░░░░░░░░│
-        │░░░░░░░░░│
-        │░░░░░░░░░│
-        └─────────┘
-        ===============   Your Hand    ===============
-        ┌─────────┐
-        │J        │
-        │         │
-        │         │
-        │    ♥    │
-        │         │
-        │         │
-        │        J│
-        └─────────┘
-        ===============     Chips      ===============
-        Yours:   +
-        Agent 1: +++
-        =========== Actions You Can Choose ===========
-        0: call, 1: raise, 2: fold
-        
-        >> You choose action (integer):
-        ```
-        We also provide a GUI for easy debugging. Please check [here](https://github.com/datamllab/rlcard-showdown/). Some demos:
-        
-        ![doudizhu-replay](https://github.com/datamllab/rlcard-showdown/blob/master/docs/imgs/doudizhu-replay.png?raw=true)
-        ![leduc-replay](https://github.com/datamllab/rlcard-showdown/blob/master/docs/imgs/leduc-replay.png?raw=true)
-        
-        ## Available Environments
-        We provide a complexity estimation for the games on several aspects. **InfoSet Number:** the number of information sets; **InfoSet Size:** the average number of states in a single information set; **Action Size:** the size of the action space. **Name:** the name that should be passed to `rlcard.make` to create the game environment. We also provide the link to the documentation and the random example.
-        
-        | Game                                                                                                                                                                                           | InfoSet Number  | InfoSet Size      | Action Size | Name            | Usage                                                                                       |
-        | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :-------------: | :---------------: | :---------: | :-------------: | :-----------------------------------------------------------------------------------------: |
-        | Blackjack ([wiki](https://en.wikipedia.org/wiki/Blackjack), [baike](https://baike.baidu.com/item/21%E7%82%B9/5481683?fr=aladdin))                                                              | 10^3            | 10^1              | 10^0        | blackjack       | [doc](docs/games.md#blackjack), [example](examples/run_random.py)                           |
-        | Leduc Hold’em ([paper](http://poker.cs.ualberta.ca/publications/UAI05.pdf))                                                                                                                    | 10^2            | 10^2              | 10^0        | leduc-holdem    | [doc](docs/games.md#leduc-holdem), [example](examples/run_random.py)                        |
-        | Limit Texas Hold'em ([wiki](https://en.wikipedia.org/wiki/Texas_hold_%27em), [baike](https://baike.baidu.com/item/%E5%BE%B7%E5%85%8B%E8%90%A8%E6%96%AF%E6%89%91%E5%85%8B/83440?fr=aladdin))    | 10^14           | 10^3              | 10^0        | limit-holdem    | [doc](docs/games.md#limit-texas-holdem), [example](examples/run_random.py)                  |
-        | Dou Dizhu ([wiki](https://en.wikipedia.org/wiki/Dou_dizhu), [baike](https://baike.baidu.com/item/%E6%96%97%E5%9C%B0%E4%B8%BB/177997?fr=aladdin))                                               | 10^53 ~ 10^83   | 10^23             | 10^4        | doudizhu        | [doc](docs/games.md#dou-dizhu), [example](examples/run_random.py)                           |
-        | Mahjong ([wiki](https://en.wikipedia.org/wiki/Competition_Mahjong_scoring_rules), [baike](https://baike.baidu.com/item/%E9%BA%BB%E5%B0%86/215))                                                | 10^121          | 10^48             | 10^2        | mahjong         | [doc](docs/games.md#mahjong), [example](examples/run_random.py)                             | 
-        | No-limit Texas Hold'em ([wiki](https://en.wikipedia.org/wiki/Texas_hold_%27em), [baike](https://baike.baidu.com/item/%E5%BE%B7%E5%85%8B%E8%90%A8%E6%96%AF%E6%89%91%E5%85%8B/83440?fr=aladdin)) | 10^162          | 10^3              | 10^4        | no-limit-holdem | [doc](docs/games.md#no-limit-texas-holdem), [example](examples/run_random.py)               |
-        | UNO ([wiki](https://en.wikipedia.org/wiki/Uno_\(card_game\)), [baike](https://baike.baidu.com/item/UNO%E7%89%8C/2249587))                                                                      |  10^163         | 10^10             | 10^1        | uno             | [doc](docs/games.md#uno), [example](examples/run_random.py)                                 |
-        | Gin Rummy ([wiki](https://en.wikipedia.org/wiki/Gin_rummy), [baike](https://baike.baidu.com/item/%E9%87%91%E6%8B%89%E7%B1%B3/3471710))                                                         | 10^52           | -                 | -           | gin-rummy       | [doc](docs/games.md#gin-rummy), [example](examples/run_random.py)                           |
-        | Bridge ([wiki](https://en.wikipedia.org/wiki/Bridge), [baike](https://baike.baidu.com/item/%E6%A1%A5%E7%89%8C/332030))                                                                         |                 | -                 | -           | bridge          | [doc](docs/games.md#bridge), [example](examples/run_random.py)                              |
-        
-        ## Supported Algorithms
-        | Algorithm | example | reference |
-        | :--------------------------------------: | :-----------------------------------------: | :------------------------------------------------------------------------------------------------------: |
-        | Deep Monte-Carlo (DMC)                   | [examples/run\_dmc.py](examples/run_dmc.py) | [[paper]](https://arxiv.org/abs/2106.06135)                                                              |
-        | Deep Q-Learning (DQN)                    | [examples/run\_rl.py](examples/run_rl.py)   | [[paper]](https://arxiv.org/abs/1312.5602)                                                               |
-        | Neural Fictitious Self-Play (NFSP)       | [examples/run\_rl.py](examples/run_rl.py)   | [[paper]](https://arxiv.org/abs/1603.01121)                                                              |
-        | Counterfactual Regret Minimization (CFR) | [examples/run\_cfr.py](examples/run_cfr.py) | [[paper]](http://papers.nips.cc/paper/3306-regret-minimization-in-games-with-incomplete-information.pdf) |
-        
-        ## Pre-trained and Rule-based Models
-        We provide a [model zoo](rlcard/models) to serve as the baselines.
-        
-        | Model                                    | Explanation                                              |
-        | :--------------------------------------: | :------------------------------------------------------: |
-        | leduc-holdem-cfr                         | Pre-trained CFR (chance sampling) model on Leduc Hold'em |
-        | leduc-holdem-rule-v1                     | Rule-based model for Leduc Hold'em, v1                   |
-        | leduc-holdem-rule-v2                     | Rule-based model for Leduc Hold'em, v2                   |
-        | uno-rule-v1                              | Rule-based model for UNO, v1                             |
-        | limit-holdem-rule-v1                     | Rule-based model for Limit Texas Hold'em, v1             |
-        | doudizhu-rule-v1                         | Rule-based model for Dou Dizhu, v1                       |
-        | gin-rummy-novice-rule                    | Gin Rummy novice rule model                              |
-        
-        ## API Cheat Sheet
-        ### How to create an environment
-        You can use the the following interface to make an environment. You may optionally specify some configurations with a dictionary.
-        *   **env = rlcard.make(env_id, config={})**: Make an environment. `env_id` is a string of a environment; `config` is a dictionary that specifies some environment configurations, which are as follows.
-        	*   `seed`: Default `None`. Set a environment local random seed for reproducing the results.
-        	*   `allow_step_back`: Default `False`. `True` if allowing `step_back` function to traverse backward in the tree.
-        	*   Game specific configurations: These fields start with `game_`. Currently, we only support `game_num_players` in Blackjack, .
-        
-        Once the environemnt is made, we can access some information of the game.
-        *   **env.num_actions**: The number of actions.
-        *   **env.num_players**: The number of players.
-        *   **env.state_shape**: The shape of the state space of the observations.
-        *   **env.action_shape**: The shape of the action features (Dou Dizhu's action can encoded as features)
-        
-        ### What is state in RLCard
-        State is a Python dictionary. It consists of observation `state['obs']`, legal actions `state['legal_actions']`, raw observation `state['raw_obs']` and raw legal actions `state['raw_legal_actions']`.
-        
-        ### Basic interfaces
-        The following interfaces provide a basic usage. It is easy to use but it has assumtions on the agent. The agent must follow [agent template](docs/developping-algorithms.md). 
-        *   **env.set_agents(agents)**: `agents` is a list of `Agent` object. The length of the list should be equal to the number of the players in the game.
-        *   **env.run(is_training=False)**: Run a complete game and return trajectories and payoffs. The function can be used after the `set_agents` is called. If `is_training` is `True`, it will use `step` function in the agent to play the game. If `is_training` is `False`, `eval_step` will be called instead.
-        
-        ### Advanced interfaces
-        For advanced usage, the following interfaces allow flexible operations on the game tree. These interfaces do not make any assumtions on the agent.
-        *   **env.reset()**: Initialize a game. Return the state and the first player ID.
-        *   **env.step(action, raw_action=False)**: Take one step in the environment. `action` can be raw action or integer; `raw_action` should be `True` if the action is raw action (string).
-        *   **env.step_back()**: Available only when `allow_step_back` is `True`. Take one step backward. This can be used for algorithms that operate on the game tree, such as CFR (chance sampling).
-        *   **env.is_over()**: Return `True` if the current game is over. Otherewise, return `False`.
-        *   **env.get_player_id()**: Return the Player ID of the current player.
-        *   **env.get_state(player_id)**: Return the state that corresponds to `player_id`.
-        *   **env.get_payoffs()**: In the end of the game, return a list of payoffs for all the players.
-        *   **env.get_perfect_information()**: (Currently only support some of the games) Obtain the perfect information at the current state.
-        
-        ## Library Structure
-        The purposes of the main modules are listed as below:
-        
-        *   [/examples](examples): Examples of using RLCard.
-        *   [/docs](docs): Documentation of RLCard.
-        *   [/tests](tests): Testing scripts for RLCard.
-        *   [/rlcard/agents](rlcard/agents): Reinforcement learning algorithms and human agents.
-        *   [/rlcard/envs](rlcard/envs): Environment wrappers (state representation, action encoding etc.)
-        *   [/rlcard/games](rlcard/games): Various game engines.
-        *   [/rlcard/models](rlcard/models): Model zoo including pre-trained models and rule models.
-        
-        ## More Documents
-        For more documentation, please refer to the [Documents](docs/README.md) for general introductions. API documents are available at our [website](http://www.rlcard.org).
-        
-        ## Contributing
-        Contribution to this project is greatly appreciated! Please create an issue for feedbacks/bugs. If you want to contribute codes, please refer to [Contributing Guide](./CONTRIBUTING.md). If you have any questions, please contact [Daochen Zha](https://github.com/daochenzha) with [daochen.zha@rice.edu](mailto:daochen.zha@rice.edu).
-        
-        ## Acknowledgements
-        We would like to thank JJ World Network Technology Co.,LTD for the generous support and all the contributions from the community contributors.
-        
 Keywords: Reinforcement Learning,game,RL,AI
-Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: torch
+License-File: LICENSE.md
+
+# RLCard: A Toolkit for Reinforcement Learning in Card Games
+<img width="500" src="https://dczha.com/files/rlcard/logo.jpg" alt="Logo" />
+
+[![Testing](https://github.com/datamllab/rlcard/actions/workflows/python-package.yml/badge.svg)](https://github.com/datamllab/rlcard/actions/workflows/python-package.yml)
+[![PyPI version](https://badge.fury.io/py/rlcard.svg)](https://badge.fury.io/py/rlcard)
+[![Coverage Status](https://coveralls.io/repos/github/datamllab/rlcard/badge.svg)](https://coveralls.io/github/datamllab/rlcard?branch=master)
+[![Downloads](https://pepy.tech/badge/rlcard)](https://pepy.tech/project/rlcard)
+[![Downloads](https://pepy.tech/badge/rlcard/month)](https://pepy.tech/project/rlcard)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
+[中文文档](README.zh-CN.md)
+
+RLCard is a toolkit for Reinforcement Learning (RL) in card games. It supports multiple card environments with easy-to-use interfaces for implementing various reinforcement learning and searching algorithms. The goal of RLCard is to bridge reinforcement learning and imperfect information games. RLCard is developed by [DATA Lab](http://faculty.cs.tamu.edu/xiahu/) at Rice and Texas A&M University, and community contributors.
+
+*   Official Website: [https://www.rlcard.org](https://www.rlcard.org)
+*   Tutorial in Jupyter Notebook: [https://github.com/datamllab/rlcard-tutorial](https://github.com/datamllab/rlcard-tutorial)
+*   Paper: [https://arxiv.org/abs/1910.04376](https://arxiv.org/abs/1910.04376)
+*   Video: [YouTube](https://youtu.be/krK2jmSdKZc)
+*   GUI: [RLCard-Showdown](https://github.com/datamllab/rlcard-showdown)
+*   Dou Dizhu Demo: [Demo](https://douzero.org/)
+*   Resources: [Awesome-Game-AI](https://github.com/datamllab/awesome-game-ai)
+*   Related Project: [DouZero Project](https://github.com/kwai/DouZero)
+*   Zhihu: https://zhuanlan.zhihu.com/p/526723604
+*   Miscellaneous Resources: Have you heard of data-centric AI? Please check out our [data-centric AI survey](https://arxiv.org/abs/2303.10158) and [awesome data-centric AI resources](https://github.com/daochenzha/data-centric-AI)!
+
+**Community:**
+*  **Slack**: Discuss in our [#rlcard-project](https://join.slack.com/t/rlcard/shared_invite/zt-rkvktsaq-xkMwz8BfKupCM6zGhO01xg) slack channel.
+*  **QQ Group**: Join our QQ group to discuss. Password: rlcardqqgroup
+	*  Group 1: 665647450
+	*  Group 2: 117349516
+
+**News:**
+*   We have updated the tutorials in Jupyter Notebook to help you walk through RLCard! Please check [RLCard Tutorial](https://github.com/datamllab/rlcard-tutorial).
+*   All the algorithms can suppport [PettingZoo](https://github.com/PettingZoo-Team/PettingZoo) now. Please check [here](examples/pettingzoo). Thanks the contribtuion from [Yifei Cheng](https://github.com/ycheng517).
+*   Please follow [DouZero](https://github.com/kwai/DouZero), a strong Dou Dizhu AI and the [ICML 2021 paper](https://arxiv.org/abs/2106.06135). An online demo is available [here](https://douzero.org/). The algorithm is also integrated in RLCard. See [Training DMC on Dou Dizhu](docs/toy-examples.md#training-dmc-on-dou-dizhu).
+*   Our package is used in [PettingZoo](https://github.com/PettingZoo-Team/PettingZoo). Please check it out!
+*   We have released RLCard-Showdown, GUI demo for RLCard. Please check out [here](https://github.com/datamllab/rlcard-showdown)!
+*   Jupyter Notebook tutorial available! We add some examples in R to call Python interfaces of RLCard with reticulate. See [here](docs/toy-examples-r.md)
+*   Thanks for the contribution of [@Clarit7](https://github.com/Clarit7) for supporting different number of players in Blackjack. We call for contributions for gradually making the games more configurable. See [here](CONTRIBUTING.md#making-configurable-environments) for more details.
+*   Thanks for the contribution of [@Clarit7](https://github.com/Clarit7) for the Blackjack and Limit Hold'em human interface.
+*   Now RLCard supports environment local seeding and multiprocessing. Thanks for the testing scripts provided by [@weepingwillowben](https://github.com/weepingwillowben).
+*   Human interface of NoLimit Holdem available. The action space of NoLimit Holdem has been abstracted. Thanks for the contribution of [@AdrianP-](https://github.com/AdrianP-).
+*   New game Gin Rummy and human GUI available. Thanks for the contribution of [@billh0420](https://github.com/billh0420).
+*   PyTorch implementation available. Thanks for the contribution of [@mjudell](https://github.com/mjudell).
+
+## Contributors
+The following games are mainly developed and maintained by community contributors. Thank you!
+*   Gin Rummy: [@billh0420](https://github.com/billh0420)
+*   Bridge: [@billh0420](https://github.com/billh0420)
+
+Thank all the contributors!
+
+<a href="https://github.com/daochenzha"><img src="https://github.com/daochenzha.png" width="40px" alt="daochenzha" /></a>&nbsp;&nbsp;
+<a href="https://github.com/hsywhu"><img src="https://github.com/hsywhu.png" width="40px" alt="hsywhu" /></a>&nbsp;&nbsp;
+<a href="https://github.com/CaoYuanpu"><img src="https://github.com/CaoYuanpu.png" width="40px" alt="CaoYuanpu" /></a>&nbsp;&nbsp;
+<a href="https://github.com/billh0420"><img src="https://github.com/billh0420.png" width="40px" alt="billh0420" /></a>&nbsp;&nbsp;
+<a href="https://github.com/ruzhwei"><img src="https://github.com/ruzhwei.png" width="40px" alt="ruzhwei" /></a>&nbsp;&nbsp;
+<a href="https://github.com/adrianpgob"><img src="https://github.com/adrianpgob.png" width="40px" alt="adrianpgob" /></a>&nbsp;&nbsp;
+<a href="https://github.com/Zhigal"><img src="https://github.com/Zhigal.png" width="40px" alt="Zhigal" /></a>&nbsp;&nbsp;
+<a href="https://github.com/aypee19"><img src="https://github.com/aypee19.png" width="40px" alt="aypee19" /></a>&nbsp;&nbsp;
+<a href="https://github.com/Clarit7"><img src="https://github.com/Clarit7.png" width="40px" alt="Clarit7" /></a>&nbsp;&nbsp;
+<a href="https://github.com/lhenry15"><img src="https://github.com/lhenry15.png" width="40px" alt="lhenry15" /></a>&nbsp;&nbsp;
+<a href="https://github.com/ismael-elatifi"><img src="https://github.com/ismael-elatifi.png" width="40px" alt="ismael-elatifi" /></a>&nbsp;&nbsp;
+<a href="https://github.com/mjudell"><img src="https://github.com/mjudell.png" width="40px" alt="mjudell" /></a>&nbsp;&nbsp;
+<a href="https://github.com/jkterry1"><img src="https://github.com/jkterry1.png" width="40px" alt="jkterry1" /></a>&nbsp;&nbsp;
+<a href="https://github.com/kaanozdogru"><img src="https://github.com/kaanozdogru.png" width="40px" alt="kaanozdogru" /></a>&nbsp;&nbsp;
+<a href="https://github.com/junyuGuo"><img src="https://github.com/junyuGuo.png" width="40px" alt="junyuGuo" /></a>&nbsp;&nbsp;
+<br />
+<a href="https://github.com/Xixo99"><img src="https://github.com/Xixo99.png" width="40px" alt="Xixo99" /></a>&nbsp;&nbsp;
+<a href="https://github.com/rodrigodelazcano"><img src="https://github.com/rodrigodelazcano.png" width="40px" alt="rodrigodelazcano" /></a>&nbsp;&nbsp;
+<a href="https://github.com/Michael1015198808"><img src="https://github.com/Michael1015198808.png" width="40px" alt="Michael1015198808" /></a>&nbsp;&nbsp;
+<a href="https://github.com/mia1996"><img src="https://github.com/mia1996.png" width="40px" alt="mia1996" /></a>&nbsp;&nbsp;
+<a href="https://github.com/kaiks"><img src="https://github.com/kaiks.png" width="40px" alt="kaiks" /></a>&nbsp;&nbsp;
+<a href="https://github.com/claude9493"><img src="https://github.com/claude9493.png" width="40px" alt="claude9493" /></a>&nbsp;&nbsp;
+<a href="https://github.com/SonSang"><img src="https://github.com/SonSang.png" width="40px" alt="SonSang" /></a>&nbsp;&nbsp;
+<a href="https://github.com/rishabhvarshney14"><img src="https://github.com/rishabhvarshney14.png" width="40px" alt="rishabhvarshney14" /></a>&nbsp;&nbsp;
+<a href="https://github.com/aetheryang"><img src="https://github.com/aetheryang.png" width="40px" alt="aetheryang" /></a>&nbsp;&nbsp;
+<a href="https://github.com/rxng8"><img src="https://github.com/rxng8.png" width="40px" alt="rxng8" /></a>&nbsp;&nbsp;
+<a href="https://github.com/nondecidibile"><img src="https://github.com/nondecidibile.png" width="40px" alt="nondecidibile" /></a>&nbsp;&nbsp;
+<a href="https://github.com/benblack769"><img src="https://github.com/benblack769.png" width="40px" alt="benblack769" /></a>&nbsp;&nbsp;
+<a href="https://github.com/zhengsx"><img src="https://github.com/zhengsx.png" width="40px" alt="zhengsx" /></a>&nbsp;&nbsp;
+<a href="https://github.com/andrewnc"><img src="https://github.com/andrewnc.png" width="40px" alt="andrewnc" /></a>&nbsp;&nbsp;
+
+## Cite this work
+If you find this repo useful, you may cite:
+
+Zha, Daochen, et al. "RLCard: A Platform for Reinforcement Learning in Card Games." IJCAI. 2020.
+```bibtex
+@inproceedings{zha2020rlcard,
+  title={RLCard: A Platform for Reinforcement Learning in Card Games},
+  author={Zha, Daochen and Lai, Kwei-Herng and Huang, Songyi and Cao, Yuanpu and Reddy, Keerthana and Vargas, Juan and Nguyen, Alex and Wei, Ruzhe and Guo, Junyu and Hu, Xia},
+  booktitle={IJCAI},
+  year={2020}
+}
+```
+
+## Installation
+Make sure that you have **Python 3.6+** and **pip** installed. We recommend installing the stable version of `rlcard` with `pip`:
+
+```
+pip3 install rlcard
+```
+The default installation will only include the card environments. To use PyTorch implementation of the training algorithms, run
+```
+pip3 install rlcard[torch]
+```
+If you are in China and the above command is too slow, you can use the mirror provided by Tsinghua University:
+```
+pip3 install rlcard -i https://pypi.tuna.tsinghua.edu.cn/simple
+```
+Alternatively, you can clone the latest version with (if you are in China and Github is slow, you can use the mirror in [Gitee](https://gitee.com/daochenzha/rlcard)):
+```
+git clone https://github.com/datamllab/rlcard.git
+```
+or only clone one branch to make it faster:
+```
+git clone -b master --single-branch --depth=1 https://github.com/datamllab/rlcard.git
+```
+Then install with
+```
+cd rlcard
+pip3 install -e .
+pip3 install -e .[torch]
+```
+
+We also provide [**conda** installation method](https://anaconda.org/toubun/rlcard):
+
+```
+conda install -c toubun rlcard
+```
+
+Conda installation only provides the card environments, you need to manually install Pytorch on your demands.
+
+## Examples
+A **short example** is as below.
+
+```python
+import rlcard
+from rlcard.agents import RandomAgent
+
+env = rlcard.make('blackjack')
+env.set_agents([RandomAgent(num_actions=env.num_actions)])
+
+print(env.num_actions) # 2
+print(env.num_players) # 1
+print(env.state_shape) # [[2]]
+print(env.action_shape) # [None]
+
+trajectories, payoffs = env.run()
+```
+
+RLCard can be flexibly connected to various algorithms. See the following examples:
+
+*   [Playing with random agents](docs/toy-examples.md#playing-with-random-agents)
+*   [Deep-Q learning on Blackjack](docs/toy-examples.md#deep-q-learning-on-blackjack)
+*   [Training CFR (chance sampling) on Leduc Hold'em](docs/toy-examples.md#training-cfr-on-leduc-holdem)
+*   [Having fun with pretrained Leduc model](docs/toy-examples.md#having-fun-with-pretrained-leduc-model)
+*   [Training DMC on Dou Dizhu](docs/toy-examples.md#training-dmc-on-dou-dizhu)
+*   [Evaluating Agents](docs/toy-examples.md#evaluating-agents)
+*   [Training Agents on PettingZoo](examples/pettingzoo)
+
+## Demo
+Run `examples/human/leduc_holdem_human.py` to play with the pre-trained Leduc Hold'em model. Leduc Hold'em is a simplified version of Texas Hold'em. Rules can be found [here](docs/games.md#leduc-holdem).
+
+```
+>> Leduc Hold'em pre-trained model
+
+>> Start a new game!
+>> Agent 1 chooses raise
+
+=============== Community Card ===============
+┌─────────┐
+│░░░░░░░░░│
+│░░░░░░░░░│
+│░░░░░░░░░│
+│░░░░░░░░░│
+│░░░░░░░░░│
+│░░░░░░░░░│
+│░░░░░░░░░│
+└─────────┘
+===============   Your Hand    ===============
+┌─────────┐
+│J        │
+│         │
+│         │
+│    ♥    │
+│         │
+│         │
+│        J│
+└─────────┘
+===============     Chips      ===============
+Yours:   +
+Agent 1: +++
+=========== Actions You Can Choose ===========
+0: call, 1: raise, 2: fold
+
+>> You choose action (integer):
+```
+We also provide a GUI for easy debugging. Please check [here](https://github.com/datamllab/rlcard-showdown/). Some demos:
+
+![doudizhu-replay](https://github.com/datamllab/rlcard-showdown/blob/master/docs/imgs/doudizhu-replay.png?raw=true)
+![leduc-replay](https://github.com/datamllab/rlcard-showdown/blob/master/docs/imgs/leduc-replay.png?raw=true)
+
+## Available Environments
+We provide a complexity estimation for the games on several aspects. **InfoSet Number:** the number of information sets; **InfoSet Size:** the average number of states in a single information set; **Action Size:** the size of the action space. **Name:** the name that should be passed to `rlcard.make` to create the game environment. We also provide the link to the documentation and the random example.
+
+| Game                                                                                                                                                                                           | InfoSet Number  | InfoSet Size      | Action Size | Name            | Usage                                                                                       |
+| :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :-------------: | :---------------: | :---------: | :-------------: | :-----------------------------------------------------------------------------------------: |
+| Blackjack ([wiki](https://en.wikipedia.org/wiki/Blackjack), [baike](https://baike.baidu.com/item/21%E7%82%B9/5481683?fr=aladdin))                                                              | 10^3            | 10^1              | 10^0        | blackjack       | [doc](docs/games.md#blackjack), [example](examples/run_random.py)                           |
+| Leduc Hold’em ([paper](http://poker.cs.ualberta.ca/publications/UAI05.pdf))                                                                                                                    | 10^2            | 10^2              | 10^0        | leduc-holdem    | [doc](docs/games.md#leduc-holdem), [example](examples/run_random.py)                        |
+| Limit Texas Hold'em ([wiki](https://en.wikipedia.org/wiki/Texas_hold_%27em), [baike](https://baike.baidu.com/item/%E5%BE%B7%E5%85%8B%E8%90%A8%E6%96%AF%E6%89%91%E5%85%8B/83440?fr=aladdin))    | 10^14           | 10^3              | 10^0        | limit-holdem    | [doc](docs/games.md#limit-texas-holdem), [example](examples/run_random.py)                  |
+| Dou Dizhu ([wiki](https://en.wikipedia.org/wiki/Dou_dizhu), [baike](https://baike.baidu.com/item/%E6%96%97%E5%9C%B0%E4%B8%BB/177997?fr=aladdin))                                               | 10^53 ~ 10^83   | 10^23             | 10^4        | doudizhu        | [doc](docs/games.md#dou-dizhu), [example](examples/run_random.py)                           |
+| Mahjong ([wiki](https://en.wikipedia.org/wiki/Competition_Mahjong_scoring_rules), [baike](https://baike.baidu.com/item/%E9%BA%BB%E5%B0%86/215))                                                | 10^121          | 10^48             | 10^2        | mahjong         | [doc](docs/games.md#mahjong), [example](examples/run_random.py)                             | 
+| No-limit Texas Hold'em ([wiki](https://en.wikipedia.org/wiki/Texas_hold_%27em), [baike](https://baike.baidu.com/item/%E5%BE%B7%E5%85%8B%E8%90%A8%E6%96%AF%E6%89%91%E5%85%8B/83440?fr=aladdin)) | 10^162          | 10^3              | 10^4        | no-limit-holdem | [doc](docs/games.md#no-limit-texas-holdem), [example](examples/run_random.py)               |
+| UNO ([wiki](https://en.wikipedia.org/wiki/Uno_\(card_game\)), [baike](https://baike.baidu.com/item/UNO%E7%89%8C/2249587))                                                                      |  10^163         | 10^10             | 10^1        | uno             | [doc](docs/games.md#uno), [example](examples/run_random.py)                                 |
+| Gin Rummy ([wiki](https://en.wikipedia.org/wiki/Gin_rummy), [baike](https://baike.baidu.com/item/%E9%87%91%E6%8B%89%E7%B1%B3/3471710))                                                         | 10^52           | -                 | -           | gin-rummy       | [doc](docs/games.md#gin-rummy), [example](examples/run_random.py)                           |
+| Bridge ([wiki](https://en.wikipedia.org/wiki/Bridge), [baike](https://baike.baidu.com/item/%E6%A1%A5%E7%89%8C/332030))                                                                         |                 | -                 | -           | bridge          | [doc](docs/games.md#bridge), [example](examples/run_random.py)                              |
+
+## Supported Algorithms
+| Algorithm | example | reference |
+| :--------------------------------------: | :-----------------------------------------: | :------------------------------------------------------------------------------------------------------: |
+| Deep Monte-Carlo (DMC)                   | [examples/run\_dmc.py](examples/run_dmc.py) | [[paper]](https://arxiv.org/abs/2106.06135)                                                              |
+| Deep Q-Learning (DQN)                    | [examples/run\_rl.py](examples/run_rl.py)   | [[paper]](https://arxiv.org/abs/1312.5602)                                                               |
+| Neural Fictitious Self-Play (NFSP)       | [examples/run\_rl.py](examples/run_rl.py)   | [[paper]](https://arxiv.org/abs/1603.01121)                                                              |
+| Counterfactual Regret Minimization (CFR) | [examples/run\_cfr.py](examples/run_cfr.py) | [[paper]](http://papers.nips.cc/paper/3306-regret-minimization-in-games-with-incomplete-information.pdf) |
+
+## Pre-trained and Rule-based Models
+We provide a [model zoo](rlcard/models) to serve as the baselines.
+
+| Model                                    | Explanation                                              |
+| :--------------------------------------: | :------------------------------------------------------: |
+| leduc-holdem-cfr                         | Pre-trained CFR (chance sampling) model on Leduc Hold'em |
+| leduc-holdem-rule-v1                     | Rule-based model for Leduc Hold'em, v1                   |
+| leduc-holdem-rule-v2                     | Rule-based model for Leduc Hold'em, v2                   |
+| uno-rule-v1                              | Rule-based model for UNO, v1                             |
+| limit-holdem-rule-v1                     | Rule-based model for Limit Texas Hold'em, v1             |
+| doudizhu-rule-v1                         | Rule-based model for Dou Dizhu, v1                       |
+| gin-rummy-novice-rule                    | Gin Rummy novice rule model                              |
+
+## API Cheat Sheet
+### How to create an environment
+You can use the the following interface to make an environment. You may optionally specify some configurations with a dictionary.
+*   **env = rlcard.make(env_id, config={})**: Make an environment. `env_id` is a string of a environment; `config` is a dictionary that specifies some environment configurations, which are as follows.
+	*   `seed`: Default `None`. Set a environment local random seed for reproducing the results.
+	*   `allow_step_back`: Default `False`. `True` if allowing `step_back` function to traverse backward in the tree.
+	*   Game specific configurations: These fields start with `game_`. Currently, we only support `game_num_players` in Blackjack, .
+
+Once the environemnt is made, we can access some information of the game.
+*   **env.num_actions**: The number of actions.
+*   **env.num_players**: The number of players.
+*   **env.state_shape**: The shape of the state space of the observations.
+*   **env.action_shape**: The shape of the action features (Dou Dizhu's action can encoded as features)
+
+### What is state in RLCard
+State is a Python dictionary. It consists of observation `state['obs']`, legal actions `state['legal_actions']`, raw observation `state['raw_obs']` and raw legal actions `state['raw_legal_actions']`.
+
+### Basic interfaces
+The following interfaces provide a basic usage. It is easy to use but it has assumtions on the agent. The agent must follow [agent template](docs/developping-algorithms.md). 
+*   **env.set_agents(agents)**: `agents` is a list of `Agent` object. The length of the list should be equal to the number of the players in the game.
+*   **env.run(is_training=False)**: Run a complete game and return trajectories and payoffs. The function can be used after the `set_agents` is called. If `is_training` is `True`, it will use `step` function in the agent to play the game. If `is_training` is `False`, `eval_step` will be called instead.
+
+### Advanced interfaces
+For advanced usage, the following interfaces allow flexible operations on the game tree. These interfaces do not make any assumtions on the agent.
+*   **env.reset()**: Initialize a game. Return the state and the first player ID.
+*   **env.step(action, raw_action=False)**: Take one step in the environment. `action` can be raw action or integer; `raw_action` should be `True` if the action is raw action (string).
+*   **env.step_back()**: Available only when `allow_step_back` is `True`. Take one step backward. This can be used for algorithms that operate on the game tree, such as CFR (chance sampling).
+*   **env.is_over()**: Return `True` if the current game is over. Otherewise, return `False`.
+*   **env.get_player_id()**: Return the Player ID of the current player.
+*   **env.get_state(player_id)**: Return the state that corresponds to `player_id`.
+*   **env.get_payoffs()**: In the end of the game, return a list of payoffs for all the players.
+*   **env.get_perfect_information()**: (Currently only support some of the games) Obtain the perfect information at the current state.
+
+## Library Structure
+The purposes of the main modules are listed as below:
+
+*   [/examples](examples): Examples of using RLCard.
+*   [/docs](docs): Documentation of RLCard.
+*   [/tests](tests): Testing scripts for RLCard.
+*   [/rlcard/agents](rlcard/agents): Reinforcement learning algorithms and human agents.
+*   [/rlcard/envs](rlcard/envs): Environment wrappers (state representation, action encoding etc.)
+*   [/rlcard/games](rlcard/games): Various game engines.
+*   [/rlcard/models](rlcard/models): Model zoo including pre-trained models and rule models.
+
+## More Documents
+For more documentation, please refer to the [Documents](docs/README.md) for general introductions. API documents are available at our [website](http://www.rlcard.org).
+
+## Contributing
+Contribution to this project is greatly appreciated! Please create an issue for feedbacks/bugs. If you want to contribute codes, please refer to [Contributing Guide](./CONTRIBUTING.md). If you have any questions, please contact [Daochen Zha](https://github.com/daochenzha) with [daochen.zha@rice.edu](mailto:daochen.zha@rice.edu).
+
+## Acknowledgements
+We would like to thank JJ World Network Technology Co.,LTD for the generous support and all the contributions from the community contributors.
```

### Comparing `rlcard-1.1.0/README.md` & `rlcard-1.2.0/rlcard.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: rlcard
+Version: 1.2.0
+Summary: A Toolkit for Reinforcement Learning in Card Games
+Home-page: https://github.com/datamllab/rlcard
+Author: Data Analytics at Texas A&M (DATA) Lab
+Author-email: daochen.zha@tamu.edu
+Keywords: Reinforcement Learning,game,RL,AI
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.7
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+Provides-Extra: torch
+License-File: LICENSE.md
+
 # RLCard: A Toolkit for Reinforcement Learning in Card Games
 <img width="500" src="https://dczha.com/files/rlcard/logo.jpg" alt="Logo" />
 
 [![Testing](https://github.com/datamllab/rlcard/actions/workflows/python-package.yml/badge.svg)](https://github.com/datamllab/rlcard/actions/workflows/python-package.yml)
 [![PyPI version](https://badge.fury.io/py/rlcard.svg)](https://badge.fury.io/py/rlcard)
 [![Coverage Status](https://coveralls.io/repos/github/datamllab/rlcard/badge.svg)](https://coveralls.io/github/datamllab/rlcard?branch=master)
 [![Downloads](https://pepy.tech/badge/rlcard)](https://pepy.tech/project/rlcard)
@@ -11,19 +30,21 @@
 [中文文档](README.zh-CN.md)
 
 RLCard is a toolkit for Reinforcement Learning (RL) in card games. It supports multiple card environments with easy-to-use interfaces for implementing various reinforcement learning and searching algorithms. The goal of RLCard is to bridge reinforcement learning and imperfect information games. RLCard is developed by [DATA Lab](http://faculty.cs.tamu.edu/xiahu/) at Rice and Texas A&M University, and community contributors.
 
 *   Official Website: [https://www.rlcard.org](https://www.rlcard.org)
 *   Tutorial in Jupyter Notebook: [https://github.com/datamllab/rlcard-tutorial](https://github.com/datamllab/rlcard-tutorial)
 *   Paper: [https://arxiv.org/abs/1910.04376](https://arxiv.org/abs/1910.04376)
+*   Video: [YouTube](https://youtu.be/krK2jmSdKZc)
 *   GUI: [RLCard-Showdown](https://github.com/datamllab/rlcard-showdown)
 *   Dou Dizhu Demo: [Demo](https://douzero.org/)
 *   Resources: [Awesome-Game-AI](https://github.com/datamllab/awesome-game-ai)
 *   Related Project: [DouZero Project](https://github.com/kwai/DouZero)
 *   Zhihu: https://zhuanlan.zhihu.com/p/526723604
+*   Miscellaneous Resources: Have you heard of data-centric AI? Please check out our [data-centric AI survey](https://arxiv.org/abs/2303.10158) and [awesome data-centric AI resources](https://github.com/daochenzha/data-centric-AI)!
 
 **Community:**
 *  **Slack**: Discuss in our [#rlcard-project](https://join.slack.com/t/rlcard/shared_invite/zt-rkvktsaq-xkMwz8BfKupCM6zGhO01xg) slack channel.
 *  **QQ Group**: Join our QQ group to discuss. Password: rlcardqqgroup
 	*  Group 1: 665647450
 	*  Group 2: 117349516
 
@@ -37,14 +58,52 @@
 *   Thanks for the contribution of [@Clarit7](https://github.com/Clarit7) for supporting different number of players in Blackjack. We call for contributions for gradually making the games more configurable. See [here](CONTRIBUTING.md#making-configurable-environments) for more details.
 *   Thanks for the contribution of [@Clarit7](https://github.com/Clarit7) for the Blackjack and Limit Hold'em human interface.
 *   Now RLCard supports environment local seeding and multiprocessing. Thanks for the testing scripts provided by [@weepingwillowben](https://github.com/weepingwillowben).
 *   Human interface of NoLimit Holdem available. The action space of NoLimit Holdem has been abstracted. Thanks for the contribution of [@AdrianP-](https://github.com/AdrianP-).
 *   New game Gin Rummy and human GUI available. Thanks for the contribution of [@billh0420](https://github.com/billh0420).
 *   PyTorch implementation available. Thanks for the contribution of [@mjudell](https://github.com/mjudell).
 
+## Contributors
+The following games are mainly developed and maintained by community contributors. Thank you!
+*   Gin Rummy: [@billh0420](https://github.com/billh0420)
+*   Bridge: [@billh0420](https://github.com/billh0420)
+
+Thank all the contributors!
+
+<a href="https://github.com/daochenzha"><img src="https://github.com/daochenzha.png" width="40px" alt="daochenzha" /></a>&nbsp;&nbsp;
+<a href="https://github.com/hsywhu"><img src="https://github.com/hsywhu.png" width="40px" alt="hsywhu" /></a>&nbsp;&nbsp;
+<a href="https://github.com/CaoYuanpu"><img src="https://github.com/CaoYuanpu.png" width="40px" alt="CaoYuanpu" /></a>&nbsp;&nbsp;
+<a href="https://github.com/billh0420"><img src="https://github.com/billh0420.png" width="40px" alt="billh0420" /></a>&nbsp;&nbsp;
+<a href="https://github.com/ruzhwei"><img src="https://github.com/ruzhwei.png" width="40px" alt="ruzhwei" /></a>&nbsp;&nbsp;
+<a href="https://github.com/adrianpgob"><img src="https://github.com/adrianpgob.png" width="40px" alt="adrianpgob" /></a>&nbsp;&nbsp;
+<a href="https://github.com/Zhigal"><img src="https://github.com/Zhigal.png" width="40px" alt="Zhigal" /></a>&nbsp;&nbsp;
+<a href="https://github.com/aypee19"><img src="https://github.com/aypee19.png" width="40px" alt="aypee19" /></a>&nbsp;&nbsp;
+<a href="https://github.com/Clarit7"><img src="https://github.com/Clarit7.png" width="40px" alt="Clarit7" /></a>&nbsp;&nbsp;
+<a href="https://github.com/lhenry15"><img src="https://github.com/lhenry15.png" width="40px" alt="lhenry15" /></a>&nbsp;&nbsp;
+<a href="https://github.com/ismael-elatifi"><img src="https://github.com/ismael-elatifi.png" width="40px" alt="ismael-elatifi" /></a>&nbsp;&nbsp;
+<a href="https://github.com/mjudell"><img src="https://github.com/mjudell.png" width="40px" alt="mjudell" /></a>&nbsp;&nbsp;
+<a href="https://github.com/jkterry1"><img src="https://github.com/jkterry1.png" width="40px" alt="jkterry1" /></a>&nbsp;&nbsp;
+<a href="https://github.com/kaanozdogru"><img src="https://github.com/kaanozdogru.png" width="40px" alt="kaanozdogru" /></a>&nbsp;&nbsp;
+<a href="https://github.com/junyuGuo"><img src="https://github.com/junyuGuo.png" width="40px" alt="junyuGuo" /></a>&nbsp;&nbsp;
+<br />
+<a href="https://github.com/Xixo99"><img src="https://github.com/Xixo99.png" width="40px" alt="Xixo99" /></a>&nbsp;&nbsp;
+<a href="https://github.com/rodrigodelazcano"><img src="https://github.com/rodrigodelazcano.png" width="40px" alt="rodrigodelazcano" /></a>&nbsp;&nbsp;
+<a href="https://github.com/Michael1015198808"><img src="https://github.com/Michael1015198808.png" width="40px" alt="Michael1015198808" /></a>&nbsp;&nbsp;
+<a href="https://github.com/mia1996"><img src="https://github.com/mia1996.png" width="40px" alt="mia1996" /></a>&nbsp;&nbsp;
+<a href="https://github.com/kaiks"><img src="https://github.com/kaiks.png" width="40px" alt="kaiks" /></a>&nbsp;&nbsp;
+<a href="https://github.com/claude9493"><img src="https://github.com/claude9493.png" width="40px" alt="claude9493" /></a>&nbsp;&nbsp;
+<a href="https://github.com/SonSang"><img src="https://github.com/SonSang.png" width="40px" alt="SonSang" /></a>&nbsp;&nbsp;
+<a href="https://github.com/rishabhvarshney14"><img src="https://github.com/rishabhvarshney14.png" width="40px" alt="rishabhvarshney14" /></a>&nbsp;&nbsp;
+<a href="https://github.com/aetheryang"><img src="https://github.com/aetheryang.png" width="40px" alt="aetheryang" /></a>&nbsp;&nbsp;
+<a href="https://github.com/rxng8"><img src="https://github.com/rxng8.png" width="40px" alt="rxng8" /></a>&nbsp;&nbsp;
+<a href="https://github.com/nondecidibile"><img src="https://github.com/nondecidibile.png" width="40px" alt="nondecidibile" /></a>&nbsp;&nbsp;
+<a href="https://github.com/benblack769"><img src="https://github.com/benblack769.png" width="40px" alt="benblack769" /></a>&nbsp;&nbsp;
+<a href="https://github.com/zhengsx"><img src="https://github.com/zhengsx.png" width="40px" alt="zhengsx" /></a>&nbsp;&nbsp;
+<a href="https://github.com/andrewnc"><img src="https://github.com/andrewnc.png" width="40px" alt="andrewnc" /></a>&nbsp;&nbsp;
+
 ## Cite this work
 If you find this repo useful, you may cite:
 
 Zha, Daochen, et al. "RLCard: A Platform for Reinforcement Learning in Card Games." IJCAI. 2020.
 ```bibtex
 @inproceedings{zha2020rlcard,
   title={RLCard: A Platform for Reinforcement Learning in Card Games},
```

### Comparing `rlcard-1.1.0/rlcard/agents/__init__.py` & `rlcard-1.2.0/rlcard/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/agents/cfr_agent.py` & `rlcard-1.2.0/rlcard/agents/cfr_agent.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/agents/dmc_agent/file_writer.py` & `rlcard-1.2.0/rlcard/agents/dmc_agent/file_writer.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/agents/dmc_agent/model.py` & `rlcard-1.2.0/rlcard/agents/dmc_agent/model.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/agents/dmc_agent/pettingzoo_model.py` & `rlcard-1.2.0/rlcard/agents/dmc_agent/pettingzoo_model.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/agents/dmc_agent/pettingzoo_utils.py` & `rlcard-1.2.0/rlcard/agents/dmc_agent/pettingzoo_utils.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/agents/dmc_agent/trainer.py` & `rlcard-1.2.0/rlcard/agents/dmc_agent/trainer.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/agents/dmc_agent/utils.py` & `rlcard-1.2.0/rlcard/agents/dmc_agent/utils.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/agents/dqn_agent.py` & `rlcard-1.2.0/rlcard/agents/nfsp_agent.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,417 +1,525 @@
-''' DQN agent
+# Copyright 2019 Matthew Judell. All rights reserved.
+# Copyright 2019 DATA Lab at Texas A&M University. All rights reserved.
+# Copyright 2019 DeepMind Technologies Ltd. All rights reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#         http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
-The code is derived from https://github.com/dennybritz/reinforcement-learning/blob/master/DQN/dqn.py
+''' Neural Fictitious Self-Play (NFSP) agent implemented in TensorFlow.
 
-Copyright (c) 2019 Matthew Judell
-Copyright (c) 2019 DATA Lab at Texas A&M University
-Copyright (c) 2016 Denny Britz
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+See the paper https://arxiv.org/abs/1603.01121 for more details.
 '''
 
 import random
+import collections
+import enum
 import numpy as np
 import torch
 import torch.nn as nn
-from collections import namedtuple
-from copy import deepcopy
+import torch.nn.functional as F
 
+from rlcard.agents.dqn_agent import DQNAgent
 from rlcard.utils.utils import remove_illegal
 
-Transition = namedtuple('Transition', ['state', 'action', 'reward', 'next_state', 'done', 'legal_actions'])
+Transition = collections.namedtuple('Transition', 'info_state action_probs')
 
-
-class DQNAgent(object):
-    '''
-    Approximate clone of rlcard.agents.dqn_agent.DQNAgent
-    that depends on PyTorch instead of Tensorflow
+class NFSPAgent(object):
+    ''' An approximate clone of rlcard.agents.nfsp_agent that uses
+    pytorch instead of tensorflow.  Note that this implementation
+    differs from Henrich and Silver (2016) in that the supervised
+    training minimizes cross-entropy with respect to the stored
+    action probabilities rather than the realized actions.
     '''
+
     def __init__(self,
-                 replay_memory_size=20000,
-                 replay_memory_init_size=100,
-                 update_target_estimator_every=1000,
-                 discount_factor=0.99,
-                 epsilon_start=1.0,
-                 epsilon_end=0.1,
-                 epsilon_decay_steps=20000,
-                 batch_size=32,
-                 num_actions=2,
+                 num_actions=4,
                  state_shape=None,
+                 hidden_layers_sizes=None,
+                 reservoir_buffer_capacity=20000,
+                 anticipatory_param=0.1,
+                 batch_size=256,
                  train_every=1,
-                 mlp_layers=None,
-                 learning_rate=0.00005,
-                 device=None):
-
-        '''
-        Q-Learning algorithm for off-policy TD control using Function Approximation.
-        Finds the optimal greedy policy while following an epsilon-greedy policy.
-
-        Args:
-            replay_memory_size (int): Size of the replay memory
-            replay_memory_init_size (int): Number of random experiences to sample when initializing
-              the reply memory.
-            update_target_estimator_every (int): Copy parameters from the Q estimator to the
-              target estimator every N steps
-            discount_factor (float): Gamma discount factor
-            epsilon_start (float): Chance to sample a random action when taking an action.
-              Epsilon is decayed over time and this is the start value
-            epsilon_end (float): The final minimum value of epsilon after decaying is done
-            epsilon_decay_steps (int): Number of steps to decay epsilon over
-            batch_size (int): Size of batches to sample from the replay memory
-            evaluate_every (int): Evaluate every N steps
-            num_actions (int): The number of the actions
-            state_space (list): The space of the state vector
-            train_every (int): Train the network every X steps.
-            mlp_layers (list): The layer number and the dimension of each layer in MLP
-            learning_rate (float): The learning rate of the DQN agent.
-            device (torch.device): whether to use the cpu or gpu
+                 rl_learning_rate=0.1,
+                 sl_learning_rate=0.005,
+                 min_buffer_size_to_learn=100,
+                 q_replay_memory_size=20000,
+                 q_replay_memory_init_size=100,
+                 q_update_target_estimator_every=1000,
+                 q_discount_factor=0.99,
+                 q_epsilon_start=0.06,
+                 q_epsilon_end=0,
+                 q_epsilon_decay_steps=int(1e6),
+                 q_batch_size=32,
+                 q_train_every=1,
+                 q_mlp_layers=None,
+                 evaluate_with='average_policy',
+                 device=None,
+                 save_path=None,
+                 save_every=float('inf')):
+        ''' Initialize the NFSP agent.
+
+        Args:
+            num_actions (int): The number of actions.
+            state_shape (list): The shape of the state space.
+            hidden_layers_sizes (list): The hidden layers sizes for the layers of
+              the average policy.
+            reservoir_buffer_capacity (int): The size of the buffer for average policy.
+            anticipatory_param (float): The hyper-parameter that balances rl/avarage policy.
+            batch_size (int): The batch_size for training average policy.
+            train_every (int): Train the SL policy every X steps.
+            rl_learning_rate (float): The learning rate of the RL agent.
+            sl_learning_rate (float): the learning rate of the average policy.
+            min_buffer_size_to_learn (int): The minimum buffer size to learn for average policy.
+            q_replay_memory_size (int): The memory size of inner DQN agent.
+            q_replay_memory_init_size (int): The initial memory size of inner DQN agent.
+            q_update_target_estimator_every (int): The frequency of updating target network for
+              inner DQN agent.
+            q_discount_factor (float): The discount factor of inner DQN agent.
+            q_epsilon_start (float): The starting epsilon of inner DQN agent.
+            q_epsilon_end (float): the end epsilon of inner DQN agent.
+            q_epsilon_decay_steps (int): The decay steps of inner DQN agent.
+            q_batch_size (int): The batch size of inner DQN agent.
+            q_train_step (int): Train the model every X steps.
+            q_mlp_layers (list): The layer sizes of inner DQN agent.
+            device (torch.device): Whether to use the cpu or gpu
         '''
         self.use_raw = False
-        self.replay_memory_init_size = replay_memory_init_size
-        self.update_target_estimator_every = update_target_estimator_every
-        self.discount_factor = discount_factor
-        self.epsilon_decay_steps = epsilon_decay_steps
-        self.batch_size = batch_size
-        self.num_actions = num_actions
-        self.train_every = train_every
+        self._num_actions = num_actions
+        self._state_shape = state_shape
+        self._layer_sizes = hidden_layers_sizes + [num_actions]
+        self._batch_size = batch_size
+        self._train_every = train_every
+        self._sl_learning_rate = sl_learning_rate
+        self._anticipatory_param = anticipatory_param
+        self._min_buffer_size_to_learn = min_buffer_size_to_learn
+
+        self._reservoir_buffer = ReservoirBuffer(reservoir_buffer_capacity)
+        self._prev_timestep = None
+        self._prev_action = None
+        self.evaluate_with = evaluate_with
 
-        # Torch device
         if device is None:
             self.device = torch.device('cuda:0' if torch.cuda.is_available() else 'cpu')
         else:
             self.device = device
 
         # Total timesteps
         self.total_t = 0
 
         # Total training step
         self.train_t = 0
 
-        # The epsilon decay scheduler
-        self.epsilons = np.linspace(epsilon_start, epsilon_end, epsilon_decay_steps)
+        # Build the action-value network
+        self._rl_agent = DQNAgent(q_replay_memory_size, q_replay_memory_init_size, \
+            q_update_target_estimator_every, q_discount_factor, q_epsilon_start, q_epsilon_end, \
+            q_epsilon_decay_steps, q_batch_size, num_actions, state_shape, q_train_every, q_mlp_layers, \
+            rl_learning_rate, device)
+
+        # Build the average policy supervised model
+        self._build_model()
+
+        self.sample_episode_policy()
+        
+        # Checkpoint saving parameters
+        self.save_path = save_path
+        self.save_every = save_every
+
+    def _build_model(self):
+        ''' Build the average policy network
+        '''
+
+        # configure the average policy network
+        policy_network = AveragePolicyNetwork(self._num_actions, self._state_shape, self._layer_sizes)
+        policy_network = policy_network.to(self.device)
+        self.policy_network = policy_network
+        self.policy_network.eval()
 
-        # Create estimators
-        self.q_estimator = Estimator(num_actions=num_actions, learning_rate=learning_rate, state_shape=state_shape, \
-            mlp_layers=mlp_layers, device=self.device)
-        self.target_estimator = Estimator(num_actions=num_actions, learning_rate=learning_rate, state_shape=state_shape, \
-            mlp_layers=mlp_layers, device=self.device)
+        # xavier init
+        for p in self.policy_network.parameters():
+            if len(p.data.shape) > 1:
+                nn.init.xavier_uniform_(p.data)
 
-        # Create replay memory
-        self.memory = Memory(replay_memory_size, batch_size)
+        # configure optimizer
+        self.policy_network_optimizer = torch.optim.Adam(self.policy_network.parameters(), lr=self._sl_learning_rate)
 
     def feed(self, ts):
-        ''' Store data in to replay buffer and train the agent. There are two stages.
-            In stage 1, populate the memory without training
-            In stage 2, train the agent every several timesteps
+        ''' Feed data to inner RL agent
 
         Args:
-            ts (list): a list of 5 elements that represent the transition
+            ts (list): A list of 5 elements that represent the transition.
         '''
-        (state, action, reward, next_state, done) = tuple(ts)
-        self.feed_memory(state['obs'], action, reward, next_state['obs'], list(next_state['legal_actions'].keys()), done)
+        self._rl_agent.feed(ts)
         self.total_t += 1
-        tmp = self.total_t - self.replay_memory_init_size
-        if tmp>=0 and tmp%self.train_every == 0:
-            self.train()
+        if self.total_t>0 and len(self._reservoir_buffer) >= self._min_buffer_size_to_learn and self.total_t%self._train_every == 0:
+            sl_loss  = self.train_sl()
+            print('\rINFO - Step {}, sl-loss: {}'.format(self.total_t, sl_loss), end='')
 
     def step(self, state):
-        ''' Predict the action for genrating training data but
-            have the predictions disconnected from the computation graph
+        ''' Returns the action to be taken.
 
         Args:
-            state (numpy.array): current state
+            state (dict): The current state
 
         Returns:
-            action (int): an action id
+            action (int): An action id
         '''
-        q_values = self.predict(state)
-        epsilon = self.epsilons[min(self.total_t, self.epsilon_decay_steps-1)]
+        obs = state['obs']
         legal_actions = list(state['legal_actions'].keys())
-        probs = np.ones(len(legal_actions), dtype=float) * epsilon / len(legal_actions)
-        best_action_idx = legal_actions.index(np.argmax(q_values))
-        probs[best_action_idx] += (1.0 - epsilon)
-        action_idx = np.random.choice(np.arange(len(probs)), p=probs)
+        if self._mode == 'best_response':
+            action = self._rl_agent.step(state)
+            one_hot = np.zeros(self._num_actions)
+            one_hot[action] = 1
+            self._add_transition(obs, one_hot)
+
+        elif self._mode == 'average_policy':
+            probs = self._act(obs)
+            probs = remove_illegal(probs, legal_actions)
+            action = np.random.choice(len(probs), p=probs)
 
-        return legal_actions[action_idx]
+        return action
 
     def eval_step(self, state):
-        ''' Predict the action for evaluation purpose.
+        ''' Use the average policy for evaluation purpose
 
         Args:
-            state (numpy.array): current state
+            state (dict): The current state.
 
         Returns:
-            action (int): an action id
+            action (int): An action id.
             info (dict): A dictionary containing information
         '''
-        q_values = self.predict(state)
-        best_action = np.argmax(q_values)
-
-        info = {}
-        info['values'] = {state['raw_legal_actions'][i]: float(q_values[list(state['legal_actions'].keys())[i]]) for i in range(len(state['legal_actions']))}
-
-        return best_action, info
+        if self.evaluate_with == 'best_response':
+            action, info = self._rl_agent.eval_step(state)
+        elif self.evaluate_with == 'average_policy':
+            obs = state['obs']
+            legal_actions = list(state['legal_actions'].keys())
+            probs = self._act(obs)
+            probs = remove_illegal(probs, legal_actions)
+            action = np.random.choice(len(probs), p=probs)
+            info = {}
+            info['probs'] = {state['raw_legal_actions'][i]: float(probs[list(state['legal_actions'].keys())[i]]) for i in range(len(state['legal_actions']))}
+        else:
+            raise ValueError("'evaluate_with' should be either 'average_policy' or 'best_response'.")
+        return action, info
 
-    def predict(self, state):
-        ''' Predict the masked Q-values
+    def sample_episode_policy(self):
+        ''' Sample average/best_response policy
+        '''
+        if np.random.rand() < self._anticipatory_param:
+            self._mode = 'best_response'
+        else:
+            self._mode = 'average_policy'
 
+    def _act(self, info_state):
+        ''' Predict action probability givin the observation and legal actions
+            Not connected to computation graph
         Args:
-            state (numpy.array): current state
+            info_state (numpy.array): An obervation.
 
         Returns:
-            q_values (numpy.array): a 1-d array where each entry represents a Q value
+            action_probs (numpy.array): The predicted action probability.
         '''
-        
-        q_values = self.q_estimator.predict_nograd(np.expand_dims(state['obs'], 0))[0]
-        masked_q_values = -np.inf * np.ones(self.num_actions, dtype=float)
-        legal_actions = list(state['legal_actions'].keys())
-        masked_q_values[legal_actions] = q_values[legal_actions]
+        info_state = np.expand_dims(info_state, axis=0)
+        info_state = torch.from_numpy(info_state).float().to(self.device)
 
-        return masked_q_values
+        with torch.no_grad():
+            log_action_probs = self.policy_network(info_state).cpu().numpy()
 
-    def train(self):
-        ''' Train the network
+        action_probs = np.exp(log_action_probs)[0]
 
-        Returns:
-            loss (float): The loss of the current batch.
-        '''
-        state_batch, action_batch, reward_batch, next_state_batch, done_batch, legal_actions_batch = self.memory.sample()
-
-        # Calculate best next actions using Q-network (Double DQN)
-        q_values_next = self.q_estimator.predict_nograd(next_state_batch)
-        legal_actions = []
-        for b in range(self.batch_size):
-            legal_actions.extend([i + b * self.num_actions for i in legal_actions_batch[b]])
-        masked_q_values = -np.inf * np.ones(self.num_actions * self.batch_size, dtype=float)
-        masked_q_values[legal_actions] = q_values_next.flatten()[legal_actions]
-        masked_q_values = masked_q_values.reshape((self.batch_size, self.num_actions))
-        best_actions = np.argmax(masked_q_values, axis=1)
-
-        # Evaluate best next actions using Target-network (Double DQN)
-        q_values_next_target = self.target_estimator.predict_nograd(next_state_batch)
-        target_batch = reward_batch + np.invert(done_batch).astype(np.float32) * \
-            self.discount_factor * q_values_next_target[np.arange(self.batch_size), best_actions]
-
-        # Perform gradient descent update
-        state_batch = np.array(state_batch)
-
-        loss = self.q_estimator.update(state_batch, action_batch, target_batch)
-        print('\rINFO - Step {}, rl-loss: {}'.format(self.total_t, loss), end='')
-
-        # Update the target estimator
-        if self.train_t % self.update_target_estimator_every == 0:
-            self.target_estimator = deepcopy(self.q_estimator)
-            print("\nINFO - Copied model parameters to target network.")
+        return action_probs
 
-        self.train_t += 1
+    def _add_transition(self, state, probs):
+        ''' Adds the new transition to the reservoir buffer.
 
-    def feed_memory(self, state, action, reward, next_state, legal_actions, done):
-        ''' Feed transition to memory
+        Transitions are in the form (state, probs).
 
         Args:
-            state (numpy.array): the current state
-            action (int): the performed action ID
-            reward (float): the reward received
-            next_state (numpy.array): the next state after performing the action
-            legal_actions (list): the legal actions of the next state
-            done (boolean): whether the episode is finished
+            state (numpy.array): The state.
+            probs (numpy.array): The probabilities of each action.
         '''
-        self.memory.save(state, action, reward, next_state, legal_actions, done)
-
-    def set_device(self, device):
-        self.device = device
-        self.q_estimator.device = device
-        self.target_estimator.device = device
-
-class Estimator(object):
-    '''
-    Approximate clone of rlcard.agents.dqn_agent.Estimator that
-    uses PyTorch instead of Tensorflow.  All methods input/output np.ndarray.
+        transition = Transition(
+                info_state=state,
+                action_probs=probs)
+        self._reservoir_buffer.add(transition)
 
-    Q-Value Estimator neural network.
-    This network is used for both the Q-Network and the Target Network.
-    '''
+    def train_sl(self):
+        ''' Compute the loss on sampled transitions and perform a avg-network update.
 
-    def __init__(self, num_actions=2, learning_rate=0.001, state_shape=None, mlp_layers=None, device=None):
-        ''' Initilalize an Estimator object.
+        If there are not enough elements in the buffer, no loss is computed and
+        `None` is returned instead.
 
-        Args:
-            num_actions (int): the number output actions
-            state_shape (list): the shape of the state space
-            mlp_layers (list): size of outputs of mlp layers
-            device (torch.device): whether to use cpu or gpu
+        Returns:
+            loss (float): The average loss obtained on this batch of transitions or `None`.
         '''
-        self.num_actions = num_actions
-        self.learning_rate=learning_rate
-        self.state_shape = state_shape
-        self.mlp_layers = mlp_layers
-        self.device = device
+        if (len(self._reservoir_buffer) < self._batch_size or
+                len(self._reservoir_buffer) < self._min_buffer_size_to_learn):
+            return None
 
-        # set up Q model and place it in eval mode
-        qnet = EstimatorNetwork(num_actions, state_shape, mlp_layers)
-        qnet = qnet.to(self.device)
-        self.qnet = qnet
-        self.qnet.eval()
+        transitions = self._reservoir_buffer.sample(self._batch_size)
+        info_states = [t.info_state for t in transitions]
+        action_probs = [t.action_probs for t in transitions]
 
-        # initialize the weights using Xavier init
-        for p in self.qnet.parameters():
-            if len(p.data.shape) > 1:
-                nn.init.xavier_uniform_(p.data)
+        self.policy_network_optimizer.zero_grad()
+        self.policy_network.train()
 
-        # set up loss function
-        self.mse_loss = nn.MSELoss(reduction='mean')
+        # (batch, state_size)
+        info_states = torch.from_numpy(np.array(info_states)).float().to(self.device)
 
-        # set up optimizer
-        self.optimizer =  torch.optim.Adam(self.qnet.parameters(), lr=self.learning_rate)
+        # (batch, num_actions)
+        eval_action_probs = torch.from_numpy(np.array(action_probs)).float().to(self.device)
 
-    def predict_nograd(self, s):
-        ''' Predicts action values, but prediction is not included
-            in the computation graph.  It is used to predict optimal next
-            actions in the Double-DQN algorithm.
-
-        Args:
-          s (np.ndarray): (batch, state_len)
-
-        Returns:
-          np.ndarray of shape (batch_size, NUM_VALID_ACTIONS) containing the estimated
-          action values.
-        '''
-        with torch.no_grad():
-            s = torch.from_numpy(s).float().to(self.device)
-            q_as = self.qnet(s).cpu().numpy()
-        return q_as
-
-    def update(self, s, a, y):
-        ''' Updates the estimator towards the given targets.
-            In this case y is the target-network estimated
-            value of the Q-network optimal actions, which
-            is labeled y in Algorithm 1 of Minh et al. (2015)
-
-        Args:
-          s (np.ndarray): (batch, state_shape) state representation
-          a (np.ndarray): (batch,) integer sampled actions
-          y (np.ndarray): (batch,) value of optimal actions according to Q-target
-
-        Returns:
-          The calculated loss on the batch.
-        '''
-        self.optimizer.zero_grad()
+        # (batch, num_actions)
+        log_forecast_action_probs = self.policy_network(info_states)
 
-        self.qnet.train()
+        ce_loss = - (eval_action_probs * log_forecast_action_probs).sum(dim=-1).mean()
+        ce_loss.backward()
 
-        s = torch.from_numpy(s).float().to(self.device)
-        a = torch.from_numpy(a).long().to(self.device)
-        y = torch.from_numpy(y).float().to(self.device)
+        self.policy_network_optimizer.step()
+        ce_loss = ce_loss.item()
+        self.policy_network.eval()
 
-        # (batch, state_shape) -> (batch, num_actions)
-        q_as = self.qnet(s)
-
-        # (batch, num_actions) -> (batch, )
-        Q = torch.gather(q_as, dim=-1, index=a.unsqueeze(-1)).squeeze(-1)
+        self.train_t += 1
 
-        # update model
-        batch_loss = self.mse_loss(Q, y)
-        batch_loss.backward()
-        self.optimizer.step()
-        batch_loss = batch_loss.item()
+        if self.save_path and self.train_t % self.save_every == 0:
+            # To preserve every checkpoint separately, 
+            # add another argument to the function call parameterized by self.train_t
+            self.save_checkpoint(self.save_path)
+            print("\nINFO - Saved model checkpoint.")
 
-        self.qnet.eval()
+        return ce_loss
 
-        return batch_loss
+    def set_device(self, device):
+        self.device = device
+        self._rl_agent.set_device(device)
+        
+    def checkpoint_attributes(self):
+        '''
+        Return the current checkpoint attributes (dict)
+        Checkpoint attributes are used to save and restore the model in the middle of training
+        Saves the model state dict, optimizer state dict, and all other instance variables
+        '''
+        
+        return {
+            'agent_type': 'NFSPAgent',
+            'policy_network': self.policy_network.checkpoint_attributes(),
+            'reservoir_buffer': self._reservoir_buffer.checkpoint_attributes(),
+            'rl_agent': self._rl_agent.checkpoint_attributes(),
+            'policy_network_optimizer': self.policy_network_optimizer.state_dict(),
+            'device': self.device,
+            'anticipatory_param': self._anticipatory_param,
+            'batch_size': self._batch_size,
+            'min_buffer_size_to_learn': self._min_buffer_size_to_learn,
+            'num_actions': self._num_actions,
+            'mode': self._mode,
+            'evaluate_with': self.evaluate_with,
+            'total_t': self.total_t,
+            'train_t': self.train_t,
+            'sl_learning_rate': self._sl_learning_rate,
+            'train_every': self._train_every,
+        }
+    
+    @classmethod
+    def from_checkpoint(cls, checkpoint):
+        '''
+        Restore the model from a checkpoint
+        
+        Args:
+            checkpoint (dict): the checkpoint attributes generated by checkpoint_attributes()
+        '''
+        print("\nINFO - Restoring model from checkpoint...")
+        agent = cls(
+            anticipatory_param=checkpoint['anticipatory_param'],
+            batch_size=checkpoint['batch_size'],
+            min_buffer_size_to_learn=checkpoint['min_buffer_size_to_learn'],
+            num_actions=checkpoint['num_actions'],
+            sl_learning_rate=checkpoint['sl_learning_rate'],
+            train_every=checkpoint['train_every'],
+            evaluate_with=checkpoint['evaluate_with'],
+            device=checkpoint['device'],
+            q_mlp_layers=checkpoint['rl_agent']['q_estimator']['mlp_layers'],
+            state_shape=checkpoint['rl_agent']['q_estimator']['state_shape'],
+            hidden_layers_sizes=[],
+        )
+        
+        agent.policy_network = AveragePolicyNetwork.from_checkpoint(checkpoint['policy_network'])
+        agent._reservoir_buffer = ReservoirBuffer.from_checkpoint(checkpoint['reservoir_buffer'])
+        agent._mode = checkpoint['mode']
+        agent.total_t = checkpoint['total_t']
+        agent.train_t = checkpoint['train_t']
+        agent.policy_network.to(agent.device)
+        agent.policy_network.eval()
+        agent.policy_network_optimizer = torch.optim.Adam(agent.policy_network.parameters(), lr=agent._sl_learning_rate)
+        agent.policy_network_optimizer.load_state_dict(checkpoint['policy_network_optimizer'])
+        agent._rl_agent.from_checkpoint(checkpoint['rl_agent'])
+        agent._rl_agent.set_device(agent.device)
+        return agent
+        
+    def save_checkpoint(self, path, filename='checkpoint_nfsp.pt'):
+        ''' Save the model checkpoint (all attributes)
 
+        Args:
+            path (str): the path to save the model
+        '''
+        torch.save(self.checkpoint_attributes(), path + '/' + filename)
+        
 
-class EstimatorNetwork(nn.Module):
-    ''' The function approximation network for Estimator
-        It is just a series of tanh layers. All in/out are torch.tensor
+class AveragePolicyNetwork(nn.Module):
+    '''
+    Approximates the history of action probabilities
+    given state (average policy). Forward pass returns
+    log probabilities of actions.
     '''
 
     def __init__(self, num_actions=2, state_shape=None, mlp_layers=None):
-        ''' Initialize the Q network
+        ''' Initialize the policy network.  It's just a bunch of ReLU
+        layers with no activation on the final one, initialized with
+        Xavier (sonnet.nets.MLP and tensorflow defaults)
 
         Args:
-            num_actions (int): number of legal actions
-            state_shape (list): shape of state tensor
-            mlp_layers (list): output size of each fc layer
+            num_actions (int): number of output actions
+            state_shape (list): shape of state tensor for each sample
+            mlp_laters (list): output size of each mlp layer including final
         '''
-        super(EstimatorNetwork, self).__init__()
+        super(AveragePolicyNetwork, self).__init__()
 
         self.num_actions = num_actions
         self.state_shape = state_shape
         self.mlp_layers = mlp_layers
 
-        # build the Q network
+        # set up mlp w/ relu activations
         layer_dims = [np.prod(self.state_shape)] + self.mlp_layers
-        fc = [nn.Flatten()]
-        fc.append(nn.BatchNorm1d(layer_dims[0]))
+        mlp = [nn.Flatten()]
+        mlp.append(nn.BatchNorm1d(layer_dims[0]))
         for i in range(len(layer_dims)-1):
-            fc.append(nn.Linear(layer_dims[i], layer_dims[i+1], bias=True))
-            fc.append(nn.Tanh())
-        fc.append(nn.Linear(layer_dims[-1], self.num_actions, bias=True))
-        self.fc_layers = nn.Sequential(*fc)
+            mlp.append(nn.Linear(layer_dims[i], layer_dims[i+1]))
+            if i != len(layer_dims) - 2: # all but final have relu
+                mlp.append(nn.ReLU())
+        self.mlp = nn.Sequential(*mlp)
 
     def forward(self, s):
-        ''' Predict action values
+        ''' Log action probabilities of each action from state
 
         Args:
-            s  (Tensor): (batch, state_shape)
+            s (Tensor): (batch, state_shape) state tensor
+
+        Returns:
+            log_action_probs (Tensor): (batch, num_actions)
+        '''
+        logits = self.mlp(s)
+        log_action_probs = F.log_softmax(logits, dim=-1)
+        return log_action_probs
+    
+    def checkpoint_attributes(self):
         '''
-        return self.fc_layers(s)
+        Return the current checkpoint attributes (dict)
+        Checkpoint attributes are used to save and restore the model in the middle of training
+        '''
+        
+        return {
+            'num_actions': self.num_actions,
+            'state_shape': self.state_shape,
+            'mlp_layers': self.mlp_layers,
+            'mlp': self.mlp.state_dict(),
+        }
+        
+    @classmethod
+    def from_checkpoint(cls, checkpoint):
+        '''
+        Restore the model from a checkpoint
+        
+        Args:
+            checkpoint (dict): the checkpoint attributes generated by checkpoint_attributes()
+        '''
+        
+        agent = cls(
+            num_actions=checkpoint['num_actions'],
+            state_shape=checkpoint['state_shape'],
+            mlp_layers=checkpoint['mlp_layers'],
+        )
+        
+        agent.mlp.load_state_dict(checkpoint['mlp'])
+        return agent
+
+class ReservoirBuffer(object):
+    ''' Allows uniform sampling over a stream of data.
+
+    This class supports the storage of arbitrary elements, such as observation
+    tensors, integer actions, etc.
 
-class Memory(object):
-    ''' Memory for saving transitions
+    See https://en.wikipedia.org/wiki/Reservoir_sampling for more details.
     '''
 
-    def __init__(self, memory_size, batch_size):
-        ''' Initialize
-        Args:
-            memory_size (int): the size of the memroy buffer
+    def __init__(self, reservoir_buffer_capacity):
+        ''' Initialize the buffer.
         '''
-        self.memory_size = memory_size
-        self.batch_size = batch_size
-        self.memory = []
+        self._reservoir_buffer_capacity = reservoir_buffer_capacity
+        self._data = []
+        self._add_calls = 0
 
-    def save(self, state, action, reward, next_state, legal_actions, done):
-        ''' Save transition into memory
+    def add(self, element):
+        ''' Potentially adds `element` to the reservoir buffer.
 
         Args:
-            state (numpy.array): the current state
-            action (int): the performed action ID
-            reward (float): the reward received
-            next_state (numpy.array): the next state after performing the action
-            legal_actions (list): the legal actions of the next state
-            done (boolean): whether the episode is finished
+            element (object): data to be added to the reservoir buffer.
         '''
-        if len(self.memory) == self.memory_size:
-            self.memory.pop(0)
-        transition = Transition(state, action, reward, next_state, done, legal_actions)
-        self.memory.append(transition)
+        if len(self._data) < self._reservoir_buffer_capacity:
+            self._data.append(element)
+        else:
+            idx = np.random.randint(0, self._add_calls + 1)
+            if idx < self._reservoir_buffer_capacity:
+                self._data[idx] = element
+        self._add_calls += 1
 
-    def sample(self):
-        ''' Sample a minibatch from the replay memory
+    def sample(self, num_samples):
+        ''' Returns `num_samples` uniformly sampled from the buffer.
+
+        Args:
+            num_samples (int): The number of samples to draw.
 
         Returns:
-            state_batch (list): a batch of states
-            action_batch (list): a batch of actions
-            reward_batch (list): a batch of rewards
-            next_state_batch (list): a batch of states
-            done_batch (list): a batch of dones
-        '''
-        samples = random.sample(self.memory, self.batch_size)
-        samples = tuple(zip(*samples))
-        return tuple(map(np.array, samples[:-1])) + (samples[-1],)
+            An iterable over `num_samples` random elements of the buffer.
+
+        Raises:
+            ValueError: If there are less than `num_samples` elements in the buffer
+        '''
+        if len(self._data) < num_samples:
+            raise ValueError("{} elements could not be sampled from size {}".format(
+                    num_samples, len(self._data)))
+        return random.sample(self._data, num_samples)
+
+    def clear(self):
+        ''' Clear the buffer
+        '''
+        self._data = []
+        self._add_calls = 0
+        
+    def checkpoint_attributes(self):
+        return {
+            'data': self._data,
+            'add_calls': self._add_calls,
+            'reservoir_buffer_capacity': self._reservoir_buffer_capacity,
+        }
+        
+    @classmethod
+    def from_checkpoint(cls, checkpoint):
+        reservoir_buffer = cls(checkpoint['reservoir_buffer_capacity'])
+        reservoir_buffer._data = checkpoint['data']
+        reservoir_buffer._add_calls = checkpoint['add_calls']
+        return reservoir_buffer
+
+    def __len__(self):
+        return len(self._data)
+
+    def __iter__(self):
+        return iter(self._data)
+
```

### Comparing `rlcard-1.1.0/rlcard/agents/human_agents/blackjack_human_agent.py` & `rlcard-1.2.0/rlcard/agents/human_agents/blackjack_human_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
         Returns:
             action (int): The action decided by human
         '''
         _print_state(state['raw_obs'], state['raw_legal_actions'], state['action_record'])
         action = int(input('>> You choose action (integer): '))
         while action < 0 or action >= len(state['legal_actions']):
-            print('Action illegel...')
+            print('Action illegal...')
             action = int(input('>> Re-choose action (integer): '))
         return state['raw_legal_actions'][action]
 
     def eval_step(self, state):
         ''' Predict the action given the current state for evaluation. The same to step here.
 
         Args:
```

### Comparing `rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gin_rummy_human_agent.py` & `rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gin_rummy_human_agent.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_cards/card_image.py` & `rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_cards/card_image.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/canvas_item.py` & `rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/canvas_item.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/configurations.py` & `rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/configurations.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/env_thread.py` & `rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/env_thread.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/game_app.py` & `rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/game_app.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/game_canvas.py` & `rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/game_canvas.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/game_canvas_debug.py` & `rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/game_canvas_debug.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/game_canvas_getter.py` & `rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/game_canvas_getter.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/game_canvas_post_doing_action.py` & `rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/game_canvas_post_doing_action.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/game_canvas_query.py` & `rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/game_canvas_query.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/game_canvas_updater.py` & `rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/game_canvas_updater.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/game_frame.py` & `rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/game_frame.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/handling_tap.py` & `rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/handling_tap.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/handling_tap_discard_pile.py` & `rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/handling_tap_discard_pile.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/handling_tap_held_pile.py` & `rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/handling_tap_held_pile.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/handling_tap_player_pane.py` & `rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/handling_tap_player_pane.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/handling_tap_stock_pile.py` & `rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/handling_tap_stock_pile.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/handling_tap_to_arrange_held_pile.py` & `rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/handling_tap_to_arrange_held_pile.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/info_messaging.py` & `rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/info_messaging.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/menu_bar.py` & `rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/menu_bar.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/preferences_window.py` & `rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/preferences_window.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/starting_new_game.py` & `rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/starting_new_game.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/status_messaging.py` & `rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/status_messaging.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/utils.py` & `rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/utils.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/utils_extra.py` & `rlcard-1.2.0/rlcard/agents/human_agents/gin_rummy_human_agent/gui_gin_rummy/utils_extra.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/agents/human_agents/leduc_holdem_human_agent.py` & `rlcard-1.2.0/rlcard/agents/human_agents/leduc_holdem_human_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
         Returns:
             action (int): The action decided by human
         '''
         _print_state(state['raw_obs'], state['action_record'])
         action = int(input('>> You choose action (integer): '))
         while action < 0 or action >= len(state['legal_actions']):
-            print('Action illegel...')
+            print('Action illegal...')
             action = int(input('>> Re-choose action (integer): '))
         return state['raw_legal_actions'][action]
 
     def eval_step(self, state):
         ''' Predict the action given the curent state for evaluation. The same to step here.
 
         Args:
```

### Comparing `rlcard-1.1.0/rlcard/agents/human_agents/limit_holdem_human_agent.py` & `rlcard-1.2.0/rlcard/agents/human_agents/limit_holdem_human_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
         Returns:
             action (int): The action decided by human
         '''
         _print_state(state['raw_obs'], state['action_record'])
         action = int(input('>> You choose action (integer): '))
         while action < 0 or action >= len(state['legal_actions']):
-            print('Action illegel...')
+            print('Action illegal...')
             action = int(input('>> Re-choose action (integer): '))
         return state['raw_legal_actions'][action]
 
     def eval_step(self, state):
         ''' Predict the action given the curent state for evaluation. The same to step here.
 
         Args:
```

### Comparing `rlcard-1.1.0/rlcard/agents/human_agents/nolimit_holdem_human_agent.py` & `rlcard-1.2.0/rlcard/agents/human_agents/nolimit_holdem_human_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
         Returns:
             action (int): The action decided by human
         '''
         _print_state(state['raw_obs'], state['action_record'])
         action = int(input('>> You choose action (integer): '))
         while action < 0 or action >= len(state['legal_actions']):
-            print('Action illegel...')
+            print('Action illegal...')
             action = int(input('>> Re-choose action (integer): '))
         return state['raw_legal_actions'][action]
 
     def eval_step(self, state):
         ''' Predict the action given the curent state for evaluation. The same to step here.
 
         Args:
```

### Comparing `rlcard-1.1.0/rlcard/agents/human_agents/uno_human_agent.py` & `rlcard-1.2.0/rlcard/agents/human_agents/uno_human_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         Returns:
             action (int): The action decided by human
         '''
         print(state['raw_obs'])
         _print_state(state['raw_obs'], state['action_record'])
         action = int(input('>> You choose action (integer): '))
         while action < 0 or action >= len(state['legal_actions']):
-            print('Action illegel...')
+            print('Action illegal...')
             action = int(input('>> Re-choose action (integer): '))
         return state['raw_legal_actions'][action]
 
     def eval_step(self, state):
         ''' Predict the action given the curent state for evaluation. The same to step here.
 
         Args:
```

### Comparing `rlcard-1.1.0/rlcard/agents/pettingzoo_agents.py` & `rlcard-1.2.0/rlcard/agents/pettingzoo_agents.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/agents/random_agent.py` & `rlcard-1.2.0/rlcard/agents/random_agent.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/envs/__init__.py` & `rlcard-1.2.0/rlcard/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/envs/blackjack.py` & `rlcard-1.2.0/rlcard/envs/blackjack.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/envs/bridge.py` & `rlcard-1.2.0/rlcard/envs/bridge.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,17 +230,17 @@
 
         # construct hidden_card_rep (during trick taking phase)
         hidden_cards_rep = np.zeros(52, dtype=int)
         if not game.is_over():
             if game.round.is_bidding_over():
                 declarer = game.round.get_declarer()
                 if current_player_id % 2 == declarer.player_id % 2:
-                    hidden_player_ids = [(current_player_id + 1) % 2, (current_player_id + 3) % 2]
+                    hidden_player_ids = [(current_player_id + 1) % 4, (current_player_id + 3) % 4]
                 else:
-                    hidden_player_ids = [declarer.player_id, (current_player_id + 2) % 2]
+                    hidden_player_ids = [declarer.player_id, (current_player_id + 2) % 4]
                 for hidden_player_id in hidden_player_ids:
                     for card in game.round.players[hidden_player_id].hand:
                         hidden_cards_rep[card.card_id] = 1
             else:
                 for player in game.round.players:
                     if player.player_id != current_player_id:
                         for card in player.hand:
```

### Comparing `rlcard-1.1.0/rlcard/envs/doudizhu.py` & `rlcard-1.2.0/rlcard/envs/doudizhu.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/envs/env.py` & `rlcard-1.2.0/rlcard/envs/env.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/envs/gin_rummy.py` & `rlcard-1.2.0/rlcard/envs/gin_rummy.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/envs/leducholdem.py` & `rlcard-1.2.0/rlcard/envs/leducholdem.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/envs/limitholdem.py` & `rlcard-1.2.0/rlcard/envs/limitholdem.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/envs/mahjong.py` & `rlcard-1.2.0/rlcard/envs/mahjong.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/envs/nolimitholdem.py` & `rlcard-1.2.0/rlcard/envs/nolimitholdem.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/envs/registration.py` & `rlcard-1.2.0/rlcard/envs/registration.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/envs/uno.py` & `rlcard-1.2.0/rlcard/envs/uno.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/base.py` & `rlcard-1.2.0/rlcard/games/base.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/blackjack/dealer.py` & `rlcard-1.2.0/rlcard/games/blackjack/dealer.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/blackjack/game.py` & `rlcard-1.2.0/rlcard/games/blackjack/game.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/blackjack/judger.py` & `rlcard-1.2.0/rlcard/games/blackjack/judger.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/bridge/dealer.py` & `rlcard-1.2.0/rlcard/games/bridge/dealer.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/bridge/game.py` & `rlcard-1.2.0/rlcard/games/bridge/game.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/bridge/judger.py` & `rlcard-1.2.0/rlcard/games/bridge/judger.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/bridge/player.py` & `rlcard-1.2.0/rlcard/games/bridge/player.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/bridge/round.py` & `rlcard-1.2.0/rlcard/games/bridge/round.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/bridge/utils/action_event.py` & `rlcard-1.2.0/rlcard/games/bridge/utils/action_event.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/bridge/utils/bridge_card.py` & `rlcard-1.2.0/rlcard/games/bridge/utils/bridge_card.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/bridge/utils/move.py` & `rlcard-1.2.0/rlcard/games/bridge/utils/move.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/bridge/utils/tray.py` & `rlcard-1.2.0/rlcard/games/bridge/utils/tray.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/doudizhu/dealer.py` & `rlcard-1.2.0/rlcard/games/doudizhu/dealer.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/doudizhu/game.py` & `rlcard-1.2.0/rlcard/games/doudizhu/game.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/doudizhu/jsondata.zip` & `rlcard-1.2.0/rlcard/games/doudizhu/jsondata.zip`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/doudizhu/judger.py` & `rlcard-1.2.0/rlcard/games/doudizhu/judger.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/doudizhu/player.py` & `rlcard-1.2.0/rlcard/games/doudizhu/player.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/doudizhu/round.py` & `rlcard-1.2.0/rlcard/games/doudizhu/round.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/doudizhu/utils.py` & `rlcard-1.2.0/rlcard/games/doudizhu/utils.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/gin_rummy/dealer.py` & `rlcard-1.2.0/rlcard/games/gin_rummy/dealer.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/gin_rummy/game.py` & `rlcard-1.2.0/rlcard/games/gin_rummy/game.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         '''
         return self.round.is_over
 
     def get_current_player(self) -> GinRummyPlayer or None:
         return self.round.get_current_player()
 
     def get_last_action(self) -> ActionEvent or None:
-        return None if len(self.actions) == 0 else self.actions[-1]
+        return self.actions[-1] if self.actions and len(self.actions) > 0 else None
 
     def get_state(self, player_id: int):
         ''' Get player's state
 
         Return:
             state (dict): The information of the state
         '''
```

### Comparing `rlcard-1.1.0/rlcard/games/gin_rummy/judge.py` & `rlcard-1.2.0/rlcard/games/gin_rummy/judge.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/gin_rummy/player.py` & `rlcard-1.2.0/rlcard/games/gin_rummy/player.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/gin_rummy/round.py` & `rlcard-1.2.0/rlcard/games/gin_rummy/round.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/gin_rummy/utils/action_event.py` & `rlcard-1.2.0/rlcard/games/gin_rummy/utils/action_event.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/gin_rummy/utils/melding.py` & `rlcard-1.2.0/rlcard/games/gin_rummy/utils/melding.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/gin_rummy/utils/move.py` & `rlcard-1.2.0/rlcard/games/gin_rummy/utils/move.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/gin_rummy/utils/scorers.py` & `rlcard-1.2.0/rlcard/games/gin_rummy/utils/scorers.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/gin_rummy/utils/settings.py` & `rlcard-1.2.0/rlcard/games/gin_rummy/utils/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 '''
 
 from typing import Dict, Any
 
 from enum import Enum
 
 
-class DealerForRound(Enum):
+class DealerForRound(int, Enum):
     North = 0
     South = 1
     Random = 2
 
 
-class Setting(Enum):
+class Setting(str, Enum):
     dealer_for_round = "dealer_for_round"
     stockpile_dead_card_count = "stockpile_dead_card_count"
     going_out_deadwood_count = "going_out_deadwood_count"
     max_drawn_card_count = "max_drawn_card_count"
     max_move_count = "max_move_count"
     is_allowed_knock = "is_allowed_knock"
     is_allowed_gin = "is_allowed_gin"
```

### Comparing `rlcard-1.1.0/rlcard/games/gin_rummy/utils/thinker.py` & `rlcard-1.2.0/rlcard/games/gin_rummy/utils/thinker.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/gin_rummy/utils/utils.py` & `rlcard-1.2.0/rlcard/games/gin_rummy/utils/utils.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/leducholdem/game.py` & `rlcard-1.2.0/rlcard/games/leducholdem/game.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/leducholdem/judger.py` & `rlcard-1.2.0/rlcard/games/leducholdem/judger.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/leducholdem/player.py` & `rlcard-1.2.0/rlcard/games/leducholdem/player.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/leducholdem/round.py` & `rlcard-1.2.0/rlcard/games/leducholdem/round.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/limitholdem/game.py` & `rlcard-1.2.0/rlcard/games/limitholdem/game.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/limitholdem/judger.py` & `rlcard-1.2.0/rlcard/games/limitholdem/judger.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/limitholdem/player.py` & `rlcard-1.2.0/rlcard/games/limitholdem/player.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/limitholdem/round.py` & `rlcard-1.2.0/rlcard/games/limitholdem/round.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/limitholdem/utils.py` & `rlcard-1.2.0/rlcard/games/limitholdem/utils.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/mahjong/card.py` & `rlcard-1.2.0/rlcard/games/mahjong/card.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/mahjong/dealer.py` & `rlcard-1.2.0/rlcard/games/mahjong/dealer.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/mahjong/game.py` & `rlcard-1.2.0/rlcard/games/mahjong/game.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/mahjong/judger.py` & `rlcard-1.2.0/rlcard/games/mahjong/judger.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/mahjong/player.py` & `rlcard-1.2.0/rlcard/games/mahjong/player.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/mahjong/round.py` & `rlcard-1.2.0/rlcard/games/mahjong/round.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/mahjong/utils.py` & `rlcard-1.2.0/rlcard/games/mahjong/utils.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/nolimitholdem/game.py` & `rlcard-1.2.0/rlcard/games/nolimitholdem/game.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/nolimitholdem/player.py` & `rlcard-1.2.0/rlcard/games/nolimitholdem/player.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/nolimitholdem/round.py` & `rlcard-1.2.0/rlcard/games/nolimitholdem/round.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/uno/card.py` & `rlcard-1.2.0/rlcard/games/uno/card.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/uno/dealer.py` & `rlcard-1.2.0/rlcard/games/uno/dealer.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/uno/game.py` & `rlcard-1.2.0/rlcard/games/uno/game.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/uno/jsondata/action_space.json` & `rlcard-1.2.0/rlcard/games/uno/jsondata/action_space.json`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/uno/judger.py` & `rlcard-1.2.0/rlcard/games/uno/judger.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/games/uno/round.py` & `rlcard-1.2.0/rlcard/games/uno/round.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,32 +48,33 @@
             self.direction = -1
             self.current_player = (0 + self.direction) % self.num_players
         elif top_card.trait == 'draw_2':
             player = players[self.current_player]
             self.dealer.deal_cards(player, 2)
 
     def proceed_round(self, players, action):
-        ''' Call other Classes's functions to keep one round running
+        ''' Call other Classes' functions to keep one round running
 
         Args:
             player (object): object of UnoPlayer
             action (str): string of legal action
         '''
         if action == 'draw':
             self._perform_draw_action(players)
             return None
         player = players[self.current_player]
         card_info = action.split('-')
         color = card_info[0]
         trait = card_info[1]
-        # remove correspongding card
+        # remove corresponding card
         remove_index = None
         if trait == 'wild' or trait == 'wild_draw_4':
             for index, card in enumerate(player.hand):
                 if trait == card.trait:
+                    card.color = color # update the color of wild card to match the action
                     remove_index = index
                     break
         else:
             for index, card in enumerate(player.hand):
                 if color == card.color and trait == card.trait:
                     remove_index = index
                     break
```

### Comparing `rlcard-1.1.0/rlcard/games/uno/utils.py` & `rlcard-1.2.0/rlcard/games/uno/utils.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/models/__init__.py` & `rlcard-1.2.0/rlcard/models/__init__.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/models/bridge_rule_models.py` & `rlcard-1.2.0/rlcard/models/bridge_rule_models.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/models/doudizhu_rule_models.py` & `rlcard-1.2.0/rlcard/models/doudizhu_rule_models.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/models/gin_rummy_rule_models.py` & `rlcard-1.2.0/rlcard/models/gin_rummy_rule_models.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/models/leducholdem_rule_models.py` & `rlcard-1.2.0/rlcard/models/leducholdem_rule_models.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/models/limitholdem_rule_models.py` & `rlcard-1.2.0/rlcard/models/limitholdem_rule_models.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/models/pretrained/leduc_holdem_cfr/average_policy.pkl` & `rlcard-1.2.0/rlcard/models/pretrained/leduc_holdem_cfr/average_policy.pkl`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/models/pretrained/leduc_holdem_cfr/policy.pkl` & `rlcard-1.2.0/rlcard/models/pretrained/leduc_holdem_cfr/policy.pkl`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/models/pretrained/leduc_holdem_cfr/regrets.pkl` & `rlcard-1.2.0/rlcard/models/pretrained/leduc_holdem_cfr/regrets.pkl`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/models/pretrained_models.py` & `rlcard-1.2.0/rlcard/models/pretrained_models.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/models/registration.py` & `rlcard-1.2.0/rlcard/models/registration.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/models/uno_rule_models.py` & `rlcard-1.2.0/rlcard/models/uno_rule_models.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/utils/logger.py` & `rlcard-1.2.0/rlcard/utils/logger.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/utils/pettingzoo_utils.py` & `rlcard-1.2.0/rlcard/utils/pettingzoo_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     return wrapped_state
 
 
 def run_game_pettingzoo(env, agents, is_training=False):
     env.reset()
     trajectories = defaultdict(list)
     for agent_name in env.agent_iter():
-        obs, reward, done, _ = env.last()
+        obs, reward, done, _, _ = env.last()
         trajectories[agent_name].append((obs, reward, done))
 
         if done:
             action = None
         else:
             if is_training:
                 action = agents[agent_name].step(obs)
```

### Comparing `rlcard-1.1.0/rlcard/utils/seeding.py` & `rlcard-1.2.0/rlcard/utils/seeding.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard/utils/utils.py` & `rlcard-1.2.0/rlcard/utils/utils.py`

 * *Files identical despite different names*

### Comparing `rlcard-1.1.0/rlcard.egg-info/SOURCES.txt` & `rlcard-1.2.0/rlcard.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.md
 README.md
 setup.py
 rlcard/__init__.py
 rlcard.egg-info/PKG-INFO
 rlcard.egg-info/SOURCES.txt
 rlcard.egg-info/dependency_links.txt
 rlcard.egg-info/requires.txt
```

### Comparing `rlcard-1.1.0/setup.py` & `rlcard-1.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     install_requires=[
         'numpy>=1.16.3',
         'termcolor'
     ],
     extras_require=extras,
     requires_python='>=3.7',
     classifiers=[
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.7",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```


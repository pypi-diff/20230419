# Comparing `tmp/pokerrl_env-0.1.1.tar.gz` & `tmp/pokerrl_env-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokerrl_env-0.1.1.tar", max compression
+gzip compressed data, was "pokerrl_env-0.1.2.tar", max compression
```

## Comparing `pokerrl_env-0.1.1.tar` & `pokerrl_env-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0     2899 2023-04-18 23:30:10.137034 pokerrl_env-0.1.1/README.md
--rw-r--r--   0        0        0      320 2023-04-17 18:11:46.664658 pokerrl_env-0.1.1/pokerrl_env/__init__.py
--rw-r--r--   0        0        0     2807 2023-04-17 05:05:22.329945 pokerrl_env-0.1.1/pokerrl_env/cardlib.py
--rw-r--r--   0        0        0     6102 2023-04-18 01:17:39.065416 pokerrl_env-0.1.1/pokerrl_env/config.py
--rw-r--r--   0        0        0     3991 2023-04-18 03:31:27.573583 pokerrl_env-0.1.1/pokerrl_env/datatypes.py
--rw-r--r--   0        0        0     1576 2023-04-19 03:49:06.659495 pokerrl_env-0.1.1/pokerrl_env/game.py
--rw-r--r--   0        0        0        0 2023-04-19 02:40:47.094863 pokerrl_env-0.1.1/pokerrl_env/gpt.pr
--rw-r--r--   0        0        0     1688 2023-04-17 07:06:58.855019 pokerrl_env-0.1.1/pokerrl_env/play.py
--rw-r--r--   0        0        0     5510 2023-04-19 01:39:25.633002 pokerrl_env-0.1.1/pokerrl_env/test_pots.py
--rw-r--r--   0        0        0    40412 2023-04-19 03:49:25.710551 pokerrl_env-0.1.1/pokerrl_env/test_transition.py
--rw-r--r--   0        0        0     3768 2023-04-19 03:49:32.524122 pokerrl_env-0.1.1/pokerrl_env/test_utils.py
--rw-r--r--   0        0        0     2638 2023-04-19 03:49:37.391376 pokerrl_env-0.1.1/pokerrl_env/test_view.py
--rw-r--r--   0        0        0    20881 2023-04-19 03:49:44.138919 pokerrl_env-0.1.1/pokerrl_env/transition.py
--rw-r--r--   0        0        0     7615 2023-04-19 03:49:49.060973 pokerrl_env-0.1.1/pokerrl_env/utils.py
--rw-r--r--   0        0        0     9600 2023-04-19 03:49:59.757293 pokerrl_env-0.1.1/pokerrl_env/view.py
--rw-r--r--   0        0        0      420 2023-04-19 03:51:15.746069 pokerrl_env-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3693 1970-01-01 00:00:00.000000 pokerrl_env-0.1.1/setup.py
--rw-r--r--   0        0        0     3532 1970-01-01 00:00:00.000000 pokerrl_env-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2899 2023-04-18 23:30:10.137034 pokerrl_env-0.1.2/README.md
+-rw-r--r--   0        0        0      320 2023-04-17 18:11:46.664658 pokerrl_env-0.1.2/pokerrl_env/__init__.py
+-rw-r--r--   0        0        0     2807 2023-04-17 05:05:22.329945 pokerrl_env-0.1.2/pokerrl_env/cardlib.py
+-rw-r--r--   0        0        0     6110 2023-04-19 03:53:03.460415 pokerrl_env-0.1.2/pokerrl_env/config.py
+-rw-r--r--   0        0        0     3991 2023-04-18 03:31:27.573583 pokerrl_env-0.1.2/pokerrl_env/datatypes.py
+-rw-r--r--   0        0        0     1576 2023-04-19 03:49:06.659495 pokerrl_env-0.1.2/pokerrl_env/game.py
+-rw-r--r--   0        0        0     1708 2023-04-19 03:53:06.134910 pokerrl_env-0.1.2/pokerrl_env/play.py
+-rw-r--r--   0        0        0     5526 2023-04-19 03:53:10.412765 pokerrl_env-0.1.2/pokerrl_env/test_pots.py
+-rw-r--r--   0        0        0    40412 2023-04-19 03:49:25.710551 pokerrl_env-0.1.2/pokerrl_env/test_transition.py
+-rw-r--r--   0        0        0     3768 2023-04-19 03:49:32.524122 pokerrl_env-0.1.2/pokerrl_env/test_utils.py
+-rw-r--r--   0        0        0     2638 2023-04-19 03:49:37.391376 pokerrl_env-0.1.2/pokerrl_env/test_view.py
+-rw-r--r--   0        0        0    20881 2023-04-19 03:49:44.138919 pokerrl_env-0.1.2/pokerrl_env/transition.py
+-rw-r--r--   0        0        0     7615 2023-04-19 03:49:49.060973 pokerrl_env-0.1.2/pokerrl_env/utils.py
+-rw-r--r--   0        0        0     9600 2023-04-19 03:49:59.757293 pokerrl_env-0.1.2/pokerrl_env/view.py
+-rw-r--r--   0        0        0      420 2023-04-19 03:54:29.401867 pokerrl_env-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3693 1970-01-01 00:00:00.000000 pokerrl_env-0.1.2/setup.py
+-rw-r--r--   0        0        0     3532 1970-01-01 00:00:00.000000 pokerrl_env-0.1.2/PKG-INFO
```

### Comparing `pokerrl_env-0.1.1/README.md` & `pokerrl_env-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pokerrl_env-0.1.1/pokerrl_env/cardlib.py` & `pokerrl_env-0.1.2/pokerrl_env/cardlib.py`

 * *Files identical despite different names*

### Comparing `pokerrl_env-0.1.1/pokerrl_env/config.py` & `pokerrl_env-0.1.2/pokerrl_env/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from pokerrl.datatypes import CALL, CHECK, FOLD, INT_POSITIONS_BY_NUM_PLAYERS, PREFLOP_ORDER_BY_NUM_PLAYERS, POSITION_TO_SEAT, PLAYERS_POSITIONS_DICT, BetLimits, GameTypes, Street
-from pokerrl.utils import calculate_fixed_limit_mask, calculate_no_limit_betsize, calculate_pot_limit_betsize, calculate_pot_limit_mask, calculate_no_limit_mask, return_deck
+from pokerrl_env.datatypes import CALL, CHECK, FOLD, INT_POSITIONS_BY_NUM_PLAYERS, PREFLOP_ORDER_BY_NUM_PLAYERS, POSITION_TO_SEAT, PLAYERS_POSITIONS_DICT, BetLimits, GameTypes, Street
+from pokerrl_env.utils import calculate_fixed_limit_mask, calculate_no_limit_betsize, calculate_pot_limit_betsize, calculate_pot_limit_mask, calculate_no_limit_mask, return_deck
 
 class Config:
     def __init__(self, game_type=GameTypes.OMAHA_HI, num_players=2, bet_limit=BetLimits.POT_LIMIT,
                  betsizes=(1, 0.9, 0.75, 0.67, 0.5, 0.33, 0.25, 0.1),
                  blinds=(0.5,1), stack_sizes=100,is_server=False):
         assert num_players >= 2, "Number of players must be at least 2"
         assert bet_limit in [BetLimits.POT_LIMIT, BetLimits.NO_LIMIT, BetLimits.FIXED_LIMIT], "Bet limit must be one of Pot limit, No limit, or Fixed limit"
```

### Comparing `pokerrl_env-0.1.1/pokerrl_env/datatypes.py` & `pokerrl_env-0.1.2/pokerrl_env/datatypes.py`

 * *Files identical despite different names*

### Comparing `pokerrl_env-0.1.1/pokerrl_env/game.py` & `pokerrl_env-0.1.2/pokerrl_env/game.py`

 * *Files identical despite different names*

### Comparing `pokerrl_env-0.1.1/pokerrl_env/play.py` & `pokerrl_env-0.1.2/pokerrl_env/play.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from pokerrl.config import Config
-from pokerrl.datatypes import StateActions
-from pokerrl.utils import return_current_player
-from pokerrl.view import player_view, human_readable_view
-from pokerrl.transition import step_state,init_state
+from pokerrl_env.config import Config
+from pokerrl_env.datatypes import StateActions
+from pokerrl_env.utils import return_current_player
+from pokerrl_env.view import player_view, human_readable_view
+from pokerrl_env.transition import step_state,init_state
 
 def get_action(action_mask,global_states,config):
     readable_actions = ['FOLD','CHECK','CALL']
     if global_states[-1,config.global_state_mapping['last_agro_action']] > StateActions.CALL:
         agro_action = 'RAISE'
     else:
         agro_action = 'BET'
```

### Comparing `pokerrl_env-0.1.1/pokerrl_env/test_pots.py` & `pokerrl_env-0.1.2/pokerrl_env/test_pots.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from pokerrl.utils import readable_card_to_int
+from pokerrl_env.utils import readable_card_to_int
 import pytest
 import numpy as np
 from typing import List, Tuple, Dict
-from pokerrl.config import Config
-from pokerrl.datatypes import Player, Street
-from pokerrl.transition import get_pots, calculate_winnings, game_over
+from pokerrl_env.config import Config
+from pokerrl_env.datatypes import Player, Street
+from pokerrl_env.transition import get_pots, calculate_winnings, game_over
 
 @pytest.fixture
 def example_players():
     return [
         Player(1, 100, 1, [8, 14], 5, 100),
         Player(2, 0, 1, [4, 5], 3, 50),
         Player(3, 150, 1, [12, 9], 5, 100)
```

### Comparing `pokerrl_env-0.1.1/pokerrl_env/test_transition.py` & `pokerrl_env-0.1.2/pokerrl_env/test_transition.py`

 * *Files identical despite different names*

### Comparing `pokerrl_env-0.1.1/pokerrl_env/test_utils.py` & `pokerrl_env-0.1.2/pokerrl_env/test_utils.py`

 * *Files identical despite different names*

### Comparing `pokerrl_env-0.1.1/pokerrl_env/test_view.py` & `pokerrl_env-0.1.2/pokerrl_env/test_view.py`

 * *Files identical despite different names*

### Comparing `pokerrl_env-0.1.1/pokerrl_env/transition.py` & `pokerrl_env-0.1.2/pokerrl_env/transition.py`

 * *Files identical despite different names*

### Comparing `pokerrl_env-0.1.1/pokerrl_env/utils.py` & `pokerrl_env-0.1.2/pokerrl_env/utils.py`

 * *Files identical despite different names*

### Comparing `pokerrl_env-0.1.1/pokerrl_env/view.py` & `pokerrl_env-0.1.2/pokerrl_env/view.py`

 * *Files identical despite different names*

### Comparing `pokerrl_env-0.1.1/setup.py` & `pokerrl_env-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['numpy>=1.19.5,<2.0.0',
  'pytest>=6.2.4,<7.0.0',
  'setuptools-rust>=1.5.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'pokerrl-env',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'A poker environment for reinforcement learning',
     'long_description': "# Poker environment for reinforcement learning\n\nTo instantiate the environment, pass in the config.\n\nthe config consists of the following parameters:\n\n- number of players (2-6), default 2\n- bet limit (fixed limit, no limit, pot limit), default pot limit\n- bet sizes allowed (array of floats), default (1, 0.9, 0.75, 0.67, 0.5, 0.33, 0.25, 0.1)\n- Game type [Holdem, OmahaHI], default OmahaHI\n\n## Example usage\n\nThis is the recommended way to use the environment.\n\n```\nfrom pokerrl import Config, Game\n\nconfig = Config(\n    num_players=2,\n    bet_limit=BetLimits.POT_LIMIT,\n    bet_sizes=[1, 0.5],\n    game_type=GameTypes.OMAHA_HI,\n)\ngame = Game(config)\nplayer_state,done,winnings,action_mask = game.reset()\nwhile not done:\n  action = model(player_state)\n  player_state,done,winnings,action_mask = game.step(action)\n```\n\n## Play a game (both sides)\n\n```\nfrom pokerrl import play_game\nplay_game()\n```\n\n## Example usage (low level)\n\n```\nfrom pokerrl import Config, init_state, step_state, GameTypes, BetLimits, player_view, Positions, get_current_player\n\nconfig = Config(\n    num_players=2,\n    bet_limit=BetLimits.POT_LIMIT,\n    bet_sizes=[1, 0.5],\n    game_type=GameTypes.OMAHA_HI,\n)\nglobal_state,done,winnings,action_mask = init_state(config)\nwhile not done:\n  player_idx = get_current_player(global_state)\n  player_state = player_view(global_state, player_idx)\n  action = model(player_state)\n  global_state,done,winnings,action_mask = step_state(global_state, action, config)\n```\n\n## Player view (low level)\n\n```\nfrom pokerrl import Config, init_state, step_state, GameTypes, BetLimits, player_view, Positions, get_current_player\n\nconfig = Config()\nglobal_state,done,winnings,action_mask = init_state(config)\nwhile not done:\n  player_idx = get_current_player(global_state)\n  human_readable_view(global_state,player_idx, config)\n  action = get_action(action_mask,global_state,config)\n  global_state,done,winnings,action_mask = step_state(global_state, action, config)\n```\n\n## State\n\nThe state is an array. To get a player's view of the state, pass the state into the view with the appropriate player index.\n\n## Design decisions\n\n- Record the total amount raised.\n  If you record the actual amount raised this means its more difficult to tell what the raise size is when facing multiple raises. But easier to tell what the raise size is when facing a single raise. Also complicates the process of determining how much a player has to call, as the raise size is in relation to the previous bet, which in multiplayer games, is not necessarily us.\n- Global state player numbers are identical to their position.\n- SB and BB posts are the first two states.\n\n- A raise is the total amount. Subtract player street total\n- A call vs a raise is the difference = villain bet - player street total\n- A call vs a bet is the full amount = villain bet - player street total\n- A bet is the full amount\n- A fold is 0\n",
     'author': 'Morgan Griffiths',
     'author_email': 'rareducks101@yahoo.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pokerrl_env-0.1.1/PKG-INFO` & `pokerrl_env-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pokerrl-env
-Version: 0.1.1
+Version: 0.1.2
 Summary: A poker environment for reinforcement learning
 License: MIT
 Author: Morgan Griffiths
 Author-email: rareducks101@yahoo.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


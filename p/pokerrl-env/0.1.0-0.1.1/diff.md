# Comparing `tmp/pokerrl_env-0.1.0.tar.gz` & `tmp/pokerrl_env-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokerrl_env-0.1.0.tar", max compression
+gzip compressed data, was "pokerrl_env-0.1.1.tar", max compression
```

## Comparing `pokerrl_env-0.1.0.tar` & `pokerrl_env-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     2899 2023-04-18 23:30:10.137034 pokerrl_env-0.1.0/README.md
--rw-r--r--   0        0        0      320 2023-04-17 18:11:46.664658 pokerrl_env-0.1.0/pokerrl_env/__init__.py
--rw-r--r--   0        0        0     2807 2023-04-17 05:05:22.329945 pokerrl_env-0.1.0/pokerrl_env/cardlib.py
--rw-r--r--   0        0        0     6102 2023-04-18 01:17:39.065416 pokerrl_env-0.1.0/pokerrl_env/config.py
--rw-r--r--   0        0        0     3991 2023-04-18 03:31:27.573583 pokerrl_env-0.1.0/pokerrl_env/datatypes.py
--rw-r--r--   0        0        0     1560 2023-04-17 20:38:46.252196 pokerrl_env-0.1.0/pokerrl_env/game.py
--rw-r--r--   0        0        0        0 2023-04-19 02:40:47.094863 pokerrl_env-0.1.0/pokerrl_env/gpt.pr
--rw-r--r--   0        0        0     1688 2023-04-17 07:06:58.855019 pokerrl_env-0.1.0/pokerrl_env/play.py
--rw-r--r--   0        0        0     5510 2023-04-19 01:39:25.633002 pokerrl_env-0.1.0/pokerrl_env/test_pots.py
--rw-r--r--   0        0        0    40392 2023-04-19 03:05:38.220718 pokerrl_env-0.1.0/pokerrl_env/test_transition.py
--rw-r--r--   0        0        0     3752 2023-04-19 03:01:00.265062 pokerrl_env-0.1.0/pokerrl_env/test_utils.py
--rw-r--r--   0        0        0     2622 2023-04-17 23:30:41.089879 pokerrl_env-0.1.0/pokerrl_env/test_view.py
--rw-r--r--   0        0        0    20865 2023-04-19 03:15:16.945722 pokerrl_env-0.1.0/pokerrl_env/transition.py
--rw-r--r--   0        0        0     7611 2023-04-19 03:14:51.187755 pokerrl_env-0.1.0/pokerrl_env/utils.py
--rw-r--r--   0        0        0     9600 2023-04-18 01:18:13.066059 pokerrl_env-0.1.0/pokerrl_env/view.py
--rw-r--r--   0        0        0      420 2023-04-19 03:27:43.140689 pokerrl_env-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3693 1970-01-01 00:00:00.000000 pokerrl_env-0.1.0/setup.py
--rw-r--r--   0        0        0     3532 1970-01-01 00:00:00.000000 pokerrl_env-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2899 2023-04-18 23:30:10.137034 pokerrl_env-0.1.1/README.md
+-rw-r--r--   0        0        0      320 2023-04-17 18:11:46.664658 pokerrl_env-0.1.1/pokerrl_env/__init__.py
+-rw-r--r--   0        0        0     2807 2023-04-17 05:05:22.329945 pokerrl_env-0.1.1/pokerrl_env/cardlib.py
+-rw-r--r--   0        0        0     6102 2023-04-18 01:17:39.065416 pokerrl_env-0.1.1/pokerrl_env/config.py
+-rw-r--r--   0        0        0     3991 2023-04-18 03:31:27.573583 pokerrl_env-0.1.1/pokerrl_env/datatypes.py
+-rw-r--r--   0        0        0     1576 2023-04-19 03:49:06.659495 pokerrl_env-0.1.1/pokerrl_env/game.py
+-rw-r--r--   0        0        0        0 2023-04-19 02:40:47.094863 pokerrl_env-0.1.1/pokerrl_env/gpt.pr
+-rw-r--r--   0        0        0     1688 2023-04-17 07:06:58.855019 pokerrl_env-0.1.1/pokerrl_env/play.py
+-rw-r--r--   0        0        0     5510 2023-04-19 01:39:25.633002 pokerrl_env-0.1.1/pokerrl_env/test_pots.py
+-rw-r--r--   0        0        0    40412 2023-04-19 03:49:25.710551 pokerrl_env-0.1.1/pokerrl_env/test_transition.py
+-rw-r--r--   0        0        0     3768 2023-04-19 03:49:32.524122 pokerrl_env-0.1.1/pokerrl_env/test_utils.py
+-rw-r--r--   0        0        0     2638 2023-04-19 03:49:37.391376 pokerrl_env-0.1.1/pokerrl_env/test_view.py
+-rw-r--r--   0        0        0    20881 2023-04-19 03:49:44.138919 pokerrl_env-0.1.1/pokerrl_env/transition.py
+-rw-r--r--   0        0        0     7615 2023-04-19 03:49:49.060973 pokerrl_env-0.1.1/pokerrl_env/utils.py
+-rw-r--r--   0        0        0     9600 2023-04-19 03:49:59.757293 pokerrl_env-0.1.1/pokerrl_env/view.py
+-rw-r--r--   0        0        0      420 2023-04-19 03:51:15.746069 pokerrl_env-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3693 1970-01-01 00:00:00.000000 pokerrl_env-0.1.1/setup.py
+-rw-r--r--   0        0        0     3532 1970-01-01 00:00:00.000000 pokerrl_env-0.1.1/PKG-INFO
```

### Comparing `pokerrl_env-0.1.0/README.md` & `pokerrl_env-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pokerrl_env-0.1.0/pokerrl_env/cardlib.py` & `pokerrl_env-0.1.1/pokerrl_env/cardlib.py`

 * *Files identical despite different names*

### Comparing `pokerrl_env-0.1.0/pokerrl_env/config.py` & `pokerrl_env-0.1.1/pokerrl_env/config.py`

 * *Files identical despite different names*

### Comparing `pokerrl_env-0.1.0/pokerrl_env/datatypes.py` & `pokerrl_env-0.1.1/pokerrl_env/datatypes.py`

 * *Files identical despite different names*

### Comparing `pokerrl_env-0.1.0/pokerrl_env/game.py` & `pokerrl_env-0.1.1/pokerrl_env/game.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from pokerrl.transition import init_state, step_state
-from pokerrl.config import Config
-from pokerrl.utils import return_current_player
-from pokerrl.view import player_view,json_view
+from pokerrl_env.transition import init_state, step_state
+from pokerrl_env.config import Config
+from pokerrl_env.utils import return_current_player
+from pokerrl_env.view import player_view,json_view
 
 class Game:
     def __init__(self,config:Config):
         self.config = config
         self.global_state = None
         self.done = None
         self.winnings = None
```

### Comparing `pokerrl_env-0.1.0/pokerrl_env/play.py` & `pokerrl_env-0.1.1/pokerrl_env/play.py`

 * *Files identical despite different names*

### Comparing `pokerrl_env-0.1.0/pokerrl_env/test_pots.py` & `pokerrl_env-0.1.1/pokerrl_env/test_pots.py`

 * *Files identical despite different names*

### Comparing `pokerrl_env-0.1.0/pokerrl_env/test_transition.py` & `pokerrl_env-0.1.1/pokerrl_env/test_transition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 import pytest
 import numpy as np
-from pokerrl.transition import *
-from pokerrl.config import Config
-from pokerrl.datatypes import POSITION_TO_SEAT, SEAT_TO_POSITION, StateActions, Street
-from pokerrl.utils import calculate_pot_limit_betsize, readable_card_to_int
-from pokerrl.transition import get_action_mask,players_finished,step_state,init_state
+from pokerrl_env.transition import *
+from pokerrl_env.config import Config
+from pokerrl_env.datatypes import POSITION_TO_SEAT, SEAT_TO_POSITION, StateActions, Street
+from pokerrl_env.utils import calculate_pot_limit_betsize, readable_card_to_int
+from pokerrl_env.transition import get_action_mask,players_finished,step_state,init_state
 
 config = Config(num_players=6)
 
 @pytest.fixture
 def river_state():
     global_state = np.zeros(config.global_state_shape, dtype=np.int32)
     for i in range(1, 4):
```

### Comparing `pokerrl_env-0.1.0/pokerrl_env/test_utils.py` & `pokerrl_env-0.1.1/pokerrl_env/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from pokerrl.datatypes import BetLimits, GameTypes, Player, Positions
-from pokerrl.utils import is_next_player_the_aggressor,return_deck
+from pokerrl_env.datatypes import BetLimits, GameTypes, Player, Positions
+from pokerrl_env.utils import is_next_player_the_aggressor,return_deck
 import pytest
-from pokerrl.config import Config
-from pokerrl.transition import init_state
+from pokerrl_env.config import Config
+from pokerrl_env.transition import init_state
 import numpy as np
 
 
 def test_default_values():
     config = Config()
     assert config.game_type == GameTypes.OMAHA_HI
     assert config.num_players == 2
```

### Comparing `pokerrl_env-0.1.0/pokerrl_env/test_view.py` & `pokerrl_env-0.1.1/pokerrl_env/test_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
-from pokerrl.datatypes import Positions
+from pokerrl_env.datatypes import Positions
 import pytest
-from pokerrl.view import player_view, human_readable_view,return_board_cards
-from pokerrl.config import Config
-from pokerrl.transition import init_state
+from pokerrl_env.view import player_view, human_readable_view,return_board_cards
+from pokerrl_env.config import Config
+from pokerrl_env.transition import init_state
 
 
 @pytest.fixture
 def config():
     return Config(num_players=6)
```

### Comparing `pokerrl_env-0.1.0/pokerrl_env/transition.py` & `pokerrl_env-0.1.1/pokerrl_env/transition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Dict, List, Tuple
 import numpy as np
-from pokerrl.config import Config
-from pokerrl.datatypes import PLAYER_ORDER_BY_STREET, POSITION_TO_SEAT,RAISE,CALL,FOLD,BET,CHECK, ModelActions, StateActions,Street,Player,Positions
-from pokerrl.cardlib import encode, hand_rank
-from pokerrl.utils import is_next_player_the_aggressor, return_deck
+from pokerrl_env.config import Config
+from pokerrl_env.datatypes import PLAYER_ORDER_BY_STREET, POSITION_TO_SEAT,RAISE,CALL,FOLD,BET,CHECK, ModelActions, StateActions,Street,Player,Positions
+from pokerrl_env.cardlib import encode, hand_rank
+from pokerrl_env.utils import is_next_player_the_aggressor, return_deck
 import copy
 
 def init_state(config: Config):
     deck = return_deck()
     
     state_SB = np.zeros(config.global_state_shape) 
     state_BB = np.zeros(config.global_state_shape)
```

### Comparing `pokerrl_env-0.1.0/pokerrl_env/utils.py` & `pokerrl_env-0.1.1/pokerrl_env/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import List
-from pokerrl.datatypes import BET, RAISE, ModelActions, Player, StateActions, Street,Positions, int_to_rank, int_to_suit,rank_to_int,suit_to_int
+from pokerrl_env.datatypes import BET, RAISE, ModelActions, Player, StateActions, Street,Positions, int_to_rank, int_to_suit,rank_to_int,suit_to_int
 from random import shuffle
 import numpy as np
 
 def return_deck():
     deck = []
     for suit in range(1,5):
         for rank in range(1,14):
```

### Comparing `pokerrl_env-0.1.0/pokerrl_env/view.py` & `pokerrl_env-0.1.1/pokerrl_env/view.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-import json
 import numpy as np
-from pokerrl.config import Config
-from pokerrl.datatypes import BOARD_CARDS_GIVEN_STREET, SEAT_TO_POSITION, INT_TO_STREET
-from pokerrl.utils import human_readable_cards
+from pokerrl_env.config import Config
+from pokerrl_env.datatypes import BOARD_CARDS_GIVEN_STREET, SEAT_TO_POSITION, INT_TO_STREET
+from pokerrl_env.utils import human_readable_cards
 
 
 def return_board_cards(global_state, config):
     num_board_cards = BOARD_CARDS_GIVEN_STREET[ global_state[config.global_state_mapping["street"]] ]
     if num_board_cards == 0:
         padded_board_cards = np.zeros(10)
     else:
```

### Comparing `pokerrl_env-0.1.0/setup.py` & `pokerrl_env-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['numpy>=1.19.5,<2.0.0',
  'pytest>=6.2.4,<7.0.0',
  'setuptools-rust>=1.5.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'pokerrl-env',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'A poker environment for reinforcement learning',
     'long_description': "# Poker environment for reinforcement learning\n\nTo instantiate the environment, pass in the config.\n\nthe config consists of the following parameters:\n\n- number of players (2-6), default 2\n- bet limit (fixed limit, no limit, pot limit), default pot limit\n- bet sizes allowed (array of floats), default (1, 0.9, 0.75, 0.67, 0.5, 0.33, 0.25, 0.1)\n- Game type [Holdem, OmahaHI], default OmahaHI\n\n## Example usage\n\nThis is the recommended way to use the environment.\n\n```\nfrom pokerrl import Config, Game\n\nconfig = Config(\n    num_players=2,\n    bet_limit=BetLimits.POT_LIMIT,\n    bet_sizes=[1, 0.5],\n    game_type=GameTypes.OMAHA_HI,\n)\ngame = Game(config)\nplayer_state,done,winnings,action_mask = game.reset()\nwhile not done:\n  action = model(player_state)\n  player_state,done,winnings,action_mask = game.step(action)\n```\n\n## Play a game (both sides)\n\n```\nfrom pokerrl import play_game\nplay_game()\n```\n\n## Example usage (low level)\n\n```\nfrom pokerrl import Config, init_state, step_state, GameTypes, BetLimits, player_view, Positions, get_current_player\n\nconfig = Config(\n    num_players=2,\n    bet_limit=BetLimits.POT_LIMIT,\n    bet_sizes=[1, 0.5],\n    game_type=GameTypes.OMAHA_HI,\n)\nglobal_state,done,winnings,action_mask = init_state(config)\nwhile not done:\n  player_idx = get_current_player(global_state)\n  player_state = player_view(global_state, player_idx)\n  action = model(player_state)\n  global_state,done,winnings,action_mask = step_state(global_state, action, config)\n```\n\n## Player view (low level)\n\n```\nfrom pokerrl import Config, init_state, step_state, GameTypes, BetLimits, player_view, Positions, get_current_player\n\nconfig = Config()\nglobal_state,done,winnings,action_mask = init_state(config)\nwhile not done:\n  player_idx = get_current_player(global_state)\n  human_readable_view(global_state,player_idx, config)\n  action = get_action(action_mask,global_state,config)\n  global_state,done,winnings,action_mask = step_state(global_state, action, config)\n```\n\n## State\n\nThe state is an array. To get a player's view of the state, pass the state into the view with the appropriate player index.\n\n## Design decisions\n\n- Record the total amount raised.\n  If you record the actual amount raised this means its more difficult to tell what the raise size is when facing multiple raises. But easier to tell what the raise size is when facing a single raise. Also complicates the process of determining how much a player has to call, as the raise size is in relation to the previous bet, which in multiplayer games, is not necessarily us.\n- Global state player numbers are identical to their position.\n- SB and BB posts are the first two states.\n\n- A raise is the total amount. Subtract player street total\n- A call vs a raise is the difference = villain bet - player street total\n- A call vs a bet is the full amount = villain bet - player street total\n- A bet is the full amount\n- A fold is 0\n",
     'author': 'Morgan Griffiths',
     'author_email': 'rareducks101@yahoo.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pokerrl_env-0.1.0/PKG-INFO` & `pokerrl_env-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pokerrl-env
-Version: 0.1.0
+Version: 0.1.1
 Summary: A poker environment for reinforcement learning
 License: MIT
 Author: Morgan Griffiths
 Author-email: rareducks101@yahoo.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


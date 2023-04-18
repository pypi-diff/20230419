# Comparing `tmp/sopel-8ball-0.3.1.tar.gz` & `tmp/sopel-8ball-0.4.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sopel-8ball-0.3.1.tar", last modified: Sun Jul 10 10:28:27 2022, max compression
+gzip compressed data, was "sopel-8ball-0.4.0.dev0.tar", last modified: Tue Apr 18 22:34:40 2023, max compression
```

## Comparing `sopel-8ball-0.3.1.tar` & `sopel-8ball-0.4.0.dev0.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxr-x   0 fstrzelecki  (1001) fstrzelecki  (1001)        0 2022-07-10 10:28:27.660835 sopel-8ball-0.3.1/
--rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)     1021 2021-07-10 22:27:18.000000 sopel-8ball-0.3.1/LICENSE.txt
--rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)     2662 2022-07-10 10:28:27.660835 sopel-8ball-0.3.1/PKG-INFO
--rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)     1284 2022-07-10 10:27:29.000000 sopel-8ball-0.3.1/README.rst
--rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)     1524 2022-07-10 10:28:27.660835 sopel-8ball-0.3.1/setup.cfg
--rw-r--r--   0 fstrzelecki  (1001) fstrzelecki  (1001)       38 2021-07-08 18:48:47.000000 sopel-8ball-0.3.1/setup.py
-drwxrwxr-x   0 fstrzelecki  (1001) fstrzelecki  (1001)        0 2022-07-10 10:28:27.660835 sopel-8ball-0.3.1/sopel_8ball/
--rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)      178 2021-07-08 21:33:17.000000 sopel-8ball-0.3.1/sopel_8ball/__init__.py
--rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)     4918 2022-07-10 10:25:35.000000 sopel-8ball-0.3.1/sopel_8ball/choices.py
--rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)      472 2021-07-09 13:37:34.000000 sopel-8ball-0.3.1/sopel_8ball/config.py
--rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)     2480 2021-07-09 15:59:39.000000 sopel-8ball-0.3.1/sopel_8ball/managers.py
--rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)     1315 2022-01-20 13:17:00.000000 sopel-8ball-0.3.1/sopel_8ball/plugin.py
-drwxrwxr-x   0 fstrzelecki  (1001) fstrzelecki  (1001)        0 2022-07-10 10:28:27.660835 sopel-8ball-0.3.1/sopel_8ball.egg-info/
--rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)     2662 2022-07-10 10:28:27.000000 sopel-8ball-0.3.1/sopel_8ball.egg-info/PKG-INFO
--rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)      402 2022-07-10 10:28:27.000000 sopel-8ball-0.3.1/sopel_8ball.egg-info/SOURCES.txt
--rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)        1 2022-07-10 10:28:27.000000 sopel-8ball-0.3.1/sopel_8ball.egg-info/dependency_links.txt
--rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)      177 2022-07-10 10:28:27.000000 sopel-8ball-0.3.1/sopel_8ball.egg-info/entry_points.txt
--rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)        1 2021-07-08 18:48:50.000000 sopel-8ball-0.3.1/sopel_8ball.egg-info/not-zip-safe
--rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)       14 2022-07-10 10:28:27.000000 sopel-8ball-0.3.1/sopel_8ball.egg-info/requires.txt
--rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)       12 2022-07-10 10:28:27.000000 sopel-8ball-0.3.1/sopel_8ball.egg-info/top_level.txt
+drwxrwxr-x   0 fstrzelecki  (1000) fstrzelecki  (1000)        0 2023-04-18 22:34:40.094285 sopel-8ball-0.4.0.dev0/
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     1021 2021-07-10 22:27:18.000000 sopel-8ball-0.4.0.dev0/LICENSE.txt
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     2564 2023-04-18 22:34:40.094285 sopel-8ball-0.4.0.dev0/PKG-INFO
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     1380 2023-04-18 22:09:45.000000 sopel-8ball-0.4.0.dev0/README.rst
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     1737 2023-04-18 22:34:29.000000 sopel-8ball-0.4.0.dev0/pyproject.toml
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)      218 2023-04-18 22:34:40.094285 sopel-8ball-0.4.0.dev0/setup.cfg
+drwxrwxr-x   0 fstrzelecki  (1000) fstrzelecki  (1000)        0 2023-04-18 22:34:40.090285 sopel-8ball-0.4.0.dev0/sopel_8ball/
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)      178 2021-07-08 21:33:17.000000 sopel-8ball-0.4.0.dev0/sopel_8ball/__init__.py
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     6253 2023-04-18 22:19:57.000000 sopel-8ball-0.4.0.dev0/sopel_8ball/choices.py
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)      472 2021-07-09 13:37:34.000000 sopel-8ball-0.4.0.dev0/sopel_8ball/config.py
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     2480 2021-07-09 15:59:39.000000 sopel-8ball-0.4.0.dev0/sopel_8ball/managers.py
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     1315 2022-01-20 13:17:00.000000 sopel-8ball-0.4.0.dev0/sopel_8ball/plugin.py
+drwxrwxr-x   0 fstrzelecki  (1000) fstrzelecki  (1000)        0 2023-04-18 22:34:40.094285 sopel-8ball-0.4.0.dev0/sopel_8ball.egg-info/
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     2564 2023-04-18 22:34:40.000000 sopel-8ball-0.4.0.dev0/sopel_8ball.egg-info/PKG-INFO
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)      374 2023-04-18 22:34:40.000000 sopel-8ball-0.4.0.dev0/sopel_8ball.egg-info/SOURCES.txt
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)        1 2023-04-18 22:34:40.000000 sopel-8ball-0.4.0.dev0/sopel_8ball.egg-info/dependency_links.txt
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)      216 2023-04-18 22:34:40.000000 sopel-8ball-0.4.0.dev0/sopel_8ball.egg-info/entry_points.txt
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)       11 2023-04-18 22:34:40.000000 sopel-8ball-0.4.0.dev0/sopel_8ball.egg-info/requires.txt
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)       12 2023-04-18 22:34:40.000000 sopel-8ball-0.4.0.dev0/sopel_8ball.egg-info/top_level.txt
```

### Comparing `sopel-8ball-0.3.1/LICENSE.txt` & `sopel-8ball-0.4.0.dev0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sopel-8ball-0.3.1/README.rst` & `sopel-8ball-0.4.0.dev0/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 ====================
 
 There are more than one style of choices you can select:
 
 * ``classic``: the classic version (10 yes, 5 maybe, 5 no)
 * ``snarky``: this version is rude (5 yes, 5 maybe, 10 no)
 * ``spooky``: use at your own risk (5 yes, 10 maybe, 5 no, 100% freaky)
+* ``weeaball``: for japanese style fan ＼(＾▽＾)／ (7 yes, 9 maybe, 7 no,
+  100% kaomoji)
 
 This can be configured with the Sopel configuration wizard::
 
     $ sopel-plugins configure 8ball
 
 Or manually, by editing your configuration and adding this section::
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sopel-8ball-0.3.1/sopel_8ball/choices.py` & `sopel-8ball-0.4.0.dev0/sopel_8ball/choices.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Choices module for the magic 8 ball."""
-from __future__ import generator_stop
+from __future__ import annotations
 
 import abc
 import random
-from typing import Tuple
+from typing import TYPE_CHECKING, Tuple
 
-from sopel.bot import Sopel  # type: ignore
-from sopel.config import Config  # type: ignore
-from sopel.tools import Identifier  # type: ignore
+if TYPE_CHECKING:
+    from sopel.bot import Sopel  # type: ignore
+    from sopel.config import Config  # type: ignore
+    from sopel.tools import Identifier  # type: ignore
 
 
 class AbstractChoiceProvider(abc.ABC):
     """Base provider class of 8 ball choices.
 
     A provider will be set up and then can be used to query the magic 8 ball
     from a destination (usually a channel) and a user::
@@ -40,30 +41,34 @@
 
         :return: all possible choices for this 8 ball
 
         This is the list of choices unfiltered and valid for any destination
         and any user.
         """
 
-    def query(self, destination: Identifier, user: Identifier) -> str:
+    def query(
+            self,
+            destination: Identifier,  # pylint: disable=unused-argument
+            user: Identifier,  # pylint: disable=unused-argument
+    ) -> str:
         """Query the 8 ball for one of its choice.
 
-        :param bot: sopel instance used to query the magic 8 ball
-        :param trigger: trigger that triggered the query
+        :param destination: where the choice will be published
+        :param user: the user's nick who requested the choice
         :return: the 8 ball's answer to that query
         """
         return random.choice(self.choices())
 
 
 class Classic(AbstractChoiceProvider):
     """The classic magic 8 ball."""
     def choices(self) -> Tuple[str, ...]:
         return (
             # affirmative answers
-            "It is Certain.",
+            "It is certain.",
             "It is decidedly so.",
             "Without a doubt.",
             "Yes definitely.",
             "You may rely on it.",
 
             "As I see it, yes.",
             "Most likely.",
@@ -88,29 +93,29 @@
 
 
 class Snarky(AbstractChoiceProvider):
     """A snarky magic 8 ball."""
     def choices(self) -> Tuple[str, ...]:
         return (
             # affirmative answers
-            "What’s the opposite of no?",
+            "What's the opposite of no?",
             "Is the sun hot?",
             "Heck yes!",
             "Of course, duh!",
             "Yeah, sure.",
 
             # non-committal answers
             "No comment.",
             "Cool query.",
-            "I wasn’t born for this.",
+            "I wasn't born for this.",
             "Sorry, I wasn't listening.",
             "Please cancel my subscription to your issues.",
 
             # negative answers
-            "What’s the opposite of yes?",
+            "What's the opposite of yes?",
             "Is the sun cold?",
             "Hell to the no!",
             "You're joking, right?",
             "Ewwww...no!",
 
             "My answer is a resounding no!",
             "Frankly, my dear—no!",
@@ -130,25 +135,60 @@
             "The elders smile from the deep.",
             "I've seen this in the dreams of a Great Old One.",
             "For once, eerie voices whisper in harmony.",
 
             # non-committal answers
             "The abyss remains silent.",
             "I hear the whispers of a thousand voices, "
-            "but none have your answer.",
+            "but none has your answer.",
             "The unfathomable truth cannot be revealed.",
             "In the darkness this won't matter anymore.",
-            "From the depth comes no answer.",
+            "From the depths comes no reply.",
 
             "The spirits are bored of this tune.",
             "The answer lies beyond the stars, ineffable.",
             "Answers are lost in the midst of black seas of infinity.",
             "You shall go mad from the revelation of the truth.",
             "I hear your call, yet their shrieking keeps me silent.",
 
             # negative answers
             "This would anger the old gods.",
             "This will bring sorrow and tears.",
             "The elders scowl from the deep.",
             "Hidden and fathomless minds pulsate in rage.",
             "The underworld grumbles with repudiation.",
         )
+
+
+class Weeaball(AbstractChoiceProvider):
+    """A weeaboo magic 8 ball."""
+    def choices(self) -> Tuple[str, ...]:
+        return (
+            # affirmative answers
+            "Atarimae. (＾▽＾)",
+            "Daijoubu~ ٩(◕‿◕｡)۶",
+            "Hai! (⌒‿⌒)",
+            "Ii kangae! (ﾉ◕ヮ◕)ﾉ*:･ﾟ✧",
+            "Mochiron. (*￣▽￣)b",
+            "Sou desu. (٥⁀▽⁀ )b",
+            "Zettai! ＼(＾▽＾)／",
+
+            # non-committal answers
+            "Betsu ni. ╮(︶︿︶)╭",
+            "Isogashii… (－ω－) zzZ",
+            "Ittai dou iu imi desu ka?! ლ(ಠ_ಠ ლ)",
+            "Katte ni shiro! (ノ°益°)ノ",
+            "Mendokusai. (＃￣0￣)",
+            "Omae kankei nai. (ಠ_ಠ)",
+            "Osoraku. ┐(°ヮ°)┌",
+            "Tsumaranai. ┐( ˘ ､ ˘ )┌",
+            "Urusai! (╬`益´)",
+
+            # negative answers
+            "Arienai. (|||❛︵❛。)"
+            "Chigau. (◞ ‸ ◟ㆀ)",
+            "Dame! o(╥﹏╥)",
+            "Iie. (ᗒᗩᗕ)",
+            "Masaka! (╯︵╰)",
+            "Muri. ▄█▀█●",
+            "Zannen. _|￣|○",
+        )
```

### Comparing `sopel-8ball-0.3.1/sopel_8ball/managers.py` & `sopel-8ball-0.4.0.dev0/sopel_8ball/managers.py`

 * *Files identical despite different names*

### Comparing `sopel-8ball-0.3.1/sopel_8ball/plugin.py` & `sopel-8ball-0.4.0.dev0/sopel_8ball/plugin.py`

 * *Files identical despite different names*


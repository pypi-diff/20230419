# Comparing `tmp/sopel-8ball-0.3.0.tar.gz` & `tmp/sopel-8ball-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sopel-8ball-0.3.0.tar", last modified: Thu Jan 20 16:54:32 2022, max compression
+gzip compressed data, was "sopel-8ball-0.3.1.tar", last modified: Sun Jul 10 10:28:27 2022, max compression
```

## Comparing `sopel-8ball-0.3.0.tar` & `sopel-8ball-0.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 fstrzelecki  (1001) fstrzelecki  (1001)        0 2022-01-20 16:54:32.280546 sopel-8ball-0.3.0/
--rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)     1021 2021-07-10 22:27:18.000000 sopel-8ball-0.3.0/LICENSE.txt
--rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)     2662 2022-01-20 16:54:32.280546 sopel-8ball-0.3.0/PKG-INFO
--rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)     1284 2021-07-10 10:31:53.000000 sopel-8ball-0.3.0/README.rst
--rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)     1524 2022-01-20 16:54:32.280546 sopel-8ball-0.3.0/setup.cfg
--rw-r--r--   0 fstrzelecki  (1001) fstrzelecki  (1001)       38 2021-07-08 18:48:47.000000 sopel-8ball-0.3.0/setup.py
-drwxrwxr-x   0 fstrzelecki  (1001) fstrzelecki  (1001)        0 2022-01-20 16:54:32.280546 sopel-8ball-0.3.0/sopel_8ball/
--rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)      178 2021-07-08 21:33:17.000000 sopel-8ball-0.3.0/sopel_8ball/__init__.py
--rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)     4920 2021-07-10 10:31:00.000000 sopel-8ball-0.3.0/sopel_8ball/choices.py
--rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)      472 2021-07-09 13:37:34.000000 sopel-8ball-0.3.0/sopel_8ball/config.py
--rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)     2480 2021-07-09 15:59:39.000000 sopel-8ball-0.3.0/sopel_8ball/managers.py
--rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)     1315 2022-01-20 13:17:00.000000 sopel-8ball-0.3.0/sopel_8ball/plugin.py
-drwxrwxr-x   0 fstrzelecki  (1001) fstrzelecki  (1001)        0 2022-01-20 16:54:32.280546 sopel-8ball-0.3.0/sopel_8ball.egg-info/
--rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)     2662 2022-01-20 16:54:32.000000 sopel-8ball-0.3.0/sopel_8ball.egg-info/PKG-INFO
--rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)      402 2022-01-20 16:54:32.000000 sopel-8ball-0.3.0/sopel_8ball.egg-info/SOURCES.txt
--rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)        1 2022-01-20 16:54:32.000000 sopel-8ball-0.3.0/sopel_8ball.egg-info/dependency_links.txt
--rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)      177 2022-01-20 16:54:32.000000 sopel-8ball-0.3.0/sopel_8ball.egg-info/entry_points.txt
--rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)        1 2021-07-08 18:48:50.000000 sopel-8ball-0.3.0/sopel_8ball.egg-info/not-zip-safe
--rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)       14 2022-01-20 16:54:32.000000 sopel-8ball-0.3.0/sopel_8ball.egg-info/requires.txt
--rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)       12 2022-01-20 16:54:32.000000 sopel-8ball-0.3.0/sopel_8ball.egg-info/top_level.txt
+drwxrwxr-x   0 fstrzelecki  (1001) fstrzelecki  (1001)        0 2022-07-10 10:28:27.660835 sopel-8ball-0.3.1/
+-rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)     1021 2021-07-10 22:27:18.000000 sopel-8ball-0.3.1/LICENSE.txt
+-rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)     2662 2022-07-10 10:28:27.660835 sopel-8ball-0.3.1/PKG-INFO
+-rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)     1284 2022-07-10 10:27:29.000000 sopel-8ball-0.3.1/README.rst
+-rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)     1524 2022-07-10 10:28:27.660835 sopel-8ball-0.3.1/setup.cfg
+-rw-r--r--   0 fstrzelecki  (1001) fstrzelecki  (1001)       38 2021-07-08 18:48:47.000000 sopel-8ball-0.3.1/setup.py
+drwxrwxr-x   0 fstrzelecki  (1001) fstrzelecki  (1001)        0 2022-07-10 10:28:27.660835 sopel-8ball-0.3.1/sopel_8ball/
+-rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)      178 2021-07-08 21:33:17.000000 sopel-8ball-0.3.1/sopel_8ball/__init__.py
+-rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)     4918 2022-07-10 10:25:35.000000 sopel-8ball-0.3.1/sopel_8ball/choices.py
+-rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)      472 2021-07-09 13:37:34.000000 sopel-8ball-0.3.1/sopel_8ball/config.py
+-rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)     2480 2021-07-09 15:59:39.000000 sopel-8ball-0.3.1/sopel_8ball/managers.py
+-rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)     1315 2022-01-20 13:17:00.000000 sopel-8ball-0.3.1/sopel_8ball/plugin.py
+drwxrwxr-x   0 fstrzelecki  (1001) fstrzelecki  (1001)        0 2022-07-10 10:28:27.660835 sopel-8ball-0.3.1/sopel_8ball.egg-info/
+-rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)     2662 2022-07-10 10:28:27.000000 sopel-8ball-0.3.1/sopel_8ball.egg-info/PKG-INFO
+-rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)      402 2022-07-10 10:28:27.000000 sopel-8ball-0.3.1/sopel_8ball.egg-info/SOURCES.txt
+-rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)        1 2022-07-10 10:28:27.000000 sopel-8ball-0.3.1/sopel_8ball.egg-info/dependency_links.txt
+-rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)      177 2022-07-10 10:28:27.000000 sopel-8ball-0.3.1/sopel_8ball.egg-info/entry_points.txt
+-rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)        1 2021-07-08 18:48:50.000000 sopel-8ball-0.3.1/sopel_8ball.egg-info/not-zip-safe
+-rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)       14 2022-07-10 10:28:27.000000 sopel-8ball-0.3.1/sopel_8ball.egg-info/requires.txt
+-rw-rw-r--   0 fstrzelecki  (1001) fstrzelecki  (1001)       12 2022-07-10 10:28:27.000000 sopel-8ball-0.3.1/sopel_8ball.egg-info/top_level.txt
```

### Comparing `sopel-8ball-0.3.0/LICENSE.txt` & `sopel-8ball-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sopel-8ball-0.3.0/PKG-INFO` & `sopel-8ball-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sopel-8ball
-Version: 0.3.0
+Version: 0.3.1
 Summary: Magic 8 ball plugin for Sopel
 Home-page: https://github.com/Exirel/sopel-8ball
 Author: Florian Strzelecki
 Author-email: florian.strzelecki@gmail.com
 License: Eiffel Forum License, version 2
 Description: ===========
         sopel-8ball
```

### Comparing `sopel-8ball-0.3.0/README.rst` & `sopel-8ball-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `sopel-8ball-0.3.0/setup.cfg` & `sopel-8ball-0.3.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sopel-8ball
-version = 0.3.0
+version = 0.3.1
 description = Magic 8 ball plugin for Sopel
 keywords = sopel plugin height-ball bot irc
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Florian Strzelecki
 author_email = florian.strzelecki@gmail.com
 url = https://github.com/Exirel/sopel-8ball
```

### Comparing `sopel-8ball-0.3.0/sopel_8ball/choices.py` & `sopel-8ball-0.3.1/sopel_8ball/choices.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import abc
 import random
 from typing import Tuple
 
 from sopel.bot import Sopel  # type: ignore
 from sopel.config import Config  # type: ignore
-from sopel.tools.target import Identifier  # type: ignore
+from sopel.tools import Identifier  # type: ignore
 
 
 class AbstractChoiceProvider(abc.ABC):
     """Base provider class of 8 ball choices.
 
     A provider will be set up and then can be used to query the magic 8 ball
     from a destination (usually a channel) and a user::
@@ -92,52 +92,52 @@
     def choices(self) -> Tuple[str, ...]:
         return (
             # affirmative answers
             "What’s the opposite of no?",
             "Is the sun hot?",
             "Heck yes!",
             "Of course, duh!",
-            "Yeah sure",
+            "Yeah, sure.",
 
             # non-committal answers
-            "No comment",
-            "Cool query",
+            "No comment.",
+            "Cool query.",
             "I wasn’t born for this.",
-            "Sorry, I wasn't listening",
+            "Sorry, I wasn't listening.",
             "Please cancel my subscription to your issues.",
 
             # negative answers
             "What’s the opposite of yes?",
             "Is the sun cold?",
             "Hell to the no!",
             "You're joking, right?",
             "Ewwww...no!",
 
             "My answer is a resounding no!",
             "Frankly, my dear—no!",
             "No no no no no no no no no no no!",
-            "Would you take ‘no’ for an answer?",
+            "Would you take \"no\" for an answer?",
             "Not in this lifetime!",
         )
 
 
 class Spooky(AbstractChoiceProvider):
     """A spooky magic 8 ball."""
     def choices(self) -> Tuple[str, ...]:
         return (
             # affirmative answers
             "The ghost over your shoulder said yes.",
             "The accursed screams in agreement.",
             "The elders smile from the deep.",
             "I've seen this in the dreams of a Great Old One.",
-            "For once eerie voices whisper in harmony.",
+            "For once, eerie voices whisper in harmony.",
 
             # non-committal answers
             "The abyss remains silent.",
-            "I hear the whispers of a thousand voices "
+            "I hear the whispers of a thousand voices, "
             "but none have your answer.",
             "The unfathomable truth cannot be revealed.",
             "In the darkness this won't matter anymore.",
             "From the depth comes no answer.",
 
             "The spirits are bored of this tune.",
             "The answer lies beyond the stars, ineffable.",
```

### Comparing `sopel-8ball-0.3.0/sopel_8ball/managers.py` & `sopel-8ball-0.3.1/sopel_8ball/managers.py`

 * *Files identical despite different names*

### Comparing `sopel-8ball-0.3.0/sopel_8ball/plugin.py` & `sopel-8ball-0.3.1/sopel_8ball/plugin.py`

 * *Files identical despite different names*

### Comparing `sopel-8ball-0.3.0/sopel_8ball.egg-info/PKG-INFO` & `sopel-8ball-0.3.1/sopel_8ball.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sopel-8ball
-Version: 0.3.0
+Version: 0.3.1
 Summary: Magic 8 ball plugin for Sopel
 Home-page: https://github.com/Exirel/sopel-8ball
 Author: Florian Strzelecki
 Author-email: florian.strzelecki@gmail.com
 License: Eiffel Forum License, version 2
 Description: ===========
         sopel-8ball
```


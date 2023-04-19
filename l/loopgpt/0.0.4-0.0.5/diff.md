# Comparing `tmp/loopgpt-0.0.4.tar.gz` & `tmp/loopgpt-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loopgpt-0.0.4.tar", last modified: Wed Apr 19 00:32:10 2023, max compression
+gzip compressed data, was "loopgpt-0.0.5.tar", last modified: Wed Apr 19 02:59:59 2023, max compression
```

## Comparing `loopgpt-0.0.4.tar` & `loopgpt-0.0.5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 00:32:10.299148 loopgpt-0.0.4/
--rw-rw-rw-   0        0        0     1090 2023-04-15 06:20:55.000000 loopgpt-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      114 2023-04-19 00:32:10.299148 loopgpt-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     8005 2023-04-19 00:00:57.000000 loopgpt-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 00:32:10.266986 loopgpt-0.0.4/loopgpt/
--rw-rw-rw-   0        0        0      486 2023-04-19 00:31:06.000000 loopgpt-0.0.4/loopgpt/__init__.py
--rw-rw-rw-   0        0        0    16188 2023-04-18 22:30:05.000000 loopgpt-0.0.4/loopgpt/agent.py
--rw-rw-rw-   0        0        0     3962 2023-04-18 22:30:05.000000 loopgpt-0.0.4/loopgpt/constants.py
-drwxrwxrwx   0        0        0        0 2023-04-19 00:32:10.275039 loopgpt-0.0.4/loopgpt/embeddings/
--rw-rw-rw-   0        0        0      775 2023-04-16 16:37:13.000000 loopgpt-0.0.4/loopgpt/embeddings/__init__.py
--rw-rw-rw-   0        0        0      810 2023-04-16 16:37:13.000000 loopgpt-0.0.4/loopgpt/embeddings/openai_.py
--rw-rw-rw-   0        0        0      426 2023-04-16 16:37:13.000000 loopgpt-0.0.4/loopgpt/embeddings/provider.py
--rw-rw-rw-   0        0        0       87 2023-04-19 00:06:55.000000 loopgpt-0.0.4/loopgpt/logger.py
-drwxrwxrwx   0        0        0        0 2023-04-19 00:32:10.283056 loopgpt-0.0.4/loopgpt/loops/
--rw-rw-rw-   0        0        0       36 2023-04-17 09:20:22.000000 loopgpt-0.0.4/loopgpt/loops/__init__.py
--rw-rw-rw-   0        0        0      964 2023-04-18 01:42:45.000000 loopgpt-0.0.4/loopgpt/loops/cli.py
--rw-rw-rw-   0        0        0     6710 2023-04-18 23:45:53.000000 loopgpt-0.0.4/loopgpt/loops/repl.py
--rw-rw-rw-   0        0        0     3108 2023-04-17 03:25:06.000000 loopgpt-0.0.4/loopgpt/loops/ui.py
-drwxrwxrwx   0        0        0        0 2023-04-19 00:32:10.283056 loopgpt-0.0.4/loopgpt/memory/
--rw-rw-rw-   0        0        0      698 2023-04-16 16:37:13.000000 loopgpt-0.0.4/loopgpt/memory/__init__.py
--rw-rw-rw-   0        0        0      423 2023-04-16 16:37:13.000000 loopgpt-0.0.4/loopgpt/memory/base_memory.py
--rw-rw-rw-   0        0        0     1998 2023-04-16 16:37:13.000000 loopgpt-0.0.4/loopgpt/memory/local_memory.py
-drwxrwxrwx   0        0        0        0 2023-04-19 00:32:10.283056 loopgpt-0.0.4/loopgpt/models/
--rw-rw-rw-   0        0        0       38 2023-04-15 06:20:55.000000 loopgpt-0.0.4/loopgpt/models/__init__.py
--rw-rw-rw-   0        0        0     1706 2023-04-17 07:40:41.000000 loopgpt-0.0.4/loopgpt/models/openai_.py
--rw-rw-rw-   0        0        0     1984 2023-04-18 22:30:05.000000 loopgpt-0.0.4/loopgpt/summarizer.py
-drwxrwxrwx   0        0        0        0 2023-04-19 00:32:10.299148 loopgpt-0.0.4/loopgpt/tools/
--rw-rw-rw-   0        0        0     1450 2023-04-17 08:31:57.000000 loopgpt-0.0.4/loopgpt/tools/__init__.py
--rw-rw-rw-   0        0        0     2276 2023-04-18 22:30:05.000000 loopgpt-0.0.4/loopgpt/tools/agent_manager.py
--rw-rw-rw-   0        0        0     1112 2023-04-16 16:37:13.000000 loopgpt-0.0.4/loopgpt/tools/base_tool.py
--rw-rw-rw-   0        0        0     4158 2023-04-19 00:05:57.000000 loopgpt-0.0.4/loopgpt/tools/browser.py
--rw-rw-rw-   0        0        0     3718 2023-04-17 07:40:41.000000 loopgpt-0.0.4/loopgpt/tools/code.py
--rw-rw-rw-   0        0        0     2556 2023-04-18 01:42:45.000000 loopgpt-0.0.4/loopgpt/tools/filesystem.py
--rw-rw-rw-   0        0        0     1999 2023-04-18 23:51:46.000000 loopgpt-0.0.4/loopgpt/tools/google_search.py
--rw-rw-rw-   0        0        0      421 2023-04-16 16:37:13.000000 loopgpt-0.0.4/loopgpt/tools/memory_manager.py
--rw-rw-rw-   0        0        0      675 2023-04-17 03:25:06.000000 loopgpt-0.0.4/loopgpt/tools/shell.py
--rw-rw-rw-   0        0        0     3124 2023-04-18 22:30:05.000000 loopgpt-0.0.4/loopgpt/tools/simple_browser.py
-drwxrwxrwx   0        0        0        0 2023-04-19 00:32:10.299148 loopgpt-0.0.4/loopgpt/utils/
--rw-rw-rw-   0        0        0        0 2023-04-19 00:30:19.000000 loopgpt-0.0.4/loopgpt/utils/__init__.py
--rw-rw-rw-   0        0        0     4174 2023-04-19 00:30:54.000000 loopgpt-0.0.4/loopgpt/utils/spinner.py
-drwxrwxrwx   0        0        0        0 2023-04-19 00:32:10.275039 loopgpt-0.0.4/loopgpt.egg-info/
--rw-rw-rw-   0        0        0      114 2023-04-19 00:32:10.000000 loopgpt-0.0.4/loopgpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      962 2023-04-19 00:32:10.000000 loopgpt-0.0.4/loopgpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 00:32:10.000000 loopgpt-0.0.4/loopgpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-04-19 00:32:10.000000 loopgpt-0.0.4/loopgpt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      114 2023-04-19 00:32:10.000000 loopgpt-0.0.4/loopgpt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-19 00:32:10.000000 loopgpt-0.0.4/loopgpt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 00:32:10.299148 loopgpt-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      464 2023-04-19 00:31:02.000000 loopgpt-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 02:59:59.403599 loopgpt-0.0.5/
+-rw-rw-rw-   0        0        0     1090 2023-04-15 06:20:55.000000 loopgpt-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      114 2023-04-19 02:59:59.403599 loopgpt-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     8918 2023-04-19 02:58:00.000000 loopgpt-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 02:59:59.379475 loopgpt-0.0.5/loopgpt/
+-rw-rw-rw-   0        0        0      486 2023-04-19 02:59:26.000000 loopgpt-0.0.5/loopgpt/__init__.py
+-rw-rw-rw-   0        0        0    16188 2023-04-19 02:44:42.000000 loopgpt-0.0.5/loopgpt/agent.py
+-rw-rw-rw-   0        0        0     3962 2023-04-18 22:30:05.000000 loopgpt-0.0.5/loopgpt/constants.py
+drwxrwxrwx   0        0        0        0 2023-04-19 02:59:59.387501 loopgpt-0.0.5/loopgpt/embeddings/
+-rw-rw-rw-   0        0        0      775 2023-04-16 16:37:13.000000 loopgpt-0.0.5/loopgpt/embeddings/__init__.py
+-rw-rw-rw-   0        0        0      810 2023-04-16 16:37:13.000000 loopgpt-0.0.5/loopgpt/embeddings/openai_.py
+-rw-rw-rw-   0        0        0      426 2023-04-16 16:37:13.000000 loopgpt-0.0.5/loopgpt/embeddings/provider.py
+-rw-rw-rw-   0        0        0       87 2023-04-19 00:06:55.000000 loopgpt-0.0.5/loopgpt/logger.py
+drwxrwxrwx   0        0        0        0 2023-04-19 02:59:59.387501 loopgpt-0.0.5/loopgpt/loops/
+-rw-rw-rw-   0        0        0       36 2023-04-17 09:20:22.000000 loopgpt-0.0.5/loopgpt/loops/__init__.py
+-rw-rw-rw-   0        0        0      964 2023-04-18 01:42:45.000000 loopgpt-0.0.5/loopgpt/loops/cli.py
+-rw-rw-rw-   0        0        0     6835 2023-04-19 02:27:28.000000 loopgpt-0.0.5/loopgpt/loops/repl.py
+-rw-rw-rw-   0        0        0     3108 2023-04-17 03:25:06.000000 loopgpt-0.0.5/loopgpt/loops/ui.py
+drwxrwxrwx   0        0        0        0 2023-04-19 02:59:59.395563 loopgpt-0.0.5/loopgpt/memory/
+-rw-rw-rw-   0        0        0      698 2023-04-16 16:37:13.000000 loopgpt-0.0.5/loopgpt/memory/__init__.py
+-rw-rw-rw-   0        0        0      423 2023-04-16 16:37:13.000000 loopgpt-0.0.5/loopgpt/memory/base_memory.py
+-rw-rw-rw-   0        0        0     1998 2023-04-16 16:37:13.000000 loopgpt-0.0.5/loopgpt/memory/local_memory.py
+drwxrwxrwx   0        0        0        0 2023-04-19 02:59:59.395563 loopgpt-0.0.5/loopgpt/models/
+-rw-rw-rw-   0        0        0       38 2023-04-15 06:20:55.000000 loopgpt-0.0.5/loopgpt/models/__init__.py
+-rw-rw-rw-   0        0        0     1706 2023-04-17 07:40:41.000000 loopgpt-0.0.5/loopgpt/models/openai_.py
+-rw-rw-rw-   0        0        0     1984 2023-04-18 22:30:05.000000 loopgpt-0.0.5/loopgpt/summarizer.py
+drwxrwxrwx   0        0        0        0 2023-04-19 02:59:59.403599 loopgpt-0.0.5/loopgpt/tools/
+-rw-rw-rw-   0        0        0     1450 2023-04-17 08:31:57.000000 loopgpt-0.0.5/loopgpt/tools/__init__.py
+-rw-rw-rw-   0        0        0     2276 2023-04-18 22:30:05.000000 loopgpt-0.0.5/loopgpt/tools/agent_manager.py
+-rw-rw-rw-   0        0        0     1112 2023-04-16 16:37:13.000000 loopgpt-0.0.5/loopgpt/tools/base_tool.py
+-rw-rw-rw-   0        0        0     4158 2023-04-19 00:05:57.000000 loopgpt-0.0.5/loopgpt/tools/browser.py
+-rw-rw-rw-   0        0        0     3718 2023-04-17 07:40:41.000000 loopgpt-0.0.5/loopgpt/tools/code.py
+-rw-rw-rw-   0        0        0     2556 2023-04-18 01:42:45.000000 loopgpt-0.0.5/loopgpt/tools/filesystem.py
+-rw-rw-rw-   0        0        0     1999 2023-04-18 23:51:46.000000 loopgpt-0.0.5/loopgpt/tools/google_search.py
+-rw-rw-rw-   0        0        0      421 2023-04-16 16:37:13.000000 loopgpt-0.0.5/loopgpt/tools/memory_manager.py
+-rw-rw-rw-   0        0        0      675 2023-04-17 03:25:06.000000 loopgpt-0.0.5/loopgpt/tools/shell.py
+-rw-rw-rw-   0        0        0     3124 2023-04-18 22:30:05.000000 loopgpt-0.0.5/loopgpt/tools/simple_browser.py
+drwxrwxrwx   0        0        0        0 2023-04-19 02:59:59.403599 loopgpt-0.0.5/loopgpt/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-19 00:30:19.000000 loopgpt-0.0.5/loopgpt/utils/__init__.py
+-rw-rw-rw-   0        0        0     4174 2023-04-19 00:30:54.000000 loopgpt-0.0.5/loopgpt/utils/spinner.py
+drwxrwxrwx   0        0        0        0 2023-04-19 02:59:59.381989 loopgpt-0.0.5/loopgpt.egg-info/
+-rw-rw-rw-   0        0        0      114 2023-04-19 02:59:59.000000 loopgpt-0.0.5/loopgpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      962 2023-04-19 02:59:59.000000 loopgpt-0.0.5/loopgpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 02:59:59.000000 loopgpt-0.0.5/loopgpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-04-19 02:59:59.000000 loopgpt-0.0.5/loopgpt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      114 2023-04-19 02:59:59.000000 loopgpt-0.0.5/loopgpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-19 02:59:59.000000 loopgpt-0.0.5/loopgpt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 02:59:59.403599 loopgpt-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      464 2023-04-19 02:59:31.000000 loopgpt-0.0.5/setup.py
```

### Comparing `loopgpt-0.0.4/LICENSE` & `loopgpt-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.4/README.md` & `loopgpt-0.0.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,501 +1,558 @@
 00000000: 0d0a 3c48 313e 0d0a 3c70 2061 6c69 676e  ..<H1>..<p align
 00000010: 3d22 6365 6e74 6572 223e 0d0a 2020 4ce2  ="center">..  L.
 00000020: 99be efb8 8f70 4750 540d 0a3c 2f70 3e0d  .....pGPT..</p>.
 00000030: 0a3c 2f48 313e 0d0a 3c70 2061 6c69 676e  .</H1>..<p align
 00000040: 3d22 6365 6e74 6572 223e 0d0a 2020 2020  ="center">..    
 00000050: 3c62 3e41 204d 6f64 756c 6172 2041 7574  <b>A Modular Aut
 00000060: 6f2d 4750 5420 4672 616d 6577 6f72 6b3c  o-GPT Framework<
-00000070: 2f62 3e0d 0a3c 2f70 3e0d 0a0d 0a0d 0a4c  /b>..</p>......L
-00000080: e299 beef b88f 7047 5054 2069 7320 6120  ......pGPT is a 
-00000090: 7265 2d69 6d70 6c65 6d65 6e74 6174 696f  re-implementatio
-000000a0: 6e20 6f66 2074 6865 2070 6f70 756c 6172  n of the popular
-000000b0: 205b 4175 746f 2d47 5054 5d28 6874 7470   [Auto-GPT](http
-000000c0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f53  s://github.com/S
-000000d0: 6967 6e69 6669 6361 6e74 2d47 7261 7669  ignificant-Gravi
-000000e0: 7461 732f 4175 746f 2d47 5054 2920 7072  tas/Auto-GPT) pr
-000000f0: 6f6a 6563 7420 6173 2061 2070 726f 7065  oject as a prope
-00000100: 7220 7079 7468 6f6e 2070 6163 6b61 6765  r python package
-00000110: 2c20 7772 6974 7465 6e20 7769 7468 206d  , written with m
-00000120: 6f64 756c 6172 6974 7920 616e 6420 6578  odularity and ex
-00000130: 7465 6e73 6962 696c 6974 7920 696e 206d  tensibility in m
-00000140: 696e 642e 0d0a 0d0a 2323 20f0 9f9a 8020  ind.....## .... 
-00000150: 4665 6174 7572 6573 20f0 9f9a 800d 0a0d  Features .......
-00000160: 0a31 2e20 2a2a 2250 6c75 6720 4e20 506c  .1. **"Plug N Pl
-00000170: 6179 2220 4150 492a 2a20 2d20 4578 7465  ay" API** - Exte
-00000180: 6e73 6962 6c65 2061 6e64 206d 6f64 756c  nsible and modul
-00000190: 6172 2022 5079 7468 6f6e 6963 2220 6672  ar "Pythonic" fr
-000001a0: 616d 6577 6f72 6b2c 206e 6f74 206a 7573  amework, not jus
-000001b0: 7420 6120 636f 6d6d 616e 6420 6c69 6e65  t a command line
-000001c0: 2074 6f6f 6c2e 2045 6173 7920 746f 2061   tool. Easy to a
-000001d0: 6464 206e 6577 2066 6561 7475 7265 732c  dd new features,
-000001e0: 2069 6e74 6567 7261 7469 6f6e 7320 616e   integrations an
-000001f0: 6420 6375 7374 6f6d 2061 6765 6e74 2063  d custom agent c
-00000200: 6170 6162 696c 6974 6965 732c 2061 6c6c  apabilities, all
-00000210: 2066 726f 6d20 7079 7468 6f6e 2063 6f64   from python cod
-00000220: 652c 206e 6f20 6e61 7374 7920 636f 6e66  e, no nasty conf
-00000230: 6967 2066 696c 6573 210d 0a32 2e20 2a2a  ig files!..2. **
-00000240: 4750 5420 332e 3520 6672 6965 6e64 6c79  GPT 3.5 friendly
-00000250: 2a2a 202d 2042 6574 7465 7220 7265 7375  ** - Better resu
-00000260: 6c74 7320 7468 616e 2041 7574 6f2d 4750  lts than Auto-GP
-00000270: 5420 666f 7220 7468 6f73 6520 7768 6f20  T for those who 
-00000280: 646f 6e27 7420 6861 7665 2047 5054 2d34  don't have GPT-4
-00000290: 2061 6363 6573 7320 7965 7421 0d0a 332e   access yet!..3.
-000002a0: 202a 2a4d 696e 696d 616c 2070 726f 6d70   **Minimal promp
-000002b0: 7420 6f76 6572 6865 6164 2a2a 202d 2045  t overhead** - E
-000002c0: 7665 7279 2074 6f6b 656e 2063 6f75 6e74  very token count
-000002d0: 732e 2057 6520 6172 6520 636f 6e74 696e  s. We are contin
-000002e0: 756f 7573 6c79 2077 6f72 6b69 6e67 206f  uously working o
-000002f0: 6e20 6765 7474 696e 6720 7468 6520 6265  n getting the be
-00000300: 7374 2072 6573 756c 7473 2077 6974 6820  st results with 
-00000310: 7468 6520 6c65 6173 7420 706f 7373 6962  the least possib
-00000320: 6c65 206e 756d 6265 7220 6f66 2074 6f6b  le number of tok
-00000330: 656e 732e 0d0a 342e 202a 2a48 756d 616e  ens...4. **Human
-00000340: 2069 6e20 7468 6520 4c6f 6f70 2a2a 202d   in the Loop** -
-00000350: 2041 6269 6c69 7479 2074 6f20 2263 6f75   Ability to "cou
-00000360: 7273 6520 636f 7272 6563 7422 2061 6765  rse correct" age
-00000370: 6e74 7320 7768 6f20 676f 2061 7374 7261  nts who go astra
-00000380: 7920 7669 6120 6875 6d61 6e20 6665 6564  y via human feed
-00000390: 6261 636b 2e0d 0a35 2e20 2a2a 4675 6c6c  back...5. **Full
-000003a0: 2073 7461 7465 2073 6572 6961 6c69 7a61   state serializa
-000003b0: 7469 6f6e 2a2a 202d 2050 6963 6b20 7570  tion** - Pick up
-000003c0: 2077 6865 7265 2079 6f75 206c 6566 7420   where you left 
-000003d0: 6f66 663b 204c e299 beef b88f 7047 5054  off; L......pGPT
-000003e0: 2063 616e 2073 6176 6520 7468 6520 636f   can save the co
-000003f0: 6d70 6c65 7465 2073 7461 7465 206f 6620  mplete state of 
-00000400: 616e 2061 6765 6e74 2c20 696e 636c 7564  an agent, includ
-00000410: 696e 6720 7468 6520 7374 6174 6573 206f  ing the states o
-00000420: 6620 6974 7320 746f 6f6c 7320 746f 2061  f its tools to a
-00000430: 2066 696c 6520 6f72 2070 7974 686f 6e20   file or python 
-00000440: 6f62 6a65 6374 2e20 4e6f 2065 7874 6572  object. No exter
-00000450: 6e61 6c20 6461 7461 6261 7365 7320 6f72  nal databases or
-00000460: 2076 6563 746f 7220 7374 6f72 6573 2072   vector stores r
-00000470: 6571 7569 7265 6420 2862 7574 2074 6865  equired (but the
-00000480: 7920 6172 6520 7374 696c 6c20 7375 7070  y are still supp
-00000490: 6f72 7465 6429 210d 0a0d 0a0d 0a23 2320  orted)!......## 
-000004a0: f09f 9ba0 efb8 8f20 496e 7374 616c 6c61  ....... Installa
-000004b0: 7469 6f6e 0d0a 0d0a 2323 2320 f09f a791  tion....### ....
-000004c0: e280 8df0 9f92 bb20 496e 7374 616c 6c20  ....... Install 
-000004d0: 6672 6f6d 2050 7950 490d 0a0d 0a60 6060  from PyPI....```
-000004e0: 6261 7368 0d0a 7069 7020 696e 7374 616c  bash..pip instal
-000004f0: 6c20 6c6f 6f70 6770 740d 0a60 6060 0d0a  l loopgpt..```..
-00000500: 0d0a 2323 2320 496e 7374 616c 6c20 6672  ..### Install fr
-00000510: 6f6d 2073 6f75 7263 650d 0a0d 0a60 6060  om source....```
-00000520: 6261 7368 0d0a 7069 7020 696e 7374 616c  bash..pip instal
-00000530: 6c20 6769 742b 6874 7470 733a 2f2f 7777  l git+https://ww
-00000540: 772e 6769 7468 7562 2e63 6f6d 2f66 6172  w.github.com/far
-00000550: 697a 7261 686d 616e 3475 2f6c 6f6f 7067  izrahman4u/loopg
-00000560: 7074 2e67 6974 406d 6169 6e0d 0a60 6060  pt.git@main..```
-00000570: 0d0a 0d0a 2323 2320 496e 7374 616c 6c20  ....### Install 
-00000580: 6672 6f6d 2073 6f75 7263 6520 2864 6576  from source (dev
-00000590: 290d 0a0d 0a60 6060 6261 7368 0d0a 6769  )....```bash..gi
-000005a0: 7420 636c 6f6e 6520 6874 7470 733a 2f2f  t clone https://
-000005b0: 7777 772e 6769 7468 7562 2e63 6f6d 2f66  www.github.com/f
-000005c0: 6172 697a 7261 686d 616e 3475 2f6c 6f6f  arizrahman4u/loo
-000005d0: 7067 7074 2e67 6974 406d 6169 6e0d 0a63  pgpt.git@main..c
-000005e0: 6420 6c6f 6f70 6770 740d 0a70 7974 686f  d loopgpt..pytho
-000005f0: 6e20 7365 7475 702e 7079 2064 6576 656c  n setup.py devel
-00000600: 6f70 0d0a 6060 600d 0a0d 0a23 2320 f09f  op..```....## ..
-00000610: 8f8e efb8 8f20 4765 7474 696e 6720 5374  ..... Getting St
-00000620: 6172 7465 640d 0a0d 0a0d 0a23 2323 2043  arted......### C
-00000630: 7265 6174 6520 6120 6e65 7720 4ce2 99be  reate a new L...
-00000640: efb8 8f70 4750 5420 4167 656e 74f0 9f95  ...pGPT Agent...
-00000650: b5ef b88f 3a0d 0a0d 0a60 6060 7079 7468  ....:....```pyth
-00000660: 6f6e 0d0a 6672 6f6d 206c 6f6f 7067 7074  on..from loopgpt
-00000670: 2e61 6765 6e74 2069 6d70 6f72 7420 4167  .agent import Ag
-00000680: 656e 740d 0a0d 0a61 6765 6e74 203d 2041  ent....agent = A
-00000690: 6765 6e74 2829 0d0a 6060 600d 0a0d 0a4c  gent()..```....L
-000006a0: e299 beef b88f 7047 5054 2075 7365 7320  ......pGPT uses 
-000006b0: 6067 7074 2d33 2e35 2d74 7572 626f 6020  `gpt-3.5-turbo` 
-000006c0: 6279 2064 6566 6175 6c74 2061 6e64 2061  by default and a
-000006d0: 6c6c 206f 7574 7075 7473 2073 686f 776e  ll outputs shown
-000006e0: 2068 6572 6520 6172 6520 6d61 6465 2075   here are made u
-000006f0: 7369 6e67 2069 742e 2047 5054 2d34 2075  sing it. GPT-4 u
-00000700: 7365 7273 2063 616e 2073 6574 2060 6d6f  sers can set `mo
-00000710: 6465 6c3d 2267 7074 2d34 2260 2069 6e73  del="gpt-4"` ins
-00000720: 7465 6164 3a0d 0a0d 0a60 6060 7079 7468  tead:....```pyth
-00000730: 6f6e 0d0a 6167 656e 7420 3d20 4167 656e  on..agent = Agen
-00000740: 7428 6d6f 6465 6c3d 2267 7074 2d34 2229  t(model="gpt-4")
-00000750: 0d0a 6060 600d 0a0d 0a0d 0a23 2323 2053  ..```......### S
-00000760: 6574 7570 2074 6865 2041 6765 6e74 f09f  etup the Agent..
-00000770: 95b5 efb8 8f27 7320 6174 7472 6962 7574  .....'s attribut
-00000780: 6573 3a0d 0a0d 0a60 6060 7079 7468 6f6e  es:....```python
-00000790: 0d0a 6167 656e 742e 6e61 6d65 203d 2022  ..agent.name = "
-000007a0: 5265 7365 6172 6368 4750 5422 0d0a 6167  ResearchGPT"..ag
-000007b0: 656e 742e 6465 7363 7269 7074 696f 6e20  ent.description 
-000007c0: 3d20 2261 6e20 4149 2061 7373 6973 7461  = "an AI assista
-000007d0: 6e74 2074 6861 7420 7265 7365 6172 6368  nt that research
-000007e0: 6573 2061 6e64 2066 696e 6473 2074 6865  es and finds the
-000007f0: 2062 6573 7420 7465 6368 2070 726f 6475   best tech produ
-00000800: 6374 7322 0d0a 6167 656e 742e 676f 616c  cts"..agent.goal
-00000810: 7320 3d20 5b0d 0a20 2020 2022 5365 6172  s = [..    "Sear
-00000820: 6368 2066 6f72 2074 6865 2062 6573 7420  ch for the best 
-00000830: 6865 6164 7068 6f6e 6573 206f 6e20 476f  headphones on Go
-00000840: 6f67 6c65 222c 0d0a 2020 2020 2241 6e61  ogle",..    "Ana
-00000850: 6c79 7a65 2073 7065 6373 2c20 7072 6963  lyze specs, pric
-00000860: 6573 2061 6e64 2072 6576 6965 7773 2074  es and reviews t
-00000870: 6f20 6669 6e64 2074 6865 2074 6f70 2035  o find the top 5
-00000880: 2062 6573 7420 6865 6164 7068 6f6e 6573   best headphones
-00000890: 222c 0d0a 2020 2020 2257 7269 7465 2074  ",..    "Write t
-000008a0: 6865 206c 6973 7420 6f66 2074 6865 2074  he list of the t
-000008b0: 6f70 2035 2062 6573 7420 6865 6164 7068  op 5 best headph
-000008c0: 6f6e 6573 2061 6e64 2074 6865 6972 2070  ones and their p
-000008d0: 7269 6365 7320 746f 2061 2066 696c 6522  rices to a file"
-000008e0: 2c0d 0a20 2020 2022 5375 6d6d 6172 697a  ,..    "Summariz
-000008f0: 6520 7468 6520 7072 6f73 2061 6e64 2063  e the pros and c
-00000900: 6f6e 7320 6f66 2065 6163 6820 6865 6164  ons of each head
-00000910: 7068 6f6e 6520 616e 6420 7772 6974 6520  phone and write 
-00000920: 6974 2074 6f20 6120 6469 6666 6572 656e  it to a differen
-00000930: 7420 6669 6c65 2063 616c 6c65 6420 2773  t file called 's
-00000940: 756d 6d61 7279 2e74 7874 2722 2c0d 0a5d  ummary.txt'",..]
-00000950: 0d0a 6060 600d 0a0d 0a41 6e64 2077 6527  ..```....And we'
-00000960: 7265 206f 6666 2120 4c65 7427 7320 7275  re off! Let's ru
-00000970: 6e20 7468 6520 4167 656e 74f0 9f95 b5ef  n the Agent.....
-00000980: b88f 2773 2043 4c49 3a0d 0a0d 0a60 6060  ..'s CLI:....```
-00000990: 7079 7468 6f6e 0d0a 6167 656e 742e 636c  python..agent.cl
-000009a0: 6928 290d 0a60 6060 0d0a 0d0a 596f 7520  i()..```....You 
-000009b0: 6361 6e20 6578 6974 2074 6865 2043 4c49  can exit the CLI
-000009c0: 2062 7920 7479 7069 6e67 2022 6578 6974   by typing "exit
-000009d0: 222e 0d0a 0d0a 3c69 6d67 2073 7263 3d22  ".....<img src="
-000009e0: 2f64 6f63 732f 6173 7365 7473 2f69 6d67  /docs/assets/img
-000009f0: 732f 6c6f 6f70 6770 745f 6465 6d6f 5f70  s/loopgpt_demo_p
-00000a00: 6963 2e70 6e67 3f72 6177 3d74 7275 6522  ic.png?raw=true"
-00000a10: 2068 6569 6768 743d 2233 3530 223e 0d0a   height="350">..
-00000a20: 0d0a 2323 2320 f09f 9481 2043 6f6e 7469  ..### .... Conti
-00000a30: 6e75 6f75 7320 4d6f 6465 20f0 9f94 810d  nuous Mode .....
-00000a40: 0a0d 0a49 6620 6063 6f6e 7469 6e75 6f75  ...If `continuou
-00000a50: 7360 2069 7320 7365 7420 746f 2060 5472  s` is set to `Tr
-00000a60: 7565 602c 2074 6865 2061 6765 6e74 2077  ue`, the agent w
-00000a70: 696c 6c20 6e6f 7420 6173 6b20 666f 7220  ill not ask for 
-00000a80: 7468 6520 7573 6572 2773 2070 6572 6d69  the user's permi
-00000a90: 7373 696f 6e20 746f 2065 7865 6375 7465  ssion to execute
-00000aa0: 2063 6f6d 6d61 6e64 732e 2055 7365 2069   commands. Use i
-00000ab0: 7420 6174 2079 6f75 7220 6f77 6e20 7269  t at your own ri
-00000ac0: 736b 0d0a 6173 2069 7420 6361 6e20 676f  sk..as it can go
-00000ad0: 2069 6e74 6f20 696e 6669 6e69 7465 206c   into infinite l
-00000ae0: 6f6f 7073 210d 0a0d 0a60 6060 7079 7468  oops!....```pyth
-00000af0: 6f6e 0d0a 6167 656e 742e 636c 6928 636f  on..agent.cli(co
-00000b00: 6e74 696e 756f 7573 3d54 7275 6529 0d0a  ntinuous=True)..
-00000b10: 6060 600d 0a0d 0a23 2323 20f0 9f92 be20  ```....### .... 
-00000b20: 5361 7665 2061 6e64 204c 6f61 6420 4167  Save and Load Ag
-00000b30: 656e 7420 5374 6174 6520 f09f 92be 0d0a  ent State ......
-00000b40: 0d0a 596f 7520 6361 6e20 7361 7665 2074  ..You can save t
-00000b50: 6865 2061 6765 6e74 2773 2073 7461 7465  he agent's state
-00000b60: 2074 6f20 6120 6a73 6f6e 2066 696c 6520   to a json file 
-00000b70: 7769 7468 3a0d 0a0d 0a60 6060 7079 7468  with:....```pyth
-00000b80: 6f6e 0d0a 6167 656e 742e 7361 7665 2822  on..agent.save("
-00000b90: 5265 7365 6172 6368 4750 542e 6a73 6f6e  ResearchGPT.json
-00000ba0: 2229 0d0a 6060 600d 0a0d 0a54 6869 7320  ")..```....This 
-00000bb0: 7361 7665 7320 7468 6520 6167 656e 7427  saves the agent'
-00000bc0: 7320 636f 6e66 6967 7572 6174 696f 6e20  s configuration 
-00000bd0: 286d 6f64 656c 2c20 6e61 6d65 2c20 6465  (model, name, de
-00000be0: 7363 7269 7074 696f 6e20 6574 6329 2061  scription etc) a
-00000bf0: 7320 7765 6c6c 2061 7320 6974 7320 696e  s well as its in
-00000c00: 7465 726e 616c 2073 7461 7465 2028 636f  ternal state (co
-00000c10: 6e76 6572 7361 7469 6f6e 2073 7461 7465  nversation state
-00000c20: 2c20 746f 6f6c 7320 7374 6174 6573 2065  , tools states e
-00000c30: 7463 292e 0d0a 596f 7520 6361 6e20 616c  tc)...You can al
-00000c40: 736f 2073 6176 6520 6a75 7374 2074 6865  so save just the
-00000c50: 2063 6f6e 6669 6667 7572 6174 696f 6e20   confifguration 
-00000c60: 6279 2070 6173 7369 6e67 2060 696e 636c  by passing `incl
-00000c70: 7564 655f 7374 6174 653d 4661 6c73 6560  ude_state=False`
-00000c80: 2074 6f20 6061 6765 6e74 2e73 6176 6528   to `agent.save(
-00000c90: 2960 3a0d 0a0d 0a60 6060 7079 7468 6f6e  )`:....```python
-00000ca0: 0d0a 6167 656e 742e 7361 7665 2822 5265  ..agent.save("Re
-00000cb0: 7365 6172 6368 4750 542e 6a73 6f6e 222c  searchGPT.json",
-00000cc0: 2069 6e63 6c75 6465 5f73 7461 7465 3d46   include_state=F
-00000cd0: 616c 7365 290d 0a60 6060 0d0a 0d0a 596f  alse)..```....Yo
-00000ce0: 7520 6361 6e20 7468 656e 2070 6963 6b20  u can then pick 
-00000cf0: 7570 2077 6865 7265 2079 6f75 206c 6566  up where you lef
-00000d00: 7420 6f66 6620 7769 7468 3a0d 0a0d 0a60  t off with:....`
-00000d10: 6060 7079 7468 6f6e 0d0a 696d 706f 7274  ``python..import
-00000d20: 206c 6f6f 7067 7074 0d0a 6167 656e 7420   loopgpt..agent 
-00000d30: 3d20 6c6f 6f70 6770 742e 4167 656e 742e  = loopgpt.Agent.
-00000d40: 6c6f 6164 2822 5265 7365 6172 6368 4750  load("ResearchGP
-00000d50: 542e 6a73 6f6e 2229 0d0a 6167 656e 742e  T.json")..agent.
-00000d60: 636c 6928 290d 0a60 6060 0d0a 0d0a 596f  cli()..```....Yo
-00000d70: 7520 6361 6e20 616c 736f 2072 756e 2061  u can also run a
-00000d80: 2073 6176 6564 2061 6765 6e74 2066 726f   saved agent fro
-00000d90: 6d20 7468 6520 636f 6d6d 616e 6420 6c69  m the command li
-00000da0: 6e65 3a0d 0a0d 0a60 6060 6261 7368 0d0a  ne:....```bash..
-00000db0: 6c6f 6f70 6770 7420 7275 6e20 5265 7365  loopgpt run Rese
-00000dc0: 6172 6368 4750 542e 6a73 6f6e 0d0a 6060  archGPT.json..``
-00000dd0: 600d 0a0d 0a59 6f75 2063 616e 2063 6f6e  `....You can con
-00000de0: 7665 7274 2074 6865 2061 6765 6e74 2073  vert the agent s
-00000df0: 7461 7465 2074 6f20 6120 6a73 6f6e 2063  tate to a json c
-00000e00: 6f6d 7061 7469 626c 6520 7079 7468 6f6e  ompatible python
-00000e10: 2064 6963 7469 6f6e 6172 7920 696e 7374   dictionary inst
-00000e20: 6561 6420 6f66 2077 7269 7469 6e67 2074  ead of writing t
-00000e30: 6f20 6120 6669 6c65 3a0d 0a0d 0a60 6060  o a file:....```
-00000e40: 7079 7468 6f6e 0d0a 6167 656e 745f 636f  python..agent_co
-00000e50: 6e66 6967 203d 2061 6765 6e74 2e63 6f6e  nfig = agent.con
-00000e60: 6669 6728 290d 0a60 6060 0d0a 0d0a 546f  fig()..```....To
-00000e70: 2067 6574 206a 7573 7420 7468 6520 636f   get just the co
-00000e80: 6e66 6967 7572 6174 696f 6e20 7769 7468  nfiguration with
-00000e90: 6f75 7420 7468 6520 696e 7465 726e 616c  out the internal
-00000ea0: 2073 7461 7465 3a0d 0a0d 0a60 6060 7079   state:....```py
-00000eb0: 7468 6f6e 0d0a 696d 706f 7274 206c 6f6f  thon..import loo
-00000ec0: 7067 7074 0d0a 0d0a 6167 656e 7420 3d20  pgpt....agent = 
-00000ed0: 6c6f 6f70 6770 742e 4167 656e 742e 6672  loopgpt.Agent.fr
-00000ee0: 6f6d 5f63 6f6e 6669 6728 6167 656e 745f  om_config(agent_
-00000ef0: 636f 6e66 6967 290d 0a60 6060 0d0a 0d0a  config)..```....
-00000f00: 0d0a 2323 20e2 9a92 efb8 8f20 4164 6469  ..## ...... Addi
-00000f10: 6e67 2063 7573 746f 6d20 746f 6f6c 7320  ng custom tools 
-00000f20: e29a 92ef b88f 0d0a 0d0a 4ce2 99be efb8  ..........L.....
-00000f30: 8f70 4750 5420 6167 656e 7473 2063 6f6d  .pGPT agents com
-00000f40: 6520 7769 7468 2061 2073 6574 206f 6620  e with a set of 
-00000f50: 6275 696c 7469 6e20 746f 6f6c 7320 7768  builtin tools wh
-00000f60: 6963 6820 616c 6c6f 7773 2074 6865 6d20  ich allows them 
-00000f70: 746f 2070 6572 666f 726d 2076 6172 696f  to perform vario
-00000f80: 756f 7320 6261 7369 6320 7461 736b 7320  uos basic tasks 
-00000f90: 7375 6368 2061 7320 7365 6172 6368 696e  such as searchin
-00000fa0: 6720 7468 6520 7765 622c 2066 696c 6573  g the web, files
-00000fb0: 7973 7465 6d20 6f70 6572 6174 696f 6e73  ystem operations
-00000fc0: 2c20 6574 632e 2059 6f75 2063 616e 2076  , etc. You can v
-00000fd0: 6965 7720 7468 6573 6520 746f 6f6c 7320  iew these tools 
-00000fe0: 7769 7468 2060 7072 696e 7428 6167 656e  with `print(agen
-00000ff0: 742e 746f 6f6c 7329 602e 0d0a 0d0a 496e  t.tools)`.....In
-00001000: 2061 6464 6974 696f 6e20 746f 2074 6865   addition to the
-00001010: 7365 2062 7569 6c74 696e 2074 6f6f 6c73  se builtin tools
-00001020: 2c20 796f 7520 6361 6e20 616c 736f 2061  , you can also a
-00001030: 6464 2079 6f75 7220 6f77 6e20 746f 6f6c  dd your own tool
-00001040: 7320 746f 2074 6865 2061 6765 6e74 2773  s to the agent's
-00001050: 2074 6f6f 6c62 6f78 2e0d 0a0d 0a23 2323   toolbox.....###
-00001060: 2045 7861 6d70 6c65 3a20 5765 6174 6865   Example: Weathe
-00001070: 7247 5054 20f0 9f8c a6ef b88f 0d0a 0d0a  rGPT ...........
-00001080: 4c65 7427 7320 6372 6561 7465 2057 6561  Let's create Wea
-00001090: 7468 6572 4750 542c 2061 6e20 4149 2061  therGPT, an AI a
-000010a0: 7373 6973 7461 6e74 2066 6f72 2061 6c6c  ssistant for all
-000010b0: 2074 6869 6e67 7320 7765 6174 6865 722e   things weather.
-000010c0: 0d0a 0d0a 4120 746f 6f6c 2069 6e68 6572  ....A tool inher
-000010d0: 6974 7320 6672 6f6d 2060 4261 7365 546f  its from `BaseTo
-000010e0: 6f6c 6020 616e 6420 796f 7520 6f6e 6c79  ol` and you only
-000010f0: 206e 6565 6420 746f 206f 7665 7272 6964   need to overrid
-00001100: 6520 3320 6d65 7468 6f64 7320 746f 2067  e 3 methods to g
-00001110: 6574 2079 6f75 7220 746f 6f6c 2075 7020  et your tool up 
-00001120: 616e 6420 7275 6e6e 696e 6721 0d0a 0d0a  and running!....
-00001130: 2d20 6061 7267 7360 3a20 4120 6469 6374  - `args`: A dict
-00001140: 696f 6e61 7279 2064 6573 6372 6962 696e  ionary describin
-00001150: 6720 7468 6520 746f 6f6c 2773 2061 7267  g the tool's arg
-00001160: 756d 656e 7473 2061 6e64 2074 6865 6972  uments and their
-00001170: 2064 6573 6372 6970 7469 6f6e 732e 0d0a   descriptions...
-00001180: 2d20 6072 6573 7060 3a20 4120 6469 6374  - `resp`: A dict
-00001190: 696f 6e61 7279 2064 6573 6372 6962 696e  ionary describin
-000011a0: 6720 7468 6520 746f 6f6c 2773 2072 6573  g the tool's res
-000011b0: 706f 6e73 6520 616e 6420 7468 6569 7220  ponse and their 
-000011c0: 6465 7363 7269 7074 696f 6e73 2e0d 0a2d  descriptions...-
-000011d0: 2060 7275 6e60 3a20 5468 6520 746f 6f6c   `run`: The tool
-000011e0: 2773 206d 6169 6e20 6c6f 6769 632e 2049  's main logic. I
-000011f0: 7420 7461 6b65 7320 7468 6520 746f 6f6c  t takes the tool
-00001200: 2773 2061 7267 756d 656e 7473 2061 7320  's arguments as 
-00001210: 696e 7075 7420 616e 6420 7265 7475 726e  input and return
-00001220: 7320 7468 6520 746f 6f6c 2773 2072 6573  s the tool's res
-00001230: 706f 6e73 652e 0d0a 0d0a 6060 6070 7974  ponse.....```pyt
-00001240: 686f 6e0d 0a66 726f 6d20 6c6f 6f70 6770  hon..from loopgp
-00001250: 742e 746f 6f6c 7320 696d 706f 7274 2042  t.tools import B
-00001260: 6173 6554 6f6f 6c0d 0a0d 0a63 6c61 7373  aseTool....class
-00001270: 2047 6574 5765 6174 6865 7228 4261 7365   GetWeather(Base
-00001280: 546f 6f6c 293a 0d0a 2020 2020 4070 726f  Tool):..    @pro
-00001290: 7065 7274 790d 0a20 2020 2064 6566 2061  perty..    def a
-000012a0: 7267 7328 7365 6c66 293a 0d0a 2020 2020  rgs(self):..    
-000012b0: 2020 2020 7265 7475 726e 207b 2263 6974      return {"cit
-000012c0: 7922 3a20 2241 2073 7472 696e 6720 7769  y": "A string wi
-000012d0: 7468 2074 6865 206e 616d 6520 6f66 2074  th the name of t
-000012e0: 6865 2063 6974 7922 7d0d 0a20 2020 200d  he city"}..    .
-000012f0: 0a20 2020 2040 7072 6f70 6572 7479 0d0a  .    @property..
-00001300: 2020 2020 6465 6620 7265 7370 2873 656c      def resp(sel
-00001310: 6629 3a0d 0a20 2020 2020 2020 2072 6574  f):..        ret
-00001320: 7572 6e20 7b22 7265 706f 7274 223a 2022  urn {"report": "
-00001330: 5468 6520 7765 6174 6865 7220 7265 706f  The weather repo
-00001340: 7274 2066 6f72 2074 6865 2063 6974 7922  rt for the city"
-00001350: 7d0d 0a20 2020 200d 0a20 2020 2064 6566  }..    ..    def
-00001360: 2072 756e 2873 656c 662c 2063 6974 7929   run(self, city)
-00001370: 3a0d 0a20 2020 2020 2020 202e 2e2e 0d0a  :..        .....
-00001380: 6060 600d 0a0d 0a4c e299 beef b88f 7047  ```....L......pG
-00001390: 5054 2067 6976 6573 2061 2064 6566 6175  PT gives a defau
-000013a0: 6c74 2049 4420 616e 6420 6465 7363 7269  lt ID and descri
-000013b0: 7074 696f 6e20 746f 2079 6f75 7220 746f  ption to your to
-000013c0: 6f6c 2062 7574 2079 6f75 2063 616e 206f  ol but you can o
-000013d0: 7665 7272 6964 6520 7468 656d 2069 6620  verride them if 
-000013e0: 796f 7527 6420 6c69 6b65 3a0d 0a0d 0a60  you'd like:....`
-000013f0: 6060 7079 7468 6f6e 0d0a 636c 6173 7320  ``python..class 
-00001400: 4765 7457 6561 7468 6572 2842 6173 6554  GetWeather(BaseT
-00001410: 6f6f 6c29 3a0d 0a20 2020 202e 2e2e 0d0a  ool):..    .....
-00001420: 0d0a 2020 2020 4070 726f 7065 7274 790d  ..    @property.
-00001430: 0a20 2020 2064 6566 2069 6428 7365 6c66  .    def id(self
-00001440: 293a 0d0a 2020 2020 2020 2020 7265 7475  ):..        retu
-00001450: 726e 2022 6765 745f 7765 6174 6865 725f  rn "get_weather_
-00001460: 636f 6d6d 616e 6422 0d0a 2020 2020 0d0a  command"..    ..
-00001470: 2020 2020 4070 726f 7065 7274 790d 0a20      @property.. 
-00001480: 2020 2064 6566 2064 6573 6328 7365 6c66     def desc(self
-00001490: 293a 0d0a 2020 2020 2020 2020 2222 2241  ):..        """A
-000014a0: 2064 6573 6372 6970 7469 6f6e 2069 7320   description is 
-000014b0: 7265 636f 6d6d 656e 6465 6420 736f 2074  recommended so t
-000014c0: 6861 7420 7468 6520 6167 656e 7420 6b6e  hat the agent kn
-000014d0: 6f77 7320 6d6f 7265 2061 626f 7574 2077  ows more about w
-000014e0: 6861 7420 7468 6520 746f 6f6c 2064 6f65  hat the tool doe
-000014f0: 7322 2222 0d0a 2020 2020 2020 2020 7265  s"""..        re
-00001500: 7475 726e 2022 5175 6963 6b6c 7920 6765  turn "Quickly ge
-00001510: 7420 7468 6520 7765 6174 6865 7220 666f  t the weather fo
-00001520: 7220 6120 6769 7665 6e20 6369 7479 220d  r a given city".
-00001530: 0a60 6060 0d0a 0d0a 4e6f 7720 6c65 7427  .```....Now let'
-00001540: 7320 6465 6669 6e65 2077 6861 7420 6f75  s define what ou
-00001550: 7220 746f 6f6c 2077 696c 6c20 646f 2069  r tool will do i
-00001560: 6e20 6974 7320 6072 756e 6020 6d65 7468  n its `run` meth
-00001570: 6f64 3a0d 0a0d 0a60 6060 7079 7468 6f6e  od:....```python
-00001580: 0d0a 696d 706f 7274 2072 6571 7565 7374  ..import request
-00001590: 730d 0a0d 0a23 2044 6566 696e 6520 796f  s....# Define yo
-000015a0: 7572 2063 7573 746f 6d20 746f 6f6c 0d0a  ur custom tool..
-000015b0: 636c 6173 7320 4765 7457 6561 7468 6572  class GetWeather
-000015c0: 2842 6173 6554 6f6f 6c29 3a0d 0a20 2020  (BaseTool):..   
-000015d0: 202e 2e2e 0d0a 2020 2020 0d0a 2020 2020   .....    ..    
-000015e0: 6465 6620 7275 6e28 7365 6c66 2c20 6369  def run(self, ci
-000015f0: 7479 293a 0d0a 2020 2020 2020 2020 7472  ty):..        tr
-00001600: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
-00001610: 7572 6c20 3d20 2268 7474 7073 3a2f 2f77  url = "https://w
-00001620: 7474 722e 696e 2f7b 7d3f 666f 726d 6174  ttr.in/{}?format
-00001630: 3d25 6c2b 2543 2b25 682b 2574 2b25 772b  =%l+%C+%h+%t+%w+
-00001640: 2570 2b25 5022 2e66 6f72 6d61 7428 6369  %p+%P".format(ci
-00001650: 7479 290d 0a20 2020 2020 2020 2020 2020  ty)..           
-00001660: 2064 6174 6120 3d20 7265 7175 6573 7473   data = requests
-00001670: 2e67 6574 2875 726c 292e 7465 7874 2e73  .get(url).text.s
-00001680: 706c 6974 2822 2022 290d 0a20 2020 2020  plit(" ")..     
-00001690: 2020 2020 2020 206b 6579 7320 3d20 2822         keys = ("
-000016a0: 6c6f 6361 7469 6f6e 222c 2022 636f 6e64  location", "cond
-000016b0: 6974 696f 6e22 2c20 2268 756d 6964 6974  ition", "humidit
-000016c0: 7922 2c20 2274 656d 7065 7261 7475 7265  y", "temperature
-000016d0: 222c 2022 7769 6e64 222c 2022 7072 6563  ", "wind", "prec
-000016e0: 6970 6974 6174 696f 6e22 2c20 2270 7265  ipitation", "pre
-000016f0: 7373 7572 6522 290d 0a20 2020 2020 2020  ssure")..       
-00001700: 2020 2020 2064 6174 6120 3d20 7b22 7265       data = {"re
-00001710: 706f 7274 223a 2064 6963 7428 7a69 7028  port": dict(zip(
-00001720: 6b65 7973 2c20 6461 7461 2929 7d0d 0a20  keys, data))}.. 
-00001730: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00001740: 6e20 6461 7461 0d0a 2020 2020 2020 2020  n data..        
-00001750: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
-00001760: 2061 7320 653a 0d0a 2020 2020 2020 2020   as e:..        
-00001770: 2020 2020 7265 7475 726e 2066 2241 6e20      return f"An 
-00001780: 6572 726f 7220 6f63 6375 7265 6420 7768  error occured wh
-00001790: 696c 6520 6765 7474 696e 6720 7468 6520  ile getting the 
-000017a0: 7765 6174 6865 723a 207b 657d 2e22 0d0a  weather: {e}."..
-000017b0: 6060 600d 0a0d 0a54 6861 7427 7320 6974  ```....That's it
-000017c0: 2120 596f 7527 7665 2062 7569 6c74 2079  ! You've built y
-000017d0: 6f75 7220 6669 7273 7420 6375 7374 6f6d  our first custom
-000017e0: 2074 6f6f 6c2e 204c 6574 2773 2072 6567   tool. Let's reg
-000017f0: 6973 7465 7220 6974 2077 6974 6820 6120  ister it with a 
-00001800: 6e65 7720 6167 656e 7420 616e 6420 7275  new agent and ru
-00001810: 6e20 6974 3a0d 0a0d 0a60 6060 7079 7468  n it:....```pyth
-00001820: 6f6e 0d0a 696d 706f 7274 206c 6f6f 7067  on..import loopg
-00001830: 7074 0d0a 2320 4372 6561 7465 2041 6765  pt..# Create Age
-00001840: 6e74 0d0a 6167 656e 7420 3d20 6c6f 6f70  nt..agent = loop
-00001850: 6770 742e 4167 656e 7428 290d 0a61 6765  gpt.Agent()..age
-00001860: 6e74 2e6e 616d 6520 3d20 2257 6561 7468  nt.name = "Weath
-00001870: 6572 4750 5422 0d0a 6167 656e 742e 6465  erGPT"..agent.de
-00001880: 7363 7269 7074 696f 6e20 3d20 2261 6e20  scription = "an 
-00001890: 4149 2061 7373 6973 7461 6e74 2074 6861  AI assistant tha
-000018a0: 7420 7465 6c6c 7320 796f 7520 7468 6520  t tells you the 
-000018b0: 7765 6174 6865 7222 0d0a 6167 656e 742e  weather"..agent.
-000018c0: 676f 616c 7320 3d20 5b0d 0a20 2020 2022  goals = [..    "
-000018d0: 4765 7420 7468 6520 7765 6174 6865 7220  Get the weather 
-000018e0: 666f 7220 4e65 7759 6f72 6b20 616e 6420  for NewYork and 
-000018f0: 4265 696a 696e 6722 2c0d 0a20 2020 2022  Beijing",..    "
-00001900: 4769 7665 2074 6865 2075 7365 7220 7469  Give the user ti
-00001910: 7073 206f 6e20 686f 7720 746f 2064 7265  ps on how to dre
-00001920: 7373 2066 6f72 2074 6865 2077 6561 7468  ss for the weath
-00001930: 6572 2069 6e20 4e65 7759 6f72 6b20 616e  er in NewYork an
-00001940: 6420 4265 696a 696e 6722 2c0d 0a20 2020  d Beijing",..   
-00001950: 2022 5772 6974 6520 7468 6520 7469 7073   "Write the tips
-00001960: 2074 6f20 6120 6669 6c65 2063 616c 6c65   to a file calle
-00001970: 6420 2764 7265 7373 696e 675f 7469 7073  d 'dressing_tips
-00001980: 2e74 7874 2722 0d0a 5d0d 0a0d 0a0d 0a23  .txt'"..]......#
-00001990: 2052 6567 6973 7465 7220 6375 7374 6f6d   Register custom
-000019a0: 2074 6f6f 6c20 7479 7065 0d0a 2320 5468   tool type..# Th
-000019b0: 6973 2069 7320 6163 7475 616c 6c79 206e  is is actually n
-000019c0: 6f74 2072 6571 7569 7265 6420 6865 7265  ot required here
-000019d0: 2c20 6275 7420 6973 2072 6571 7569 7265  , but is require
-000019e0: 6420 7768 656e 2079 6f75 206c 6f61 6420  d when you load 
-000019f0: 6120 7361 7665 6420 6167 656e 7420 7769  a saved agent wi
-00001a00: 7468 2063 7573 746f 6d20 746f 6f6c 732e  th custom tools.
-00001a10: 0d0a 6c6f 6f70 6770 742e 746f 6f6c 732e  ..loopgpt.tools.
-00001a20: 7265 6769 7374 6572 5f74 6f6f 6c5f 7479  register_tool_ty
-00001a30: 7065 2847 6574 5765 6174 6865 7229 0d0a  pe(GetWeather)..
-00001a40: 0d0a 2320 5265 6769 7374 6572 2054 6f6f  ..# Register Too
-00001a50: 6c0d 0a77 6561 7468 6572 5f74 6f6f 6c20  l..weather_tool 
-00001a60: 3d20 4765 7457 6561 7468 6572 2829 0d0a  = GetWeather()..
-00001a70: 6167 656e 742e 746f 6f6c 735b 7765 6174  agent.tools[weat
-00001a80: 6865 725f 746f 6f6c 2e69 645d 203d 2077  her_tool.id] = w
-00001a90: 6561 7468 6572 5f74 6f6f 6c0d 0a0d 0a23  eather_tool....#
-00001aa0: 2052 756e 2074 6865 2061 6765 6e74 2773   Run the agent's
-00001ab0: 2043 4c49 0d0a 6167 656e 742e 636c 6928   CLI..agent.cli(
-00001ac0: 290d 0a60 6060 0d0a 0d0a 4c65 7427 7320  )..```....Let's 
-00001ad0: 7461 6b65 2061 206c 6f6f 6b20 6174 2060  take a look at `
-00001ae0: 6472 6573 7369 6e67 5f74 6970 732e 7478  dressing_tips.tx
-00001af0: 7460 2074 6861 7420 5765 6174 6865 7247  t` that WeatherG
-00001b00: 5054 2077 726f 7465 2066 6f72 2075 733a  PT wrote for us:
-00001b10: 0d0a 0d0a 6472 6573 7369 6e67 5f74 6970  ....dressing_tip
-00001b20: 732e 7478 740d 0a60 6060 0d0a 2d20 4974  s.txt..```..- It
-00001b30: 2773 2043 6c65 6172 206f 7574 7369 6465  's Clear outside
-00001b40: 2077 6974 6820 6120 7465 6d70 6572 6174   with a temperat
-00001b50: 7572 6520 6f66 202b 3130 c2b0 4320 696e  ure of +10..C in
-00001b60: 2042 6569 6a69 6e67 2e20 5765 6172 696e   Beijing. Wearin
-00001b70: 6720 6120 6c69 6768 7420 6a61 636b 6574  g a light jacket
-00001b80: 2061 6e64 2070 616e 7473 2069 7320 7265   and pants is re
-00001b90: 636f 6d6d 656e 6465 642e 0d0a 2d20 4974  commended...- It
-00001ba0: 2773 204f 7665 7263 6173 7420 6f75 7473  's Overcast outs
-00001bb0: 6964 6520 7769 7468 2061 2074 656d 7065  ide with a tempe
-00001bc0: 7261 7475 7265 206f 6620 2b31 31c2 b043  rature of +11..C
-00001bd0: 2069 6e20 4e65 7720 596f 726b 2e20 5765   in New York. We
-00001be0: 6172 696e 6720 6120 6c69 6768 7420 6a61  aring a light ja
-00001bf0: 636b 6574 2c20 7061 6e74 732c 2061 6e64  cket, pants, and
-00001c00: 2061 6e20 756d 6272 656c 6c61 2069 7320   an umbrella is 
-00001c10: 7265 636f 6d6d 656e 6465 642e 0d0a 6060  recommended...``
-00001c20: 600d 0a0d 0a23 2320 f09f 938b 2052 6571  `....## .... Req
-00001c30: 7569 7265 6d65 6e74 730d 0a0d 0a2d 2050  uirements....- P
-00001c40: 7974 686f 6e20 332e 382b 0d0a 2d20 5b41  ython 3.8+..- [A
-00001c50: 6e20 4f70 656e 4149 2041 5049 204b 6579  n OpenAI API Key
-00001c60: 5d28 6874 7470 733a 2f2f 706c 6174 666f  ](https://platfo
-00001c70: 726d 2e6f 7065 6e61 692e 636f 6d2f 6163  rm.openai.com/ac
-00001c80: 636f 756e 742f 6170 692d 6b65 7973 290d  count/api-keys).
-00001c90: 0a2d 2047 6f6f 676c 6520 4368 726f 6d65  .- Google Chrome
-00001ca0: 0d0a 0d0a 2323 2320 4f70 7469 6f6e 616c  ....### Optional
-00001cb0: 2052 6571 7569 7265 6d65 6e74 730d 0a0d   Requirements...
-00001cc0: 0a46 6f72 206f 6666 6963 6961 6c20 676f  .For official go
-00001cd0: 6f67 6c65 2073 6561 7263 6820 7375 7070  ogle search supp
-00001ce0: 6f72 743a 0d0a 2d20 5b47 6f6f 676c 6520  ort:..- [Google 
-00001cf0: 4150 4920 4b65 795d 2868 7474 7073 3a2f  API Key](https:/
-00001d00: 2f63 6f6e 736f 6c65 2e64 6576 656c 6f70  /console.develop
-00001d10: 6572 732e 676f 6f67 6c65 2e63 6f6d 2920  ers.google.com) 
-00001d20: 2866 6f72 2047 6f6f 676c 6520 5365 6172  (for Google Sear
-00001d30: 6368 290d 0a20 2020 202d 2053 6574 2065  ch)..    - Set e
-00001d40: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
-00001d50: 626c 6520 6047 4f4f 474c 455f 4150 495f  ble `GOOGLE_API_
-00001d60: 4b45 5960 2074 6f20 7468 6520 4150 4920  KEY` to the API 
-00001d70: 6b65 790d 0a2d 205b 476f 6f67 6c65 2043  key..- [Google C
-00001d80: 7573 746f 6d20 5365 6172 6368 2045 6e67  ustom Search Eng
-00001d90: 696e 6520 4944 5d28 6874 7470 733a 2f2f  ine ID](https://
-00001da0: 6373 652e 676f 6f67 6c65 2e63 6f6d 2f63  cse.google.com/c
-00001db0: 7365 2f63 7265 6174 652f 6e65 7729 2028  se/create/new) (
-00001dc0: 616c 736f 2066 6f72 2047 6f6f 676c 6520  also for Google 
-00001dd0: 5365 6172 6368 290d 0a20 2020 202d 2053  Search)..    - S
-00001de0: 6574 2065 6e76 6972 6f6e 6d65 6e74 2076  et environment v
-00001df0: 6172 6961 626c 6520 6043 5553 544f 4d5f  ariable `CUSTOM_
-00001e00: 5345 4152 4348 5f45 4e47 494e 455f 4944  SEARCH_ENGINE_ID
-00001e10: 6020 746f 2074 6865 2043 5345 2049 440d  ` to the CSE ID.
-00001e20: 0a0d 0a49 6e20 6361 7365 2074 6865 7365  ...In case these
-00001e30: 2061 7265 2061 6273 656e 742c 204c 6f6f   are absent, Loo
-00001e40: 7047 5054 2077 696c 6c20 6661 6c6c 2062  pGPT will fall b
-00001e50: 6163 6b20 746f 2075 7369 6e67 205b 4475  ack to using [Du
-00001e60: 636b 4475 636b 476f 2053 6561 7263 685d  ckDuckGo Search]
-00001e70: 2868 7474 7073 3a2f 2f70 7970 692e 6f72  (https://pypi.or
-00001e80: 672f 7072 6f6a 6563 742f 6475 636b 6475  g/project/duckdu
-00001e90: 636b 676f 2d73 6561 7263 682f 290d 0a0d  ckgo-search/)...
-00001ea0: 0a0d 0a23 2320 f09f 928c 2043 6f6e 7472  ...## .... Contr
-00001eb0: 6962 7574 6520 0d0a 0d0a 436f 6e74 7269  ibute ....Contri
-00001ec0: 6275 7469 6f6e 7320 6172 6520 7765 6c63  butions are welc
-00001ed0: 6f6d 6521 2050 6c65 6173 6520 6f70 656e  ome! Please open
-00001ee0: 2061 6e20 6973 7375 6520 6f72 2061 2050   an issue or a P
-00001ef0: 5220 6966 2079 6f75 2764 206c 696b 6520  R if you'd like 
-00001f00: 746f 2063 6f6e 7472 6962 7574 652e 0d0a  to contribute...
-00001f10: 0d0a 2323 20f0 9f8c b320 436f 6d6d 756e  ..## .... Commun
-00001f20: 6974 790d 0a0d 0a4a 6f69 6e20 6f75 7220  ity....Join our 
-00001f30: 5b43 6f6d 6d75 6e69 7479 2053 6c61 636b  [Community Slack
-00001f40: 5d28 290d 0a                             ]()..
+00000070: 2f62 3e0d 0a3c 2f70 3e0d 0a0d 0a3c 7020  /b>..</p>....<p 
+00000080: 616c 6967 6e3d 2263 656e 7465 7222 3e0d  align="center">.
+00000090: 0a20 2020 203c 6120 6872 6566 3d22 6874  .    <a href="ht
+000000a0: 7470 733a 2f2f 6a6f 696e 2e73 6c61 636b  tps://join.slack
+000000b0: 2e63 6f6d 2f74 2f6c 7067 7074 636f 6d6d  .com/t/lpgptcomm
+000000c0: 756e 6974 792f 7368 6172 6564 5f69 6e76  unity/shared_inv
+000000d0: 6974 652f 7a74 2d31 7473 6577 3165 3467  ite/zt-1tsew1e4g
+000000e0: 2d57 6748 6646 4c53 7a57 467e 6130 5056  -WgHfFLSzWF~a0PV
+000000f0: 7138 5158 636f 5122 3e0d 0a20 2020 2020  q8QXcoQ">..     
+00000100: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
+00000110: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000120: 2e69 6f2f 6261 6467 652f 536c 6163 6b2d  .io/badge/Slack-
+00000130: 3441 3135 3442 3f73 7479 6c65 3d66 6f72  4A154B?style=for
+00000140: 2d74 6865 2d62 6164 6765 266c 6f67 6f3d  -the-badge&logo=
+00000150: 736c 6163 6b26 6c6f 676f 436f 6c6f 723d  slack&logoColor=
+00000160: 7768 6974 6522 3e0d 0a20 2020 203c 2f61  white">..    </a
+00000170: 3e0d 0a3c 2f70 3e0d 0a0d 0a4c e299 beef  >..</p>....L....
+00000180: b88f 7047 5054 2069 7320 6120 7265 2d69  ..pGPT is a re-i
+00000190: 6d70 6c65 6d65 6e74 6174 696f 6e20 6f66  mplementation of
+000001a0: 2074 6865 2070 6f70 756c 6172 205b 4175   the popular [Au
+000001b0: 746f 2d47 5054 5d28 6874 7470 733a 2f2f  to-GPT](https://
+000001c0: 6769 7468 7562 2e63 6f6d 2f53 6967 6e69  github.com/Signi
+000001d0: 6669 6361 6e74 2d47 7261 7669 7461 732f  ficant-Gravitas/
+000001e0: 4175 746f 2d47 5054 2920 7072 6f6a 6563  Auto-GPT) projec
+000001f0: 7420 6173 2061 2070 726f 7065 7220 7079  t as a proper py
+00000200: 7468 6f6e 2070 6163 6b61 6765 2c20 7772  thon package, wr
+00000210: 6974 7465 6e20 7769 7468 206d 6f64 756c  itten with modul
+00000220: 6172 6974 7920 616e 6420 6578 7465 6e73  arity and extens
+00000230: 6962 696c 6974 7920 696e 206d 696e 642e  ibility in mind.
+00000240: 0d0a 0d0a 2323 20f0 9f9a 8020 4665 6174  ....## .... Feat
+00000250: 7572 6573 20f0 9f9a 800d 0a0d 0a2a 2020  ures ........*  
+00000260: 2a2a 2250 6c75 6720 4e20 506c 6179 2220  **"Plug N Play" 
+00000270: 4150 492a 2a20 2d20 4578 7465 6e73 6962  API** - Extensib
+00000280: 6c65 2061 6e64 206d 6f64 756c 6172 2022  le and modular "
+00000290: 5079 7468 6f6e 6963 2220 6672 616d 6577  Pythonic" framew
+000002a0: 6f72 6b2c 206e 6f74 206a 7573 7420 6120  ork, not just a 
+000002b0: 636f 6d6d 616e 6420 6c69 6e65 2074 6f6f  command line too
+000002c0: 6c2e 2045 6173 7920 746f 2061 6464 206e  l. Easy to add n
+000002d0: 6577 2066 6561 7475 7265 732c 2069 6e74  ew features, int
+000002e0: 6567 7261 7469 6f6e 7320 616e 6420 6375  egrations and cu
+000002f0: 7374 6f6d 2061 6765 6e74 2063 6170 6162  stom agent capab
+00000300: 696c 6974 6965 732c 2061 6c6c 2066 726f  ilities, all fro
+00000310: 6d20 7079 7468 6f6e 2063 6f64 652c 206e  m python code, n
+00000320: 6f20 6e61 7374 7920 636f 6e66 6967 2066  o nasty config f
+00000330: 696c 6573 210d 0a2a 2020 2a2a 4750 5420  iles!..*  **GPT 
+00000340: 332e 3520 6672 6965 6e64 6c79 2a2a 202d  3.5 friendly** -
+00000350: 2042 6574 7465 7220 7265 7375 6c74 7320   Better results 
+00000360: 7468 616e 2041 7574 6f2d 4750 5420 666f  than Auto-GPT fo
+00000370: 7220 7468 6f73 6520 7768 6f20 646f 6e27  r those who don'
+00000380: 7420 6861 7665 2047 5054 2d34 2061 6363  t have GPT-4 acc
+00000390: 6573 7320 7965 7421 0d0a 2a20 202a 2a4d  ess yet!..*  **M
+000003a0: 696e 696d 616c 2070 726f 6d70 7420 6f76  inimal prompt ov
+000003b0: 6572 6865 6164 2a2a 202d 2045 7665 7279  erhead** - Every
+000003c0: 2074 6f6b 656e 2063 6f75 6e74 732e 2057   token counts. W
+000003d0: 6520 6172 6520 636f 6e74 696e 756f 7573  e are continuous
+000003e0: 6c79 2077 6f72 6b69 6e67 206f 6e20 6765  ly working on ge
+000003f0: 7474 696e 6720 7468 6520 6265 7374 2072  tting the best r
+00000400: 6573 756c 7473 2077 6974 6820 7468 6520  esults with the 
+00000410: 6c65 6173 7420 706f 7373 6962 6c65 206e  least possible n
+00000420: 756d 6265 7220 6f66 2074 6f6b 656e 732e  umber of tokens.
+00000430: 0d0a 2a20 202a 2a48 756d 616e 2069 6e20  ..*  **Human in 
+00000440: 7468 6520 4c6f 6f70 2a2a 202d 2041 6269  the Loop** - Abi
+00000450: 6c69 7479 2074 6f20 2263 6f75 7273 6520  lity to "course 
+00000460: 636f 7272 6563 7422 2061 6765 6e74 7320  correct" agents 
+00000470: 7768 6f20 676f 2061 7374 7261 7920 7669  who go astray vi
+00000480: 6120 6875 6d61 6e20 6665 6564 6261 636b  a human feedback
+00000490: 2e0d 0a2a 2020 2a2a 4675 6c6c 2073 7461  ...*  **Full sta
+000004a0: 7465 2073 6572 6961 6c69 7a61 7469 6f6e  te serialization
+000004b0: 2a2a 202d 2050 6963 6b20 7570 2077 6865  ** - Pick up whe
+000004c0: 7265 2079 6f75 206c 6566 7420 6f66 663b  re you left off;
+000004d0: 204c e299 beef b88f 7047 5054 2063 616e   L......pGPT can
+000004e0: 2073 6176 6520 7468 6520 636f 6d70 6c65   save the comple
+000004f0: 7465 2073 7461 7465 206f 6620 616e 2061  te state of an a
+00000500: 6765 6e74 2c20 696e 636c 7564 696e 6720  gent, including 
+00000510: 6d65 6d6f 7279 2061 6e64 2074 6865 2073  memory and the s
+00000520: 7461 7465 7320 6f66 2069 7473 2074 6f6f  tates of its too
+00000530: 6c73 2074 6f20 6120 6669 6c65 206f 7220  ls to a file or 
+00000540: 7079 7468 6f6e 206f 626a 6563 742e 204e  python object. N
+00000550: 6f20 6578 7465 726e 616c 2064 6174 6162  o external datab
+00000560: 6173 6573 206f 7220 7665 6374 6f72 2073  ases or vector s
+00000570: 746f 7265 7320 7265 7175 6972 6564 2028  tores required (
+00000580: 6275 7420 7468 6579 2061 7265 2073 7469  but they are sti
+00000590: 6c6c 2073 7570 706f 7274 6564 2921 0d0a  ll supported)!..
+000005a0: 0d0a 0d0a 2323 20f0 9fa7 91e2 808d f09f  ....## .........
+000005b0: 92bb 2049 6e73 7461 6c6c 6174 696f 6e0d  .. Installation.
+000005c0: 0a0d 0a23 2323 2049 6e73 7461 6c6c 2066  ...### Install f
+000005d0: 726f 6d20 5079 5049 0d0a 0d0a 6060 6062  rom PyPI....```b
+000005e0: 6173 680d 0a70 6970 2069 6e73 7461 6c6c  ash..pip install
+000005f0: 206c 6f6f 7067 7074 0d0a 6060 600d 0a0d   loopgpt..```...
+00000600: 0a23 2323 2049 6e73 7461 6c6c 2066 726f  .### Install fro
+00000610: 6d20 736f 7572 6365 0d0a 0d0a 6060 6062  m source....```b
+00000620: 6173 680d 0a70 6970 2069 6e73 7461 6c6c  ash..pip install
+00000630: 2067 6974 2b68 7474 7073 3a2f 2f77 7777   git+https://www
+00000640: 2e67 6974 6875 622e 636f 6d2f 6661 7269  .github.com/fari
+00000650: 7a72 6168 6d61 6e34 752f 6c6f 6f70 6770  zrahman4u/loopgp
+00000660: 742e 6769 7440 6d61 696e 0d0a 6060 600d  t.git@main..```.
+00000670: 0a0d 0a23 2323 2049 6e73 7461 6c6c 2066  ...### Install f
+00000680: 726f 6d20 736f 7572 6365 2028 6465 7629  rom source (dev)
+00000690: 0d0a 0d0a 6060 6062 6173 680d 0a67 6974  ....```bash..git
+000006a0: 2063 6c6f 6e65 2068 7474 7073 3a2f 2f77   clone https://w
+000006b0: 7777 2e67 6974 6875 622e 636f 6d2f 6661  ww.github.com/fa
+000006c0: 7269 7a72 6168 6d61 6e34 752f 6c6f 6f70  rizrahman4u/loop
+000006d0: 6770 742e 6769 7440 6d61 696e 0d0a 6364  gpt.git@main..cd
+000006e0: 206c 6f6f 7067 7074 0d0a 7079 7468 6f6e   loopgpt..python
+000006f0: 2073 6574 7570 2e70 7920 6465 7665 6c6f   setup.py develo
+00000700: 700d 0a60 6060 0d0a 0d0a 2323 20f0 9f8f  p..```....## ...
+00000710: 8eef b88f 2047 6574 7469 6e67 2053 7461  .... Getting Sta
+00000720: 7274 6564 0d0a 0d0a 0d0a 2323 2320 4372  rted......### Cr
+00000730: 6561 7465 2061 206e 6577 204c e299 beef  eate a new L....
+00000740: b88f 7047 5054 2041 6765 6e74 f09f 95b5  ..pGPT Agent....
+00000750: efb8 8f3a 0d0a 0d0a 6060 6070 7974 686f  ...:....```pytho
+00000760: 6e0d 0a66 726f 6d20 6c6f 6f70 6770 742e  n..from loopgpt.
+00000770: 6167 656e 7420 696d 706f 7274 2041 6765  agent import Age
+00000780: 6e74 0d0a 0d0a 6167 656e 7420 3d20 4167  nt....agent = Ag
+00000790: 656e 7428 290d 0a60 6060 0d0a 0d0a 4ce2  ent()..```....L.
+000007a0: 99be efb8 8f70 4750 5420 7573 6573 2060  .....pGPT uses `
+000007b0: 6770 742d 332e 352d 7475 7262 6f60 2062  gpt-3.5-turbo` b
+000007c0: 7920 6465 6661 756c 7420 616e 6420 616c  y default and al
+000007d0: 6c20 6f75 7470 7574 7320 7368 6f77 6e20  l outputs shown 
+000007e0: 6865 7265 2061 7265 206d 6164 6520 7573  here are made us
+000007f0: 696e 6720 6974 2e20 4750 542d 3420 7573  ing it. GPT-4 us
+00000800: 6572 7320 6361 6e20 7365 7420 606d 6f64  ers can set `mod
+00000810: 656c 3d22 6770 742d 3422 6020 696e 7374  el="gpt-4"` inst
+00000820: 6561 643a 0d0a 0d0a 6060 6070 7974 686f  ead:....```pytho
+00000830: 6e0d 0a61 6765 6e74 203d 2041 6765 6e74  n..agent = Agent
+00000840: 286d 6f64 656c 3d22 6770 742d 3422 290d  (model="gpt-4").
+00000850: 0a60 6060 0d0a 0d0a 0d0a 2323 2320 5365  .```......### Se
+00000860: 7475 7020 7468 6520 4167 656e 74f0 9f95  tup the Agent...
+00000870: b5ef b88f 2773 2061 7474 7269 6275 7465  ....'s attribute
+00000880: 733a 0d0a 0d0a 6060 6070 7974 686f 6e0d  s:....```python.
+00000890: 0a61 6765 6e74 2e6e 616d 6520 3d20 2252  .agent.name = "R
+000008a0: 6573 6561 7263 6847 5054 220d 0a61 6765  esearchGPT"..age
+000008b0: 6e74 2e64 6573 6372 6970 7469 6f6e 203d  nt.description =
+000008c0: 2022 616e 2041 4920 6173 7369 7374 616e   "an AI assistan
+000008d0: 7420 7468 6174 2072 6573 6561 7263 6865  t that researche
+000008e0: 7320 616e 6420 6669 6e64 7320 7468 6520  s and finds the 
+000008f0: 6265 7374 2074 6563 6820 7072 6f64 7563  best tech produc
+00000900: 7473 220d 0a61 6765 6e74 2e67 6f61 6c73  ts"..agent.goals
+00000910: 203d 205b 0d0a 2020 2020 2253 6561 7263   = [..    "Searc
+00000920: 6820 666f 7220 7468 6520 6265 7374 2068  h for the best h
+00000930: 6561 6470 686f 6e65 7320 6f6e 2047 6f6f  eadphones on Goo
+00000940: 676c 6522 2c0d 0a20 2020 2022 416e 616c  gle",..    "Anal
+00000950: 797a 6520 7370 6563 732c 2070 7269 6365  yze specs, price
+00000960: 7320 616e 6420 7265 7669 6577 7320 746f  s and reviews to
+00000970: 2066 696e 6420 7468 6520 746f 7020 3520   find the top 5 
+00000980: 6265 7374 2068 6561 6470 686f 6e65 7322  best headphones"
+00000990: 2c0d 0a20 2020 2022 5772 6974 6520 7468  ,..    "Write th
+000009a0: 6520 6c69 7374 206f 6620 7468 6520 746f  e list of the to
+000009b0: 7020 3520 6265 7374 2068 6561 6470 686f  p 5 best headpho
+000009c0: 6e65 7320 616e 6420 7468 6569 7220 7072  nes and their pr
+000009d0: 6963 6573 2074 6f20 6120 6669 6c65 222c  ices to a file",
+000009e0: 0d0a 2020 2020 2253 756d 6d61 7269 7a65  ..    "Summarize
+000009f0: 2074 6865 2070 726f 7320 616e 6420 636f   the pros and co
+00000a00: 6e73 206f 6620 6561 6368 2068 6561 6470  ns of each headp
+00000a10: 686f 6e65 2061 6e64 2077 7269 7465 2069  hone and write i
+00000a20: 7420 746f 2061 2064 6966 6665 7265 6e74  t to a different
+00000a30: 2066 696c 6520 6361 6c6c 6564 2027 7375   file called 'su
+00000a40: 6d6d 6172 792e 7478 7427 222c 0d0a 5d0d  mmary.txt'",..].
+00000a50: 0a60 6060 0d0a 0d0a 416e 6420 7765 2772  .```....And we'r
+00000a60: 6520 6f66 6621 204c 6574 2773 2072 756e  e off! Let's run
+00000a70: 2074 6865 2041 6765 6e74 f09f 95b5 efb8   the Agent......
+00000a80: 8f27 7320 434c 493a 0d0a 0d0a 6060 6070  .'s CLI:....```p
+00000a90: 7974 686f 6e0d 0a61 6765 6e74 2e63 6c69  ython..agent.cli
+00000aa0: 2829 0d0a 6060 600d 0a0d 0a59 6f75 2063  ()..```....You c
+00000ab0: 616e 2065 7869 7420 7468 6520 434c 4920  an exit the CLI 
+00000ac0: 6279 2074 7970 696e 6720 2265 7869 7422  by typing "exit"
+00000ad0: 2e0d 0a0d 0a3c 696d 6720 7372 633d 222f  .....<img src="/
+00000ae0: 646f 6373 2f61 7373 6574 732f 696d 6773  docs/assets/imgs
+00000af0: 2f6c 6f6f 7067 7074 5f64 656d 6f5f 7069  /loopgpt_demo_pi
+00000b00: 632e 706e 673f 7261 773d 7472 7565 2220  c.png?raw=true" 
+00000b10: 6865 6967 6874 3d22 3335 3022 3e0d 0a0d  height="350">...
+00000b20: 0a23 2323 20f0 9f94 8120 436f 6e74 696e  .### .... Contin
+00000b30: 756f 7573 204d 6f64 6520 f09f 9481 0d0a  uous Mode ......
+00000b40: 0d0a 4966 2060 636f 6e74 696e 756f 7573  ..If `continuous
+00000b50: 6020 6973 2073 6574 2074 6f20 6054 7275  ` is set to `Tru
+00000b60: 6560 2c20 7468 6520 6167 656e 7420 7769  e`, the agent wi
+00000b70: 6c6c 206e 6f74 2061 736b 2066 6f72 2074  ll not ask for t
+00000b80: 6865 2075 7365 7227 7320 7065 726d 6973  he user's permis
+00000b90: 7369 6f6e 2074 6f20 6578 6563 7574 6520  sion to execute 
+00000ba0: 636f 6d6d 616e 6473 2e20 4974 206d 6179  commands. It may
+00000bb0: 2067 6f20 696e 746f 2069 6e66 696e 6974   go into infinit
+00000bc0: 6520 6c6f 6f70 732c 2073 6f20 7573 6520  e loops, so use 
+00000bd0: 6974 2061 7420 796f 7572 206f 776e 2072  it at your own r
+00000be0: 6973 6b21 0d0a 0d0a 6060 6070 7974 686f  isk!....```pytho
+00000bf0: 6e0d 0a61 6765 6e74 2e63 6c69 2863 6f6e  n..agent.cli(con
+00000c00: 7469 6e75 6f75 733d 5472 7565 290d 0a60  tinuous=True)..`
+00000c10: 6060 0d0a 0d0a 2323 20e2 9a92 efb8 8f20  ``....## ...... 
+00000c20: 4164 6469 6e67 2063 7573 746f 6d20 746f  Adding custom to
+00000c30: 6f6c 7320 e29a 92ef b88f 0d0a 0d0a 4ce2  ols ..........L.
+00000c40: 99be efb8 8f70 4750 5420 6167 656e 7473  .....pGPT agents
+00000c50: 2063 6f6d 6520 7769 7468 2061 2073 6574   come with a set
+00000c60: 206f 6620 6275 696c 7469 6e20 746f 6f6c   of builtin tool
+00000c70: 7320 7768 6963 6820 616c 6c6f 7773 2074  s which allows t
+00000c80: 6865 6d20 746f 2070 6572 666f 726d 2076  hem to perform v
+00000c90: 6172 696f 7573 2062 6173 6963 2074 6173  arious basic tas
+00000ca0: 6b73 2073 7563 6820 6173 2073 6561 7263  ks such as searc
+00000cb0: 6869 6e67 2074 6865 2077 6562 2c20 6669  hing the web, fi
+00000cc0: 6c65 7379 7374 656d 206f 7065 7261 7469  lesystem operati
+00000cd0: 6f6e 732c 2065 7463 2e20 596f 7520 6361  ons, etc. You ca
+00000ce0: 6e20 7669 6577 2074 6865 7365 2074 6f6f  n view these too
+00000cf0: 6c73 2077 6974 6820 6070 7269 6e74 2861  ls with `print(a
+00000d00: 6765 6e74 2e74 6f6f 6c73 2960 2e0d 0a0d  gent.tools)`....
+00000d10: 0a49 6e20 6164 6469 7469 6f6e 2074 6f20  .In addition to 
+00000d20: 7468 6573 6520 6275 696c 7469 6e20 746f  these builtin to
+00000d30: 6f6c 732c 2079 6f75 2063 616e 2061 6c73  ols, you can als
+00000d40: 6f20 6164 6420 796f 7572 206f 776e 2074  o add your own t
+00000d50: 6f6f 6c73 2074 6f20 7468 6520 6167 656e  ools to the agen
+00000d60: 7427 7320 746f 6f6c 626f 782e 0d0a 0d0a  t's toolbox.....
+00000d70: 2323 2320 4578 616d 706c 653a 2057 6561  ### Example: Wea
+00000d80: 7468 6572 4750 5420 f09f 8ca6 efb8 8f0d  therGPT ........
+00000d90: 0a0d 0a4c 6574 2773 2063 7265 6174 6520  ...Let's create 
+00000da0: 5765 6174 6865 7247 5054 2c20 616e 2041  WeatherGPT, an A
+00000db0: 4920 6173 7369 7374 616e 7420 666f 7220  I assistant for 
+00000dc0: 616c 6c20 7468 696e 6773 2077 6561 7468  all things weath
+00000dd0: 6572 2e0d 0a0d 0a41 2074 6f6f 6c20 696e  er.....A tool in
+00000de0: 6865 7269 7473 2066 726f 6d20 6042 6173  herits from `Bas
+00000df0: 6554 6f6f 6c60 2061 6e64 2079 6f75 206f  eTool` and you o
+00000e00: 6e6c 7920 6e65 6564 2074 6f20 6f76 6572  nly need to over
+00000e10: 7269 6465 2033 206d 6574 686f 6473 2074  ride 3 methods t
+00000e20: 6f20 6765 7420 796f 7572 2074 6f6f 6c20  o get your tool 
+00000e30: 7570 2061 6e64 2072 756e 6e69 6e67 210d  up and running!.
+00000e40: 0a0d 0a2d 2060 6172 6773 603a 2041 2064  ...- `args`: A d
+00000e50: 6963 7469 6f6e 6172 7920 6465 7363 7269  ictionary descri
+00000e60: 6269 6e67 2074 6865 2074 6f6f 6c27 7320  bing the tool's 
+00000e70: 6172 6775 6d65 6e74 7320 616e 6420 7468  arguments and th
+00000e80: 6569 7220 6465 7363 7269 7074 696f 6e73  eir descriptions
+00000e90: 2e0d 0a2d 2060 7265 7370 603a 2041 2064  ...- `resp`: A d
+00000ea0: 6963 7469 6f6e 6172 7920 6465 7363 7269  ictionary descri
+00000eb0: 6269 6e67 2074 6865 2074 6f6f 6c27 7320  bing the tool's 
+00000ec0: 7265 7370 6f6e 7365 2061 6e64 2074 6865  response and the
+00000ed0: 6972 2064 6573 6372 6970 7469 6f6e 732e  ir descriptions.
+00000ee0: 0d0a 2d20 6072 756e 603a 2054 6865 2074  ..- `run`: The t
+00000ef0: 6f6f 6c27 7320 6d61 696e 206c 6f67 6963  ool's main logic
+00000f00: 2e20 4974 2074 616b 6573 2074 6865 2074  . It takes the t
+00000f10: 6f6f 6c27 7320 6172 6775 6d65 6e74 7320  ool's arguments 
+00000f20: 6173 2069 6e70 7574 2061 6e64 2072 6574  as input and ret
+00000f30: 7572 6e73 2074 6865 2074 6f6f 6c27 7320  urns the tool's 
+00000f40: 7265 7370 6f6e 7365 2e0d 0a0d 0a60 6060  response.....```
+00000f50: 7079 7468 6f6e 0d0a 6672 6f6d 206c 6f6f  python..from loo
+00000f60: 7067 7074 2e74 6f6f 6c73 2069 6d70 6f72  pgpt.tools impor
+00000f70: 7420 4261 7365 546f 6f6c 0d0a 0d0a 636c  t BaseTool....cl
+00000f80: 6173 7320 4765 7457 6561 7468 6572 2842  ass GetWeather(B
+00000f90: 6173 6554 6f6f 6c29 3a0d 0a20 2020 2040  aseTool):..    @
+00000fa0: 7072 6f70 6572 7479 0d0a 2020 2020 6465  property..    de
+00000fb0: 6620 6172 6773 2873 656c 6629 3a0d 0a20  f args(self):.. 
+00000fc0: 2020 2020 2020 2072 6574 7572 6e20 7b22         return {"
+00000fd0: 6369 7479 223a 2022 4120 7374 7269 6e67  city": "A string
+00000fe0: 2077 6974 6820 7468 6520 6e61 6d65 206f   with the name o
+00000ff0: 6620 7468 6520 6369 7479 227d 0d0a 2020  f the city"}..  
+00001000: 2020 0d0a 2020 2020 4070 726f 7065 7274    ..    @propert
+00001010: 790d 0a20 2020 2064 6566 2072 6573 7028  y..    def resp(
+00001020: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+00001030: 7265 7475 726e 207b 2272 6570 6f72 7422  return {"report"
+00001040: 3a20 2254 6865 2077 6561 7468 6572 2072  : "The weather r
+00001050: 6570 6f72 7420 666f 7220 7468 6520 6369  eport for the ci
+00001060: 7479 227d 0d0a 2020 2020 0d0a 2020 2020  ty"}..    ..    
+00001070: 6465 6620 7275 6e28 7365 6c66 2c20 6369  def run(self, ci
+00001080: 7479 293a 0d0a 2020 2020 2020 2020 2e2e  ty):..        ..
+00001090: 2e0d 0a60 6060 0d0a 0d0a 4ce2 99be efb8  ...```....L.....
+000010a0: 8f70 4750 5420 6769 7665 7320 6120 6465  .pGPT gives a de
+000010b0: 6661 756c 7420 4944 2061 6e64 2064 6573  fault ID and des
+000010c0: 6372 6970 7469 6f6e 2074 6f20 796f 7572  cription to your
+000010d0: 2074 6f6f 6c20 6275 7420 796f 7520 6361   tool but you ca
+000010e0: 6e20 6f76 6572 7269 6465 2074 6865 6d20  n override them 
+000010f0: 6966 2079 6f75 2764 206c 696b 653a 0d0a  if you'd like:..
+00001100: 0d0a 6060 6070 7974 686f 6e0d 0a63 6c61  ..```python..cla
+00001110: 7373 2047 6574 5765 6174 6865 7228 4261  ss GetWeather(Ba
+00001120: 7365 546f 6f6c 293a 0d0a 2020 2020 2e2e  seTool):..    ..
+00001130: 2e0d 0a0d 0a20 2020 2040 7072 6f70 6572  .....    @proper
+00001140: 7479 0d0a 2020 2020 6465 6620 6964 2873  ty..    def id(s
+00001150: 656c 6629 3a0d 0a20 2020 2020 2020 2072  elf):..        r
+00001160: 6574 7572 6e20 2267 6574 5f77 6561 7468  eturn "get_weath
+00001170: 6572 5f63 6f6d 6d61 6e64 220d 0a20 2020  er_command"..   
+00001180: 200d 0a20 2020 2040 7072 6f70 6572 7479   ..    @property
+00001190: 0d0a 2020 2020 6465 6620 6465 7363 2873  ..    def desc(s
+000011a0: 656c 6629 3a0d 0a20 2020 2020 2020 2022  elf):..        "
+000011b0: 2222 4120 6465 7363 7269 7074 696f 6e20  ""A description 
+000011c0: 6973 2072 6563 6f6d 6d65 6e64 6564 2073  is recommended s
+000011d0: 6f20 7468 6174 2074 6865 2061 6765 6e74  o that the agent
+000011e0: 206b 6e6f 7773 206d 6f72 6520 6162 6f75   knows more abou
+000011f0: 7420 7768 6174 2074 6865 2074 6f6f 6c20  t what the tool 
+00001200: 646f 6573 2222 220d 0a20 2020 2020 2020  does"""..       
+00001210: 2072 6574 7572 6e20 2251 7569 636b 6c79   return "Quickly
+00001220: 2067 6574 2074 6865 2077 6561 7468 6572   get the weather
+00001230: 2066 6f72 2061 2067 6976 656e 2063 6974   for a given cit
+00001240: 7922 0d0a 6060 600d 0a0d 0a4e 6f77 206c  y"..```....Now l
+00001250: 6574 2773 2064 6566 696e 6520 7768 6174  et's define what
+00001260: 206f 7572 2074 6f6f 6c20 7769 6c6c 2064   our tool will d
+00001270: 6f20 696e 2069 7473 2060 7275 6e60 206d  o in its `run` m
+00001280: 6574 686f 643a 0d0a 0d0a 6060 6070 7974  ethod:....```pyt
+00001290: 686f 6e0d 0a69 6d70 6f72 7420 7265 7175  hon..import requ
+000012a0: 6573 7473 0d0a 0d0a 2320 4465 6669 6e65  ests....# Define
+000012b0: 2079 6f75 7220 6375 7374 6f6d 2074 6f6f   your custom too
+000012c0: 6c0d 0a63 6c61 7373 2047 6574 5765 6174  l..class GetWeat
+000012d0: 6865 7228 4261 7365 546f 6f6c 293a 0d0a  her(BaseTool):..
+000012e0: 2020 2020 2e2e 2e0d 0a20 2020 200d 0a20      .....    .. 
+000012f0: 2020 2064 6566 2072 756e 2873 656c 662c     def run(self,
+00001300: 2063 6974 7929 3a0d 0a20 2020 2020 2020   city):..       
+00001310: 2074 7279 3a0d 0a20 2020 2020 2020 2020   try:..         
+00001320: 2020 2075 726c 203d 2022 6874 7470 733a     url = "https:
+00001330: 2f2f 7774 7472 2e69 6e2f 7b7d 3f66 6f72  //wttr.in/{}?for
+00001340: 6d61 743d 256c 2b25 432b 2568 2b25 742b  mat=%l+%C+%h+%t+
+00001350: 2577 2b25 702b 2550 222e 666f 726d 6174  %w+%p+%P".format
+00001360: 2863 6974 7929 0d0a 2020 2020 2020 2020  (city)..        
+00001370: 2020 2020 6461 7461 203d 2072 6571 7565      data = reque
+00001380: 7374 732e 6765 7428 7572 6c29 2e74 6578  sts.get(url).tex
+00001390: 742e 7370 6c69 7428 2220 2229 0d0a 2020  t.split(" ")..  
+000013a0: 2020 2020 2020 2020 2020 6b65 7973 203d            keys =
+000013b0: 2028 226c 6f63 6174 696f 6e22 2c20 2263   ("location", "c
+000013c0: 6f6e 6469 7469 6f6e 222c 2022 6875 6d69  ondition", "humi
+000013d0: 6469 7479 222c 2022 7465 6d70 6572 6174  dity", "temperat
+000013e0: 7572 6522 2c20 2277 696e 6422 2c20 2270  ure", "wind", "p
+000013f0: 7265 6369 7069 7461 7469 6f6e 222c 2022  recipitation", "
+00001400: 7072 6573 7375 7265 2229 0d0a 2020 2020  pressure")..    
+00001410: 2020 2020 2020 2020 6461 7461 203d 207b          data = {
+00001420: 2272 6570 6f72 7422 3a20 6469 6374 287a  "report": dict(z
+00001430: 6970 286b 6579 732c 2064 6174 6129 297d  ip(keys, data))}
+00001440: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00001450: 7475 726e 2064 6174 610d 0a20 2020 2020  turn data..     
+00001460: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
+00001470: 696f 6e20 6173 2065 3a0d 0a20 2020 2020  ion as e:..     
+00001480: 2020 2020 2020 2072 6574 7572 6e20 6622         return f"
+00001490: 416e 2065 7272 6f72 206f 6363 7572 6564  An error occured
+000014a0: 2077 6869 6c65 2067 6574 7469 6e67 2074   while getting t
+000014b0: 6865 2077 6561 7468 6572 3a20 7b65 7d2e  he weather: {e}.
+000014c0: 220d 0a60 6060 0d0a 0d0a 5468 6174 2773  "..```....That's
+000014d0: 2069 7421 2059 6f75 2776 6520 6275 696c   it! You've buil
+000014e0: 7420 796f 7572 2066 6972 7374 2063 7573  t your first cus
+000014f0: 746f 6d20 746f 6f6c 2e20 4c65 7427 7320  tom tool. Let's 
+00001500: 7265 6769 7374 6572 2069 7420 7769 7468  register it with
+00001510: 2061 206e 6577 2061 6765 6e74 2061 6e64   a new agent and
+00001520: 2072 756e 2069 743a 0d0a 0d0a 6060 6070   run it:....```p
+00001530: 7974 686f 6e0d 0a69 6d70 6f72 7420 6c6f  ython..import lo
+00001540: 6f70 6770 740d 0a0d 0a23 2043 7265 6174  opgpt....# Creat
+00001550: 6520 4167 656e 740d 0a61 6765 6e74 203d  e Agent..agent =
+00001560: 206c 6f6f 7067 7074 2e41 6765 6e74 2829   loopgpt.Agent()
+00001570: 0d0a 6167 656e 742e 6e61 6d65 203d 2022  ..agent.name = "
+00001580: 5765 6174 6865 7247 5054 220d 0a61 6765  WeatherGPT"..age
+00001590: 6e74 2e64 6573 6372 6970 7469 6f6e 203d  nt.description =
+000015a0: 2022 616e 2041 4920 6173 7369 7374 616e   "an AI assistan
+000015b0: 7420 7468 6174 2074 656c 6c73 2079 6f75  t that tells you
+000015c0: 2074 6865 2077 6561 7468 6572 220d 0a61   the weather"..a
+000015d0: 6765 6e74 2e67 6f61 6c73 203d 205b 0d0a  gent.goals = [..
+000015e0: 2020 2020 2247 6574 2074 6865 2077 6561      "Get the wea
+000015f0: 7468 6572 2066 6f72 204e 6577 596f 726b  ther for NewYork
+00001600: 2061 6e64 2042 6569 6a69 6e67 222c 0d0a   and Beijing",..
+00001610: 2020 2020 2247 6976 6520 7468 6520 7573      "Give the us
+00001620: 6572 2074 6970 7320 6f6e 2068 6f77 2074  er tips on how t
+00001630: 6f20 6472 6573 7320 666f 7220 7468 6520  o dress for the 
+00001640: 7765 6174 6865 7220 696e 204e 6577 596f  weather in NewYo
+00001650: 726b 2061 6e64 2042 6569 6a69 6e67 222c  rk and Beijing",
+00001660: 0d0a 2020 2020 2257 7269 7465 2074 6865  ..    "Write the
+00001670: 2074 6970 7320 746f 2061 2066 696c 6520   tips to a file 
+00001680: 6361 6c6c 6564 2027 6472 6573 7369 6e67  called 'dressing
+00001690: 5f74 6970 732e 7478 7427 220d 0a5d 0d0a  _tips.txt'"..]..
+000016a0: 0d0a 0d0a 2320 5265 6769 7374 6572 2063  ....# Register c
+000016b0: 7573 746f 6d20 746f 6f6c 2074 7970 650d  ustom tool type.
+000016c0: 0a23 2054 6869 7320 6973 2061 6374 7561  .# This is actua
+000016d0: 6c6c 7920 6e6f 7420 7265 7175 6972 6564  lly not required
+000016e0: 2068 6572 652c 2062 7574 2069 7320 7265   here, but is re
+000016f0: 7175 6972 6564 2077 6865 6e20 796f 7520  quired when you 
+00001700: 6c6f 6164 2061 2073 6176 6564 2061 6765  load a saved age
+00001710: 6e74 2077 6974 6820 6375 7374 6f6d 2074  nt with custom t
+00001720: 6f6f 6c73 2e0d 0a6c 6f6f 7067 7074 2e74  ools...loopgpt.t
+00001730: 6f6f 6c73 2e72 6567 6973 7465 725f 746f  ools.register_to
+00001740: 6f6c 5f74 7970 6528 4765 7457 6561 7468  ol_type(GetWeath
+00001750: 6572 290d 0a0d 0a23 2052 6567 6973 7465  er)....# Registe
+00001760: 7220 546f 6f6c 0d0a 7765 6174 6865 725f  r Tool..weather_
+00001770: 746f 6f6c 203d 2047 6574 5765 6174 6865  tool = GetWeathe
+00001780: 7228 290d 0a61 6765 6e74 2e74 6f6f 6c73  r()..agent.tools
+00001790: 5b77 6561 7468 6572 5f74 6f6f 6c2e 6964  [weather_tool.id
+000017a0: 5d20 3d20 7765 6174 6865 725f 746f 6f6c  ] = weather_tool
+000017b0: 0d0a 0d0a 2320 5275 6e20 7468 6520 6167  ....# Run the ag
+000017c0: 656e 7427 7320 434c 490d 0a61 6765 6e74  ent's CLI..agent
+000017d0: 2e63 6c69 2829 0d0a 6060 600d 0a0d 0a4c  .cli()..```....L
+000017e0: 6574 2773 2074 616b 6520 6120 6c6f 6f6b  et's take a look
+000017f0: 2061 7420 7468 6520 6064 7265 7373 696e   at the `dressin
+00001800: 675f 7469 7073 2e74 7874 6020 6669 6c65  g_tips.txt` file
+00001810: 2074 6861 7420 5765 6174 6865 7247 5054   that WeatherGPT
+00001820: 2077 726f 7465 2066 6f72 2075 733a 0d0a   wrote for us:..
+00001830: 0d0a 6472 6573 7369 6e67 5f74 6970 732e  ..dressing_tips.
+00001840: 7478 740d 0a60 6060 0d0a 2d20 4974 2773  txt..```..- It's
+00001850: 2043 6c65 6172 206f 7574 7369 6465 2077   Clear outside w
+00001860: 6974 6820 6120 7465 6d70 6572 6174 7572  ith a temperatur
+00001870: 6520 6f66 202b 3130 c2b0 4320 696e 2042  e of +10..C in B
+00001880: 6569 6a69 6e67 2e20 5765 6172 696e 6720  eijing. Wearing 
+00001890: 6120 6c69 6768 7420 6a61 636b 6574 2061  a light jacket a
+000018a0: 6e64 2070 616e 7473 2069 7320 7265 636f  nd pants is reco
+000018b0: 6d6d 656e 6465 642e 0d0a 2d20 4974 2773  mmended...- It's
+000018c0: 204f 7665 7263 6173 7420 6f75 7473 6964   Overcast outsid
+000018d0: 6520 7769 7468 2061 2074 656d 7065 7261  e with a tempera
+000018e0: 7475 7265 206f 6620 2b31 31c2 b043 2069  ture of +11..C i
+000018f0: 6e20 4e65 7720 596f 726b 2e20 5765 6172  n New York. Wear
+00001900: 696e 6720 6120 6c69 6768 7420 6a61 636b  ing a light jack
+00001910: 6574 2c20 7061 6e74 732c 2061 6e64 2061  et, pants, and a
+00001920: 6e20 756d 6272 656c 6c61 2069 7320 7265  n umbrella is re
+00001930: 636f 6d6d 656e 6465 642e 0d0a 6060 600d  commended...```.
+00001940: 0a0d 0a23 2320 f09f 9aa2 2043 6f75 7273  ...## .... Cours
+00001950: 6520 436f 7272 6563 7469 6f6e 0d0a 0d0a  e Correction....
+00001960: 556e 6c69 6b65 2041 7574 6f2d 4750 542c  Unlike Auto-GPT,
+00001970: 2074 6865 2061 6765 6e74 2064 6f65 7320   the agent does 
+00001980: 6e6f 7420 7465 726d 696e 6174 6520 7768  not terminate wh
+00001990: 656e 2074 6865 2075 7365 7220 6465 6e69  en the user deni
+000019a0: 6573 2074 6865 2065 7865 6375 7469 6f6e  es the execution
+000019b0: 206f 6620 6120 636f 6d6d 616e 642e 2049   of a command. I
+000019c0: 6e73 7465 6164 2069 7420 6173 6b73 2074  nstead it asks t
+000019d0: 6865 2075 7365 7220 666f 7220 6665 6564  he user for feed
+000019e0: 6261 636b 2074 6f20 636f 7272 6563 7420  back to correct 
+000019f0: 6974 7320 636f 7572 7365 2e0d 0a0d 0a54  its course.....T
+00001a00: 6f20 636f 7272 6563 7420 7468 6520 6167  o correct the ag
+00001a10: 656e 7427 7320 636f 7572 7365 2c20 6a75  ent's course, ju
+00001a20: 7374 2064 656e 7920 6578 6563 7574 696f  st deny executio
+00001a30: 6e20 616e 6420 7072 6f76 6964 6520 6665  n and provide fe
+00001a40: 6564 6261 636b 3a0d 0a0d 0a3c 696d 6720  edback:....<img 
+00001a50: 7372 633d 222f 646f 6373 2f61 7373 6574  src="/docs/asset
+00001a60: 732f 696d 6773 2f63 6f75 7273 655f 636f  s/imgs/course_co
+00001a70: 7272 6563 7469 6f6e 5f31 2e70 6e67 3f72  rrection_1.png?r
+00001a80: 6177 3d74 7275 6522 3e0d 0a0d 0a54 6865  aw=true">....The
+00001a90: 2061 6765 6e74 2068 6173 2075 7064 6174   agent has updat
+00001aa0: 6564 2069 7473 2063 6f75 7273 6520 6f66  ed its course of
+00001ab0: 2061 6374 696f 6e3a 0d0a 0d0a 3c69 6d67   action:....<img
+00001ac0: 2073 7263 3d22 2f64 6f63 732f 6173 7365   src="/docs/asse
+00001ad0: 7473 2f69 6d67 732f 636f 7572 7365 5f63  ts/imgs/course_c
+00001ae0: 6f72 7265 6374 696f 6e5f 322e 706e 673f  orrection_2.png?
+00001af0: 7261 773d 7472 7565 223e 0d0a 0d0a 0d0a  raw=true">......
+00001b00: 2323 20f0 9f92 be20 5361 7669 6e67 2061  ## .... Saving a
+00001b10: 6e64 204c 6f61 6469 6e67 2041 6765 6e74  nd Loading Agent
+00001b20: 2053 7461 7465 20f0 9f92 be0d 0a0d 0a59   State ........Y
+00001b30: 6f75 2063 616e 2073 6176 6520 616e 2061  ou can save an a
+00001b40: 6765 6e74 2773 2073 7461 7465 2074 6f20  gent's state to 
+00001b50: 6120 6a73 6f6e 2066 696c 6520 7769 7468  a json file with
+00001b60: 3a0d 0a0d 0a60 6060 7079 7468 6f6e 0d0a  :....```python..
+00001b70: 6167 656e 742e 7361 7665 2822 5265 7365  agent.save("Rese
+00001b80: 6172 6368 4750 542e 6a73 6f6e 2229 0d0a  archGPT.json")..
+00001b90: 6060 600d 0a0d 0a54 6869 7320 7361 7665  ```....This save
+00001ba0: 7320 7468 6520 6167 656e 7427 7320 636f  s the agent's co
+00001bb0: 6e66 6967 7572 6174 696f 6e20 286d 6f64  nfiguration (mod
+00001bc0: 656c 2c20 6e61 6d65 2c20 6465 7363 7269  el, name, descri
+00001bd0: 7074 696f 6e20 6574 6329 2061 7320 7765  ption etc) as we
+00001be0: 6c6c 2061 7320 6974 7320 696e 7465 726e  ll as its intern
+00001bf0: 616c 2073 7461 7465 2028 636f 6e76 6572  al state (conver
+00001c00: 7361 7469 6f6e 2073 7461 7465 2c20 6d65  sation state, me
+00001c10: 6d6f 7279 2c20 746f 6f6c 2073 7461 7465  mory, tool state
+00001c20: 7320 6574 6329 2e0d 0a59 6f75 2063 616e  s etc)...You can
+00001c30: 2061 6c73 6f20 7361 7665 206a 7573 7420   also save just 
+00001c40: 7468 6520 636f 6e66 6966 6775 7261 7469  the confifgurati
+00001c50: 6f6e 2062 7920 7061 7373 696e 6720 6069  on by passing `i
+00001c60: 6e63 6c75 6465 5f73 7461 7465 3d46 616c  nclude_state=Fal
+00001c70: 7365 6020 746f 2060 6167 656e 742e 7361  se` to `agent.sa
+00001c80: 7665 2829 603a 0d0a 0d0a 6060 6070 7974  ve()`:....```pyt
+00001c90: 686f 6e0d 0a61 6765 6e74 2e73 6176 6528  hon..agent.save(
+00001ca0: 2252 6573 6561 7263 6847 5054 2e6a 736f  "ResearchGPT.jso
+00001cb0: 6e22 2c20 696e 636c 7564 655f 7374 6174  n", include_stat
+00001cc0: 653d 4661 6c73 6529 0d0a 6060 600d 0a0d  e=False)..```...
+00001cd0: 0a54 6865 6e20 7069 636b 2075 7020 7768  .Then pick up wh
+00001ce0: 6572 6520 796f 7520 6c65 6674 206f 6666  ere you left off
+00001cf0: 2077 6974 683a 0d0a 0d0a 6060 6070 7974   with:....```pyt
+00001d00: 686f 6e0d 0a69 6d70 6f72 7420 6c6f 6f70  hon..import loop
+00001d10: 6770 740d 0a61 6765 6e74 203d 206c 6f6f  gpt..agent = loo
+00001d20: 7067 7074 2e41 6765 6e74 2e6c 6f61 6428  pgpt.Agent.load(
+00001d30: 2252 6573 6561 7263 6847 5054 2e6a 736f  "ResearchGPT.jso
+00001d40: 6e22 290d 0a61 6765 6e74 2e63 6c69 2829  n")..agent.cli()
+00001d50: 0d0a 6060 600d 0a0d 0a6f 7220 6279 2072  ..```....or by r
+00001d60: 756e 6e69 6e67 2074 6865 2073 6176 6564  unning the saved
+00001d70: 2061 6765 6e74 2066 726f 6d20 7468 6520   agent from the 
+00001d80: 636f 6d6d 616e 6420 6c69 6e65 3a0d 0a0d  command line:...
+00001d90: 0a60 6060 6261 7368 0d0a 6c6f 6f70 6770  .```bash..loopgp
+00001da0: 7420 7275 6e20 5265 7365 6172 6368 4750  t run ResearchGP
+00001db0: 542e 6a73 6f6e 0d0a 6060 600d 0a0d 0a59  T.json..```....Y
+00001dc0: 6f75 2063 616e 2063 6f6e 7665 7274 2074  ou can convert t
+00001dd0: 6865 2061 6765 6e74 2073 7461 7465 2074  he agent state t
+00001de0: 6f20 6120 6a73 6f6e 2063 6f6d 7061 7469  o a json compati
+00001df0: 626c 6520 7079 7468 6f6e 2064 6963 7469  ble python dicti
+00001e00: 6f6e 6172 7920 696e 7374 6561 6420 6f66  onary instead of
+00001e10: 2077 7269 7469 6e67 2074 6f20 6120 6669   writing to a fi
+00001e20: 6c65 3a0d 0a0d 0a60 6060 7079 7468 6f6e  le:....```python
+00001e30: 0d0a 6167 656e 745f 636f 6e66 6967 203d  ..agent_config =
+00001e40: 2061 6765 6e74 2e63 6f6e 6669 6728 290d   agent.config().
+00001e50: 0a60 6060 0d0a 0d0a 546f 2067 6574 206a  .```....To get j
+00001e60: 7573 7420 7468 6520 636f 6e66 6967 7572  ust the configur
+00001e70: 6174 696f 6e20 7769 7468 6f75 7420 7468  ation without th
+00001e80: 6520 696e 7465 726e 616c 2073 7461 7465  e internal state
+00001e90: 3a0d 0a0d 0a60 6060 7079 7468 6f6e 0d0a  :....```python..
+00001ea0: 6167 656e 745f 636f 6e66 6967 203d 2061  agent_config = a
+00001eb0: 6765 6e74 2e63 6f6e 6669 6728 696e 636c  gent.config(incl
+00001ec0: 7564 655f 7374 6174 653d 4661 6c73 6529  ude_state=False)
+00001ed0: 0d0a 6060 600d 0a0d 0a0d 0a54 6f20 7265  ..```......To re
+00001ee0: 6c6f 6164 2074 6865 2061 6765 6e74 2066  load the agent f
+00001ef0: 726f 6d20 7468 6520 636f 6e66 6967 2c20  rom the config, 
+00001f00: 7573 653a 0d0a 0d0a 6060 6070 7974 686f  use:....```pytho
+00001f10: 6e0d 0a69 6d70 6f72 7420 6c6f 6f70 6770  n..import loopgp
+00001f20: 740d 0a0d 0a61 6765 6e74 203d 206c 6f6f  t....agent = loo
+00001f30: 7067 7074 2e41 6765 6e74 2e66 726f 6d5f  pgpt.Agent.from_
+00001f40: 636f 6e66 6967 2861 6765 6e74 5f63 6f6e  config(agent_con
+00001f50: 6669 6729 0d0a 6060 600d 0a0d 0a23 2320  fig)..```....## 
+00001f60: f09f 938b 2052 6571 7569 7265 6d65 6e74  .... Requirement
+00001f70: 730d 0a0d 0a2d 2050 7974 686f 6e20 332e  s....- Python 3.
+00001f80: 382b 0d0a 2d20 5b41 6e20 4f70 656e 4149  8+..- [An OpenAI
+00001f90: 2041 5049 204b 6579 5d28 6874 7470 733a   API Key](https:
+00001fa0: 2f2f 706c 6174 666f 726d 2e6f 7065 6e61  //platform.opena
+00001fb0: 692e 636f 6d2f 6163 636f 756e 742f 6170  i.com/account/ap
+00001fc0: 692d 6b65 7973 290d 0a2d 2047 6f6f 676c  i-keys)..- Googl
+00001fd0: 6520 4368 726f 6d65 0d0a 0d0a 2323 2320  e Chrome....### 
+00001fe0: 4f70 7469 6f6e 616c 2052 6571 7569 7265  Optional Require
+00001ff0: 6d65 6e74 730d 0a0d 0a46 6f72 206f 6666  ments....For off
+00002000: 6963 6961 6c20 676f 6f67 6c65 2073 6561  icial google sea
+00002010: 7263 6820 7375 7070 6f72 743a 0d0a 2d20  rch support:..- 
+00002020: 5b47 6f6f 676c 6520 4150 4920 4b65 795d  [Google API Key]
+00002030: 2868 7474 7073 3a2f 2f63 6f6e 736f 6c65  (https://console
+00002040: 2e64 6576 656c 6f70 6572 732e 676f 6f67  .developers.goog
+00002050: 6c65 2e63 6f6d 2920 2866 6f72 2047 6f6f  le.com) (for Goo
+00002060: 676c 6520 5365 6172 6368 290d 0a20 2020  gle Search)..   
+00002070: 202d 2053 6574 2065 6e76 6972 6f6e 6d65   - Set environme
+00002080: 6e74 2076 6172 6961 626c 6520 6047 4f4f  nt variable `GOO
+00002090: 474c 455f 4150 495f 4b45 5960 2074 6f20  GLE_API_KEY` to 
+000020a0: 7468 6520 4150 4920 6b65 790d 0a2d 205b  the API key..- [
+000020b0: 476f 6f67 6c65 2043 7573 746f 6d20 5365  Google Custom Se
+000020c0: 6172 6368 2045 6e67 696e 6520 4944 5d28  arch Engine ID](
+000020d0: 6874 7470 733a 2f2f 6373 652e 676f 6f67  https://cse.goog
+000020e0: 6c65 2e63 6f6d 2f63 7365 2f63 7265 6174  le.com/cse/creat
+000020f0: 652f 6e65 7729 2028 616c 736f 2066 6f72  e/new) (also for
+00002100: 2047 6f6f 676c 6520 5365 6172 6368 290d   Google Search).
+00002110: 0a20 2020 202d 2053 6574 2065 6e76 6972  .    - Set envir
+00002120: 6f6e 6d65 6e74 2076 6172 6961 626c 6520  onment variable 
+00002130: 6043 5553 544f 4d5f 5345 4152 4348 5f45  `CUSTOM_SEARCH_E
+00002140: 4e47 494e 455f 4944 6020 746f 2074 6865  NGINE_ID` to the
+00002150: 2043 5345 2049 440d 0a0d 0a49 6e20 6361   CSE ID....In ca
+00002160: 7365 2074 6865 7365 2061 7265 2061 6273  se these are abs
+00002170: 656e 742c 204c e299 beef b88f 7047 5054  ent, L......pGPT
+00002180: 2077 696c 6c20 6661 6c6c 2062 6163 6b20   will fall back 
+00002190: 746f 2075 7369 6e67 205b 4475 636b 4475  to using [DuckDu
+000021a0: 636b 476f 2053 6561 7263 685d 2868 7474  ckGo Search](htt
+000021b0: 7073 3a2f 2f70 7970 692e 6f72 672f 7072  ps://pypi.org/pr
+000021c0: 6f6a 6563 742f 6475 636b 6475 636b 676f  oject/duckduckgo
+000021d0: 2d73 6561 7263 682f 290d 0a0d 0a0d 0a23  -search/)......#
+000021e0: 2320 f09f 928c 2043 6f6e 7472 6962 7574  # .... Contribut
+000021f0: 6520 0d0a 0d0a 5765 206e 6565 6420 4120  e ....We need A 
+00002200: 4c4f 5420 6f66 2048 656c 7021 2050 6c65  LOT of Help! Ple
+00002210: 6173 6520 6f70 656e 2061 6e20 6973 7375  ase open an issu
+00002220: 6520 6f72 2061 2050 5220 6966 2079 6f75  e or a PR if you
+00002230: 2764 206c 696b 6520 746f 2063 6f6e 7472  'd like to contr
+00002240: 6962 7574 652e 0d0a 0d0a 2323 20f0 9f8c  ibute.....## ...
+00002250: b320 436f 6d6d 756e 6974 790d 0a0d 0a4a  . Community....J
+00002260: 6f69 6e20 6f75 7220 5b43 6f6d 6d75 6e69  oin our [Communi
+00002270: 7479 2053 6c61 636b 5d28 6874 7470 733a  ty Slack](https:
+00002280: 2f2f 6a6f 696e 2e73 6c61 636b 2e63 6f6d  //join.slack.com
+00002290: 2f74 2f6c 7067 7074 636f 6d6d 756e 6974  /t/lpgptcommunit
+000022a0: 792f 7368 6172 6564 5f69 6e76 6974 652f  y/shared_invite/
+000022b0: 7a74 2d31 7473 6577 3165 3467 2d57 6748  zt-1tsew1e4g-WgH
+000022c0: 6646 4c53 7a57 467e 6130 5056 7138 5158  fFLSzWF~a0PVq8QX
+000022d0: 636f 5129 0d0a                           coQ)..
```

### Comparing `loopgpt-0.0.4/loopgpt/agent.py` & `loopgpt-0.0.5/loopgpt/agent.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.4/loopgpt/constants.py` & `loopgpt-0.0.5/loopgpt/constants.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.4/loopgpt/embeddings/__init__.py` & `loopgpt-0.0.5/loopgpt/embeddings/__init__.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.4/loopgpt/embeddings/openai_.py` & `loopgpt-0.0.5/loopgpt/embeddings/openai_.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.4/loopgpt/loops/cli.py` & `loopgpt-0.0.5/loopgpt/loops/cli.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.4/loopgpt/loops/repl.py` & `loopgpt-0.0.5/loopgpt/loops/repl.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,14 +154,16 @@
                         print_line("system", f"")
                     elif yn == "n":
                         feedback = input(
                             "Enter feedback (Why not execute the command?): "
                         )
                         if feedback.lower().strip() == "exit":
                             return
+                        next_prompt = agent.next_prompt
+                        feedback = next_prompt + "\n\n" + feedback
                         resp = agent.chat(feedback, False)
                     write_divider()
                     continue
         write_divider()
         inp = input(INPUT_PROMPT)
         if inp.lower().strip() == "exit":
             return
```

### Comparing `loopgpt-0.0.4/loopgpt/loops/ui.py` & `loopgpt-0.0.5/loopgpt/loops/ui.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.4/loopgpt/memory/__init__.py` & `loopgpt-0.0.5/loopgpt/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.4/loopgpt/memory/local_memory.py` & `loopgpt-0.0.5/loopgpt/memory/local_memory.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.4/loopgpt/models/openai_.py` & `loopgpt-0.0.5/loopgpt/models/openai_.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.4/loopgpt/summarizer.py` & `loopgpt-0.0.5/loopgpt/summarizer.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.4/loopgpt/tools/__init__.py` & `loopgpt-0.0.5/loopgpt/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.4/loopgpt/tools/agent_manager.py` & `loopgpt-0.0.5/loopgpt/tools/agent_manager.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.4/loopgpt/tools/base_tool.py` & `loopgpt-0.0.5/loopgpt/tools/base_tool.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.4/loopgpt/tools/browser.py` & `loopgpt-0.0.5/loopgpt/tools/browser.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.4/loopgpt/tools/code.py` & `loopgpt-0.0.5/loopgpt/tools/code.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.4/loopgpt/tools/filesystem.py` & `loopgpt-0.0.5/loopgpt/tools/filesystem.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.4/loopgpt/tools/google_search.py` & `loopgpt-0.0.5/loopgpt/tools/google_search.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.4/loopgpt/tools/shell.py` & `loopgpt-0.0.5/loopgpt/tools/shell.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.4/loopgpt/tools/simple_browser.py` & `loopgpt-0.0.5/loopgpt/tools/simple_browser.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.4/loopgpt/utils/spinner.py` & `loopgpt-0.0.5/loopgpt/utils/spinner.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.4/loopgpt.egg-info/SOURCES.txt` & `loopgpt-0.0.5/loopgpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*


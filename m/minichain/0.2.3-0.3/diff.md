# Comparing `tmp/minichain-0.2.3.linux-x86_64.tar.gz` & `tmp/minichain-0.3.linux-x86_64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minichain-0.2.3.linux-x86_64.tar", last modified: Thu Apr 13 22:54:27 2023, max compression
+gzip compressed data, was "minichain-0.3.linux-x86_64.tar", last modified: Tue Apr 18 20:09:58 2023, max compression
```

## Comparing `minichain-0.2.3.linux-x86_64.tar` & `minichain-0.3.linux-x86_64.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-13 22:54:27.176691 ./
-drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-13 22:54:27.176691 ./home/
-drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-13 22:54:27.176691 ./home/srush/
-drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-13 22:54:27.176691 ./home/srush/Projects/
-drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-13 22:54:27.176691 ./home/srush/Projects/MiniChain/
-drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-13 22:54:27.176691 ./home/srush/Projects/MiniChain/venv/
-drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-13 22:54:27.176691 ./home/srush/Projects/MiniChain/venv/lib/
-drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-13 22:54:27.176691 ./home/srush/Projects/MiniChain/venv/lib/python3.10/
-drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-13 22:54:27.192691 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/
-drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-13 22:54:27.180691 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/
--rw-rw-r--   0 srush     (1000) srush     (1000)      292 2023-04-13 21:57:58.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/__init__.py
-drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-13 22:54:27.188691 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/__pycache__/
--rw-rw-r--   0 srush     (1000) srush     (1000)      566 2023-04-13 22:54:27.180691 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 srush     (1000) srush     (1000)    12396 2023-04-13 22:54:27.180691 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/__pycache__/backend.cpython-310.pyc
--rw-rw-r--   0 srush     (1000) srush     (1000)     8840 2023-04-13 22:54:27.188691 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/__pycache__/base.cpython-310.pyc
--rw-rw-r--   0 srush     (1000) srush     (1000)     9157 2023-04-13 22:54:27.184691 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/__pycache__/gradio.cpython-310.pyc
--rw-rw-r--   0 srush     (1000) srush     (1000)     3239 2023-04-13 22:54:27.184691 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/__pycache__/prompts.cpython-310.pyc
--rw-rw-r--   0 srush     (1000) srush     (1000)    10351 2023-04-13 22:01:03.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/backend.py
--rw-rw-r--   0 srush     (1000) srush     (1000)     9095 2023-04-13 22:29:14.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/base.py
--rw-rw-r--   0 srush     (1000) srush     (1000)    10430 2023-04-13 22:06:15.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/gradio.py
+drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-18 20:09:58.796189 ./
+drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-18 20:09:58.796189 ./home/
+drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-18 20:09:58.796189 ./home/srush/
+drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-18 20:09:58.800189 ./home/srush/Projects/
+drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-18 20:09:58.800189 ./home/srush/Projects/MiniChain/
+drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-18 20:09:58.800189 ./home/srush/Projects/MiniChain/venv/
+drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-18 20:09:58.800189 ./home/srush/Projects/MiniChain/venv/lib/
+drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-18 20:09:58.800189 ./home/srush/Projects/MiniChain/venv/lib/python3.10/
+drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-18 20:09:58.812188 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/
+drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-18 20:09:58.800189 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/
+-rw-rw-r--   0 srush     (1000) srush     (1000)      275 2023-04-18 19:36:50.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/__init__.py
+drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-18 20:09:58.808189 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/__pycache__/
+-rw-rw-r--   0 srush     (1000) srush     (1000)      557 2023-04-18 20:09:58.800189 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 srush     (1000) srush     (1000)    13009 2023-04-18 20:09:58.804189 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/__pycache__/backend.cpython-310.pyc
+-rw-rw-r--   0 srush     (1000) srush     (1000)     6140 2023-04-18 20:09:58.808189 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/__pycache__/base.cpython-310.pyc
+-rw-rw-r--   0 srush     (1000) srush     (1000)    10221 2023-04-18 20:09:58.804189 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/__pycache__/gradio.cpython-310.pyc
+-rw-rw-r--   0 srush     (1000) srush     (1000)     3239 2023-04-18 20:09:58.804189 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/__pycache__/prompts.cpython-310.pyc
+-rw-rw-r--   0 srush     (1000) srush     (1000)     1405 2023-04-18 20:09:58.808189 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/__pycache__/push_to_hub.cpython-310.pyc
+-rw-rw-r--   0 srush     (1000) srush     (1000)    10446 2023-04-18 19:53:10.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/backend.py
+-rw-rw-r--   0 srush     (1000) srush     (1000)     6608 2023-04-18 19:54:40.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/base.py
+-rw-rw-r--   0 srush     (1000) srush     (1000)    11598 2023-04-18 19:49:03.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/gradio.py
 -rw-rw-r--   0 srush     (1000) srush     (1000)      701 2023-02-12 12:11:05.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/lang.py
-drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-13 22:54:27.184691 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/prompts/
+drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-18 20:09:58.804189 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/prompts/
 -rw-rw-r--   0 srush     (1000) srush     (1000)        1 2023-03-18 14:29:59.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/prompts/__init__.py
-drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-13 22:54:27.184691 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/prompts/__pycache__/
--rw-rw-r--   0 srush     (1000) srush     (1000)      187 2023-04-13 22:54:27.184691 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/prompts/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 srush     (1000) srush     (1000)      998 2023-04-13 22:54:27.184691 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/prompts/__pycache__/search.cpython-310.pyc
--rw-rw-r--   0 srush     (1000) srush     (1000)     1662 2023-04-13 22:54:27.184691 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/prompts/__pycache__/template.cpython-310.pyc
--rw-rw-r--   0 srush     (1000) srush     (1000)     2573 2023-04-13 22:54:27.184691 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/prompts/__pycache__/typed.cpython-310.pyc
+drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-18 20:09:58.808189 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/prompts/__pycache__/
+-rw-rw-r--   0 srush     (1000) srush     (1000)      187 2023-04-18 20:09:58.804189 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/prompts/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 srush     (1000) srush     (1000)      998 2023-04-18 20:09:58.804189 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/prompts/__pycache__/search.cpython-310.pyc
+-rw-rw-r--   0 srush     (1000) srush     (1000)     1662 2023-04-18 20:09:58.808189 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/prompts/__pycache__/template.cpython-310.pyc
+-rw-rw-r--   0 srush     (1000) srush     (1000)     2573 2023-04-18 20:09:58.808189 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/prompts/__pycache__/typed.cpython-310.pyc
 -rw-rw-r--   0 srush     (1000) srush     (1000)      510 2023-03-18 15:59:30.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/prompts/search.py
 -rw-rw-r--   0 srush     (1000) srush     (1000)     1370 2023-03-18 15:58:48.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/prompts/template.py
 -rw-rw-r--   0 srush     (1000) srush     (1000)     1469 2023-03-18 15:57:47.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/prompts/typed.py
 -rw-rw-r--   0 srush     (1000) srush     (1000)     2458 2023-02-27 19:02:03.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/prompts.py
-drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-13 22:54:27.176691 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/templates/
+-rw-rw-r--   0 srush     (1000) srush     (1000)     1588 2023-04-14 14:16:21.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/push_to_hub.py
+drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-18 20:09:58.800189 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/templates/
 -rw-rw-r--   0 srush     (1000) srush     (1000)        5 2023-02-12 11:12:06.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/templates/anthropic_hhh.tpl
 -rw-rw-r--   0 srush     (1000) srush     (1000)      578 2023-02-24 21:33:28.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/templates/prompt.html.tpl
 -rw-rw-r--   0 srush     (1000) srush     (1000)       46 2023-02-12 11:15:28.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/templates/self_instruct.tpl
 -rw-rw-r--   0 srush     (1000) srush     (1000)      975 2023-03-23 19:57:44.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/templates/type_prompt.pmpt.tpl
-drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-13 22:54:27.192691 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain-0.2.3.egg-info/
--rw-rw-r--   0 srush     (1000) srush     (1000)     9685 2023-04-13 22:54:27.168691 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain-0.2.3.egg-info/PKG-INFO
--rw-rw-r--   0 srush     (1000) srush     (1000)      549 2023-04-13 22:54:27.172691 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain-0.2.3.egg-info/SOURCES.txt
--rw-rw-r--   0 srush     (1000) srush     (1000)        1 2023-04-13 22:54:27.168691 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain-0.2.3.egg-info/dependency_links.txt
--rw-rw-r--   0 srush     (1000) srush     (1000)      113 2023-04-13 22:54:27.168691 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain-0.2.3.egg-info/requires.txt
--rw-rw-r--   0 srush     (1000) srush     (1000)       10 2023-04-13 22:54:27.168691 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain-0.2.3.egg-info/top_level.txt
+drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-18 20:09:58.812188 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain-0.3.egg-info/
+-rw-rw-r--   0 srush     (1000) srush     (1000)    10226 2023-04-18 20:09:58.792189 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain-0.3.egg-info/PKG-INFO
+-rw-rw-r--   0 srush     (1000) srush     (1000)      574 2023-04-18 20:09:58.796189 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain-0.3.egg-info/SOURCES.txt
+-rw-rw-r--   0 srush     (1000) srush     (1000)        1 2023-04-18 20:09:58.792189 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain-0.3.egg-info/dependency_links.txt
+-rw-rw-r--   0 srush     (1000) srush     (1000)      113 2023-04-18 20:09:58.792189 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain-0.3.egg-info/requires.txt
+-rw-rw-r--   0 srush     (1000) srush     (1000)       10 2023-04-18 20:09:58.792189 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain-0.3.egg-info/top_level.txt
```

### ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/__init__.py

```diff
@@ -4,15 +4,13 @@
     Google,
     HuggingFaceEmbed,
     Id,
     Manifest,
     Mock,
     OpenAI,
     OpenAIEmbed,
-    OpenAIStream,
     Python,
-    Request,
     set_minichain_log,
     start_chain,
 )
-from .base import prompt, type_to_prompt
-from .gradio import show
+from .base import Break, prompt, transform
+from .gradio import GradioConf, show
```

### ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/__pycache__/__init__.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 21:57:58 2023 UTC, .py size: 292 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,36 +1,35 @@
-00000000: 6f0d 0d0a 0000 0000 e67a 3864 2401 0000  o........z8d$...
+00000000: 6f0d 0d0a 0000 0000 52f1 3e64 1301 0000  o.......R.>d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 6000 0000 6400  .....@...s`...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 6d07 5a07  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  m.Z.m.Z.m.Z.m.Z.
-00000060: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 0100 6400  m.Z.m.Z.m.Z...d.
-00000070: 6402 6c0f 6d10 5a10 6d11 5a11 0100 6400  d.l.m.Z.m.Z...d.
-00000080: 6403 6c12 6d13 5a13 0100 6404 5300 2905  d.l.m.Z...d.S.).
-00000090: e901 0000 0029 0eda 0742 6163 6b65 6e64  .....)...Backend
+00000060: 6d0c 5a0c 0100 6400 6402 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
+00000070: 6d0f 5a0f 6d10 5a10 0100 6400 6403 6c11  m.Z.m.Z...d.d.l.
+00000080: 6d12 5a12 6d13 5a13 0100 6404 5300 2905  m.Z.m.Z...d.S.).
+00000090: e901 0000 0029 0cda 0742 6163 6b65 6e64  .....)...Backend
 000000a0: da04 4261 7368 da06 476f 6f67 6c65 da10  ..Bash..Google..
 000000b0: 4875 6767 696e 6746 6163 6545 6d62 6564  HuggingFaceEmbed
 000000c0: da02 4964 da08 4d61 6e69 6665 7374 da04  ..Id..Manifest..
 000000d0: 4d6f 636b da06 4f70 656e 4149 da0b 4f70  Mock..OpenAI..Op
-000000e0: 656e 4149 456d 6265 64da 0c4f 7065 6e41  enAIEmbed..OpenA
-000000f0: 4953 7472 6561 6dda 0650 7974 686f 6eda  IStream..Python.
-00000100: 0752 6571 7565 7374 da11 7365 745f 6d69  .Request..set_mi
-00000110: 6e69 6368 6169 6e5f 6c6f 67da 0b73 7461  nichain_log..sta
-00000120: 7274 5f63 6861 696e 2902 da06 7072 6f6d  rt_chain)...prom
-00000130: 7074 da0e 7479 7065 5f74 6f5f 7072 6f6d  pt..type_to_prom
-00000140: 7074 2901 da04 7368 6f77 4e29 14da 0762  pt)...showN)...b
-00000150: 6163 6b65 6e64 7202 0000 0072 0300 0000  ackendr....r....
-00000160: 7204 0000 0072 0500 0000 7206 0000 0072  r....r....r....r
-00000170: 0700 0000 7208 0000 0072 0900 0000 720a  ....r....r....r.
-00000180: 0000 0072 0b00 0000 720c 0000 0072 0d00  ...r....r....r..
-00000190: 0000 720e 0000 0072 0f00 0000 da04 6261  ..r....r......ba
-000001a0: 7365 7210 0000 0072 1100 0000 da06 6772  ser....r......gr
-000001b0: 6164 696f 7212 0000 00a9 0072 1600 0000  adior......r....
-000001c0: 7216 0000 00fa 562f 686f 6d65 2f73 7275  r.....V/home/sru
-000001d0: 7368 2f50 726f 6a65 6374 732f 4d69 6e69  sh/Projects/Mini
-000001e0: 4368 6169 6e2f 7665 6e76 2f6c 6962 2f70  Chain/venv/lib/p
-000001f0: 7974 686f 6e33 2e31 302f 7369 7465 2d70  ython3.10/site-p
-00000200: 6163 6b61 6765 732f 6d69 6e69 6368 6169  ackages/minichai
-00000210: 6e2f 5f5f 696e 6974 5f5f 2e70 79da 083c  n/__init__.py..<
-00000220: 6d6f 6475 6c65 3e01 0000 0073 0600 0000  module>....s....
-00000230: 4000 1010 1001                           @.....
+000000e0: 656e 4149 456d 6265 64da 0650 7974 686f  enAIEmbed..Pytho
+000000f0: 6eda 1173 6574 5f6d 696e 6963 6861 696e  n..set_minichain
+00000100: 5f6c 6f67 da0b 7374 6172 745f 6368 6169  _log..start_chai
+00000110: 6e29 03da 0542 7265 616b da06 7072 6f6d  n)...Break..prom
+00000120: 7074 da09 7472 616e 7366 6f72 6d29 02da  pt..transform)..
+00000130: 0a47 7261 6469 6f43 6f6e 66da 0473 686f  .GradioConf..sho
+00000140: 774e 2914 da07 6261 636b 656e 6472 0200  wN)...backendr..
+00000150: 0000 7203 0000 0072 0400 0000 7205 0000  ..r....r....r...
+00000160: 0072 0600 0000 7207 0000 0072 0800 0000  .r....r....r....
+00000170: 7209 0000 0072 0a00 0000 720b 0000 0072  r....r....r....r
+00000180: 0c00 0000 720d 0000 00da 0462 6173 6572  ....r......baser
+00000190: 0e00 0000 720f 0000 0072 1000 0000 da06  ....r....r......
+000001a0: 6772 6164 696f 7211 0000 0072 1200 0000  gradior....r....
+000001b0: a900 7216 0000 0072 1600 0000 fa56 2f68  ..r....r.....V/h
+000001c0: 6f6d 652f 7372 7573 682f 5072 6f6a 6563  ome/srush/Projec
+000001d0: 7473 2f4d 696e 6943 6861 696e 2f76 656e  ts/MiniChain/ven
+000001e0: 762f 6c69 622f 7079 7468 6f6e 332e 3130  v/lib/python3.10
+000001f0: 2f73 6974 652d 7061 636b 6167 6573 2f6d  /site-packages/m
+00000200: 696e 6963 6861 696e 2f5f 5f69 6e69 745f  inichain/__init_
+00000210: 5f2e 7079 da08 3c6d 6f64 756c 653e 0100  _.py..<module>..
+00000220: 0000 7306 0000 0038 0014 0e14 01         ..s....8.....
```

### ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/__pycache__/backend.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 22:01:03 2023 UTC, .py size: 10351 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,775 +1,814 @@
-00000000: 6f0d 0d0a 0000 0000 9f7b 3864 6f28 0000  o........{8do(..
+00000000: 6f0d 0d0a 0000 0000 26f5 3e64 ce28 0000  o.......&.>d.(..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 a201 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 ae01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c05 6d06 5a06 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 6d09 5a09 6d0a 5a0a  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  m.Z.m.Z.m.Z.m.Z.
-00000080: 0100 6400 6405 6c0f 6d10 5a10 6d11 5a11  ..d.d.l.m.Z.m.Z.
-00000090: 0100 6508 7238 6400 6401 6c12 5a12 6504  ..e.r8d.d.l.Z.e.
-000000a0: 4700 6406 6407 8400 6407 8302 8301 5a13  G.d.d...d.....Z.
-000000b0: 4700 6408 6409 8400 6409 8302 5a14 4700  G.d.d...d...Z.G.
-000000c0: 640a 640b 8400 640b 6514 8303 5a15 4700  d.d...d.e...Z.G.
-000000d0: 640c 640d 8400 640d 6514 8303 5a16 4700  d.d...d.e...Z.G.
-000000e0: 640e 640f 8400 640f 6514 8303 5a17 4700  d.d...d.e...Z.G.
-000000f0: 6410 6411 8400 6411 6514 8303 5a18 4700  d.d...d.e...Z.G.
-00000100: 6412 6413 8400 6413 6514 8303 5a19 4700  d.d...d.e...Z.G.
-00000110: 6414 6415 8400 6415 6514 8303 5a1a 4700  d.d...d.e...Z.G.
-00000120: 6416 6417 8400 6417 8302 5a1b 4700 6418  d.d...d...Z.G.d.
-00000130: 6419 8400 6419 651a 8303 5a1c 4700 641a  d...d.e...Z.G.d.
-00000140: 641b 8400 641b 651a 8303 5a1d 4700 641c  d...d.e...Z.G.d.
-00000150: 641d 8400 641d 6514 8303 5a1e 4700 641e  d...d.e...Z.G.d.
-00000160: 641f 8400 641f 651e 8303 5a1f 4700 6420  d...d.e...Z.G.d 
-00000170: 6421 8400 6421 651e 8303 5a20 4700 6422  d!..d!e...Z G.d"
-00000180: 6423 8400 6423 6514 8303 5a21 4700 6424  d#..d#e...Z!G.d$
-00000190: 6425 8400 6425 8302 5a22 6426 6523 6427  d%..d%..Z"d&e#d'
-000001a0: 6401 6604 6428 6429 8404 5a24 4700 642a  d.f.d(d)..Z$G.d*
-000001b0: 642b 8400 642b 8302 5a25 6426 6523 6427  d+..d+..Z%d&e#d'
-000001c0: 6525 6604 642c 642d 8404 5a26 6401 5300  e%f.d,d-..Z&d.S.
-000001d0: 292e e900 0000 004e 2901 da09 6461 7461  )......N)...data
-000001e0: 636c 6173 7329 01da 0d54 7261 6365 6261  class)...Traceba
-000001f0: 636b 5479 7065 2907 da0d 5459 5045 5f43  ckType)...TYPE_C
-00000200: 4845 434b 494e 47da 0341 6e79 da04 4469  HECKING..Any..Di
-00000210: 6374 da04 4c69 7374 da08 4f70 7469 6f6e  ct..List..Option
-00000220: 616c da08 5365 7175 656e 6365 da05 5475  al..Sequence..Tu
-00000230: 706c 6529 02da 0c73 7461 7274 5f61 6374  ple)...start_act
-00000240: 696f 6eda 0774 6f5f 6669 6c65 6300 0000  ion..to_filec...
-00000250: 0000 0000 0000 0000 0000 0000 0003 0000  ................
-00000260: 0040 0000 0073 2a00 0000 6500 5a01 6400  .@...s*...e.Z.d.
-00000270: 5a02 5500 6503 6504 6401 3c00 6402 5a05  Z.U.e.e.d.<.d.Z.
-00000280: 6506 6507 6503 1900 1900 6504 6403 3c00  e.e.e.....e.d.<.
-00000290: 6402 5300 2904 da07 5265 7175 6573 74da  d.S.)...Request.
-000002a0: 0670 726f 6d70 744e da04 7374 6f70 2908  .promptN..stop).
-000002b0: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-000002c0: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-000002d0: 6d65 5f5f da03 7374 72da 0f5f 5f61 6e6e  me__..str..__ann
-000002e0: 6f74 6174 696f 6e73 5f5f 720f 0000 0072  otations__r....r
-000002f0: 0800 0000 7209 0000 00a9 0072 1500 0000  ....r......r....
-00000300: 7215 0000 00fa 552f 686f 6d65 2f73 7275  r.....U/home/sru
-00000310: 7368 2f50 726f 6a65 6374 732f 4d69 6e69  sh/Projects/Mini
-00000320: 4368 6169 6e2f 7665 6e76 2f6c 6962 2f70  Chain/venv/lib/p
-00000330: 7974 686f 6e33 2e31 302f 7369 7465 2d70  ython3.10/site-p
-00000340: 6163 6b61 6765 732f 6d69 6e69 6368 6169  ackages/minichai
-00000350: 6e2f 6261 636b 656e 642e 7079 720d 0000  n/backend.pyr...
-00000360: 000e 0000 0073 0600 0000 0a00 0802 1801  .....s..........
-00000370: 720d 0000 0063 0000 0000 0000 0000 0000  r....c..........
-00000380: 0000 0000 0000 0400 0000 4000 0000 7340  ..........@...s@
-00000390: 0000 0065 005a 0164 005a 0264 015a 0365  ...e.Z.d.Z.d.Z.e
-000003a0: 0464 0264 0384 0083 015a 0564 0465 0664  .d.d.....Z.d.e.d
-000003b0: 0565 0766 0464 0664 0784 045a 0864 0465  .e.f.d.d...Z.d.e
-000003c0: 0664 0565 0766 0464 0864 0984 045a 0964  .d.e.f.d.d...Z.d
-000003d0: 0a53 0029 0bda 0742 6163 6b65 6e64 5463  .S.)...BackendTc
-000003e0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-000003f0: 0100 0000 4300 0000 f304 0000 0064 0153  ....C........d.S
-00000400: 00a9 024e da00 7215 0000 00a9 01da 0473  ...N..r........s
-00000410: 656c 6672 1500 0000 7215 0000 0072 1600  elfr....r....r..
-00000420: 0000 da0b 6465 7363 7269 7074 696f 6e17  ....description.
-00000430: 0000 0073 0200 0000 0402 7a13 4261 636b  ...s......z.Back
-00000440: 656e 642e 6465 7363 7269 7074 696f 6eda  end.description.
-00000450: 0772 6571 7565 7374 da06 7265 7475 726e  .request..return
-00000460: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00000470: 0001 0000 0043 0000 0073 0400 0000 7400  .....C...s....t.
-00000480: 8201 a901 4e29 01da 134e 6f74 496d 706c  ....N)...NotImpl
-00000490: 656d 656e 7465 6445 7272 6f72 a902 721c  ementedError..r.
-000004a0: 0000 0072 1e00 0000 7215 0000 0072 1500  ...r....r....r..
-000004b0: 0000 7216 0000 00da 0372 756e 1b00 0000  ..r......run....
-000004c0: f302 0000 0004 017a 0b42 6163 6b65 6e64  .......z.Backend
-000004d0: 2e72 756e 6302 0000 0000 0000 0000 0000  .runc...........
-000004e0: 0002 0000 0003 0000 00c3 0000 0073 0c00  .............s..
-000004f0: 0000 8101 7c00 a000 7c01 a101 5300 7220  ....|...|...S.r 
-00000500: 0000 0029 0172 2300 0000 7222 0000 0072  ...).r#...r"...r
-00000510: 1500 0000 7215 0000 0072 1600 0000 da04  ....r....r......
-00000520: 6172 756e 1e00 0000 7304 0000 0002 800a  arun....s.......
-00000530: 017a 0c42 6163 6b65 6e64 2e61 7275 6e4e  .z.Backend.arunN
-00000540: 290a 7210 0000 0072 1100 0000 7212 0000  ).r....r....r...
-00000550: 00da 0d6e 6565 6473 5f72 6571 7565 7374  ...needs_request
-00000560: da08 7072 6f70 6572 7479 721d 0000 0072  ..propertyr....r
-00000570: 0d00 0000 7213 0000 0072 2300 0000 7225  ....r....r#...r%
-00000580: 0000 0072 1500 0000 7215 0000 0072 1500  ...r....r....r..
-00000590: 0000 7216 0000 0072 1700 0000 1400 0000  ..r....r........
-000005a0: 730c 0000 0008 0004 0102 020a 0112 0316  s...............
-000005b0: 0372 1700 0000 6300 0000 0000 0000 0000  .r....c.........
-000005c0: 0000 0000 0000 0004 0000 0040 0000 00f3  ...........@....
-000005d0: 1e00 0000 6500 5a01 6400 5a02 6401 6503  ....e.Z.d.Z.d.e.
-000005e0: 6402 6504 6604 6403 6404 8404 5a05 6405  d.e.f.d.d...Z.d.
-000005f0: 5300 2906 da02 4964 721e 0000 0072 1f00  S.)...Idr....r..
-00000600: 0000 6302 0000 0000 0000 0000 0000 0002  ..c.............
-00000610: 0000 0001 0000 0043 0000 0073 0600 0000  .......C...s....
-00000620: 7c01 6a00 5300 7220 0000 0029 0172 0e00  |.j.S.r ...).r..
-00000630: 0000 7222 0000 0072 1500 0000 7215 0000  ..r"...r....r...
-00000640: 0072 1600 0000 7223 0000 0023 0000 0073  .r....r#...#...s
-00000650: 0200 0000 0601 7a06 4964 2e72 756e 4ea9  ......z.Id.runN.
-00000660: 0672 1000 0000 7211 0000 0072 1200 0000  .r....r....r....
-00000670: 720d 0000 0072 1300 0000 7223 0000 0072  r....r....r#...r
-00000680: 1500 0000 7215 0000 0072 1500 0000 7216  ....r....r....r.
-00000690: 0000 0072 2900 0000 2200 0000 f304 0000  ...r)...".......
-000006a0: 0008 0016 0172 2900 0000 6300 0000 0000  .....r)...c.....
-000006b0: 0000 0000 0000 0000 0000 0004 0000 0040  ...............@
-000006c0: 0000 0073 5400 0000 6500 5a01 6400 5a02  ...sT...e.Z.d.Z.
-000006d0: 6700 6601 6401 6503 6504 1900 6602 6402  g.f.d.e.e...f.d.
-000006e0: 6403 8405 5a05 6404 6506 6405 6504 6604  d...Z.d.e.d.e.f.
-000006f0: 6406 6407 8404 5a07 6404 6506 6405 6504  d.d...Z.d.e.d.e.
-00000700: 6604 6408 6409 8404 5a08 6405 6504 6602  f.d.d...Z.d.e.f.
-00000710: 640a 640b 8404 5a09 640c 5300 290d da04  d.d...Z.d.S.)...
-00000720: 4d6f 636b da07 616e 7377 6572 7363 0200  Mock..answersc..
-00000730: 0000 0000 0000 0000 0000 0200 0000 0200  ................
-00000740: 0000 4300 0000 7310 0000 0064 017c 005f  ..C...s....d.|._
-00000750: 007c 017c 005f 0164 0053 0029 024e e9ff  .|.|._.d.S.).N..
-00000760: ffff ff29 02da 0169 722d 0000 00a9 0272  ...)...ir-.....r
-00000770: 1c00 0000 722d 0000 0072 1500 0000 7215  ....r-...r....r.
-00000780: 0000 0072 1600 0000 da08 5f5f 696e 6974  ...r......__init
-00000790: 5f5f 2800 0000 7304 0000 0006 010a 017a  __(...s........z
-000007a0: 0d4d 6f63 6b2e 5f5f 696e 6974 5f5f 721e  .Mock.__init__r.
-000007b0: 0000 0072 1f00 0000 6302 0000 0000 0000  ...r....c.......
-000007c0: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
-000007d0: 0073 2400 0000 7c00 0400 6a00 6401 3700  .s$...|...j.d.7.
-000007e0: 0200 5f00 7c00 6a01 7c00 6a00 7402 7c00  .._.|.j.|.j.t.|.
-000007f0: 6a01 8301 1600 1900 5300 2902 4ee9 0100  j.......S.).N...
-00000800: 0000 2903 722f 0000 0072 2d00 0000 da03  ..).r/...r-.....
-00000810: 6c65 6e72 2200 0000 7215 0000 0072 1500  lenr"...r....r..
-00000820: 0000 7216 0000 0072 2300 0000 2c00 0000  ..r....r#...,...
-00000830: 7304 0000 000e 0116 017a 084d 6f63 6b2e  s........z.Mock.
-00000840: 7275 6e63 0200 0000 0000 0000 0000 0000  runc............
-00000850: 0400 0000 0400 0000 6300 0000 7344 0000  ........c...sD..
-00000860: 0081 007c 0004 006a 0064 0137 0002 005f  ...|...j.d.7..._
-00000870: 007c 006a 017c 006a 0074 027c 006a 0183  .|.j.|.j.t.|.j..
-00000880: 0116 0019 007d 027c 0244 005d 0a7d 037c  .....}.|.D.].}.|
-00000890: 0356 0001 0074 03a0 0464 02a1 0101 0071  .V...t...d.....q
-000008a0: 1564 0053 0029 034e 7232 0000 00e9 0a00  .d.S.).Nr2......
-000008b0: 0000 2905 722f 0000 0072 2d00 0000 7233  ..).r/...r-...r3
-000008c0: 0000 00da 0474 696d 65da 0573 6c65 6570  .....time..sleep
-000008d0: 2904 721c 0000 0072 1e00 0000 da06 7265  ).r....r......re
-000008e0: 7375 6c74 da01 6372 1500 0000 7215 0000  sult..cr....r...
-000008f0: 0072 1600 0000 da0a 7275 6e5f 7374 7265  .r......run_stre
-00000900: 616d 3000 0000 730e 0000 0002 800e 0116  am0...s.........
-00000910: 0108 0106 010c 0104 fe7a 0f4d 6f63 6b2e  .........z.Mock.
-00000920: 7275 6e5f 7374 7265 616d 6301 0000 0000  run_streamc.....
-00000930: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
-00000940: 0000 00f3 0c00 0000 6401 7c00 6a00 9b00  ........d.|.j...
-00000950: 9d02 5300 2902 4e7a 0f4d 6f63 6b65 6420  ..S.).Nz.Mocked 
-00000960: 4261 636b 656e 6420 2901 722d 0000 0072  Backend ).r-...r
-00000970: 1b00 0000 7215 0000 0072 1500 0000 7216  ....r....r....r.
-00000980: 0000 00da 085f 5f72 6570 725f 5f37 0000  .....__repr__7..
-00000990: 00f3 0200 0000 0c01 7a0d 4d6f 636b 2e5f  ........z.Mock._
-000009a0: 5f72 6570 725f 5f4e 290a 7210 0000 0072  _repr__N).r....r
-000009b0: 1100 0000 7212 0000 0072 0700 0000 7213  ....r....r....r.
-000009c0: 0000 0072 3100 0000 720d 0000 0072 2300  ...r1...r....r#.
-000009d0: 0000 7239 0000 0072 3b00 0000 7215 0000  ..r9...r;...r...
-000009e0: 0072 1500 0000 7215 0000 0072 1600 0000  .r....r....r....
-000009f0: 722c 0000 0027 0000 0073 0a00 0000 0800  r,...'...s......
-00000a00: 1601 1204 1204 1207 722c 0000 0063 0000  ........r,...c..
-00000a10: 0000 0000 0000 0000 0000 0000 0000 0400  ................
-00000a20: 0000 4000 0000 7336 0000 0065 005a 0164  ..@...s6...e.Z.d
-00000a30: 005a 0264 0a64 0364 0484 045a 0364 0565  .Z.d.d.d...Z.d.e
-00000a40: 0464 0165 0566 0464 0664 0784 045a 0664  .d.e.f.d.d...Z.d
-00000a50: 0165 0566 0264 0864 0984 045a 0764 0253  .e.f.d.d...Z.d.S
-00000a60: 0029 0bda 0647 6f6f 676c 6572 1f00 0000  .)...Googler....
-00000a70: 4e63 0100 0000 0000 0000 0000 0000 0100  Nc..............
-00000a80: 0000 0100 0000 4300 0000 f304 0000 0064  ......C........d
-00000a90: 0053 0072 2000 0000 7215 0000 0072 1b00  .S.r ...r....r..
-00000aa0: 0000 7215 0000 0072 1500 0000 7216 0000  ..r....r....r...
-00000ab0: 0072 3100 0000 3c00 0000 7224 0000 007a  .r1...<...r$...z
-00000ac0: 0f47 6f6f 676c 652e 5f5f 696e 6974 5f5f  .Google.__init__
-00000ad0: 721e 0000 0063 0200 0000 0000 0000 0000  r....c..........
-00000ae0: 0000 0800 0000 0700 0000 4300 0000 731c  ..........C...s.
-00000af0: 0100 0064 0164 026c 006d 017d 0201 0074  ...d.d.l.m.}...t
-00000b00: 026a 03a0 0464 03a1 017d 037c 0373 124a  .j...d...}.|.s.J
-00000b10: 0064 0483 0182 017c 037c 005f 057c 006a  .d.....|.|._.|.j
-00000b20: 0564 057c 016a 0664 0664 0764 0864 099c  .d.|.j.d.d.d.d..
-00000b30: 067d 047c 027c 0483 017d 057c 05a0 07a1  .}.|.|...}.|....
-00000b40: 007d 0664 0a7c 06a0 08a1 0076 0072 4064  .}.d.|.....v.r@d
-00000b50: 0b7c 0664 0a19 00a0 08a1 0076 0072 407c  .|.d.......v.r@|
-00000b60: 0664 0a19 0064 0b19 007d 0774 097c 0783  .d...d...}.t.|..
-00000b70: 0153 0064 0a7c 06a0 08a1 0076 0072 5864  .S.d.|.....v.rXd
-00000b80: 0c7c 0664 0a19 00a0 08a1 0076 0072 587c  .|.d.......v.rX|
-00000b90: 0664 0a19 0064 0c19 007d 0774 097c 0783  .d...d...}.t.|..
-00000ba0: 0153 0064 0a7c 06a0 08a1 0076 0072 7264  .S.d.|.....v.rrd
-00000bb0: 0d7c 0664 0a19 00a0 08a1 0076 0072 727c  .|.d.......v.rr|
-00000bc0: 0664 0a19 0064 0d19 0064 0119 007d 0774  .d...d...d...}.t
-00000bd0: 097c 0783 0153 0064 0c7c 0664 0e19 0064  .|...S.d.|.d...d
-00000be0: 0119 00a0 08a1 0076 0072 887c 0664 0e19  .......v.r.|.d..
-00000bf0: 0064 0119 0064 0c19 007d 0774 097c 0783  .d...d...}.t.|..
-00000c00: 0153 0064 0f7d 0774 097c 0783 0153 0029  .S.d.}.t.|...S.)
-00000c10: 104e 7201 0000 0029 01da 0c47 6f6f 676c  .Nr....)...Googl
-00000c20: 6553 6561 7263 68da 0853 4552 505f 4b45  eSearch..SERP_KE
-00000c30: 597a 3f4e 6565 6420 6120 5345 5250 5f4b  Yz?Need a SERP_K
-00000c40: 4559 2e20 4765 7420 6f6e 6520 6865 7265  EY. Get one here
-00000c50: 2068 7474 7073 3a2f 2f73 6572 7061 7069   https://serpapi
-00000c60: 2e63 6f6d 2f75 7365 7273 2f77 656c 636f  .com/users/welco
-00000c70: 6d65 da06 676f 6f67 6c65 7a0a 676f 6f67  me..googlez.goog
-00000c80: 6c65 2e63 6f6d da02 7573 da02 656e 2906  le.com..us..en).
-00000c90: da07 6170 695f 6b65 79da 0665 6e67 696e  ..api_key..engin
-00000ca0: 65da 0171 da0d 676f 6f67 6c65 5f64 6f6d  e..q..google_dom
-00000cb0: 6169 6eda 0267 6cda 0268 6cda 0a61 6e73  ain..gl..hl..ans
-00000cc0: 7765 725f 626f 78da 0661 6e73 7765 72da  wer_box..answer.
-00000cd0: 0773 6e69 7070 6574 da19 736e 6970 7065  .snippet..snippe
-00000ce0: 745f 6869 6768 6c69 6768 7465 645f 776f  t_highlighted_wo
-00000cf0: 7264 73da 0f6f 7267 616e 6963 5f72 6573  rds..organic_res
-00000d00: 756c 7473 721a 0000 0029 0ada 0773 6572  ultsr....)...ser
-00000d10: 7061 7069 723f 0000 00da 026f 73da 0765  papir?.....os..e
-00000d20: 6e76 6972 6f6e da03 6765 74da 0b73 6572  nviron..get..ser
-00000d30: 7061 7069 5f6b 6579 720e 0000 00da 0867  papi_keyr......g
-00000d40: 6574 5f64 6963 74da 046b 6579 7372 1300  et_dict..keysr..
-00000d50: 0000 2908 721c 0000 0072 1e00 0000 723f  ..).r....r....r?
-00000d60: 0000 0072 5300 0000 da06 7061 7261 6d73  ...rS.....params
-00000d70: da06 7365 6172 6368 da03 7265 73da 0574  ..search..res..t
-00000d80: 6f72 6574 7215 0000 0072 1500 0000 7216  oretr....r....r.
-00000d90: 0000 0072 2300 0000 3f00 0000 7342 0000  ...r#...?...sB..
-00000da0: 000c 010c 0202 0204 ff02 0204 fe06 0304  ................
-00000db0: 0302 0104 0102 0102 0102 0106 fa08 0908  ................
-00000dc0: 011c 020c 0108 0c1c f50c 0108 0a0a f802  ................
-00000dd0: ff0e 0202 fe10 0408 0514 fc10 0108 0304  ................
-00000de0: ff08 017a 0a47 6f6f 676c 652e 7275 6e63  ...z.Google.runc
-00000df0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00000e00: 0100 0000 4300 0000 7218 0000 0029 024e  ....C...r....).N
-00000e10: 7a15 476f 6f67 6c65 2053 6561 7263 6820  z.Google Search 
-00000e20: 4261 636b 656e 6472 1500 0000 721b 0000  Backendr....r...
-00000e30: 0072 1500 0000 7215 0000 0072 1600 0000  .r....r....r....
-00000e40: 723b 0000 0063 0000 0072 2400 0000 7a0f  r;...c...r$...z.
-00000e50: 476f 6f67 6c65 2e5f 5f72 6570 725f 5f29  Google.__repr__)
-00000e60: 0272 1f00 0000 4e29 0872 1000 0000 7211  .r....N).r....r.
-00000e70: 0000 0072 1200 0000 7231 0000 0072 0d00  ...r....r1...r..
-00000e80: 0000 7213 0000 0072 2300 0000 723b 0000  ..r....r#...r;..
-00000e90: 0072 1500 0000 7215 0000 0072 1500 0000  .r....r....r....
-00000ea0: 7216 0000 0072 3d00 0000 3b00 0000 7308  r....r=...;...s.
-00000eb0: 0000 0008 000a 0112 0312 2472 3d00 0000  ..........$r=...
-00000ec0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000ed0: 0004 0000 0040 0000 0073 3000 0000 6500  .....@...s0...e.
-00000ee0: 5a01 6400 5a02 6401 5a03 6402 6504 6403  Z.d.Z.d.Z.d.e.d.
-00000ef0: 6505 6604 6404 6405 8404 5a06 6403 6505  e.f.d.d...Z.d.e.
-00000f00: 6602 6406 6407 8404 5a07 6408 5300 2909  f.d.d...Z.d.S.).
-00000f10: da06 5079 7468 6f6e 7a30 4578 6563 7574  ..Pythonz0Execut
-00000f20: 6573 2050 7974 686f 6e20 636f 6d6d 616e  es Python comman
-00000f30: 6473 2061 6e64 2072 6574 7572 6e73 2074  ds and returns t
-00000f40: 6865 206f 7574 7075 742e 721e 0000 0072  he output.r....r
-00000f50: 1f00 0000 6302 0000 0000 0000 0000 0000  ....c...........
-00000f60: 0007 0000 0008 0000 0043 0000 0073 8a00  .........C...s..
-00000f70: 0000 6401 6402 6c00 6d01 7d02 0100 6401  ..d.d.l.m.}...d.
-00000f80: 6403 6c02 6d03 7d03 0100 7c01 6a04 a005  d.l.m.}...|.j...
-00000f90: a100 7d04 7c04 a006 6404 a101 7224 6405  ..}.|...d...r$d.
-00000fa0: a007 7c04 a005 a100 a008 6405 a101 6406  ..|.......d...d.
-00000fb0: 6407 8502 1900 a101 7d04 7c03 8300 7d05  d.......}.|...}.
-00000fc0: 7c02 7c05 8301 8f0c 0100 7409 7c04 8301  |.|.......t.|...
-00000fd0: 0100 5700 6408 0400 0400 8303 0100 6e08  ..W.d.........n.
-00000fe0: 3100 733a 7701 0100 0100 0100 5900 0100  1.s:w.......Y...
-00000ff0: 7c05 a00a a100 7d06 7c06 5300 2909 fa25  |.....}.|.S.)..%
-00001000: 5275 6e20 636f 6d6d 616e 6473 2061 6e64  Run commands and
-00001010: 2072 6574 7572 6e20 6669 6e61 6c20 6f75   return final ou
-00001020: 7470 7574 2e72 0100 0000 2901 da0f 7265  tput.r....)...re
-00001030: 6469 7265 6374 5f73 7464 6f75 7429 01da  direct_stdout)..
-00001040: 0853 7472 696e 6749 4f7a 0360 6060 da01  .StringIOz.```..
-00001050: 0a72 3200 0000 722e 0000 004e 290b da0a  .r2...r....N)...
-00001060: 636f 6e74 6578 746c 6962 725c 0000 00da  contextlibr\....
-00001070: 0269 6f72 5d00 0000 720e 0000 00da 0573  .ior]...r......s
-00001080: 7472 6970 da0a 7374 6172 7473 7769 7468  trip..startswith
-00001090: da04 6a6f 696e da05 7370 6c69 74da 0465  ..join..split..e
-000010a0: 7865 63da 0867 6574 7661 6c75 6529 0772  xec..getvalue).r
-000010b0: 1c00 0000 721e 0000 0072 5c00 0000 725d  ....r....r\...r]
-000010c0: 0000 00da 0170 da01 66da 0173 7215 0000  .....p..f..sr...
-000010d0: 0072 1500 0000 7216 0000 0072 2300 0000  .r....r....r#...
-000010e0: 6a00 0000 7316 0000 000c 020c 010a 020a  j...s...........
-000010f0: 011c 0106 020a 010a 011c ff08 0204 017a  ...............z
-00001100: 0a50 7974 686f 6e2e 7275 6e63 0100 0000  .Python.runc....
-00001110: 0000 0000 0000 0000 0100 0000 0100 0000  ................
-00001120: 4300 0000 7218 0000 0029 024e 7a0e 5079  C...r....).Nz.Py
-00001130: 7468 6f6e 2d42 6163 6b65 6e64 7215 0000  thon-Backendr...
-00001140: 0072 1b00 0000 7215 0000 0072 1500 0000  .r....r....r....
-00001150: 7216 0000 0072 3b00 0000 7900 0000 7224  r....r;...y...r$
-00001160: 0000 007a 0f50 7974 686f 6e2e 5f5f 7265  ...z.Python.__re
-00001170: 7072 5f5f 4e29 0872 1000 0000 7211 0000  pr__N).r....r...
-00001180: 0072 1200 0000 da07 5f5f 646f 635f 5f72  .r......__doc__r
-00001190: 0d00 0000 7213 0000 0072 2300 0000 723b  ....r....r#...r;
-000011a0: 0000 0072 1500 0000 7215 0000 0072 1500  ...r....r....r..
-000011b0: 0000 7216 0000 0072 5a00 0000 6700 0000  ..r....rZ...g...
-000011c0: 7308 0000 0008 0004 0112 0212 0f72 5a00  s............rZ.
-000011d0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-000011e0: 0000 0005 0000 0040 0000 0073 4400 0000  .......@...sD...
-000011f0: 6500 5a01 6400 5a02 6401 5a03 640e 6403  e.Z.d.Z.d.Z.d.d.
-00001200: 6504 6404 6504 6604 6405 6406 8405 5a05  e.d.e.f.d.d...Z.
-00001210: 6407 6506 6408 6507 6604 6409 640a 8404  d.e.d.e.f.d.d...
-00001220: 5a08 6408 6507 6602 640b 640c 8404 5a09  Z.d.e.f.d.d...Z.
-00001230: 640d 5300 290f da04 4261 7368 7a2e 4578  d.S.)...Bashz.Ex
-00001240: 6563 7574 6573 2062 6173 6820 636f 6d6d  ecutes bash comm
-00001250: 616e 6473 2061 6e64 2072 6574 7572 6e73  ands and returns
-00001260: 2074 6865 206f 7574 7075 742e 46da 0e73   the output.F..s
-00001270: 7472 6970 5f6e 6577 6c69 6e65 73da 1172  trip_newlines..r
-00001280: 6574 7572 6e5f 6572 725f 6f75 7470 7574  eturn_err_output
-00001290: 6303 0000 0000 0000 0000 0000 0003 0000  c...............
-000012a0: 0002 0000 0043 0000 0073 1000 0000 7c01  .....C...s....|.
-000012b0: 7c00 5f00 7c02 7c00 5f01 6401 5300 2902  |._.|.|._.d.S.).
-000012c0: 7a23 496e 6974 6961 6c69 7a65 2077 6974  z#Initialize wit
-000012d0: 6820 7374 7269 7070 696e 6720 6e65 776c  h stripping newl
-000012e0: 696e 6573 2e4e 2902 726c 0000 0072 6d00  ines.N).rl...rm.
-000012f0: 0000 2903 721c 0000 0072 6c00 0000 726d  ..).r....rl...rm
-00001300: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
-00001310: 0000 7231 0000 0080 0000 0073 0400 0000  ..r1.......s....
-00001320: 0602 0a01 7a0d 4261 7368 2e5f 5f69 6e69  ....z.Bash.__ini
-00001330: 745f 5f72 1e00 0000 721f 0000 0063 0200  t__r....r....c..
-00001340: 0000 0000 0000 0000 0000 0400 0000 0a00  ................
-00001350: 0000 4300 0000 7386 0000 007a 1274 006a  ..C...s....z.t.j
-00001360: 017c 016a 0264 0164 0174 006a 0374 006a  .|.j.d.d.t.j.t.j
-00001370: 0464 028d 056a 05a0 06a1 007d 0257 006e  .d...j.....}.W.n
-00001380: 2704 0074 006a 0779 3901 007d 0301 007a  '..t.j.y9..}...z
-00001390: 1a7c 006a 0872 2b74 097c 036a 05a0 06a1  .|.j.r+t.|.j....
-000013a0: 0083 0157 0006 0059 0064 037d 037e 0353  ...W...Y.d.}.~.S
-000013b0: 0074 097c 0383 0157 0006 0059 0064 037d  .t.|...W...Y.d.}
-000013c0: 037e 0353 0064 037d 037e 0377 0177 007c  .~.S.d.}.~.w.w.|
-000013d0: 006a 0a72 417c 02a0 0ba1 007d 027c 0253  .j.rA|.....}.|.S
-000013e0: 0029 0472 5b00 0000 5429 04da 0573 6865  .).r[...T)...she
-000013f0: 6c6c da05 6368 6563 6bda 0673 7464 6f75  ll..check..stdou
-00001400: 74da 0673 7464 6572 724e 290c da0a 7375  t..stderrN)...su
-00001410: 6270 726f 6365 7373 7223 0000 0072 0e00  bprocessr#...r..
-00001420: 0000 da04 5049 5045 da06 5354 444f 5554  ....PIPE..STDOUT
-00001430: 7270 0000 00da 0664 6563 6f64 65da 1243  rp.....decode..C
-00001440: 616c 6c65 6450 726f 6365 7373 4572 726f  alledProcessErro
-00001450: 7272 6d00 0000 7213 0000 0072 6c00 0000  rrm...r....rl...
-00001460: 7261 0000 0029 0472 1c00 0000 721e 0000  ra...).r....r...
-00001470: 00da 066f 7574 7075 74da 0565 7272 6f72  ...output..error
-00001480: 7215 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
-00001490: 2300 0000 8500 0000 7326 0000 0002 0204  #.......s&......
-000014a0: 0104 0102 0102 0104 0104 0104 fb06 0606  ................
-000014b0: fa10 0706 011a 0114 0108 8002 fd06 0408  ................
-000014c0: 0104 017a 0842 6173 682e 7275 6e63 0100  ...z.Bash.runc..
-000014d0: 0000 0000 0000 0000 0000 0100 0000 0100  ................
-000014e0: 0000 4300 0000 7218 0000 0029 024e 7a0c  ..C...r....).Nz.
-000014f0: 4261 7368 2d42 6163 6b65 6e64 7215 0000  Bash-Backendr...
-00001500: 0072 1b00 0000 7215 0000 0072 1500 0000  .r....r....r....
-00001510: 7216 0000 0072 3b00 0000 9700 0000 7224  r....r;.......r$
-00001520: 0000 007a 0d42 6173 682e 5f5f 7265 7072  ...z.Bash.__repr
-00001530: 5f5f 4e29 0246 4629 0a72 1000 0000 7211  __N).FF).r....r.
-00001540: 0000 0072 1200 0000 726a 0000 00da 0462  ...r....rj.....b
-00001550: 6f6f 6c72 3100 0000 720d 0000 0072 1300  oolr1...r....r..
-00001560: 0000 7223 0000 0072 3b00 0000 7215 0000  ..r#...r;...r...
-00001570: 0072 1500 0000 7215 0000 0072 1600 0000  .r....r....r....
-00001580: 726b 0000 007d 0000 0073 0a00 0000 0800  rk...}...s......
-00001590: 0401 1402 1205 1212 726b 0000 0063 0000  ........rk...c..
-000015a0: 0000 0000 0000 0000 0000 0000 0000 0900  ................
-000015b0: 0000 4000 0000 733c 0000 0065 005a 0164  ..@...s<...e.Z.d
-000015c0: 005a 0209 0109 0209 0364 0d64 0465 0364  .Z.......d.d.e.d
-000015d0: 0565 0464 0665 0564 0764 0866 0864 0964  .e.d.e.d.d.f.d.d
-000015e0: 0a84 055a 0664 0765 0366 0264 0b64 0c84  ...Z.d.e.f.d.d..
-000015f0: 045a 0764 0853 0029 0eda 0a4f 7065 6e41  .Z.d.S.)...OpenA
-00001600: 4942 6173 65fa 1074 6578 742d 6461 7669  IBase..text-davi
-00001610: 6e63 692d 3030 33e9 0001 0000 e700 0000  nci-003.........
-00001620: 0000 0000 00da 056d 6f64 656c da0a 6d61  .......model..ma
-00001630: 785f 746f 6b65 6e73 da0b 7465 6d70 6572  x_tokens..temper
-00001640: 6174 7572 6572 1f00 0000 4e63 0400 0000  aturer....Nc....
-00001650: 0000 0000 0000 0000 0400 0000 0500 0000  ................
-00001660: 4300 0000 731a 0000 007c 017c 005f 0074  C...s....|.|._.t
-00001670: 017c 017c 027c 0364 018d 037c 005f 0264  .|.|.|.d...|._.d
-00001680: 0053 0029 024e 2903 727e 0000 0072 7f00  .S.).N).r~...r..
-00001690: 0000 7280 0000 0029 0372 7e00 0000 da04  ..r....).r~.....
-000016a0: 6469 6374 da07 6f70 7469 6f6e 7329 0472  dict..options).r
-000016b0: 1c00 0000 727e 0000 0072 7f00 0000 7280  ....r~...r....r.
-000016c0: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
-000016d0: 0000 7231 0000 009c 0000 0073 0c00 0000  ..r1.......s....
-000016e0: 0606 0201 0201 0201 0201 0cfd 7a13 4f70  ............z.Op
-000016f0: 656e 4149 4261 7365 2e5f 5f69 6e69 745f  enAIBase.__init_
-00001700: 5f63 0100 0000 0000 0000 0000 0000 0100  _c..............
-00001710: 0000 0200 0000 4300 0000 723a 0000 0029  ......C...r:...)
-00001720: 024e 7a0f 4f70 656e 4149 2042 6163 6b65  .Nz.OpenAI Backe
-00001730: 6e64 2029 0172 8200 0000 721b 0000 0072  nd ).r....r....r
-00001740: 1500 0000 7215 0000 0072 1600 0000 723b  ....r....r....r;
-00001750: 0000 00a9 0000 0072 3c00 0000 7a13 4f70  .......r<...z.Op
-00001760: 656e 4149 4261 7365 2e5f 5f72 6570 725f  enAIBase.__repr_
-00001770: 5f29 0372 7b00 0000 727c 0000 0072 7d00  _).r{...r|...r}.
-00001780: 0000 2908 7210 0000 0072 1100 0000 7212  ..).r....r....r.
-00001790: 0000 0072 1300 0000 da03 696e 74da 0566  ...r......int..f
-000017a0: 6c6f 6174 7231 0000 0072 3b00 0000 7215  loatr1...r;...r.
-000017b0: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
-000017c0: 0000 727a 0000 009b 0000 0073 1c00 0000  ..rz.......s....
-000017d0: 0800 0203 0201 0201 04fc 0202 02fe 0203  ................
-000017e0: 02fd 0204 02fc 0205 0afb 120d 727a 0000  ............rz..
-000017f0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00001800: 0000 0400 0000 4000 0000 7338 0000 0065  ......@...s8...e
-00001810: 005a 0164 005a 0267 0066 0164 0165 0365  .Z.d.Z.g.f.d.e.e
-00001820: 0419 0066 0264 0264 0384 055a 0564 0464  ...f.d.d...Z.d.d
-00001830: 0584 005a 0664 0665 0466 0264 0764 0884  ...Z.d.e.f.d.d..
-00001840: 045a 0764 0953 0029 0ada 0c4f 7065 6e41  .Z.d.S.)...OpenA
-00001850: 4953 7472 6561 6d72 2d00 0000 6302 0000  IStreamr-...c...
-00001860: 0000 0000 0000 0000 0002 0000 0001 0000  ................
-00001870: 0043 0000 0072 3e00 0000 7220 0000 0072  .C...r>...r ...r
-00001880: 1500 0000 7230 0000 0072 1500 0000 7215  ....r0...r....r.
-00001890: 0000 0072 1600 0000 7231 0000 00ae 0000  ...r....r1......
-000018a0: 0072 2400 0000 7a15 4f70 656e 4149 5374  .r$...z.OpenAISt
-000018b0: 7265 616d 2e5f 5f69 6e69 745f 5f63 0200  ream.__init__c..
-000018c0: 0000 0000 0000 0000 0000 0500 0000 0500  ................
-000018d0: 0000 6300 0000 737a 0000 0081 0064 0164  ..c...sz.....d.d
-000018e0: 006c 007d 0274 016a 02a0 0364 02a1 017c  .l.}.t.j...d...|
-000018f0: 005f 047c 006a 0473 134a 0064 0383 0182  ._.|.j.s.J.d....
-00001900: 017c 006a 047c 025f 047c 026a 056a 0664  .|.j.|._.|.j.j.d
-00001910: 0464 057c 0164 069c 0267 0164 0764 088d  .d.|.d...g.d.d..
-00001920: 0344 005d 167d 037c 0364 0919 0064 0119  .D.].}.|.d...d..
-00001930: 00a0 0364 0a69 00a1 02a0 0364 0ba1 017d  ...d.i.....d...}
-00001940: 047c 0464 0075 0172 3a7c 0456 0001 0071  .|.d.u.r:|.V...q
-00001950: 2464 0053 0029 0c4e 7201 0000 00da 0e4f  $d.S.).Nr......O
-00001960: 5045 4e41 495f 4150 495f 4b45 59fa 3c4e  PENAI_API_KEY.<N
-00001970: 6565 6420 616e 204f 5045 4e41 495f 4150  eed an OPENAI_AP
-00001980: 495f 4b45 592e 2047 6574 206f 6e65 2068  I_KEY. Get one h
-00001990: 6572 6520 6874 7470 733a 2f2f 6f70 656e  ere https://open
-000019a0: 6169 2e63 6f6d 2f61 7069 2f7a 0567 7074  ai.com/api/z.gpt
-000019b0: 2d34 da04 7573 6572 2902 da04 726f 6c65  -4..user)...role
-000019c0: da07 636f 6e74 656e 7454 2903 727e 0000  ..contentT).r~..
-000019d0: 00da 086d 6573 7361 6765 73da 0673 7472  ...messages..str
-000019e0: 6561 6dda 0763 686f 6963 6573 da05 6465  eam..choices..de
-000019f0: 6c74 6172 8a00 0000 2907 da06 6f70 656e  ltar....)...open
-00001a00: 6169 7250 0000 0072 5100 0000 7252 0000  airP...rQ...rR..
-00001a10: 0072 4400 0000 da0e 4368 6174 436f 6d70  .rD.....ChatComp
-00001a20: 6c65 7469 6f6e da06 6372 6561 7465 2905  letion..create).
-00001a30: 721c 0000 0072 0e00 0000 728f 0000 00da  r....r....r.....
-00001a40: 0563 6875 6e6b 728a 0000 0072 1500 0000  .chunkr....r....
-00001a50: 7215 0000 0072 1600 0000 7239 0000 00b1  r....r....r9....
-00001a60: 0000 0073 2400 0000 0280 0801 0e02 0402  ...s$...........
-00001a70: 04ff 0202 04fe 0803 0602 0201 0a01 0201  ................
-00001a80: 0afd 1a05 0801 0601 0280 04f9 7a17 4f70  ............z.Op
-00001a90: 656e 4149 5374 7265 616d 2e72 756e 5f73  enAIStream.run_s
-00001aa0: 7472 6561 6d72 1f00 0000 6301 0000 0000  treamr....c.....
-00001ab0: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
-00001ac0: 0000 0072 1800 0000 2902 4e7a 154f 7065  ...r....).Nz.Ope
-00001ad0: 6e41 4920 5374 7265 616d 2042 6163 6b65  nAI Stream Backe
-00001ae0: 6e64 7215 0000 0072 1b00 0000 7215 0000  ndr....r....r...
-00001af0: 0072 1500 0000 7216 0000 0072 3b00 0000  .r....r....r;...
-00001b00: c300 0000 7224 0000 007a 154f 7065 6e41  ....r$...z.OpenA
-00001b10: 4953 7472 6561 6d2e 5f5f 7265 7072 5f5f  IStream.__repr__
-00001b20: 4e29 0872 1000 0000 7211 0000 0072 1200  N).r....r....r..
-00001b30: 0000 7207 0000 0072 1300 0000 7231 0000  ..r....r....r1..
-00001b40: 0072 3900 0000 723b 0000 0072 1500 0000  .r9...r;...r....
-00001b50: 7215 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
-00001b60: 8500 0000 ad00 0000 7308 0000 0008 0016  ........s.......
-00001b70: 0108 0312 1272 8500 0000 6300 0000 0000  .....r....c.....
-00001b80: 0000 0000 0000 0000 0000 0004 0000 0040  ...............@
-00001b90: 0000 0073 3000 0000 6500 5a01 6400 5a02  ...s0...e.Z.d.Z.
-00001ba0: 6401 6503 6402 6504 6604 6403 6404 8404  d.e.d.e.f.d.d...
-00001bb0: 5a05 6401 6503 6402 6504 6604 6405 6406  Z.d.e.d.e.f.d.d.
-00001bc0: 8404 5a06 6407 5300 2908 da06 4f70 656e  ..Z.d.S.)...Open
-00001bd0: 4149 721e 0000 0072 1f00 0000 6302 0000  AIr....r....c...
-00001be0: 0000 0000 0000 0000 0004 0000 0006 0000  ................
-00001bf0: 0043 0000 0073 3e00 0000 6401 6400 6c00  .C...s>...d.d.l.
-00001c00: 7d02 7c02 6a01 6402 7c00 6a02 6403 1900  }.|.j.d.|.j.d...
-00001c10: 6404 7403 6a04 9b00 6405 8d04 7d02 7c02  d.t.j...d...}.|.
-00001c20: 6a05 7c01 6a06 7c01 6a07 6406 8d02 7d03  j.|.j.|.j.d...}.
-00001c30: 7408 7c03 8301 5300 2907 4e72 0100 0000  t.|...S.).Nr....
-00001c40: 728f 0000 0072 7f00 0000 da06 7371 6c69  r....r......sqli
-00001c50: 7465 2904 da0b 636c 6965 6e74 5f6e 616d  te)...client_nam
-00001c60: 6572 7f00 0000 da0a 6361 6368 655f 6e61  er......cache_na
-00001c70: 6d65 da10 6361 6368 655f 636f 6e6e 6563  me..cache_connec
-00001c80: 7469 6f6e 2901 da0e 7374 6f70 5f73 6571  tion)...stop_seq
-00001c90: 7565 6e63 6573 2909 da08 6d61 6e69 6665  uences)...manife
-00001ca0: 7374 da08 4d61 6e69 6665 7374 7282 0000  st..Manifestr...
-00001cb0: 00da 104d 696e 6963 6861 696e 436f 6e74  ...MinichainCont
-00001cc0: 6578 74da 046e 616d 6572 2300 0000 720e  ext..namer#...r.
-00001cd0: 0000 0072 0f00 0000 7213 0000 0029 0472  ...r....r....).r
-00001ce0: 1c00 0000 721e 0000 0072 9900 0000 da03  ....r....r......
-00001cf0: 616e 7372 1500 0000 7215 0000 0072 1600  ansr....r....r..
-00001d00: 0000 7223 0000 00c8 0000 0073 1800 0000  ..r#.......s....
-00001d10: 0801 0402 0201 0801 0201 0601 06fc 0407  ................
-00001d20: 0405 0401 06fa 0808 7a0a 4f70 656e 4149  ........z.OpenAI
-00001d30: 2e72 756e 6302 0000 0000 0000 0000 0000  .runc...........
-00001d40: 0004 0000 0006 0000 00c3 0000 0073 6400  .............sd.
-00001d50: 0000 8101 6401 6400 6c00 7d02 7401 6a02  ....d.d.l.}.t.j.
-00001d60: a003 6402 a101 7c00 5f04 7c02 6a05 6a06  ..d...|._.|.j.j.
-00001d70: 7c00 6a04 6403 6404 8d02 0100 7c02 6a05  |.j.d.d.....|.j.
-00001d80: 6a07 6a08 6406 6900 7c00 6a09 a401 7c01  j.j.d.i.|.j...|.
-00001d90: 6a0a 7c01 6a0b 6405 9c02 a401 8e01 4900  j.|.j.d.......I.
-00001da0: 6400 4800 7d03 740c 7c03 6a0d 6401 1900  d.H.}.t.|.j.d...
-00001db0: 6a0e 8301 5300 2907 4e72 0100 0000 7286  j...S.).Nr....r.
-00001dc0: 0000 0046 2902 7244 0000 00da 0d64 6562  ...F).rD.....deb
-00001dd0: 7567 5f65 6e61 626c 6564 2902 720f 0000  ug_enabled).r...
-00001de0: 0072 0e00 0000 7215 0000 0029 0fda 0c61  .r....r....)...a
-00001df0: 7379 6e63 5f6f 7065 6e61 6972 5000 0000  sync_openairP...
-00001e00: 7251 0000 0072 5200 0000 7244 0000 0072  rQ...rR...rD...r
-00001e10: 9300 0000 da09 636f 6e66 6967 7572 65da  ......configure.
-00001e20: 0b43 6f6d 706c 6574 696f 6e73 da0c 6173  .Completions..as
-00001e30: 796e 635f 6372 6561 7465 7282 0000 0072  ync_creater....r
-00001e40: 0f00 0000 720e 0000 0072 1300 0000 728d  ....r....r....r.
-00001e50: 0000 00da 0474 6578 7429 0472 1c00 0000  .....text).r....
-00001e60: 721e 0000 0072 9f00 0000 729d 0000 0072  r....r....r....r
-00001e70: 1500 0000 7215 0000 0072 1600 0000 7225  ....r....r....r%
-00001e80: 0000 00dc 0000 0073 1c00 0000 0280 0801  .......s........
-00001e90: 0e02 0601 0401 0201 06fe 0c04 0401 02ff  ................
-00001ea0: 0402 0401 10fd 1005 7a0b 4f70 656e 4149  ........z.OpenAI
-00001eb0: 2e61 7275 6e4e 2907 7210 0000 0072 1100  .arunN).r....r..
-00001ec0: 0000 7212 0000 0072 0d00 0000 7213 0000  ..r....r....r...
-00001ed0: 0072 2300 0000 7225 0000 0072 1500 0000  .r#...r%...r....
-00001ee0: 7215 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
-00001ef0: 9300 0000 c700 0000 7306 0000 0008 0012  ........s.......
-00001f00: 0116 1472 9300 0000 6300 0000 0000 0000  ...r....c.......
-00001f10: 0000 0000 0000 0000 0007 0000 0000 0000  ................
-00001f20: 0073 3e00 0000 6500 5a01 6400 5a02 640b  .s>...e.Z.d.Z.d.
-00001f30: 6402 6503 6403 6504 6404 6405 6606 8700  d.e.d.e.d.d.f...
-00001f40: 6601 6406 6407 840d 5a05 6408 6506 6404  f.d.d...Z.d.e.d.
-00001f50: 6503 6604 6409 640a 8404 5a07 8700 0400  e.f.d.d...Z.....
-00001f60: 5a08 5300 290c da0b 4f70 656e 4149 456d  Z.S.)...OpenAIEm
-00001f70: 6265 64fa 1674 6578 742d 656d 6265 6464  bed..text-embedd
-00001f80: 696e 672d 6164 612d 3030 3272 7e00 0000  ing-ada-002r~...
-00001f90: da06 6b77 6172 6773 721f 0000 004e 6302  ..kwargsr....Nc.
-00001fa0: 0000 0000 0000 0000 0000 0003 0000 0004  ................
-00001fb0: 0000 000b 0000 0073 1800 0000 7400 8300  .......s....t...
-00001fc0: 6a01 7c01 6601 6900 7c02 a401 8e01 0100  j.|.f.i.|.......
-00001fd0: 6400 5300 7220 0000 0029 02da 0573 7570  d.S.r ...)...sup
-00001fe0: 6572 7231 0000 0029 0372 1c00 0000 727e  err1...).r....r~
-00001ff0: 0000 0072 a600 0000 a901 da09 5f5f 636c  ...r........__cl
-00002000: 6173 735f 5f72 1500 0000 7216 0000 0072  ass__r....r....r
-00002010: 3100 0000 ed00 0000 f302 0000 0018 017a  1..............z
-00002020: 144f 7065 6e41 4945 6d62 6564 2e5f 5f69  .OpenAIEmbed.__i
-00002030: 6e69 745f 5f72 1e00 0000 6302 0000 0000  nit__r....c.....
-00002040: 0000 0000 0000 0004 0000 0004 0000 0043  ...............C
-00002050: 0000 0073 5000 0000 6401 6400 6c00 7d02  ...sP...d.d.l.}.
-00002060: 7401 6a02 a003 6402 a101 7c00 5f04 7c00  t.j...d...|._.|.
-00002070: 6a04 7312 4a00 6403 8301 8201 7c00 6a04  j.s.J.d.....|.j.
-00002080: 7c02 5f04 7c02 6a05 6a06 7c00 6a07 7c01  |._.|.j.j.|.j.|.
-00002090: 6a08 6404 8d02 7d03 7c03 6405 1900 6401  j.d...}.|.d...d.
-000020a0: 1900 6406 1900 5300 2907 4e72 0100 0000  ..d...S.).Nr....
-000020b0: 7286 0000 0072 8700 0000 2902 7245 0000  r....r....).rE..
-000020c0: 00da 0569 6e70 7574 da04 6461 7461 da09  ...input..data..
-000020d0: 656d 6265 6464 696e 6729 0972 8f00 0000  embedding).r....
-000020e0: 7250 0000 0072 5100 0000 7252 0000 0072  rP...rQ...rR...r
-000020f0: 4400 0000 da09 456d 6265 6464 696e 6772  D.....Embeddingr
-00002100: 9100 0000 727e 0000 0072 0e00 0000 2904  ....r~...r....).
-00002110: 721c 0000 0072 1e00 0000 728f 0000 0072  r....r....r....r
-00002120: 9d00 0000 7215 0000 0072 1500 0000 7216  ....r....r....r.
-00002130: 0000 0072 2300 0000 f000 0000 7318 0000  ...r#.......s...
-00002140: 0008 010e 0204 0204 ff02 0204 fe08 0306  ................
-00002150: 0204 0104 0106 fe10 047a 0f4f 7065 6e41  .........z.OpenA
-00002160: 4945 6d62 6564 2e72 756e 2901 72a5 0000  IEmbed.run).r...
-00002170: 0029 0972 1000 0000 7211 0000 0072 1200  .).r....r....r..
-00002180: 0000 7213 0000 0072 0500 0000 7231 0000  ..r....r....r1..
-00002190: 0072 0d00 0000 7223 0000 00da 0d5f 5f63  .r....r#.....__c
-000021a0: 6c61 7373 6365 6c6c 5f5f 7215 0000 0072  lasscell__r....r
-000021b0: 1500 0000 72a8 0000 0072 1600 0000 72a4  ....r....r....r.
-000021c0: 0000 00ec 0000 0073 0600 0000 0800 1c01  .......s........
-000021d0: 1a03 72a4 0000 0063 0000 0000 0000 0000  ..r....c........
-000021e0: 0000 0000 0000 0000 0500 0000 4000 0000  ............@...
-000021f0: 7320 0000 0065 005a 0164 005a 0264 0764  s ...e.Z.d.Z.d.d
-00002200: 0265 0364 0364 0466 0464 0564 0684 055a  .e.d.d.f.d.d...Z
-00002210: 0464 0453 0029 08da 0f48 7567 6769 6e67  .d.S.)...Hugging
-00002220: 4661 6365 4261 7365 da04 6770 7432 727e  FaceBase..gpt2r~
-00002230: 0000 0072 1f00 0000 4e63 0200 0000 0000  ...r....Nc......
-00002240: 0000 0000 0000 0200 0000 0200 0000 4300  ..............C.
-00002250: 0000 730a 0000 007c 017c 005f 0064 0053  ..s....|.|._.d.S
-00002260: 0072 2000 0000 2901 727e 0000 0029 0272  .r ...).r~...).r
-00002270: 1c00 0000 727e 0000 0072 1500 0000 7215  ....r~...r....r.
-00002280: 0000 0072 1600 0000 7231 0000 0001 0100  ...r....r1......
-00002290: 0073 0200 0000 0a01 7a18 4875 6767 696e  .s......z.Huggin
-000022a0: 6746 6163 6542 6173 652e 5f5f 696e 6974  gFaceBase.__init
-000022b0: 5f5f 2901 72b1 0000 0029 0572 1000 0000  __).r....).r....
-000022c0: 7211 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
-000022d0: 3100 0000 7215 0000 0072 1500 0000 7215  1...r....r....r.
-000022e0: 0000 0072 1600 0000 72b0 0000 0000 0100  ...r....r.......
-000022f0: 0073 0400 0000 0800 1801 72b0 0000 0063  .s........r....c
-00002300: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002310: 0400 0000 4000 0000 7228 0000 0029 06da  ....@...r(...)..
-00002320: 0b48 7567 6769 6e67 4661 6365 721e 0000  .HuggingFacer...
-00002330: 0072 1f00 0000 6302 0000 0000 0000 0000  .r....c.........
-00002340: 0000 0004 0000 0005 0000 0043 0000 00f3  ...........C....
-00002350: 4e00 0000 6401 6402 6c00 6d01 7d02 0100  N...d.d.l.m.}...
-00002360: 7402 6a03 a004 6403 a101 7c00 5f05 7c00  t.j...d...|._.|.
-00002370: 6a05 7314 4a00 6404 8301 8201 7c02 7c00  j.s.J.d.....|.|.
-00002380: 6a05 7c00 6a06 6405 6406 8d03 7c00 5f07  j.|.j.d.d...|._.
-00002390: 7c00 6a07 7c01 6a08 6407 8d01 7d03 7c03  |.j.|.j.d...}.|.
-000023a0: 5300 2908 4e72 0100 0000 a901 da0c 496e  S.).Nr........In
-000023b0: 6665 7265 6e63 6541 7069 da06 4846 5f4b  ferenceApi..HF_K
-000023c0: 4559 fa34 4e65 6564 2061 6e20 4846 5f4b  EY.4Need an HF_K
-000023d0: 4559 2e20 4765 7420 6f6e 6520 6865 7265  EY. Get one here
-000023e0: 2068 7474 7073 3a2f 2f68 7567 6769 6e67   https://hugging
-000023f0: 6661 6365 2e63 6f2f 7a0f 7465 7874 2d67  face.co/z.text-g
-00002400: 656e 6572 6174 696f 6ea9 03da 0574 6f6b  eneration....tok
-00002410: 656e da07 7265 706f 5f69 64da 0474 6173  en..repo_id..tas
-00002420: 6ba9 01da 0669 6e70 7574 73a9 09da 1d68  k....inputs....h
-00002430: 7567 6769 6e67 6661 6365 5f68 7562 2e69  uggingface_hub.i
-00002440: 6e66 6572 656e 6365 5f61 7069 72b5 0000  nference_apir...
-00002450: 0072 5000 0000 7251 0000 0072 5200 0000  .rP...rQ...rR...
-00002460: 7244 0000 0072 7e00 0000 da06 636c 6965  rD...r~.....clie
-00002470: 6e74 720e 0000 00a9 0472 1c00 0000 721e  ntr......r....r.
-00002480: 0000 0072 b500 0000 da08 7265 7370 6f6e  ...r......respon
-00002490: 7365 7215 0000 0072 1500 0000 7216 0000  ser....r....r...
-000024a0: 0072 2300 0000 0601 0000 f310 0000 000c  .r#.............
-000024b0: 020e 020e 0102 020a 0108 ff0e 0304 017a  ...............z
-000024c0: 0f48 7567 6769 6e67 4661 6365 2e72 756e  .HuggingFace.run
-000024d0: 4e72 2a00 0000 7215 0000 0072 1500 0000  Nr*...r....r....
-000024e0: 7215 0000 0072 1600 0000 72b2 0000 0005  r....r....r.....
-000024f0: 0100 0072 2b00 0000 72b2 0000 0063 0000  ...r+...r....c..
-00002500: 0000 0000 0000 0000 0000 0000 0000 0400  ................
-00002510: 0000 4000 0000 7228 0000 0029 06da 1048  ..@...r(...)...H
-00002520: 7567 6769 6e67 4661 6365 456d 6265 6472  uggingFaceEmbedr
-00002530: 1e00 0000 721f 0000 0063 0200 0000 0000  ....r....c......
-00002540: 0000 0000 0000 0400 0000 0500 0000 4300  ..............C.
-00002550: 0000 72b3 0000 0029 084e 7201 0000 0072  ..r....).Nr....r
-00002560: b400 0000 72b6 0000 0072 b700 0000 7a12  ....r....r....z.
-00002570: 6665 6174 7572 652d 6578 7472 6163 7469  feature-extracti
-00002580: 6f6e 72b8 0000 0072 bc00 0000 72be 0000  onr....r....r...
-00002590: 0072 c100 0000 7215 0000 0072 1500 0000  .r....r....r....
-000025a0: 7216 0000 0072 2300 0000 1501 0000 72c3  r....r#.......r.
-000025b0: 0000 007a 1448 7567 6769 6e67 4661 6365  ...z.HuggingFace
-000025c0: 456d 6265 642e 7275 6e4e 722a 0000 0072  Embed.runNr*...r
-000025d0: 1500 0000 7215 0000 0072 1500 0000 7216  ....r....r....r.
-000025e0: 0000 0072 c400 0000 1401 0000 722b 0000  ...r........r+..
-000025f0: 0072 c400 0000 6300 0000 0000 0000 0000  .r....c.........
-00002600: 0000 0000 0000 0004 0000 0040 0000 0073  ...........@...s
-00002610: 2800 0000 6500 5a01 6400 5a02 640a 6405  (...e.Z.d.Z.d.d.
-00002620: 6406 8404 5a03 6407 6504 6403 6505 6604  d...Z.d.e.d.e.f.
-00002630: 6408 6409 8404 5a06 6404 5300 290b 729a  d.d...Z.d.S.).r.
-00002640: 0000 0072 c000 0000 fa11 6d61 6e69 6665  ...r......manife
-00002650: 7374 2e4d 616e 6966 6573 7472 1f00 0000  st.Manifestr....
-00002660: 4e63 0200 0000 0000 0000 0000 0000 0200  Nc..............
-00002670: 0000 0200 0000 4300 0000 730a 0000 007c  ......C...s....|
-00002680: 017c 005f 0064 0153 0029 027a 4443 6c69  .|._.d.S.).zDCli
-00002690: 656e 7420 6672 6f6d 205b 4d61 6e69 6665  ent from [Manife
-000026a0: 7374 2d4d 4c5d 2868 7474 7073 3a2f 2f67  st-ML](https://g
-000026b0: 6974 6875 622e 636f 6d2f 4861 7a79 5265  ithub.com/HazyRe
-000026c0: 7365 6172 6368 2f6d 616e 6966 6573 7429  search/manifest)
-000026d0: 2e4e 2901 72c0 0000 0029 0272 1c00 0000  .N).r....).r....
-000026e0: 72c0 0000 0072 1500 0000 7215 0000 0072  r....r....r....r
-000026f0: 1600 0000 7231 0000 0024 0100 0073 0200  ....r1...$...s..
-00002700: 0000 0a02 7a11 4d61 6e69 6665 7374 2e5f  ....z.Manifest._
-00002710: 5f69 6e69 745f 5f72 1e00 0000 6302 0000  _init__r....c...
-00002720: 0000 0000 0000 0000 0003 0000 0008 0000  ................
-00002730: 0043 0000 0073 4800 0000 7a06 6401 6400  .C...sH...z.d.d.
-00002740: 6c00 7d02 5700 6e0b 0400 7401 7911 0100  l.}.W.n...t.y...
-00002750: 0100 0100 7401 6402 8301 8201 7700 7402  ....t.d.....w.t.
-00002760: 7c00 6a03 7c02 6a04 8302 731d 4a00 6403  |.j.|.j...s.J.d.
-00002770: 8301 8201 7c00 6a03 a005 7c01 6a06 a101  ....|.j...|.j...
-00002780: 5300 2904 4e72 0100 0000 7a36 6070 6970  S.).Nr....z6`pip
-00002790: 2069 6e73 7461 6c6c 206d 616e 6966 6573   install manifes
-000027a0: 742d 6d6c 6020 746f 2075 7365 2074 6865  t-ml` to use the
-000027b0: 204d 616e 6966 6573 7420 4261 636b 656e   Manifest Backen
-000027c0: 642e 7a2e 436c 6965 6e74 206d 7573 7420  d.z.Client must 
-000027d0: 6265 2061 2060 6d61 6e69 6665 7374 2e4d  be a `manifest.M
-000027e0: 616e 6966 6573 7460 2069 6e73 7461 6e63  anifest` instanc
-000027f0: 652e 2907 7299 0000 00da 0b49 6d70 6f72  e.).r......Impor
-00002800: 7445 7272 6f72 da0a 6973 696e 7374 616e  tError..isinstan
-00002810: 6365 72c0 0000 0072 9a00 0000 7223 0000  cer....r....r#..
-00002820: 0072 0e00 0000 2903 721c 0000 0072 1e00  .r....).r....r..
-00002830: 0000 7299 0000 0072 1500 0000 7215 0000  ..r....r....r...
-00002840: 0072 1600 0000 7223 0000 0028 0100 0073  .r....r#...(...s
-00002850: 1600 0000 0201 0c01 0c01 0801 02ff 0202  ................
-00002860: 0801 06ff 0202 04fe 0e04 7a0c 4d61 6e69  ..........z.Mani
-00002870: 6665 7374 2e72 756e 2904 72c0 0000 0072  fest.run).r....r
-00002880: c500 0000 721f 0000 004e 2907 7210 0000  ....r....N).r...
-00002890: 0072 1100 0000 7212 0000 0072 3100 0000  .r....r....r1...
-000028a0: 720d 0000 0072 1300 0000 7223 0000 0072  r....r....r#...r
-000028b0: 1500 0000 7215 0000 0072 1500 0000 7216  ....r....r....r.
-000028c0: 0000 0072 9a00 0000 2301 0000 7306 0000  ...r....#...s...
-000028d0: 0008 000a 0116 0472 9a00 0000 6300 0000  .......r....c...
-000028e0: 0000 0000 0000 0000 0000 0000 0007 0000  ................
-000028f0: 0040 0000 0073 6200 0000 6500 5a01 6400  .@...sb...e.Z.d.
-00002900: 5a02 5500 6401 5a03 6504 6505 6402 3c00  Z.U.d.Z.e.e.d.<.
-00002910: 6900 5a06 6507 6508 6504 6504 6602 1900  i.Z.e.e.e.e.f...
-00002920: 6508 6509 650a 650b 6509 6604 1900 6602  e.e.e.e.e.f...f.
-00002930: 1900 6505 6403 3c00 6900 5a0c 6507 6504  ..e.d.<.i.Z.e.e.
-00002940: 6504 6602 1900 6505 6404 3c00 6405 5a0d  e.f...e.d.<.d.Z.
-00002950: 650b 6505 6406 3c00 6407 5300 2908 729b  e.e.d.<.d.S.).r.
-00002960: 0000 0072 0100 0000 da03 6964 5fda 0c70  ...r......id_..p
-00002970: 726f 6d70 745f 7374 6f72 65da 0c70 726f  rompt_store..pro
-00002980: 6d70 745f 636f 756e 7472 1a00 0000 729c  mpt_countr....r.
-00002990: 0000 004e 290e 7210 0000 0072 1100 0000  ...N).r....r....
-000029a0: 7212 0000 0072 c800 0000 7283 0000 0072  r....r....r....r
-000029b0: 1400 0000 72c9 0000 0072 0600 0000 720a  ....r....r....r.
-000029c0: 0000 0072 0500 0000 720d 0000 0072 1300  ...r....r....r..
-000029d0: 0000 72ca 0000 0072 9c00 0000 7215 0000  ..r....r....r...
-000029e0: 0072 1500 0000 7215 0000 0072 1600 0000  .r....r....r....
-000029f0: 729b 0000 0034 0100 0073 0a00 0000 0a00  r....4...s......
-00002a00: 0c01 2801 1401 1001 729b 0000 0072 9c00  ..(.....r....r..
-00002a10: 0000 721f 0000 0063 0100 0000 0000 0000  ..r....c........
-00002a20: 0000 0000 0100 0000 0400 0000 4300 0000  ............C...
-00002a30: 7318 0000 0074 0074 017c 009b 0064 019d  s....t.t.|...d..
-00002a40: 0264 0283 0283 0101 0064 0053 00a9 034e  .d.......d.S...N
-00002a50: 7a04 2e6c 6f67 da01 7729 0272 0c00 0000  z..log..w).r....
-00002a60: da04 6f70 656e a901 729c 0000 0072 1500  ..open..r....r..
-00002a70: 0000 7215 0000 0072 1600 0000 da11 7365  ..r....r......se
-00002a80: 745f 6d69 6e69 6368 6169 6e5f 6c6f 673b  t_minichain_log;
-00002a90: 0100 0072 aa00 0000 72cf 0000 0063 0000  ...r....r....c..
-00002aa0: 0000 0000 0000 0000 0000 0000 0000 0800  ................
-00002ab0: 0000 4000 0000 734a 0000 0065 005a 0164  ..@...sJ...e.Z.d
-00002ac0: 005a 0264 015a 0364 0265 0466 0264 0364  .Z.d.Z.d.e.f.d.d
-00002ad0: 0484 045a 0564 0e64 0664 0784 045a 0664  ...Z.d.d.d...Z.d
-00002ae0: 0865 0764 0965 0865 0919 0064 0a65 0865  .e.d.e.e...d.e.e
-00002af0: 0a19 0064 0564 0b66 0864 0c64 0d84 045a  ...d.d.f.d.d...Z
-00002b00: 0b64 0b53 0029 0fda 094d 696e 6943 6861  .d.S.)...MiniCha
-00002b10: 696e 7a80 0a20 2020 204d 696e 6943 6861  inz..    MiniCha
-00002b20: 696e 2073 6573 7369 6f6e 206f 626a 6563  in session objec
-00002b30: 7420 7769 7468 2062 6163 6b65 6e64 732e  t with backends.
-00002b40: 204d 616b 6520 6261 636b 656e 6420 6279   Make backend by
-00002b50: 2063 616c 6c69 6e67 0a20 2020 2060 6d69   calling.    `mi
-00002b60: 6e69 6368 6169 6e2e 4f70 656e 4149 2829  nichain.OpenAI()
-00002b70: 6020 7769 7468 2061 7267 7320 666f 7220  ` with args for 
-00002b80: 604f 7065 6e41 4960 2063 6c61 7373 2e0a  `OpenAI` class..
-00002b90: 2020 2020 729c 0000 0063 0200 0000 0000      r....c......
-00002ba0: 0000 0000 0000 0200 0000 0400 0000 4300  ..............C.
-00002bb0: 0000 731e 0000 0074 0074 017c 019b 0064  ..s....t.t.|...d
-00002bc0: 019d 0264 0283 0283 0101 007c 017c 005f  ...d.......|.|._
-00002bd0: 0264 0053 0072 cb00 0000 2903 720c 0000  .d.S.r....).r...
-00002be0: 0072 cd00 0000 729c 0000 0029 0272 1c00  .r....r....).r..
-00002bf0: 0000 729c 0000 0072 1500 0000 7215 0000  ..r....r....r...
-00002c00: 0072 1600 0000 7231 0000 0045 0100 0073  .r....r1...E...s
-00002c10: 0400 0000 1401 0a01 7a12 4d69 6e69 4368  ........z.MiniCh
-00002c20: 6169 6e2e 5f5f 696e 6974 5f5f 721f 0000  ain.__init__r...
-00002c30: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
-00002c40: 0000 0300 0000 4300 0000 7326 0000 0069  ......C...s&...i
-00002c50: 0074 005f 0169 0074 005f 027c 006a 0374  .t._.i.t._.|.j.t
-00002c60: 005f 0374 047c 006a 0364 018d 017c 005f  ._.t.|.j.d...|._
-00002c70: 057c 0053 0029 024e 2901 da0b 6163 7469  .|.S.).N)...acti
-00002c80: 6f6e 5f74 7970 6529 0672 9b00 0000 72c9  on_type).r....r.
-00002c90: 0000 0072 ca00 0000 729c 0000 0072 0b00  ...r....r....r..
-00002ca0: 0000 da06 6163 7469 6f6e 721b 0000 0072  ....actionr....r
-00002cb0: 1500 0000 7215 0000 0072 1600 0000 da09  ....r....r......
-00002cc0: 5f5f 656e 7465 725f 5f49 0100 0073 0a00  __enter__I...s..
-00002cd0: 0000 0601 0601 0801 0e01 0401 7a13 4d69  ............z.Mi
-00002ce0: 6e69 4368 6169 6e2e 5f5f 656e 7465 725f  niChain.__enter_
-00002cf0: 5fda 0474 7970 65da 0965 7863 6570 7469  _..type..excepti
-00002d00: 6f6e da09 7472 6163 6562 6163 6b4e 6304  on..tracebackNc.
-00002d10: 0000 0000 0000 0000 0000 0004 0000 0002  ................
-00002d20: 0000 0043 0000 0073 2c00 0000 7c00 6a00  ...C...s,...|.j.
-00002d30: a001 a100 0100 7402 7403 6a04 8301 7c00  ......t.t.j...|.
-00002d40: 5f04 6900 7403 5f04 6900 7403 5f05 6401  _.i.t._.i.t._.d.
-00002d50: 7403 5f06 6400 5300 7219 0000 0029 0772  t._.d.S.r....).r
-00002d60: d200 0000 da06 6669 6e69 7368 7281 0000  ......finishr...
-00002d70: 0072 9b00 0000 72c9 0000 0072 ca00 0000  .r....r....r....
-00002d80: 729c 0000 0029 0472 1c00 0000 72d4 0000  r....).r....r...
-00002d90: 0072 d500 0000 72d6 0000 0072 1500 0000  .r....r....r....
-00002da0: 7215 0000 0072 1600 0000 da08 5f5f 6578  r....r......__ex
-00002db0: 6974 5f5f 5001 0000 730a 0000 000a 060c  it__P...s.......
-00002dc0: 0106 0106 010a 017a 124d 696e 6943 6861  .......z.MiniCha
-00002dd0: 696e 2e5f 5f65 7869 745f 5f29 0272 1f00  in.__exit__).r..
-00002de0: 0000 72d0 0000 0029 0c72 1000 0000 7211  ..r....).r....r.
-00002df0: 0000 0072 1200 0000 726a 0000 0072 1300  ...r....rj...r..
-00002e00: 0000 7231 0000 0072 d300 0000 72d4 0000  ..r1...r....r...
-00002e10: 0072 0800 0000 da0d 4261 7365 4578 6365  .r......BaseExce
-00002e20: 7074 696f 6e72 0300 0000 72d8 0000 0072  ptionr....r....r
-00002e30: 1500 0000 7215 0000 0072 1500 0000 7216  ....r....r....r.
-00002e40: 0000 0072 d000 0000 3f01 0000 731a 0000  ...r....?...s...
-00002e50: 0008 0004 010e 050a 0402 0702 0202 fe06  ................
-00002e60: 0302 fd06 0402 fc02 050e fb72 d000 0000  ...........r....
-00002e70: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00002e80: 0002 0000 0043 0000 0073 0800 0000 7400  .....C...s....t.
-00002e90: 7c00 8301 5300 2901 7a65 0a20 2020 2049  |...S.).ze.    I
-00002ea0: 6e69 7469 616c 697a 6520 6120 6368 6169  nitialize a chai
-00002eb0: 6e2e 204c 6f67 7320 746f 207b 6e61 6d65  n. Logs to {name
-00002ec0: 7d2e 6c6f 672e 2052 6574 7572 6e73 2061  }.log. Returns a
-00002ed0: 2060 4d69 6e69 4368 6169 6e60 2074 6861   `MiniChain` tha
-00002ee0: 740a 2020 2020 686f 6c64 7320 4c4c 4d20  t.    holds LLM 
-00002ef0: 6261 636b 656e 6473 2e2e 0a20 2020 2029  backends...    )
-00002f00: 0172 d000 0000 72ce 0000 0072 1500 0000  .r....r....r....
-00002f10: 7215 0000 0072 1600 0000 da0b 7374 6172  r....r......star
-00002f20: 745f 6368 6169 6e5d 0100 0073 0200 0000  t_chain]...s....
-00002f30: 0805 72da 0000 0029 2772 5000 0000 7272  ..r....)'rP...rr
-00002f40: 0000 0072 3500 0000 da0b 6461 7461 636c  ...r5.....datacl
-00002f50: 6173 7365 7372 0200 0000 da05 7479 7065  assesr......type
-00002f60: 7372 0300 0000 da06 7479 7069 6e67 7204  sr......typingr.
-00002f70: 0000 0072 0500 0000 7206 0000 0072 0700  ...r....r....r..
-00002f80: 0000 7208 0000 0072 0900 0000 720a 0000  ..r....r....r...
-00002f90: 00da 0565 6c69 6f74 720b 0000 0072 0c00  ...eliotr....r..
-00002fa0: 0000 7299 0000 0072 0d00 0000 7217 0000  ..r....r....r...
-00002fb0: 0072 2900 0000 722c 0000 0072 3d00 0000  .r)...r,...r=...
-00002fc0: 725a 0000 0072 6b00 0000 727a 0000 0072  rZ...rk...rz...r
-00002fd0: 8500 0000 7293 0000 0072 a400 0000 72b0  ....r....r....r.
-00002fe0: 0000 0072 b200 0000 72c4 0000 0072 9a00  ...r....r....r..
-00002ff0: 0000 729b 0000 0072 1300 0000 72cf 0000  ..r....r....r...
-00003000: 0072 d000 0000 72da 0000 0072 1500 0000  .r....r....r....
-00003010: 7215 0000 0072 1500 0000 7216 0000 00da  r....r....r.....
-00003020: 083c 6d6f 6475 6c65 3e01 0000 0073 3a00  .<module>....s:.
-00003030: 0000 0800 0801 0801 0c01 0c01 2401 1002  ............$...
-00003040: 0402 0801 0203 1001 0e05 100e 1005 1014  ................
-00003050: 102c 1016 101e 0e12 101a 1025 1014 1005  .,.........%....
-00003060: 100f 100f 0e11 1207 0e04 161e            ............
+00000080: 0100 6400 6401 6c0f 5a10 6400 6405 6c11  ..d.d.l.Z.d.d.l.
+00000090: 6d12 5a12 6d13 5a13 0100 6508 723c 6400  m.Z.m.Z...e.r<d.
+000000a0: 6401 6c14 5a14 4700 6406 6407 8400 6407  d.l.Z.G.d.d...d.
+000000b0: 8302 5a15 4700 6408 6409 8400 6409 6515  ..Z.G.d.d...d.e.
+000000c0: 8303 5a16 4700 640a 640b 8400 640b 6515  ..Z.G.d.d...d.e.
+000000d0: 8303 5a17 4700 640c 640d 8400 640d 6515  ..Z.G.d.d...d.e.
+000000e0: 8303 5a18 4700 640e 640f 8400 640f 6515  ..Z.G.d.d...d.e.
+000000f0: 8303 5a19 4700 6410 6411 8400 6411 6515  ..Z.G.d.d...d.e.
+00000100: 8303 5a1a 4700 6412 6413 8400 6413 6515  ..Z.G.d.d...d.e.
+00000110: 8303 5a1b 4700 6414 6415 8400 6415 651b  ..Z.G.d.d...d.e.
+00000120: 8303 5a1c 4700 6416 6417 8400 6417 651b  ..Z.G.d.d...d.e.
+00000130: 8303 5a1d 4700 6418 6419 8400 6419 6515  ..Z.G.d.d...d.e.
+00000140: 8303 5a1e 4700 641a 641b 8400 641b 651e  ..Z.G.d.d...d.e.
+00000150: 8303 5a1f 4700 641c 641d 8400 641d 651e  ..Z.G.d.d...d.e.
+00000160: 8303 5a20 4700 641e 641f 8400 641f 6515  ..Z G.d.d...d.e.
+00000170: 8303 5a21 6504 4700 6420 6421 8400 6421  ..Z!e.G.d d!..d!
+00000180: 8302 8301 5a22 6504 4700 6422 6423 8400  ....Z"e.G.d"d#..
+00000190: 6423 8302 8301 5a23 4700 6424 6425 8400  d#....Z#G.d$d%..
+000001a0: 6425 8302 5a24 6426 6525 6427 6401 6604  d%..Z$d&e%d'd.f.
+000001b0: 6428 6429 8404 5a26 4700 642a 642b 8400  d(d)..Z&G.d*d+..
+000001c0: 642b 8302 5a27 6426 6525 6427 6527 6604  d+..Z'd&e%d'e'f.
+000001d0: 642c 642d 8404 5a28 6401 5300 292e e900  d,d-..Z(d.S.)...
+000001e0: 0000 004e 2901 da09 6461 7461 636c 6173  ...N)...dataclas
+000001f0: 7329 01da 0d54 7261 6365 6261 636b 5479  s)...TracebackTy
+00000200: 7065 2907 da0d 5459 5045 5f43 4845 434b  pe)...TYPE_CHECK
+00000210: 494e 47da 0341 6e79 da04 4469 6374 da08  ING..Any..Dict..
+00000220: 4974 6572 6174 6f72 da04 4c69 7374 da08  Iterator..List..
+00000230: 4f70 7469 6f6e 616c da05 5475 706c 6529  Optional..Tuple)
+00000240: 02da 0c73 7461 7274 5f61 6374 696f 6eda  ...start_action.
+00000250: 0774 6f5f 6669 6c65 6300 0000 0000 0000  .to_filec.......
+00000260: 0000 0000 0000 0000 0005 0000 0040 0000  .............@..
+00000270: 0073 7800 0000 6500 5a01 6400 5a02 6503  .sx...e.Z.d.Z.e.
+00000280: 6401 6504 6602 6402 6403 8404 8301 5a05  d.e.f.d.d.....Z.
+00000290: 6404 6504 6401 6504 6604 6405 6406 8404  d.e.d.e.f.d.d...
+000002a0: 5a06 6404 6504 6401 6507 6504 1900 6604  Z.d.e.d.e.e...f.
+000002b0: 6407 6408 8404 5a08 6404 6504 6401 6504  d.d...Z.d.e.d.e.
+000002c0: 6604 6409 640a 8404 5a09 6401 650a 6a0b  f.d.d...Z.d.e.j.
+000002d0: 6602 640b 640c 8404 5a0c 6401 650a 6a0b  f.d.d...Z.d.e.j.
+000002e0: 6602 640d 640e 8404 5a0d 640f 5300 2910  f.d.d...Z.d.S.).
+000002f0: da07 4261 636b 656e 64da 0672 6574 7572  ..Backend..retur
+00000300: 6e63 0100 0000 0000 0000 0000 0000 0100  nc..............
+00000310: 0000 0100 0000 4300 0000 f304 0000 0064  ......C........d
+00000320: 0153 00a9 024e da00 a900 a901 da04 7365  .S...N........se
+00000330: 6c66 7212 0000 0072 1200 0000 fa55 2f68  lfr....r.....U/h
+00000340: 6f6d 652f 7372 7573 682f 5072 6f6a 6563  ome/srush/Projec
+00000350: 7473 2f4d 696e 6943 6861 696e 2f76 656e  ts/MiniChain/ven
+00000360: 762f 6c69 622f 7079 7468 6f6e 332e 3130  v/lib/python3.10
+00000370: 2f73 6974 652d 7061 636b 6167 6573 2f6d  /site-packages/m
+00000380: 696e 6963 6861 696e 2f62 6163 6b65 6e64  inichain/backend
+00000390: 2e70 79da 0b64 6573 6372 6970 7469 6f6e  .py..description
+000003a0: 1000 0000 7302 0000 0004 027a 1342 6163  ....s......z.Bac
+000003b0: 6b65 6e64 2e64 6573 6372 6970 7469 6f6e  kend.description
+000003c0: da07 7265 7175 6573 7463 0200 0000 0000  ..requestc......
+000003d0: 0000 0000 0000 0200 0000 0100 0000 4300  ..............C.
+000003e0: 0000 f304 0000 0074 0082 01a9 014e a901  .......t.....N..
+000003f0: da13 4e6f 7449 6d70 6c65 6d65 6e74 6564  ..NotImplemented
+00000400: 4572 726f 72a9 0272 1400 0000 7217 0000  Error..r....r...
+00000410: 0072 1200 0000 7212 0000 0072 1500 0000  .r....r....r....
+00000420: da03 7275 6e14 0000 00f3 0200 0000 0401  ..run...........
+00000430: 7a0b 4261 636b 656e 642e 7275 6e63 0200  z.Backend.runc..
+00000440: 0000 0000 0000 0000 0000 0200 0000 0100  ................
+00000450: 0000 4300 0000 7218 0000 0072 1900 0000  ..C...r....r....
+00000460: 721a 0000 0072 1c00 0000 7212 0000 0072  r....r....r....r
+00000470: 1200 0000 7215 0000 00da 0a72 756e 5f73  ....r......run_s
+00000480: 7472 6561 6d17 0000 0072 1e00 0000 7a12  tream....r....z.
+00000490: 4261 636b 656e 642e 7275 6e5f 7374 7265  Backend.run_stre
+000004a0: 616d 6302 0000 0000 0000 0000 0000 0002  amc.............
+000004b0: 0000 0003 0000 00c3 0000 0073 0c00 0000  ...........s....
+000004c0: 8101 7c00 a000 7c01 a101 5300 7219 0000  ..|...|...S.r...
+000004d0: 0029 0172 1d00 0000 721c 0000 0072 1200  .).r....r....r..
+000004e0: 0000 7212 0000 0072 1500 0000 da04 6172  ..r....r......ar
+000004f0: 756e 1a00 0000 7304 0000 0002 800a 017a  un....s........z
+00000500: 0c42 6163 6b65 6e64 2e61 7275 6e63 0100  .Backend.arunc..
+00000510: 0000 0000 0000 0000 0000 0100 0000 0300  ................
+00000520: 0000 4300 0000 f30c 0000 0074 006a 0164  ..C........t.j.d
+00000530: 0164 028d 0153 00a9 034e 4629 01da 0a73  .d...S...NF)...s
+00000540: 686f 775f 6c61 6265 6ca9 02da 0267 72da  how_label....gr.
+00000550: 0754 6578 7462 6f78 7213 0000 0072 1200  .Textboxr....r..
+00000560: 0000 7212 0000 0072 1500 0000 da0b 626c  ..r....r......bl
+00000570: 6f63 6b5f 696e 7075 741d 0000 00f3 0200  ock_input.......
+00000580: 0000 0c01 7a13 4261 636b 656e 642e 626c  ....z.Backend.bl
+00000590: 6f63 6b5f 696e 7075 7463 0100 0000 0000  ock_inputc......
+000005a0: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
+000005b0: 0000 7221 0000 0072 2200 0000 7224 0000  ..r!...r"...r$..
+000005c0: 0072 1300 0000 7212 0000 0072 1200 0000  .r....r....r....
+000005d0: 7215 0000 00da 0c62 6c6f 636b 5f6f 7574  r......block_out
+000005e0: 7075 7420 0000 0072 2800 0000 7a14 4261  put ...r(...z.Ba
+000005f0: 636b 656e 642e 626c 6f63 6b5f 6f75 7470  ckend.block_outp
+00000600: 7574 4e29 0eda 085f 5f6e 616d 655f 5fda  utN)...__name__.
+00000610: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+00000620: 7561 6c6e 616d 655f 5fda 0870 726f 7065  ualname__..prope
+00000630: 7274 79da 0373 7472 7216 0000 0072 1d00  rty..strr....r..
+00000640: 0000 7207 0000 0072 1f00 0000 7220 0000  ..r....r....r ..
+00000650: 0072 2500 0000 da06 426c 6f63 6b73 7227  .r%.....Blocksr'
+00000660: 0000 0072 2900 0000 7212 0000 0072 1200  ...r)...r....r..
+00000670: 0000 7212 0000 0072 1500 0000 720d 0000  ..r....r....r...
+00000680: 000f 0000 0073 1000 0000 0800 0201 1001  .....s..........
+00000690: 1203 1603 1203 1003 1403 720d 0000 0063  ..........r....c
+000006a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000006b0: 0400 0000 4000 0000 f31e 0000 0065 005a  ....@........e.Z
+000006c0: 0164 005a 0264 0165 0364 0265 0366 0464  .d.Z.d.e.d.e.f.d
+000006d0: 0364 0484 045a 0464 0553 0029 06da 0249  .d...Z.d.S.)...I
+000006e0: 6472 1700 0000 720e 0000 0063 0200 0000  dr....r....c....
+000006f0: 0000 0000 0000 0000 0200 0000 0100 0000  ................
+00000700: 4300 0000 7304 0000 007c 0153 0072 1900  C...s....|.S.r..
+00000710: 0000 7212 0000 0072 1c00 0000 7212 0000  ..r....r....r...
+00000720: 0072 1200 0000 7215 0000 0072 1d00 0000  .r....r....r....
+00000730: 2500 0000 721e 0000 007a 0649 642e 7275  %...r....z.Id.ru
+00000740: 6e4e a905 722a 0000 0072 2b00 0000 722c  nN..r*...r+...r,
+00000750: 0000 0072 2e00 0000 721d 0000 0072 1200  ...r....r....r..
+00000760: 0000 7212 0000 0072 1200 0000 7215 0000  ..r....r....r...
+00000770: 0072 3100 0000 2400 0000 f304 0000 0008  .r1...$.........
+00000780: 0016 0172 3100 0000 6300 0000 0000 0000  ...r1...c.......
+00000790: 0000 0000 0000 0000 0005 0000 0040 0000  .............@..
+000007a0: 0073 5800 0000 6500 5a01 6400 5a02 6700  .sX...e.Z.d.Z.g.
+000007b0: 6601 6401 6503 6504 1900 6602 6402 6403  f.d.e.e...f.d.d.
+000007c0: 8405 5a05 6404 6504 6405 6504 6604 6406  ..Z.d.e.d.e.f.d.
+000007d0: 6407 8404 5a06 6404 6504 6405 6507 6504  d...Z.d.e.d.e.e.
+000007e0: 1900 6604 6408 6409 8404 5a08 6405 6504  ..f.d.d...Z.d.e.
+000007f0: 6602 640a 640b 8404 5a09 640c 5300 290d  f.d.d...Z.d.S.).
+00000800: da04 4d6f 636b da07 616e 7377 6572 7363  ..Mock..answersc
+00000810: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00000820: 0200 0000 4300 0000 7310 0000 0064 017c  ....C...s....d.|
+00000830: 005f 007c 017c 005f 0164 0053 0029 024e  ._.|.|._.d.S.).N
+00000840: e9ff ffff ff29 02da 0169 7235 0000 0029  .....)...ir5...)
+00000850: 0272 1400 0000 7235 0000 0072 1200 0000  .r....r5...r....
+00000860: 7212 0000 0072 1500 0000 da08 5f5f 696e  r....r......__in
+00000870: 6974 5f5f 2a00 0000 7304 0000 0006 010a  it__*...s.......
+00000880: 017a 0d4d 6f63 6b2e 5f5f 696e 6974 5f5f  .z.Mock.__init__
+00000890: 7217 0000 0072 0e00 0000 6302 0000 0000  r....r....c.....
+000008a0: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
+000008b0: 0000 0073 2400 0000 7c00 0400 6a00 6401  ...s$...|...j.d.
+000008c0: 3700 0200 5f00 7c00 6a01 7c00 6a00 7402  7..._.|.j.|.j.t.
+000008d0: 7c00 6a01 8301 1600 1900 5300 2902 4ee9  |.j.......S.).N.
+000008e0: 0100 0000 2903 7237 0000 0072 3500 0000  ....).r7...r5...
+000008f0: da03 6c65 6e72 1c00 0000 7212 0000 0072  ..lenr....r....r
+00000900: 1200 0000 7215 0000 0072 1d00 0000 2e00  ....r....r......
+00000910: 0000 7304 0000 000e 0116 017a 084d 6f63  ..s........z.Moc
+00000920: 6b2e 7275 6e63 0200 0000 0000 0000 0000  k.runc..........
+00000930: 0000 0400 0000 0400 0000 6300 0000 7344  ..........c...sD
+00000940: 0000 0081 007c 0004 006a 0064 0137 0002  .....|...j.d.7..
+00000950: 005f 007c 006a 017c 006a 0074 027c 006a  ._.|.j.|.j.t.|.j
+00000960: 0183 0116 0019 007d 027c 0244 005d 0a7d  .......}.|.D.].}
+00000970: 037c 0356 0001 0074 03a0 0464 02a1 0101  .|.V...t...d....
+00000980: 0071 1564 0053 0029 034e 7239 0000 0067  .q.d.S.).Nr9...g
+00000990: 9a99 9999 9999 b93f 2905 7237 0000 0072  .......?).r7...r
+000009a0: 3500 0000 723a 0000 00da 0474 696d 65da  5...r:.....time.
+000009b0: 0573 6c65 6570 2904 7214 0000 0072 1700  .sleep).r....r..
+000009c0: 0000 da06 7265 7375 6c74 da01 6372 1200  ....result..cr..
+000009d0: 0000 7212 0000 0072 1500 0000 721f 0000  ..r....r....r...
+000009e0: 0032 0000 0073 0e00 0000 0280 0e01 1601  .2...s..........
+000009f0: 0801 0601 0c01 04fe 7a0f 4d6f 636b 2e72  ........z.Mock.r
+00000a00: 756e 5f73 7472 6561 6d63 0100 0000 0000  un_streamc......
+00000a10: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
+00000a20: 0000 f30c 0000 0064 017c 006a 009b 009d  .......d.|.j....
+00000a30: 0253 0029 024e 7a0f 4d6f 636b 6564 2042  .S.).Nz.Mocked B
+00000a40: 6163 6b65 6e64 2029 0172 3500 0000 7213  ackend ).r5...r.
+00000a50: 0000 0072 1200 0000 7212 0000 0072 1500  ...r....r....r..
+00000a60: 0000 da08 5f5f 7265 7072 5f5f 3900 0000  ....__repr__9...
+00000a70: 7228 0000 007a 0d4d 6f63 6b2e 5f5f 7265  r(...z.Mock.__re
+00000a80: 7072 5f5f 4e29 0a72 2a00 0000 722b 0000  pr__N).r*...r+..
+00000a90: 0072 2c00 0000 7208 0000 0072 2e00 0000  .r,...r....r....
+00000aa0: 7238 0000 0072 1d00 0000 7207 0000 0072  r8...r....r....r
+00000ab0: 1f00 0000 7240 0000 0072 1200 0000 7212  ....r@...r....r.
+00000ac0: 0000 0072 1200 0000 7215 0000 0072 3400  ...r....r....r4.
+00000ad0: 0000 2900 0000 730a 0000 0008 0016 0112  ..)...s.........
+00000ae0: 0416 0412 0772 3400 0000 6300 0000 0000  .....r4...c.....
+00000af0: 0000 0000 0000 0000 0000 0004 0000 0040  ...............@
+00000b00: 0000 0073 3600 0000 6500 5a01 6400 5a02  ...s6...e.Z.d.Z.
+00000b10: 640a 6403 6404 8404 5a03 6405 6504 6401  d.d.d...Z.d.e.d.
+00000b20: 6504 6604 6406 6407 8404 5a05 6401 6504  e.f.d.d...Z.d.e.
+00000b30: 6602 6408 6409 8404 5a06 6402 5300 290b  f.d.d...Z.d.S.).
+00000b40: da06 476f 6f67 6c65 720e 0000 004e 6301  ..Googler....Nc.
+00000b50: 0000 0000 0000 0000 0000 0001 0000 0001  ................
+00000b60: 0000 0043 0000 0073 0400 0000 6400 5300  ...C...s....d.S.
+00000b70: 7219 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
+00000b80: 1200 0000 7212 0000 0072 1500 0000 7238  ....r....r....r8
+00000b90: 0000 003e 0000 0072 1e00 0000 7a0f 476f  ...>...r....z.Go
+00000ba0: 6f67 6c65 2e5f 5f69 6e69 745f 5f72 1700  ogle.__init__r..
+00000bb0: 0000 6302 0000 0000 0000 0000 0000 0008  ..c.............
+00000bc0: 0000 0007 0000 0043 0000 0073 1a01 0000  .......C...s....
+00000bd0: 6401 6402 6c00 6d01 7d02 0100 7402 6a03  d.d.l.m.}...t.j.
+00000be0: a004 6403 a101 7d03 7c03 7312 4a00 6404  ..d...}.|.s.J.d.
+00000bf0: 8301 8201 7c03 7c00 5f05 7c00 6a05 6405  ....|.|._.|.j.d.
+00000c00: 7c01 6406 6407 6408 6409 9c06 7d04 7c02  |.d.d.d.d...}.|.
+00000c10: 7c04 8301 7d05 7c05 a006 a100 7d06 640a  |...}.|.....}.d.
+00000c20: 7c06 a007 a100 7600 723f 640b 7c06 640a  |.....v.r?d.|.d.
+00000c30: 1900 a007 a100 7600 723f 7c06 640a 1900  ......v.r?|.d...
+00000c40: 640b 1900 7d07 7408 7c07 8301 5300 640a  d...}.t.|...S.d.
+00000c50: 7c06 a007 a100 7600 7257 640c 7c06 640a  |.....v.rWd.|.d.
+00000c60: 1900 a007 a100 7600 7257 7c06 640a 1900  ......v.rW|.d...
+00000c70: 640c 1900 7d07 7408 7c07 8301 5300 640a  d...}.t.|...S.d.
+00000c80: 7c06 a007 a100 7600 7271 640d 7c06 640a  |.....v.rqd.|.d.
+00000c90: 1900 a007 a100 7600 7271 7c06 640a 1900  ......v.rq|.d...
+00000ca0: 640d 1900 6401 1900 7d07 7408 7c07 8301  d...d...}.t.|...
+00000cb0: 5300 640c 7c06 640e 1900 6401 1900 a007  S.d.|.d...d.....
+00000cc0: a100 7600 7287 7c06 640e 1900 6401 1900  ..v.r.|.d...d...
+00000cd0: 640c 1900 7d07 7408 7c07 8301 5300 640f  d...}.t.|...S.d.
+00000ce0: 7d07 7408 7c07 8301 5300 2910 4e72 0100  }.t.|...S.).Nr..
+00000cf0: 0000 2901 da0c 476f 6f67 6c65 5365 6172  ..)...GoogleSear
+00000d00: 6368 da08 5345 5250 5f4b 4559 7a3f 4e65  ch..SERP_KEYz?Ne
+00000d10: 6564 2061 2053 4552 505f 4b45 592e 2047  ed a SERP_KEY. G
+00000d20: 6574 206f 6e65 2068 6572 6520 6874 7470  et one here http
+00000d30: 733a 2f2f 7365 7270 6170 692e 636f 6d2f  s://serpapi.com/
+00000d40: 7573 6572 732f 7765 6c63 6f6d 65da 0667  users/welcome..g
+00000d50: 6f6f 676c 657a 0a67 6f6f 676c 652e 636f  ooglez.google.co
+00000d60: 6dda 0275 73da 0265 6e29 06da 0761 7069  m..us..en)...api
+00000d70: 5f6b 6579 da06 656e 6769 6e65 da01 71da  _key..engine..q.
+00000d80: 0d67 6f6f 676c 655f 646f 6d61 696e da02  .google_domain..
+00000d90: 676c da02 686c da0a 616e 7377 6572 5f62  gl..hl..answer_b
+00000da0: 6f78 da06 616e 7377 6572 da07 736e 6970  ox..answer..snip
+00000db0: 7065 74da 1973 6e69 7070 6574 5f68 6967  pet..snippet_hig
+00000dc0: 686c 6967 6874 6564 5f77 6f72 6473 da0f  hlighted_words..
+00000dd0: 6f72 6761 6e69 635f 7265 7375 6c74 7372  organic_resultsr
+00000de0: 1100 0000 2909 da07 7365 7270 6170 6972  ....)...serpapir
+00000df0: 4200 0000 da02 6f73 da07 656e 7669 726f  B.....os..enviro
+00000e00: 6eda 0367 6574 da0b 7365 7270 6170 695f  n..get..serpapi_
+00000e10: 6b65 79da 0867 6574 5f64 6963 74da 046b  key..get_dict..k
+00000e20: 6579 7372 2e00 0000 2908 7214 0000 0072  eysr....).r....r
+00000e30: 1700 0000 7242 0000 0072 5600 0000 da06  ....rB...rV.....
+00000e40: 7061 7261 6d73 da06 7365 6172 6368 da03  params..search..
+00000e50: 7265 73da 0574 6f72 6574 7212 0000 0072  res..toretr....r
+00000e60: 1200 0000 7215 0000 0072 1d00 0000 4100  ....r....r....A.
+00000e70: 0000 7342 0000 000c 010c 0202 0204 ff02  ..sB............
+00000e80: 0204 fe06 0304 0302 0102 0102 0102 0102  ................
+00000e90: 0106 fa08 0908 011c 020c 0108 0c1c f50c  ................
+00000ea0: 0108 0a0a f802 ff0e 0202 fe10 0408 0514  ................
+00000eb0: fc10 0108 0304 ff08 017a 0a47 6f6f 676c  .........z.Googl
+00000ec0: 652e 7275 6e63 0100 0000 0000 0000 0000  e.runc..........
+00000ed0: 0000 0100 0000 0100 0000 4300 0000 720f  ..........C...r.
+00000ee0: 0000 0029 024e 7a15 476f 6f67 6c65 2053  ...).Nz.Google S
+00000ef0: 6561 7263 6820 4261 636b 656e 6472 1200  earch Backendr..
+00000f00: 0000 7213 0000 0072 1200 0000 7212 0000  ..r....r....r...
+00000f10: 0072 1500 0000 7240 0000 0065 0000 0072  .r....r@...e...r
+00000f20: 1e00 0000 7a0f 476f 6f67 6c65 2e5f 5f72  ....z.Google.__r
+00000f30: 6570 725f 5f29 0272 0e00 0000 4e29 0772  epr__).r....N).r
+00000f40: 2a00 0000 722b 0000 0072 2c00 0000 7238  *...r+...r,...r8
+00000f50: 0000 0072 2e00 0000 721d 0000 0072 4000  ...r....r....r@.
+00000f60: 0000 7212 0000 0072 1200 0000 7212 0000  ..r....r....r...
+00000f70: 0072 1500 0000 7241 0000 003d 0000 0073  .r....rA...=...s
+00000f80: 0800 0000 0800 0a01 1203 1224 7241 0000  ...........$rA..
+00000f90: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00000fa0: 0000 0400 0000 4000 0000 7350 0000 0065  ......@...sP...e
+00000fb0: 005a 0164 005a 0264 015a 0364 0265 046a  .Z.d.Z.d.Z.d.e.j
+00000fc0: 0566 0264 0364 0484 045a 0664 0265 046a  .f.d.d...Z.d.e.j
+00000fd0: 0566 0264 0564 0684 045a 0764 0765 0864  .f.d.d...Z.d.e.d
+00000fe0: 0265 0866 0464 0864 0984 045a 0964 0265  .e.f.d.d...Z.d.e
+00000ff0: 0866 0264 0a64 0b84 045a 0a64 0c53 0029  .f.d.d...Z.d.S.)
+00001000: 0dda 0650 7974 686f 6e7a 3045 7865 6375  ...Pythonz0Execu
+00001010: 7465 7320 5079 7468 6f6e 2063 6f6d 6d61  tes Python comma
+00001020: 6e64 7320 616e 6420 7265 7475 726e 7320  nds and returns 
+00001030: 7468 6520 6f75 7470 7574 2e72 0e00 0000  the output.r....
+00001040: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00001050: 0002 0000 0043 0000 00f3 0800 0000 7400  .....C........t.
+00001060: a001 a100 5300 7219 0000 00a9 0272 2500  ....S.r......r%.
+00001070: 0000 da04 436f 6465 7213 0000 0072 1200  ....Coder....r..
+00001080: 0000 7212 0000 0072 1500 0000 7227 0000  ..r....r....r'..
+00001090: 006c 0000 00f3 0200 0000 0801 7a12 5079  .l..........z.Py
+000010a0: 7468 6f6e 2e62 6c6f 636b 5f69 6e70 7574  thon.block_input
+000010b0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+000010c0: 0002 0000 0043 0000 0072 5e00 0000 7219  .....C...r^...r.
+000010d0: 0000 0072 5f00 0000 7213 0000 0072 1200  ...r_...r....r..
+000010e0: 0000 7212 0000 0072 1500 0000 7229 0000  ..r....r....r)..
+000010f0: 006f 0000 0072 6100 0000 7a13 5079 7468  .o...ra...z.Pyth
+00001100: 6f6e 2e62 6c6f 636b 5f6f 7574 7075 7472  on.block_outputr
+00001110: 1700 0000 6302 0000 0000 0000 0000 0000  ....c...........
+00001120: 0007 0000 0008 0000 0043 0000 0073 8800  .........C...s..
+00001130: 0000 6401 6402 6c00 6d01 7d02 0100 6401  ..d.d.l.m.}...d.
+00001140: 6403 6c02 6d03 7d03 0100 7c01 a004 a100  d.l.m.}...|.....
+00001150: 7d04 7c04 a005 6404 a101 7223 6405 a006  }.|...d...r#d...
+00001160: 7c04 a004 a100 a007 6405 a101 6406 6407  |.......d...d.d.
+00001170: 8502 1900 a101 7d04 7c03 8300 7d05 7c02  ......}.|...}.|.
+00001180: 7c05 8301 8f0c 0100 7408 7c04 8301 0100  |.......t.|.....
+00001190: 5700 6408 0400 0400 8303 0100 6e08 3100  W.d.........n.1.
+000011a0: 7339 7701 0100 0100 0100 5900 0100 7c05  s9w.......Y...|.
+000011b0: a009 a100 7d06 7c06 5300 2909 fa25 5275  ....}.|.S.)..%Ru
+000011c0: 6e20 636f 6d6d 616e 6473 2061 6e64 2072  n commands and r
+000011d0: 6574 7572 6e20 6669 6e61 6c20 6f75 7470  eturn final outp
+000011e0: 7574 2e72 0100 0000 2901 da0f 7265 6469  ut.r....)...redi
+000011f0: 7265 6374 5f73 7464 6f75 7429 01da 0853  rect_stdout)...S
+00001200: 7472 696e 6749 4f7a 0360 6060 da01 0a72  tringIOz.```...r
+00001210: 3900 0000 7236 0000 004e 290a da0a 636f  9...r6...N)...co
+00001220: 6e74 6578 746c 6962 7263 0000 00da 0269  ntextlibrc.....i
+00001230: 6f72 6400 0000 da05 7374 7269 70da 0a73  ord.....strip..s
+00001240: 7461 7274 7377 6974 68da 046a 6f69 6eda  tartswith..join.
+00001250: 0573 706c 6974 da04 6578 6563 da08 6765  .split..exec..ge
+00001260: 7476 616c 7565 2907 7214 0000 0072 1700  tvalue).r....r..
+00001270: 0000 7263 0000 0072 6400 0000 da01 70da  ..rc...rd.....p.
+00001280: 0166 da01 7372 1200 0000 7212 0000 0072  .f..sr....r....r
+00001290: 1500 0000 721d 0000 0072 0000 0073 1600  ....r....r...s..
+000012a0: 0000 0c02 0c01 0802 0a01 1c01 0602 0a01  ................
+000012b0: 0a01 1cff 0802 0401 7a0a 5079 7468 6f6e  ........z.Python
+000012c0: 2e72 756e 6301 0000 0000 0000 0000 0000  .runc...........
+000012d0: 0001 0000 0001 0000 0043 0000 0072 0f00  .........C...r..
+000012e0: 0000 2902 4e7a 0e50 7974 686f 6e2d 4261  ..).Nz.Python-Ba
+000012f0: 636b 656e 6472 1200 0000 7213 0000 0072  ckendr....r....r
+00001300: 1200 0000 7212 0000 0072 1500 0000 7240  ....r....r....r@
+00001310: 0000 0081 0000 0072 1e00 0000 7a0f 5079  .......r....z.Py
+00001320: 7468 6f6e 2e5f 5f72 6570 725f 5f4e 290b  thon.__repr__N).
+00001330: 722a 0000 0072 2b00 0000 722c 0000 00da  r*...r+...r,....
+00001340: 075f 5f64 6f63 5f5f 7225 0000 0072 2f00  .__doc__r%...r/.
+00001350: 0000 7227 0000 0072 2900 0000 722e 0000  ..r'...r)...r...
+00001360: 0072 1d00 0000 7240 0000 0072 1200 0000  .r....r@...r....
+00001370: 7212 0000 0072 1200 0000 7215 0000 0072  r....r....r....r
+00001380: 5d00 0000 6900 0000 730c 0000 0008 0004  ]...i...s.......
+00001390: 0110 0210 0312 0312 0f72 5d00 0000 6300  .........r]...c.
+000013a0: 0000 0000 0000 0000 0000 0000 0000 0005  ................
+000013b0: 0000 0040 0000 0073 6400 0000 6500 5a01  ...@...sd...e.Z.
+000013c0: 6400 5a02 6401 5a03 6402 6504 6a05 6602  d.Z.d.Z.d.e.j.f.
+000013d0: 6403 6404 8404 5a06 6402 6504 6a05 6602  d.d...Z.d.e.j.f.
+000013e0: 6405 6406 8404 5a07 6412 6408 6508 6409  d.d...Z.d.d.e.d.
+000013f0: 6508 6604 640a 640b 8405 5a09 640c 650a  e.f.d.d...Z.d.e.
+00001400: 6402 650a 6604 640d 640e 8404 5a0b 6402  d.e.f.d.d...Z.d.
+00001410: 650a 6602 640f 6410 8404 5a0c 6411 5300  e.f.d.d...Z.d.S.
+00001420: 2913 da04 4261 7368 7a2e 4578 6563 7574  )...Bashz.Execut
+00001430: 6573 2062 6173 6820 636f 6d6d 616e 6473  es bash commands
+00001440: 2061 6e64 2072 6574 7572 6e73 2074 6865   and returns the
+00001450: 206f 7574 7075 742e 720e 0000 0063 0100   output.r....c..
+00001460: 0000 0000 0000 0000 0000 0100 0000 0200  ................
+00001470: 0000 4300 0000 725e 0000 0072 1900 0000  ..C...r^...r....
+00001480: 725f 0000 0072 1300 0000 7212 0000 0072  r_...r....r....r
+00001490: 1200 0000 7215 0000 0072 2700 0000 8800  ....r....r'.....
+000014a0: 0000 7261 0000 007a 1042 6173 682e 626c  ..ra...z.Bash.bl
+000014b0: 6f63 6b5f 696e 7075 7463 0100 0000 0000  ock_inputc......
+000014c0: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
+000014d0: 0000 725e 0000 0072 1900 0000 725f 0000  ..r^...r....r_..
+000014e0: 0072 1300 0000 7212 0000 0072 1200 0000  .r....r....r....
+000014f0: 7215 0000 0072 2900 0000 8b00 0000 7261  r....r).......ra
+00001500: 0000 007a 1142 6173 682e 626c 6f63 6b5f  ...z.Bash.block_
+00001510: 6f75 7470 7574 46da 0e73 7472 6970 5f6e  outputF..strip_n
+00001520: 6577 6c69 6e65 73da 1172 6574 7572 6e5f  ewlines..return_
+00001530: 6572 725f 6f75 7470 7574 6303 0000 0000  err_outputc.....
+00001540: 0000 0000 0000 0003 0000 0002 0000 0043  ...............C
+00001550: 0000 0073 1000 0000 7c01 7c00 5f00 7c02  ...s....|.|._.|.
+00001560: 7c00 5f01 6401 5300 2902 7a23 496e 6974  |._.d.S.).z#Init
+00001570: 6961 6c69 7a65 2077 6974 6820 7374 7269  ialize with stri
+00001580: 7070 696e 6720 6e65 776c 696e 6573 2e4e  pping newlines.N
+00001590: 2902 7273 0000 0072 7400 0000 2903 7214  ).rs...rt...).r.
+000015a0: 0000 0072 7300 0000 7274 0000 0072 1200  ...rs...rt...r..
+000015b0: 0000 7212 0000 0072 1500 0000 7238 0000  ..r....r....r8..
+000015c0: 008e 0000 0073 0400 0000 0602 0a01 7a0d  .....s........z.
+000015d0: 4261 7368 2e5f 5f69 6e69 745f 5f72 1700  Bash.__init__r..
+000015e0: 0000 6302 0000 0000 0000 0000 0000 0004  ..c.............
+000015f0: 0000 000a 0000 0043 0000 0073 8400 0000  .......C...s....
+00001600: 7a11 7400 6a01 7c01 6401 6401 7400 6a02  z.t.j.|.d.d.t.j.
+00001610: 7400 6a03 6402 8d05 6a04 a005 a100 7d02  t.j.d...j.....}.
+00001620: 5700 6e27 0400 7400 6a06 7938 0100 7d03  W.n'..t.j.y8..}.
+00001630: 0100 7a1a 7c00 6a07 722a 7408 7c03 6a04  ..z.|.j.r*t.|.j.
+00001640: a005 a100 8301 5700 0600 5900 6403 7d03  ......W...Y.d.}.
+00001650: 7e03 5300 7408 7c03 8301 5700 0600 5900  ~.S.t.|...W...Y.
+00001660: 6403 7d03 7e03 5300 6403 7d03 7e03 7701  d.}.~.S.d.}.~.w.
+00001670: 7700 7c00 6a09 7240 7c02 a00a a100 7d02  w.|.j.r@|.....}.
+00001680: 7c02 5300 2904 7262 0000 0054 2904 da05  |.S.).rb...T)...
+00001690: 7368 656c 6cda 0563 6865 636b da06 7374  shell..check..st
+000016a0: 646f 7574 da06 7374 6465 7272 4e29 0bda  dout..stderrN)..
+000016b0: 0a73 7562 7072 6f63 6573 7372 1d00 0000  .subprocessr....
+000016c0: da04 5049 5045 da06 5354 444f 5554 7277  ..PIPE..STDOUTrw
+000016d0: 0000 00da 0664 6563 6f64 65da 1243 616c  .....decode..Cal
+000016e0: 6c65 6450 726f 6365 7373 4572 726f 7272  ledProcessErrorr
+000016f0: 7400 0000 722e 0000 0072 7300 0000 7268  t...r....rs...rh
+00001700: 0000 0029 0472 1400 0000 7217 0000 00da  ...).r....r.....
+00001710: 066f 7574 7075 74da 0565 7272 6f72 7212  .output..errorr.
+00001720: 0000 0072 1200 0000 7215 0000 0072 1d00  ...r....r....r..
+00001730: 0000 9300 0000 7326 0000 0002 0204 0102  ......s&........
+00001740: 0102 0102 0104 0104 0104 fb06 0606 fa10  ................
+00001750: 0706 011a 0114 0108 8002 fd06 0408 0104  ................
+00001760: 017a 0842 6173 682e 7275 6e63 0100 0000  .z.Bash.runc....
+00001770: 0000 0000 0000 0000 0100 0000 0100 0000  ................
+00001780: 4300 0000 720f 0000 0029 024e 7a0c 4261  C...r....).Nz.Ba
+00001790: 7368 2d42 6163 6b65 6e64 7212 0000 0072  sh-Backendr....r
+000017a0: 1300 0000 7212 0000 0072 1200 0000 7215  ....r....r....r.
+000017b0: 0000 0072 4000 0000 a500 0000 721e 0000  ...r@.......r...
+000017c0: 007a 0d42 6173 682e 5f5f 7265 7072 5f5f  .z.Bash.__repr__
+000017d0: 4e29 0246 4629 0d72 2a00 0000 722b 0000  N).FF).r*...r+..
+000017e0: 0072 2c00 0000 7271 0000 0072 2500 0000  .r,...rq...r%...
+000017f0: 722f 0000 0072 2700 0000 7229 0000 00da  r/...r'...r)....
+00001800: 0462 6f6f 6c72 3800 0000 722e 0000 0072  .boolr8...r....r
+00001810: 1d00 0000 7240 0000 0072 1200 0000 7212  ....r@...r....r.
+00001820: 0000 0072 1200 0000 7215 0000 0072 7200  ...r....r....rr.
+00001830: 0000 8500 0000 730e 0000 0008 0004 0110  ......s.........
+00001840: 0210 0314 0312 0512 1272 7200 0000 6300  .........rr...c.
+00001850: 0000 0000 0000 0000 0000 0000 0000 000b  ................
+00001860: 0000 0040 0000 0073 4a00 0000 6500 5a01  ...@...sJ...e.Z.
+00001870: 6400 5a02 0901 0902 0903 0904 640e 6405  d.Z.........d.d.
+00001880: 6503 6406 6504 6407 6505 6408 6506 6507  e.d.e.d.e.d.e.e.
+00001890: 6503 1900 1900 6409 6404 660a 640a 640b  e.....d.d.f.d.d.
+000018a0: 8405 5a08 6409 6503 6602 640c 640d 8404  ..Z.d.e.f.d.d...
+000018b0: 5a09 6404 5300 290f da0a 4f70 656e 4149  Z.d.S.)...OpenAI
+000018c0: 4261 7365 fa0d 6770 742d 332e 352d 7475  Base..gpt-3.5-tu
+000018d0: 7262 6fe9 0001 0000 e700 0000 0000 0000  rbo.............
+000018e0: 004e da05 6d6f 6465 6cda 0a6d 6178 5f74  .N..model..max_t
+000018f0: 6f6b 656e 73da 0b74 656d 7065 7261 7475  okens..temperatu
+00001900: 7265 da04 7374 6f70 720e 0000 0063 0500  re..stopr....c..
+00001910: 0000 0000 0000 0000 0000 0500 0000 0500  ................
+00001920: 0000 4300 0000 7320 0000 007c 017c 005f  ..C...s ...|.|._
+00001930: 007c 047c 005f 0174 027c 017c 027c 0364  .|.|._.t.|.|.|.d
+00001940: 018d 037c 005f 0364 0053 0029 024e 2903  ...|._.d.S.).N).
+00001950: 7285 0000 0072 8600 0000 7287 0000 0029  r....r....r....)
+00001960: 0472 8500 0000 7288 0000 00da 0464 6963  .r....r......dic
+00001970: 74da 076f 7074 696f 6e73 2905 7214 0000  t..options).r...
+00001980: 0072 8500 0000 7286 0000 0072 8700 0000  .r....r....r....
+00001990: 7288 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
+000019a0: 1500 0000 7238 0000 00aa 0000 0073 0e00  ....r8.......s..
+000019b0: 0000 0607 0601 0201 0201 0201 0201 0cfd  ................
+000019c0: 7a13 4f70 656e 4149 4261 7365 2e5f 5f69  z.OpenAIBase.__i
+000019d0: 6e69 745f 5f63 0100 0000 0000 0000 0000  nit__c..........
+000019e0: 0000 0100 0000 0200 0000 4300 0000 723f  ..........C...r?
+000019f0: 0000 0029 024e 7a0f 4f70 656e 4149 2042  ...).Nz.OpenAI B
+00001a00: 6163 6b65 6e64 2029 0172 8a00 0000 7213  ackend ).r....r.
+00001a10: 0000 0072 1200 0000 7212 0000 0072 1500  ...r....r....r..
+00001a20: 0000 7240 0000 00b9 0000 0072 2800 0000  ..r@.......r(...
+00001a30: 7a13 4f70 656e 4149 4261 7365 2e5f 5f72  z.OpenAIBase.__r
+00001a40: 6570 725f 5f29 0472 8200 0000 7283 0000  epr__).r....r...
+00001a50: 0072 8400 0000 4e29 0a72 2a00 0000 722b  .r....N).r*...r+
+00001a60: 0000 0072 2c00 0000 722e 0000 00da 0369  ...r,...r......i
+00001a70: 6e74 da05 666c 6f61 7472 0900 0000 7208  nt..floatr....r.
+00001a80: 0000 0072 3800 0000 7240 0000 0072 1200  ...r8...r@...r..
+00001a90: 0000 7212 0000 0072 1200 0000 7215 0000  ..r....r....r...
+00001aa0: 0072 8100 0000 a900 0000 7322 0000 0008  .r........s"....
+00001ab0: 0002 0302 0102 0102 0104 fb02 0202 fe02  ................
+00001ac0: 0302 fd02 0402 fc0a 0502 fb02 060a fa12  ................
+00001ad0: 0f72 8100 0000 6300 0000 0000 0000 0000  .r....c.........
+00001ae0: 0000 0000 0000 0005 0000 0040 0000 0073  ...........@...s
+00001af0: 3400 0000 6500 5a01 6400 5a02 6401 6503  4...e.Z.d.Z.d.e.
+00001b00: 6402 6503 6604 6403 6404 8404 5a04 6405  d.e.f.d.d...Z.d.
+00001b10: 6503 6402 6505 6503 1900 6604 6406 6407  e.d.e.e...f.d.d.
+00001b20: 8404 5a06 6408 5300 2909 da06 4f70 656e  ..Z.d.S.)...Open
+00001b30: 4149 7217 0000 0072 0e00 0000 6302 0000  AIr....r....c...
+00001b40: 0000 0000 0000 0000 0005 0000 0006 0000  ................
+00001b50: 0043 0000 0073 5200 0000 6401 6400 6c00  .C...sR...d.d.l.
+00001b60: 7d02 6402 6403 6802 7d03 7c02 6a01 7c00  }.d.d.h.}.|.j.|.
+00001b70: 6a02 7c03 7600 7211 6404 6e01 6405 7c00  j.|.v.r.d.n.d.|.
+00001b80: 6a03 6406 1900 6407 7404 6a05 9b00 6408  j.d...d.t.j...d.
+00001b90: 8d04 7d02 7c02 6a06 7c01 7c00 6a07 6409  ..}.|.j.|.|.j.d.
+00001ba0: 8d02 7d04 7408 7c04 8301 5300 290a 4e72  ..}.t.|...S.).Nr
+00001bb0: 0100 0000 7a05 6770 742d 3472 8200 0000  ....z.gpt-4r....
+00001bc0: da0a 6f70 656e 6169 6368 6174 da06 6f70  ..openaichat..op
+00001bd0: 656e 6169 7286 0000 00da 0673 716c 6974  enair......sqlit
+00001be0: 6529 04da 0b63 6c69 656e 745f 6e61 6d65  e)...client_name
+00001bf0: 7286 0000 00da 0a63 6163 6865 5f6e 616d  r......cache_nam
+00001c00: 65da 1063 6163 6865 5f63 6f6e 6e65 6374  e..cache_connect
+00001c10: 696f 6e29 01da 0e73 746f 705f 7365 7175  ion)...stop_sequ
+00001c20: 656e 6365 7329 09da 086d 616e 6966 6573  ences)...manifes
+00001c30: 74da 084d 616e 6966 6573 7472 8500 0000  t..Manifestr....
+00001c40: 728a 0000 00da 104d 696e 6963 6861 696e  r......Minichain
+00001c50: 436f 6e74 6578 74da 046e 616d 6572 1d00  Context..namer..
+00001c60: 0000 7288 0000 0072 2e00 0000 2905 7214  ..r....r....).r.
+00001c70: 0000 0072 1700 0000 7295 0000 00da 0463  ...r....r......c
+00001c80: 6861 74da 0361 6e73 7212 0000 0072 1200  hat..ansr....r..
+00001c90: 0000 7215 0000 0072 1d00 0000 be00 0000  ..r....r........
+00001ca0: 731a 0000 0008 0108 0204 0110 0108 0102  s...............
+00001cb0: 0106 0106 fc04 0702 0104 0106 fe08 047a  ...............z
+00001cc0: 0a4f 7065 6e41 492e 7275 6eda 0670 726f  .OpenAI.run..pro
+00001cd0: 6d70 7463 0200 0000 0000 0000 0000 0000  mptc............
+00001ce0: 0500 0000 0600 0000 6300 0000 7380 0000  ........c...s...
+00001cf0: 0081 0064 0164 006c 007d 0274 016a 02a0  ...d.d.l.}.t.j..
+00001d00: 0364 02a1 017c 005f 047c 006a 0473 134a  .d...|._.|.j.s.J
+00001d10: 0064 0383 0182 017c 006a 047c 025f 047c  .d.....|.j.|._.|
+00001d20: 026a 056a 067c 006a 0764 047c 0164 059c  .j.j.|.j.d.|.d..
+00001d30: 0267 0164 067c 006a 0864 078d 0444 005d  .g.d.|.j.d...D.]
+00001d40: 167d 037c 0364 0819 0064 0119 00a0 0364  .}.|.d...d.....d
+00001d50: 0969 00a1 02a0 0364 0aa1 017d 047c 0464  .i.....d...}.|.d
+00001d60: 0075 0172 3d7c 0456 0001 0071 2764 0053  .u.r=|.V...q'd.S
+00001d70: 0029 0b4e 7201 0000 00da 0e4f 5045 4e41  .).Nr......OPENA
+00001d80: 495f 4150 495f 4b45 59fa 3c4e 6565 6420  I_API_KEY.<Need 
+00001d90: 616e 204f 5045 4e41 495f 4150 495f 4b45  an OPENAI_API_KE
+00001da0: 592e 2047 6574 206f 6e65 2068 6572 6520  Y. Get one here 
+00001db0: 6874 7470 733a 2f2f 6f70 656e 6169 2e63  https://openai.c
+00001dc0: 6f6d 2f61 7069 2fda 0475 7365 7229 02da  om/api/..user)..
+00001dd0: 0472 6f6c 65da 0763 6f6e 7465 6e74 5429  .role..contentT)
+00001de0: 0472 8500 0000 da08 6d65 7373 6167 6573  .r......messages
+00001df0: da06 7374 7265 616d 7288 0000 00da 0763  ..streamr......c
+00001e00: 686f 6963 6573 da05 6465 6c74 6172 a000  hoices..deltar..
+00001e10: 0000 2909 728f 0000 0072 5300 0000 7254  ..).r....rS...rT
+00001e20: 0000 0072 5500 0000 7247 0000 00da 0e43  ...rU...rG.....C
+00001e30: 6861 7443 6f6d 706c 6574 696f 6eda 0663  hatCompletion..c
+00001e40: 7265 6174 6572 8500 0000 7288 0000 0029  reater....r....)
+00001e50: 0572 1400 0000 729b 0000 0072 8f00 0000  .r....r....r....
+00001e60: da05 6368 756e 6b72 a000 0000 7212 0000  ..chunkr....r...
+00001e70: 0072 1200 0000 7215 0000 0072 1f00 0000  .r....r....r....
+00001e80: cf00 0000 7326 0000 0002 8008 010e 0204  ....s&..........
+00001e90: 0204 ff02 0204 fe08 0306 0204 010a 0102  ................
+00001ea0: 0104 010a fc1a 0608 0106 0102 8004 f87a  ...............z
+00001eb0: 114f 7065 6e41 492e 7275 6e5f 7374 7265  .OpenAI.run_stre
+00001ec0: 616d 4e29 0772 2a00 0000 722b 0000 0072  amN).r*...r+...r
+00001ed0: 2c00 0000 722e 0000 0072 1d00 0000 7207  ,...r....r....r.
+00001ee0: 0000 0072 1f00 0000 7212 0000 0072 1200  ...r....r....r..
+00001ef0: 0000 7212 0000 0072 1500 0000 728d 0000  ..r....r....r...
+00001f00: 00bd 0000 0073 0600 0000 0800 1201 1a11  .....s..........
+00001f10: 728d 0000 0063 0000 0000 0000 0000 0000  r....c..........
+00001f20: 0000 0000 0000 0700 0000 0000 0000 734e  ..............sN
+00001f30: 0000 0065 005a 0164 005a 0264 0165 036a  ...e.Z.d.Z.d.e.j
+00001f40: 0466 0264 0264 0384 045a 0564 0d64 0565  .f.d.d...Z.d.d.e
+00001f50: 0664 0665 0764 0164 0766 0687 0066 0164  .d.e.d.d.f...f.d
+00001f60: 0864 0984 0d5a 0864 0a65 0664 0165 0666  .d...Z.d.e.d.e.f
+00001f70: 0464 0b64 0c84 045a 0987 0004 005a 0a53  .d.d...Z.....Z.S
+00001f80: 0029 0eda 0b4f 7065 6e41 4945 6d62 6564  .)...OpenAIEmbed
+00001f90: 720e 0000 0063 0100 0000 0000 0000 0000  r....c..........
+00001fa0: 0000 0100 0000 0300 0000 4300 0000 7221  ..........C...r!
+00001fb0: 0000 0029 034e da09 456d 6265 6464 696e  ...).N..Embeddin
+00001fc0: 6729 01da 056c 6162 656c 7224 0000 0072  g)...labelr$...r
+00001fd0: 1300 0000 7212 0000 0072 1200 0000 7215  ....r....r....r.
+00001fe0: 0000 0072 2900 0000 e400 0000 7228 0000  ...r).......r(..
+00001ff0: 007a 184f 7065 6e41 4945 6d62 6564 2e62  .z.OpenAIEmbed.b
+00002000: 6c6f 636b 5f6f 7574 7075 74fa 1674 6578  lock_output..tex
+00002010: 742d 656d 6265 6464 696e 672d 6164 612d  t-embedding-ada-
+00002020: 3030 3272 8500 0000 da06 6b77 6172 6773  002r......kwargs
+00002030: 4e63 0200 0000 0000 0000 0000 0000 0300  Nc..............
+00002040: 0000 0400 0000 0b00 0000 7318 0000 0074  ..........s....t
+00002050: 0083 006a 017c 0166 0169 007c 02a4 018e  ...j.|.f.i.|....
+00002060: 0101 0064 0053 0072 1900 0000 2902 da05  ...d.S.r....)...
+00002070: 7375 7065 7272 3800 0000 2903 7214 0000  superr8...).r...
+00002080: 0072 8500 0000 72ac 0000 00a9 01da 095f  .r....r........_
+00002090: 5f63 6c61 7373 5f5f 7212 0000 0072 1500  _class__r....r..
+000020a0: 0000 7238 0000 00e7 0000 00f3 0200 0000  ..r8............
+000020b0: 1801 7a14 4f70 656e 4149 456d 6265 642e  ..z.OpenAIEmbed.
+000020c0: 5f5f 696e 6974 5f5f 7217 0000 0063 0200  __init__r....c..
+000020d0: 0000 0000 0000 0000 0000 0400 0000 0400  ................
+000020e0: 0000 4300 0000 734e 0000 0064 0164 006c  ..C...sN...d.d.l
+000020f0: 007d 0274 016a 02a0 0364 02a1 017c 005f  .}.t.j...d...|._
+00002100: 047c 006a 0473 124a 0064 0383 0182 017c  .|.j.s.J.d.....|
+00002110: 006a 047c 025f 047c 026a 056a 067c 006a  .j.|._.|.j.j.|.j
+00002120: 077c 0164 048d 027d 037c 0364 0519 0064  .|.d...}.|.d...d
+00002130: 0119 0064 0619 0053 0029 074e 7201 0000  ...d...S.).Nr...
+00002140: 0072 9c00 0000 729d 0000 0029 0272 4800  .r....r....).rH.
+00002150: 0000 da05 696e 7075 74da 0464 6174 61da  ....input..data.
+00002160: 0965 6d62 6564 6469 6e67 2908 728f 0000  .embedding).r...
+00002170: 0072 5300 0000 7254 0000 0072 5500 0000  .rS...rT...rU...
+00002180: 7247 0000 0072 a900 0000 72a6 0000 0072  rG...r....r....r
+00002190: 8500 0000 2904 7214 0000 0072 1700 0000  ....).r....r....
+000021a0: 728f 0000 0072 9a00 0000 7212 0000 0072  r....r....r....r
+000021b0: 1200 0000 7215 0000 0072 1d00 0000 ea00  ....r....r......
+000021c0: 0000 7318 0000 0008 010e 0204 0204 ff02  ..s.............
+000021d0: 0204 fe08 0306 0204 0102 0106 fe10 047a  ...............z
+000021e0: 0f4f 7065 6e41 4945 6d62 6564 2e72 756e  .OpenAIEmbed.run
+000021f0: 2901 72ab 0000 0029 0b72 2a00 0000 722b  ).r....).r*...r+
+00002200: 0000 0072 2c00 0000 7225 0000 0072 2f00  ...r,...r%...r/.
+00002210: 0000 7229 0000 0072 2e00 0000 7205 0000  ..r)...r....r...
+00002220: 0072 3800 0000 721d 0000 00da 0d5f 5f63  .r8...r......__c
+00002230: 6c61 7373 6365 6c6c 5f5f 7212 0000 0072  lasscell__r....r
+00002240: 1200 0000 72ae 0000 0072 1500 0000 72a8  ....r....r....r.
+00002250: 0000 00e3 0000 0073 0800 0000 0800 1001  .......s........
+00002260: 1c03 1a03 72a8 0000 0063 0000 0000 0000  ....r....c......
+00002270: 0000 0000 0000 0000 0000 0500 0000 4000  ..............@.
+00002280: 0000 7320 0000 0065 005a 0164 005a 0264  ..s ...e.Z.d.Z.d
+00002290: 0764 0265 0364 0364 0466 0464 0564 0684  .d.e.d.d.f.d.d..
+000022a0: 055a 0464 0453 0029 08da 0f48 7567 6769  .Z.d.S.)...Huggi
+000022b0: 6e67 4661 6365 4261 7365 da04 6770 7432  ngFaceBase..gpt2
+000022c0: 7285 0000 0072 0e00 0000 4e63 0200 0000  r....r....Nc....
+000022d0: 0000 0000 0000 0000 0200 0000 0200 0000  ................
+000022e0: 4300 0000 730a 0000 007c 017c 005f 0064  C...s....|.|._.d
+000022f0: 0053 0072 1900 0000 2901 7285 0000 0029  .S.r....).r....)
+00002300: 0272 1400 0000 7285 0000 0072 1200 0000  .r....r....r....
+00002310: 7212 0000 0072 1500 0000 7238 0000 00fb  r....r....r8....
+00002320: 0000 0073 0200 0000 0a01 7a18 4875 6767  ...s......z.Hugg
+00002330: 696e 6746 6163 6542 6173 652e 5f5f 696e  ingFaceBase.__in
+00002340: 6974 5f5f 2901 72b6 0000 0029 0572 2a00  it__).r....).r*.
+00002350: 0000 722b 0000 0072 2c00 0000 722e 0000  ..r+...r,...r...
+00002360: 0072 3800 0000 7212 0000 0072 1200 0000  .r8...r....r....
+00002370: 7212 0000 0072 1500 0000 72b5 0000 00fa  r....r....r.....
+00002380: 0000 0073 0400 0000 0800 1801 72b5 0000  ...s........r...
+00002390: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+000023a0: 0000 0400 0000 4000 0000 7230 0000 0029  ......@...r0...)
+000023b0: 06da 0b48 7567 6769 6e67 4661 6365 7217  ...HuggingFacer.
+000023c0: 0000 0072 0e00 0000 6302 0000 0000 0000  ...r....c.......
+000023d0: 0000 0000 0004 0000 0005 0000 0043 0000  .............C..
+000023e0: 00f3 4c00 0000 6401 6402 6c00 6d01 7d02  ..L...d.d.l.m.}.
+000023f0: 0100 7402 6a03 a004 6403 a101 7c00 5f05  ..t.j...d...|._.
+00002400: 7c00 6a05 7314 4a00 6404 8301 8201 7c02  |.j.s.J.d.....|.
+00002410: 7c00 6a05 7c00 6a06 6405 6406 8d03 7c00  |.j.|.j.d.d...|.
+00002420: 5f07 7c00 6a07 7c01 6407 8d01 7d03 7c03  _.|.j.|.d...}.|.
+00002430: 5300 2908 4e72 0100 0000 a901 da0c 496e  S.).Nr........In
+00002440: 6665 7265 6e63 6541 7069 da06 4846 5f4b  ferenceApi..HF_K
+00002450: 4559 fa34 4e65 6564 2061 6e20 4846 5f4b  EY.4Need an HF_K
+00002460: 4559 2e20 4765 7420 6f6e 6520 6865 7265  EY. Get one here
+00002470: 2068 7474 7073 3a2f 2f68 7567 6769 6e67   https://hugging
+00002480: 6661 6365 2e63 6f2f 7a0f 7465 7874 2d67  face.co/z.text-g
+00002490: 656e 6572 6174 696f 6ea9 03da 0574 6f6b  eneration....tok
+000024a0: 656e da07 7265 706f 5f69 64da 0474 6173  en..repo_id..tas
+000024b0: 6ba9 01da 0669 6e70 7574 73a9 08da 1d68  k....inputs....h
+000024c0: 7567 6769 6e67 6661 6365 5f68 7562 2e69  uggingface_hub.i
+000024d0: 6e66 6572 656e 6365 5f61 7069 72ba 0000  nference_apir...
+000024e0: 0072 5300 0000 7254 0000 0072 5500 0000  .rS...rT...rU...
+000024f0: 7247 0000 0072 8500 0000 da06 636c 6965  rG...r......clie
+00002500: 6e74 a904 7214 0000 0072 1700 0000 72ba  nt..r....r....r.
+00002510: 0000 00da 0872 6573 706f 6e73 6572 1200  .....responser..
+00002520: 0000 7212 0000 0072 1500 0000 721d 0000  ..r....r....r...
+00002530: 0000 0100 00f3 1000 0000 0c02 0e02 0e01  ................
+00002540: 0202 0a01 08ff 0c03 0401 7a0f 4875 6767  ..........z.Hugg
+00002550: 696e 6746 6163 652e 7275 6e4e 7232 0000  ingFace.runNr2..
+00002560: 0072 1200 0000 7212 0000 0072 1200 0000  .r....r....r....
+00002570: 7215 0000 0072 b700 0000 ff00 0000 7233  r....r........r3
+00002580: 0000 0072 b700 0000 6300 0000 0000 0000  ...r....c.......
+00002590: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
+000025a0: 0072 3000 0000 2906 da10 4875 6767 696e  .r0...)...Huggin
+000025b0: 6746 6163 6545 6d62 6564 7217 0000 0072  gFaceEmbedr....r
+000025c0: 0e00 0000 6302 0000 0000 0000 0000 0000  ....c...........
+000025d0: 0004 0000 0005 0000 0043 0000 0072 b800  .........C...r..
+000025e0: 0000 2908 4e72 0100 0000 72b9 0000 0072  ..).Nr....r....r
+000025f0: bb00 0000 72bc 0000 007a 1266 6561 7475  ....r....z.featu
+00002600: 7265 2d65 7874 7261 6374 696f 6e72 bd00  re-extractionr..
+00002610: 0000 72c1 0000 0072 c300 0000 72c6 0000  ..r....r....r...
+00002620: 0072 1200 0000 7212 0000 0072 1500 0000  .r....r....r....
+00002630: 721d 0000 000f 0100 0072 c800 0000 7a14  r........r....z.
+00002640: 4875 6767 696e 6746 6163 6545 6d62 6564  HuggingFaceEmbed
+00002650: 2e72 756e 4e72 3200 0000 7212 0000 0072  .runNr2...r....r
+00002660: 1200 0000 7212 0000 0072 1500 0000 72c9  ....r....r....r.
+00002670: 0000 000e 0100 0072 3300 0000 72c9 0000  .......r3...r...
+00002680: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00002690: 0000 0400 0000 4000 0000 7328 0000 0065  ......@...s(...e
+000026a0: 005a 0164 005a 0264 0a64 0564 0684 045a  .Z.d.Z.d.d.d...Z
+000026b0: 0364 0765 0464 0365 0466 0464 0864 0984  .d.e.d.e.f.d.d..
+000026c0: 045a 0564 0453 0029 0b72 9600 0000 72c5  .Z.d.S.).r....r.
+000026d0: 0000 00fa 116d 616e 6966 6573 742e 4d61  .....manifest.Ma
+000026e0: 6e69 6665 7374 720e 0000 004e 6302 0000  nifestr....Nc...
+000026f0: 0000 0000 0000 0000 0002 0000 0002 0000  ................
+00002700: 0043 0000 0073 0a00 0000 7c01 7c00 5f00  .C...s....|.|._.
+00002710: 6401 5300 2902 7a44 436c 6965 6e74 2066  d.S.).zDClient f
+00002720: 726f 6d20 5b4d 616e 6966 6573 742d 4d4c  rom [Manifest-ML
+00002730: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00002740: 2e63 6f6d 2f48 617a 7952 6573 6561 7263  .com/HazyResearc
+00002750: 682f 6d61 6e69 6665 7374 292e 4e29 0172  h/manifest).N).r
+00002760: c500 0000 2902 7214 0000 0072 c500 0000  ....).r....r....
+00002770: 7212 0000 0072 1200 0000 7215 0000 0072  r....r....r....r
+00002780: 3800 0000 1e01 0000 7302 0000 000a 027a  8.......s......z
+00002790: 114d 616e 6966 6573 742e 5f5f 696e 6974  .Manifest.__init
+000027a0: 5f5f 7217 0000 0063 0200 0000 0000 0000  __r....c........
+000027b0: 0000 0000 0300 0000 0800 0000 4300 0000  ............C...
+000027c0: 7346 0000 007a 0664 0164 006c 007d 0257  sF...z.d.d.l.}.W
+000027d0: 006e 0b04 0074 0179 1101 0001 0001 0074  .n...t.y.......t
+000027e0: 0164 0283 0182 0177 0074 027c 006a 037c  .d.....w.t.|.j.|
+000027f0: 026a 0483 0273 1d4a 0064 0383 0182 017c  .j...s.J.d.....|
+00002800: 006a 03a0 057c 01a1 0153 0029 044e 7201  .j...|...S.).Nr.
+00002810: 0000 007a 3660 7069 7020 696e 7374 616c  ...z6`pip instal
+00002820: 6c20 6d61 6e69 6665 7374 2d6d 6c60 2074  l manifest-ml` t
+00002830: 6f20 7573 6520 7468 6520 4d61 6e69 6665  o use the Manife
+00002840: 7374 2042 6163 6b65 6e64 2e7a 2e43 6c69  st Backend.z.Cli
+00002850: 656e 7420 6d75 7374 2062 6520 6120 606d  ent must be a `m
+00002860: 616e 6966 6573 742e 4d61 6e69 6665 7374  anifest.Manifest
+00002870: 6020 696e 7374 616e 6365 2e29 0672 9500  ` instance.).r..
+00002880: 0000 da0b 496d 706f 7274 4572 726f 72da  ....ImportError.
+00002890: 0a69 7369 6e73 7461 6e63 6572 c500 0000  .isinstancer....
+000028a0: 7296 0000 0072 1d00 0000 2903 7214 0000  r....r....).r...
+000028b0: 0072 1700 0000 7295 0000 0072 1200 0000  .r....r....r....
+000028c0: 7212 0000 0072 1500 0000 721d 0000 0022  r....r....r...."
+000028d0: 0100 0073 1600 0000 0201 0c01 0c01 0801  ...s............
+000028e0: 02ff 0202 0801 06ff 0202 04fe 0c04 7a0c  ..............z.
+000028f0: 4d61 6e69 6665 7374 2e72 756e 2904 72c5  Manifest.run).r.
+00002900: 0000 0072 ca00 0000 720e 0000 004e 2906  ...r....r....N).
+00002910: 722a 0000 0072 2b00 0000 722c 0000 0072  r*...r+...r,...r
+00002920: 3800 0000 722e 0000 0072 1d00 0000 7212  8...r....r....r.
+00002930: 0000 0072 1200 0000 7212 0000 0072 1500  ...r....r....r..
+00002940: 0000 7296 0000 001d 0100 0073 0600 0000  ..r........s....
+00002950: 0800 0a01 1604 7296 0000 0063 0000 0000  ......r....c....
+00002960: 0000 0000 0000 0000 0000 0000 0300 0000  ................
+00002970: 4000 0000 7342 0000 0065 005a 0164 005a  @...sB...e.Z.d.Z
+00002980: 0255 0064 015a 0365 0465 0564 023c 0064  .U.d.Z.e.e.d.<.d
+00002990: 015a 0665 0765 0419 0065 0564 033c 0064  .Z.e.e...e.d.<.d
+000029a0: 015a 0865 0465 0564 043c 0064 055a 0965  .Z.e.e.d.<.d.Z.e
+000029b0: 0a65 0564 063c 0064 0753 0029 08da 0652  .e.d.<.d.S.)...R
+000029c0: 756e 4c6f 6772 1100 0000 7217 0000 0072  unLogr....r....r
+000029d0: c700 0000 727e 0000 0072 0100 0000 da07  ....r~...r......
+000029e0: 6479 6e61 6d69 634e 290b 722a 0000 0072  dynamicN).r*...r
+000029f0: 2b00 0000 722c 0000 0072 1700 0000 722e  +...r,...r....r.
+00002a00: 0000 00da 0f5f 5f61 6e6e 6f74 6174 696f  .....__annotatio
+00002a10: 6e73 5f5f 72c7 0000 0072 0900 0000 727e  ns__r....r....r~
+00002a20: 0000 0072 ce00 0000 728b 0000 0072 1200  ...r....r....r..
+00002a30: 0000 7212 0000 0072 1200 0000 7215 0000  ..r....r....r...
+00002a40: 0072 cd00 0000 2e01 0000 730a 0000 000a  .r........s.....
+00002a50: 000c 0210 010c 0110 0172 cd00 0000 6300  .........r....c.
+00002a60: 0000 0000 0000 0000 0000 0000 0000 0003  ................
+00002a70: 0000 0040 0000 0073 3400 0000 6500 5a01  ...@...s4...e.Z.
+00002a80: 6400 5a02 5500 6401 5a03 6504 6505 6402  d.Z.U.d.Z.e.e.d.
+00002a90: 3c00 6506 8300 5a07 6506 6505 6403 3c00  <.e...Z.e.e.d.<.
+00002aa0: 6401 5a08 6504 6505 6404 3c00 6405 5300  d.Z.e.e.d.<.d.S.
+00002ab0: 2906 da0a 5072 6f6d 7074 536e 6170 7211  )...PromptSnapr.
+00002ac0: 0000 00da 0669 6e70 7574 5fda 0772 756e  .....input_..run
+00002ad0: 5f6c 6f67 727e 0000 004e 2909 722a 0000  _logr~...N).r*..
+00002ae0: 0072 2b00 0000 722c 0000 0072 d100 0000  .r+...r,...r....
+00002af0: 7205 0000 0072 cf00 0000 72cd 0000 0072  r....r....r....r
+00002b00: d200 0000 727e 0000 0072 1200 0000 7212  ....r~...r....r.
+00002b10: 0000 0072 1200 0000 7215 0000 0072 d000  ...r....r....r..
+00002b20: 0000 3601 0000 7308 0000 000a 000c 020e  ..6...s.........
+00002b30: 0110 0172 d000 0000 6300 0000 0000 0000  ...r....c.......
+00002b40: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
+00002b50: 0073 5a00 0000 6500 5a01 6400 5a02 5500  .sZ...e.Z.d.Z.U.
+00002b60: 6401 5a03 6504 6505 6402 3c00 6900 5a06  d.Z.e.e.d.<.i.Z.
+00002b70: 6507 6508 6504 6504 6602 1900 6509 650a  e.e.e.e.f...e.e.
+00002b80: 1900 6602 1900 6505 6403 3c00 6900 5a0b  ..f...e.d.<.i.Z.
+00002b90: 6507 6504 6504 6602 1900 6505 6404 3c00  e.e.e.f...e.d.<.
+00002ba0: 6405 5a0c 650d 6505 6406 3c00 6407 5300  d.Z.e.e.d.<.d.S.
+00002bb0: 2908 7297 0000 0072 0100 0000 da03 6964  ).r....r......id
+00002bc0: 5fda 0c70 726f 6d70 745f 7374 6f72 65da  _..prompt_store.
+00002bd0: 0c70 726f 6d70 745f 636f 756e 7472 1100  .prompt_countr..
+00002be0: 0000 7298 0000 004e 290e 722a 0000 0072  ..r....N).r*...r
+00002bf0: 2b00 0000 722c 0000 0072 d300 0000 728b  +...r,...r....r.
+00002c00: 0000 0072 cf00 0000 72d4 0000 0072 0600  ...r....r....r..
+00002c10: 0000 720a 0000 0072 0800 0000 72d0 0000  ..r....r....r...
+00002c20: 0072 d500 0000 7298 0000 0072 2e00 0000  .r....r....r....
+00002c30: 7212 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
+00002c40: 1500 0000 7297 0000 003d 0100 0073 0a00  ....r....=...s..
+00002c50: 0000 0a00 0c01 2001 1401 1001 7297 0000  ...... .....r...
+00002c60: 0072 9800 0000 720e 0000 0063 0100 0000  .r....r....c....
+00002c70: 0000 0000 0000 0000 0100 0000 0400 0000  ................
+00002c80: 4300 0000 7318 0000 0074 0074 017c 009b  C...s....t.t.|..
+00002c90: 0064 019d 0264 0283 0283 0101 0064 0053  .d...d.......d.S
+00002ca0: 00a9 034e 7a04 2e6c 6f67 da01 7729 0272  ...Nz..log..w).r
+00002cb0: 0c00 0000 da04 6f70 656e a901 7298 0000  ......open..r...
+00002cc0: 0072 1200 0000 7212 0000 0072 1500 0000  .r....r....r....
+00002cd0: da11 7365 745f 6d69 6e69 6368 6169 6e5f  ..set_minichain_
+00002ce0: 6c6f 6744 0100 0072 b000 0000 72da 0000  logD...r....r...
+00002cf0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00002d00: 0000 0800 0000 4000 0000 734a 0000 0065  ......@...sJ...e
+00002d10: 005a 0164 005a 0264 015a 0364 0265 0466  .Z.d.Z.d.Z.d.e.f
+00002d20: 0264 0364 0484 045a 0564 0e64 0664 0784  .d.d...Z.d.d.d..
+00002d30: 045a 0664 0865 0764 0965 0865 0919 0064  .Z.d.e.d.e.e...d
+00002d40: 0a65 0865 0a19 0064 0564 0b66 0864 0c64  .e.e...d.d.f.d.d
+00002d50: 0d84 045a 0b64 0b53 0029 0fda 094d 696e  ...Z.d.S.)...Min
+00002d60: 6943 6861 696e 7a80 0a20 2020 204d 696e  iChainz..    Min
+00002d70: 6943 6861 696e 2073 6573 7369 6f6e 206f  iChain session o
+00002d80: 626a 6563 7420 7769 7468 2062 6163 6b65  bject with backe
+00002d90: 6e64 732e 204d 616b 6520 6261 636b 656e  nds. Make backen
+00002da0: 6420 6279 2063 616c 6c69 6e67 0a20 2020  d by calling.   
+00002db0: 2060 6d69 6e69 6368 6169 6e2e 4f70 656e   `minichain.Open
+00002dc0: 4149 2829 6020 7769 7468 2061 7267 7320  AI()` with args 
+00002dd0: 666f 7220 604f 7065 6e41 4960 2063 6c61  for `OpenAI` cla
+00002de0: 7373 2e0a 2020 2020 7298 0000 0063 0200  ss..    r....c..
+00002df0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+00002e00: 0000 4300 0000 731e 0000 0074 0074 017c  ..C...s....t.t.|
+00002e10: 019b 0064 019d 0264 0283 0283 0101 007c  ...d...d.......|
+00002e20: 017c 005f 0264 0053 0072 d600 0000 2903  .|._.d.S.r....).
+00002e30: 720c 0000 0072 d800 0000 7298 0000 0029  r....r....r....)
+00002e40: 0272 1400 0000 7298 0000 0072 1200 0000  .r....r....r....
+00002e50: 7212 0000 0072 1500 0000 7238 0000 004e  r....r....r8...N
+00002e60: 0100 0073 0400 0000 1401 0a01 7a12 4d69  ...s........z.Mi
+00002e70: 6e69 4368 6169 6e2e 5f5f 696e 6974 5f5f  niChain.__init__
+00002e80: 720e 0000 0063 0100 0000 0000 0000 0000  r....c..........
+00002e90: 0000 0100 0000 0300 0000 4300 0000 7326  ..........C...s&
+00002ea0: 0000 0069 0074 005f 0169 0074 005f 027c  ...i.t._.i.t._.|
+00002eb0: 006a 0374 005f 0374 047c 006a 0364 018d  .j.t._.t.|.j.d..
+00002ec0: 017c 005f 057c 0053 0029 024e 2901 da0b  .|._.|.S.).N)...
+00002ed0: 6163 7469 6f6e 5f74 7970 6529 0672 9700  action_type).r..
+00002ee0: 0000 72d4 0000 0072 d500 0000 7298 0000  ..r....r....r...
+00002ef0: 0072 0b00 0000 da06 6163 7469 6f6e 7213  .r......actionr.
+00002f00: 0000 0072 1200 0000 7212 0000 0072 1500  ...r....r....r..
+00002f10: 0000 da09 5f5f 656e 7465 725f 5f52 0100  ....__enter__R..
+00002f20: 0073 0a00 0000 0601 0601 0801 0e01 0401  .s..............
+00002f30: 7a13 4d69 6e69 4368 6169 6e2e 5f5f 656e  z.MiniChain.__en
+00002f40: 7465 725f 5fda 0474 7970 65da 0965 7863  ter__..type..exc
+00002f50: 6570 7469 6f6e da09 7472 6163 6562 6163  eption..tracebac
+00002f60: 6b4e 6304 0000 0000 0000 0000 0000 0004  kNc.............
+00002f70: 0000 0002 0000 0043 0000 0073 2c00 0000  .......C...s,...
+00002f80: 7c00 6a00 a001 a100 0100 7402 7403 6a04  |.j.......t.t.j.
+00002f90: 8301 7c00 5f04 6900 7403 5f04 6900 7403  ..|._.i.t._.i.t.
+00002fa0: 5f05 6401 7403 5f06 6400 5300 7210 0000  _.d.t._.d.S.r...
+00002fb0: 0029 0772 dd00 0000 da06 6669 6e69 7368  .).r......finish
+00002fc0: 7289 0000 0072 9700 0000 72d4 0000 0072  r....r....r....r
+00002fd0: d500 0000 7298 0000 0029 0472 1400 0000  ....r....).r....
+00002fe0: 72df 0000 0072 e000 0000 72e1 0000 0072  r....r....r....r
+00002ff0: 1200 0000 7212 0000 0072 1500 0000 da08  ....r....r......
+00003000: 5f5f 6578 6974 5f5f 5901 0000 730a 0000  __exit__Y...s...
+00003010: 000a 060c 0106 0106 010a 017a 124d 696e  ...........z.Min
+00003020: 6943 6861 696e 2e5f 5f65 7869 745f 5f29  iChain.__exit__)
+00003030: 0272 0e00 0000 72db 0000 0029 0c72 2a00  .r....r....).r*.
+00003040: 0000 722b 0000 0072 2c00 0000 7271 0000  ..r+...r,...rq..
+00003050: 0072 2e00 0000 7238 0000 0072 de00 0000  .r....r8...r....
+00003060: 72df 0000 0072 0900 0000 da0d 4261 7365  r....r......Base
+00003070: 4578 6365 7074 696f 6e72 0300 0000 72e3  Exceptionr....r.
+00003080: 0000 0072 1200 0000 7212 0000 0072 1200  ...r....r....r..
+00003090: 0000 7215 0000 0072 db00 0000 4801 0000  ..r....r....H...
+000030a0: 731a 0000 0008 0004 010e 050a 0402 0702  s...............
+000030b0: 0202 fe06 0302 fd06 0402 fc02 050e fb72  ...............r
+000030c0: db00 0000 6301 0000 0000 0000 0000 0000  ....c...........
+000030d0: 0001 0000 0002 0000 0043 0000 0073 0800  .........C...s..
+000030e0: 0000 7400 7c00 8301 5300 2901 7a65 0a20  ..t.|...S.).ze. 
+000030f0: 2020 2049 6e69 7469 616c 697a 6520 6120     Initialize a 
+00003100: 6368 6169 6e2e 204c 6f67 7320 746f 207b  chain. Logs to {
+00003110: 6e61 6d65 7d2e 6c6f 672e 2052 6574 7572  name}.log. Retur
+00003120: 6e73 2061 2060 4d69 6e69 4368 6169 6e60  ns a `MiniChain`
+00003130: 2074 6861 740a 2020 2020 686f 6c64 7320   that.    holds 
+00003140: 4c4c 4d20 6261 636b 656e 6473 2e2e 0a20  LLM backends... 
+00003150: 2020 2029 0172 db00 0000 72d9 0000 0072     ).r....r....r
+00003160: 1200 0000 7212 0000 0072 1500 0000 da0b  ....r....r......
+00003170: 7374 6172 745f 6368 6169 6e66 0100 0073  start_chainf...s
+00003180: 0200 0000 0805 72e5 0000 0029 2972 5300  ......r....))rS.
+00003190: 0000 7279 0000 0072 3b00 0000 da0b 6461  ..ry...r;.....da
+000031a0: 7461 636c 6173 7365 7372 0200 0000 da05  taclassesr......
+000031b0: 7479 7065 7372 0300 0000 da06 7479 7069  typesr......typi
+000031c0: 6e67 7204 0000 0072 0500 0000 7206 0000  ngr....r....r...
+000031d0: 0072 0700 0000 7208 0000 0072 0900 0000  .r....r....r....
+000031e0: 720a 0000 00da 0667 7261 6469 6f72 2500  r......gradior%.
+000031f0: 0000 da05 656c 696f 7472 0b00 0000 720c  ....eliotr....r.
+00003200: 0000 0072 9500 0000 720d 0000 0072 3100  ...r....r....r1.
+00003210: 0000 7234 0000 0072 4100 0000 725d 0000  ..r4...rA...r]..
+00003220: 0072 7200 0000 7281 0000 0072 8d00 0000  .rr...r....r....
+00003230: 72a8 0000 0072 b500 0000 72b7 0000 0072  r....r....r....r
+00003240: c900 0000 7296 0000 0072 cd00 0000 72d0  ....r....r....r.
+00003250: 0000 0072 9700 0000 722e 0000 0072 da00  ...r....r....r..
+00003260: 0000 72db 0000 0072 e500 0000 7212 0000  ..r....r....r...
+00003270: 0072 1200 0000 7212 0000 0072 1500 0000  .r....r....r....
+00003280: da08 3c6d 6f64 756c 653e 0100 0000 733e  ..<module>....s>
+00003290: 0000 0008 0008 0108 010c 010c 0124 0108  .............$..
+000032a0: 0210 0104 0208 010e 0310 1510 0510 1410  ................
+000032b0: 2c10 1c10 2410 1410 2610 1710 0510 0f10  ,...$...&.......
+000032c0: 0f02 1110 0102 0710 010e 0612 070e 0416  ................
+000032d0: 1e                                       .
```

### ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/__pycache__/base.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 22:29:14 2023 UTC, .py size: 9095 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,553 +1,384 @@
-00000000: 6f0d 0d0a 0000 0000 3a82 3864 8723 0000  o.......:.8d.#..
+00000000: 6f0d 0d0a 0000 0000 80f5 3e64 d019 0000  o.........>d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0014 0000 0040 0000 0073 f001 0000 6400  .....@...s....d.
-00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
-00000040: 6d03 5a03 6d04 5a04 6d05 5a05 0100 6400  m.Z.m.Z.m.Z...d.
-00000050: 6403 6c06 6d07 5a07 0100 6400 6404 6c08  d.l.m.Z...d.d.l.
-00000060: 6d09 5a09 0100 6400 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
-00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  m.Z.m.Z.m.Z.m.Z.
-00000080: 6d10 5a10 6d11 5a11 6d12 5a12 6d13 5a13  m.Z.m.Z.m.Z.m.Z.
-00000090: 6d14 5a14 6d15 5a15 6d16 5a16 0100 6400  m.Z.m.Z.m.Z...d.
-000000a0: 6406 6c17 6d18 5a18 0100 6400 6407 6c19  d.l.m.Z...d.d.l.
-000000b0: 6d1a 5a1a 6d1b 5a1b 6d1c 5a1c 6d1d 5a1d  m.Z.m.Z.m.Z.m.Z.
-000000c0: 6d1e 5a1e 0100 6408 6409 6c1f 6d20 5a20  m.Z...d.d.l.m Z 
-000000d0: 6d21 5a21 6d22 5a22 0100 651a 651c 640a  m!Z!m"Z"..e.e.d.
-000000e0: 8301 651e 8300 640b 6701 640c 8d03 5a23  ..e...d.g.d...Z#
-000000f0: 640d 6514 6524 6522 6602 1900 640e 6522  d.e.e$e"f...d.e"
-00000100: 6604 640f 6410 8404 5a25 6513 6411 8301  f.d.d...Z%e.d...
-00000110: 5a26 6513 6412 8301 5a27 6513 6413 8301  Z&e.d...Z'e.d...
-00000120: 5a28 6414 6512 6507 1900 640e 650d 6524  Z(d.e.e...d.e.e$
-00000130: 6529 6602 1900 6604 6415 6416 8404 5a06  e)f...f.d.d...Z.
-00000140: 6414 650b 640e 650b 6604 6417 6418 8404  d.e.d.e.f.d.d...
-00000150: 5a2a 6419 652b 640e 6524 6604 641a 641b  Z*d.e+d.e$f.d.d.
-00000160: 8404 5a2c 641c 641d 8400 5a2d 6503 4700  ..Z,d.d...Z-e.G.
-00000170: 641e 641f 8400 641f 8302 8301 5a2e 6503  d.d...d.....Z.e.
-00000180: 4700 6420 6421 8400 6421 8302 8301 5a2f  G.d d!..d!....Z/
-00000190: 6503 4700 6422 6423 8400 6423 8302 8301  e.G.d"d#..d#....
-000001a0: 5a30 4700 6424 6425 8400 6425 650e 6526  Z0G.d$d%..d%e.e&
-000001b0: 6527 6528 6603 1900 8303 5a31 0926 0901  e'e(f.....Z1.&..
-000001c0: 0901 0901 0927 0901 0901 6430 6428 6520  .....'....d0d(e 
-000001d0: 6429 6514 6524 650b 6602 1900 642a 6510  d)e.e$e.f...d*e.
-000001e0: 6524 1900 642b 6510 6524 1900 642c 6510  e$..d+e.e$..d,e.
-000001f0: 6524 1900 642d 6532 640e 650c 650b 6701  e$..d-e2d.e.e.g.
-00000200: 6531 6526 6527 6528 6603 1900 6602 1900  e1e&e'e(f...f...
-00000210: 660e 642e 642f 8405 5a33 6401 5300 2931  f.d.d/..Z3d.S.)1
-00000220: e900 0000 004e 2904 da06 6173 6469 6374  .....N)...asdict
-00000230: da09 6461 7461 636c 6173 73da 0666 6965  ..dataclass..fie
-00000240: 6c64 73da 0c69 735f 6461 7461 636c 6173  lds..is_dataclas
-00000250: 7329 01da 0445 6e75 6d29 01da 0563 6f75  s)...Enum)...cou
-00000260: 6e74 290c da03 416e 79da 0843 616c 6c61  nt)...Any..Calla
-00000270: 626c 65da 0444 6963 74da 0747 656e 6572  ble..Dict..Gener
-00000280: 6963 da04 4c69 7374 da08 4f70 7469 6f6e  ic..List..Option
-00000290: 616c da05 5475 706c 65da 0454 7970 65da  al..Tuple..Type.
-000002a0: 0754 7970 6556 6172 da05 556e 696f 6eda  .TypeVar..Union.
-000002b0: 0867 6574 5f61 7267 73da 0a67 6574 5f6f  .get_args..get_o
-000002c0: 7269 6769 6e29 01da 0c73 7461 7274 5f61  rigin)...start_a
-000002d0: 6374 696f 6e29 05da 0b45 6e76 6972 6f6e  ction)...Environ
-000002e0: 6d65 6e74 da10 4669 6c65 5379 7374 656d  ment..FileSystem
-000002f0: 4c6f 6164 6572 da0d 5061 636b 6167 654c  Loader..PackageL
-00000300: 6f61 6465 72da 0854 656d 706c 6174 65da  oader..Template.
-00000310: 1173 656c 6563 745f 6175 746f 6573 6361  .select_autoesca
-00000320: 7065 e901 0000 0029 03da 0742 6163 6b65  pe.....)...Backe
-00000330: 6e64 da10 4d69 6e69 6368 6169 6e43 6f6e  nd..MinichainCon
-00000340: 7465 7874 da07 5265 7175 6573 74da 096d  text..Request..m
-00000350: 696e 6963 6861 696e 7a23 6a69 6e6a 6132  inichainz#jinja2
-00000360: 5f68 6967 686c 6967 6874 2e48 6967 686c  _highlight.Highl
-00000370: 6967 6874 4578 7465 6e73 696f 6e29 03da  ightExtension)..
-00000380: 066c 6f61 6465 72da 0a61 7574 6f65 7363  .loader..autoesc
-00000390: 6170 65da 0a65 7874 656e 7369 6f6e 73da  ape..extensions.
-000003a0: 0172 da06 7265 7475 726e 6301 0000 0000  .r..returnc.....
-000003b0: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
-000003c0: 0000 0073 1600 0000 7400 7c00 7401 8302  ...s....t.|.t...
-000003d0: 7209 7402 7c00 8301 5300 7c00 5300 a901  r.t.|...S.|.S...
-000003e0: 4e29 03da 0a69 7369 6e73 7461 6e63 65da  N)...isinstance.
-000003f0: 0373 7472 721d 0000 0029 0172 2200 0000  .strr....).r"...
-00000400: a900 7227 0000 00fa 522f 686f 6d65 2f73  ..r'....R/home/s
-00000410: 7275 7368 2f50 726f 6a65 6374 732f 4d69  rush/Projects/Mi
-00000420: 6e69 4368 6169 6e2f 7665 6e76 2f6c 6962  niChain/venv/lib
-00000430: 2f70 7974 686f 6e33 2e31 302f 7369 7465  /python3.10/site
-00000440: 2d70 6163 6b61 6765 732f 6d69 6e69 6368  -packages/minich
-00000450: 6169 6e2f 6261 7365 2e70 79da 075f 7072  ain/base.py.._pr
-00000460: 6f6d 7074 2600 0000 7306 0000 000a 0108  ompt&...s.......
-00000470: 0104 0272 2900 0000 da05 496e 7075 74da  ...r).....Input.
-00000480: 064f 7574 7075 74da 0846 6e4f 7574 7075  .Output..FnOutpu
-00000490: 74da 0178 6301 0000 0000 0000 0000 0000  t..xc...........
-000004a0: 0002 0000 0002 0000 0043 0000 0073 1200  .........C...s..
-000004b0: 0000 6401 6402 8400 7c00 4400 8301 7d01  ..d.d...|.D...}.
-000004c0: 7c01 5300 2903 4e63 0100 0000 0000 0000  |.S.).Nc........
-000004d0: 0000 0000 0200 0000 0400 0000 5300 0000  ............S...
-000004e0: 7316 0000 0069 007c 005d 077d 017c 016a  s....i.|.].}.|.j
-000004f0: 007c 016a 0193 0271 0253 0072 2700 0000  .|.j...q.S.r'...
-00000500: 2902 da04 6e61 6d65 da05 7661 6c75 6529  )...name..value)
-00000510: 02da 022e 30da 0165 7227 0000 0072 2700  ....0..er'...r'.
-00000520: 0000 7228 0000 00da 0a3c 6469 6374 636f  ..r(.....<dictco
-00000530: 6d70 3e33 0000 0073 0200 0000 1600 7a18  mp>3...s......z.
-00000540: 656e 756d 2e3c 6c6f 6361 6c73 3e2e 3c64  enum.<locals>.<d
-00000550: 6963 7463 6f6d 703e 7227 0000 0029 0272  ictcomp>r'...).r
-00000560: 2d00 0000 da01 6472 2700 0000 7227 0000  -.....dr'...r'..
-00000570: 0072 2800 0000 da04 656e 756d 3200 0000  .r(.....enum2...
-00000580: 7304 0000 000e 0104 0172 3400 0000 6301  s........r4...c.
-00000590: 0000 0000 0000 0000 0000 0001 0000 0004  ................
-000005a0: 0000 0043 0000 0073 6600 0000 7400 7401  ...C...sf...t.t.
-000005b0: 7c00 8301 6400 7500 7209 7c00 6e03 7401  |...d.u.r.|.n.t.
-000005c0: 7c00 8301 7402 8302 721a 6401 7403 7404  |...t...r.d.t.t.
-000005d0: 7c00 8301 6402 1900 8301 6403 9c02 5300  |...d.....d...S.
-000005e0: 7400 7c00 7405 8302 7223 7406 7c00 8301  t.|.t...r#t.|...
-000005f0: 5300 7407 7c00 8301 7230 6404 6405 8400  S.t.|...r0d.d...
-00000600: 7408 7c00 8301 4400 8301 5300 7c00 6a09  t.|...D...S.|.j.
-00000610: 5300 2906 4eda 046c 6973 7472 0100 0000  S.).N..listr....
-00000620: 2902 da03 5f74 5fda 0174 6301 0000 0000  )..._t_..tc.....
-00000630: 0000 0000 0000 0002 0000 0005 0000 0053  ...............S
-00000640: 0000 0073 1a00 0000 6900 7c00 5d09 7d01  ...s....i.|.].}.
-00000650: 7c01 6a00 7401 7c01 6a02 8301 9302 7102  |.j.t.|.j.....q.
-00000660: 5300 7227 0000 0029 0372 2e00 0000 da04  S.r'...).r......
-00000670: 7761 6c6b da04 7479 7065 2902 7230 0000  walk..type).r0..
-00000680: 00da 0179 7227 0000 0072 2700 0000 7228  ...yr'...r'...r(
-00000690: 0000 0072 3200 0000 3e00 0000 7302 0000  ...r2...>...s...
-000006a0: 001a 007a 1877 616c 6b2e 3c6c 6f63 616c  ...z.walk.<local
-000006b0: 733e 2e3c 6469 6374 636f 6d70 3e29 0ada  s>.<dictcomp>)..
-000006c0: 0a69 7373 7562 636c 6173 7372 1300 0000  .issubclassr....
-000006d0: 720c 0000 0072 3800 0000 7212 0000 0072  r....r8...r....r
-000006e0: 0600 0000 7234 0000 0072 0500 0000 7204  ....r4...r....r.
-000006f0: 0000 00da 085f 5f6e 616d 655f 5f29 0172  .....__name__).r
-00000700: 2d00 0000 7227 0000 0072 2700 0000 7228  -...r'...r'...r(
-00000710: 0000 0072 3800 0000 3700 0000 730e 0000  ...r8...7...s...
-00000720: 001e 0116 010a 0108 0108 0212 0106 0172  ...............r
-00000730: 3800 0000 da03 6f75 7463 0100 0000 0000  8.....outc......
-00000740: 0000 0000 0000 0300 0000 0400 0000 4300  ..............C.
-00000750: 0000 7320 0000 0074 00a0 0164 01a1 017d  ..s ...t...d...}
-00000760: 0174 027c 0083 017d 027c 01a0 0364 027c  .t.|...}.|...d.|
-00000770: 0269 01a1 0153 0029 034e 7a14 7479 7065  .i...S.).Nz.type
-00000780: 5f70 726f 6d70 742e 706d 7074 2e74 706c  _prompt.pmpt.tpl
-00000790: da03 7479 7029 04da 0365 6e76 da0c 6765  ..typ)...env..ge
-000007a0: 745f 7465 6d70 6c61 7465 7238 0000 00da  t_templater8....
-000007b0: 0672 656e 6465 7229 0372 3d00 0000 da03  .render).r=.....
-000007c0: 746d 7072 3300 0000 7227 0000 0072 2700  tmpr3...r'...r'.
-000007d0: 0000 7228 0000 00da 0e74 7970 655f 746f  ..r(.....type_to
-000007e0: 5f70 726f 6d70 7442 0000 0073 0600 0000  _promptB...s....
-000007f0: 0a01 0801 0e01 7243 0000 0063 0100 0000  ......rC...c....
-00000800: 0000 0000 0000 0000 0200 0000 0200 0000  ................
-00000810: 4b00 0000 7308 0000 007c 007c 0183 0153  K...s....|.|...S
-00000820: 0072 2400 0000 7227 0000 0029 02da 056d  .r$...r'...)...m
-00000830: 6f64 656c da06 6b77 6172 6773 7227 0000  odel..kwargsr'..
-00000840: 0072 2700 0000 7228 0000 00da 0673 696d  .r'...r(.....sim
-00000850: 706c 6548 0000 0073 0200 0000 0801 7246  pleH...s......rF
-00000860: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000870: 0000 0000 0300 0000 4000 0000 7322 0000  ........@...s"..
-00000880: 0065 005a 0164 005a 0255 0064 0165 0364  .e.Z.d.Z.U.d.e.d
-00000890: 023c 0065 0465 0519 0065 0364 033c 0064  .<.e.e...e.d.<.d
-000008a0: 0453 0029 05da 0748 6973 746f 7279 7a1f  .S.)...Historyz.
-000008b0: 5072 6f6d 7074 5b49 6e70 7574 2c20 4f75  Prompt[Input, Ou
-000008c0: 7470 7574 2c20 466e 4f75 7470 7574 5dda  tput, FnOutput].
-000008d0: 0670 726f 6d70 74da 0669 6e70 7574 734e  .prompt..inputsN
-000008e0: 2906 723c 0000 00da 0a5f 5f6d 6f64 756c  ).r<.....__modul
-000008f0: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-00000900: 5fda 0f5f 5f61 6e6e 6f74 6174 696f 6e73  _..__annotations
-00000910: 5f5f 720c 0000 0072 0800 0000 7227 0000  __r....r....r'..
-00000920: 0072 2700 0000 7227 0000 0072 2800 0000  .r'...r'...r(...
-00000930: 7247 0000 004c 0000 0073 0600 0000 0a00  rG...L...s......
-00000940: 0802 1001 7247 0000 0063 0000 0000 0000  ....rG...c......
-00000950: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
-00000960: 0000 7326 0000 0065 005a 0164 005a 0255  ..s&...e.Z.d.Z.U
-00000970: 0065 0365 0464 013c 0065 0565 0464 023c  .e.e.d.<.e.e.d.<
-00000980: 0064 0364 0484 005a 0664 0553 0029 06da  .d.d...Z.d.S.)..
-00000990: 0446 6169 6cda 0761 7267 5f6e 756d da04  .Fail..arg_num..
-000009a0: 6461 7461 6301 0000 0000 0000 0000 0000  datac...........
-000009b0: 0001 0000 0001 0000 0043 0000 0073 0400  .........C...s..
-000009c0: 0000 6401 5300 2902 4eda 0466 6169 6c72  ..d.S.).N..failr
-000009d0: 2700 0000 2901 da04 7365 6c66 7227 0000  '...)...selfr'..
-000009e0: 0072 2700 0000 7228 0000 00da 075f 5f73  .r'...r(.....__s
-000009f0: 7472 5f5f 5700 0000 7302 0000 0004 017a  tr__W...s......z
-00000a00: 0c46 6169 6c2e 5f5f 7374 725f 5f4e 2907  .Fail.__str__N).
-00000a10: 723c 0000 0072 4a00 0000 724b 0000 00da  r<...rJ...rK....
-00000a20: 0369 6e74 724c 0000 0072 0800 0000 7252  .intrL...r....rR
-00000a30: 0000 0072 2700 0000 7227 0000 0072 2700  ...r'...r'...r'.
-00000a40: 0000 7228 0000 0072 4d00 0000 5200 0000  ..r(...rM...R...
-00000a50: 7308 0000 000a 0008 0208 010c 0272 4d00  s............rM.
-00000a60: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00000a70: 0000 0007 0000 0040 0000 0073 3c00 0000  .......@...s<...
-00000a80: 6500 5a01 6400 5a02 5500 6503 6504 6401  e.Z.d.Z.U.e.e.d.
-00000a90: 3c00 640b 6404 6505 6405 6506 6406 6506  <.d.d.e.d.e.d.e.
-00000aa0: 6606 6407 6408 8405 5a07 6406 6506 6602  f.d.d...Z.d.e.f.
-00000ab0: 6409 640a 8404 5a08 6403 5300 290c da05  d.d...Z.d.S.)...
-00000ac0: 4368 6169 6eda 0768 6973 746f 7279 7201  Chain..historyr.
-00000ad0: 0000 004e da05 7472 6961 6c72 4f00 0000  ...N..trialrO...
-00000ae0: 7223 0000 0063 0300 0000 0000 0000 0000  r#...c..........
-00000af0: 0000 0800 0000 0500 0000 6300 0000 7308  ..........c...s.
-00000b00: 0100 0081 0067 007d 0367 007d 047c 006a  .....g.}.g.}.|.j
-00000b10: 006a 0144 005d 1d7d 057c 057d 0674 027c  .j.D.].}.|.}.t.|
-00000b20: 0574 0383 0272 1c7c 05a0 04a1 0044 005d  .t...r.|.....D.]
-00000b30: 057d 0664 0056 0001 0071 167c 03a0 057c  .}.d.V...q.|...|
-00000b40: 06a1 0101 007c 04a0 0564 01a1 0101 0071  .....|...d.....q
-00000b50: 097c 006a 006a 06a0 077c 037c 017c 02a1  .|.j.j...|.|.|..
-00000b60: 0344 005d 057d 0764 0056 0001 0071 3074  .D.].}.d.V...q0t
-00000b70: 027c 0774 0883 0272 7f7c 047c 076a 0905  .|.t...r.|.|.j..
-00000b80: 0019 0064 0237 0003 003c 007c 006a 006a  ...d.7...<.|.j.j
-00000b90: 017c 076a 0919 007d 0574 027c 0574 0383  .|.j...}.t.|.t..
-00000ba0: 0273 524a 0082 017c 056a 047c 047c 076a  .sRJ...|.j.|.|.j
-00000bb0: 0919 007c 076a 0a64 038d 0244 005d 057d  ...|.j.d...D.].}
-00000bc0: 0664 0056 0001 0071 5d7c 067c 037c 076a  .d.V...q]|.|.|.j
-00000bd0: 093c 007c 006a 006a 06a0 077c 037c 017c  .<.|.j.j...|.|.|
-00000be0: 02a1 0344 005d 057d 0764 0056 0001 0071  ...D.].}.d.V...q
-00000bf0: 7164 0056 0001 0074 027c 0774 0883 0273  qd.V...t.|.t...s
-00000c00: 3b7c 0756 0001 0064 0053 0029 044e 7201  ;|.V...d.S.).Nr.
-00000c10: 0000 0072 1a00 0000 2902 7256 0000 0072  ...r....).rV...r
-00000c20: 4f00 0000 290b 7255 0000 0072 4900 0000  O...).rU...rI...
-00000c30: 7225 0000 0072 5400 0000 da07 7275 6e5f  r%...rT.....run_
-00000c40: 6765 6eda 0661 7070 656e 6472 4800 0000  gen..appendrH...
-00000c50: da06 6578 7061 6e64 724d 0000 0072 4e00  ..expandrM...rN.
-00000c60: 0000 724f 0000 0029 0872 5100 0000 7256  ..rO...).rQ...rV
-00000c70: 0000 0072 4f00 0000 da04 6172 6773 7207  ...rO.....argsr.
-00000c80: 0000 00da 0369 6e70 da04 696e 7032 723d  .....inp..inp2r=
-00000c90: 0000 0072 2700 0000 7227 0000 0072 2800  ...r'...r'...r(.
-00000ca0: 0000 7257 0000 0060 0000 0073 3000 0000  ..rW...`...s0...
-00000cb0: 0280 0401 0401 0c01 0401 0a01 0c01 0801  ................
-00000cc0: 0a01 0c01 1601 0801 0a01 1201 0e01 0e01  ................
-00000cd0: 1a01 0801 0a01 1601 0801 0601 0af7 0a0b  ................
-00000ce0: 7a0d 4368 6169 6e2e 7275 6e5f 6765 6e63  z.Chain.run_genc
-00000cf0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00000d00: 0300 0000 4300 0000 7322 0000 007c 00a0  ....C...s"...|..
-00000d10: 00a1 0044 005d 0a7d 017c 0164 0075 0172  ...D.].}.|.d.u.r
-00000d20: 0e7c 0102 0001 0053 0071 0464 0053 0072  .|.....S.q.d.S.r
-00000d30: 2400 0000 2901 7257 0000 0029 0272 5100  $...).rW...).rQ.
-00000d40: 0000 722d 0000 0072 2700 0000 7227 0000  ..r-...r'...r'..
-00000d50: 0072 2800 0000 da03 7275 6e79 0000 0073  .r(.....runy...s
-00000d60: 0a00 0000 0c01 0801 0801 02ff 04ff 7a09  ..............z.
-00000d70: 4368 6169 6e2e 7275 6ea9 0272 0100 0000  Chain.run..r....
-00000d80: 4e29 0972 3c00 0000 724a 0000 0072 4b00  N).r<...rJ...rK.
-00000d90: 0000 7247 0000 0072 4c00 0000 7253 0000  ..rG...rL...rS..
-00000da0: 0072 0800 0000 7257 0000 0072 5d00 0000  .r....rW...r]...
-00000db0: 7227 0000 0072 2700 0000 7227 0000 0072  r'...r'...r'...r
-00000dc0: 2800 0000 7254 0000 005b 0000 0073 0800  (...rT...[...s..
-00000dd0: 0000 0a00 0803 1802 1219 7254 0000 0063  ..........rT...c
-00000de0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000df0: 1000 0000 4000 0000 7312 0100 0065 005a  ....@...s....e.Z
-00000e00: 0164 005a 0265 0383 005a 0465 0564 0164  .d.Z.e...Z.e.d.d
-00000e10: 0264 0266 0464 0365 0664 0465 0765 0865  .d.f.d.e.d.e.e.e
-00000e20: 0965 0867 0165 0a66 0219 0066 0219 0064  .e.g.e.f...f...d
-00000e30: 0565 0b65 0819 0064 0665 0b65 0819 0064  .e.e...d.e.e...d
-00000e40: 0765 0b65 0819 0064 0865 0965 0965 0c67  .e.e...d.e.e.e.g
-00000e50: 0165 0a66 0219 0067 0165 0d66 0219 0064  .e.f...g.e.f...d
-00000e60: 0965 0e66 0e64 0a64 0b84 055a 0f64 0c65  .e.f.d.d...Z.d.e
-00000e70: 0864 0d65 1066 0464 0e64 0f84 045a 1109  .d.e.f.d.d...Z..
-00000e80: 0164 2064 1065 0765 0865 1266 0219 0064  .d d.e.e.e.f...d
-00000e90: 0d65 1365 1265 0865 0a66 0319 0066 0464  .e.e.e.e.f...f.d
-00000ea0: 1164 1284 055a 1409 0164 2064 1065 0765  .d...Z...d d.e.e
-00000eb0: 0865 1266 0219 0064 0d65 1365 1265 0865  .e.f...d.e.e.e.e
-00000ec0: 0a66 0319 0066 0464 1364 1484 055a 1564  .f...f.d.d...Z.d
-00000ed0: 1565 1064 0d65 1266 0464 1664 1784 045a  .e.d.e.f.d.d...Z
-00000ee0: 1664 1865 1064 0d65 0d66 0464 1964 1a84  .d.e.d.e.f.d.d..
-00000ef0: 045a 1747 0064 1b64 1c84 0064 1c83 025a  .Z.G.d.d...d...Z
-00000f00: 1864 2164 1e64 1f84 015a 1964 0253 0029  .d!d.d...Z.d.S.)
-00000f10: 22da 0650 726f 6d70 7446 4eda 0762 6163  "..PromptFN..bac
-00000f20: 6b65 6e64 da06 7061 7273 6572 da0d 7465  kend..parser..te
-00000f30: 6d70 6c61 7465 5f66 696c 65da 0874 656d  mplate_file..tem
-00000f40: 706c 6174 65da 0d73 746f 705f 7465 6d70  plate..stop_temp
-00000f50: 6c61 7465 da02 666e da06 7374 7265 616d  late..fn..stream
-00000f60: 630a 0000 0000 0000 0000 0000 000a 0000  c...............
-00000f70: 0003 0000 0043 0000 0073 6400 0000 7c01  .....C...sd...|.
-00000f80: 7c00 5f00 7c07 7c00 5f01 7402 7c01 6401  |._.|.|._.t.|.d.
-00000f90: 8302 720e 7c01 6a03 6e01 6402 7c00 5f03  ..r.|.j.n.d.|._.
-00000fa0: 7c02 7c00 5f04 7c03 7c00 5f05 7c04 7c00  |.|._.|.|._.|.|.
-00000fb0: 5f06 7c05 7c00 5f07 7c08 7c00 5f08 7c09  _.|.|._.|.|._.|.
-00000fc0: 7c00 5f09 7c06 7c00 5f0a 7c06 6a0b 7c00  |._.|.|._.|.j.|.
-00000fd0: 5f0c 740d 6a0e a00f a100 7c00 5f10 6400  _.t.j.....|._.d.
-00000fe0: 5300 2903 4eda 0b64 6573 6372 6970 7469  S.).N..descripti
-00000ff0: 6f6e da00 2911 7260 0000 0072 6600 0000  on..).r`...rf...
-00001000: da07 6861 7361 7474 7272 6700 0000 7261  ..hasattrrg...ra
-00001010: 0000 0072 6200 0000 7263 0000 0072 6400  ...rb...rc...rd.
-00001020: 0000 da0b 626c 6f63 6b5f 696e 7075 74da  ....block_input.
-00001030: 0c62 6c6f 636b 5f6f 7574 7075 7472 6500  .block_outputre.
-00001040: 0000 723c 0000 00da 035f 666e 725f 0000  ..r<....._fnr_..
-00001050: 00da 0763 6f75 6e74 6572 da08 5f5f 6e65  ...counter..__ne
-00001060: 7874 5f5f da03 5f69 6429 0a72 5100 0000  xt__.._id).rQ...
-00001070: 7260 0000 0072 6100 0000 7262 0000 0072  r`...ra...rb...r
-00001080: 6300 0000 7264 0000 0072 6500 0000 7266  c...rd...re...rf
-00001090: 0000 0072 6a00 0000 726b 0000 0072 2700  ...rj...rk...r'.
-000010a0: 0000 7227 0000 0072 2800 0000 da08 5f5f  ..r'...r(.....__
-000010b0: 696e 6974 5f5f 8200 0000 731a 0000 0006  init__....s.....
-000010c0: 0c06 0112 0204 ff06 0306 0106 0106 0106  ................
-000010d0: 0106 0106 0108 0110 017a 0f50 726f 6d70  .........z.Promp
-000010e0: 742e 5f5f 696e 6974 5f5f da08 7265 7370  t.__init__..resp
-000010f0: 6f6e 7365 7223 0000 0063 0200 0000 0000  onser#...c......
-00001100: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
-00001110: 0000 733c 0000 0074 007c 006a 0174 0283  ..s<...t.|.j.t..
-00001120: 0272 197c 006a 0164 016b 0272 0d7c 0153  .r.|.j.d.k.r.|.S
-00001130: 007c 006a 0164 026b 0272 1774 03a0 047c  .|.j.d.k.r.t...|
-00001140: 01a1 0153 0064 0353 007c 00a0 017c 01a1  ...S.d.S.|...|..
-00001150: 0153 0029 047a 5e0a 2020 2020 2020 2020  .S.).z^.        
-00001160: 436f 6e76 6572 7420 6672 6f6d 2074 6865  Convert from the
-00001170: 2073 7472 696e 6720 7265 7370 6f6e 7365   string response
-00001180: 206f 6620 7468 6520 6675 6e63 7469 6f6e   of the function
-00001190: 0a20 2020 2020 2020 2074 6f20 7468 6520  .        to the 
-000011a0: 6f75 7470 7574 2074 7970 652e 0a20 2020  output type..   
-000011b0: 2020 2020 2072 2600 0000 da04 6a73 6f6e       r&.....json
-000011c0: 4e29 0572 2500 0000 7261 0000 0072 2600  N).r%...ra...r&.
-000011d0: 0000 7272 0000 00da 056c 6f61 6473 2902  ..rr.....loads).
-000011e0: 7251 0000 0072 7100 0000 7227 0000 0072  rQ...rq...r'...r
-000011f0: 2700 0000 7228 0000 00da 0570 6172 7365  '...r(.....parse
-00001200: 9d00 0000 730e 0000 000c 050a 0104 010a  ....s...........
-00001210: 010a 0104 ff0a 037a 0c50 726f 6d70 742e  .......z.Prompt.
-00001220: 7061 7273 6572 2200 0000 6303 0000 0000  parser"...c.....
-00001230: 0000 0000 0000 0006 0000 0009 0000 0043  ...............C
-00001240: 0000 0073 d200 0000 7400 7401 7c00 6a02  ...s....t.t.|.j.
-00001250: 8301 6401 8d01 8f4d 0100 7403 7c01 8301  ..d....M..t.|...
-00001260: 7d03 7400 6402 7c03 6a04 6403 8d02 8f17  }.t.d.|.j.d.....
-00001270: 0100 7c00 6a05 a006 7407 7c00 6a05 6404  ..|.j...t.|.j.d.
-00001280: 8302 7220 7c03 6e02 7c03 6a04 a101 7d04  ..r |.n.|.j...}.
-00001290: 5700 6400 0400 0400 8303 0100 6e08 3100  W.d.........n.1.
-000012a0: 732e 7701 0100 0100 0100 5900 0100 7400  s.w.......Y...t.
-000012b0: 6405 7c04 6406 8d02 8f0d 0100 7c00 a008  d.|.d.......|...
-000012c0: 7c04 a101 7d05 5700 6400 0400 0400 8303  |...}.W.d.......
-000012d0: 0100 6e08 3100 7349 7701 0100 0100 0100  ..n.1.sIw.......
-000012e0: 5900 0100 5700 6400 0400 0400 8303 0100  Y...W.d.........
-000012f0: 6e08 3100 7358 7701 0100 0100 0100 5900  n.1.sXw.......Y.
-00001300: 0100 7409 7c04 7401 8302 7364 6407 7d04  ..t.|.t...sdd.}.
-00001310: 7c03 7c04 7c05 6603 5300 2908 4e29 01da  |.|.|.f.S.).N)..
-00001320: 0b61 6374 696f 6e5f 7479 7065 da08 5072  .action_type..Pr
-00001330: 6f6d 7074 6564 2902 7275 0000 0072 4800  ompted).ru...rH.
-00001340: 0000 da0d 6e65 6564 735f 7265 7175 6573  ....needs_reques
-00001350: 74da 0852 6573 706f 6e73 6529 0272 7500  t..Response).ru.
-00001360: 0000 da06 7265 7375 6c74 7a06 2864 6174  ....resultz.(dat
-00001370: 6129 290a 7214 0000 0072 2600 0000 7265  a)).r....r&...re
-00001380: 0000 0072 2900 0000 7248 0000 0072 6000  ...r)...rH...r`.
-00001390: 0000 725d 0000 0072 6900 0000 7274 0000  ..r]...ri...rt..
-000013a0: 0072 2500 0000 2906 7251 0000 0072 2200  .r%...).rQ...r".
-000013b0: 0000 7266 0000 00da 0772 6571 7565 7374  ..rf.....request
-000013c0: 7271 0000 00da 066f 7574 7075 7472 2700  rq.....outputr'.
-000013d0: 0000 7227 0000 0072 2800 0000 da0b 7275  ..r'...r(.....ru
-000013e0: 6e5f 7665 7262 6f73 65aa 0000 0073 2200  n_verbose....s".
-000013f0: 0000 1203 0801 1001 0601 0a02 06ff 0402  ................
-00001400: 06fd 1cff 0e06 0c01 1cff 0280 1cf8 0a0a  ................
-00001410: 0401 0a01 7a12 5072 6f6d 7074 2e72 756e  ....z.Prompt.run
-00001420: 5f76 6572 626f 7365 6303 0000 0000 0000  _verbosec.......
-00001430: 0000 0000 0004 0000 0005 0000 0063 0000  .............c..
-00001440: 0073 3e00 0000 8100 7400 7c01 8301 7d03  .s>.....t.|...}.
-00001450: 7c00 6a01 a002 7403 7c00 6a01 6401 8302  |.j...t.|.j.d...
-00001460: 7210 7c03 6e02 7c03 6a04 a101 4400 5d08  r.|.n.|.j...D.].
-00001470: 7d01 7c03 7c01 7c01 6603 5600 0100 7114  }.|.|.|.f.V...q.
-00001480: 6400 5300 2902 4e72 7700 0000 2905 7229  d.S.).Nrw...).r)
-00001490: 0000 0072 6000 0000 da0a 7275 6e5f 7374  ...r`.....run_st
-000014a0: 7265 616d 7269 0000 0072 4800 0000 2904  reamri...rH...).
-000014b0: 7251 0000 0072 2200 0000 7266 0000 0072  rQ...r"...rf...r
-000014c0: 7a00 0000 7227 0000 0072 2700 0000 7228  z...r'...r'...r(
-000014d0: 0000 0072 7d00 0000 bb00 0000 730e 0000  ...r}.......s...
-000014e0: 0002 8008 0306 0114 0108 ff0e 0304 fd7a  ...............z
-000014f0: 1150 726f 6d70 742e 7275 6e5f 7374 7265  .Prompt.run_stre
-00001500: 616d 725b 0000 0063 0200 0000 0000 0000  amr[...c........
-00001510: 0000 0000 0600 0000 0400 0000 4300 0000  ............C...
-00001520: 7372 0000 007c 017d 027c 006a 0072 1274  sr...|.}.|.j.r.t
-00001530: 0174 0264 0183 0164 028d 016a 037c 006a  .t.d...d...j.|.j
-00001540: 0064 038d 017d 036e 087c 006a 0472 1a74  .d...}.n.|.j.r.t
-00001550: 057c 006a 0483 017d 037c 036a 0664 0469  .|.j...}.|.j.d.i
-00001560: 007c 02a4 018e 017d 047c 006a 0772 3274  .|.....}.|.j.r2t
-00001570: 057c 006a 0783 016a 0664 0469 007c 02a4  .|.j...j.d.i.|..
-00001580: 018e 0167 017d 056e 0264 007d 0574 087c  ...g.}.n.d.}.t.|
-00001590: 047c 0583 0253 0029 054e da01 2e29 0172  .|...S.).N...).r
-000015a0: 1f00 0000 2901 722e 0000 0072 2700 0000  ....).r....r'...
-000015b0: 2909 7262 0000 0072 1500 0000 7216 0000  ).rb...r....r...
-000015c0: 0072 4000 0000 7263 0000 0072 1800 0000  .r@...rc...r....
-000015d0: 7241 0000 0072 6400 0000 721d 0000 0029  rA...rd...r....)
-000015e0: 0672 5100 0000 725b 0000 0072 4500 0000  .rQ...r[...rE...
-000015f0: 7242 0000 0072 2d00 0000 da04 7374 6f70  rB...r-.....stop
-00001600: 7227 0000 0072 2700 0000 7228 0000 00da  r'...r'...r(....
-00001610: 0d74 656d 706c 6174 655f 6669 6c6c c400  .template_fill..
-00001620: 0000 7318 0000 0004 0106 010e 0104 0108  ..s.............
-00001630: ff06 030a 0110 0206 021a 0104 020a 017a  ...............z
-00001640: 1450 726f 6d70 742e 7465 6d70 6c61 7465  .Prompt.template
-00001650: 5f66 696c 6c72 5a00 0000 6301 0000 0000  _fillrZ...c.....
-00001660: 0000 0000 0000 0002 0000 0004 0000 0047  ...............G
-00001670: 0000 0073 0e00 0000 7400 7401 7c00 7c01  ...s....t.t.|.|.
-00001680: 8302 8301 5300 7224 0000 0029 0272 5400  ....S.r$...).rT.
-00001690: 0000 7247 0000 0029 0272 5100 0000 725a  ..rG...).rQ...rZ
-000016a0: 0000 0072 2700 0000 7227 0000 0072 2800  ...r'...r'...r(.
-000016b0: 0000 da08 5f5f 6361 6c6c 5f5f d500 0000  ....__call__....
-000016c0: f302 0000 000e 017a 0f50 726f 6d70 742e  .......z.Prompt.
-000016d0: 5f5f 6361 6c6c 5f5f 6300 0000 0000 0000  __call__c.......
-000016e0: 0000 0000 0000 0000 0007 0000 0040 0000  .............@..
-000016f0: 0073 3c00 0000 6500 5a01 6400 5a02 6401  .s<...e.Z.d.Z.d.
-00001700: 6402 8400 5a03 640d 6404 6504 6405 6505  d...Z.d.d.e.d.e.
-00001710: 6406 6506 6606 6407 6408 8405 5a07 6409  d.e.f.d.d...Z.d.
-00001720: 640a 8400 5a08 640b 640c 8400 5a09 6403  d...Z.d.d...Z.d.
-00001730: 5300 290e 7a0c 5072 6f6d 7074 2e4d 6f64  S.).z.Prompt.Mod
-00001740: 656c 6304 0000 0000 0000 0000 0000 0004  elc.............
-00001750: 0000 0002 0000 0043 0000 0073 1c00 0000  .......C...s....
-00001760: 7c01 7c00 5f00 7c02 7c00 5f01 7c03 7c00  |.|._.|.|._.|.|.
-00001770: 5f02 6400 7c00 5f03 6400 5300 7224 0000  _.d.|._.d.S.r$..
-00001780: 0029 0472 4800 0000 7256 0000 0072 4f00  .).rH...rV...rO.
-00001790: 0000 da07 7275 6e5f 6c6f 6729 0472 5100  ....run_log).rQ.
-000017a0: 0000 7248 0000 0072 5600 0000 724f 0000  ..rH...rV...rO..
-000017b0: 0072 2700 0000 7227 0000 0072 2800 0000  .r'...r'...r(...
-000017c0: 7270 0000 00d9 0000 0073 0800 0000 0601  rp.......s......
-000017d0: 0601 0601 0a01 7a15 5072 6f6d 7074 2e4d  ......z.Prompt.M
-000017e0: 6f64 656c 2e5f 5f69 6e69 745f 5f4e da06  odel.__init__N..
-000017f0: 6172 676e 756d 724f 0000 0072 2300 0000  argnumrO...r#...
-00001800: 6303 0000 0000 0000 0000 0000 0003 0000  c...............
-00001810: 0003 0000 0043 0000 0073 0e00 0000 7400  .....C...s....t.
-00001820: 7c01 6401 1800 7c02 8302 5300 2902 4e72  |.d...|...S.).Nr
-00001830: 1a00 0000 2901 724d 0000 0029 0372 5100  ....).rM...).rQ.
-00001840: 0000 7284 0000 0072 4f00 0000 7227 0000  ..r....rO...r'..
-00001850: 0072 2700 0000 7228 0000 0072 5000 0000  .r'...r(...rP...
-00001860: df00 0000 7282 0000 007a 1150 726f 6d70  ....r....z.Promp
-00001870: 742e 4d6f 6465 6c2e 6661 696c 6302 0000  t.Model.failc...
-00001880: 0000 0000 0000 0000 0003 0000 0003 0000  ................
-00001890: 0043 0000 0073 1400 0000 7c00 a000 7c01  .C...s....|...|.
-000018a0: a101 4400 5d02 7d02 7105 7c02 5300 7224  ..D.].}.q.|.S.r$
-000018b0: 0000 0029 0172 6600 0000 2903 7251 0000  ...).rf...).rQ..
-000018c0: 00da 0669 6e70 7574 5f72 2200 0000 7227  ...input_r"...r'
-000018d0: 0000 0072 2700 0000 7228 0000 0072 8100  ...r'...r(...r..
-000018e0: 0000 e200 0000 7306 0000 000e 0102 0104  ......s.........
-000018f0: 017a 1550 726f 6d70 742e 4d6f 6465 6c2e  .z.Prompt.Model.
-00001900: 5f5f 6361 6c6c 5f5f 6302 0000 0000 0000  __call__c.......
-00001910: 0000 0000 0006 0000 0005 0000 0063 0000  .............c..
-00001920: 0073 0401 0000 8100 7c00 6a00 6400 7500  .s......|.j.d.u.
-00001930: 730a 4a00 6401 8301 8201 7c00 6a01 6a02  s.J.d.....|.j.j.
-00001940: 6400 7501 7316 7c00 6a01 6a03 6400 7501  d.u.s.|.j.j.d.u.
-00001950: 7237 7404 7c01 7405 8302 731f 7406 7c01  r7t.|.t...s.t.|.
-00001960: 8301 7d01 7405 640a 6900 7c01 a401 8e01  ..}.t.d.i.|.....
-00001970: 7d01 7c00 6a07 7c01 6402 3c00 7c00 6a08  }.|.j.|.d.<.|.j.
-00001980: 7c01 6403 3c00 7c00 6a01 a009 7c01 a101  |.d.<.|.j...|...
-00001990: 7d02 6e02 7c01 7d02 7c00 6a01 6a0a 7268  }.n.|.}.|.j.j.rh
-000019a0: 740b 7c00 6a01 6a0c 6404 8302 7268 6405  t.|.j.j.d...rhd.
-000019b0: 7c00 5f00 7c00 6a01 a00d 7c02 a101 4400  |._.|.j...|...D.
-000019c0: 5d18 5c03 7d03 7d04 7d05 7c03 7c00 6a00  ].\.}.}.}.|.|.j.
-000019d0: 6406 1900 7c04 1700 7c00 6a00 6407 1900  d...|...|.j.d...
-000019e0: 7c05 1700 6603 7c00 5f00 7c05 5600 0100  |...f.|._.|.V...
-000019f0: 714d 6400 5300 740e 7c01 8301 6408 6408  qMd.S.t.|...d.d.
-00001a00: 6603 7c00 5f00 6400 5600 0100 7c00 6a01  f.|._.d.V...|.j.
-00001a10: a00f 7c02 a101 7c00 5f00 7c00 6a00 6409  ..|...|._.|.j.d.
-00001a20: 1900 5600 0100 6400 5300 290b 4e7a 234f  ..V...d.S.).Nz#O
-00001a30: 6e6c 7920 6361 6c6c 2060 6d6f 6465 6c60  nly call `model`
-00001a40: 206f 6e63 6520 7065 7220 6675 6e63 7469   once per functi
-00001a50: 6f6e da06 5f74 7269 616c da0a 5f66 6169  on.._trial.._fai
-00001a60: 6c5f 6461 7461 727d 0000 0029 0372 6800  l_datar}...).rh.
-00001a70: 0000 7268 0000 0072 6800 0000 721a 0000  ..rh...rh...r...
-00001a80: 00e9 0200 0000 7268 0000 00e9 ffff ffff  ......rh........
-00001a90: 7227 0000 0029 1072 8300 0000 7248 0000  r'...).r....rH..
-00001aa0: 0072 6300 0000 7262 0000 0072 2500 0000  .rc...rb...r%...
-00001ab0: da04 6469 6374 7202 0000 0072 5600 0000  ..dictr....rV...
-00001ac0: 724f 0000 0072 8000 0000 7266 0000 0072  rO...r....rf...r
-00001ad0: 6900 0000 7260 0000 0072 7d00 0000 721d  i...r`...r}...r.
-00001ae0: 0000 0072 7c00 0000 2906 7251 0000 0072  ...r|...).rQ...r
-00001af0: 8500 0000 7279 0000 00da 0161 da01 62da  ....ry.....a..b.
-00001b00: 0163 7227 0000 0072 2700 0000 7228 0000  .cr'...r'...r(..
-00001b10: 0072 6600 0000 e700 0000 732e 0000 0002  .rf.......s.....
-00001b20: 8012 010a 0202 ff0a 0202 fe0a 0408 010e  ................
-00001b30: 010a 010a 010e 0204 0216 0106 0116 0120  ............... 
-00001b40: 0108 0104 fe10 0406 010e 0110 017a 1350  .............z.P
-00001b50: 726f 6d70 742e 4d6f 6465 6c2e 7374 7265  rompt.Model.stre
-00001b60: 616d 7224 0000 0029 0a72 3c00 0000 724a  amr$...).r<...rJ
-00001b70: 0000 0072 4b00 0000 7270 0000 0072 5300  ...rK...rp...rS.
-00001b80: 0000 7208 0000 0072 4d00 0000 7250 0000  ..r....rM...rP..
-00001b90: 0072 8100 0000 7266 0000 0072 2700 0000  .r....rf...r'...
-00001ba0: 7227 0000 0072 2700 0000 7228 0000 00da  r'...r'...r(....
-00001bb0: 054d 6f64 656c d800 0000 730a 0000 0008  .Model....s.....
-00001bc0: 0008 0118 0608 030c 0572 8e00 0000 7201  .........r....r.
-00001bd0: 0000 0063 0400 0000 0000 0000 0000 0000  ...c............
-00001be0: 0900 0000 0600 0000 6300 0000 736a 0100  ........c...sj..
-00001bf0: 0081 0074 006a 01a0 027c 006a 0364 01a1  ...t.j...|.j.d..
-00001c00: 0201 007c 0264 026b 0272 1774 006a 017c  ...|.d.k.r.t.j.|
-00001c10: 006a 0305 0019 0064 0337 0003 003c 0074  .j.....d.7...<.t
-00001c20: 006a 017c 006a 0319 007d 0474 006a 04a0  .j.|.j...}.t.j..
-00001c30: 027c 006a 037c 0466 0267 00a1 0201 0074  .|.j.|.f.g.....t
-00001c40: 006a 047c 006a 037c 0466 0219 00a0 0564  .j.|.j.|.f.....d
-00001c50: 0474 0664 0483 0164 0464 0466 04a1 0101  .t.d...d.d.f....
-00001c60: 007c 00a0 077c 007c 027c 03a1 037d 057c  .|...|.|.|...}.|
-00001c70: 006a 0872 827c 006a 097c 0567 017c 01a2  .j.r.|.j.|.g.|..
-00001c80: 0152 008e 0044 005d 357d 067c 056a 0a7d  .R...D.]5}.|.j.}
-00001c90: 077c 056a 0a73 594a 0074 0b7c 0583 0183  .|.j.sYJ.t.|....
-00001ca0: 0182 017c 017c 0764 0219 007c 0764 0319  ...|.|.d...|.d..
-00001cb0: 007c 0666 047d 0874 006a 017c 006a 0319  .|.f.}.t.j.|.j..
-00001cc0: 007d 0474 006a 04a0 027c 006a 037c 0466  .}.t.j...|.j.|.f
-00001cd0: 0267 00a1 0201 007c 0874 006a 047c 006a  .g.....|.t.j.|.j
-00001ce0: 037c 0466 0219 0064 013c 0064 0056 0001  .|.f...d.<.d.V..
-00001cf0: 0071 4b6e 097c 006a 097c 0567 017c 01a2  .qKn.|.j.|.g.|..
-00001d00: 0152 008e 007d 0674 0c7c 0674 0d83 0273  .R...}.t.|.t...s
-00001d10: b07c 056a 0a73 994a 0074 0b7c 0583 0183  .|.j.s.J.t.|....
-00001d20: 0182 017c 056a 0a7d 077c 017c 0764 0219  ...|.j.}.|.|.d..
-00001d30: 007c 0764 0319 007c 0666 047d 087c 0874  .|.d...|.f.}.|.t
-00001d40: 006a 047c 006a 037c 0466 0219 0064 013c  .j.|.j.|.f...d.<
-00001d50: 007c 0656 0001 0064 0053 0029 054e 7289  .|.V...d.S.).Nr.
-00001d60: 0000 0072 0100 0000 721a 0000 0072 6800  ...r....r....rh.
-00001d70: 0000 290e 721c 0000 00da 0c70 726f 6d70  ..).r......promp
-00001d80: 745f 636f 756e 74da 0a73 6574 6465 6661  t_count..setdefa
-00001d90: 756c 7472 6f00 0000 da0c 7072 6f6d 7074  ultro.....prompt
-00001da0: 5f73 746f 7265 7258 0000 0072 1d00 0000  _storerX...r....
-00001db0: 728e 0000 0072 6600 0000 7265 0000 0072  r....rf...re...r
-00001dc0: 8300 0000 7226 0000 0072 2500 0000 724d  ....r&...r%...rM
-00001dd0: 0000 0029 0972 5100 0000 725a 0000 0072  ...).rQ...rZ...r
-00001de0: 5600 0000 724f 0000 0072 0700 0000 7244  V...rO...r....rD
-00001df0: 0000 0072 7b00 0000 7237 0000 0072 8300  ...r{...r7...r..
-00001e00: 0000 7227 0000 0072 2700 0000 7228 0000  ..r'...r'...r(..
-00001e10: 0072 5900 0000 0101 0000 7332 0000 0002  .rY.......s2....
-00001e20: 8010 0108 0114 010c 0114 0122 010e 0206  ..........."....
-00001e30: 0216 0106 0212 0114 010c 0114 0114 0108  ................
-00001e40: 0102 f812 0a0a 0212 0106 0114 0114 010a  ................
-00001e50: 027a 0d50 726f 6d70 742e 6578 7061 6e64  .z.Prompt.expand
-00001e60: 2901 4672 5e00 0000 291a 723c 0000 0072  ).Fr^...).r<...r
-00001e70: 4a00 0000 724b 0000 0072 0700 0000 726d  J...rK...r....rm
-00001e80: 0000 0072 4600 0000 721b 0000 0072 1100  ...rF...r....r..
-00001e90: 0000 7226 0000 0072 0900 0000 722b 0000  ..r&...r....r+..
-00001ea0: 0072 0d00 0000 722a 0000 0072 2c00 0000  .r....r*...r,...
-00001eb0: da04 626f 6f6c 7270 0000 0072 0800 0000  ..boolrp...r....
-00001ec0: 7274 0000 0072 1d00 0000 720e 0000 0072  rt...r....r....r
-00001ed0: 7c00 0000 727d 0000 0072 8000 0000 7281  |...r}...r....r.
-00001ee0: 0000 0072 8e00 0000 7259 0000 0072 2700  ...r....rY...r'.
-00001ef0: 0000 7227 0000 0072 2700 0000 7228 0000  ..r'...r'...r(..
-00001f00: 0072 5f00 0000 7f00 0000 734c 0000 0008  .r_.......sL....
-00001f10: 0006 0102 0902 0102 0102 0104 f602 0202  ................
-00001f20: fe14 0302 fd06 0402 fc06 0502 fb06 0602  ................
-00001f30: fa16 0702 f902 080a f812 1b02 0e04 ff0a  ................
-00001f40: 0102 ff0c 020a fe02 1204 ff0a 0102 ff0c  ................
-00001f50: 020a fe12 0912 110e 030e 2972 5f00 0000  ..........)r_...
-00001f60: 7226 0000 0046 7260 0000 0072 6100 0000  r&...Fr`...ra...
-00001f70: 7262 0000 0072 6300 0000 7264 0000 0072  rb...rc...rd...r
-00001f80: 6600 0000 6308 0000 0000 0000 0000 0000  f...c...........
-00001f90: 0008 0000 0008 0000 0003 0000 0073 1a00  .............s..
-00001fa0: 0000 8700 8701 8702 8703 8704 8705 8706  ................
-00001fb0: 8707 6608 6401 6402 8408 5300 2903 4e63  ..f.d.d...S.).Nc
-00001fc0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00001fd0: 0a00 0000 1300 0000 7318 0000 0074 0088  ........s....t..
-00001fe0: 0088 0388 0788 0688 047c 0088 0588 0188  .........|......
-00001ff0: 0283 0953 0072 2400 0000 2901 725f 0000  ...S.r$...).r_..
-00002000: 0029 0172 6500 0000 a908 7260 0000 0072  .).re.....r`...r
-00002010: 6a00 0000 726b 0000 0072 6100 0000 7264  j...rk...ra...rd
-00002020: 0000 0072 6600 0000 7263 0000 0072 6200  ...rf...rc...rb.
-00002030: 0000 7227 0000 0072 2800 0000 da08 3c6c  ..r'...r(.....<l
-00002040: 616d 6264 613e 2b01 0000 7316 0000 0002  ambda>+...s.....
-00002050: 0002 0102 0102 0102 0102 0102 0102 0102  ................
-00002060: 0102 0104 f77a 1870 726f 6d70 742e 3c6c  .....z.prompt.<l
-00002070: 6f63 616c 733e 2e3c 6c61 6d62 6461 3e72  ocals>.<lambda>r
-00002080: 2700 0000 2908 7260 0000 0072 6100 0000  '...).r`...ra...
-00002090: 7262 0000 0072 6300 0000 7264 0000 0072  rb...rc...rd...r
-000020a0: 6600 0000 726a 0000 0072 6b00 0000 7227  f...rj...rk...r'
-000020b0: 0000 0072 9300 0000 7228 0000 0072 4800  ...r....r(...rH.
-000020c0: 0000 2101 0000 7302 0000 001a 0a72 4800  ..!...s......rH.
-000020d0: 0000 2907 7226 0000 004e 4e4e 464e 4e29  ..).r&...NNNFNN)
-000020e0: 3472 7200 0000 da0b 6461 7461 636c 6173  4rr.....dataclas
-000020f0: 7365 7372 0200 0000 7203 0000 0072 0400  sesr....r....r..
-00002100: 0000 7205 0000 0072 3400 0000 7206 0000  ..r....r4...r...
-00002110: 00da 0969 7465 7274 6f6f 6c73 7207 0000  ...itertoolsr...
-00002120: 00da 0674 7970 696e 6772 0800 0000 7209  ...typingr....r.
-00002130: 0000 0072 0a00 0000 720b 0000 0072 0c00  ...r....r....r..
-00002140: 0000 720d 0000 0072 0e00 0000 720f 0000  ..r....r....r...
-00002150: 0072 1000 0000 7211 0000 0072 1200 0000  .r....r....r....
-00002160: 7213 0000 00da 0565 6c69 6f74 7214 0000  r......eliotr...
-00002170: 00da 066a 696e 6a61 3272 1500 0000 7216  ...jinja2r....r.
-00002180: 0000 0072 1700 0000 7218 0000 0072 1900  ...r....r....r..
-00002190: 0000 7260 0000 0072 1b00 0000 721c 0000  ..r`...r....r...
-000021a0: 0072 1d00 0000 723f 0000 0072 2600 0000  .r....r?...r&...
-000021b0: 7229 0000 0072 2a00 0000 722b 0000 0072  r)...r*...r+...r
-000021c0: 2c00 0000 7253 0000 0072 3800 0000 7239  ,...rS...r8...r9
-000021d0: 0000 0072 4300 0000 7246 0000 0072 4700  ...rC...rF...rG.
-000021e0: 0000 724d 0000 0072 5400 0000 725f 0000  ..rM...rT...r_..
-000021f0: 0072 9200 0000 7248 0000 0072 2700 0000  .r....rH...r'...
-00002200: 7227 0000 0072 2700 0000 7228 0000 00da  r'...r'...r(....
-00002210: 083c 6d6f 6475 6c65 3e01 0000 0073 6600  .<module>....sf.
-00002220: 0000 0800 1801 0c01 0c01 3801 0c0f 1c01  ..........8.....
-00002230: 1408 0202 0601 0401 0401 06fd 1a07 0807  ................
-00002240: 0801 0801 1e03 1205 120b 0806 0204 1001  ................
-00002250: 0205 1001 0208 1001 1a23 007f 0225 0201  .........#...%..
-00002260: 0201 0201 0201 0201 0201 04f8 0201 02ff  ................
-00002270: 0a02 02fe 0603 02fd 0604 02fc 0605 02fb  ................
-00002280: 0206 02fa 1609 0ef7                      ........
+00000020: 0010 0000 0040 0000 0073 3401 0000 6400  .....@...s4...d.
+00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
+00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
+00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
+00000060: 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  m.Z.m.Z.m.Z.m.Z.
+00000070: 6d0e 5a0e 0100 6400 6404 6c0f 6d10 5a10  m.Z...d.d.l.m.Z.
+00000080: 6d11 5a11 6d12 5a12 0100 6405 6406 6c13  m.Z.m.Z...d.d.l.
+00000090: 6d14 5a14 6d15 5a15 6d16 5a16 6d17 5a17  m.Z.m.Z.m.Z.m.Z.
+000000a0: 0100 650d 6407 8301 5a18 650d 6408 8301  ..e.d...Z.e.d...
+000000b0: 5a19 650d 6409 8301 5a1a 6502 4700 640a  Z.e.d...Z.e.G.d.
+000000c0: 640b 8400 640b 8302 8301 5a1b 6502 4700  d...d.....Z.e.G.
+000000d0: 640c 640d 8400 640d 8302 8301 5a1c 6502  d.d...d.....Z.e.
+000000e0: 4700 640e 640f 8400 640f 8302 8301 5a1d  G.d.d...d.....Z.
+000000f0: 4700 6410 6411 8400 6411 6508 6518 6519  G.d.d...d.e.e.e.
+00000100: 651a 6603 1900 8303 5a1e 6700 6412 6412  e.f.....Z.g.d.d.
+00000110: 6412 6604 6413 650b 6514 1900 6414 650c  d.f.d.e.e...d.e.
+00000120: 651f 1900 6415 650c 651f 1900 6416 650c  e...d.e.e...d.e.
+00000130: 6506 1900 6417 6507 6506 6701 651e 6518  e...d.e.e.g.e.e.
+00000140: 6519 651a 6603 1900 6602 1900 660a 6418  e.e.f...f...f.d.
+00000150: 6419 8405 5a20 641a 641b 8400 5a21 6412  d...Z d.d...Z!d.
+00000160: 5300 291c e900 0000 0029 02da 0661 7364  S.)......)...asd
+00000170: 6963 74da 0964 6174 6163 6c61 7373 2901  ict..dataclass).
+00000180: da05 636f 756e 7429 09da 0341 6e79 da08  ..count)...Any..
+00000190: 4361 6c6c 6162 6c65 da07 4765 6e65 7269  Callable..Generi
+000001a0: 63da 0849 7465 7261 626c 65da 0849 7465  c..Iterable..Ite
+000001b0: 7261 746f 72da 044c 6973 74da 084f 7074  rator..List..Opt
+000001c0: 696f 6e61 6cda 0754 7970 6556 6172 da05  ional..TypeVar..
+000001d0: 556e 696f 6e29 03da 0b45 6e76 6972 6f6e  Union)...Environ
+000001e0: 6d65 6e74 da10 4669 6c65 5379 7374 656d  ment..FileSystem
+000001f0: 4c6f 6164 6572 da08 5465 6d70 6c61 7465  Loader..Template
+00000200: e901 0000 0029 04da 0742 6163 6b65 6e64  .....)...Backend
+00000210: da10 4d69 6e69 6368 6169 6e43 6f6e 7465  ..MinichainConte
+00000220: 7874 da0a 5072 6f6d 7074 536e 6170 da06  xt..PromptSnap..
+00000230: 5275 6e4c 6f67 da05 496e 7075 74da 064f  RunLog..Input..O
+00000240: 7574 7075 74da 0846 6e4f 7574 7075 7463  utput..FnOutputc
+00000250: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000260: 0400 0000 4000 0000 7334 0000 0065 005a  ....@...s4...e.Z
+00000270: 0164 005a 0255 0065 0365 0465 0519 0067  .d.Z.U.e.e.e...g
+00000280: 0165 0665 0519 0066 0219 0065 0764 013c  .e.e...f...e.d.<
+00000290: 0065 0465 0519 0065 0764 023c 0064 0353  .e.e...e.d.<.d.S
+000002a0: 0029 04da 0748 6973 746f 7279 da06 6578  .)...History..ex
+000002b0: 7061 6e64 da06 696e 7075 7473 4e29 08da  pand..inputsN)..
+000002c0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
+000002d0: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
+000002e0: 655f 5f72 0600 0000 720a 0000 0072 0500  e__r....r....r..
+000002f0: 0000 7209 0000 00da 0f5f 5f61 6e6e 6f74  ..r......__annot
+00000300: 6174 696f 6e73 5f5f a900 7220 0000 0072  ations__..r ...r
+00000310: 2000 0000 fa52 2f68 6f6d 652f 7372 7573   ....R/home/srus
+00000320: 682f 5072 6f6a 6563 7473 2f4d 696e 6943  h/Projects/MiniC
+00000330: 6861 696e 2f76 656e 762f 6c69 622f 7079  hain/venv/lib/py
+00000340: 7468 6f6e 332e 3130 2f73 6974 652d 7061  thon3.10/site-pa
+00000350: 636b 6167 6573 2f6d 696e 6963 6861 696e  ckages/minichain
+00000360: 2f62 6173 652e 7079 7219 0000 0018 0000  /base.pyr.......
+00000370: 0073 0600 0000 0a00 1a02 1001 7219 0000  .s..........r...
+00000380: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00000390: 0000 0100 0000 4000 0000 730c 0000 0065  ......@...s....e
+000003a0: 005a 0164 005a 0264 0153 0029 02da 0542  .Z.d.Z.d.S.)...B
+000003b0: 7265 616b 4e29 0372 1c00 0000 721d 0000  reakN).r....r...
+000003c0: 0072 1e00 0000 7220 0000 0072 2000 0000  .r....r ...r ...
+000003d0: 7220 0000 0072 2100 0000 7222 0000 001e  r ...r!...r"....
+000003e0: 0000 0073 0400 0000 0800 0402 7222 0000  ...s........r"..
+000003f0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00000400: 0000 0300 0000 4000 0000 7346 0000 0065  ......@...sF...e
+00000410: 005a 0164 005a 0255 0065 0365 0464 013c  .Z.d.Z.U.e.e.d.<
+00000420: 0065 0565 0464 023c 0064 035a 0665 0765  .e.e.d.<.d.Z.e.e
+00000430: 0464 043c 0064 0565 0766 0264 0664 0784  .d.<.d.e.f.d.d..
+00000440: 045a 0864 0565 0766 0264 0864 0984 045a  .Z.d.e.f.d.d...Z
+00000450: 0964 0353 0029 0ada 0543 6861 696e da07  .d.S.)...Chain..
+00000460: 6869 7374 6f72 79da 046e 616d 654e da05  history..nameN..
+00000470: 6361 6368 65da 0672 6574 7572 6e63 0100  cache..returnc..
+00000480: 0000 0000 0000 0000 0000 0600 0000 0500  ................
+00000490: 0000 6300 0000 73d4 0000 0081 0067 007d  ..c...s......g.}
+000004a0: 0174 007c 006a 016a 0283 0144 005d 435c  .t.|.j.j...D.]C\
+000004b0: 027d 027d 037c 037d 0474 037c 0374 0483  .}.}.|.}.t.|.t..
+000004c0: 0272 477c 036a 0564 0075 0172 297c 036a  .rG|.j.d.u.r)|.j
+000004d0: 057d 0474 037c 0474 0683 0272 2874 0683  .}.t.|.t...r(t..
+000004e0: 0056 0001 0001 0064 0053 006e 1e7c 03a0  .V.....d.S.n.|..
+000004f0: 07a1 0044 005d 167d 0474 037c 0474 0683  ...D.].}.t.|.t..
+00000500: 0272 4074 0683 007c 035f 0574 0683 0056  .r@t...|._.t...V
+00000510: 0001 0001 0001 0064 0053 0064 0056 0001  .......d.S.d.V..
+00000520: 0071 2d7c 047c 035f 057c 01a0 087c 04a1  .q-|.|._.|...|..
+00000530: 0101 0071 097c 006a 016a 097c 018e 0044  ...q.|.j.j.|...D
+00000540: 005d 117d 0574 037c 0574 0683 0272 6174  .].}.t.|.t...rat
+00000550: 0683 0056 0001 0001 0064 0053 0064 0056  ...V.....d.S.d.V
+00000560: 0001 0071 537c 0556 0001 0064 0053 00a9  ...qS|.V...d.S..
+00000570: 014e 290a da09 656e 756d 6572 6174 6572  .N)...enumerater
+00000580: 2400 0000 721b 0000 00da 0a69 7369 6e73  $...r......isins
+00000590: 7461 6e63 6572 2300 0000 7226 0000 0072  tancer#...r&...r
+000005a0: 2200 0000 da07 7275 6e5f 6765 6eda 0661  ".....run_gen..a
+000005b0: 7070 656e 6472 1a00 0000 2906 da04 7365  ppendr....)...se
+000005c0: 6c66 da04 6172 6773 da01 69da 0a62 6173  lf..args..i..bas
+000005d0: 655f 696e 7075 74da 0e66 756e 6374 696f  e_input..functio
+000005e0: 6e5f 696e 7075 74da 036f 7574 7220 0000  n_input..outr ..
+000005f0: 0072 2000 0000 7221 0000 0072 2b00 0000  .r ...r!...r+...
+00000600: 2900 0000 7332 0000 0002 8004 0214 0104  )...s2..........
+00000610: 010a 010a 0106 010a 0108 0106 0102 fe0c  ................
+00000620: 040a 0108 0108 0108 0108 0106 020c 0110  ................
+00000630: 020a 0108 0106 0108 020a 017a 0d43 6861  ...........z.Cha
+00000640: 696e 2e72 756e 5f67 656e 6301 0000 0000  in.run_genc.....
+00000650: 0000 0000 0000 0002 0000 0002 0000 0043  ...............C
+00000660: 0000 0073 1200 0000 7c00 a000 a100 4400  ...s....|.....D.
+00000670: 5d02 7d01 7104 7c01 5300 7228 0000 0029  ].}.q.|.S.r(...)
+00000680: 0172 2b00 0000 2902 722d 0000 00da 0178  .r+...).r-.....x
+00000690: 7220 0000 0072 2000 0000 7221 0000 00da  r ...r ...r!....
+000006a0: 0372 756e 4700 0000 7306 0000 000c 0102  .runG...s.......
+000006b0: 0104 017a 0943 6861 696e 2e72 756e 290a  ...z.Chain.run).
+000006c0: 721c 0000 0072 1d00 0000 721e 0000 0072  r....r....r....r
+000006d0: 1900 0000 721f 0000 00da 0373 7472 7226  ....r......strr&
+000006e0: 0000 0072 0500 0000 722b 0000 0072 3400  ...r....r+...r4.
+000006f0: 0000 7220 0000 0072 2000 0000 7220 0000  ..r ...r ...r ..
+00000700: 0072 2100 0000 7223 0000 0023 0000 0073  .r!...r#...#...s
+00000710: 0c00 0000 0a00 0802 0801 0c01 0e02 121e  ................
+00000720: 7223 0000 0063 0000 0000 0000 0000 0000  r#...c..........
+00000730: 0000 0000 0000 0b00 0000 4000 0000 73d6  ..........@...s.
+00000740: 0000 0065 005a 0164 005a 0265 0383 005a  ...e.Z.d.Z.e...Z
+00000750: 0409 0164 1b64 0265 0565 0565 0667 0165  ...d.d.e.e.e.g.e
+00000760: 0766 0219 0067 0165 0865 0919 0066 0219  .f...g.e.e...f..
+00000770: 0064 0365 0a65 0b65 0c19 0065 0c66 0219  .d.e.e.e...e.f..
+00000780: 0064 0465 0d65 0e19 0064 0565 0d65 0e19  .d.e.e...d.e.e..
+00000790: 0064 0665 0f66 0a64 0764 0884 055a 1064  .d.e.f.d.d...Z.d
+000007a0: 1c64 0a65 0e64 0b65 1164 0c65 1265 1319  .d.e.d.e.d.e.e..
+000007b0: 0066 0664 0d64 0e84 055a 1464 0f65 0f64  .f.d.d...Z.d.e.d
+000007c0: 0c65 0e66 0464 1064 1184 045a 1564 1265  .e.f.d.d...Z.d.e
+000007d0: 0f64 0c65 1666 0464 1364 1484 045a 1747  .d.e.f.d.d...Z.G
+000007e0: 0064 1564 1684 0064 1683 025a 1864 0164  .d.d...d...Z.d.d
+000007f0: 179c 0164 1265 0b65 0f19 0064 1865 0f64  ...d.e.e...d.e.d
+00000800: 0c65 1265 0d65 0919 0019 0066 0664 1964  .e.e.e.....f.d.d
+00000810: 1a84 065a 1964 0153 0029 1dda 0650 726f  ...Z.d.S.)...Pro
+00000820: 6d70 744e da02 666e da07 6261 636b 656e  mptN..fn..backen
+00000830: 64da 0d74 656d 706c 6174 655f 6669 6c65  d..template_file
+00000840: da08 7465 6d70 6c61 7465 da0b 6772 6164  ..template..grad
+00000850: 696f 5f63 6f6e 6663 0600 0000 0000 0000  io_confc........
+00000860: 0000 0000 0600 0000 0300 0000 4300 0000  ............C...
+00000870: 734a 0000 007c 017c 005f 0074 017c 0274  sJ...|.|._.t.|.t
+00000880: 0283 0273 0d7c 0267 017c 005f 036e 037c  ...s.|.g.|._.n.|
+00000890: 027c 005f 037c 037c 005f 047c 047c 005f  .|._.|.|._.|.|._
+000008a0: 057c 057c 005f 067c 016a 077c 005f 0874  .|.|._.|.j.|._.t
+000008b0: 096a 0aa0 0ba1 007c 005f 0c64 0053 0072  .j.....|._.d.S.r
+000008c0: 2800 0000 290d 7237 0000 0072 2a00 0000  (...).r7...r*...
+000008d0: 720a 0000 0072 3800 0000 7239 0000 0072  r....r8...r9...r
+000008e0: 3a00 0000 723b 0000 0072 1c00 0000 da03  :...r;...r......
+000008f0: 5f66 6e72 3600 0000 da07 636f 756e 7465  _fnr6.....counte
+00000900: 72da 085f 5f6e 6578 745f 5fda 035f 6964  r..__next__.._id
+00000910: 2906 722d 0000 0072 3700 0000 7238 0000  ).r-...r7...r8..
+00000920: 0072 3900 0000 723a 0000 0072 3b00 0000  .r9...r:...r;...
+00000930: 7220 0000 0072 2000 0000 7221 0000 00da  r ...r ...r!....
+00000940: 085f 5f69 6e69 745f 5f50 0000 0073 1200  .__init__P...s..
+00000950: 0000 0608 0a01 0a01 0602 0602 0601 0601  ................
+00000960: 0802 1001 7a0f 5072 6f6d 7074 2e5f 5f69  ....z.Prompt.__i
+00000970: 6e69 745f 5f72 0100 0000 da07 7265 7175  nit__r......requ
+00000980: 6573 74da 0874 6f6f 6c5f 6e75 6d72 2700  est..tool_numr'.
+00000990: 0000 6303 0000 0000 0000 0000 0000 0005  ..c.............
+000009a0: 0000 0004 0000 0063 0000 0073 7000 0000  .......c...sp...
+000009b0: 8100 7400 7c00 6a01 7c02 1900 6401 8302  ..t.|.j.|...d...
+000009c0: 731f 7402 7c01 6400 8302 5600 0100 7c00  s.t.|.d...V...|.
+000009d0: 6a01 7c02 1900 a003 7c01 a101 7d03 7402  j.|.....|...}.t.
+000009e0: 7c01 7c03 8302 5600 0100 6400 5300 7402  |.|...V...d.S.t.
+000009f0: 7c01 6400 8302 5600 0100 7c00 6a01 7c02  |.d...V...|.j.|.
+00000a00: 1900 a004 7c01 a101 4400 5d08 7d04 7402  ....|...D.].}.t.
+00000a10: 7c01 7c04 8302 5600 0100 712d 6400 5300  |.|...V...q-d.S.
+00000a20: 2902 4eda 0a72 756e 5f73 7472 6561 6d29  ).N..run_stream)
+00000a30: 05da 0768 6173 6174 7472 7238 0000 0072  ...hasattrr8...r
+00000a40: 1500 0000 7234 0000 0072 4300 0000 2905  ....r4...rC...).
+00000a50: 722d 0000 0072 4100 0000 7242 0000 00da  r-...rA...rB....
+00000a60: 0872 6573 706f 6e73 65da 0172 7220 0000  .response..rr ..
+00000a70: 0072 2000 0000 7221 0000 0072 3400 0000  .r ...r!...r4...
+00000a80: 6500 0000 7312 0000 0002 8010 010c 0110  e...s...........
+00000a90: 0110 010c 0214 010e 0104 ff7a 0a50 726f  ...........z.Pro
+00000aa0: 6d70 742e 7275 6eda 0369 6e70 6302 0000  mpt.run..inpc...
+00000ab0: 0000 0000 0000 0000 0004 0000 0005 0000  ................
+00000ac0: 0043 0000 0073 4800 0000 7c01 7d02 7c00  .C...sH...|.}.|.
+00000ad0: 6a00 7212 7401 7402 6401 8301 6402 8d01  j.r.t.t.d...d...
+00000ae0: 6a03 7c00 6a00 6403 8d01 7d03 6e08 7c00  j.|.j.d...}.n.|.
+00000af0: 6a04 721a 7405 7c00 6a04 8301 7d03 7406  j.r.t.|.j...}.t.
+00000b00: 7c03 6a07 6404 6900 7c02 a401 8e01 8301  |.j.d.i.|.......
+00000b10: 5300 2905 4eda 012e 2901 da06 6c6f 6164  S.).N...)...load
+00000b20: 6572 2901 7225 0000 0072 2000 0000 2908  er).r%...r ...).
+00000b30: 7239 0000 0072 0e00 0000 720f 0000 00da  r9...r....r.....
+00000b40: 0c67 6574 5f74 656d 706c 6174 6572 3a00  .get_templater:.
+00000b50: 0000 7210 0000 0072 3500 0000 da06 7265  ..r....r5.....re
+00000b60: 6e64 6572 2904 722d 0000 0072 4700 0000  nder).r-...rG...
+00000b70: da06 6b77 6172 6773 da03 746d 7072 2000  ..kwargs..tmpr .
+00000b80: 0000 7220 0000 0072 2100 0000 da0d 7465  ..r ...r!.....te
+00000b90: 6d70 6c61 7465 5f66 696c 6c6f 0000 0073  mplate_fillo...s
+00000ba0: 1000 0000 0401 0601 0e01 0401 08ff 0603  ................
+00000bb0: 0a01 1402 7a14 5072 6f6d 7074 2e74 656d  ....z.Prompt.tem
+00000bc0: 706c 6174 655f 6669 6c6c 722e 0000 0063  plate_fillr....c
+00000bd0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00000be0: 0500 0000 4700 0000 731a 0000 0074 0074  ....G...s....t.t
+00000bf0: 017c 006a 0274 037c 0183 0183 027c 006a  .|.j.t.|.....|.j
+00000c00: 046a 0583 0253 0072 2800 0000 2906 7223  .j...S.r(...).r#
+00000c10: 0000 0072 1900 0000 721a 0000 00da 046c  ...r....r......l
+00000c20: 6973 7472 3700 0000 721c 0000 0029 0272  istr7...r....).r
+00000c30: 2d00 0000 722e 0000 0072 2000 0000 7220  -...r....r ...r 
+00000c40: 0000 0072 2100 0000 da08 5f5f 6361 6c6c  ...r!.....__call
+00000c50: 5f5f 7a00 0000 7302 0000 001a 017a 0f50  __z...s......z.P
+00000c60: 726f 6d70 742e 5f5f 6361 6c6c 5f5f 6300  rompt.__call__c.
+00000c70: 0000 0000 0000 0000 0000 0000 0000 0009  ................
+00000c80: 0000 0040 0000 0073 5800 0000 6500 5a01  ...@...sX...e.Z.
+00000c90: 6400 5a02 6401 6402 6403 6503 6604 6404  d.Z.d.d.d.e.f.d.
+00000ca0: 6405 8404 5a04 640f 6407 6503 6408 6505  d...Z.d.d.e.d.e.
+00000cb0: 6409 6503 6606 640a 640b 8405 5a06 0906  d.e.f.d.d...Z...
+00000cc0: 640f 6407 6503 6408 6505 6409 6507 6508  d.d.e.d.e.d.e.e.
+00000cd0: 6509 1900 1900 6606 640c 640d 8405 5a0a  e.....f.d.d...Z.
+00000ce0: 640e 5300 2910 7a0c 5072 6f6d 7074 2e4d  d.S.).z.Prompt.M
+00000cf0: 6f64 656c da06 7072 6f6d 7074 7a1f 5072  odel..promptz.Pr
+00000d00: 6f6d 7074 5b49 6e70 7574 2c20 4f75 7470  ompt[Input, Outp
+00000d10: 7574 2c20 466e 4f75 7470 7574 5dda 0464  ut, FnOutput]..d
+00000d20: 6174 6163 0300 0000 0000 0000 0000 0000  atac............
+00000d30: 0300 0000 0200 0000 4300 0000 7318 0000  ........C...s...
+00000d40: 007c 017c 005f 007c 027c 005f 0174 0283  .|.|._.|.|._.t..
+00000d50: 007c 005f 0364 0053 0072 2800 0000 2904  .|._.d.S.r(...).
+00000d60: 7251 0000 0072 5200 0000 7215 0000 00da  rQ...rR...r.....
+00000d70: 0772 756e 5f6c 6f67 2903 722d 0000 0072  .run_log).r-...r
+00000d80: 5100 0000 7252 0000 0072 2000 0000 7220  Q...rR...r ...r 
+00000d90: 0000 0072 2100 0000 7240 0000 007e 0000  ...r!...r@...~..
+00000da0: 0073 0600 0000 0601 0601 0c01 7a15 5072  .s..........z.Pr
+00000db0: 6f6d 7074 2e4d 6f64 656c 2e5f 5f69 6e69  ompt.Model.__ini
+00000dc0: 745f 5f72 0100 0000 da0b 6d6f 6465 6c5f  t__r......model_
+00000dd0: 696e 7075 7472 4200 0000 7227 0000 0063  inputrB...r'...c
+00000de0: 0300 0000 0000 0000 0000 0000 0400 0000  ................
+00000df0: 0400 0000 6300 0000 731e 0000 0081 007c  ....c...s......|
+00000e00: 00a0 007c 017c 02a1 0244 005d 057d 037c  ...|.|...D.].}.|
+00000e10: 0356 0001 0071 0764 0053 0072 2800 0000  .V...q.d.S.r(...
+00000e20: 2901 da06 7374 7265 616d 2904 722d 0000  )...stream).r-..
+00000e30: 0072 5400 0000 7242 0000 0072 4600 0000  .rT...rB...rF...
+00000e40: 7220 0000 0072 2000 0000 7221 0000 0072  r ...r ...r!...r
+00000e50: 5000 0000 8300 0000 7308 0000 0002 8010  P.......s.......
+00000e60: 0108 0104 ff7a 1550 726f 6d70 742e 4d6f  .....z.Prompt.Mo
+00000e70: 6465 6c2e 5f5f 6361 6c6c 5f5f 6303 0000  del.__call__c...
+00000e80: 0000 0000 0000 0000 0007 0000 0006 0000  ................
+00000e90: 0063 0000 0073 a000 0000 8100 7c00 6a00  .c...s......|.j.
+00000ea0: 6a01 6400 7501 730d 7c00 6a00 6a02 6400  j.d.u.s.|.j.j.d.
+00000eb0: 7501 721d 7403 7c01 7404 8302 7316 7405  u.r.t.|.t...s.t.
+00000ec0: 7c01 8301 7d01 7c00 6a00 a006 7c01 a101  |...}.|.j...|...
+00000ed0: 7d03 6e02 7c01 7d03 7c00 6a00 a007 7c03  }.n.|.}.|.j...|.
+00000ee0: 7c02 a102 4400 5d27 7d04 7c00 6a08 6a09  |...D.]'}.|.j.j.
+00000ef0: 7d05 7c04 6a09 6400 7500 7234 7c05 7d06  }.|.j.d.u.r4|.}.
+00000f00: 6e0b 7c05 733a 7c04 6a09 7d06 6e05 7c05  n.|.s:|.j.}.n.|.
+00000f10: 7c04 6a09 1700 7d06 740a 7c04 6a0b 7c06  |.j...}.t.|.j.|.
+00000f20: 7c02 6401 8d03 7c00 5f08 7c00 6a08 6a09  |.d...|._.|.j.j.
+00000f30: 5600 0100 7126 6400 5300 2902 4e29 01da  V...q&d.S.).N)..
+00000f40: 0764 796e 616d 6963 290c 7251 0000 0072  .dynamic).rQ...r
+00000f50: 3a00 0000 7239 0000 0072 2a00 0000 da04  :...r9...r*.....
+00000f60: 6469 6374 7202 0000 0072 4e00 0000 7234  dictr....rN...r4
+00000f70: 0000 0072 5300 0000 7245 0000 0072 1500  ...rS...rE...r..
+00000f80: 0000 7241 0000 0029 0772 2d00 0000 7254  ..rA...).r-...rT
+00000f90: 0000 0072 4200 0000 da06 7265 7375 6c74  ...rB.....result
+00000fa0: 7253 0000 0072 4600 0000 7232 0000 0072  rS...rF...r2...r
+00000fb0: 2000 0000 7220 0000 0072 2100 0000 7255   ...r ...r!...rU
+00000fc0: 0000 008d 0000 0073 2600 0000 0280 0a04  .......s&.......
+00000fd0: 02ff 0a02 02fe 0a04 0801 0e01 0402 1202  ................
+00000fe0: 0801 0a01 0601 0401 0801 0a02 1201 0c01  ................
+00000ff0: 04f7 7a13 5072 6f6d 7074 2e4d 6f64 656c  ..z.Prompt.Model
+00001000: 2e73 7472 6561 6d4e a901 7201 0000 0029  .streamN..r....)
+00001010: 0b72 1c00 0000 721d 0000 0072 1e00 0000  .r....r....r....
+00001020: 7205 0000 0072 4000 0000 da03 696e 7472  r....r@.....intr
+00001030: 5000 0000 7209 0000 0072 0b00 0000 7235  P...r....r....r5
+00001040: 0000 0072 5500 0000 7220 0000 0072 2000  ...rU...r ...r .
+00001050: 0000 7220 0000 0072 2100 0000 da05 4d6f  ..r ...r!.....Mo
+00001060: 6465 6c7d 0000 0073 1600 0000 0800 1201  del}...s........
+00001070: 1805 020b 04ff 0201 02ff 0201 02ff 0a02  ................
+00001080: 0efe 725b 0000 0029 0172 5200 0000 7252  ..r[...).rR...rR
+00001090: 0000 0063 0100 0000 0000 0000 0100 0000  ...c............
+000010a0: 0800 0000 0500 0000 6700 0000 7322 0100  ........g...s"..
+000010b0: 0081 0074 006a 01a0 027c 006a 0364 01a1  ...t.j...|.j.d..
+000010c0: 0201 0074 006a 017c 006a 0305 0019 0064  ...t.j.|.j.....d
+000010d0: 0237 0003 003c 0074 006a 017c 006a 0319  .7...<.t.j.|.j..
+000010e0: 007d 0374 006a 04a0 027c 006a 037c 0366  .}.t.j...|.j.|.f
+000010f0: 0267 00a1 0201 0074 006a 047c 006a 037c  .g.....t.j.|.j.|
+00001100: 0366 0219 00a0 0574 0683 00a1 0101 007c  .f.....t.......|
+00001110: 00a0 077c 007c 01a1 027d 047c 006a 087c  ...|.|...}.|.j.|
+00001120: 0467 017c 02a2 0152 008e 0044 005d 317d  .g.|...R...D.]1}
+00001130: 057c 046a 097d 067c 046a 0973 4c4a 0074  .|.j.}.|.j.sLJ.t
+00001140: 0a7c 0483 0183 0182 0174 067c 027c 067c  .|.......t.|.|.|
+00001150: 0583 037d 0774 006a 017c 006a 0319 007d  ...}.t.j.|.j...}
+00001160: 0374 006a 04a0 027c 006a 037c 0366 0267  .t.j...|.j.|.f.g
+00001170: 00a1 0201 007c 0774 006a 047c 006a 037c  .....|.t.j.|.j.|
+00001180: 0366 0219 0064 013c 0064 0056 0001 0071  .f...d.<.d.V...q
+00001190: 3e7c 046a 0973 794a 0074 0a7c 0483 0183  >|.j.syJ.t.|....
+000011a0: 0182 017c 046a 097d 0674 067c 027c 067c  ...|.j.}.t.|.|.|
+000011b0: 0583 037d 077c 0774 006a 047c 006a 037c  ...}.|.t.j.|.j.|
+000011c0: 0366 0219 0064 013c 007c 0556 0001 0064  .f...d.<.|.V...d
+000011d0: 0053 0029 034e e9ff ffff ff72 1100 0000  .S.).N.....r....
+000011e0: 290b 7213 0000 00da 0c70 726f 6d70 745f  ).r......prompt_
+000011f0: 636f 756e 74da 0a73 6574 6465 6661 756c  count..setdefaul
+00001200: 7472 3f00 0000 da0c 7072 6f6d 7074 5f73  tr?.....prompt_s
+00001210: 746f 7265 722c 0000 0072 1400 0000 725b  torer,...r....r[
+00001220: 0000 0072 3700 0000 7253 0000 0072 3500  ...r7...rS...r5.
+00001230: 0000 2908 722d 0000 0072 5200 0000 722e  ..).r-...rR...r.
+00001240: 0000 0072 0400 0000 da05 6d6f 6465 6cda  ...r......model.
+00001250: 066f 7574 7075 74da 0174 da04 736e 6170  .output..t..snap
+00001260: 7220 0000 0072 2000 0000 7221 0000 0072  r ...r ...r!...r
+00001270: 1a00 0000 a500 0000 7328 0000 0002 8010  ........s(......
+00001280: 0414 010c 0114 0318 010c 0316 0106 0112  ................
+00001290: 010c 010c 0114 0114 0108 0112 0206 010c  ................
+000012a0: 0114 010a 017a 0d50 726f 6d70 742e 6578  .....z.Prompt.ex
+000012b0: 7061 6e64 7228 0000 0072 5900 0000 291a  pandr(...rY...).
+000012c0: 721c 0000 0072 1d00 0000 721e 0000 0072  r....r....r....r
+000012d0: 0400 0000 723d 0000 0072 0600 0000 7216  ....r=...r....r.
+000012e0: 0000 0072 1700 0000 7208 0000 0072 1800  ...r....r....r..
+000012f0: 0000 720d 0000 0072 0a00 0000 7212 0000  ..r....r....r...
+00001300: 0072 0b00 0000 7235 0000 0072 0500 0000  .r....r5...r....
+00001310: 7240 0000 0072 5a00 0000 7209 0000 0072  r@...rZ...r....r
+00001320: 1500 0000 7234 0000 0072 4e00 0000 7223  ....r4...rN...r#
+00001330: 0000 0072 5000 0000 725b 0000 0072 1a00  ...rP...r[...r..
+00001340: 0000 7220 0000 0072 2000 0000 7220 0000  ..r ...r ...r ..
+00001350: 0072 2100 0000 7236 0000 004d 0000 0073  .r!...r6...M...s
+00001360: 3400 0000 0800 0601 0208 04fa 1a02 02fe  4...............
+00001370: 0e03 02fd 0604 02fc 0605 02fb 0206 0afa  ................
+00001380: 1c15 120a 120b 0e03 0229 06ff 0601 02ff  .........)......
+00001390: 0201 02ff 0a02 0efe 7236 0000 004e 7238  ........r6...Nr8
+000013a0: 0000 0072 3900 0000 723a 0000 0072 3b00  ...r9...r:...r;.
+000013b0: 0000 7227 0000 0063 0400 0000 0000 0000  ..r'...c........
+000013c0: 0000 0000 0400 0000 0400 0000 0300 0000  ................
+000013d0: 7312 0000 0087 0087 0187 0287 0366 0464  s............f.d
+000013e0: 0164 0284 0853 0029 034e 6301 0000 0000  .d...S.).Nc.....
+000013f0: 0000 0000 0000 0001 0000 0006 0000 0013  ................
+00001400: 0000 0073 1000 0000 7400 7c00 8800 8803  ...s....t.|.....
+00001410: 8802 8801 8305 5300 7228 0000 0029 0172  ......S.r(...).r
+00001420: 3600 0000 a901 7237 0000 00a9 0472 3800  6.....r7.....r8.
+00001430: 0000 723b 0000 0072 3a00 0000 7239 0000  ..r;...r:...r9..
+00001440: 0072 2000 0000 7221 0000 00da 083c 6c61  .r ...r!.....<la
+00001450: 6d62 6461 3ec9 0000 0073 0200 0000 1000  mbda>....s......
+00001460: 7a18 7072 6f6d 7074 2e3c 6c6f 6361 6c73  z.prompt.<locals
+00001470: 3e2e 3c6c 616d 6264 613e 7220 0000 0029  >.<lambda>r ...)
+00001480: 0472 3800 0000 7239 0000 0072 3a00 0000  .r8...r9...r:...
+00001490: 723b 0000 0072 2000 0000 7265 0000 0072  r;...r ...re...r
+000014a0: 2100 0000 7251 0000 00c3 0000 0073 0200  !...rQ.......s..
+000014b0: 0000 1206 7251 0000 0063 0000 0000 0000  ....rQ...c......
+000014c0: 0000 0000 0000 0000 0000 0200 0000 4300  ..............C.
+000014d0: 0000 7308 0000 0064 0164 0284 0053 0029  ..s....d.d...S.)
+000014e0: 034e 6301 0000 0000 0000 0000 0000 0001  .Nc.............
+000014f0: 0000 0003 0000 0013 0000 0073 0c00 0000  ...........s....
+00001500: 8700 6601 6401 6402 8408 5300 2903 4e63  ..f.d.d...S.).Nc
+00001510: 0000 0000 0000 0000 0000 0000 0100 0000  ................
+00001520: 0500 0000 1700 0000 731e 0000 0074 0074  ........s....t.t
+00001530: 0187 0066 0164 0164 0284 0874 027c 0083  ...f.d.d...t.|..
+00001540: 0183 0288 006a 0383 0253 0029 034e 6300  .....j...S.).Nc.
+00001550: 0000 0000 0000 0000 0000 0001 0000 0003  ................
+00001560: 0000 0017 0000 0073 0e00 0000 7400 8800  .......s....t...
+00001570: 7c00 8e00 6601 8301 5300 7228 0000 0029  |...f...S.r(...)
+00001580: 01da 0469 7465 7229 0172 3300 0000 7264  ...iter).r3...rd
+00001590: 0000 0072 2000 0000 7221 0000 0072 6600  ...r ...r!...rf.
+000015a0: 0000 ce00 0000 7302 0000 000e 007a 3f74  ......s......z?t
+000015b0: 7261 6e73 666f 726d 2e3c 6c6f 6361 6c73  ransform.<locals
+000015c0: 3e2e 3c6c 616d 6264 613e 2e3c 6c6f 6361  >.<lambda>.<loca
+000015d0: 6c73 3e2e 3c6c 616d 6264 613e 2e3c 6c6f  ls>.<lambda>.<lo
+000015e0: 6361 6c73 3e2e 3c6c 616d 6264 613e 2904  cals>.<lambda>).
+000015f0: 7223 0000 0072 1900 0000 724f 0000 0072  r#...r....rO...r
+00001600: 1c00 0000 2901 722e 0000 0072 6400 0000  ....).r....rd...
+00001610: 7220 0000 0072 2100 0000 7266 0000 00cd  r ...r!...rf....
+00001620: 0000 0073 0600 0000 0200 1801 04ff 7a2d  ...s..........z-
+00001630: 7472 616e 7366 6f72 6d2e 3c6c 6f63 616c  transform.<local
+00001640: 733e 2e3c 6c61 6d62 6461 3e2e 3c6c 6f63  s>.<lambda>.<loc
+00001650: 616c 733e 2e3c 6c61 6d62 6461 3e72 2000  als>.<lambda>r .
+00001660: 0000 7264 0000 0072 2000 0000 7264 0000  ..rd...r ...rd..
+00001670: 0072 2100 0000 7266 0000 00cd 0000 0073  .r!...rf.......s
+00001680: 0200 0000 0c00 7a1b 7472 616e 7366 6f72  ......z.transfor
+00001690: 6d2e 3c6c 6f63 616c 733e 2e3c 6c61 6d62  m.<locals>.<lamb
+000016a0: 6461 3e72 2000 0000 7220 0000 0072 2000  da>r ...r ...r .
+000016b0: 0000 7220 0000 0072 2100 0000 da09 7472  ..r ...r!.....tr
+000016c0: 616e 7366 6f72 6dcc 0000 0073 0200 0000  ansform....s....
+000016d0: 0801 7268 0000 0029 22da 0b64 6174 6163  ..rh...)"..datac
+000016e0: 6c61 7373 6573 7202 0000 0072 0300 0000  lassesr....r....
+000016f0: da09 6974 6572 746f 6f6c 7372 0400 0000  ..itertoolsr....
+00001700: da06 7479 7069 6e67 7205 0000 0072 0600  ..typingr....r..
+00001710: 0000 7207 0000 0072 0800 0000 7209 0000  ..r....r....r...
+00001720: 0072 0a00 0000 720b 0000 0072 0c00 0000  .r....r....r....
+00001730: 720d 0000 00da 066a 696e 6a61 3272 0e00  r......jinja2r..
+00001740: 0000 720f 0000 0072 1000 0000 7238 0000  ..r....r....r8..
+00001750: 0072 1200 0000 7213 0000 0072 1400 0000  .r....r....r....
+00001760: 7215 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
+00001770: 1800 0000 7219 0000 0072 2200 0000 7223  ....r....r"...r#
+00001780: 0000 0072 3600 0000 7235 0000 0072 5100  ...r6...r5...rQ.
+00001790: 0000 7268 0000 0072 2000 0000 7220 0000  ..rh...r ...r ..
+000017a0: 0072 2000 0000 7221 0000 00da 083c 6d6f  .r ...r!.....<mo
+000017b0: 6475 6c65 3e01 0000 0073 3e00 0000 1000  dule>....s>.....
+000017c0: 0c01 2c01 140c 1802 0802 0801 0801 0203  ..,.............
+000017d0: 1001 0205 1001 0204 1001 1a29 0277 0201  ...........).w..
+000017e0: 0201 0201 04fc 0601 02ff 0602 02fe 0603  ................
+000017f0: 02fd 0604 02fc 1605 0afb 0c09            ............
```

### ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/__pycache__/gradio.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 22:06:15 2023 UTC, .py size: 10430 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,573 +1,639 @@
-00000000: 6f0d 0d0a 0000 0000 d77c 3864 be28 0000  o........|8d.(..
+00000000: 6f0d 0d0a 0000 0000 2ff4 3e64 4e2d 0000  o......./.>dN-..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0015 0000 0040 0000 0073 b401 0000 6400  .....@...s....d.
+00000020: 0019 0000 0040 0000 0073 de01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 0100 6400  d.l.m.Z.m.Z...d.
 00000050: 6403 6c05 6d06 5a06 6d07 5a07 6d08 5a08  d.l.m.Z.m.Z.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c  m.Z.m.Z.m.Z.m.Z.
 00000070: 0100 6400 6401 6c0d 5a0e 6400 6404 6c0f  ..d.d.l.Z.d.d.l.
 00000080: 6d10 5a10 0100 6400 6405 6c11 6d12 5a12  m.Z...d.d.l.m.Z.
 00000090: 0100 6406 6407 6c13 6d14 5a14 0100 6406  ..d.d.l.m.Z...d.
 000000a0: 6408 6c15 6d16 5a16 0100 6409 5a17 6503  d.l.m.Z...d.Z.e.
 000000b0: 4700 640a 640b 8400 640b 8302 8301 5a18  G.d.d...d.....Z.
 000000c0: 6503 4700 640c 640d 8400 640d 8302 8301  e.G.d.d...d.....
-000000d0: 5a19 650e a01a 6900 a101 5a1b 650e a01a  Z.e...i...Z.e...
-000000e0: 6900 a101 5a1c 6503 4700 640e 640f 8400  i...Z.e.G.d.d...
-000000f0: 640f 8302 8301 5a1d 6519 8300 6601 6410  d.....Z.e...f.d.
-00000100: 6516 6506 6506 6506 6603 1900 6411 651e  e.e.e.e.f...d.e.
-00000110: 6412 6519 6413 651d 6608 6414 6415 8405  d.e.d.e.f.d.d...
-00000120: 5a1f 6416 6509 6516 6506 6506 6506 6603  Z.d.e.e.e.e.e.f.
-00000130: 1900 1900 6413 651d 6604 6417 6418 8404  ....d.e.f.d.d...
-00000140: 5a20 6419 6801 6601 641a 650a 6521 1900  Z d.h.f.d.e.e!..
-00000150: 6413 6401 6604 641b 641c 8405 5a22 641d  d.d.f.d.d...Z"d.
-00000160: 6701 6700 6700 6401 641e 6419 6801 641d  g.g.g.d.d.d.h.d.
-00000170: 641d 641d 6609 641f 6516 6506 6506 6506  d.d.f.d.e.e.e.e.
-00000180: 6603 1900 6420 650c 6509 6521 1900 6509  f...d e.e.e!..e.
-00000190: 650b 6521 1900 1900 6602 1900 6421 6509  e.e!....f...d!e.
-000001a0: 6516 6506 6506 6506 6603 1900 1900 6422  e.e.e.e.f.....d"
-000001b0: 6509 6521 1900 6423 6506 6424 6521 641a  e.e!..d#e.d$e!d.
-000001c0: 650a 6521 1900 6425 6521 6426 6521 6413  e.e!..d%e!d&e!d.
-000001d0: 650e 6a23 6614 6427 6428 8405 5a24 6401  e.j#f.d'd(..Z$d.
-000001e0: 5300 2929 e900 0000 004e 2902 da09 6461  S.)).....N)...da
-000001f0: 7461 636c 6173 73da 0566 6965 6c64 2907  taclass..field).
-00000200: da03 416e 79da 0843 616c 6c61 626c 65da  ..Any..Callable.
-00000210: 0444 6963 74da 044c 6973 74da 0353 6574  .Dict..List..Set
-00000220: da05 5475 706c 65da 0555 6e69 6f6e 2901  ..Tuple..Union).
-00000230: da05 426c 6f63 6b29 01da 0b73 7461 7274  ..Block)...start
-00000240: 5f63 6861 696e e901 0000 0029 01da 104d  _chain.....)...M
-00000250: 696e 6963 6861 696e 436f 6e74 6578 7429  inichainContext)
-00000260: 01da 0650 726f 6d70 7461 2501 0000 0a23  ...Prompta%....#
-00000270: 636c 6561 6e20 6469 762e 666f 726d 207b  clean div.form {
-00000280: 626f 7264 6572 3a20 3070 787d 0a23 7265  border: 0px}.#re
-00000290: 7370 6f6e 7365 207b 626f 7264 6572 3a20  sponse {border: 
-000002a0: 3070 783b 2062 6163 6b67 726f 756e 643a  0px; background:
-000002b0: 2023 6666 6565 6336 7d0a 2370 726f 6d70   #ffeec6}.#promp
-000002c0: 7420 7b62 6f72 6465 723a 2030 7078 3b62  t {border: 0px;b
-000002d0: 6163 6b67 726f 756e 643a 2061 6c69 6365  ackground: alice
-000002e0: 626c 7565 7d0a 236a 736f 6e20 7b62 6f72  blue}.#json {bor
-000002f0: 6465 723a 2030 7078 7d0a 7370 616e 2e68  der: 0px}.span.h
-00000300: 6561 6420 7b66 6f6e 742d 7369 7a65 3a20  ead {font-size: 
-00000310: 3630 7074 3b20 666f 6e74 2d66 616d 696c  60pt; font-famil
-00000320: 793a 2063 7572 7369 7665 3b7d 0a64 6976  y: cursive;}.div
-00000330: 2e67 7261 6469 6f2d 636f 6e74 6169 6e65  .gradio-containe
-00000340: 7220 7b63 6f6c 6f72 3a20 626c 6163 6b7d  r {color: black}
-00000350: 0a64 6976 2e66 6f72 6d20 7b62 6163 6b67  .div.form {backg
-00000360: 726f 756e 643a 2069 6e68 6572 6974 7d0a  round: inherit}.
-00000370: 6469 762e 666f 726d 2064 6976 207b 6261  div.form div {ba
-00000380: 636b 6772 6f75 6e64 3a20 696e 6865 7269  ckground: inheri
-00000390: 747d 0a63 0000 0000 0000 0000 0000 0000  t}.c............
-000003a0: 0000 0000 0300 0000 4000 0000 7324 0000  ........@...s$..
-000003b0: 0065 005a 0164 005a 0255 0065 0365 0464  .e.Z.d.Z.U.e.e.d
-000003c0: 013c 0064 0265 0366 0264 0364 0484 045a  .<.d.e.f.d.d...Z
-000003d0: 0564 0553 0029 06da 0448 544d 4cda 0468  .d.S.)...HTML..h
-000003e0: 746d 6cda 0672 6574 7572 6e63 0100 0000  tml..returnc....
-000003f0: 0000 0000 0000 0000 0100 0000 0100 0000  ................
-00000400: 4300 0000 7306 0000 007c 006a 0053 00a9  C...s....|.j.S..
-00000410: 014e 2901 7211 0000 0029 01da 0473 656c  .N).r....)...sel
-00000420: 66a9 0072 1500 0000 fa54 2f68 6f6d 652f  f..r.....T/home/
-00000430: 7372 7573 682f 5072 6f6a 6563 7473 2f4d  srush/Projects/M
-00000440: 696e 6943 6861 696e 2f76 656e 762f 6c69  iniChain/venv/li
-00000450: 622f 7079 7468 6f6e 332e 3130 2f73 6974  b/python3.10/sit
-00000460: 652d 7061 636b 6167 6573 2f6d 696e 6963  e-packages/minic
-00000470: 6861 696e 2f67 7261 6469 6f2e 7079 da0b  hain/gradio.py..
-00000480: 5f72 6570 725f 6874 6d6c 5f29 0000 0073  _repr_html_)...s
-00000490: 0200 0000 0601 7a10 4854 4d4c 2e5f 7265  ......z.HTML._re
-000004a0: 7072 5f68 746d 6c5f 4e29 06da 085f 5f6e  pr_html_N)...__n
-000004b0: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-000004c0: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
-000004d0: 0373 7472 da0f 5f5f 616e 6e6f 7461 7469  .str..__annotati
-000004e0: 6f6e 735f 5f72 1700 0000 7215 0000 0072  ons__r....r....r
-000004f0: 1500 0000 7215 0000 0072 1600 0000 7210  ....r....r....r.
-00000500: 0000 0025 0000 0073 0600 0000 0a00 0802  ...%...s........
-00000510: 1202 7210 0000 0063 0000 0000 0000 0000  ..r....c........
-00000520: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
-00000530: 731a 0000 0065 005a 0164 005a 0255 0064  s....e.Z.d.Z.U.d
-00000540: 015a 0365 0465 0564 023c 0064 0353 0029  .Z.e.e.d.<.d.S.)
-00000550: 04da 0e44 6973 706c 6179 4f70 7469 6f6e  ...DisplayOption
-00000560: 7354 da08 6d61 726b 646f 776e 4e29 0672  sT..markdownN).r
-00000570: 1800 0000 7219 0000 0072 1a00 0000 721e  ....r....r....r.
-00000580: 0000 00da 0462 6f6f 6c72 1c00 0000 7215  .....boolr....r.
-00000590: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
-000005a0: 0000 721d 0000 002d 0000 0073 0400 0000  ..r....-...s....
-000005b0: 0a00 1002 721d 0000 0063 0000 0000 0000  ....r....c......
-000005c0: 0000 0000 0000 0000 0000 0600 0000 4000  ..............@.
-000005d0: 0000 73ac 0000 0065 005a 0164 005a 0255  ..s....e.Z.d.Z.U
-000005e0: 0065 0365 0464 018d 015a 0565 0665 0765  .e.e.d...Z.e.e.e
-000005f0: 0865 0965 0a66 0219 0067 0165 0865 0965  .e.e.f...g.e.e.e
-00000600: 0a66 0219 0066 0219 0019 0065 0b64 023c  .f...f.....e.d.<
-00000610: 0065 0365 0c64 018d 015a 0d65 0e65 0919  .e.e.d...Z.e.e..
-00000620: 0065 0b64 033c 0065 0365 0c64 018d 015a  .e.d.<.e.e.d...Z
-00000630: 0f65 0e65 0919 0065 0b64 043c 0064 0f64  .e.e...e.d.<.d.d
-00000640: 0764 0884 045a 1064 0365 0665 0919 0064  .d...Z.d.e.e...d
-00000650: 0664 0066 0464 0964 0a84 045a 1164 0b65  .d.f.d.d...Z.d.e
-00000660: 0865 0965 0a66 0219 0064 0665 0865 0965  .e.e.f...d.e.e.e
-00000670: 0a66 0219 0066 0464 0c64 0d84 045a 1264  .f...f.d.d...Z.d
-00000680: 0e53 0029 10da 0b43 6f6e 7374 7275 6374  .S.)...Construct
-00000690: 6f72 2901 da0f 6465 6661 756c 745f 6661  or)...default_fa
-000006a0: 6374 6f72 79da 0366 6e73 da06 696e 7075  ctory..fns..inpu
-000006b0: 7473 da07 6f75 7470 7574 73da 056f 7468  ts..outputs..oth
-000006c0: 6572 7212 0000 0063 0200 0000 0000 0000  err....c........
-000006d0: 0000 0000 0200 0000 0500 0000 4300 0000  ............C...
-000006e0: 7324 0000 0074 007c 006a 017c 016a 0117  s$...t.|.j.|.j..
-000006f0: 007c 006a 027c 016a 0242 007c 006a 037c  .|.j.|.j.B.|.j.|
-00000700: 016a 0342 0083 0353 0072 1300 0000 2904  .j.B...S.r....).
-00000710: 7220 0000 0072 2200 0000 7223 0000 0072  r ...r"...r#...r
-00000720: 2400 0000 2902 7214 0000 0072 2500 0000  $...).r....r%...
-00000730: 7215 0000 0072 1500 0000 7216 0000 00da  r....r....r.....
-00000740: 056d 6572 6765 3e00 0000 730a 0000 0002  .merge>...s.....
-00000750: 010a 010a 010a 0104 fd7a 1143 6f6e 7374  .........z.Const
-00000760: 7275 6374 6f72 2e6d 6572 6765 6302 0000  ructor.mergec...
-00000770: 0000 0000 0000 0000 0002 0000 0005 0000  ................
-00000780: 0043 0000 0073 1a00 0000 7400 7c00 6a01  .C...s....t.|.j.
-00000790: 7c00 6a02 7403 7c01 8301 4200 7c00 6a04  |.j.t.|...B.|.j.
-000007a0: 8303 5300 7213 0000 0029 0572 2000 0000  ..S.r....).r ...
-000007b0: 7222 0000 0072 2300 0000 da03 7365 7472  r"...r#.....setr
-000007c0: 2400 0000 2902 7214 0000 0072 2300 0000  $...).r....r#...
-000007d0: 7215 0000 0072 1500 0000 7216 0000 00da  r....r....r.....
-000007e0: 0a61 6464 5f69 6e70 7574 7345 0000 0073  .add_inputsE...s
-000007f0: 0200 0000 1a01 7a16 436f 6e73 7472 7563  ......z.Construc
-00000800: 746f 722e 6164 645f 696e 7075 7473 da04  tor.add_inputs..
-00000810: 6461 7461 6302 0000 0000 0000 0000 0000  datac...........
-00000820: 0004 0000 0004 0000 0043 0000 0073 2400  .........C...s$.
-00000830: 0000 6900 7d02 7c00 6a00 4400 5d0a 7d03  ..i.}.|.j.D.].}.
-00000840: 6900 7c02 a501 7c03 7c01 8301 a501 7d02  i.|...|.|.....}.
-00000850: 7105 7c02 5300 7213 0000 0029 0172 2200  q.|.S.r....).r".
-00000860: 0000 2904 7214 0000 0072 2900 0000 da03  ..).r....r).....
-00000870: 6f75 74da 0266 6e72 1500 0000 7215 0000  out..fnr....r...
-00000880: 0072 1600 0000 722b 0000 0048 0000 0073  .r....r+...H...s
-00000890: 0800 0000 0401 0a01 1201 0401 7a0e 436f  ............z.Co
-000008a0: 6e73 7472 7563 746f 722e 666e 4e29 0472  nstructor.fnN).r
-000008b0: 2500 0000 7220 0000 0072 1200 0000 7220  %...r ...r....r 
-000008c0: 0000 0029 1372 1800 0000 7219 0000 0072  ...).r....r....r
-000008d0: 1a00 0000 7203 0000 00da 046c 6973 7472  ....r......listr
-000008e0: 2200 0000 7207 0000 0072 0500 0000 7206  "...r....r....r.
-000008f0: 0000 0072 0b00 0000 7204 0000 0072 1c00  ...r....r....r..
-00000900: 0000 7227 0000 0072 2300 0000 7208 0000  ..r'...r#...r...
-00000910: 0072 2400 0000 7226 0000 0072 2800 0000  .r$...r&...r(...
-00000920: 722b 0000 0072 1500 0000 7215 0000 0072  r+...r....r....r
-00000930: 1500 0000 7216 0000 0072 2000 0000 3600  ....r....r ...6.
-00000940: 0000 7312 0000 000a 0002 0202 012c ff16  ..s..........,..
-00000950: 0316 010a 0216 0726 0372 2000 0000 da0b  .......&.r .....
-00000960: 6261 7365 5f70 726f 6d70 74da 0169 da0f  base_prompt..i..
-00000970: 6469 7370 6c61 795f 6f70 7469 6f6e 7372  display_optionsr
-00000980: 1200 0000 6303 0000 0000 0000 0000 0000  ....c...........
-00000990: 0004 0000 0008 0000 0003 0000 0073 bc01  .............s..
-000009a0: 0000 7400 6a01 6401 7402 8800 6a03 8301  ..t.j.d.t...j...
-000009b0: 9b00 9d02 6402 6403 8d02 8f24 0100 8800  ....d.d....$....
-000009c0: 6a04 6400 7501 7218 8800 a004 a100 8904  j.d.u.r.........
-000009d0: 6e12 7405 8800 6a06 6404 8302 7224 8800  n.t...j.d...r$..
-000009e0: 6a06 a004 a100 8904 6e06 7400 6a07 6405  j.......n.t.j.d.
-000009f0: 6406 8d01 8904 5700 6400 0400 0400 8303  d.....W.d.......
-00000a00: 0100 6e08 3100 7334 7701 0100 0100 0100  ..n.1.s4w.......
-00000a10: 5900 0100 7400 6a01 6407 6408 6403 8d02  Y...t.j.d.d.d...
-00000a20: 8f24 0100 8800 6a08 6400 7501 724b 8800  .$....j.d.u.rK..
-00000a30: a008 a100 8905 6e12 7405 8800 6a06 6409  ......n.t...j.d.
-00000a40: 8302 7257 8800 6a06 a008 a100 8905 6e06  ..rW..j.......n.
-00000a50: 7400 6a07 6405 6406 8d01 8905 5700 6400  t.j.d.d.....W.d.
-00000a60: 0400 0400 8303 0100 6e08 3100 7367 7701  ........n.1.sgw.
-00000a70: 0100 0100 0100 5900 0100 7400 6a01 640a  ......Y...t.j.d.
-00000a80: 640b 640c 640d 8d03 8f3c 0100 7400 6a09  d.d.d....<..t.j.
-00000a90: 640e 8800 6a06 9b00 9d02 640f 6410 8d02  d...j.....d.d...
-00000aa0: 0100 7400 6a0a 640f 6411 6412 8d02 8902  ..t.j.d.d.d.....
-00000ab0: 7400 6a0a 640f 6413 6412 8d02 8903 7400  t.j.d.d.d.....t.
-00000ac0: 6a0a 640f 6414 6412 8d02 8906 8800 6a0b  j.d.d.d.......j.
-00000ad0: 72a9 7400 6a0c 6415 8800 6a0b 9b00 9d02  r.t.j.d...j.....
-00000ae0: 740d 8800 6a0b 8301 a00e a100 6416 6417  t...j.......d.d.
-00000af0: 8d03 0100 5700 6400 0400 0400 8303 0100  ....W.d.........
-00000b00: 6e08 3100 73b3 7701 0100 0100 0100 5900  n.1.s.w.......Y.
-00000b10: 0100 6418 740f 7410 7411 6602 1900 6419  ..d.t.t.t.f...d.
-00000b20: 740f 7410 7411 6602 1900 6604 8700 8701  t.t.t.f...f.....
-00000b30: 8702 8703 8704 8705 8706 6607 641a 641b  ..........f.d.d.
-00000b40: 840c 7d03 7412 7c03 6701 7413 8300 8802  ..}.t.|.g.t.....
-00000b50: 8804 8805 8803 8806 6805 8303 5300 291c  ........h...S.).
-00000b60: 4e75 0e00 0000 f09f 91a9 2020 5072 6f6d  Nu........  Prom
-00000b70: 7074 3a20 da06 7072 6f6d 7074 a902 da05  pt: ..prompt....
-00000b80: 6c61 6265 6cda 0765 6c65 6d5f 6964 da0b  label..elem_id..
-00000b90: 626c 6f63 6b5f 696e 7075 74da 00a9 0172  block_input....r
-00000ba0: 3200 0000 7504 0000 00f0 9f92 bbda 0872  2...u..........r
-00000bb0: 6573 706f 6e73 65da 0c62 6c6f 636b 5f6f  esponse..block_o
-00000bc0: 7574 7075 747a 032e 2e2e da08 6164 7661  utputz......adva
-00000bd0: 6e63 6564 46a9 0372 3200 0000 7233 0000  ncedF..r2...r3..
-00000be0: 00da 046f 7065 6e7a 0942 6163 6b65 6e64  ...openz.Backend
-00000bf0: 3a20 da04 6a73 6f6e a901 7233 0000 00da  : ..json..r3....
-00000c00: 0549 6e70 7574 2902 7233 0000 0072 3200  .Input).r3...r2.
-00000c10: 0000 da06 4f75 7470 7574 7a0e 5072 6576  ....Outputz.Prev
-00000c20: 696f 7573 2054 7269 616c 7a0a 5465 6d70  ious Trialz.Temp
-00000c30: 6c61 7465 3a20 da05 696e 6e65 7229 0372  late: ..inner).r
-00000c40: 3200 0000 da05 7661 6c75 6572 3300 0000  2.....valuer3...
-00000c50: 7229 0000 0072 1200 0000 6301 0000 0000  r)...r....c.....
-00000c60: 0000 0000 0000 0013 0000 000a 0000 0013  ................
-00000c70: 0000 0073 6401 0000 6401 7d01 8800 6a00  ...sd...d.}...j.
-00000c80: 8801 6602 7c00 7401 1900 7601 720d 6900  ..f.|.t...v.r.i.
-00000c90: 5300 8800 6a00 8801 6402 1800 6602 7c00  S...j...d...f.|.
-00000ca0: 7401 1900 7600 7228 7c00 7401 1900 8800  t...v.r(|.t.....
-00000cb0: 6a00 8801 6402 1800 6602 1900 6403 1900  j...d...f...d...
-00000cc0: 6402 1900 6a02 7d01 7403 7c00 7401 1900  d...j.}.t.|.t...
-00000cd0: 8800 6a00 8801 6602 1900 8301 7d02 7c00  ..j...f.....}.|.
-00000ce0: 7401 1900 8800 6a00 8801 6602 1900 6403  t.....j...f...d.
-00000cf0: 1900 5c04 7d03 7d04 7d05 7d06 6404 7404  ..\.}.}.}.}.d.t.
-00000d00: 6405 7404 6604 6406 6407 8404 7d07 6404  d.t.f.d.d...}.d.
-00000d10: 7404 6405 7404 6604 6408 6409 8404 7d08  t.d.t.f.d.d...}.
-00000d20: 640a 7d09 7405 7c04 6a02 7c01 8302 4400  d.}.t.|.j.|...D.
-00000d30: 5d0e 5c02 7d0a 7d0b 7c0a 7c0b 6b03 7266  ].\.}.}.|.|.k.rf
-00000d40: 0100 6e05 7c09 6402 3700 7d09 715c 7c09  ..n.|.d.7.}.q\|.
-00000d50: 640b 6b04 7279 640c 7c04 6a02 7c09 6400  d.k.ryd.|.j.|.d.
-00000d60: 8502 1900 1700 7d0c 6e03 7c04 6a02 7d0c  ......}.n.|.j.}.
-00000d70: 7c02 6402 6b02 7283 6700 7d0d 6e19 7c00  |.d.k.r.g.}.n.|.
-00000d80: 7401 1900 8800 6a00 8801 6602 1900 7c02  t.....j...f...|.
-00000d90: 640d 1800 1900 5c04 7d0e 7d0f 7d10 7d11  d.....\.}.}.}.}.
-00000da0: 7c0e 7c0f 6a02 7c10 7c11 640e 9c04 7d0d  |.|.j.|.|.d...}.
-00000db0: 8802 7c07 7c03 8301 8804 7c08 7c0c 8301  ..|.|.....|.|...
-00000dc0: 8805 7c08 7c06 8301 8803 7c07 7c05 8301  ..|.|.....|.|...
-00000dd0: 8806 7c0d 6905 7d12 7c12 5300 290f 4e72  ..|.i.}.|.S.).Nr
-00000de0: 3500 0000 720d 0000 00e9 ffff ffff da01  5...r...........
-00000df0: 7372 1200 0000 6301 0000 0000 0000 0000  sr....c.........
-00000e00: 0000 0001 0000 0003 0000 0053 0000 0073  ...........S...s
-00000e10: 1600 0000 7400 7c00 7401 8302 7209 6401  ....t.|.t...r.d.
-00000e20: 7c00 6901 5300 7c00 5300 2902 4eda 0673  |.i.S.|.S.).N..s
-00000e30: 7472 696e 6729 02da 0a69 7369 6e73 7461  tring)...isinsta
-00000e40: 6e63 6572 1b00 0000 a901 7243 0000 0072  ncer......rC...r
-00000e50: 1500 0000 7215 0000 0072 1600 0000 da06  ....r....r......
-00000e60: 666f 726d 6174 8600 0000 7306 0000 000a  format....s.....
-00000e70: 0108 0104 017a 2f74 6f5f 6772 6164 696f  .....z/to_gradio
-00000e80: 5f62 6c6f 636b 2e3c 6c6f 6361 6c73 3e2e  _block.<locals>.
-00000e90: 7570 6461 7465 2e3c 6c6f 6361 6c73 3e2e  update.<locals>.
-00000ea0: 666f 726d 6174 6301 0000 0000 0000 0000  formatc.........
-00000eb0: 0000 0001 0000 0002 0000 0053 0000 0073  ...........S...s
-00000ec0: 0800 0000 7400 7c00 8301 5300 7213 0000  ....t.|...S.r...
-00000ed0: 0029 0172 1b00 0000 7246 0000 0072 1500  .).r....rF...r..
-00000ee0: 0000 7215 0000 0072 1600 0000 da04 6d61  ..r....r......ma
-00000ef0: 726b 8b00 0000 7302 0000 0008 017a 2d74  rk....s......z-t
-00000f00: 6f5f 6772 6164 696f 5f62 6c6f 636b 2e3c  o_gradio_block.<
-00000f10: 6c6f 6361 6c73 3e2e 7570 6461 7465 2e3c  locals>.update.<
-00000f20: 6c6f 6361 6c73 3e2e 6d61 726b 7201 0000  locals>.markr...
-00000f30: 00e9 1e00 0000 7a04 2e2e 2e0a e902 0000  ......z.........
-00000f40: 0029 04da 0569 6e70 7574 7230 0000 0072  .)...inputr0...r
-00000f50: 3700 0000 da06 6f75 7470 7574 2906 da03  7.....output)...
-00000f60: 5f69 64da 0861 6c6c 5f64 6174 6172 3000  _id..all_datar0.
-00000f70: 0000 da03 6c65 6e72 0400 0000 da03 7a69  ....lenr......zi
-00000f80: 7029 1372 2900 0000 da0d 7072 6576 5f72  p).r).....prev_r
-00000f90: 6571 7565 7374 5fda 0674 7269 616c 73da  equest_..trials.
-00000fa0: 0669 6e70 7574 5fda 0872 6571 7565 7374  .input_..request
-00000fb0: 5fda 0972 6573 706f 6e73 655f da07 6f75  _..response_..ou
-00000fc0: 7470 7574 5f72 4700 0000 7248 0000 00da  tput_rG...rH....
-00000fd0: 016a da01 61da 0162 da0a 6e65 775f 7072  .j..a..b..new_pr
-00000fe0: 6f6d 7074 da0f 7072 6576 696f 7573 5f74  ompt..previous_t
-00000ff0: 7269 616c 73da 0c74 7269 616c 5f69 6e70  rials..trial_inp
-00001000: 7574 5fda 0e74 7269 616c 5f72 6571 7565  ut_..trial_reque
-00001010: 7374 5fda 0f74 7269 616c 5f72 6573 706f  st_..trial_respo
-00001020: 6e73 655f da0d 7472 6961 6c5f 6f75 7470  nse_..trial_outp
-00001030: 7574 5fda 0372 6574 a907 722d 0000 0072  ut_..ret..r-...r
-00001040: 2e00 0000 724b 0000 0072 3c00 0000 7230  ....rK...r<...r0
-00001050: 0000 00da 0672 6573 756c 74da 0574 7269  .....result..tri
-00001060: 616c 7215 0000 0072 1600 0000 da06 7570  alr....r......up
-00001070: 6461 7465 7c00 0000 734c 0000 0004 0112  date|...sL......
-00001080: 0104 0116 0220 0116 011e 0112 0212 0504  ..... ..........
-00001090: 0314 0108 0104 010a 0108 0214 0106 0208  ................
-000010a0: 0206 0102 0202 0102 ff08 0202 fe06 020c  ................
-000010b0: fe02 0404 0102 0102 0106 fc08 0708 0108  ................
-000010c0: 0108 0104 0104 fb04 077a 1f74 6f5f 6772  .........z.to_gr
-000010d0: 6164 696f 5f62 6c6f 636b 2e3c 6c6f 6361  adio_block.<loca
-000010e0: 6c73 3e2e 7570 6461 7465 2914 da02 6772  ls>.update)...gr
-000010f0: da09 4163 636f 7264 696f 6e72 1b00 0000  ..Accordionr....
-00001100: da03 5f66 6e72 3400 0000 da07 6861 7361  .._fnr4.....hasa
-00001110: 7474 72da 0762 6163 6b65 6e64 da07 5465  ttr..backend..Te
-00001120: 7874 626f 7872 3800 0000 da08 4d61 726b  xtboxr8.....Mark
-00001130: 646f 776e da04 4a53 4f4e da0d 7465 6d70  down..JSON..temp
-00001140: 6c61 7465 5f66 696c 65da 0443 6f64 6572  late_file..Coder
-00001150: 3b00 0000 da04 7265 6164 7206 0000 0072  ;.....readr....r
-00001160: 0b00 0000 7204 0000 0072 2000 0000 7227  ....r....r ...r'
-00001170: 0000 0029 0472 2d00 0000 722e 0000 0072  ...).r-...r....r
-00001180: 2f00 0000 7264 0000 0072 1500 0000 7261  /...rd...r....ra
-00001190: 0000 0072 1600 0000 da0f 746f 5f67 7261  ...r......to_gra
-000011a0: 6469 6f5f 626c 6f63 6b4f 0000 0073 3e00  dio_blockO...s>.
-000011b0: 0000 1c06 0a01 0a01 0c01 0c01 0c02 0280  ................
-000011c0: 1cfa 1008 0a01 0a01 0c01 0c01 0c02 0280  ................
-000011d0: 1cfa 1208 1601 0e01 0e01 0e01 0602 0402  ................
-000011e0: 0a01 0c01 0201 06fd 0280 1cf8 3217 1a32  ............2..2
-000011f0: 7270 0000 00da 0770 726f 6d70 7473 6301  rp.....promptsc.
-00001200: 0000 0000 0000 0000 0000 0005 0000 0006  ................
-00001210: 0000 0043 0000 0073 5200 0000 7400 8300  ...C...sR...t...
-00001220: 7d01 6900 7d02 7c00 4400 5d1f 7d03 7c02  }.i.}.|.D.].}.|.
-00001230: a001 7c03 6a02 6401 a102 0100 7c02 7c03  ..|.j.d.....|.|.
-00001240: 6a02 1900 7d04 7c01 a003 7404 7c03 7c04  j...}.|...t.|.|.
-00001250: 8302 a101 7d01 7c02 7c03 6a02 0500 1900  ....}.|.|.j.....
-00001260: 6402 3700 0300 3c00 7107 7c01 5300 2903  d.7...<.q.|.S.).
-00001270: 4e72 0100 0000 720d 0000 0029 0572 2000  Nr....r....).r .
-00001280: 0000 da0a 7365 7464 6566 6175 6c74 724d  ....setdefaultrM
-00001290: 0000 0072 2600 0000 7270 0000 0029 0572  ...r&...rp...).r
-000012a0: 7100 0000 da04 636f 6e73 da05 636f 756e  q.....cons..coun
-000012b0: 74da 0170 722e 0000 0072 1500 0000 7215  t..pr....r....r.
-000012c0: 0000 0072 1600 0000 da0c 6368 6169 6e5f  ...r......chain_
-000012d0: 626c 6f63 6b73 b100 0000 7310 0000 0006  blocks....s.....
-000012e0: 0104 0108 010e 010a 0110 0114 0104 0172  ...............r
-000012f0: 7600 0000 da0e 4f50 454e 4149 5f41 5049  v.....OPENAI_API
-00001300: 5f4b 4559 da04 6b65 7973 6301 0000 0000  _KEY..keysc.....
-00001310: 0000 0000 0000 0003 0000 0008 0000 0003  ................
-00001320: 0000 0073 1401 0000 7400 6401 6402 8400  ...s....t.d.d...
-00001330: 7c00 4400 8301 8301 720b 6400 5300 6900  |.D.....r.d.S.i.
-00001340: 8900 7401 6a02 6403 6404 6405 6406 8d03  ..t.j.d.d.d.d...
-00001350: 8f5a 0100 6407 7c00 7600 7233 6407 7403  .Z..d.|.v.r3d.t.
-00001360: 6a04 7601 7233 7401 6a05 7403 6a04 a006  j.v.r3t.j.t.j...
-00001370: 6407 a101 6408 6404 6409 640a 8d04 8800  d...d.d.d.d.....
-00001380: 6407 3c00 7401 a007 640b a101 0100 640c  d.<.t...d.....d.
-00001390: 7c00 7600 724b 7401 a007 640d a101 0100  |.v.rKt...d.....
-000013a0: 7401 6a05 7403 6a04 a006 640c a101 640e  t.j.t.j...d...d.
-000013b0: 640f 6409 640a 8d04 8800 640c 3c00 6410  d.d.d.....d.<.d.
-000013c0: 7c00 7600 7263 7401 a007 6411 a101 0100  |.v.rct...d.....
-000013d0: 7401 6a05 7403 6a04 a006 6410 a101 6412  t.j.t.j...d...d.
-000013e0: 640f 6409 640a 8d04 8800 6410 3c00 7401  d.d.d.....d.<.t.
-000013f0: a008 6413 a101 7d01 5700 6400 0400 0400  ..d...}.W.d.....
-00001400: 8303 0100 6e08 3100 7372 7701 0100 0100  ....n.1.srw.....
-00001410: 0100 5900 0100 8700 6601 6414 6415 8408  ..Y.....f.d.d...
-00001420: 7d02 7c01 6a09 7c02 740a 8800 a00b a100  }.|.j.|.t.......
-00001430: 8301 6416 8d02 0100 6400 5300 2917 4e63  ..d.....d.S.).Nc
-00001440: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00001450: 0400 0000 5300 0000 7316 0000 0067 007c  ....S...s....g.|
-00001460: 005d 077d 017c 0174 006a 0176 0091 0271  .].}.|.t.j.v...q
-00001470: 0253 0072 1500 0000 2902 da02 6f73 da07  .S.r....)...os..
-00001480: 656e 7669 726f 6e29 02da 022e 30da 016b  environ)....0..k
-00001490: 7215 0000 0072 1500 0000 7216 0000 00da  r....r....r.....
-000014a0: 0a3c 6c69 7374 636f 6d70 3ebd 0000 0073  .<listcomp>....s
-000014b0: 0200 0000 1600 7a1c 6170 695f 6b65 7973  ......z.api_keys
-000014c0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
-000014d0: 6f6d 703e 7a08 4150 4920 4b65 7973 723c  omp>z.API Keysr<
-000014e0: 0000 0046 723a 0000 0072 7700 0000 7a0a  ...Fr:...rw...z.
-000014f0: 4f70 656e 4149 204b 6579 da08 7061 7373  OpenAI Key..pass
-00001500: 776f 7264 2903 7232 0000 0072 3300 0000  word).r2...r3...
-00001510: da04 7479 7065 7a56 0a20 2020 2020 2020  ..typezV.       
-00001520: 2020 2020 202a 205b 4f70 656e 4149 204b       * [OpenAI K
-00001530: 6579 5d28 6874 7470 733a 2f2f 706c 6174  ey](https://plat
-00001540: 666f 726d 2e6f 7065 6e61 692e 636f 6d2f  form.openai.com/
-00001550: 6163 636f 756e 742f 6170 692d 6b65 7973  account/api-keys
-00001560: 290a 2020 2020 2020 2020 2020 2020 da06  ).            ..
-00001570: 4846 5f4b 4559 7a56 0a20 2020 2020 2020  HF_KEYzV.       
-00001580: 2020 2020 202a 205b 4875 6767 696e 6720       * [Hugging 
-00001590: 4661 6365 204b 6579 5d28 6874 7470 733a  Face Key](https:
-000015a0: 2f2f 6875 6767 696e 6766 6163 652e 636f  //huggingface.co
-000015b0: 2f73 6574 7469 6e67 732f 746f 6b65 6e73  /settings/tokens
-000015c0: 290a 2020 2020 2020 2020 2020 2020 7a10  ).            z.
-000015d0: 4875 6767 696e 6720 4661 6365 204b 6579  Hugging Face Key
-000015e0: 7240 0000 00da 0853 4552 505f 4b45 597a  r@.....SERP_KEYz
-000015f0: 4b0a 2020 2020 2020 2020 2020 2020 2a20  K.            * 
-00001600: 5b53 6561 7263 6820 4b65 795d 2868 7474  [Search Key](htt
-00001610: 7073 3a2f 2f73 6572 7061 7069 2e63 6f6d  ps://serpapi.com
-00001620: 2f75 7365 7273 2f73 6967 6e5f 696e 290a  /users/sign_in).
-00001630: 2020 2020 2020 2020 2020 2020 7a0a 5365              z.Se
-00001640: 6172 6368 204b 6579 da04 5361 7665 6301  arch Key..Savec.
-00001650: 0000 0000 0000 0000 0000 0003 0000 0004  ................
-00001660: 0000 0013 0000 0073 3c00 0000 8800 a000  .......s<.......
-00001670: a100 4400 5d17 5c02 7d01 7d02 7c00 7c02  ..D.].\.}.}.|.|.
-00001680: 1900 6400 7501 721b 7c00 7c02 1900 6401  ..d.u.r.|.|...d.
-00001690: 6b03 721b 7c00 7c02 1900 7401 6a02 7c01  k.r.|.|...t.j.|.
-000016a0: 3c00 7104 6900 5300 2902 4e72 3500 0000  <.q.i.S.).Nr5...
-000016b0: 2903 da05 6974 656d 7372 7900 0000 727a  )...itemsry...rz
-000016c0: 0000 0029 0372 2900 0000 727c 0000 00da  ...).r)...r|....
-000016d0: 0176 a901 da09 6b65 795f 6e61 6d65 7372  .v....key_namesr
-000016e0: 1500 0000 7216 0000 00da 0761 7069 5f72  ....r......api_r
-000016f0: 756e ec00 0000 730a 0000 0010 0118 010e  un....s.........
-00001700: 0102 8004 017a 1961 7069 5f6b 6579 732e  .....z.api_keys.
-00001710: 3c6c 6f63 616c 733e 2e61 7069 5f72 756e  <locals>.api_run
-00001720: 2901 7223 0000 0029 0cda 0361 6c6c 7265  ).r#...)...allre
-00001730: 0000 0072 6600 0000 7279 0000 0072 7a00  ...rf...ry...rz.
-00001740: 0000 726a 0000 00da 0367 6574 726b 0000  ..rj.....getrk..
-00001750: 00da 0642 7574 746f 6eda 0563 6c69 636b  ...Button..click
-00001760: 7227 0000 00da 0676 616c 7565 7329 0372  r'.....values).r
-00001770: 7800 0000 da07 6170 695f 6274 6e72 8700  x.....api_btnr..
-00001780: 0000 7215 0000 0072 8500 0000 7216 0000  ..r....r....r...
-00001790: 00da 0861 7069 5f6b 6579 73bc 0000 0073  ...api_keys....s
-000017a0: 4c00 0000 1201 0401 0401 1202 1201 0401  L...............
-000017b0: 0a01 0201 0201 0201 0afc 0406 0201 04ff  ................
-000017c0: 0806 0401 0201 04ff 0406 0a01 0201 0201  ................
-000017d0: 0201 0afc 0807 0401 0201 04ff 0405 0a01  ................
-000017e0: 0201 0201 0201 0afc 0c07 1cd7 0c2b 1a06  .............+..
-000017f0: 728e 0000 0072 3500 0000 721e 0000 0072  r....r5...r....r
-00001800: 3000 0000 da08 6578 616d 706c 6573 da0a  0.....examples..
-00001810: 7375 6270 726f 6d70 7473 da06 6669 656c  subprompts..fiel
-00001820: 6473 da0d 696e 6974 6961 6c5f 7374 6174  ds..initial_stat
-00001830: 65da 086f 7574 5f74 7970 65da 0b64 6573  e..out_type..des
-00001840: 6372 6970 7469 6f6e da04 636f 6465 630a  cription..codec.
-00001850: 0000 0000 0000 0000 0000 000f 0000 0009  ................
-00001860: 0000 0003 0000 0073 ac01 0000 6401 6402  .......s....d.d.
-00001870: 8400 7400 a001 8805 a101 6a02 4400 8301  ..t.......j.D...
-00001880: 8901 7403 6a04 7405 6403 1700 7c09 1700  ..t.j.t.d...|...
-00001890: 7403 6a06 a007 a100 6404 8d02 8fb3 7d0a  t.j.....d.....}.
-000018a0: 7408 8300 0100 7409 8300 8900 7403 a00a  t.....t.....t...
-000018b0: 8802 a101 8906 8800 a00b 7409 8806 6801  ..........t...h.
-000018c0: 8806 6801 6405 8d02 a101 8900 7403 a00c  ..h.d.......t...
-000018d0: 7c07 a101 0100 740d 6406 6402 8400 8801  |.....t.d.d.....
-000018e0: 4400 8301 8301 8903 7403 6a0e 7c01 8803  D.......t.j.|...
-000018f0: 6407 8d02 7d01 7403 6a0f 6408 6409 8d01  d...}.t.j.d.d...
-00001900: 7d0b 8800 a010 8803 a101 8900 8800 a00b  }...............
-00001910: 7411 7c02 8301 a101 8900 7403 6a12 640a  t.|.......t.j.d.
-00001920: 640b 640c 8d02 8f17 0100 7c05 640d 6b02  d.d.......|.d.k.
-00001930: 7266 7403 6a13 6e02 7403 6a0c 7d0c 7c0c  rft.j.n.t.j.}.|.
-00001940: 640e 640f 8d01 8904 5700 6410 0400 0400  d.d.....W.d.....
-00001950: 8303 0100 6e08 3100 7378 7701 0100 0100  ....n.1.sxw.....
-00001960: 0100 5900 0100 6411 7414 7415 7416 6602  ..Y...d.t.t.t.f.
-00001970: 1900 6412 7414 7415 7416 6602 1900 6604  ..d.t.t.t.f...f.
-00001980: 8704 8706 6602 6413 6414 840c 7d0d 8800  ....f.d.d...}...
-00001990: a00b 7409 7c0d 6701 7417 8300 8804 6801  ..t.|.g.t.....h.
-000019a0: 8303 a101 8900 8700 8701 8702 8703 8705  ................
-000019b0: 8706 6606 6415 6416 8408 7d0e 7c0b 6a18  ..f.d.d...}.|.j.
-000019c0: 7c0e 8800 6a19 8800 6a1a 6405 8d03 0100  |...j...j.d.....
-000019d0: 7c08 72c4 7403 6a1b 7c08 6417 640e 6418  |.r.t.j.|.d.d.d.
-000019e0: 8d03 0100 5700 6410 0400 0400 8303 0100  ....W.d.........
-000019f0: 7c0a 5300 5700 6410 0400 0400 8303 0100  |.S.W.d.........
-00001a00: 7c0a 5300 3100 73cf 7701 0100 0100 0100  |.S.1.s.w.......
-00001a10: 5900 0100 7c0a 5300 2919 6152 0200 000a  Y...|.S.).aR....
-00001a20: 2020 2020 436f 6e73 7472 7563 7473 2061      Constructs a
-00001a30: 2067 7261 6469 6f20 636f 6d70 6f6e 656e   gradio componen
-00001a40: 7420 746f 2073 686f 7720 6120 7072 6f6d  t to show a prom
-00001a50: 7074 2063 6861 696e 2e0a 0a20 2020 2041  pt chain...    A
-00001a60: 7267 733a 0a20 2020 2020 2020 2070 726f  rgs:.        pro
-00001a70: 6d70 743a 2041 2070 726f 6d70 7420 6f72  mpt: A prompt or
-00001a80: 2070 726f 6d70 7420 6368 6169 6e20 746f   prompt chain to
-00001a90: 2064 6973 706c 6179 2e0a 2020 2020 2020   display..      
-00001aa0: 2020 6578 616d 706c 6573 3a20 4120 6c69    examples: A li
-00001ab0: 7374 206f 6620 6578 616d 706c 6520 696e  st of example in
-00001ac0: 7075 7473 2c20 6569 7468 6572 2073 7472  puts, either str
-00001ad0: 696e 6720 6f72 2074 7570 6c65 7320 6f66  ing or tuples of
-00001ae0: 2066 6965 6c64 730a 2020 2020 2020 2020   fields.        
-00001af0: 7375 6270 726f 6d70 7473 3a20 5468 6520  subprompts: The 
-00001b00: 6050 726f 6d70 7460 206f 626a 6563 7473  `Prompt` objects
-00001b10: 2074 6f20 6469 7370 6c61 792e 0a20 2020   to display..   
-00001b20: 2020 2020 2066 6965 6c64 733a 2054 6865       fields: The
-00001b30: 206e 616d 6573 206f 6620 7468 6520 6669   names of the fi
-00001b40: 656c 6420 696e 7075 7420 746f 2074 6865  eld input to the
-00001b50: 2070 726f 6d70 742e 0a20 2020 2020 2020   prompt..       
-00001b60: 2069 6e69 7469 616c 5f73 7461 7465 3a20   initial_state: 
-00001b70: 466f 7220 7374 6174 6566 756c 2070 726f  For stateful pro
-00001b80: 6d70 7473 2c20 7468 6520 696e 6974 6961  mpts, the initia
-00001b90: 6c20 7661 6c75 652e 0a20 2020 2020 2020  l value..       
-00001ba0: 206f 7574 5f74 7970 653a 2074 7970 6520   out_type: type 
-00001bb0: 6f66 2066 696e 616c 206f 7574 7075 740a  of final output.
-00001bc0: 2020 2020 2020 2020 6b65 7973 3a20 7573          keys: us
-00001bd0: 6572 206b 6579 7320 7265 7175 6972 6564  er keys required
-00001be0: 0a20 2020 2020 2020 2064 6573 6372 6970  .        descrip
-00001bf0: 7469 6f6e 3a20 6465 7363 7269 7074 696f  tion: descriptio
-00001c00: 6e20 6f66 2074 6865 206d 6f64 656c 0a20  n of the model. 
-00001c10: 2020 2020 2020 2063 6f64 653a 2063 6f64         code: cod
-00001c20: 6520 746f 2064 6973 706c 6179 0a20 2020  e to display.   
-00001c30: 2020 2020 2063 7373 203a 2061 6464 6974       css : addit
-00001c40: 696f 6e61 6c20 6373 730a 0a20 2020 2052  ional css..    R
-00001c50: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-00001c60: 4772 6164 696f 2062 6c6f 636b 0a20 2020  Gradio block.   
-00001c70: 2063 0100 0000 0000 0000 0000 0000 0200   c..............
-00001c80: 0000 0400 0000 5300 0000 7318 0000 0067  ......S...s....g
-00001c90: 007c 005d 087d 017c 0164 006b 0372 027c  .|.].}.|.d.k.r.|
-00001ca0: 0191 0271 0253 0029 01da 0573 7461 7465  ...q.S.)...state
-00001cb0: 7215 0000 0029 0272 7b00 0000 da03 6172  r....).r{.....ar
-00001cc0: 6772 1500 0000 7215 0000 0072 1600 0000  gr....r....r....
-00001cd0: 727d 0000 0013 0100 00f3 0200 0000 1800  r}..............
-00001ce0: 7a18 7368 6f77 2e3c 6c6f 6361 6c73 3e2e  z.show.<locals>.
-00001cf0: 3c6c 6973 7463 6f6d 703e da01 0a29 02da  <listcomp>...)..
-00001d00: 0363 7373 da05 7468 656d 6529 0272 2300  .css..theme).r#.
-00001d10: 0000 7224 0000 0063 0100 0000 0000 0000  ..r$...c........
-00001d20: 0000 0000 0200 0000 0500 0000 5300 0000  ............S...
-00001d30: 7318 0000 0067 007c 005d 087d 0174 006a  s....g.|.].}.t.j
-00001d40: 017c 0164 008d 0191 0271 0253 0029 0172  .|.d.....q.S.).r
-00001d50: 3600 0000 2902 7265 0000 0072 6a00 0000  6...).re...rj...
-00001d60: 2902 727b 0000 00da 0166 7215 0000 0072  ).r{.....fr....r
-00001d70: 1500 0000 7216 0000 0072 7d00 0000 2201  ....r....r}...".
-00001d80: 0000 7298 0000 0029 0272 8f00 0000 7223  ..r....).r....r#
-00001d90: 0000 00da 0352 756e 7236 0000 0075 0600  .....Runr6...u..
-00001da0: 0000 e29c 94ef b88f 7262 0000 0072 3100  ........rb...r1.
-00001db0: 0000 723c 0000 0072 4000 0000 723d 0000  ..r<...r@...r=..
-00001dc0: 004e 7229 0000 0072 1200 0000 6301 0000  .Nr)...r....c...
-00001dd0: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-00001de0: 0013 0000 0073 1400 0000 7c00 7400 1900  .....s....|.t...
-00001df0: 7d01 8801 7c01 8800 7c01 6902 5300 7213  }...|...|.i.S.r.
-00001e00: 0000 0029 01da 0c66 696e 616c 5f6f 7574  ...)...final_out
-00001e10: 7075 7429 0272 2900 0000 da05 6669 6e61  put).r).....fina
-00001e20: 6c29 0272 4c00 0000 7296 0000 0072 1500  l).rL...r....r..
-00001e30: 0000 7216 0000 00da 096f 7574 7075 745f  ..r......output_
-00001e40: 666e 2f01 0000 7304 0000 0008 010c 017a  fn/...s........z
-00001e50: 1773 686f 772e 3c6c 6f63 616c 733e 2e6f  .show.<locals>.o
-00001e60: 7574 7075 745f 666e 6301 0000 0000 0000  utput_fnc.......
-00001e70: 0000 0000 0003 0000 0008 0000 0033 0000  .............3..
-00001e80: 0073 ac00 0000 8100 8700 6601 6401 6402  .s........f.d.d.
-00001e90: 8408 7400 8802 8804 8302 4400 8301 7d01  ..t.......D...}.
-00001ea0: 8803 6400 7501 7217 8800 8806 1900 7c01  ..d.u.r.......|.
-00001eb0: 6403 3c00 7401 6404 8301 8f2b 0100 8805  d.<.t.d....+....
-00001ec0: 6405 6900 7c01 a401 8e01 a002 a100 4400  d.i.|.........D.
-00001ed0: 5d19 7d02 7403 7404 6a05 8301 8800 7406  ].}.t.t.j.....t.
-00001ee0: 3c00 7c02 8800 7407 3c00 8801 a008 8800  <.|...t.<.......
-00001ef0: a101 5600 0100 7c02 6400 7501 723e 0100  ..V...|.d.u.r>..
-00001f00: 6e01 7125 5700 6400 0400 0400 8303 0100  n.q%W.d.........
-00001f10: 6e08 3100 7349 7701 0100 0100 0100 5900  n.1.sIw.......Y.
-00001f20: 0100 8801 a008 8800 a101 5600 0100 6400  ..........V...d.
-00001f30: 5300 2906 4e63 0100 0000 0000 0000 0000  S.).Nc..........
-00001f40: 0000 0300 0000 0500 0000 1300 0000 731a  ..............s.
-00001f50: 0000 0069 007c 005d 095c 027d 017d 027c  ...i.|.].\.}.}.|
-00001f60: 0188 007c 0219 0093 0271 0253 0072 1500  ...|.....q.S.r..
-00001f70: 0000 7215 0000 0029 0372 7b00 0000 727c  ..r....).r{...r|
-00001f80: 0000 0072 8400 0000 a901 7229 0000 0072  ...r......r)...r
-00001f90: 1500 0000 7216 0000 00da 0a3c 6469 6374  ....r......<dict
-00001fa0: 636f 6d70 3e36 0100 0073 0200 0000 1a00  comp>6...s......
-00001fb0: 7a25 7368 6f77 2e3c 6c6f 6361 6c73 3e2e  z%show.<locals>.
-00001fc0: 7275 6e2e 3c6c 6f63 616c 733e 2e3c 6469  run.<locals>.<di
-00001fd0: 6374 636f 6d70 3e72 9600 0000 da04 7465  ctcomp>r......te
-00001fe0: 6d70 7215 0000 0029 0972 5000 0000 720c  mpr....).rP...r.
-00001ff0: 0000 00da 0772 756e 5f67 656e da04 6469  .....run_gen..di
-00002000: 6374 720e 0000 00da 0c70 726f 6d70 745f  ctr......prompt_
-00002010: 7374 6f72 6572 4e00 0000 729e 0000 0072  storerN...r....r
-00002020: 2b00 0000 2903 7229 0000 00da 0d70 726f  +...).r).....pro
-00002030: 6d70 745f 696e 7075 7473 724c 0000 0029  mpt_inputsrL...)
-00002040: 06da 0b63 6f6e 7374 7275 6374 6f72 7291  ...constructorr.
-00002050: 0000 0072 9200 0000 7223 0000 0072 3000  ...r....r#...r0.
-00002060: 0000 7296 0000 0072 a100 0000 7216 0000  ..r....r....r...
-00002070: 00da 0372 756e 3501 0000 731e 0000 0002  ...run5...s.....
-00002080: 8018 0108 010c 010a 0216 020e 0108 010c  ................
-00002090: 0108 0104 0102 ff02 801c fa10 087a 1173  .............z.s
-000020a0: 686f 772e 3c6c 6f63 616c 733e 2e72 756e  how.<locals>.run
-000020b0: da06 7079 7468 6f6e 2902 da08 6c61 6e67  ..python)...lang
-000020c0: 7561 6765 7233 0000 0029 1cda 0769 6e73  uager3...)...ins
-000020d0: 7065 6374 da0e 6765 7466 756c 6c61 7267  pect..getfullarg
-000020e0: 7370 6563 da04 6172 6773 7265 0000 00da  spec..argsre....
-000020f0: 0642 6c6f 636b 73da 0343 5353 da06 7468  .Blocks..CSS..th
-00002100: 656d 6573 da0a 4d6f 6e6f 6368 726f 6d65  emes..Monochrome
-00002110: 728e 0000 0072 2000 0000 da05 5374 6174  r....r .....Stat
-00002120: 6572 2600 0000 726b 0000 0072 2c00 0000  er&...rk...r,...
-00002130: da08 4578 616d 706c 6573 728a 0000 0072  ..Examplesr....r
-00002140: 2800 0000 7276 0000 0072 6600 0000 726c  (...rv...rf...rl
-00002150: 0000 0072 0600 0000 720b 0000 0072 0400  ...r....r....r..
-00002160: 0000 7227 0000 0072 8b00 0000 7223 0000  ..r'...r....r#..
-00002170: 0072 2400 0000 726e 0000 0029 0f72 3000  .r$...rn...).r0.
-00002180: 0000 728f 0000 0072 9000 0000 7291 0000  ..r....r....r...
-00002190: 0072 9200 0000 7293 0000 0072 7800 0000  .r....r....rx...
-000021a0: 7294 0000 0072 9500 0000 729a 0000 00da  r....r....r.....
-000021b0: 0464 656d 6fda 0971 7565 7279 5f62 746e  .demo..query_btn
-000021c0: da03 7479 7072 a000 0000 72a9 0000 0072  ..typr....r....r
-000021d0: 1500 0000 2907 72a8 0000 0072 9100 0000  ....).r....r....
-000021e0: 7292 0000 0072 2300 0000 724c 0000 0072  r....r#...rL...r
-000021f0: 3000 0000 7296 0000 0072 1600 0000 da04  0...r....r......
-00002200: 7368 6f77 f500 0000 733a 0000 0016 1e1e  show....s:......
-00002210: 0106 0206 020a 0316 010a 0312 030e 010c  ................
-00002220: 010a 010e 0310 0314 010c 011c fe28 0418  .............(..
-00002230: 0416 0214 0f04 0212 010a cd04 3502 fd0a  ............5...
-00002240: ce04 3510 cb04 3572 b800 0000 2925 72ac  ..5...5r....)%r.
-00002250: 0000 0072 7900 0000 da0b 6461 7461 636c  ...ry.....datacl
-00002260: 6173 7365 7372 0200 0000 7203 0000 00da  assesr....r.....
-00002270: 0674 7970 696e 6772 0400 0000 7205 0000  .typingr....r...
-00002280: 0072 0600 0000 7207 0000 0072 0800 0000  .r....r....r....
-00002290: 7209 0000 0072 0a00 0000 da06 6772 6164  r....r......grad
-000022a0: 696f 7265 0000 00da 0d67 7261 6469 6f2e  iore.....gradio.
-000022b0: 626c 6f63 6b73 720b 0000 00da 096d 696e  blocksr......min
-000022c0: 6963 6861 696e 720c 0000 0072 6900 0000  ichainr....ri...
-000022d0: 720e 0000 00da 0462 6173 6572 0f00 0000  r......baser....
-000022e0: 72b0 0000 0072 1000 0000 721d 0000 0072  r....r....r....r
-000022f0: b300 0000 724e 0000 0072 9e00 0000 7220  ....rN...r....r 
-00002300: 0000 00da 0369 6e74 7270 0000 0072 7600  .....intrp...rv.
-00002310: 0000 721b 0000 0072 8e00 0000 72af 0000  ..r....r....r...
-00002320: 0072 b800 0000 7215 0000 0072 1500 0000  .r....r....r....
-00002330: 7215 0000 0072 1600 0000 da08 3c6d 6f64  r....r......<mod
-00002340: 756c 653e 0100 0000 7378 0000 0008 0008  ule>....sx......
-00002350: 0110 0124 0108 020c 010c 020c 020c 0104  ...$............
-00002360: 0202 1710 0102 0710 010a 040a 0102 0310  ................
-00002370: 0104 1b04 fd0c 0102 ff02 0202 fe02 0302  ................
-00002380: fd02 040a fc20 621c 0b04 3b02 0102 0102  ..... b...;.....
-00002390: 0102 0104 0102 0102 0102 0104 f60c 0102  ................
-000023a0: ff16 0202 fe10 0302 fd06 0402 fc02 0502  ................
-000023b0: fb02 0602 fa06 0702 f902 0802 f802 0902  ................
-000023c0: f704 0b0e f5                             .....
+000000d0: 5a19 6503 4700 640e 640f 8400 640f 8302  Z.e.G.d.d...d...
+000000e0: 8301 5a1a 650e a01b 6900 a101 5a1c 650e  ..Z.e...i...Z.e.
+000000f0: a01b 6900 a101 5a1d 6503 4700 6410 6411  ..i...Z.e.G.d.d.
+00000100: 8400 6411 8302 8301 5a1e 651a 8300 6412  ..d.....Z.e...d.
+00000110: 6602 6413 6516 6506 6506 6506 6603 1900  f.d.e.e.e.e.f...
+00000120: 6414 651f 6415 651a 6416 6520 6417 651e  d.e.d.e.d.e d.e.
+00000130: 660a 6418 6419 8405 5a21 0912 642e 641a  f.d.d...Z!..d.d.
+00000140: 6509 6516 6506 6506 6506 6603 1900 1900  e.e.e.e.e.f.....
+00000150: 6416 6520 6417 651e 6606 641b 641c 8405  d.e d.e.f.d.d...
+00000160: 5a22 641d 6801 6601 641e 650a 6523 1900  Z"d.h.f.d.e.e#..
+00000170: 6417 6401 6604 641f 6420 8405 5a24 6421  d.d.f.d.d ..Z$d!
+00000180: 6701 6700 6700 6401 6422 641d 6801 6421  g.g.g.d.d"d.h.d!
+00000190: 6421 6421 6412 660a 6423 6516 6506 6506  d!d!d.f.d#e.e.e.
+000001a0: 6506 6603 1900 6424 650c 6509 6523 1900  e.f...d$e.e.e#..
+000001b0: 6509 650b 6523 1900 1900 6602 1900 6425  e.e.e#....f...d%
+000001c0: 6509 6516 6506 6506 6506 6603 1900 1900  e.e.e.e.e.f.....
+000001d0: 6426 6509 6523 1900 6427 6506 6428 6523  d&e.e#..d'e.d(e#
+000001e0: 641e 650a 6523 1900 6429 6523 642a 6523  d.e.e#..d)e#d*e#
+000001f0: 642b 6523 6416 6520 6417 650e 6a25 6618  d+e#d.e d.e.j%f.
+00000200: 642c 642d 8405 5a26 6401 5300 292f e900  d,d-..Z&d.S.)/..
+00000210: 0000 004e 2902 da09 6461 7461 636c 6173  ...N)...dataclas
+00000220: 73da 0566 6965 6c64 2907 da03 416e 79da  s..field)...Any.
+00000230: 0843 616c 6c61 626c 65da 0444 6963 74da  .Callable..Dict.
+00000240: 044c 6973 74da 0353 6574 da05 5475 706c  .List..Set..Tupl
+00000250: 65da 0555 6e69 6f6e 2901 da05 426c 6f63  e..Union)...Bloc
+00000260: 6b29 01da 0b73 7461 7274 5f63 6861 696e  k)...start_chain
+00000270: e901 0000 0029 01da 104d 696e 6963 6861  .....)...Minicha
+00000280: 696e 436f 6e74 6578 7429 01da 0650 726f  inContext)...Pro
+00000290: 6d70 7461 3901 0000 0a23 636c 6561 6e20  mpta9....#clean 
+000002a0: 6469 762e 666f 726d 207b 626f 7264 6572  div.form {border
+000002b0: 3a20 3070 787d 0a23 7265 7370 6f6e 7365  : 0px}.#response
+000002c0: 207b 626f 7264 6572 3a20 3070 783b 2062   {border: 0px; b
+000002d0: 6163 6b67 726f 756e 643a 2023 6666 6565  ackground: #ffee
+000002e0: 6336 7d0a 2370 726f 6d70 7420 7b62 6f72  c6}.#prompt {bor
+000002f0: 6465 723a 2030 7078 3b62 6163 6b67 726f  der: 0px;backgro
+00000300: 756e 643a 2061 6c69 6365 626c 7565 7d0a  und: aliceblue}.
+00000310: 236a 736f 6e20 7b62 6f72 6465 723a 2030  #json {border: 0
+00000320: 7078 7d0a 7370 616e 2e68 6561 6420 7b66  px}.span.head {f
+00000330: 6f6e 742d 7369 7a65 3a20 3630 7074 3b20  ont-size: 60pt; 
+00000340: 666f 6e74 2d66 616d 696c 793a 2063 7572  font-family: cur
+00000350: 7369 7665 3b7d 0a64 6976 2e67 7261 6469  sive;}.div.gradi
+00000360: 6f2d 636f 6e74 6169 6e65 7220 7b63 6f6c  o-container {col
+00000370: 6f72 3a20 626c 6163 6b7d 0a64 6976 2e66  or: black}.div.f
+00000380: 6f72 6d20 7b62 6163 6b67 726f 756e 643a  orm {background:
+00000390: 2069 6e68 6572 6974 7d0a 6469 762e 666f   inherit}.div.fo
+000003a0: 726d 2064 6976 2e62 6c6f 636b 207b 7061  rm div.block {pa
+000003b0: 6464 696e 673a 2030 7078 3b20 6261 636b  dding: 0px; back
+000003c0: 6772 6f75 6e64 3a20 2366 6366 6366 637d  ground: #fcfcfc}
+000003d0: 0a63 0000 0000 0000 0000 0000 0000 0000  .c..............
+000003e0: 0000 0300 0000 4000 0000 7376 0000 0065  ......@...sv...e
+000003f0: 005a 0164 005a 0255 0064 0164 0284 005a  .Z.d.Z.U.d.d...Z
+00000400: 0365 0467 0065 056a 0666 0219 0065 0764  .e.g.e.j.f...e.d
+00000410: 033c 0064 0464 0284 005a 0865 0467 0065  .<.d.d...Z.e.g.e
+00000420: 056a 0666 0219 0065 0764 053c 0064 0664  .j.f...e.d.<.d.d
+00000430: 0284 005a 0965 0465 0a67 0165 0a66 0219  ...Z.e.e.g.e.f..
+00000440: 0065 0764 073c 0064 0864 0284 005a 0b65  .e.d.<.d.d...Z.e
+00000450: 0465 0a67 0165 0a66 0219 0065 0764 093c  .e.g.e.f...e.d.<
+00000460: 0064 0a53 0029 0bda 0a47 7261 6469 6f43  .d.S.)...GradioC
+00000470: 6f6e 6663 0000 0000 0000 0000 0000 0000  onfc............
+00000480: 0000 0000 0300 0000 4300 0000 f30c 0000  ........C.......
+00000490: 0074 006a 0164 0164 028d 0153 00a9 034e  .t.j.d.d...S...N
+000004a0: 4629 01da 0a73 686f 775f 6c61 6265 6ca9  F)...show_label.
+000004b0: 02da 0267 72da 0754 6578 7462 6f78 a900  ...gr..Textbox..
+000004c0: 7217 0000 0072 1700 0000 fa54 2f68 6f6d  r....r.....T/hom
+000004d0: 652f 7372 7573 682f 5072 6f6a 6563 7473  e/srush/Projects
+000004e0: 2f4d 696e 6943 6861 696e 2f76 656e 762f  /MiniChain/venv/
+000004f0: 6c69 622f 7079 7468 6f6e 332e 3130 2f73  lib/python3.10/s
+00000500: 6974 652d 7061 636b 6167 6573 2f6d 696e  ite-packages/min
+00000510: 6963 6861 696e 2f67 7261 6469 6f2e 7079  ichain/gradio.py
+00000520: da08 3c6c 616d 6264 613e 1c00 0000 f302  ..<lambda>......
+00000530: 0000 000c 007a 1347 7261 6469 6f43 6f6e  .....z.GradioCon
+00000540: 662e 3c6c 616d 6264 613e da0b 626c 6f63  f.<lambda>..bloc
+00000550: 6b5f 696e 7075 7463 0000 0000 0000 0000  k_inputc........
+00000560: 0000 0000 0000 0000 0300 0000 4300 0000  ............C...
+00000570: 7211 0000 0072 1200 0000 7214 0000 0072  r....r....r....r
+00000580: 1700 0000 7217 0000 0072 1700 0000 7218  ....r....r....r.
+00000590: 0000 0072 1900 0000 1d00 0000 721a 0000  ...r........r...
+000005a0: 00da 0c62 6c6f 636b 5f6f 7574 7075 7463  ...block_outputc
+000005b0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+000005c0: 0100 0000 4300 0000 f304 0000 007c 0053  ....C........|.S
+000005d0: 00a9 014e 7217 0000 00a9 01da 0178 7217  ...Nr........xr.
+000005e0: 0000 0072 1700 0000 7218 0000 0072 1900  ...r....r....r..
+000005f0: 0000 1e00 0000 f302 0000 0004 00da 1270  ...............p
+00000600: 6f73 7470 726f 6365 7373 5f6f 7574 7075  ostprocess_outpu
+00000610: 7463 0100 0000 0000 0000 0000 0000 0100  tc..............
+00000620: 0000 0100 0000 4300 0000 721d 0000 0072  ......C...r....r
+00000630: 1e00 0000 7217 0000 0072 1f00 0000 7217  ....r....r....r.
+00000640: 0000 0072 1700 0000 7218 0000 0072 1900  ...r....r....r..
+00000650: 0000 1f00 0000 7221 0000 00da 1070 7265  ......r!.....pre
+00000660: 7072 6f63 6573 735f 696e 7075 744e 290c  process_inputN).
+00000670: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+00000680: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+00000690: 6d65 5f5f 721b 0000 0072 0500 0000 7215  me__r....r....r.
+000006a0: 0000 00da 0642 6c6f 636b 73da 0f5f 5f61  .....Blocks..__a
+000006b0: 6e6e 6f74 6174 696f 6e73 5f5f 721c 0000  nnotations__r...
+000006c0: 0072 2200 0000 7204 0000 0072 2300 0000  .r"...r....r#...
+000006d0: 7217 0000 0072 1700 0000 7217 0000 0072  r....r....r....r
+000006e0: 1800 0000 7210 0000 001a 0000 0073 0a00  ....r........s..
+000006f0: 0000 0a00 1a02 1a01 1a01 1e01 7210 0000  ............r...
+00000700: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00000710: 0000 0300 0000 4000 0000 7324 0000 0065  ......@...s$...e
+00000720: 005a 0164 005a 0255 0065 0365 0464 013c  .Z.d.Z.U.e.e.d.<
+00000730: 0064 0265 0366 0264 0364 0484 045a 0564  .d.e.f.d.d...Z.d
+00000740: 0553 0029 06da 0448 544d 4cda 0468 746d  .S.)...HTML..htm
+00000750: 6cda 0672 6574 7572 6e63 0100 0000 0000  l..returnc......
+00000760: 0000 0000 0000 0100 0000 0100 0000 4300  ..............C.
+00000770: 0000 7306 0000 007c 006a 0053 0072 1e00  ..s....|.j.S.r..
+00000780: 0000 2901 722a 0000 0029 01da 0473 656c  ..).r*...)...sel
+00000790: 6672 1700 0000 7217 0000 0072 1800 0000  fr....r....r....
+000007a0: da0b 5f72 6570 725f 6874 6d6c 5f26 0000  .._repr_html_&..
+000007b0: 0073 0200 0000 0601 7a10 4854 4d4c 2e5f  .s......z.HTML._
+000007c0: 7265 7072 5f68 746d 6c5f 4e29 0672 2400  repr_html_N).r$.
+000007d0: 0000 7225 0000 0072 2600 0000 da03 7374  ..r%...r&.....st
+000007e0: 7272 2800 0000 722d 0000 0072 1700 0000  rr(...r-...r....
+000007f0: 7217 0000 0072 1700 0000 7218 0000 0072  r....r....r....r
+00000800: 2900 0000 2200 0000 7306 0000 000a 0008  )..."...s.......
+00000810: 0212 0272 2900 0000 6300 0000 0000 0000  ...r)...c.......
+00000820: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
+00000830: 0073 1a00 0000 6500 5a01 6400 5a02 5500  .s....e.Z.d.Z.U.
+00000840: 6401 5a03 6504 6505 6402 3c00 6403 5300  d.Z.e.e.d.<.d.S.
+00000850: 2904 da0e 4469 7370 6c61 794f 7074 696f  )...DisplayOptio
+00000860: 6e73 54da 086d 6172 6b64 6f77 6e4e 2906  nsT..markdownN).
+00000870: 7224 0000 0072 2500 0000 7226 0000 0072  r$...r%...r&...r
+00000880: 3000 0000 da04 626f 6f6c 7228 0000 0072  0.....boolr(...r
+00000890: 1700 0000 7217 0000 0072 1700 0000 7218  ....r....r....r.
+000008a0: 0000 0072 2f00 0000 2a00 0000 7304 0000  ...r/...*...s...
+000008b0: 000a 0010 0272 2f00 0000 6300 0000 0000  .....r/...c.....
+000008c0: 0000 0000 0000 0000 0000 0006 0000 0040  ...............@
+000008d0: 0000 0073 ac00 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
+000008e0: 5500 6503 6504 6401 8d01 5a05 6506 6507  U.e.e.d...Z.e.e.
+000008f0: 6508 6509 650a 6602 1900 6701 6508 6509  e.e.e.f...g.e.e.
+00000900: 650a 6602 1900 6602 1900 1900 650b 6402  e.f...f.....e.d.
+00000910: 3c00 6503 650c 6401 8d01 5a0d 650e 6509  <.e.e.d...Z.e.e.
+00000920: 1900 650b 6403 3c00 6503 650c 6401 8d01  ..e.d.<.e.e.d...
+00000930: 5a0f 650e 6509 1900 650b 6404 3c00 640f  Z.e.e...e.d.<.d.
+00000940: 6407 6408 8404 5a10 6403 6506 6509 1900  d.d...Z.d.e.e...
+00000950: 6406 6400 6604 6409 640a 8404 5a11 640b  d.d.f.d.d...Z.d.
+00000960: 6508 6509 650a 6602 1900 6406 6508 6509  e.e.e.f...d.e.e.
+00000970: 650a 6602 1900 6604 640c 640d 8404 5a12  e.f...f.d.d...Z.
+00000980: 640e 5300 2910 da0b 436f 6e73 7472 7563  d.S.)...Construc
+00000990: 746f 7229 01da 0f64 6566 6175 6c74 5f66  tor)...default_f
+000009a0: 6163 746f 7279 da03 666e 73da 0669 6e70  actory..fns..inp
+000009b0: 7574 73da 076f 7574 7075 7473 da05 6f74  uts..outputs..ot
+000009c0: 6865 7272 2b00 0000 6302 0000 0000 0000  herr+...c.......
+000009d0: 0000 0000 0002 0000 0005 0000 0043 0000  .............C..
+000009e0: 0073 2400 0000 7400 7c00 6a01 7c01 6a01  .s$...t.|.j.|.j.
+000009f0: 1700 7c00 6a02 7c01 6a02 4200 7c00 6a03  ..|.j.|.j.B.|.j.
+00000a00: 7c01 6a03 4200 8303 5300 721e 0000 0029  |.j.B...S.r....)
+00000a10: 0472 3200 0000 7234 0000 0072 3500 0000  .r2...r4...r5...
+00000a20: 7236 0000 0029 0272 2c00 0000 7237 0000  r6...).r,...r7..
+00000a30: 0072 1700 0000 7217 0000 0072 1800 0000  .r....r....r....
+00000a40: da05 6d65 7267 653b 0000 0073 0a00 0000  ..merge;...s....
+00000a50: 0201 0a01 0a01 0a01 04fd 7a11 436f 6e73  ..........z.Cons
+00000a60: 7472 7563 746f 722e 6d65 7267 6563 0200  tructor.mergec..
+00000a70: 0000 0000 0000 0000 0000 0200 0000 0500  ................
+00000a80: 0000 4300 0000 731a 0000 0074 007c 006a  ..C...s....t.|.j
+00000a90: 017c 006a 0274 037c 0183 0142 007c 006a  .|.j.t.|...B.|.j
+00000aa0: 0483 0353 0072 1e00 0000 2905 7232 0000  ...S.r....).r2..
+00000ab0: 0072 3400 0000 7235 0000 00da 0373 6574  .r4...r5.....set
+00000ac0: 7236 0000 0029 0272 2c00 0000 7235 0000  r6...).r,...r5..
+00000ad0: 0072 1700 0000 7217 0000 0072 1800 0000  .r....r....r....
+00000ae0: da0a 6164 645f 696e 7075 7473 4200 0000  ..add_inputsB...
+00000af0: 7302 0000 001a 017a 1643 6f6e 7374 7275  s......z.Constru
+00000b00: 6374 6f72 2e61 6464 5f69 6e70 7574 73da  ctor.add_inputs.
+00000b10: 0464 6174 6163 0200 0000 0000 0000 0000  .datac..........
+00000b20: 0000 0400 0000 0400 0000 4300 0000 7324  ..........C...s$
+00000b30: 0000 0069 007d 027c 006a 0044 005d 0a7d  ...i.}.|.j.D.].}
+00000b40: 0369 007c 02a5 017c 037c 0183 01a5 017d  .i.|...|.|.....}
+00000b50: 0271 057c 0253 0072 1e00 0000 2901 7234  .q.|.S.r....).r4
+00000b60: 0000 0029 0472 2c00 0000 723b 0000 00da  ...).r,...r;....
+00000b70: 036f 7574 da02 666e 7217 0000 0072 1700  .out..fnr....r..
+00000b80: 0000 7218 0000 0072 3d00 0000 4500 0000  ..r....r=...E...
+00000b90: 7308 0000 0004 010a 0112 0104 017a 0e43  s............z.C
+00000ba0: 6f6e 7374 7275 6374 6f72 2e66 6e4e 2904  onstructor.fnN).
+00000bb0: 7237 0000 0072 3200 0000 722b 0000 0072  r7...r2...r+...r
+00000bc0: 3200 0000 2913 7224 0000 0072 2500 0000  2...).r$...r%...
+00000bd0: 7226 0000 0072 0300 0000 da04 6c69 7374  r&...r......list
+00000be0: 7234 0000 0072 0700 0000 7205 0000 0072  r4...r....r....r
+00000bf0: 0600 0000 720b 0000 0072 0400 0000 7228  ....r....r....r(
+00000c00: 0000 0072 3900 0000 7235 0000 0072 0800  ...r9...r5...r..
+00000c10: 0000 7236 0000 0072 3800 0000 723a 0000  ..r6...r8...r:..
+00000c20: 0072 3d00 0000 7217 0000 0072 1700 0000  .r=...r....r....
+00000c30: 7217 0000 0072 1800 0000 7232 0000 0033  r....r....r2...3
+00000c40: 0000 0073 1200 0000 0a00 0202 0201 2cff  ...s..........,.
+00000c50: 1603 1601 0a02 1607 2603 7232 0000 0054  ........&.r2...T
+00000c60: da0b 6261 7365 5f70 726f 6d70 74da 0169  ..base_prompt..i
+00000c70: da0f 6469 7370 6c61 795f 6f70 7469 6f6e  ..display_option
+00000c80: 73da 0d73 686f 775f 6164 7661 6e63 6564  s..show_advanced
+00000c90: 722b 0000 0063 0400 0000 0000 0000 0000  r+...c..........
+00000ca0: 0000 0900 0000 0900 0000 0300 0000 73f2  ..............s.
+00000cb0: 0100 0067 0089 0667 0089 0788 027d 0474  ...g...g.....}.t
+00000cc0: 006a 0164 0174 0288 026a 0383 019b 009d  .j.d.t...j......
+00000cd0: 0264 0264 0364 048d 038f 2d89 0088 026a  .d.d.d....-....j
+00000ce0: 0444 005d 217d 057c 046a 0564 0075 0172  .D.]!}.|.j.d.u.r
+00000cf0: 257c 046a 05a0 06a1 007d 066e 0f74 077c  %|.j.....}.n.t.|
+00000d00: 0564 0583 0272 2f7c 05a0 06a1 007d 066e  .d...r/|.....}.n
+00000d10: 0574 0883 00a0 06a1 007d 0688 06a0 097c  .t.......}.....|
+00000d20: 06a1 0101 0071 1857 0064 0004 0004 0083  .....q.W.d......
+00000d30: 0301 006e 0831 0073 4477 0101 0001 0001  ...n.1.sDw......
+00000d40: 0059 0001 0074 006a 0164 0664 0764 0364  .Y...t.j.d.d.d.d
+00000d50: 048d 038f 7289 0188 026a 0444 005d 217d  ....r....j.D.]!}
+00000d60: 057c 046a 0564 0075 0172 627c 046a 05a0  .|.j.d.u.rb|.j..
+00000d70: 0aa1 007d 076e 0f74 077c 0564 0883 0272  ...}.n.t.|.d...r
+00000d80: 6c7c 05a0 0aa1 007d 076e 0574 0883 00a0  l|.....}.n.t....
+00000d90: 0aa1 007d 0788 07a0 097c 07a1 0101 0071  ...}.....|.....q
+00000da0: 5574 006a 0164 0964 037c 0364 0a8d 038f  Ut.j.d.d.|.d....
+00000db0: 3501 0074 006a 0b64 0b88 026a 049b 009d  5..t.j.d...j....
+00000dc0: 0264 0c64 0d8d 0201 0074 006a 0c64 0c64  .d.d.....t.j.d.d
+00000dd0: 0e64 0f8d 0289 0474 006a 0c64 0c64 1064  .d.....t.j.d.d.d
+00000de0: 0f8d 0289 0588 026a 0d72 ad74 006a 0e64  .......j.r.t.j.d
+00000df0: 1188 026a 0d9b 009d 0274 0f88 026a 0d83  ...j.....t...j..
+00000e00: 01a0 10a1 0064 1264 138d 0301 0057 0064  .....d.d.....W.d
+00000e10: 0004 0004 0083 0301 006e 0831 0073 b777  .........n.1.s.w
+00000e20: 0101 0001 0001 0059 0001 0057 0064 0004  .......Y...W.d..
+00000e30: 0004 0083 0301 006e 0831 0073 c677 0101  .......n.1.s.w..
+00000e40: 0001 0001 0059 0001 0064 1474 1174 1274  .....Y...d.t.t.t
+00000e50: 1366 0219 0064 1574 1174 1274 1366 0219  .f...d.t.t.t.f..
+00000e60: 0066 0487 0087 0187 0287 0387 0487 0587  .f..............
+00000e70: 0687 0766 0864 1664 1784 0c7d 0874 147c  ...f.d.d...}.t.|
+00000e80: 0867 0174 1583 0088 0088 0188 0488 0568  .g.t...........h
+00000e90: 0474 1588 0683 0142 0074 1588 0783 0142  .t.....B.t.....B
+00000ea0: 0083 0353 0029 184e 750e 0000 00f0 9f91  ...S.).Nu.......
+00000eb0: a920 2050 726f 6d70 743a 20da 0670 726f  .  Prompt: ..pro
+00000ec0: 6d70 7446 2903 da05 6c61 6265 6cda 0765  mptF)...label..e
+00000ed0: 6c65 6d5f 6964 da07 7669 7369 626c 6572  lem_id..visibler
+00000ee0: 1b00 0000 7504 0000 00f0 9f92 bbda 0872  ....u..........r
+00000ef0: 6573 706f 6e73 6572 1c00 0000 7a03 2e2e  esponser....z...
+00000f00: 2e29 0372 4400 0000 da04 6f70 656e 7246  .).rD.....openrF
+00000f10: 0000 007a 0942 6163 6b65 6e64 3a20 da04  ...z.Backend: ..
+00000f20: 6a73 6f6e 2901 7245 0000 00da 0549 6e70  json).rE.....Inp
+00000f30: 7574 2902 7245 0000 0072 4400 0000 da06  ut).rE...rD.....
+00000f40: 4f75 7470 7574 7a0a 5465 6d70 6c61 7465  Outputz.Template
+00000f50: 3a20 da05 696e 6e65 7229 0372 4400 0000  : ..inner).rD...
+00000f60: da05 7661 6c75 6572 4500 0000 723b 0000  ..valuerE...r;..
+00000f70: 0072 2b00 0000 6301 0000 0000 0000 0000  .r+...c.........
+00000f80: 0000 0012 0000 000a 0000 0013 0000 0073  ...............s
+00000f90: ea01 0000 6401 7d01 8802 6a00 8803 6602  ....d.}...j...f.
+00000fa0: 7c00 7401 1900 7601 7229 6900 7d02 7402  |.t...v.r)i.}.t.
+00000fb0: 8806 8807 8302 4400 5d14 5c02 7d03 7d04  ......D.].\.}.}.
+00000fc0: 7403 6a04 6402 6403 8d01 7c02 7c03 3c00  t.j.d.d...|.|.<.
+00000fd0: 7403 6a04 6402 6403 8d01 7c02 7c04 3c00  t.j.d.d...|.|.<.
+00000fe0: 7112 7c02 5300 8802 6a00 8803 6404 1800  q.|.S...j...d...
+00000ff0: 6602 7c00 7401 1900 7600 7243 7c00 7401  f.|.t...v.rC|.t.
+00001000: 1900 8802 6a00 8803 6404 1800 6602 1900  ....j...d...f...
+00001010: 6405 1900 6a05 6a06 7d01 7c00 7401 1900  d...j.j.}.|.t...
+00001020: 8802 6a00 8803 6602 1900 6405 1900 7d05  ..j...f...d...}.
+00001030: 7c05 6a07 7c05 6a05 6a06 7c05 6a05 6a08  |.j.|.j.j.|.j.j.
+00001040: 7c05 6a09 6604 5c04 7d06 7d07 7d08 7d09  |.j.f.\.}.}.}.}.
+00001050: 6406 740a 6407 740a 6604 6408 6409 8404  d.t.d.t.f.d.d...
+00001060: 7d0a 6406 740a 6407 740a 6604 640a 640b  }.d.t.d.t.f.d.d.
+00001070: 8404 7d0b 640c 7d0c 7402 7c07 7c01 8302  ..}.d.}.t.|.|...
+00001080: 4400 5d0e 5c02 7d0d 7d0e 7c0d 7c0e 6b03  D.].\.}.}.|.|.k.
+00001090: 7281 0100 6e05 7c0c 6404 3700 7d0c 7177  r...n.|.d.7.}.qw
+000010a0: 8802 6a0b 640d 7501 7297 8802 6a0b a00c  ..j.d.u.r...j...
+000010b0: 7c07 a101 7d07 8802 6a0b a00d 7c09 a101  |...}...j...|...
+000010c0: 7d09 7c07 7d0f 8804 7c0a 7c06 8301 8805  }.|.}...|.|.....
+000010d0: 7c0a 7c08 8301 8800 7403 6a04 640e 6403  |.|.....t.j.d.d.
+000010e0: 8d01 8801 7403 6a04 740e 7c09 8301 6403  ....t.j.t.|...d.
+000010f0: 8d01 6904 7d02 740f 7402 8806 8807 8302  ..i.}.t.t.......
+00001100: 8301 4400 5d3a 5c02 7d0c 5c02 7d10 7d11  ..D.]:\.}.\.}.}.
+00001110: 7c0c 7c05 6a05 6a10 6b02 72e2 7403 6a04  |.|.j.j.k.r.t.j.
+00001120: 7c0f 640e 640f 8d02 7c02 7c10 3c00 7c09  |.d.d...|.|.<.|.
+00001130: 72d9 7403 6a04 7c09 640e 640f 8d02 7c02  r.t.j.|.d.d...|.
+00001140: 7c11 3c00 71b8 7403 6a04 640e 6403 8d01  |.<.q.t.j.d.d...
+00001150: 7c02 7c11 3c00 71b8 7403 6a04 6402 6403  |.|.<.q.t.j.d.d.
+00001160: 8d01 7c02 7c10 3c00 7403 6a04 6402 6403  ..|.|.<.t.j.d.d.
+00001170: 8d01 7c02 7c11 3c00 71b8 7c02 5300 2910  ..|.|.<.q.|.S.).
+00001180: 7a17 5570 6461 7465 2074 6865 2070 726f  z.Update the pro
+00001190: 6d70 7420 626c 6f63 6bda 0046 2901 7246  mpt block..F).rF
+000011a0: 0000 0072 0d00 0000 e9ff ffff ffda 0173  ...r...........s
+000011b0: 722b 0000 0063 0100 0000 0000 0000 0000  r+...c..........
+000011c0: 0000 0100 0000 0300 0000 5300 0000 7316  ..........S...s.
+000011d0: 0000 0074 007c 0074 0183 0272 0964 017c  ...t.|.t...r.d.|
+000011e0: 0069 0153 007c 0053 0029 024e da06 7374  .i.S.|.S.).N..st
+000011f0: 7269 6e67 2902 da0a 6973 696e 7374 616e  ring)...isinstan
+00001200: 6365 722e 0000 00a9 0172 5000 0000 7217  cer......rP...r.
+00001210: 0000 0072 1700 0000 7218 0000 00da 0666  ...r....r......f
+00001220: 6f72 6d61 7495 0000 0073 0600 0000 0a01  ormat....s......
+00001230: 0801 0401 7a2f 746f 5f67 7261 6469 6f5f  ....z/to_gradio_
+00001240: 626c 6f63 6b2e 3c6c 6f63 616c 733e 2e75  block.<locals>.u
+00001250: 7064 6174 652e 3c6c 6f63 616c 733e 2e66  pdate.<locals>.f
+00001260: 6f72 6d61 7463 0100 0000 0000 0000 0000  ormatc..........
+00001270: 0000 0100 0000 0200 0000 5300 0000 7308  ..........S...s.
+00001280: 0000 0074 007c 0083 0153 0072 1e00 0000  ...t.|...S.r....
+00001290: 2901 722e 0000 0072 5300 0000 7217 0000  ).r....rS...r...
+000012a0: 0072 1700 0000 7218 0000 00da 046d 6172  .r....r......mar
+000012b0: 6b9a 0000 0073 0200 0000 0801 7a2d 746f  k....s......z-to
+000012c0: 5f67 7261 6469 6f5f 626c 6f63 6b2e 3c6c  _gradio_block.<l
+000012d0: 6f63 616c 733e 2e75 7064 6174 652e 3c6c  ocals>.update.<l
+000012e0: 6f63 616c 733e 2e6d 6172 6b72 0100 0000  ocals>.markr....
+000012f0: 4e54 2902 724d 0000 0072 4600 0000 2911  NT).rM...rF...).
+00001300: da03 5f69 64da 0861 6c6c 5f64 6174 61da  .._id..all_data.
+00001310: 037a 6970 7215 0000 00da 0675 7064 6174  .zipr......updat
+00001320: 65da 0772 756e 5f6c 6f67 da07 7265 7175  e..run_log..requ
+00001330: 6573 74da 0669 6e70 7574 5f72 4700 0000  est..input_rG...
+00001340: da06 6f75 7470 7574 7204 0000 00da 0b67  ..outputr......g
+00001350: 7261 6469 6f5f 636f 6e66 7223 0000 0072  radio_confr#...r
+00001360: 2200 0000 7231 0000 00da 0965 6e75 6d65  "...r1.....enume
+00001370: 7261 7465 da07 6479 6e61 6d69 6329 1272  rate..dynamic).r
+00001380: 3b00 0000 da0d 7072 6576 5f72 6571 7565  ;.....prev_reque
+00001390: 7374 5fda 0372 6574 da01 70da 0172 da04  st_..ret..p..r..
+000013a0: 736e 6170 725c 0000 00da 0872 6571 7565  snapr\.....reque
+000013b0: 7374 5fda 0972 6573 706f 6e73 655f da07  st_..response_..
+000013c0: 6f75 7470 7574 5f72 5400 0000 7255 0000  output_rT...rU..
+000013d0: 00da 016a da01 61da 0162 da0a 6e65 775f  ...j..a..b..new_
+000013e0: 7072 6f6d 7074 7243 0000 00da 0672 6573  promptrC.....res
+000013f0: 756c 74a9 08da 0c61 6363 6f72 6469 6f6e  ult....accordion
+00001400: 5f69 6eda 0d61 6363 6f72 6469 6f6e 5f6f  _in..accordion_o
+00001410: 7574 723f 0000 0072 4000 0000 da05 696e  utr?...r@.....in
+00001420: 7075 7472 4900 0000 da07 7072 6f6d 7074  putrI.....prompt
+00001430: 73da 0772 6573 756c 7473 7217 0000 0072  s..resultsr....r
+00001440: 1800 0000 7259 0000 0080 0000 0073 5000  ....rY.......sP.
+00001450: 0000 0402 1201 0401 1201 1001 1201 0401  ................
+00001460: 1602 1e01 1602 0402 0601 0601 0401 0cfc  ................
+00001470: 1207 1205 0403 1201 0801 0401 0a01 0a02  ................
+00001480: 0c01 0c01 0404 0803 0801 0c01 1001 04fc  ................
+00001490: 1a06 0c01 1201 0401 1401 1202 1002 1201  ................
+000014a0: 0402 7a1f 746f 5f67 7261 6469 6f5f 626c  ..z.to_gradio_bl
+000014b0: 6f63 6b2e 3c6c 6f63 616c 733e 2e75 7064  ock.<locals>.upd
+000014c0: 6174 6529 1672 1500 0000 da09 4163 636f  ate).r......Acco
+000014d0: 7264 696f 6e72 2e00 0000 da03 5f66 6eda  rdionr......_fn.
+000014e0: 0762 6163 6b65 6e64 725e 0000 0072 1b00  .backendr^...r..
+000014f0: 0000 da07 6861 7361 7474 7272 1000 0000  ....hasattrr....
+00001500: da06 6170 7065 6e64 721c 0000 00da 084d  ..appendr......M
+00001510: 6172 6b64 6f77 6eda 044a 534f 4eda 0d74  arkdown..JSON..t
+00001520: 656d 706c 6174 655f 6669 6c65 da04 436f  emplate_file..Co
+00001530: 6465 7248 0000 00da 0472 6561 6472 0600  derH.....readr..
+00001540: 0000 720b 0000 0072 0400 0000 7232 0000  ..r....r....r2..
+00001550: 0072 3900 0000 2909 723f 0000 0072 4000  .r9...).r?...r@.
+00001560: 0000 7241 0000 0072 4200 0000 da02 6270  ..rA...rB.....bp
+00001570: 7276 0000 0072 4300 0000 726d 0000 0072  rv...rC...rm...r
+00001580: 5900 0000 7217 0000 0072 6e00 0000 7218  Y...r....rn...r.
+00001590: 0000 00da 0f74 6f5f 6772 6164 696f 5f62  .....to_gradio_b
+000015a0: 6c6f 636b 4c00 0000 7358 0000 0004 0604  lockL...sX......
+000015b0: 0104 0104 0112 0106 ff02 020a 010a 010c  ................
+000015c0: 010a 010a 010a 020c 0102 f91c fd12 0c0a  ................
+000015d0: 010a 010c 010a 010a 010a 020c 0112 0216  ................
+000015e0: 010e 010e 0106 0204 010a 010c 0102 0106  ................
+000015f0: fd02 801c fa02 801c f634 1f02 3e04 0104  .........4..>...
+00001600: 011a 0104 fd72 7f00 0000 7272 0000 0063  .....r....rr...c
+00001610: 0200 0000 0000 0000 0000 0000 0600 0000  ................
+00001620: 0800 0000 4300 0000 7356 0000 0074 0083  ....C...sV...t..
+00001630: 007d 0269 007d 037c 0044 005d 217d 047c  .}.i.}.|.D.]!}.|
+00001640: 03a0 017c 046a 0264 01a1 0201 007c 037c  ...|.j.d.....|.|
+00001650: 046a 0219 007d 057c 02a0 0374 047c 047c  .j...}.|...t.|.|
+00001660: 057c 0164 028d 03a1 017d 027c 037c 046a  .|.d.....}.|.|.j
+00001670: 0205 0019 0064 0337 0003 003c 0071 077c  .....d.7...<.q.|
+00001680: 0253 0029 044e 7201 0000 00a9 0172 4200  .S.).Nr......rB.
+00001690: 0000 720d 0000 0029 0572 3200 0000 da0a  ..r....).r2.....
+000016a0: 7365 7464 6566 6175 6c74 7256 0000 0072  setdefaultrV...r
+000016b0: 3800 0000 727f 0000 0029 0672 7200 0000  8...r....).rr...
+000016c0: 7242 0000 00da 0463 6f6e 73da 0563 6f75  rB.....cons..cou
+000016d0: 6e74 7263 0000 0072 4000 0000 7217 0000  ntrc...r@...r...
+000016e0: 0072 1700 0000 7218 0000 00da 0c63 6861  .r....r......cha
+000016f0: 696e 5f62 6c6f 636b 73c5 0000 0073 1000  in_blocks....s..
+00001700: 0000 0603 0401 0801 0e01 0a01 1401 1401  ................
+00001710: 0401 7284 0000 00da 0e4f 5045 4e41 495f  ..r......OPENAI_
+00001720: 4150 495f 4b45 59da 046b 6579 7363 0100  API_KEY..keysc..
+00001730: 0000 0000 0000 0000 0000 0300 0000 0800  ................
+00001740: 0000 0300 0000 7314 0100 0074 0064 0164  ......s....t.d.d
+00001750: 0284 007c 0044 0083 0183 0172 0b64 0053  ...|.D.....r.d.S
+00001760: 0069 0089 0074 016a 0264 0364 0464 0564  .i...t.j.d.d.d.d
+00001770: 068d 038f 5a01 0064 077c 0076 0072 3364  ....Z..d.|.v.r3d
+00001780: 0774 036a 0476 0172 3374 016a 0574 036a  .t.j.v.r3t.j.t.j
+00001790: 04a0 0664 07a1 0164 0864 0464 0964 0a8d  ...d...d.d.d.d..
+000017a0: 0488 0064 073c 0074 01a0 0764 0ba1 0101  ...d.<.t...d....
+000017b0: 0064 0c7c 0076 0072 4b74 01a0 0764 0da1  .d.|.v.rKt...d..
+000017c0: 0101 0074 016a 0574 036a 04a0 0664 0ca1  ...t.j.t.j...d..
+000017d0: 0164 0e64 0f64 0964 0a8d 0488 0064 0c3c  .d.d.d.d.....d.<
+000017e0: 0064 107c 0076 0072 6374 01a0 0764 11a1  .d.|.v.rct...d..
+000017f0: 0101 0074 016a 0574 036a 04a0 0664 10a1  ...t.j.t.j...d..
+00001800: 0164 1264 0f64 0964 0a8d 0488 0064 103c  .d.d.d.d.....d.<
+00001810: 0074 01a0 0864 13a1 017d 0157 0064 0004  .t...d...}.W.d..
+00001820: 0004 0083 0301 006e 0831 0073 7277 0101  .......n.1.srw..
+00001830: 0001 0001 0059 0001 0087 0066 0164 1464  .....Y.....f.d.d
+00001840: 1584 087d 027c 016a 097c 0274 0a88 00a0  ...}.|.j.|.t....
+00001850: 0ba1 0083 0164 168d 0201 0064 0053 0029  .....d.....d.S.)
+00001860: 174e 6301 0000 0000 0000 0000 0000 0002  .Nc.............
+00001870: 0000 0004 0000 0053 0000 0073 1600 0000  .......S...s....
+00001880: 6700 7c00 5d07 7d01 7c01 7400 6a01 7600  g.|.].}.|.t.j.v.
+00001890: 9102 7102 5300 7217 0000 0029 02da 026f  ..q.S.r....)...o
+000018a0: 73da 0765 6e76 6972 6f6e 2902 da02 2e30  s..environ)....0
+000018b0: da01 6b72 1700 0000 7217 0000 0072 1800  ..kr....r....r..
+000018c0: 0000 da0a 3c6c 6973 7463 6f6d 703e d300  ....<listcomp>..
+000018d0: 0000 7302 0000 0016 007a 1c61 7069 5f6b  ..s......z.api_k
+000018e0: 6579 732e 3c6c 6f63 616c 733e 2e3c 6c69  eys.<locals>.<li
+000018f0: 7374 636f 6d70 3e7a 0841 5049 204b 6579  stcomp>z.API Key
+00001900: 7372 4900 0000 4629 0372 4400 0000 7245  srI...F).rD...rE
+00001910: 0000 0072 4800 0000 7285 0000 007a 0a4f  ...rH...r....z.O
+00001920: 7065 6e41 4920 4b65 79da 0870 6173 7377  penAI Key..passw
+00001930: 6f72 6429 0372 4400 0000 7245 0000 00da  ord).rD...rE....
+00001940: 0474 7970 657a 560a 2020 2020 2020 2020  .typezV.        
+00001950: 2020 2020 2a20 5b4f 7065 6e41 4920 4b65      * [OpenAI Ke
+00001960: 795d 2868 7474 7073 3a2f 2f70 6c61 7466  y](https://platf
+00001970: 6f72 6d2e 6f70 656e 6169 2e63 6f6d 2f61  orm.openai.com/a
+00001980: 6363 6f75 6e74 2f61 7069 2d6b 6579 7329  ccount/api-keys)
+00001990: 0a20 2020 2020 2020 2020 2020 20da 0648  .            ..H
+000019a0: 465f 4b45 597a 560a 2020 2020 2020 2020  F_KEYzV.        
+000019b0: 2020 2020 2a20 5b48 7567 6769 6e67 2046      * [Hugging F
+000019c0: 6163 6520 4b65 795d 2868 7474 7073 3a2f  ace Key](https:/
+000019d0: 2f68 7567 6769 6e67 6661 6365 2e63 6f2f  /huggingface.co/
+000019e0: 7365 7474 696e 6773 2f74 6f6b 656e 7329  settings/tokens)
+000019f0: 0a20 2020 2020 2020 2020 2020 207a 1048  .            z.H
+00001a00: 7567 6769 6e67 2046 6163 6520 4b65 7972  ugging Face Keyr
+00001a10: 4c00 0000 da08 5345 5250 5f4b 4559 7a4b  L.....SERP_KEYzK
+00001a20: 0a20 2020 2020 2020 2020 2020 202a 205b  .            * [
+00001a30: 5365 6172 6368 204b 6579 5d28 6874 7470  Search Key](http
+00001a40: 733a 2f2f 7365 7270 6170 692e 636f 6d2f  s://serpapi.com/
+00001a50: 7573 6572 732f 7369 676e 5f69 6e29 0a20  users/sign_in). 
+00001a60: 2020 2020 2020 2020 2020 207a 0a53 6561             z.Sea
+00001a70: 7263 6820 4b65 79da 0453 6176 6563 0100  rch Key..Savec..
+00001a80: 0000 0000 0000 0000 0000 0300 0000 0400  ................
+00001a90: 0000 1300 0000 733c 0000 0088 00a0 00a1  ......s<........
+00001aa0: 0044 005d 175c 027d 017d 027c 007c 0219  .D.].\.}.}.|.|..
+00001ab0: 0064 0075 0172 1b7c 007c 0219 0064 016b  .d.u.r.|.|...d.k
+00001ac0: 0372 1b7c 007c 0219 0074 016a 027c 013c  .r.|.|...t.j.|.<
+00001ad0: 0071 0469 0053 0029 024e 724e 0000 0029  .q.i.S.).NrN...)
+00001ae0: 03da 0569 7465 6d73 7287 0000 0072 8800  ...itemsr....r..
+00001af0: 0000 2903 723b 0000 0072 8a00 0000 da01  ..).r;...r......
+00001b00: 76a9 01da 096b 6579 5f6e 616d 6573 7217  v....key_namesr.
+00001b10: 0000 0072 1800 0000 da07 6170 695f 7275  ...r......api_ru
+00001b20: 6e02 0100 0073 0a00 0000 1001 1801 0e01  n....s..........
+00001b30: 0280 0401 7a19 6170 695f 6b65 7973 2e3c  ....z.api_keys.<
+00001b40: 6c6f 6361 6c73 3e2e 6170 695f 7275 6e29  locals>.api_run)
+00001b50: 0172 3500 0000 290c da03 616c 6c72 1500  .r5...)...allr..
+00001b60: 0000 7274 0000 0072 8700 0000 7288 0000  ..rt...r....r...
+00001b70: 0072 1600 0000 da03 6765 7472 7900 0000  .r......getry...
+00001b80: da06 4275 7474 6f6e da05 636c 6963 6b72  ..Button..clickr
+00001b90: 3900 0000 da06 7661 6c75 6573 2903 7286  9.....values).r.
+00001ba0: 0000 00da 0761 7069 5f62 746e 7295 0000  .....api_btnr...
+00001bb0: 0072 1700 0000 7293 0000 0072 1800 0000  .r....r....r....
+00001bc0: da08 6170 695f 6b65 7973 d200 0000 734c  ..api_keys....sL
+00001bd0: 0000 0012 0104 0104 0112 0212 0104 010a  ................
+00001be0: 0102 0102 0102 010a fc04 0602 0104 ff08  ................
+00001bf0: 0604 0102 0104 ff04 060a 0102 0102 0102  ................
+00001c00: 010a fc08 0704 0102 0104 ff04 050a 0102  ................
+00001c10: 0102 0102 010a fc0c 071c d70c 2b1a 0672  ............+..r
+00001c20: 9c00 0000 724e 0000 0072 3000 0000 7243  ....rN...r0...rC
+00001c30: 0000 00da 0865 7861 6d70 6c65 73da 0a73  .....examples..s
+00001c40: 7562 7072 6f6d 7074 73da 0666 6965 6c64  ubprompts..field
+00001c50: 73da 0d69 6e69 7469 616c 5f73 7461 7465  s..initial_state
+00001c60: da08 6f75 745f 7479 7065 da0b 6465 7363  ..out_type..desc
+00001c70: 7269 7074 696f 6eda 0463 6f64 65da 0363  ription..code..c
+00001c80: 7373 630b 0000 0000 0000 0000 0000 000f  ssc.............
+00001c90: 0000 0009 0000 0003 0000 0073 8a01 0000  ...........s....
+00001ca0: 6401 6402 8400 7400 a001 8804 a101 6a02  d.d...t.......j.
+00001cb0: 4400 8301 8901 7403 6a04 7405 6403 1700  D.....t.j.t.d...
+00001cc0: 7c09 1700 7403 6a06 a007 a100 6404 8d02  |...t.j.....d...
+00001cd0: 8fa2 7d0b 7408 8300 0100 7409 8300 8900  ..}.t.....t.....
+00001ce0: 7403 a00a 8802 a101 8905 8800 a00b 7409  t.............t.
+00001cf0: 8805 6801 8805 6801 6405 8d02 a101 8900  ..h...h.d.......
+00001d00: 7403 a00c 7c07 a101 0100 740d 6406 6402  t...|.....t.d.d.
+00001d10: 8400 8801 4400 8301 8301 8903 7403 6a0e  ....D.......t.j.
+00001d20: 7c01 8803 6407 8d02 7d01 7403 6a0f 6408  |...d...}.t.j.d.
+00001d30: 6409 8d01 7d0c 8800 a010 8803 a101 8900  d...}...........
+00001d40: 7403 a011 a100 8f11 0100 8800 a00b 7412  t.............t.
+00001d50: 7c02 7c0a 640a 8d02 a101 8900 5700 640b  |.|.d.......W.d.
+00001d60: 0400 0400 8303 0100 6e08 3100 7368 7701  ........n.1.shw.
+00001d70: 0100 0100 0100 5900 0100 640c 7413 7414  ......Y...d.t.t.
+00001d80: 7415 6602 1900 640d 7413 7414 7415 6602  t.f...d.t.t.t.f.
+00001d90: 1900 6604 8705 6601 640e 640f 840c 7d0d  ..f...f.d.d...}.
+00001da0: 8800 a00b 7409 7c0d 6701 7416 8300 7416  ....t.|.g.t...t.
+00001db0: 8300 8303 a101 8900 8700 8701 8702 8703  ................
+00001dc0: 8704 8705 6606 6410 6411 8408 7d0e 7c0c  ....f.d.d...}.|.
+00001dd0: 6a17 7c0e 8800 6a18 8800 6a19 6405 8d03  j.|...j...j.d...
+00001de0: 0100 7c08 72b3 7403 6a1a 7c08 6412 6413  ..|.r.t.j.|.d.d.
+00001df0: 6414 8d03 0100 5700 640b 0400 0400 8303  d.....W.d.......
+00001e00: 0100 7c0b 5300 5700 640b 0400 0400 8303  ..|.S.W.d.......
+00001e10: 0100 7c0b 5300 3100 73be 7701 0100 0100  ..|.S.1.s.w.....
+00001e20: 0100 5900 0100 7c0b 5300 2915 618b 0200  ..Y...|.S.).a...
+00001e30: 000a 2020 2020 436f 6e73 7472 7563 7473  ..    Constructs
+00001e40: 2061 2067 7261 6469 6f20 636f 6d70 6f6e   a gradio compon
+00001e50: 656e 7420 746f 2073 686f 7720 6120 7072  ent to show a pr
+00001e60: 6f6d 7074 2063 6861 696e 2e0a 0a20 2020  ompt chain...   
+00001e70: 2041 7267 733a 0a20 2020 2020 2020 2070   Args:.        p
+00001e80: 726f 6d70 743a 2041 2070 726f 6d70 7420  rompt: A prompt 
+00001e90: 6f72 2070 726f 6d70 7420 6368 6169 6e20  or prompt chain 
+00001ea0: 746f 2064 6973 706c 6179 2e0a 2020 2020  to display..    
+00001eb0: 2020 2020 6578 616d 706c 6573 3a20 4120      examples: A 
+00001ec0: 6c69 7374 206f 6620 6578 616d 706c 6520  list of example 
+00001ed0: 696e 7075 7473 2c20 6569 7468 6572 2073  inputs, either s
+00001ee0: 7472 696e 6720 6f72 2074 7570 6c65 7320  tring or tuples 
+00001ef0: 6f66 2066 6965 6c64 730a 2020 2020 2020  of fields.      
+00001f00: 2020 7375 6270 726f 6d70 7473 3a20 5468    subprompts: Th
+00001f10: 6520 6050 726f 6d70 7460 206f 626a 6563  e `Prompt` objec
+00001f20: 7473 2074 6f20 6469 7370 6c61 792e 0a20  ts to display.. 
+00001f30: 2020 2020 2020 2066 6965 6c64 733a 2054         fields: T
+00001f40: 6865 206e 616d 6573 206f 6620 7468 6520  he names of the 
+00001f50: 6669 656c 6420 696e 7075 7420 746f 2074  field input to t
+00001f60: 6865 2070 726f 6d70 742e 0a20 2020 2020  he prompt..     
+00001f70: 2020 2069 6e69 7469 616c 5f73 7461 7465     initial_state
+00001f80: 3a20 466f 7220 7374 6174 6566 756c 2070  : For stateful p
+00001f90: 726f 6d70 7473 2c20 7468 6520 696e 6974  rompts, the init
+00001fa0: 6961 6c20 7661 6c75 652e 0a20 2020 2020  ial value..     
+00001fb0: 2020 206f 7574 5f74 7970 653a 2074 7970     out_type: typ
+00001fc0: 6520 6f66 2066 696e 616c 206f 7574 7075  e of final outpu
+00001fd0: 740a 2020 2020 2020 2020 6b65 7973 3a20  t.        keys: 
+00001fe0: 7573 6572 206b 6579 7320 7265 7175 6972  user keys requir
+00001ff0: 6564 0a20 2020 2020 2020 2064 6573 6372  ed.        descr
+00002000: 6970 7469 6f6e 3a20 6465 7363 7269 7074  iption: descript
+00002010: 696f 6e20 6f66 2074 6865 206d 6f64 656c  ion of the model
+00002020: 0a20 2020 2020 2020 2063 6f64 653a 2063  .        code: c
+00002030: 6f64 6520 746f 2064 6973 706c 6179 0a20  ode to display. 
+00002040: 2020 2020 2020 2063 7373 203a 2061 6464         css : add
+00002050: 6974 696f 6e61 6c20 6373 730a 2020 2020  itional css.    
+00002060: 2020 2020 7368 6f77 5f61 6476 616e 6365      show_advance
+00002070: 6420 3a20 7368 6f77 2074 6865 2022 2e2e  d : show the "..
+00002080: 2e22 2061 6476 616e 6365 6420 656c 656d  ." advanced elem
+00002090: 656e 7473 0a0a 2020 2020 5265 7475 726e  ents..    Return
+000020a0: 733a 0a20 2020 2020 2020 2047 7261 6469  s:.        Gradi
+000020b0: 6f20 626c 6f63 6b0a 2020 2020 6301 0000  o block.    c...
+000020c0: 0000 0000 0000 0000 0002 0000 0004 0000  ................
+000020d0: 0053 0000 0073 1800 0000 6700 7c00 5d08  .S...s....g.|.].
+000020e0: 7d01 7c01 6400 6b03 7202 7c01 9102 7102  }.|.d.k.r.|...q.
+000020f0: 5300 a901 da05 7374 6174 6572 1700 0000  S.....stater....
+00002100: 2902 7289 0000 00da 0361 7267 7217 0000  ).r......argr...
+00002110: 0072 1700 0000 7218 0000 0072 8b00 0000  .r....r....r....
+00002120: 2b01 0000 f302 0000 0018 007a 1873 686f  +..........z.sho
+00002130: 772e 3c6c 6f63 616c 733e 2e3c 6c69 7374  w.<locals>.<list
+00002140: 636f 6d70 3eda 010a 2902 72a4 0000 00da  comp>...).r.....
+00002150: 0574 6865 6d65 2902 7235 0000 0072 3600  .theme).r5...r6.
+00002160: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
+00002170: 0000 0005 0000 0053 0000 0073 1800 0000  .......S...s....
+00002180: 6700 7c00 5d08 7d01 7400 6a01 7c01 6400  g.|.].}.t.j.|.d.
+00002190: 8d01 9102 7102 5300 2901 a901 7244 0000  ....q.S.)...rD..
+000021a0: 0072 1400 0000 2902 7289 0000 00da 0166  .r....).r......f
+000021b0: 7217 0000 0072 1700 0000 7218 0000 0072  r....r....r....r
+000021c0: 8b00 0000 3a01 0000 72a8 0000 0029 0272  ....:...r....).r
+000021d0: 9d00 0000 7235 0000 00da 0352 756e 72ab  ....r5.....Runr.
+000021e0: 0000 0072 8000 0000 4e72 3b00 0000 722b  ...r....Nr;...r+
+000021f0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00002200: 0200 0000 0200 0000 1300 0000 7310 0000  ............s...
+00002210: 007c 0074 0019 007d 0188 007c 0169 0153  .|.t...}...|.i.S
+00002220: 0072 1e00 0000 2901 da0c 6669 6e61 6c5f  .r....)...final_
+00002230: 6f75 7470 7574 2902 723b 0000 00da 0566  output).r;.....f
+00002240: 696e 616c 72a5 0000 0072 1700 0000 7218  inalr....r....r.
+00002250: 0000 00da 096f 7574 7075 745f 666e 4a01  .....output_fnJ.
+00002260: 0000 7304 0000 0008 0108 017a 1773 686f  ..s........z.sho
+00002270: 772e 3c6c 6f63 616c 733e 2e6f 7574 7075  w.<locals>.outpu
+00002280: 745f 666e 6301 0000 0000 0000 0000 0000  t_fnc...........
+00002290: 0003 0000 0008 0000 0033 0000 0073 ac00  .........3...s..
+000022a0: 0000 8100 8700 6601 6401 6402 8408 7400  ......f.d.d...t.
+000022b0: 8802 8804 8302 4400 8301 7d01 8803 6400  ......D...}...d.
+000022c0: 7501 7217 8800 8806 1900 7c01 6403 3c00  u.r.......|.d.<.
+000022d0: 7401 6404 8301 8f2b 0100 8805 6405 6900  t.d....+....d.i.
+000022e0: 7c01 a401 8e01 a002 a100 4400 5d19 7d02  |.........D.].}.
+000022f0: 7403 7404 6a05 8301 8800 7406 3c00 7c02  t.t.j.....t.<.|.
+00002300: 8800 7407 3c00 8801 a008 8800 a101 5600  ..t.<.........V.
+00002310: 0100 7c02 6400 7501 723e 0100 6e01 7125  ..|.d.u.r>..n.q%
+00002320: 5700 6400 0400 0400 8303 0100 6e08 3100  W.d.........n.1.
+00002330: 7349 7701 0100 0100 0100 5900 0100 8801  sIw.......Y.....
+00002340: a008 8800 a101 5600 0100 6400 5300 2906  ......V...d.S.).
+00002350: 4e63 0100 0000 0000 0000 0000 0000 0300  Nc..............
+00002360: 0000 0500 0000 1300 0000 731a 0000 0069  ..........s....i
+00002370: 007c 005d 095c 027d 017d 027c 0188 007c  .|.].\.}.}.|...|
+00002380: 0219 0093 0271 0253 0072 1700 0000 7217  .....q.S.r....r.
+00002390: 0000 0029 0372 8900 0000 728a 0000 0072  ...).r....r....r
+000023a0: 9200 0000 a901 723b 0000 0072 1700 0000  ......r;...r....
+000023b0: 7218 0000 00da 0a3c 6469 6374 636f 6d70  r......<dictcomp
+000023c0: 3e51 0100 0073 0200 0000 1a00 7a25 7368  >Q...s......z%sh
+000023d0: 6f77 2e3c 6c6f 6361 6c73 3e2e 7275 6e2e  ow.<locals>.run.
+000023e0: 3c6c 6f63 616c 733e 2e3c 6469 6374 636f  <locals>.<dictco
+000023f0: 6d70 3e72 a600 0000 da04 7465 6d70 7217  mp>r......tempr.
+00002400: 0000 0029 0972 5800 0000 720c 0000 00da  ...).rX...r.....
+00002410: 0772 756e 5f67 656e da04 6469 6374 720e  .run_gen..dictr.
+00002420: 0000 00da 0c70 726f 6d70 745f 7374 6f72  .....prompt_stor
+00002430: 6572 5700 0000 72ae 0000 0072 3d00 0000  erW...r....r=...
+00002440: 2903 723b 0000 00da 0d70 726f 6d70 745f  ).r;.....prompt_
+00002450: 696e 7075 7473 725d 0000 00a9 06da 0b63  inputsr].......c
+00002460: 6f6e 7374 7275 6374 6f72 729f 0000 0072  onstructorr....r
+00002470: a000 0000 7235 0000 0072 4300 0000 72a6  ....r5...rC...r.
+00002480: 0000 0072 b100 0000 7218 0000 00da 0372  ...r....r......r
+00002490: 756e 5001 0000 731e 0000 0002 8018 0108  unP...s.........
+000024a0: 010c 010a 0216 020e 0108 010c 0108 0104  ................
+000024b0: 0102 ff02 801c fa10 087a 1173 686f 772e  .........z.show.
+000024c0: 3c6c 6f63 616c 733e 2e72 756e da06 7079  <locals>.run..py
+000024d0: 7468 6f6e 724c 0000 0029 02da 086c 616e  thonrL...)...lan
+000024e0: 6775 6167 6572 4500 0000 291b da07 696e  guagerE...)...in
+000024f0: 7370 6563 74da 0e67 6574 6675 6c6c 6172  spect..getfullar
+00002500: 6773 7065 63da 0461 7267 7372 1500 0000  gspec..argsr....
+00002510: 7227 0000 00da 0343 5353 da06 7468 656d  r'.....CSS..them
+00002520: 6573 da0a 4d6f 6e6f 6368 726f 6d65 729c  es..Monochromer.
+00002530: 0000 0072 3200 0000 da05 5374 6174 6572  ...r2.....Stater
+00002540: 3800 0000 7279 0000 0072 3e00 0000 da08  8...ry...r>.....
+00002550: 4578 616d 706c 6573 7298 0000 0072 3a00  Examplesr....r:.
+00002560: 0000 da03 426f 7872 8400 0000 7206 0000  ....Boxr....r...
+00002570: 0072 0b00 0000 7204 0000 0072 3900 0000  .r....r....r9...
+00002580: 7299 0000 0072 3500 0000 7236 0000 0072  r....r5...r6...r
+00002590: 7c00 0000 290f 7243 0000 0072 9d00 0000  |...).rC...r....
+000025a0: 729e 0000 0072 9f00 0000 72a0 0000 0072  r....r....r....r
+000025b0: a100 0000 7286 0000 0072 a200 0000 72a3  ....r....r....r.
+000025c0: 0000 0072 a400 0000 7242 0000 00da 0464  ...r....rB.....d
+000025d0: 656d 6fda 0971 7565 7279 5f62 746e 72b0  emo..query_btnr.
+000025e0: 0000 0072 ba00 0000 7217 0000 0072 b800  ...r....r....r..
+000025f0: 0000 7218 0000 00da 0473 686f 770b 0100  ..r......show...
+00002600: 0073 3a00 0000 1620 1e01 0602 0602 0a03  .s:.... ........
+00002610: 1601 0a03 1203 0e01 0c01 0a01 0a02 0402  ................
+00002620: 0a01 06ff 1cfe 260b 1804 1602 140f 0402  ......&.........
+00002630: 1201 0aca 0438 02fd 0acb 0438 10c8 0438  .....8.....8...8
+00002640: 72c8 0000 0029 0154 2927 72bd 0000 0072  r....).T)'r....r
+00002650: 8700 0000 da0b 6461 7461 636c 6173 7365  ......dataclasse
+00002660: 7372 0200 0000 7203 0000 00da 0674 7970  sr....r......typ
+00002670: 696e 6772 0400 0000 7205 0000 0072 0600  ingr....r....r..
+00002680: 0000 7207 0000 0072 0800 0000 7209 0000  ..r....r....r...
+00002690: 0072 0a00 0000 da06 6772 6164 696f 7215  .r......gradior.
+000026a0: 0000 00da 0d67 7261 6469 6f2e 626c 6f63  .....gradio.bloc
+000026b0: 6b73 720b 0000 00da 096d 696e 6963 6861  ksr......minicha
+000026c0: 696e 720c 0000 0072 7600 0000 720e 0000  inr....rv...r...
+000026d0: 00da 0462 6173 6572 0f00 0000 72c0 0000  ...baser....r...
+000026e0: 0072 1000 0000 7229 0000 0072 2f00 0000  .r....r)...r/...
+000026f0: 72c3 0000 0072 5700 0000 72ae 0000 0072  r....rW...r....r
+00002700: 3200 0000 da03 696e 7472 3100 0000 727f  2.....intr1...r.
+00002710: 0000 0072 8400 0000 722e 0000 0072 9c00  ...r....r....r..
+00002720: 0000 7227 0000 0072 c800 0000 7217 0000  ..r'...r....r...
+00002730: 0072 1700 0000 7217 0000 0072 1800 0000  .r....r....r....
+00002740: da08 3c6d 6f64 756c 653e 0100 0000 739a  ..<module>....s.
+00002750: 0000 0008 0008 0110 0124 0108 020c 010c  .........$......
+00002760: 020c 020c 0104 0202 0c10 0102 0710 0102  ................
+00002770: 0710 010a 040a 0102 0310 0104 1b02 0104  ................
+00002780: fc0c 0102 ff02 0202 fe02 0302 fd02 0402  ................
+00002790: fc02 050a fb02 7a04 ff10 0102 ff02 0102  ......z.........
+000027a0: ff02 020a fe1c 0d04 3b02 0102 0102 0102  ........;.......
+000027b0: 0104 0102 0102 0102 0102 0104 f50c 0102  ................
+000027c0: ff16 0202 fe10 0302 fd06 0402 fc02 0502  ................
+000027d0: fb02 0602 fa06 0702 f902 0802 f802 0902  ................
+000027e0: f702 0a02 f602 0b02 f504 0c0e f4         .............
```

### ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/backend.py

```diff
@@ -1,82 +1,84 @@
 import os
 import subprocess
 import time
 from dataclasses import dataclass
 from types import TracebackType
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Sequence, Tuple
+from typing import TYPE_CHECKING, Any, Dict, Iterator, List, Optional, Tuple
 
+import gradio as gr
 from eliot import start_action, to_file
 
 if TYPE_CHECKING:
     import manifest
 
 
-@dataclass
-class Request:
-    prompt: str
-    stop: Optional[Sequence[str]] = None
-
-
 class Backend:
-    needs_request = True
-
     @property
-    def description(self):
+    def description(self) -> str:
         return ""
 
-    def run(self, request: Request) -> str:
+    def run(self, request: str) -> str:
         raise NotImplementedError
 
-    async def arun(self, request: Request) -> str:
+    def run_stream(self, request: str) -> Iterator[str]:
+        raise NotImplementedError
+
+    async def arun(self, request: str) -> str:
         return self.run(request)
 
+    def block_input(self) -> gr.Blocks:
+        return gr.Textbox(show_label=False)
+
+    def block_output(self) -> gr.Blocks:
+        return gr.Textbox(show_label=False)
+
 
 class Id(Backend):
-    def run(self, request: Request) -> str:
-        return request.prompt
+    def run(self, request: str) -> str:
+        return request
 
 
 class Mock(Backend):
     def __init__(self, answers: List[str] = []):
         self.i = -1
         self.answers = answers
 
-    def run(self, request: Request) -> str:
+    def run(self, request: str) -> str:
         self.i += 1
         return self.answers[self.i % len(self.answers)]
 
-    def run_stream(self, request: Request) -> str:
+    def run_stream(self, request: str) -> Iterator[str]:
         self.i += 1
         result = self.answers[self.i % len(self.answers)]
         for c in result:
             yield c
-            time.sleep(10)
+            time.sleep(0.1)
 
     def __repr__(self) -> str:
         return f"Mocked Backend {self.answers}"
 
 
 class Google(Backend):
     def __init__(self) -> None:
         pass
 
-    def run(self, request: Request) -> str:
+    def run(self, request: str) -> str:
         from serpapi import GoogleSearch
 
         serpapi_key = os.environ.get("SERP_KEY")
         assert (
             serpapi_key
         ), "Need a SERP_KEY. Get one here https://serpapi.com/users/welcome"
         self.serpapi_key = serpapi_key
 
         params = {
             "api_key": self.serpapi_key,
             "engine": "google",
-            "q": request.prompt,
+            "q": request,
             "google_domain": "google.com",
             "gl": "us",
             "hl": "en",
         }
 
         search = GoogleSearch(params)
         res = search.get_dict()
@@ -99,20 +101,26 @@
     def __repr__(self) -> str:
         return "Google Search Backend"
 
 
 class Python(Backend):
     """Executes Python commands and returns the output."""
 
-    def run(self, request: Request) -> str:
+    def block_input(self) -> gr.Blocks:
+        return gr.Code()
+
+    def block_output(self) -> gr.Blocks:
+        return gr.Code()
+
+    def run(self, request: str) -> str:
         """Run commands and return final output."""
         from contextlib import redirect_stdout
         from io import StringIO
 
-        p = request.prompt.strip()
+        p = request.strip()
         if p.startswith("```"):
             p = "\n".join(p.strip().split("\n")[1:-1])
 
         f = StringIO()
         with redirect_stdout(f):
             exec(p)
         s = f.getvalue()
@@ -121,24 +129,30 @@
     def __repr__(self) -> str:
         return "Python-Backend"
 
 
 class Bash(Backend):
     """Executes bash commands and returns the output."""
 
+    def block_input(self) -> gr.Blocks:
+        return gr.Code()
+
+    def block_output(self) -> gr.Blocks:
+        return gr.Code()
+
     def __init__(self, strip_newlines: bool = False, return_err_output: bool = False):
         """Initialize with stripping newlines."""
         self.strip_newlines = strip_newlines
         self.return_err_output = return_err_output
 
-    def run(self, request: Request) -> str:
+    def run(self, request: str) -> str:
         """Run commands and return final output."""
         try:
             output = subprocess.run(
-                request.prompt,
+                request,
                 shell=True,
                 check=True,
                 stdout=subprocess.PIPE,
                 stderr=subprocess.STDOUT,
             ).stdout.decode()
         except subprocess.CalledProcessError as error:
             if self.return_err_output:
@@ -151,167 +165,162 @@
     def __repr__(self) -> str:
         return "Bash-Backend"
 
 
 class OpenAIBase(Backend):
     def __init__(
         self,
-        model: str = "text-davinci-003",
+        model: str = "gpt-3.5-turbo",
         max_tokens: int = 256,
         temperature: float = 0.0,
+        stop: Optional[List[str]] = None,
     ) -> None:
         self.model = model
+        self.stop = stop
         self.options = dict(
             model=model,
             max_tokens=max_tokens,
             temperature=temperature,
         )
 
     def __repr__(self) -> str:
         return f"OpenAI Backend {self.options}"
 
 
-class OpenAIStream:
-    def __init__(self, answers: List[str] = []):
-        pass
+class OpenAI(OpenAIBase):
+    def run(self, request: str) -> str:
+        import manifest
 
-    def run_stream(self, prompt):
+        chat = {"gpt-4", "gpt-3.5-turbo"}
+        manifest = manifest.Manifest(
+            client_name="openaichat" if self.model in chat else "openai",
+            max_tokens=self.options["max_tokens"],
+            cache_name="sqlite",
+            cache_connection=f"{MinichainContext.name}",
+        )
+
+        ans = manifest.run(
+            request,
+            stop_sequences=self.stop,
+        )
+        return str(ans)
+
+    def run_stream(self, prompt: str) -> Iterator[str]:
         import openai
 
         self.api_key = os.environ.get("OPENAI_API_KEY")
         assert (
             self.api_key
         ), "Need an OPENAI_API_KEY. Get one here https://openai.com/api/"
         openai.api_key = self.api_key
 
         for chunk in openai.ChatCompletion.create(
-            model="gpt-4",
+            model=self.model,
             messages=[{"role": "user", "content": prompt}],
             stream=True,
+            stop=self.stop,
         ):
             content = chunk["choices"][0].get("delta", {}).get("content")
             if content is not None:
                 yield content
 
-    def __repr__(self) -> str:
-        return "OpenAI Stream Backend"
-
-
-class OpenAI(OpenAIBase):
-    def run(self, request: Request) -> str:
-        import manifest
-
-        manifest = manifest.Manifest(
-            client_name="openai",
-            max_tokens=self.options["max_tokens"],
-            cache_name="sqlite",
-            cache_connection=f"{MinichainContext.name}",
-        )
-
-        ans = manifest.run(
-            # openai.Completion.create(
-            # **self.options,
-            # kstop=request.stop,
-            # prompt=
-            request.prompt,
-            stop_sequences=request.stop,
-        )
-        return str(ans)
-
-    async def arun(self, request: Request) -> str:
-        import async_openai
-
-        self.api_key = os.environ.get("OPENAI_API_KEY")
-        async_openai.OpenAI.configure(
-            api_key=self.api_key,
-            debug_enabled=False,
-        )
-        ans = await async_openai.OpenAI.Completions.async_create(
-            **self.options,
-            stop=request.stop,
-            prompt=request.prompt,
-        )
-        return str(ans.choices[0].text)
-
 
 class OpenAIEmbed(OpenAIBase):
+    def block_output(self) -> gr.Blocks:
+        return gr.Textbox(label="Embedding")
+
     def __init__(self, model: str = "text-embedding-ada-002", **kwargs: Any) -> None:
         super().__init__(model, **kwargs)
 
-    def run(self, request: Request) -> str:
+    def run(self, request: str) -> str:
         import openai
 
         self.api_key = os.environ.get("OPENAI_API_KEY")
         assert (
             self.api_key
         ), "Need an OPENAI_API_KEY. Get one here https://openai.com/api/"
         openai.api_key = self.api_key
 
         ans = openai.Embedding.create(
             engine=self.model,
-            input=request.prompt,
+            input=request,
         )
         return ans["data"][0]["embedding"]  # type: ignore
 
 
 class HuggingFaceBase(Backend):
     def __init__(self, model: str = "gpt2") -> None:
         self.model = model
 
 
 class HuggingFace(HuggingFaceBase):
-    def run(self, request: Request) -> str:
+    def run(self, request: str) -> str:
 
         from huggingface_hub.inference_api import InferenceApi
 
         self.api_key = os.environ.get("HF_KEY")
         assert self.api_key, "Need an HF_KEY. Get one here https://huggingface.co/"
 
         self.client = InferenceApi(
             token=self.api_key, repo_id=self.model, task="text-generation"
         )
-        response = self.client(inputs=request.prompt)
+        response = self.client(inputs=request)
         return response  # type: ignore
 
 
 class HuggingFaceEmbed(HuggingFaceBase):
-    def run(self, request: Request) -> str:
+    def run(self, request: str) -> str:
 
         from huggingface_hub.inference_api import InferenceApi
 
         self.api_key = os.environ.get("HF_KEY")
         assert self.api_key, "Need an HF_KEY. Get one here https://huggingface.co/"
 
         self.client = InferenceApi(
             token=self.api_key, repo_id=self.model, task="feature-extraction"
         )
-        response = self.client(inputs=request.prompt)
+        response = self.client(inputs=request)
         return response  # type: ignore
 
 
 class Manifest(Backend):
     def __init__(self, client: "manifest.Manifest") -> None:
         "Client from [Manifest-ML](https://github.com/HazyResearch/manifest)."
         self.client = client
 
-    def run(self, request: Request) -> str:
+    def run(self, request: str) -> str:
         try:
             import manifest
         except ImportError:
             raise ImportError("`pip install manifest-ml` to use the Manifest Backend.")
         assert isinstance(
             self.client, manifest.Manifest
         ), "Client must be a `manifest.Manifest` instance."
 
-        return self.client.run(request.prompt)  # type: ignore
+        return self.client.run(request)  # type: ignore
+
+
+@dataclass
+class RunLog:
+    request: str = ""
+    response: Optional[str] = ""
+    output: str = ""
+    dynamic: int = 0
+
+
+@dataclass
+class PromptSnap:
+    input_: Any = ""
+    run_log: RunLog = RunLog()
+    output: Any = ""
 
 
 class MinichainContext:
     id_: int = 0
-    prompt_store: Dict[Tuple[int, int], Tuple[Any, Request, str, Any]] = {}
+    prompt_store: Dict[Tuple[int, int], List[PromptSnap]] = {}
     prompt_count: Dict[int, int] = {}
     name: str = ""
 
 
 def set_minichain_log(name: str) -> None:
     to_file(open(f"{name}.log", "w"))
```

### ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/base.py

```diff
@@ -1,309 +1,207 @@
-import json
-from dataclasses import asdict, dataclass, fields, is_dataclass
-from enum import Enum
+from dataclasses import asdict, dataclass
 from itertools import count
 from typing import (
     Any,
     Callable,
-    Dict,
     Generic,
+    Iterable,
+    Iterator,
     List,
     Optional,
-    Tuple,
-    Type,
     TypeVar,
     Union,
-    get_args,
-    get_origin,
 )
 
-from eliot import start_action
-from jinja2 import (
-    Environment,
-    FileSystemLoader,
-    PackageLoader,
-    Template,
-    select_autoescape,
-)
-
-from .backend import Backend, MinichainContext, Request
-
-env = Environment(
-    loader=PackageLoader("minichain"),
-    autoescape=select_autoescape(),
-    extensions=["jinja2_highlight.HighlightExtension"],
-)
-
-
-def _prompt(r: Union[str, Request]) -> Request:
-    if isinstance(r, str):
-        return Request(r)
-    else:
-        return r
+from jinja2 import Environment, FileSystemLoader, Template
 
+from .backend import Backend, MinichainContext, PromptSnap, RunLog
 
 Input = TypeVar("Input")
 Output = TypeVar("Output")
 FnOutput = TypeVar("FnOutput")
 
 
-def enum(x: Type[Enum]) -> Dict[str, int]:
-    d = {e.name: e.value for e in x}
-    return d
-
-
-def walk(x: Any) -> Any:
-    if issubclass(x if get_origin(x) is None else get_origin(x), List):
-        return {"_t_": "list", "t": walk(get_args(x)[0])}
-    if issubclass(x, Enum):
-        return enum(x)
-
-    if is_dataclass(x):
-        return {y.name: walk(y.type) for y in fields(x)}
-    return x.__name__
-
-
-def type_to_prompt(out: type) -> str:
-    tmp = env.get_template("type_prompt.pmpt.tpl")
-    d = walk(out)
-    return tmp.render({"typ": d})
-
-
-def simple(model, **kwargs):  # type: ignore
-    return model(kwargs)
-
-
 @dataclass
 class History:
-    prompt: "Prompt[Input, Output, FnOutput]"
+    expand: Callable[[List[Any]], Iterator[Any]]
     inputs: List[Any]
 
 
 @dataclass
-class Fail:
-    arg_num: int
-    data: Any
-
-    def __str__(self):
-        return "fail"
+class Break:
+    pass
 
 
 @dataclass
 class Chain:
-    # TODO: Add caching
     history: History
+    name: str
+    cache: Any = None
 
-    def run_gen(self, trial: int = 0, data: Any = None) -> Any:
+    def run_gen(self) -> Any:
+        # Lazily instantiate all the inputs
         args = []
-        count = []
-        for inp in self.history.inputs:
-            inp2 = inp
-            if isinstance(inp, Chain):
-                for inp2 in inp.run_gen():
-                    yield None
-            args.append(inp2)
-            count.append(0)
-        for out in self.history.prompt.expand(args, trial, data):
-            yield None
-        while isinstance(out, Fail):
-            count[out.arg_num] += 1
-            inp = self.history.inputs[out.arg_num]
-            assert isinstance(inp, Chain)
-            for inp2 in inp.run_gen(trial=count[out.arg_num], data=out.data):
-                yield None
-            args[out.arg_num] = inp2
-            for out in self.history.prompt.expand(args, trial, data):
-                yield None
-            yield None
+        for i, base_input in enumerate(self.history.inputs):
+            function_input = base_input
+            if isinstance(base_input, Chain):
+                if base_input.cache is not None:
+                    function_input = base_input.cache
+                    if isinstance(function_input, Break):
+                        yield Break()
+                        return
+                else:
+                    for function_input in base_input.run_gen():
+                        if isinstance(function_input, Break):
+                            base_input.cache = Break()
+                            yield Break()
+                            return
+                        yield None
+
+                    base_input.cache = function_input
+            args.append(function_input)
+        # Run the current prompt
+        for out in self.history.expand(*args):
+            if isinstance(out, Break):
+                yield Break()
+                return
 
+            yield None
         yield out
 
     def run(self) -> Any:
         for x in self.run_gen():
-            if x is not None:
-                return x
+            pass
+        return x
 
 
 class Prompt(Generic[Input, Output, FnOutput]):
     counter = count()
 
     def __init__(
         self,
-        backend: Backend,
-        parser: Union[str, Callable[[str], Output]],
+        fn: Callable[[Callable[[Input], Output]], Iterable[FnOutput]],
+        backend: Union[List[Backend], Backend],
         template_file: Optional[str],
         template: Optional[str],
-        stop_template: Optional[str],
-        fn: Callable[[Callable[[Input], Output]], FnOutput] = simple,
-        stream: bool = False,
-        block_input=None,
-        block_output=None,
+        gradio_conf: Any = None,
     ):
-        self.backend: Backend = backend
-        self.stream = stream
-        self.description: str = (
-            backend.description if hasattr(backend, "description") else ""
-        )
-        self.parser: Union[str, Callable[[str], Output]] = parser
+        self.fn = fn
+        if not isinstance(backend, List):
+            self.backend = [backend]
+        else:
+            self.backend = backend
+
         self.template_file: Optional[str] = template_file
         self.template: Optional[str] = template
-        self.stop_template: Optional[str] = stop_template
-        self.block_input = block_input
-        self.block_output = block_output
-        self.fn = fn
+        self.gradio_conf = gradio_conf
+
         self._fn: str = fn.__name__
         self._id: int = Prompt.counter.__next__()
 
-    def parse(self, response: str) -> Any:
-        """
-        Convert from the string response of the function
-        to the output type.
-        """
-        if isinstance(self.parser, str):
-            if self.parser == "str":
-                return response
-            elif self.parser == "json":
-                return json.loads(response)
+    def run(self, request: str, tool_num: int = 0) -> Iterator[RunLog]:
+        if not hasattr(self.backend[tool_num], "run_stream"):
+            yield RunLog(request, None)
+            response: Union[str, Any] = self.backend[tool_num].run(request)
+            yield RunLog(request, response)
         else:
-            return self.parser(response)
+            yield RunLog(request, None)
+            for r in self.backend[tool_num].run_stream(request):
+                yield RunLog(request, r)
 
-    def run_verbose(
-        self, r: Union[str, Request], stream=False
-    ) -> Tuple[Request, str, Output]:
-        with start_action(action_type=str(self.fn)):
-            request = _prompt(r)
-            with start_action(action_type="Prompted", prompt=request.prompt):
-                response: Union[str, Any] = self.backend.run(
-                    request
-                    if hasattr(self.backend, "needs_request")
-                    else request.prompt
-                )
-            with start_action(action_type="Response", result=response):
-                output = self.parse(response)
-        if not isinstance(response, str):
-            response = "(data)"
-        return (request, response, output)
-
-    def run_stream(
-        self, r: Union[str, Request], stream=False
-    ) -> Tuple[Request, str, Output]:
-        request = _prompt(r)
-        for r in self.backend.run_stream(
-            request if hasattr(self.backend, "needs_request") else request.prompt
-        ):
-            yield (request, r, r)
-
-    def template_fill(self, inp: Any) -> Request:
+    def template_fill(self, inp: Any) -> str:
         kwargs = inp
         if self.template_file:
             tmp = Environment(loader=FileSystemLoader(".")).get_template(
                 name=self.template_file
             )
         elif self.template:
             tmp = Template(self.template)
 
-        x = tmp.render(**kwargs)
-
-        if self.stop_template:
-            stop = [Template(self.stop_template).render(**kwargs)]
-        else:
-            stop = None
-        return Request(x, stop)
+        return str(tmp.render(**kwargs))
 
-    def __call__(self, *args: Any) -> FnOutput:
-        return Chain(History(self, args))
+    def __call__(self, *args: Any) -> Chain:
+        return Chain(History(self.expand, list(args)), self.fn.__name__)
 
     class Model:
-        def __init__(self, prompt, trial, data):
+        def __init__(self, prompt: "Prompt[Input, Output, FnOutput]", data: Any):
             self.prompt = prompt
-            self.trial = trial
             self.data = data
-            self.run_log = None
-
-        def fail(self, argnum: int, data: Any = None) -> Fail:
-            return Fail(argnum - 1, data)
-
-        def __call__(self, input_):
-            for r in self.stream(input_):
-                pass
-            return r
+            self.run_log = RunLog()
 
-        def stream(self, input_):
-            assert self.run_log is None, "Only call `model` once per function"
+        def __call__(self, model_input: Any, tool_num: int = 0) -> Any:
+            for r in self.stream(model_input, tool_num):
+                yield r
+
+            # print("hello tool")
+            # for out in self.prompt.dynamic[tool_num].expand(*model_input):
+            #     self.run_log = self.prompt.dynamic[tool_num].model.run_log
+            #     self.run_log.dynamic = tool_num
+            #     yield out
+
+        def stream(
+            self, model_input: Any, tool_num: int = 0
+        ) -> Iterator[Optional[str]]:
             if (
                 self.prompt.template is not None
                 or self.prompt.template_file is not None
             ):
-                if not isinstance(input_, dict):
-                    input_ = asdict(input_)
-                input_ = dict(**input_)
-                input_["_trial"] = self.trial
-                input_["_fail_data"] = self.data
-
-                result = self.prompt.template_fill(input_)
-            else:
-                result = input_
-            if self.prompt.stream and hasattr(self.prompt.backend, "run_stream"):
-                self.run_log = ("", "", "")
-                for a, b, c in self.prompt.run_stream(result):
-                    self.run_log = (a, self.run_log[1] + b, self.run_log[2] + c)
-                    yield c
+                if not isinstance(model_input, dict):
+                    model_input = asdict(model_input)
+                result = self.prompt.template_fill(model_input)
             else:
-                self.run_log = (Request(input_), "", "")
-                yield None
-                self.run_log = self.prompt.run_verbose(result)
-                yield self.run_log[-1]
+                result = model_input
 
-    def expand(self, args, trial=0, data=None):
+            for run_log in self.prompt.run(result, tool_num):
+                r = self.run_log.response
+                if run_log.response is None:
+                    out = r
+                elif not r:
+                    out = run_log.response
+                else:
+                    out = r + run_log.response
+                self.run_log = RunLog(run_log.request, out, dynamic=tool_num)
+                yield self.run_log.response
+
+    def expand(
+        self, *args: List[Any], data: Any = None
+    ) -> Iterator[Optional[FnOutput]]:
+        # Times prompt has been used.
         MinichainContext.prompt_count.setdefault(self._id, -1)
-        if trial == 0:
-            MinichainContext.prompt_count[self._id] += 1
+        MinichainContext.prompt_count[self._id] += 1
         count = MinichainContext.prompt_count[self._id]
-        MinichainContext.prompt_store.setdefault((self._id, count), [])
-        MinichainContext.prompt_store[self._id, count].append(("", Request(""), "", ""))
-
-        model = self.Model(self, trial, data)
-
-        if self.stream:
-            for output in self.fn(model, *args):
 
-                t = model.run_log
-                assert model.run_log, str(model)
-                run_log = (args, t[0], t[1], output)
-                count = MinichainContext.prompt_count[self._id]
-                MinichainContext.prompt_store.setdefault((self._id, count), [])
-                MinichainContext.prompt_store[self._id, count][-1] = run_log
-                yield None
-        else:
-            output = self.fn(model, *args)
+        # Snap of the prompt
+        MinichainContext.prompt_store.setdefault((self._id, count), [])
+        MinichainContext.prompt_store[self._id, count].append(PromptSnap())
 
-        if not isinstance(output, Fail):
-            assert model.run_log, str(model)
+        # Model to be passed to function
+        model = self.Model(self, data)
+        for output in self.fn(model, *args):
             t = model.run_log
-            run_log = (args, t[0], t[1], output)
-            MinichainContext.prompt_store[self._id, count][-1] = run_log
+            assert model.run_log, str(model)
+            snap = PromptSnap(args, t, output)
+            count = MinichainContext.prompt_count[self._id]
+            MinichainContext.prompt_store.setdefault((self._id, count), [])
+            MinichainContext.prompt_store[self._id, count][-1] = snap
+            yield None
 
+        assert model.run_log, str(model)
+        t = model.run_log
+        snap = PromptSnap(args, t, output)
+        MinichainContext.prompt_store[self._id, count][-1] = snap
         yield output
 
 
 def prompt(
-    backend: Backend,
-    parser: Union[str, Any] = "str",
+    backend: List[Backend] = [],
     template_file: Optional[str] = None,
     template: Optional[str] = None,
-    stop_template: Optional[str] = None,
-    stream: bool = False,
-    block_input=None,
-    block_output=None,
+    gradio_conf: Optional[Any] = None,
 ) -> Callable[[Any], Prompt[Input, Output, FnOutput]]:
-    return lambda fn: Prompt(
-        backend,
-        parser,
-        template_file,
-        template,
-        stop_template,
-        fn,
-        stream,
-        block_input,
-        block_output,
+    return lambda fn: Prompt(fn, backend, template_file, template, gradio_conf)
+
+
+def transform():  # type: ignore
+    return lambda fn: lambda *args: Chain(
+        History(lambda *x: iter((fn(*x),)), list(args)), fn.__name__
     )
```

### ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/gradio.py

```diff
@@ -15,27 +15,24 @@
 #clean div.form {border: 0px}
 #response {border: 0px; background: #ffeec6}
 #prompt {border: 0px;background: aliceblue}
 #json {border: 0px}
 span.head {font-size: 60pt; font-family: cursive;}
 div.gradio-container {color: black}
 div.form {background: inherit}
-div.form div {background: inherit}
+div.form div.block {padding: 0px; background: #fcfcfc}
 """
-# #result {border: 0px; background: #c5e0e5}
-# #inner {margin: 10px; padding: 10px; font-size: 20px; }
-# #inner textarea {border: 0px}
-
-# body {
-#   --text-sm: 15px;
-#   --text-md: 20px;
-#   --text-lg: 22px;
-#   --input-text-size: 20px;
-#   --section-text-size: 20px;
-# }
+
+
+@dataclass
+class GradioConf:
+    block_input: Callable[[], gr.Blocks] = lambda: gr.Textbox(show_label=False)
+    block_output: Callable[[], gr.Blocks] = lambda: gr.Textbox(show_label=False)
+    postprocess_output: Callable[[Any], Any] = lambda x: x
+    preprocess_input: Callable[[Any], Any] = lambda x: x
 
 
 @dataclass
 class HTML:
     html: str
 
     def _repr_html_(self) -> str:
@@ -76,115 +73,140 @@
         return out
 
 
 def to_gradio_block(
     base_prompt: Prompt[Any, Any, Any],
     i: int,
     display_options: DisplayOptions = DisplayOptions(),
+    show_advanced: bool = True,
 ) -> Constructor:
+    prompts = []
+    results = []
+    bp = base_prompt
+    with gr.Accordion(
+        label=f"👩  Prompt: {str(base_prompt._fn)}", elem_id="prompt", visible=False
+    ) as accordion_in:
+        for backend in base_prompt.backend:
+            if bp.gradio_conf is not None:
+                prompt = bp.gradio_conf.block_input()
+            elif hasattr(backend, "block_input"):
+                prompt = backend.block_input()
+            else:
+                prompt = GradioConf().block_input()
+            prompts.append(prompt)
+
+    with gr.Accordion(label="💻", elem_id="response", visible=False) as accordion_out:
+        for backend in base_prompt.backend:
+            if bp.gradio_conf is not None:
+                result = bp.gradio_conf.block_output()
+            elif hasattr(backend, "block_output"):
+                result = backend.block_output()
+            else:
+                result = GradioConf().block_output()
+            results.append(result)
+
+        with gr.Accordion(label="...", open=False, visible=show_advanced):
+            gr.Markdown(f"Backend: {base_prompt.backend}", elem_id="json")
+            input = gr.JSON(elem_id="json", label="Input")
+            json = gr.JSON(elem_id="json", label="Output")
+
+            if base_prompt.template_file:
+                gr.Code(
+                    label=f"Template: {base_prompt.template_file}",
+                    value=open(base_prompt.template_file).read(),
+                    elem_id="inner",
+                )
+                # btn = gr.Button("Modify Template")
+                # if base_prompt.template_file is not None:
+
+                #     def update_template(template: str) -> None:
+                #         if base_prompt.template_file is not None:
+                #             with open(base_prompt.template_file, "w") as doc:
+                #                 doc.write(template)
 
-    with gr.Accordion(label=f"👩  Prompt: {str(base_prompt._fn)}", elem_id="prompt"):
-        if base_prompt.block_input is not None:
-            prompt = base_prompt.block_input()
-        elif hasattr(base_prompt.backend, "block_input"):
-            prompt = base_prompt.backend.block_input()
-        else:
-            prompt = gr.Textbox(label="")
-
-    with gr.Accordion(label="💻", elem_id="response"):
-        if base_prompt.block_output is not None:
-            result = base_prompt.block_output()
-        elif hasattr(base_prompt.backend, "block_output"):
-            result = base_prompt.backend.block_output()
-        else:
-            result = gr.Textbox(label="")
-
-    with gr.Accordion(label="...", elem_id="advanced", open=False):
-        gr.Markdown(f"Backend: {base_prompt.backend}", elem_id="json")
-        input = gr.JSON(elem_id="json", label="Input")
-        json = gr.JSON(elem_id="json", label="Output")
-        trial = gr.JSON(elem_id="json", label="Previous Trial")
-
-        if base_prompt.template_file:
-            # gr.Markdown(f"<center>{base_prompt.template_file}</center>")
-            gr.Code(
-                label=f"Template: {base_prompt.template_file}",
-                value=open(base_prompt.template_file).read(),
-                elem_id="inner",
-            )
-            # btn = gr.Button("Modify Template")
-            # if base_prompt.template_file is not None:
-
-            #     def update_template(template: str) -> None:
-            #         if base_prompt.template_file is not None:
-            #             with open(base_prompt.template_file, "w") as doc:
-            #                 doc.write(template)
-
-            #     btn.click(update_template, inputs=c)
+                #     btn.click(update_template, inputs=c)
 
     def update(data: Dict[Block, Any]) -> Dict[Block, Any]:
+        "Update the prompt block"
         prev_request_ = ""
         if (base_prompt._id, i) not in data[all_data]:
-            return {}
+            ret = {}
+            for p, r in zip(prompts, results):
+                ret[p] = gr.update(visible=False)
+                ret[r] = gr.update(visible=False)
+            return ret
 
         if (base_prompt._id, i - 1) in data[all_data]:
-            prev_request_ = data[all_data][base_prompt._id, i - 1][-1][1].prompt
-        trials = len(data[all_data][base_prompt._id, i])
-        input_, request_, response_, output_ = data[all_data][base_prompt._id, i][-1]
+            prev_request_ = data[all_data][base_prompt._id, i - 1][-1].run_log.request
+
+        snap = data[all_data][base_prompt._id, i][-1]
+        input_, request_, response_, output_ = (
+            snap.input_,
+            snap.run_log.request,
+            snap.run_log.response,
+            snap.output,
+        )
 
         def format(s: Any) -> Any:
             if isinstance(s, str):
                 return {"string": s}
             return s
 
         def mark(s: Any) -> Any:
             return str(s)  # f"```text\n{s}\n```"
 
         j = 0
-        for (a, b) in zip(request_.prompt, prev_request_):
+        for (a, b) in zip(request_, prev_request_):
             if a != b:
                 break
             j += 1
 
-        if j > 30:
-            new_prompt = "...\n" + request_.prompt[j:]
-        else:
-            new_prompt = request_.prompt
-
-        if trials == 1:
-            previous_trials = []
-        else:
-            trial_input_, trial_request_, trial_response_, trial_output_ = data[
-                all_data
-            ][base_prompt._id, i][trials - 2]
-            previous_trials = {
-                "input": trial_input_,
-                "prompt": trial_request_.prompt,
-                "response": trial_response_,
-                "output": trial_output_,
-            }
+        if base_prompt.gradio_conf is not None:
+            request_ = base_prompt.gradio_conf.preprocess_input(request_)
+            output_ = base_prompt.gradio_conf.postprocess_output(output_)
+        # if j > 30:
+        #     new_prompt = "...\n" + request_[j:]
+        # else:
+        new_prompt = request_
+
         ret = {
             input: format(input_),
-            prompt: mark(new_prompt),
-            result: mark(output_),
             json: format(response_),
-            trial: previous_trials,
+            accordion_in: gr.update(visible=True),
+            accordion_out: gr.update(visible=bool(output_)),
         }
+        for j, (prompt, result) in enumerate(zip(prompts, results)):
+            if j == snap.run_log.dynamic:
+                ret[prompt] = gr.update(value=new_prompt, visible=True)
+                if output_:
+                    ret[result] = gr.update(value=output_, visible=True)
+                else:
+                    ret[result] = gr.update(visible=True)
+            else:
+                ret[prompt] = gr.update(visible=False)
+                ret[result] = gr.update(visible=False)
+
         return ret
 
-    return Constructor([update], set(), {input, prompt, result, json, trial})
+    return Constructor(
+        [update],
+        set(),
+        {accordion_in, accordion_out, input, json} | set(prompts) | set(results),
+    )
 
 
-def chain_blocks(prompts: List[Prompt[Any, Any, Any]]) -> Constructor:
+def chain_blocks(
+    prompts: List[Prompt[Any, Any, Any]], show_advanced: bool = True
+) -> Constructor:
     cons = Constructor()
-    count = {}
+    count: Dict[int, int] = {}
     for p in prompts:
         count.setdefault(p._id, 0)
         i = count[p._id]
-        cons = cons.merge(to_gradio_block(p, i))
+        cons = cons.merge(to_gradio_block(p, i, show_advanced=show_advanced))
         count[p._id] += 1
     return cons
 
 
 def api_keys(keys: Set[str] = {"OPENAI_API_KEY"}) -> None:
     if all([k in os.environ for k in keys]):
         return
@@ -248,15 +270,16 @@
     subprompts: List[Prompt[Any, Any, Any]] = [],
     fields: List[str] = [],
     initial_state: Any = None,
     out_type: str = "markdown",
     keys: Set[str] = {"OPENAI_API_KEY"},
     description: str = "",
     code: str = "",
-    css="",
+    css: str = "",
+    show_advanced: bool = True,
 ) -> gr.Blocks:
     """
     Constructs a gradio component to show a prompt chain.
 
     Args:
         prompt: A prompt or prompt chain to display.
         examples: A list of example inputs, either string or tuples of fields
@@ -264,14 +287,15 @@
         fields: The names of the field input to the prompt.
         initial_state: For stateful prompts, the initial value.
         out_type: type of final output
         keys: user keys required
         description: description of the model
         code: code to display
         css : additional css
+        show_advanced : show the "..." advanced elements
 
     Returns:
         Gradio block
     """
     fields = [arg for arg in inspect.getfullargspec(prompt).args if arg != "state"]
     with gr.Blocks(css=CSS + "\n" + css, theme=gr.themes.Monochrome()) as demo:
         # API Keys
@@ -288,27 +312,30 @@
 
         # Build the top query box with one input for each field.
         inputs = list([gr.Textbox(label=f) for f in fields])
         examples = gr.Examples(examples=examples, inputs=inputs)
         query_btn = gr.Button(label="Run")
         constructor = constructor.add_inputs(inputs)
 
-        # Intermediate prompt displays
-        constructor = constructor.merge(chain_blocks(subprompts))
+        with gr.Box():
+            # Intermediate prompt displays
+            constructor = constructor.merge(
+                chain_blocks(subprompts, show_advanced=show_advanced)
+            )
 
         # Final Output result
-        with gr.Accordion(label="✔️", elem_id="result"):
-            typ = gr.JSON if out_type == "json" else gr.Markdown
-            output = typ(elem_id="inner")
+        # with gr.Accordion(label="✔️", elem_id="result"):
+        # typ = gr.JSON if out_type == "json" else gr.Markdown
+        # output = typ(elem_id="inner")
 
         def output_fn(data: Dict[Block, Any]) -> Dict[Block, Any]:
             final = data[final_output]
-            return {state: final, output: final}
+            return {state: final}  # output: final}
 
-        constructor = constructor.merge(Constructor([output_fn], set(), {output}))
+        constructor = constructor.merge(Constructor([output_fn], set(), set()))
 
         def run(data):  # type: ignore
             prompt_inputs = {k: data[v] for k, v in zip(fields, inputs)}
             if initial_state is not None:
                 prompt_inputs["state"] = data[state]
 
             with start_chain("temp"):
```

### Comparing `./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain-0.2.3.egg-info/PKG-INFO` & `./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain-0.3.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minichain
-Version: 0.2.3
+Version: 0.3
 Summary: A tiny library for large language models
 Home-page: https://github.com/srush/minichain
 Author: Sasha Rush
 Author-email: srush.research@gmail.com
 License: MIT
 Project-URL: Documentation, https://srush.github.io/minichain
 Project-URL: Source Code, https://github.com/srush/minichain
@@ -26,23 +26,24 @@
 A tiny library for coding with **large** language models. Check out the [MiniChain Zoo](https://srush-minichain.hf.space/) to get a sense of how it works.
 
 ## Coding
 
 * Code ([math_demo.py](https://github.com/srush/MiniChain/blob/main/examples/math_demo.py)): Annotate Python functions that call language models.
 
 ```python
-@prompt(OpenAI(), template_file="math.pmpt.tpl")
+@prompt(OpenAI(), template_file="math.pmpt.tpl"
 def math_prompt(model, question):
     "Prompt to call GPT with a Jinja template"
     return model(dict(question=question))
 
-@prompt(Python())
+@prompt(Python(), template="import math\n{{code}}")
 def python(model, code):
     "Prompt to call Python interpreter"
-    return int(model(code))
+    code = "\n".join(code.strip().split("\n")[1:-1])
+    return model(dict(code=code))
 
 def math_demo(question):
     "Chain them together"
     return python(math_prompt(question))
 ```
 
 * Chains ([Space](https://srush-minichain.hf.space/)): MiniChain builds a graph (think like PyTorch) of all the calls you make for debugging and error handling.
@@ -50,15 +51,15 @@
 
 
 ```python
 show(math_demo,
      examples=["What is the sum of the powers of 3 (3^i) that are smaller than 100?",
                "What is the sum of the 10 first positive integers?"],
      subprompts=[math_prompt, python],
-     out_type="markdown").launch()
+     out_type="markdown").queue().launch()
 ```
 
 
 * Template ([math.pmpt.tpl](https://github.com/srush/MiniChain/blob/main/examples/math.pmpt.tpl)): Prompts are separated from code.
 
 ```
 ...
@@ -71,15 +72,15 @@
 {{question}}
 Code:
 ```
 
 * Installation
 
 ```bash
-pip install git+https://github.com/srush/MiniChain/
+pip install minichain
 export OPENAI_API_KEY="sk-***"
 ```
 
 ## Examples
 
 This library allows us to implement several popular approaches in a few lines of code.
 
@@ -116,42 +117,47 @@
 
 ![image](https://user-images.githubusercontent.com/35882/221280012-d58c186d-4da2-4cb6-96af-4c4d9069943f.png)
 
 
 ```python
 @prompt(OpenAI())
 def color_prompt(model, input):
-    response = model(f"Answer 'Yes' if this is a color, {input}. Answer:")
-    return out == "Yes"
+    return model(f"Answer 'Yes' if this is a color, {input}. Answer:")
 ```
 
 Prompt functions act like python functions, except they are lazy to access the result you need to call `run()`.
 
 ```python
-if color_prompt("blue").run():
+if color_prompt("blue").run() == "Yes":
     print("It's a color")
 ```
-Alternatively you can chain prompts together.
+Alternatively you can chain prompts together. Prompts are lazy, so if you want to manipulate them you need to add `@transform()` to your function. For example:
+
+```python
+@transform()
+def said_yes(input):
+    return input == "Yes"
+```
 
 ![image](https://user-images.githubusercontent.com/35882/221281771-3770be96-02ce-4866-a6f8-c458c9a11c6f.png)
 
 ```python
 @prompt(OpenAI())
 def adjective_prompt(model, input):
     return model(f"Give an adjective to describe {input}. Answer:")
 ```
 
 
 ```python
 adjective = adjective_prompt("rainbow")
-if color_prompt(adjective).run():
+if said_yes(color_prompt(adjective)).run():
     print("It's a color")
-
 ```
 
+
 We also include an argument `template_file` which assumes model uses template from the
 [Jinja](https://jinja.palletsprojects.com/en/3.1.x/templates/) language.
 This allows us to separate prompt text from the python code.
 
 ```python
 @prompt(OpenAI(), template_file="math.pmpt.tpl")
 def math_prompt(model, question):
@@ -165,18 +171,17 @@
 by calling `show` and `launch`. This can be done directly in a notebook as well.
 
 ```python
 show(math_demo,
      examples=["What is the sum of the powers of 3 (3^i) that are smaller than 100?",
               "What is the sum of the 10 first positive integers?"],
      subprompts=[math_prompt, python],
-     out_type="markdown").launch()
+     out_type="markdown").queue().launch()
 ```
 
-You can also get the full log the process by calling `set_minichain_log('chain_name')`.
 
 ### Memory
 
 MiniChain does not build in an explicit stateful memory class. We recommend implementing it as a queue.
 
 ![image](https://user-images.githubusercontent.com/35882/221622653-7b13783e-0439-4d59-8f57-b98b82ab83c0.png)
 
@@ -189,17 +194,26 @@
     human_input: str = ""
 
     def push(self, response: str) -> "State":
         memory = self.memory if len(self.memory) < MEMORY_LIMIT else self.memory[1:]
         return State(memory + [(self.human_input, response)])
 ```
 
-See the full [Chat](https://srush.github.io/MiniChain/examples/chatgpt/) example.
+See the full Chat example.
 It keeps track of the last two responses that it has seen.
 
+### Tools and agents.
+
+MiniChain does not provide `agents` or `tools`. If you want that functionality you can use the `tool_num` argument of model which allows you to select from multiple different possible backends. It's easy to add new backends of your own (see the GradioExample).
+
+```python
+@prompt([Python(), Bash()])
+def math_prompt(model, input, lang):
+    return model(input, tool_num= 0 if lang == "python" else 1)
+```
 
 ### Documents and Embeddings
 
 MiniChain does not manage documents and embeddings. We recommend using
 the [Hugging Face Datasets](https://huggingface.co/docs/datasets/index) library with
 built in FAISS indexing.
```

### Comparing `./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain-0.2.3.egg-info/SOURCES.txt` & `./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain-0.3.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 setup.cfg
 setup.py
 minichain/__init__.py
 minichain/backend.py
 minichain/base.py
 minichain/gradio.py
+minichain/push_to_hub.py
 minichain.egg-info/PKG-INFO
 minichain.egg-info/SOURCES.txt
 minichain.egg-info/dependency_links.txt
 minichain.egg-info/requires.txt
 minichain.egg-info/top_level.txt
 minichain/prompts/__init__.py
 minichain/prompts/search.py
```


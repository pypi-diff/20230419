# Comparing `tmp/minichain-0.3.1.linux-x86_64.tar.gz` & `tmp/minichain-0.3.2.linux-x86_64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minichain-0.3.1.linux-x86_64.tar", last modified: Tue Apr 18 22:17:14 2023, max compression
+gzip compressed data, was "minichain-0.3.2.linux-x86_64.tar", last modified: Wed Apr 19 15:10:31 2023, max compression
```

## Comparing `minichain-0.3.1.linux-x86_64.tar` & `minichain-0.3.2.linux-x86_64.tar`

### file list

```diff
@@ -1,45 +1,42 @@
-drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-18 22:17:14.678467 ./
-drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-18 22:17:14.678467 ./home/
-drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-18 22:17:14.678467 ./home/srush/
-drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-18 22:17:14.678467 ./home/srush/Projects/
-drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-18 22:17:14.678467 ./home/srush/Projects/MiniChain/
-drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-18 22:17:14.678467 ./home/srush/Projects/MiniChain/venv/
-drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-18 22:17:14.678467 ./home/srush/Projects/MiniChain/venv/lib/
-drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-18 22:17:14.678467 ./home/srush/Projects/MiniChain/venv/lib/python3.10/
-drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-18 22:17:14.690467 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/
-drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-18 22:17:14.678467 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/
+drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-19 15:10:31.362680 ./
+drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-19 15:10:31.362680 ./home/
+drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-19 15:10:31.362680 ./home/srush/
+drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-19 15:10:31.362680 ./home/srush/Projects/
+drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-19 15:10:31.362680 ./home/srush/Projects/MiniChain/
+drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-19 15:10:31.362680 ./home/srush/Projects/MiniChain/venv/
+drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-19 15:10:31.362680 ./home/srush/Projects/MiniChain/venv/lib/
+drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-19 15:10:31.362680 ./home/srush/Projects/MiniChain/venv/lib/python3.10/
+drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-19 15:10:31.374681 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/
+drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-19 15:10:31.362680 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/
 -rw-rw-r--   0 srush     (1000) srush     (1000)      275 2023-04-18 21:18:59.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/__init__.py
-drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-18 22:17:14.690467 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/__pycache__/
--rw-rw-r--   0 srush     (1000) srush     (1000)      557 2023-04-18 22:17:14.682467 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 srush     (1000) srush     (1000)    13031 2023-04-18 22:17:14.682467 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/__pycache__/backend.cpython-310.pyc
--rw-rw-r--   0 srush     (1000) srush     (1000)     6140 2023-04-18 22:17:14.690467 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/__pycache__/base.cpython-310.pyc
--rw-rw-r--   0 srush     (1000) srush     (1000)    10254 2023-04-18 22:17:14.686467 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/__pycache__/gradio.cpython-310.pyc
--rw-rw-r--   0 srush     (1000) srush     (1000)     3239 2023-04-18 22:17:14.686467 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/__pycache__/prompts.cpython-310.pyc
--rw-rw-r--   0 srush     (1000) srush     (1000)     1405 2023-04-18 22:17:14.686467 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/__pycache__/push_to_hub.cpython-310.pyc
--rw-rw-r--   0 srush     (1000) srush     (1000)    10444 2023-04-18 21:30:52.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/backend.py
+drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-19 15:10:31.370680 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/__pycache__/
+-rw-rw-r--   0 srush     (1000) srush     (1000)      557 2023-04-19 15:10:31.362680 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 srush     (1000) srush     (1000)    12915 2023-04-19 15:10:31.366680 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/__pycache__/backend.cpython-310.pyc
+-rw-rw-r--   0 srush     (1000) srush     (1000)     6140 2023-04-19 15:10:31.370680 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/__pycache__/base.cpython-310.pyc
+-rw-rw-r--   0 srush     (1000) srush     (1000)    10254 2023-04-19 15:10:31.366680 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/__pycache__/gradio.cpython-310.pyc
+-rw-rw-r--   0 srush     (1000) srush     (1000)     1405 2023-04-19 15:10:31.370680 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/__pycache__/push_to_hub.cpython-310.pyc
+-rw-rw-r--   0 srush     (1000) srush     (1000)    10480 2023-04-19 13:01:49.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/backend.py
 -rw-rw-r--   0 srush     (1000) srush     (1000)     6608 2023-04-18 21:18:59.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/base.py
--rw-rw-r--   0 srush     (1000) srush     (1000)    11605 2023-04-18 21:30:57.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/gradio.py
--rw-rw-r--   0 srush     (1000) srush     (1000)      701 2023-02-12 12:11:05.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/lang.py
-drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-18 22:17:14.686467 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/prompts/
+-rw-rw-r--   0 srush     (1000) srush     (1000)    11660 2023-04-19 13:01:32.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/gradio.py
+drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-19 15:10:31.370680 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/prompts/
 -rw-rw-r--   0 srush     (1000) srush     (1000)        1 2023-03-18 14:29:59.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/prompts/__init__.py
-drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-18 22:17:14.686467 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/prompts/__pycache__/
--rw-rw-r--   0 srush     (1000) srush     (1000)      187 2023-04-18 22:17:14.686467 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/prompts/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 srush     (1000) srush     (1000)      998 2023-04-18 22:17:14.686467 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/prompts/__pycache__/search.cpython-310.pyc
--rw-rw-r--   0 srush     (1000) srush     (1000)     1662 2023-04-18 22:17:14.686467 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/prompts/__pycache__/template.cpython-310.pyc
--rw-rw-r--   0 srush     (1000) srush     (1000)     2573 2023-04-18 22:17:14.686467 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/prompts/__pycache__/typed.cpython-310.pyc
+drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-19 15:10:31.370680 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/prompts/__pycache__/
+-rw-rw-r--   0 srush     (1000) srush     (1000)      187 2023-04-19 15:10:31.370680 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/prompts/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 srush     (1000) srush     (1000)      998 2023-04-19 15:10:31.370680 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/prompts/__pycache__/search.cpython-310.pyc
+-rw-rw-r--   0 srush     (1000) srush     (1000)     1662 2023-04-19 15:10:31.370680 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/prompts/__pycache__/template.cpython-310.pyc
+-rw-rw-r--   0 srush     (1000) srush     (1000)     2573 2023-04-19 15:10:31.370680 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/prompts/__pycache__/typed.cpython-310.pyc
 -rw-rw-r--   0 srush     (1000) srush     (1000)      510 2023-03-18 15:59:30.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/prompts/search.py
 -rw-rw-r--   0 srush     (1000) srush     (1000)     1370 2023-03-18 15:58:48.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/prompts/template.py
 -rw-rw-r--   0 srush     (1000) srush     (1000)     1469 2023-03-18 15:57:47.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/prompts/typed.py
--rw-rw-r--   0 srush     (1000) srush     (1000)     2458 2023-02-27 19:02:03.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/prompts.py
 -rw-rw-r--   0 srush     (1000) srush     (1000)     1588 2023-04-14 14:16:21.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/push_to_hub.py
-drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-18 22:17:14.678467 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/templates/
+drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-19 15:10:31.362680 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/templates/
 -rw-rw-r--   0 srush     (1000) srush     (1000)        5 2023-02-12 11:12:06.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/templates/anthropic_hhh.tpl
 -rw-rw-r--   0 srush     (1000) srush     (1000)      578 2023-02-24 21:33:28.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/templates/prompt.html.tpl
 -rw-rw-r--   0 srush     (1000) srush     (1000)       46 2023-02-12 11:15:28.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/templates/self_instruct.tpl
 -rw-rw-r--   0 srush     (1000) srush     (1000)      975 2023-03-23 19:57:44.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/templates/type_prompt.pmpt.tpl
-drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-18 22:17:14.690467 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain-0.3.1.egg-info/
--rw-rw-r--   0 srush     (1000) srush     (1000)    10228 2023-04-18 22:17:14.674467 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain-0.3.1.egg-info/PKG-INFO
--rw-rw-r--   0 srush     (1000) srush     (1000)      574 2023-04-18 22:17:14.674467 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain-0.3.1.egg-info/SOURCES.txt
--rw-rw-r--   0 srush     (1000) srush     (1000)        1 2023-04-18 22:17:14.674467 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain-0.3.1.egg-info/dependency_links.txt
--rw-rw-r--   0 srush     (1000) srush     (1000)      113 2023-04-18 22:17:14.674467 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain-0.3.1.egg-info/requires.txt
--rw-rw-r--   0 srush     (1000) srush     (1000)       10 2023-04-18 22:17:14.674467 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain-0.3.1.egg-info/top_level.txt
+drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-19 15:10:31.374681 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain-0.3.2.egg-info/
+-rw-rw-r--   0 srush     (1000) srush     (1000)    10228 2023-04-19 15:10:31.358679 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain-0.3.2.egg-info/PKG-INFO
+-rw-rw-r--   0 srush     (1000) srush     (1000)      574 2023-04-19 15:10:31.358679 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain-0.3.2.egg-info/SOURCES.txt
+-rw-rw-r--   0 srush     (1000) srush     (1000)        1 2023-04-19 15:10:31.358679 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain-0.3.2.egg-info/dependency_links.txt
+-rw-rw-r--   0 srush     (1000) srush     (1000)      113 2023-04-19 15:10:31.358679 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain-0.3.2.egg-info/requires.txt
+-rw-rw-r--   0 srush     (1000) srush     (1000)       10 2023-04-19 15:10:31.358679 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain-0.3.2.egg-info/top_level.txt
```

### ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/__pycache__/backend.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 21:30:52 2023 UTC, .py size: 10444 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,815 +1,808 @@
-00000000: 6f0d 0d0a 0000 0000 0c0c 3f64 cc28 0000  o.........?d.(..
+00000000: 6f0d 0d0a 0000 0000 3de6 3f64 f028 0000  o.......=.?d.(..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 ae01 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 a601 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c05 6d06 5a06 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 6d09 5a09 6d0a 5a0a  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  m.Z.m.Z.m.Z.m.Z.
-00000080: 0100 6400 6401 6c0f 5a10 6400 6405 6c11  ..d.d.l.Z.d.d.l.
-00000090: 6d12 5a12 6d13 5a13 0100 6508 723c 6400  m.Z.m.Z...e.r<d.
-000000a0: 6401 6c14 5a14 4700 6406 6407 8400 6407  d.l.Z.G.d.d...d.
-000000b0: 8302 5a15 4700 6408 6409 8400 6409 6515  ..Z.G.d.d...d.e.
-000000c0: 8303 5a16 4700 640a 640b 8400 640b 6515  ..Z.G.d.d...d.e.
-000000d0: 8303 5a17 4700 640c 640d 8400 640d 6515  ..Z.G.d.d...d.e.
-000000e0: 8303 5a18 4700 640e 640f 8400 640f 6515  ..Z.G.d.d...d.e.
-000000f0: 8303 5a19 4700 6410 6411 8400 6411 6515  ..Z.G.d.d...d.e.
-00000100: 8303 5a1a 4700 6412 6413 8400 6413 6515  ..Z.G.d.d...d.e.
-00000110: 8303 5a1b 4700 6414 6415 8400 6415 651b  ..Z.G.d.d...d.e.
-00000120: 8303 5a1c 4700 6416 6417 8400 6417 651b  ..Z.G.d.d...d.e.
-00000130: 8303 5a1d 4700 6418 6419 8400 6419 6515  ..Z.G.d.d...d.e.
-00000140: 8303 5a1e 4700 641a 641b 8400 641b 651e  ..Z.G.d.d...d.e.
-00000150: 8303 5a1f 4700 641c 641d 8400 641d 651e  ..Z.G.d.d...d.e.
-00000160: 8303 5a20 4700 641e 641f 8400 641f 6515  ..Z G.d.d...d.e.
-00000170: 8303 5a21 6504 4700 6420 6421 8400 6421  ..Z!e.G.d d!..d!
-00000180: 8302 8301 5a22 6504 4700 6422 6423 8400  ....Z"e.G.d"d#..
-00000190: 6423 8302 8301 5a23 4700 6424 6425 8400  d#....Z#G.d$d%..
-000001a0: 6425 8302 5a24 6426 6525 6427 6401 6604  d%..Z$d&e%d'd.f.
-000001b0: 6428 6429 8404 5a26 4700 642a 642b 8400  d(d)..Z&G.d*d+..
-000001c0: 642b 8302 5a27 6426 6525 6427 6527 6604  d+..Z'd&e%d'e'f.
-000001d0: 642c 642d 8404 5a28 6401 5300 292e e900  d,d-..Z(d.S.)...
-000001e0: 0000 004e 2901 da09 6461 7461 636c 6173  ...N)...dataclas
-000001f0: 7329 01da 0d54 7261 6365 6261 636b 5479  s)...TracebackTy
-00000200: 7065 2907 da0d 5459 5045 5f43 4845 434b  pe)...TYPE_CHECK
-00000210: 494e 47da 0341 6e79 da04 4469 6374 da08  ING..Any..Dict..
-00000220: 4974 6572 6174 6f72 da04 4c69 7374 da08  Iterator..List..
-00000230: 4f70 7469 6f6e 616c da05 5475 706c 6529  Optional..Tuple)
-00000240: 02da 0c73 7461 7274 5f61 6374 696f 6eda  ...start_action.
-00000250: 0774 6f5f 6669 6c65 6300 0000 0000 0000  .to_filec.......
-00000260: 0000 0000 0000 0000 0005 0000 0040 0000  .............@..
-00000270: 0073 7800 0000 6500 5a01 6400 5a02 6503  .sx...e.Z.d.Z.e.
-00000280: 6401 6504 6602 6402 6403 8404 8301 5a05  d.e.f.d.d.....Z.
-00000290: 6404 6504 6401 6504 6604 6405 6406 8404  d.e.d.e.f.d.d...
-000002a0: 5a06 6404 6504 6401 6507 6504 1900 6604  Z.d.e.d.e.e...f.
-000002b0: 6407 6408 8404 5a08 6404 6504 6401 6504  d.d...Z.d.e.d.e.
-000002c0: 6604 6409 640a 8404 5a09 6401 650a 6a0b  f.d.d...Z.d.e.j.
-000002d0: 6602 640b 640c 8404 5a0c 6401 650a 6a0b  f.d.d...Z.d.e.j.
-000002e0: 6602 640d 640e 8404 5a0d 640f 5300 2910  f.d.d...Z.d.S.).
-000002f0: da07 4261 636b 656e 64da 0672 6574 7572  ..Backend..retur
-00000300: 6e63 0100 0000 0000 0000 0000 0000 0100  nc..............
-00000310: 0000 0100 0000 4300 0000 f304 0000 0064  ......C........d
-00000320: 0153 00a9 024e da00 a900 a901 da04 7365  .S...N........se
-00000330: 6c66 7212 0000 0072 1200 0000 fa55 2f68  lfr....r.....U/h
-00000340: 6f6d 652f 7372 7573 682f 5072 6f6a 6563  ome/srush/Projec
-00000350: 7473 2f4d 696e 6943 6861 696e 2f76 656e  ts/MiniChain/ven
-00000360: 762f 6c69 622f 7079 7468 6f6e 332e 3130  v/lib/python3.10
-00000370: 2f73 6974 652d 7061 636b 6167 6573 2f6d  /site-packages/m
-00000380: 696e 6963 6861 696e 2f62 6163 6b65 6e64  inichain/backend
-00000390: 2e70 79da 0b64 6573 6372 6970 7469 6f6e  .py..description
-000003a0: 1000 0000 7302 0000 0004 027a 1342 6163  ....s......z.Bac
-000003b0: 6b65 6e64 2e64 6573 6372 6970 7469 6f6e  kend.description
-000003c0: da07 7265 7175 6573 7463 0200 0000 0000  ..requestc......
-000003d0: 0000 0000 0000 0200 0000 0100 0000 4300  ..............C.
-000003e0: 0000 7304 0000 0074 0082 01a9 014e 2901  ..s....t.....N).
-000003f0: da13 4e6f 7449 6d70 6c65 6d65 6e74 6564  ..NotImplemented
-00000400: 4572 726f 72a9 0272 1400 0000 7217 0000  Error..r....r...
-00000410: 0072 1200 0000 7212 0000 0072 1500 0000  .r....r....r....
-00000420: da03 7275 6e14 0000 00f3 0200 0000 0401  ..run...........
-00000430: 7a0b 4261 636b 656e 642e 7275 6e63 0200  z.Backend.runc..
-00000440: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-00000450: 0000 6300 0000 7312 0000 0081 007c 00a0  ..c...s......|..
-00000460: 007c 01a1 0156 0001 0064 0053 0072 1800  .|...V...d.S.r..
-00000470: 0000 a901 721b 0000 0072 1a00 0000 7212  ....r....r....r.
-00000480: 0000 0072 1200 0000 7215 0000 00da 0a72  ...r....r......r
-00000490: 756e 5f73 7472 6561 6d17 0000 0073 0400  un_stream....s..
-000004a0: 0000 0280 1001 7a12 4261 636b 656e 642e  ......z.Backend.
-000004b0: 7275 6e5f 7374 7265 616d 6302 0000 0000  run_streamc.....
-000004c0: 0000 0000 0000 0002 0000 0003 0000 00c3  ................
-000004d0: 0000 0073 0c00 0000 8101 7c00 a000 7c01  ...s......|...|.
-000004e0: a101 5300 7218 0000 0072 1d00 0000 721a  ..S.r....r....r.
-000004f0: 0000 0072 1200 0000 7212 0000 0072 1500  ...r....r....r..
-00000500: 0000 da04 6172 756e 1a00 0000 7304 0000  ....arun....s...
-00000510: 0002 800a 017a 0c42 6163 6b65 6e64 2e61  .....z.Backend.a
-00000520: 7275 6e63 0100 0000 0000 0000 0000 0000  runc............
-00000530: 0100 0000 0300 0000 4300 0000 f30c 0000  ........C.......
-00000540: 0074 006a 0164 0164 028d 0153 00a9 034e  .t.j.d.d...S...N
-00000550: 4629 01da 0a73 686f 775f 6c61 6265 6ca9  F)...show_label.
-00000560: 02da 0267 72da 0754 6578 7462 6f78 7213  ...gr..Textboxr.
-00000570: 0000 0072 1200 0000 7212 0000 0072 1500  ...r....r....r..
-00000580: 0000 da0b 626c 6f63 6b5f 696e 7075 741d  ....block_input.
-00000590: 0000 00f3 0200 0000 0c01 7a13 4261 636b  ..........z.Back
-000005a0: 656e 642e 626c 6f63 6b5f 696e 7075 7463  end.block_inputc
-000005b0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-000005c0: 0300 0000 4300 0000 7220 0000 0072 2100  ....C...r ...r!.
-000005d0: 0000 7223 0000 0072 1300 0000 7212 0000  ..r#...r....r...
-000005e0: 0072 1200 0000 7215 0000 00da 0c62 6c6f  .r....r......blo
-000005f0: 636b 5f6f 7574 7075 7420 0000 0072 2700  ck_output ...r'.
-00000600: 0000 7a14 4261 636b 656e 642e 626c 6f63  ..z.Backend.bloc
-00000610: 6b5f 6f75 7470 7574 4e29 0eda 085f 5f6e  k_outputN)...__n
-00000620: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-00000630: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
-00000640: 0870 726f 7065 7274 79da 0373 7472 7216  .property..strr.
-00000650: 0000 0072 1b00 0000 7207 0000 0072 1e00  ...r....r....r..
-00000660: 0000 721f 0000 0072 2400 0000 da06 426c  ..r....r$.....Bl
-00000670: 6f63 6b73 7226 0000 0072 2800 0000 7212  ocksr&...r(...r.
-00000680: 0000 0072 1200 0000 7212 0000 0072 1500  ...r....r....r..
-00000690: 0000 720d 0000 000f 0000 0073 1000 0000  ..r........s....
-000006a0: 0800 0201 1001 1203 1603 1203 1003 1403  ................
-000006b0: 720d 0000 0063 0000 0000 0000 0000 0000  r....c..........
-000006c0: 0000 0000 0000 0400 0000 4000 0000 f31e  ..........@.....
-000006d0: 0000 0065 005a 0164 005a 0264 0165 0364  ...e.Z.d.Z.d.e.d
-000006e0: 0265 0366 0464 0364 0484 045a 0464 0553  .e.f.d.d...Z.d.S
-000006f0: 0029 06da 0249 6472 1700 0000 720e 0000  .)...Idr....r...
-00000700: 0063 0200 0000 0000 0000 0000 0000 0200  .c..............
-00000710: 0000 0100 0000 4300 0000 7304 0000 007c  ......C...s....|
-00000720: 0153 0072 1800 0000 7212 0000 0072 1a00  .S.r....r....r..
-00000730: 0000 7212 0000 0072 1200 0000 7215 0000  ..r....r....r...
-00000740: 0072 1b00 0000 2500 0000 721c 0000 007a  .r....%...r....z
-00000750: 0649 642e 7275 6e4e a905 7229 0000 0072  .Id.runN..r)...r
-00000760: 2a00 0000 722b 0000 0072 2d00 0000 721b  *...r+...r-...r.
-00000770: 0000 0072 1200 0000 7212 0000 0072 1200  ...r....r....r..
-00000780: 0000 7215 0000 0072 3000 0000 2400 0000  ..r....r0...$...
-00000790: f304 0000 0008 0016 0172 3000 0000 6300  .........r0...c.
-000007a0: 0000 0000 0000 0000 0000 0000 0000 0005  ................
-000007b0: 0000 0040 0000 0073 5800 0000 6500 5a01  ...@...sX...e.Z.
-000007c0: 6400 5a02 6700 6601 6401 6503 6504 1900  d.Z.g.f.d.e.e...
-000007d0: 6602 6402 6403 8405 5a05 6404 6504 6405  f.d.d...Z.d.e.d.
-000007e0: 6504 6604 6406 6407 8404 5a06 6404 6504  e.f.d.d...Z.d.e.
-000007f0: 6405 6507 6504 1900 6604 6408 6409 8404  d.e.e...f.d.d...
-00000800: 5a08 6405 6504 6602 640a 640b 8404 5a09  Z.d.e.f.d.d...Z.
-00000810: 640c 5300 290d da04 4d6f 636b da07 616e  d.S.)...Mock..an
-00000820: 7377 6572 7363 0200 0000 0000 0000 0000  swersc..........
-00000830: 0000 0200 0000 0200 0000 4300 0000 7310  ..........C...s.
-00000840: 0000 0064 017c 005f 007c 017c 005f 0164  ...d.|._.|.|._.d
-00000850: 0053 0029 024e e9ff ffff ff29 02da 0169  .S.).N.....)...i
-00000860: 7234 0000 0029 0272 1400 0000 7234 0000  r4...).r....r4..
-00000870: 0072 1200 0000 7212 0000 0072 1500 0000  .r....r....r....
-00000880: da08 5f5f 696e 6974 5f5f 2a00 0000 7304  ..__init__*...s.
-00000890: 0000 0006 010a 017a 0d4d 6f63 6b2e 5f5f  .......z.Mock.__
-000008a0: 696e 6974 5f5f 7217 0000 0072 0e00 0000  init__r....r....
-000008b0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-000008c0: 0004 0000 0043 0000 0073 2400 0000 7c00  .....C...s$...|.
-000008d0: 0400 6a00 6401 3700 0200 5f00 7c00 6a01  ..j.d.7..._.|.j.
-000008e0: 7c00 6a00 7402 7c00 6a01 8301 1600 1900  |.j.t.|.j.......
-000008f0: 5300 2902 4ee9 0100 0000 2903 7236 0000  S.).N.....).r6..
-00000900: 0072 3400 0000 da03 6c65 6e72 1a00 0000  .r4.....lenr....
-00000910: 7212 0000 0072 1200 0000 7215 0000 0072  r....r....r....r
-00000920: 1b00 0000 2e00 0000 7304 0000 000e 0116  ........s.......
-00000930: 017a 084d 6f63 6b2e 7275 6e63 0200 0000  .z.Mock.runc....
-00000940: 0000 0000 0000 0000 0400 0000 0400 0000  ................
-00000950: 6300 0000 7344 0000 0081 007c 0004 006a  c...sD.....|...j
-00000960: 0064 0137 0002 005f 007c 006a 017c 006a  .d.7..._.|.j.|.j
-00000970: 0074 027c 006a 0183 0116 0019 007d 027c  .t.|.j.......}.|
-00000980: 0244 005d 0a7d 037c 0356 0001 0074 03a0  .D.].}.|.V...t..
-00000990: 0464 02a1 0101 0071 1564 0053 0029 034e  .d.....q.d.S.).N
-000009a0: 7238 0000 0067 9a99 9999 9999 b93f 2905  r8...g.......?).
-000009b0: 7236 0000 0072 3400 0000 7239 0000 00da  r6...r4...r9....
-000009c0: 0474 696d 65da 0573 6c65 6570 2904 7214  .time..sleep).r.
-000009d0: 0000 0072 1700 0000 da06 7265 7375 6c74  ...r......result
-000009e0: da01 6372 1200 0000 7212 0000 0072 1500  ..cr....r....r..
-000009f0: 0000 721e 0000 0032 0000 0073 0e00 0000  ..r....2...s....
-00000a00: 0280 0e01 1601 0801 0601 0c01 04fe 7a0f  ..............z.
-00000a10: 4d6f 636b 2e72 756e 5f73 7472 6561 6d63  Mock.run_streamc
-00000a20: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00000a30: 0200 0000 4300 0000 f30c 0000 0064 017c  ....C........d.|
-00000a40: 006a 009b 009d 0253 0029 024e 7a0f 4d6f  .j.....S.).Nz.Mo
-00000a50: 636b 6564 2042 6163 6b65 6e64 2029 0172  cked Backend ).r
-00000a60: 3400 0000 7213 0000 0072 1200 0000 7212  4...r....r....r.
-00000a70: 0000 0072 1500 0000 da08 5f5f 7265 7072  ...r......__repr
-00000a80: 5f5f 3900 0000 7227 0000 007a 0d4d 6f63  __9...r'...z.Moc
-00000a90: 6b2e 5f5f 7265 7072 5f5f 4e29 0a72 2900  k.__repr__N).r).
-00000aa0: 0000 722a 0000 0072 2b00 0000 7208 0000  ..r*...r+...r...
-00000ab0: 0072 2d00 0000 7237 0000 0072 1b00 0000  .r-...r7...r....
-00000ac0: 7207 0000 0072 1e00 0000 723f 0000 0072  r....r....r?...r
-00000ad0: 1200 0000 7212 0000 0072 1200 0000 7215  ....r....r....r.
-00000ae0: 0000 0072 3300 0000 2900 0000 730a 0000  ...r3...)...s...
-00000af0: 0008 0016 0112 0416 0412 0772 3300 0000  ...........r3...
-00000b00: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000b10: 0004 0000 0040 0000 0073 3600 0000 6500  .....@...s6...e.
-00000b20: 5a01 6400 5a02 640a 6403 6404 8404 5a03  Z.d.Z.d.d.d...Z.
-00000b30: 6405 6504 6401 6504 6604 6406 6407 8404  d.e.d.e.f.d.d...
-00000b40: 5a05 6401 6504 6602 6408 6409 8404 5a06  Z.d.e.f.d.d...Z.
-00000b50: 6402 5300 290b da06 476f 6f67 6c65 720e  d.S.)...Googler.
-00000b60: 0000 004e 6301 0000 0000 0000 0000 0000  ...Nc...........
-00000b70: 0001 0000 0001 0000 0043 0000 0073 0400  .........C...s..
-00000b80: 0000 6400 5300 7218 0000 0072 1200 0000  ..d.S.r....r....
-00000b90: 7213 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
-00000ba0: 1500 0000 7237 0000 003e 0000 0072 1c00  ....r7...>...r..
-00000bb0: 0000 7a0f 476f 6f67 6c65 2e5f 5f69 6e69  ..z.Google.__ini
-00000bc0: 745f 5f72 1700 0000 6302 0000 0000 0000  t__r....c.......
-00000bd0: 0000 0000 0008 0000 0007 0000 0043 0000  .............C..
-00000be0: 0073 1a01 0000 6401 6402 6c00 6d01 7d02  .s....d.d.l.m.}.
-00000bf0: 0100 7402 6a03 a004 6403 a101 7d03 7c03  ..t.j...d...}.|.
-00000c00: 7312 4a00 6404 8301 8201 7c03 7c00 5f05  s.J.d.....|.|._.
-00000c10: 7c00 6a05 6405 7c01 6406 6407 6408 6409  |.j.d.|.d.d.d.d.
-00000c20: 9c06 7d04 7c02 7c04 8301 7d05 7c05 a006  ..}.|.|...}.|...
-00000c30: a100 7d06 640a 7c06 a007 a100 7600 723f  ..}.d.|.....v.r?
-00000c40: 640b 7c06 640a 1900 a007 a100 7600 723f  d.|.d.......v.r?
-00000c50: 7c06 640a 1900 640b 1900 7d07 7408 7c07  |.d...d...}.t.|.
-00000c60: 8301 5300 640a 7c06 a007 a100 7600 7257  ..S.d.|.....v.rW
-00000c70: 640c 7c06 640a 1900 a007 a100 7600 7257  d.|.d.......v.rW
-00000c80: 7c06 640a 1900 640c 1900 7d07 7408 7c07  |.d...d...}.t.|.
-00000c90: 8301 5300 640a 7c06 a007 a100 7600 7271  ..S.d.|.....v.rq
-00000ca0: 640d 7c06 640a 1900 a007 a100 7600 7271  d.|.d.......v.rq
-00000cb0: 7c06 640a 1900 640d 1900 6401 1900 7d07  |.d...d...d...}.
-00000cc0: 7408 7c07 8301 5300 640c 7c06 640e 1900  t.|...S.d.|.d...
-00000cd0: 6401 1900 a007 a100 7600 7287 7c06 640e  d.......v.r.|.d.
-00000ce0: 1900 6401 1900 640c 1900 7d07 7408 7c07  ..d...d...}.t.|.
-00000cf0: 8301 5300 640f 7d07 7408 7c07 8301 5300  ..S.d.}.t.|...S.
-00000d00: 2910 4e72 0100 0000 2901 da0c 476f 6f67  ).Nr....)...Goog
-00000d10: 6c65 5365 6172 6368 da08 5345 5250 5f4b  leSearch..SERP_K
-00000d20: 4559 7a3f 4e65 6564 2061 2053 4552 505f  EYz?Need a SERP_
-00000d30: 4b45 592e 2047 6574 206f 6e65 2068 6572  KEY. Get one her
-00000d40: 6520 6874 7470 733a 2f2f 7365 7270 6170  e https://serpap
-00000d50: 692e 636f 6d2f 7573 6572 732f 7765 6c63  i.com/users/welc
-00000d60: 6f6d 65da 0667 6f6f 676c 657a 0a67 6f6f  ome..googlez.goo
-00000d70: 676c 652e 636f 6dda 0275 73da 0265 6e29  gle.com..us..en)
-00000d80: 06da 0761 7069 5f6b 6579 da06 656e 6769  ...api_key..engi
-00000d90: 6e65 da01 71da 0d67 6f6f 676c 655f 646f  ne..q..google_do
-00000da0: 6d61 696e da02 676c da02 686c da0a 616e  main..gl..hl..an
-00000db0: 7377 6572 5f62 6f78 da06 616e 7377 6572  swer_box..answer
-00000dc0: da07 736e 6970 7065 74da 1973 6e69 7070  ..snippet..snipp
-00000dd0: 6574 5f68 6967 686c 6967 6874 6564 5f77  et_highlighted_w
-00000de0: 6f72 6473 da0f 6f72 6761 6e69 635f 7265  ords..organic_re
-00000df0: 7375 6c74 7372 1100 0000 2909 da07 7365  sultsr....)...se
-00000e00: 7270 6170 6972 4100 0000 da02 6f73 da07  rpapirA.....os..
-00000e10: 656e 7669 726f 6eda 0367 6574 da0b 7365  environ..get..se
-00000e20: 7270 6170 695f 6b65 79da 0867 6574 5f64  rpapi_key..get_d
-00000e30: 6963 74da 046b 6579 7372 2d00 0000 2908  ict..keysr-...).
-00000e40: 7214 0000 0072 1700 0000 7241 0000 0072  r....r....rA...r
-00000e50: 5500 0000 da06 7061 7261 6d73 da06 7365  U.....params..se
-00000e60: 6172 6368 da03 7265 73da 0574 6f72 6574  arch..res..toret
-00000e70: 7212 0000 0072 1200 0000 7215 0000 0072  r....r....r....r
-00000e80: 1b00 0000 4100 0000 7342 0000 000c 010c  ....A...sB......
-00000e90: 0202 0204 ff02 0204 fe06 0304 0302 0102  ................
-00000ea0: 0102 0102 0102 0106 fa08 0908 011c 020c  ................
-00000eb0: 0108 0c1c f50c 0108 0a0a f802 ff0e 0202  ................
-00000ec0: fe10 0408 0514 fc10 0108 0304 ff08 017a  ...............z
-00000ed0: 0a47 6f6f 676c 652e 7275 6e63 0100 0000  .Google.runc....
-00000ee0: 0000 0000 0000 0000 0100 0000 0100 0000  ................
-00000ef0: 4300 0000 720f 0000 0029 024e 7a15 476f  C...r....).Nz.Go
-00000f00: 6f67 6c65 2053 6561 7263 6820 4261 636b  ogle Search Back
-00000f10: 656e 6472 1200 0000 7213 0000 0072 1200  endr....r....r..
-00000f20: 0000 7212 0000 0072 1500 0000 723f 0000  ..r....r....r?..
-00000f30: 0065 0000 0072 1c00 0000 7a0f 476f 6f67  .e...r....z.Goog
-00000f40: 6c65 2e5f 5f72 6570 725f 5f29 0272 0e00  le.__repr__).r..
-00000f50: 0000 4e29 0772 2900 0000 722a 0000 0072  ..N).r)...r*...r
-00000f60: 2b00 0000 7237 0000 0072 2d00 0000 721b  +...r7...r-...r.
-00000f70: 0000 0072 3f00 0000 7212 0000 0072 1200  ...r?...r....r..
-00000f80: 0000 7212 0000 0072 1500 0000 7240 0000  ..r....r....r@..
-00000f90: 003d 0000 0073 0800 0000 0800 0a01 1203  .=...s..........
-00000fa0: 1224 7240 0000 0063 0000 0000 0000 0000  .$r@...c........
-00000fb0: 0000 0000 0000 0000 0400 0000 4000 0000  ............@...
-00000fc0: 7350 0000 0065 005a 0164 005a 0264 015a  sP...e.Z.d.Z.d.Z
-00000fd0: 0364 0265 046a 0566 0264 0364 0484 045a  .d.e.j.f.d.d...Z
-00000fe0: 0664 0265 046a 0566 0264 0564 0684 045a  .d.e.j.f.d.d...Z
-00000ff0: 0764 0765 0864 0265 0866 0464 0864 0984  .d.e.d.e.f.d.d..
-00001000: 045a 0964 0265 0866 0264 0a64 0b84 045a  .Z.d.e.f.d.d...Z
-00001010: 0a64 0c53 0029 0dda 0650 7974 686f 6e7a  .d.S.)...Pythonz
-00001020: 3045 7865 6375 7465 7320 5079 7468 6f6e  0Executes Python
-00001030: 2063 6f6d 6d61 6e64 7320 616e 6420 7265   commands and re
-00001040: 7475 726e 7320 7468 6520 6f75 7470 7574  turns the output
-00001050: 2e72 0e00 0000 6301 0000 0000 0000 0000  .r....c.........
-00001060: 0000 0001 0000 0002 0000 0043 0000 00f3  ...........C....
-00001070: 0800 0000 7400 a001 a100 5300 7218 0000  ....t.....S.r...
-00001080: 00a9 0272 2400 0000 da04 436f 6465 7213  ...r$.....Coder.
-00001090: 0000 0072 1200 0000 7212 0000 0072 1500  ...r....r....r..
-000010a0: 0000 7226 0000 006c 0000 00f3 0200 0000  ..r&...l........
-000010b0: 0801 7a12 5079 7468 6f6e 2e62 6c6f 636b  ..z.Python.block
-000010c0: 5f69 6e70 7574 6301 0000 0000 0000 0000  _inputc.........
-000010d0: 0000 0001 0000 0002 0000 0043 0000 0072  ...........C...r
-000010e0: 5d00 0000 7218 0000 0072 5e00 0000 7213  ]...r....r^...r.
-000010f0: 0000 0072 1200 0000 7212 0000 0072 1500  ...r....r....r..
-00001100: 0000 7228 0000 006f 0000 0072 6000 0000  ..r(...o...r`...
-00001110: 7a13 5079 7468 6f6e 2e62 6c6f 636b 5f6f  z.Python.block_o
-00001120: 7574 7075 7472 1700 0000 6302 0000 0000  utputr....c.....
-00001130: 0000 0000 0000 0007 0000 0008 0000 0043  ...............C
-00001140: 0000 0073 8800 0000 6401 6402 6c00 6d01  ...s....d.d.l.m.
-00001150: 7d02 0100 6401 6403 6c02 6d03 7d03 0100  }...d.d.l.m.}...
-00001160: 7c01 a004 a100 7d04 7c04 a005 6404 a101  |.....}.|...d...
-00001170: 7223 6405 a006 7c04 a004 a100 a007 6405  r#d...|.......d.
-00001180: a101 6406 6407 8502 1900 a101 7d04 7c03  ..d.d.......}.|.
-00001190: 8300 7d05 7c02 7c05 8301 8f0c 0100 7408  ..}.|.|.......t.
-000011a0: 7c04 8301 0100 5700 6408 0400 0400 8303  |.....W.d.......
-000011b0: 0100 6e08 3100 7339 7701 0100 0100 0100  ..n.1.s9w.......
-000011c0: 5900 0100 7c05 a009 a100 7d06 7c06 5300  Y...|.....}.|.S.
-000011d0: 2909 fa25 5275 6e20 636f 6d6d 616e 6473  )..%Run commands
-000011e0: 2061 6e64 2072 6574 7572 6e20 6669 6e61   and return fina
-000011f0: 6c20 6f75 7470 7574 2e72 0100 0000 2901  l output.r....).
-00001200: da0f 7265 6469 7265 6374 5f73 7464 6f75  ..redirect_stdou
-00001210: 7429 01da 0853 7472 696e 6749 4f7a 0360  t)...StringIOz.`
-00001220: 6060 da01 0a72 3800 0000 7235 0000 004e  ``...r8...r5...N
-00001230: 290a da0a 636f 6e74 6578 746c 6962 7262  )...contextlibrb
-00001240: 0000 00da 0269 6f72 6300 0000 da05 7374  .....iorc.....st
-00001250: 7269 70da 0a73 7461 7274 7377 6974 68da  rip..startswith.
-00001260: 046a 6f69 6eda 0573 706c 6974 da04 6578  .join..split..ex
-00001270: 6563 da08 6765 7476 616c 7565 2907 7214  ec..getvalue).r.
-00001280: 0000 0072 1700 0000 7262 0000 0072 6300  ...r....rb...rc.
-00001290: 0000 da01 70da 0166 da01 7372 1200 0000  ....p..f..sr....
-000012a0: 7212 0000 0072 1500 0000 721b 0000 0072  r....r....r....r
-000012b0: 0000 0073 1600 0000 0c02 0c01 0802 0a01  ...s............
-000012c0: 1c01 0602 0a01 0a01 1cff 0802 0401 7a0a  ..............z.
-000012d0: 5079 7468 6f6e 2e72 756e 6301 0000 0000  Python.runc.....
-000012e0: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
-000012f0: 0000 0072 0f00 0000 2902 4e7a 0e50 7974  ...r....).Nz.Pyt
-00001300: 686f 6e2d 4261 636b 656e 6472 1200 0000  hon-Backendr....
-00001310: 7213 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
-00001320: 1500 0000 723f 0000 0081 0000 0072 1c00  ....r?.......r..
-00001330: 0000 7a0f 5079 7468 6f6e 2e5f 5f72 6570  ..z.Python.__rep
-00001340: 725f 5f4e 290b 7229 0000 0072 2a00 0000  r__N).r)...r*...
-00001350: 722b 0000 00da 075f 5f64 6f63 5f5f 7224  r+.....__doc__r$
-00001360: 0000 0072 2e00 0000 7226 0000 0072 2800  ...r....r&...r(.
-00001370: 0000 722d 0000 0072 1b00 0000 723f 0000  ..r-...r....r?..
-00001380: 0072 1200 0000 7212 0000 0072 1200 0000  .r....r....r....
-00001390: 7215 0000 0072 5c00 0000 6900 0000 730c  r....r\...i...s.
-000013a0: 0000 0008 0004 0110 0210 0312 0312 0f72  ...............r
-000013b0: 5c00 0000 6300 0000 0000 0000 0000 0000  \...c...........
-000013c0: 0000 0000 0005 0000 0040 0000 0073 6400  .........@...sd.
-000013d0: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
-000013e0: 6504 6a05 6602 6403 6404 8404 5a06 6402  e.j.f.d.d...Z.d.
-000013f0: 6504 6a05 6602 6405 6406 8404 5a07 6412  e.j.f.d.d...Z.d.
-00001400: 6408 6508 6409 6508 6604 640a 640b 8405  d.e.d.e.f.d.d...
-00001410: 5a09 640c 650a 6402 650a 6604 640d 640e  Z.d.e.d.e.f.d.d.
-00001420: 8404 5a0b 6402 650a 6602 640f 6410 8404  ..Z.d.e.f.d.d...
-00001430: 5a0c 6411 5300 2913 da04 4261 7368 7a2e  Z.d.S.)...Bashz.
-00001440: 4578 6563 7574 6573 2062 6173 6820 636f  Executes bash co
-00001450: 6d6d 616e 6473 2061 6e64 2072 6574 7572  mmands and retur
-00001460: 6e73 2074 6865 206f 7574 7075 742e 720e  ns the output.r.
-00001470: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00001480: 0100 0000 0200 0000 4300 0000 725d 0000  ........C...r]..
-00001490: 0072 1800 0000 725e 0000 0072 1300 0000  .r....r^...r....
-000014a0: 7212 0000 0072 1200 0000 7215 0000 0072  r....r....r....r
-000014b0: 2600 0000 8800 0000 7260 0000 007a 1042  &.......r`...z.B
-000014c0: 6173 682e 626c 6f63 6b5f 696e 7075 7463  ash.block_inputc
-000014d0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-000014e0: 0200 0000 4300 0000 725d 0000 0072 1800  ....C...r]...r..
-000014f0: 0000 725e 0000 0072 1300 0000 7212 0000  ..r^...r....r...
-00001500: 0072 1200 0000 7215 0000 0072 2800 0000  .r....r....r(...
-00001510: 8b00 0000 7260 0000 007a 1142 6173 682e  ....r`...z.Bash.
-00001520: 626c 6f63 6b5f 6f75 7470 7574 46da 0e73  block_outputF..s
-00001530: 7472 6970 5f6e 6577 6c69 6e65 73da 1172  trip_newlines..r
-00001540: 6574 7572 6e5f 6572 725f 6f75 7470 7574  eturn_err_output
-00001550: 6303 0000 0000 0000 0000 0000 0003 0000  c...............
-00001560: 0002 0000 0043 0000 0073 1000 0000 7c01  .....C...s....|.
-00001570: 7c00 5f00 7c02 7c00 5f01 6401 5300 2902  |._.|.|._.d.S.).
-00001580: 7a23 496e 6974 6961 6c69 7a65 2077 6974  z#Initialize wit
-00001590: 6820 7374 7269 7070 696e 6720 6e65 776c  h stripping newl
-000015a0: 696e 6573 2e4e 2902 7272 0000 0072 7300  ines.N).rr...rs.
-000015b0: 0000 2903 7214 0000 0072 7200 0000 7273  ..).r....rr...rs
-000015c0: 0000 0072 1200 0000 7212 0000 0072 1500  ...r....r....r..
-000015d0: 0000 7237 0000 008e 0000 0073 0400 0000  ..r7.......s....
-000015e0: 0602 0a01 7a0d 4261 7368 2e5f 5f69 6e69  ....z.Bash.__ini
-000015f0: 745f 5f72 1700 0000 6302 0000 0000 0000  t__r....c.......
-00001600: 0000 0000 0004 0000 000a 0000 0043 0000  .............C..
-00001610: 0073 8400 0000 7a11 7400 6a01 7c01 6401  .s....z.t.j.|.d.
-00001620: 6401 7400 6a02 7400 6a03 6402 8d05 6a04  d.t.j.t.j.d...j.
-00001630: a005 a100 7d02 5700 6e27 0400 7400 6a06  ....}.W.n'..t.j.
-00001640: 7938 0100 7d03 0100 7a1a 7c00 6a07 722a  y8..}...z.|.j.r*
-00001650: 7408 7c03 6a04 a005 a100 8301 5700 0600  t.|.j.......W...
-00001660: 5900 6403 7d03 7e03 5300 7408 7c03 8301  Y.d.}.~.S.t.|...
-00001670: 5700 0600 5900 6403 7d03 7e03 5300 6403  W...Y.d.}.~.S.d.
-00001680: 7d03 7e03 7701 7700 7c00 6a09 7240 7c02  }.~.w.w.|.j.r@|.
-00001690: a00a a100 7d02 7c02 5300 2904 7261 0000  ....}.|.S.).ra..
-000016a0: 0054 2904 da05 7368 656c 6cda 0563 6865  .T)...shell..che
-000016b0: 636b da06 7374 646f 7574 da06 7374 6465  ck..stdout..stde
-000016c0: 7272 4e29 0bda 0a73 7562 7072 6f63 6573  rrN)...subproces
-000016d0: 7372 1b00 0000 da04 5049 5045 da06 5354  sr......PIPE..ST
-000016e0: 444f 5554 7276 0000 00da 0664 6563 6f64  DOUTrv.....decod
-000016f0: 65da 1243 616c 6c65 6450 726f 6365 7373  e..CalledProcess
-00001700: 4572 726f 7272 7300 0000 722d 0000 0072  Errorrs...r-...r
-00001710: 7200 0000 7267 0000 0029 0472 1400 0000  r...rg...).r....
-00001720: 7217 0000 00da 066f 7574 7075 74da 0565  r......output..e
-00001730: 7272 6f72 7212 0000 0072 1200 0000 7215  rrorr....r....r.
-00001740: 0000 0072 1b00 0000 9300 0000 7326 0000  ...r........s&..
-00001750: 0002 0204 0102 0102 0102 0104 0104 0104  ................
-00001760: fb06 0606 fa10 0706 011a 0114 0108 8002  ................
-00001770: fd06 0408 0104 017a 0842 6173 682e 7275  .......z.Bash.ru
-00001780: 6e63 0100 0000 0000 0000 0000 0000 0100  nc..............
-00001790: 0000 0100 0000 4300 0000 720f 0000 0029  ......C...r....)
-000017a0: 024e 7a0c 4261 7368 2d42 6163 6b65 6e64  .Nz.Bash-Backend
-000017b0: 7212 0000 0072 1300 0000 7212 0000 0072  r....r....r....r
-000017c0: 1200 0000 7215 0000 0072 3f00 0000 a500  ....r....r?.....
-000017d0: 0000 721c 0000 007a 0d42 6173 682e 5f5f  ..r....z.Bash.__
-000017e0: 7265 7072 5f5f 4e29 0246 4629 0d72 2900  repr__N).FF).r).
-000017f0: 0000 722a 0000 0072 2b00 0000 7270 0000  ..r*...r+...rp..
-00001800: 0072 2400 0000 722e 0000 0072 2600 0000  .r$...r....r&...
-00001810: 7228 0000 00da 0462 6f6f 6c72 3700 0000  r(.....boolr7...
-00001820: 722d 0000 0072 1b00 0000 723f 0000 0072  r-...r....r?...r
-00001830: 1200 0000 7212 0000 0072 1200 0000 7215  ....r....r....r.
-00001840: 0000 0072 7100 0000 8500 0000 730e 0000  ...rq.......s...
-00001850: 0008 0004 0110 0210 0314 0312 0512 1272  ...............r
-00001860: 7100 0000 6300 0000 0000 0000 0000 0000  q...c...........
-00001870: 0000 0000 000b 0000 0040 0000 0073 4a00  .........@...sJ.
-00001880: 0000 6500 5a01 6400 5a02 0901 0902 0903  ..e.Z.d.Z.......
-00001890: 0904 640e 6405 6503 6406 6504 6407 6505  ..d.d.e.d.e.d.e.
-000018a0: 6408 6506 6507 6503 1900 1900 6409 6404  d.e.e.e.....d.d.
-000018b0: 660a 640a 640b 8405 5a08 6409 6503 6602  f.d.d...Z.d.e.f.
-000018c0: 640c 640d 8404 5a09 6404 5300 290f da0a  d.d...Z.d.S.)...
-000018d0: 4f70 656e 4149 4261 7365 fa0d 6770 742d  OpenAIBase..gpt-
-000018e0: 332e 352d 7475 7262 6fe9 0001 0000 e700  3.5-turbo.......
-000018f0: 0000 0000 0000 004e da05 6d6f 6465 6cda  .......N..model.
-00001900: 0a6d 6178 5f74 6f6b 656e 73da 0b74 656d  .max_tokens..tem
-00001910: 7065 7261 7475 7265 da04 7374 6f70 720e  perature..stopr.
-00001920: 0000 0063 0500 0000 0000 0000 0000 0000  ...c............
-00001930: 0500 0000 0500 0000 4300 0000 7320 0000  ........C...s ..
-00001940: 007c 017c 005f 007c 047c 005f 0174 027c  .|.|._.|.|._.t.|
-00001950: 017c 027c 0364 018d 037c 005f 0364 0053  .|.|.d...|._.d.S
-00001960: 0029 024e 2903 7284 0000 0072 8500 0000  .).N).r....r....
-00001970: 7286 0000 0029 0472 8400 0000 7287 0000  r....).r....r...
-00001980: 00da 0464 6963 74da 076f 7074 696f 6e73  ...dict..options
-00001990: 2905 7214 0000 0072 8400 0000 7285 0000  ).r....r....r...
-000019a0: 0072 8600 0000 7287 0000 0072 1200 0000  .r....r....r....
-000019b0: 7212 0000 0072 1500 0000 7237 0000 00aa  r....r....r7....
-000019c0: 0000 0073 0e00 0000 0607 0601 0201 0201  ...s............
-000019d0: 0201 0201 0cfd 7a13 4f70 656e 4149 4261  ......z.OpenAIBa
-000019e0: 7365 2e5f 5f69 6e69 745f 5f63 0100 0000  se.__init__c....
-000019f0: 0000 0000 0000 0000 0100 0000 0200 0000  ................
-00001a00: 4300 0000 723e 0000 0029 024e 7a0f 4f70  C...r>...).Nz.Op
-00001a10: 656e 4149 2042 6163 6b65 6e64 2029 0172  enAI Backend ).r
-00001a20: 8900 0000 7213 0000 0072 1200 0000 7212  ....r....r....r.
-00001a30: 0000 0072 1500 0000 723f 0000 00b9 0000  ...r....r?......
-00001a40: 0072 2700 0000 7a13 4f70 656e 4149 4261  .r'...z.OpenAIBa
-00001a50: 7365 2e5f 5f72 6570 725f 5f29 0472 8100  se.__repr__).r..
-00001a60: 0000 7282 0000 0072 8300 0000 4e29 0a72  ..r....r....N).r
-00001a70: 2900 0000 722a 0000 0072 2b00 0000 722d  )...r*...r+...r-
-00001a80: 0000 00da 0369 6e74 da05 666c 6f61 7472  .....int..floatr
-00001a90: 0900 0000 7208 0000 0072 3700 0000 723f  ....r....r7...r?
-00001aa0: 0000 0072 1200 0000 7212 0000 0072 1200  ...r....r....r..
-00001ab0: 0000 7215 0000 0072 8000 0000 a900 0000  ..r....r........
-00001ac0: 7322 0000 0008 0002 0302 0102 0102 0104  s"..............
-00001ad0: fb02 0202 fe02 0302 fd02 0402 fc0a 0502  ................
-00001ae0: fb02 060a fa12 0f72 8000 0000 6300 0000  .......r....c...
-00001af0: 0000 0000 0000 0000 0000 0000 0005 0000  ................
-00001b00: 0040 0000 0073 3400 0000 6500 5a01 6400  .@...s4...e.Z.d.
-00001b10: 5a02 6401 6503 6402 6503 6604 6403 6404  Z.d.e.d.e.f.d.d.
-00001b20: 8404 5a04 6405 6503 6402 6505 6503 1900  ..Z.d.e.d.e.e...
-00001b30: 6604 6406 6407 8404 5a06 6408 5300 2909  f.d.d...Z.d.S.).
-00001b40: da06 4f70 656e 4149 7217 0000 0072 0e00  ..OpenAIr....r..
-00001b50: 0000 6302 0000 0000 0000 0000 0000 0005  ..c.............
-00001b60: 0000 0006 0000 0043 0000 0073 5200 0000  .......C...sR...
-00001b70: 6401 6400 6c00 7d02 6402 6403 6802 7d03  d.d.l.}.d.d.h.}.
-00001b80: 7c02 6a01 7c00 6a02 7c03 7600 7211 6404  |.j.|.j.|.v.r.d.
-00001b90: 6e01 6405 7c00 6a03 6406 1900 6407 7404  n.d.|.j.d...d.t.
-00001ba0: 6a05 9b00 6408 8d04 7d02 7c02 6a06 7c01  j...d...}.|.j.|.
-00001bb0: 7c00 6a07 6409 8d02 7d04 7408 7c04 8301  |.j.d...}.t.|...
-00001bc0: 5300 290a 4e72 0100 0000 7a05 6770 742d  S.).Nr....z.gpt-
-00001bd0: 3472 8100 0000 da0a 6f70 656e 6169 6368  4r......openaich
-00001be0: 6174 da06 6f70 656e 6169 7285 0000 00da  at..openair.....
-00001bf0: 0673 716c 6974 6529 04da 0b63 6c69 656e  .sqlite)...clien
-00001c00: 745f 6e61 6d65 7285 0000 00da 0a63 6163  t_namer......cac
-00001c10: 6865 5f6e 616d 65da 1063 6163 6865 5f63  he_name..cache_c
-00001c20: 6f6e 6e65 6374 696f 6e29 01da 0e73 746f  onnection)...sto
-00001c30: 705f 7365 7175 656e 6365 7329 09da 086d  p_sequences)...m
-00001c40: 616e 6966 6573 74da 084d 616e 6966 6573  anifest..Manifes
-00001c50: 7472 8400 0000 7289 0000 00da 104d 696e  tr....r......Min
-00001c60: 6963 6861 696e 436f 6e74 6578 74da 046e  ichainContext..n
-00001c70: 616d 6572 1b00 0000 7287 0000 0072 2d00  amer....r....r-.
-00001c80: 0000 2905 7214 0000 0072 1700 0000 7294  ..).r....r....r.
-00001c90: 0000 00da 0463 6861 74da 0361 6e73 7212  .....chat..ansr.
-00001ca0: 0000 0072 1200 0000 7215 0000 0072 1b00  ...r....r....r..
-00001cb0: 0000 be00 0000 731a 0000 0008 0108 0204  ......s.........
-00001cc0: 0110 0108 0102 0106 0106 fc04 0702 0104  ................
-00001cd0: 0106 fe08 047a 0a4f 7065 6e41 492e 7275  .....z.OpenAI.ru
-00001ce0: 6eda 0670 726f 6d70 7463 0200 0000 0000  n..promptc......
-00001cf0: 0000 0000 0000 0500 0000 0600 0000 6300  ..............c.
-00001d00: 0000 7380 0000 0081 0064 0164 006c 007d  ..s......d.d.l.}
-00001d10: 0274 016a 02a0 0364 02a1 017c 005f 047c  .t.j...d...|._.|
-00001d20: 006a 0473 134a 0064 0383 0182 017c 006a  .j.s.J.d.....|.j
-00001d30: 047c 025f 047c 026a 056a 067c 006a 0764  .|._.|.j.j.|.j.d
-00001d40: 047c 0164 059c 0267 0164 067c 006a 0864  .|.d...g.d.|.j.d
-00001d50: 078d 0444 005d 167d 037c 0364 0819 0064  ...D.].}.|.d...d
-00001d60: 0119 00a0 0364 0969 00a1 02a0 0364 0aa1  .....d.i.....d..
-00001d70: 017d 047c 0464 0075 0172 3d7c 0456 0001  .}.|.d.u.r=|.V..
-00001d80: 0071 2764 0053 0029 0b4e 7201 0000 00da  .q'd.S.).Nr.....
-00001d90: 0e4f 5045 4e41 495f 4150 495f 4b45 59fa  .OPENAI_API_KEY.
-00001da0: 3c4e 6565 6420 616e 204f 5045 4e41 495f  <Need an OPENAI_
-00001db0: 4150 495f 4b45 592e 2047 6574 206f 6e65  API_KEY. Get one
-00001dc0: 2068 6572 6520 6874 7470 733a 2f2f 6f70   here https://op
-00001dd0: 656e 6169 2e63 6f6d 2f61 7069 2fda 0475  enai.com/api/..u
-00001de0: 7365 7229 02da 0472 6f6c 65da 0763 6f6e  ser)...role..con
-00001df0: 7465 6e74 5429 0472 8400 0000 da08 6d65  tentT).r......me
-00001e00: 7373 6167 6573 da06 7374 7265 616d 7287  ssages..streamr.
-00001e10: 0000 00da 0763 686f 6963 6573 da05 6465  .....choices..de
-00001e20: 6c74 6172 9f00 0000 2909 728e 0000 0072  ltar....).r....r
-00001e30: 5200 0000 7253 0000 0072 5400 0000 7246  R...rS...rT...rF
-00001e40: 0000 00da 0e43 6861 7443 6f6d 706c 6574  .....ChatComplet
-00001e50: 696f 6eda 0663 7265 6174 6572 8400 0000  ion..creater....
-00001e60: 7287 0000 0029 0572 1400 0000 729a 0000  r....).r....r...
-00001e70: 0072 8e00 0000 da05 6368 756e 6b72 9f00  .r......chunkr..
-00001e80: 0000 7212 0000 0072 1200 0000 7215 0000  ..r....r....r...
-00001e90: 0072 1e00 0000 cf00 0000 7326 0000 0002  .r........s&....
-00001ea0: 8008 010e 0204 0204 ff02 0204 fe08 0306  ................
-00001eb0: 0204 010a 0102 0104 010a fc1a 0608 0106  ................
-00001ec0: 0102 8004 f87a 114f 7065 6e41 492e 7275  .....z.OpenAI.ru
-00001ed0: 6e5f 7374 7265 616d 4e29 0772 2900 0000  n_streamN).r)...
-00001ee0: 722a 0000 0072 2b00 0000 722d 0000 0072  r*...r+...r-...r
-00001ef0: 1b00 0000 7207 0000 0072 1e00 0000 7212  ....r....r....r.
-00001f00: 0000 0072 1200 0000 7212 0000 0072 1500  ...r....r....r..
-00001f10: 0000 728c 0000 00bd 0000 0073 0600 0000  ..r........s....
-00001f20: 0800 1201 1a11 728c 0000 0063 0000 0000  ......r....c....
-00001f30: 0000 0000 0000 0000 0000 0000 0700 0000  ................
-00001f40: 0000 0000 734e 0000 0065 005a 0164 005a  ....sN...e.Z.d.Z
-00001f50: 0264 0165 036a 0466 0264 0264 0384 045a  .d.e.j.f.d.d...Z
-00001f60: 0564 0d64 0565 0664 0665 0764 0164 0766  .d.d.e.d.e.d.d.f
-00001f70: 0687 0066 0164 0864 0984 0d5a 0864 0a65  ...f.d.d...Z.d.e
-00001f80: 0664 0165 0666 0464 0b64 0c84 045a 0987  .d.e.f.d.d...Z..
-00001f90: 0004 005a 0a53 0029 0eda 0b4f 7065 6e41  ...Z.S.)...OpenA
-00001fa0: 4945 6d62 6564 720e 0000 0063 0100 0000  IEmbedr....c....
-00001fb0: 0000 0000 0000 0000 0100 0000 0300 0000  ................
-00001fc0: 4300 0000 7220 0000 0029 034e da09 456d  C...r ...).N..Em
-00001fd0: 6265 6464 696e 6729 01da 056c 6162 656c  bedding)...label
-00001fe0: 7223 0000 0072 1300 0000 7212 0000 0072  r#...r....r....r
-00001ff0: 1200 0000 7215 0000 0072 2800 0000 e400  ....r....r(.....
-00002000: 0000 7227 0000 007a 184f 7065 6e41 4945  ..r'...z.OpenAIE
-00002010: 6d62 6564 2e62 6c6f 636b 5f6f 7574 7075  mbed.block_outpu
-00002020: 74fa 1674 6578 742d 656d 6265 6464 696e  t..text-embeddin
-00002030: 672d 6164 612d 3030 3272 8400 0000 da06  g-ada-002r......
-00002040: 6b77 6172 6773 4e63 0200 0000 0000 0000  kwargsNc........
-00002050: 0000 0000 0300 0000 0400 0000 0b00 0000  ................
-00002060: 7318 0000 0074 0083 006a 017c 0166 0169  s....t...j.|.f.i
-00002070: 007c 02a4 018e 0101 0064 0053 0072 1800  .|.......d.S.r..
-00002080: 0000 2902 da05 7375 7065 7272 3700 0000  ..)...superr7...
-00002090: 2903 7214 0000 0072 8400 0000 72ab 0000  ).r....r....r...
-000020a0: 00a9 01da 095f 5f63 6c61 7373 5f5f 7212  .....__class__r.
-000020b0: 0000 0072 1500 0000 7237 0000 00e7 0000  ...r....r7......
-000020c0: 00f3 0200 0000 1801 7a14 4f70 656e 4149  ........z.OpenAI
-000020d0: 456d 6265 642e 5f5f 696e 6974 5f5f 7217  Embed.__init__r.
-000020e0: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-000020f0: 0400 0000 0400 0000 4300 0000 734e 0000  ........C...sN..
-00002100: 0064 0164 006c 007d 0274 016a 02a0 0364  .d.d.l.}.t.j...d
-00002110: 02a1 017c 005f 047c 006a 0473 124a 0064  ...|._.|.j.s.J.d
-00002120: 0383 0182 017c 006a 047c 025f 047c 026a  .....|.j.|._.|.j
-00002130: 056a 067c 006a 077c 0164 048d 027d 037c  .j.|.j.|.d...}.|
-00002140: 0364 0519 0064 0119 0064 0619 0053 0029  .d...d...d...S.)
-00002150: 074e 7201 0000 0072 9b00 0000 729c 0000  .Nr....r....r...
-00002160: 0029 0272 4700 0000 da05 696e 7075 74da  .).rG.....input.
-00002170: 0464 6174 61da 0965 6d62 6564 6469 6e67  .data..embedding
-00002180: 2908 728e 0000 0072 5200 0000 7253 0000  ).r....rR...rS..
-00002190: 0072 5400 0000 7246 0000 0072 a800 0000  .rT...rF...r....
-000021a0: 72a5 0000 0072 8400 0000 2904 7214 0000  r....r....).r...
-000021b0: 0072 1700 0000 728e 0000 0072 9900 0000  .r....r....r....
-000021c0: 7212 0000 0072 1200 0000 7215 0000 0072  r....r....r....r
-000021d0: 1b00 0000 ea00 0000 7318 0000 0008 010e  ........s.......
-000021e0: 0204 0204 ff02 0204 fe08 0306 0204 0102  ................
-000021f0: 0106 fe10 047a 0f4f 7065 6e41 4945 6d62  .....z.OpenAIEmb
-00002200: 6564 2e72 756e 2901 72aa 0000 0029 0b72  ed.run).r....).r
-00002210: 2900 0000 722a 0000 0072 2b00 0000 7224  )...r*...r+...r$
-00002220: 0000 0072 2e00 0000 7228 0000 0072 2d00  ...r....r(...r-.
-00002230: 0000 7205 0000 0072 3700 0000 721b 0000  ..r....r7...r...
-00002240: 00da 0d5f 5f63 6c61 7373 6365 6c6c 5f5f  ...__classcell__
-00002250: 7212 0000 0072 1200 0000 72ad 0000 0072  r....r....r....r
-00002260: 1500 0000 72a7 0000 00e3 0000 0073 0800  ....r........s..
-00002270: 0000 0800 1001 1c03 1a03 72a7 0000 0063  ..........r....c
-00002280: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002290: 0500 0000 4000 0000 7320 0000 0065 005a  ....@...s ...e.Z
-000022a0: 0164 005a 0264 0764 0265 0364 0364 0466  .d.Z.d.d.e.d.d.f
-000022b0: 0464 0564 0684 055a 0464 0453 0029 08da  .d.d...Z.d.S.)..
-000022c0: 0f48 7567 6769 6e67 4661 6365 4261 7365  .HuggingFaceBase
-000022d0: da04 6770 7432 7284 0000 0072 0e00 0000  ..gpt2r....r....
-000022e0: 4e63 0200 0000 0000 0000 0000 0000 0200  Nc..............
-000022f0: 0000 0200 0000 4300 0000 730a 0000 007c  ......C...s....|
-00002300: 017c 005f 0064 0053 0072 1800 0000 2901  .|._.d.S.r....).
-00002310: 7284 0000 0029 0272 1400 0000 7284 0000  r....).r....r...
-00002320: 0072 1200 0000 7212 0000 0072 1500 0000  .r....r....r....
-00002330: 7237 0000 00fb 0000 0073 0200 0000 0a01  r7.......s......
-00002340: 7a18 4875 6767 696e 6746 6163 6542 6173  z.HuggingFaceBas
-00002350: 652e 5f5f 696e 6974 5f5f 2901 72b5 0000  e.__init__).r...
-00002360: 0029 0572 2900 0000 722a 0000 0072 2b00  .).r)...r*...r+.
-00002370: 0000 722d 0000 0072 3700 0000 7212 0000  ..r-...r7...r...
-00002380: 0072 1200 0000 7212 0000 0072 1500 0000  .r....r....r....
-00002390: 72b4 0000 00fa 0000 0073 0400 0000 0800  r........s......
-000023a0: 1801 72b4 0000 0063 0000 0000 0000 0000  ..r....c........
-000023b0: 0000 0000 0000 0000 0400 0000 4000 0000  ............@...
-000023c0: 722f 0000 0029 06da 0b48 7567 6769 6e67  r/...)...Hugging
-000023d0: 4661 6365 7217 0000 0072 0e00 0000 6302  Facer....r....c.
-000023e0: 0000 0000 0000 0000 0000 0004 0000 0005  ................
-000023f0: 0000 0043 0000 00f3 4c00 0000 6401 6402  ...C....L...d.d.
-00002400: 6c00 6d01 7d02 0100 7402 6a03 a004 6403  l.m.}...t.j...d.
-00002410: a101 7c00 5f05 7c00 6a05 7314 4a00 6404  ..|._.|.j.s.J.d.
-00002420: 8301 8201 7c02 7c00 6a05 7c00 6a06 6405  ....|.|.j.|.j.d.
-00002430: 6406 8d03 7c00 5f07 7c00 6a07 7c01 6407  d...|._.|.j.|.d.
-00002440: 8d01 7d03 7c03 5300 2908 4e72 0100 0000  ..}.|.S.).Nr....
-00002450: a901 da0c 496e 6665 7265 6e63 6541 7069  ....InferenceApi
-00002460: da06 4846 5f4b 4559 fa34 4e65 6564 2061  ..HF_KEY.4Need a
-00002470: 6e20 4846 5f4b 4559 2e20 4765 7420 6f6e  n HF_KEY. Get on
-00002480: 6520 6865 7265 2068 7474 7073 3a2f 2f68  e here https://h
-00002490: 7567 6769 6e67 6661 6365 2e63 6f2f 7a0f  uggingface.co/z.
-000024a0: 7465 7874 2d67 656e 6572 6174 696f 6ea9  text-generation.
-000024b0: 03da 0574 6f6b 656e da07 7265 706f 5f69  ...token..repo_i
-000024c0: 64da 0474 6173 6ba9 01da 0669 6e70 7574  d..task....input
-000024d0: 73a9 08da 1d68 7567 6769 6e67 6661 6365  s....huggingface
-000024e0: 5f68 7562 2e69 6e66 6572 656e 6365 5f61  _hub.inference_a
-000024f0: 7069 72b9 0000 0072 5200 0000 7253 0000  pir....rR...rS..
-00002500: 0072 5400 0000 7246 0000 0072 8400 0000  .rT...rF...r....
-00002510: da06 636c 6965 6e74 a904 7214 0000 0072  ..client..r....r
-00002520: 1700 0000 72b9 0000 00da 0872 6573 706f  ....r......respo
-00002530: 6e73 6572 1200 0000 7212 0000 0072 1500  nser....r....r..
-00002540: 0000 721b 0000 0000 0100 00f3 1000 0000  ..r.............
-00002550: 0c02 0e02 0e01 0202 0a01 08ff 0c03 0401  ................
-00002560: 7a0f 4875 6767 696e 6746 6163 652e 7275  z.HuggingFace.ru
-00002570: 6e4e 7231 0000 0072 1200 0000 7212 0000  nNr1...r....r...
-00002580: 0072 1200 0000 7215 0000 0072 b600 0000  .r....r....r....
-00002590: ff00 0000 7232 0000 0072 b600 0000 6300  ....r2...r....c.
-000025a0: 0000 0000 0000 0000 0000 0000 0000 0004  ................
-000025b0: 0000 0040 0000 0072 2f00 0000 2906 da10  ...@...r/...)...
-000025c0: 4875 6767 696e 6746 6163 6545 6d62 6564  HuggingFaceEmbed
-000025d0: 7217 0000 0072 0e00 0000 6302 0000 0000  r....r....c.....
-000025e0: 0000 0000 0000 0004 0000 0005 0000 0043  ...............C
-000025f0: 0000 0072 b700 0000 2908 4e72 0100 0000  ...r....).Nr....
-00002600: 72b8 0000 0072 ba00 0000 72bb 0000 007a  r....r....r....z
-00002610: 1266 6561 7475 7265 2d65 7874 7261 6374  .feature-extract
-00002620: 696f 6e72 bc00 0000 72c0 0000 0072 c200  ionr....r....r..
-00002630: 0000 72c5 0000 0072 1200 0000 7212 0000  ..r....r....r...
-00002640: 0072 1500 0000 721b 0000 000f 0100 0072  .r....r........r
-00002650: c700 0000 7a14 4875 6767 696e 6746 6163  ....z.HuggingFac
-00002660: 6545 6d62 6564 2e72 756e 4e72 3100 0000  eEmbed.runNr1...
-00002670: 7212 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
-00002680: 1500 0000 72c8 0000 000e 0100 0072 3200  ....r........r2.
-00002690: 0000 72c8 0000 0063 0000 0000 0000 0000  ..r....c........
-000026a0: 0000 0000 0000 0000 0400 0000 4000 0000  ............@...
-000026b0: 7328 0000 0065 005a 0164 005a 0264 0a64  s(...e.Z.d.Z.d.d
-000026c0: 0564 0684 045a 0364 0765 0464 0365 0466  .d...Z.d.e.d.e.f
-000026d0: 0464 0864 0984 045a 0564 0453 0029 0b72  .d.d...Z.d.S.).r
-000026e0: 9500 0000 72c4 0000 00fa 116d 616e 6966  ....r......manif
-000026f0: 6573 742e 4d61 6e69 6665 7374 720e 0000  est.Manifestr...
-00002700: 004e 6302 0000 0000 0000 0000 0000 0002  .Nc.............
-00002710: 0000 0002 0000 0043 0000 0073 0a00 0000  .......C...s....
-00002720: 7c01 7c00 5f00 6401 5300 2902 7a44 436c  |.|._.d.S.).zDCl
-00002730: 6965 6e74 2066 726f 6d20 5b4d 616e 6966  ient from [Manif
-00002740: 6573 742d 4d4c 5d28 6874 7470 733a 2f2f  est-ML](https://
-00002750: 6769 7468 7562 2e63 6f6d 2f48 617a 7952  github.com/HazyR
-00002760: 6573 6561 7263 682f 6d61 6e69 6665 7374  esearch/manifest
-00002770: 292e 4e29 0172 c400 0000 2902 7214 0000  ).N).r....).r...
-00002780: 0072 c400 0000 7212 0000 0072 1200 0000  .r....r....r....
-00002790: 7215 0000 0072 3700 0000 1e01 0000 7302  r....r7.......s.
-000027a0: 0000 000a 027a 114d 616e 6966 6573 742e  .....z.Manifest.
-000027b0: 5f5f 696e 6974 5f5f 7217 0000 0063 0200  __init__r....c..
-000027c0: 0000 0000 0000 0000 0000 0300 0000 0800  ................
-000027d0: 0000 4300 0000 7346 0000 007a 0664 0164  ..C...sF...z.d.d
-000027e0: 006c 007d 0257 006e 0b04 0074 0179 1101  .l.}.W.n...t.y..
-000027f0: 0001 0001 0074 0164 0283 0182 0177 0074  .....t.d.....w.t
-00002800: 027c 006a 037c 026a 0483 0273 1d4a 0064  .|.j.|.j...s.J.d
-00002810: 0383 0182 017c 006a 03a0 057c 01a1 0153  .....|.j...|...S
-00002820: 0029 044e 7201 0000 007a 3660 7069 7020  .).Nr....z6`pip 
-00002830: 696e 7374 616c 6c20 6d61 6e69 6665 7374  install manifest
-00002840: 2d6d 6c60 2074 6f20 7573 6520 7468 6520  -ml` to use the 
-00002850: 4d61 6e69 6665 7374 2042 6163 6b65 6e64  Manifest Backend
-00002860: 2e7a 2e43 6c69 656e 7420 6d75 7374 2062  .z.Client must b
-00002870: 6520 6120 606d 616e 6966 6573 742e 4d61  e a `manifest.Ma
-00002880: 6e69 6665 7374 6020 696e 7374 616e 6365  nifest` instance
-00002890: 2e29 0672 9400 0000 da0b 496d 706f 7274  .).r......Import
-000028a0: 4572 726f 72da 0a69 7369 6e73 7461 6e63  Error..isinstanc
-000028b0: 6572 c400 0000 7295 0000 0072 1b00 0000  er....r....r....
-000028c0: 2903 7214 0000 0072 1700 0000 7294 0000  ).r....r....r...
-000028d0: 0072 1200 0000 7212 0000 0072 1500 0000  .r....r....r....
-000028e0: 721b 0000 0022 0100 0073 1600 0000 0201  r...."...s......
-000028f0: 0c01 0c01 0801 02ff 0202 0801 06ff 0202  ................
-00002900: 04fe 0c04 7a0c 4d61 6e69 6665 7374 2e72  ....z.Manifest.r
-00002910: 756e 2904 72c4 0000 0072 c900 0000 720e  un).r....r....r.
-00002920: 0000 004e 2906 7229 0000 0072 2a00 0000  ...N).r)...r*...
-00002930: 722b 0000 0072 3700 0000 722d 0000 0072  r+...r7...r-...r
-00002940: 1b00 0000 7212 0000 0072 1200 0000 7212  ....r....r....r.
-00002950: 0000 0072 1500 0000 7295 0000 001d 0100  ...r....r.......
-00002960: 0073 0600 0000 0800 0a01 1604 7295 0000  .s..........r...
-00002970: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00002980: 0000 0300 0000 4000 0000 7342 0000 0065  ......@...sB...e
-00002990: 005a 0164 005a 0255 0064 015a 0365 0465  .Z.d.Z.U.d.Z.e.e
-000029a0: 0564 023c 0064 015a 0665 0765 0419 0065  .d.<.d.Z.e.e...e
-000029b0: 0564 033c 0064 015a 0865 0465 0564 043c  .d.<.d.Z.e.e.d.<
-000029c0: 0064 055a 0965 0a65 0564 063c 0064 0753  .d.Z.e.e.d.<.d.S
-000029d0: 0029 08da 0652 756e 4c6f 6772 1100 0000  .)...RunLogr....
-000029e0: 7217 0000 0072 c600 0000 727d 0000 0072  r....r....r}...r
-000029f0: 0100 0000 da07 6479 6e61 6d69 634e 290b  ......dynamicN).
-00002a00: 7229 0000 0072 2a00 0000 722b 0000 0072  r)...r*...r+...r
-00002a10: 1700 0000 722d 0000 00da 0f5f 5f61 6e6e  ....r-.....__ann
-00002a20: 6f74 6174 696f 6e73 5f5f 72c6 0000 0072  otations__r....r
-00002a30: 0900 0000 727d 0000 0072 cd00 0000 728a  ....r}...r....r.
-00002a40: 0000 0072 1200 0000 7212 0000 0072 1200  ...r....r....r..
-00002a50: 0000 7215 0000 0072 cc00 0000 2e01 0000  ..r....r........
-00002a60: 730a 0000 000a 000c 0210 010c 0110 0172  s..............r
-00002a70: cc00 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00002a80: 0000 0000 0003 0000 0040 0000 0073 3400  .........@...s4.
-00002a90: 0000 6500 5a01 6400 5a02 5500 6401 5a03  ..e.Z.d.Z.U.d.Z.
-00002aa0: 6504 6505 6402 3c00 6506 8300 5a07 6506  e.e.d.<.e...Z.e.
-00002ab0: 6505 6403 3c00 6401 5a08 6504 6505 6404  e.d.<.d.Z.e.e.d.
-00002ac0: 3c00 6405 5300 2906 da0a 5072 6f6d 7074  <.d.S.)...Prompt
-00002ad0: 536e 6170 7211 0000 00da 0669 6e70 7574  Snapr......input
-00002ae0: 5fda 0772 756e 5f6c 6f67 727d 0000 004e  _..run_logr}...N
-00002af0: 2909 7229 0000 0072 2a00 0000 722b 0000  ).r)...r*...r+..
-00002b00: 0072 d000 0000 7205 0000 0072 ce00 0000  .r....r....r....
-00002b10: 72cc 0000 0072 d100 0000 727d 0000 0072  r....r....r}...r
-00002b20: 1200 0000 7212 0000 0072 1200 0000 7215  ....r....r....r.
-00002b30: 0000 0072 cf00 0000 3601 0000 7308 0000  ...r....6...s...
-00002b40: 000a 000c 020e 0110 0172 cf00 0000 6300  .........r....c.
-00002b50: 0000 0000 0000 0000 0000 0000 0000 0004  ................
-00002b60: 0000 0040 0000 0073 5a00 0000 6500 5a01  ...@...sZ...e.Z.
-00002b70: 6400 5a02 5500 6401 5a03 6504 6505 6402  d.Z.U.d.Z.e.e.d.
-00002b80: 3c00 6900 5a06 6507 6508 6504 6504 6602  <.i.Z.e.e.e.e.f.
-00002b90: 1900 6509 650a 1900 6602 1900 6505 6403  ..e.e...f...e.d.
-00002ba0: 3c00 6900 5a0b 6507 6504 6504 6602 1900  <.i.Z.e.e.e.f...
-00002bb0: 6505 6404 3c00 6405 5a0c 650d 6505 6406  e.d.<.d.Z.e.e.d.
-00002bc0: 3c00 6407 5300 2908 7296 0000 0072 0100  <.d.S.).r....r..
-00002bd0: 0000 da03 6964 5fda 0c70 726f 6d70 745f  ....id_..prompt_
-00002be0: 7374 6f72 65da 0c70 726f 6d70 745f 636f  store..prompt_co
-00002bf0: 756e 7472 1100 0000 7297 0000 004e 290e  untr....r....N).
-00002c00: 7229 0000 0072 2a00 0000 722b 0000 0072  r)...r*...r+...r
-00002c10: d200 0000 728a 0000 0072 ce00 0000 72d3  ....r....r....r.
-00002c20: 0000 0072 0600 0000 720a 0000 0072 0800  ...r....r....r..
-00002c30: 0000 72cf 0000 0072 d400 0000 7297 0000  ..r....r....r...
-00002c40: 0072 2d00 0000 7212 0000 0072 1200 0000  .r-...r....r....
-00002c50: 7212 0000 0072 1500 0000 7296 0000 003d  r....r....r....=
-00002c60: 0100 0073 0a00 0000 0a00 0c01 2001 1401  ...s........ ...
-00002c70: 1001 7296 0000 0072 9700 0000 720e 0000  ..r....r....r...
-00002c80: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
-00002c90: 0000 0400 0000 4300 0000 7318 0000 0074  ......C...s....t
-00002ca0: 0074 017c 009b 0064 019d 0264 0283 0283  .t.|...d...d....
-00002cb0: 0101 0064 0053 00a9 034e 7a04 2e6c 6f67  ...d.S...Nz..log
-00002cc0: da01 7729 0272 0c00 0000 da04 6f70 656e  ..w).r......open
-00002cd0: a901 7297 0000 0072 1200 0000 7212 0000  ..r....r....r...
-00002ce0: 0072 1500 0000 da11 7365 745f 6d69 6e69  .r......set_mini
-00002cf0: 6368 6169 6e5f 6c6f 6744 0100 0072 af00  chain_logD...r..
-00002d00: 0000 72d9 0000 0063 0000 0000 0000 0000  ..r....c........
-00002d10: 0000 0000 0000 0000 0800 0000 4000 0000  ............@...
-00002d20: 734a 0000 0065 005a 0164 005a 0264 015a  sJ...e.Z.d.Z.d.Z
-00002d30: 0364 0265 0466 0264 0364 0484 045a 0564  .d.e.f.d.d...Z.d
-00002d40: 0e64 0664 0784 045a 0664 0865 0764 0965  .d.d...Z.d.e.d.e
-00002d50: 0865 0919 0064 0a65 0865 0a19 0064 0564  .e...d.e.e...d.d
-00002d60: 0b66 0864 0c64 0d84 045a 0b64 0b53 0029  .f.d.d...Z.d.S.)
-00002d70: 0fda 094d 696e 6943 6861 696e 7a80 0a20  ...MiniChainz.. 
-00002d80: 2020 204d 696e 6943 6861 696e 2073 6573     MiniChain ses
-00002d90: 7369 6f6e 206f 626a 6563 7420 7769 7468  sion object with
-00002da0: 2062 6163 6b65 6e64 732e 204d 616b 6520   backends. Make 
-00002db0: 6261 636b 656e 6420 6279 2063 616c 6c69  backend by calli
-00002dc0: 6e67 0a20 2020 2060 6d69 6e69 6368 6169  ng.    `minichai
-00002dd0: 6e2e 4f70 656e 4149 2829 6020 7769 7468  n.OpenAI()` with
-00002de0: 2061 7267 7320 666f 7220 604f 7065 6e41   args for `OpenA
-00002df0: 4960 2063 6c61 7373 2e0a 2020 2020 7297  I` class..    r.
-00002e00: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-00002e10: 0200 0000 0400 0000 4300 0000 731e 0000  ........C...s...
-00002e20: 0074 0074 017c 019b 0064 019d 0264 0283  .t.t.|...d...d..
-00002e30: 0283 0101 007c 017c 005f 0264 0053 0072  .....|.|._.d.S.r
-00002e40: d500 0000 2903 720c 0000 0072 d700 0000  ....).r....r....
-00002e50: 7297 0000 0029 0272 1400 0000 7297 0000  r....).r....r...
-00002e60: 0072 1200 0000 7212 0000 0072 1500 0000  .r....r....r....
-00002e70: 7237 0000 004e 0100 0073 0400 0000 1401  r7...N...s......
-00002e80: 0a01 7a12 4d69 6e69 4368 6169 6e2e 5f5f  ..z.MiniChain.__
-00002e90: 696e 6974 5f5f 720e 0000 0063 0100 0000  init__r....c....
-00002ea0: 0000 0000 0000 0000 0100 0000 0300 0000  ................
-00002eb0: 4300 0000 7326 0000 0069 0074 005f 0169  C...s&...i.t._.i
-00002ec0: 0074 005f 027c 006a 0374 005f 0374 047c  .t._.|.j.t._.t.|
-00002ed0: 006a 0364 018d 017c 005f 057c 0053 0029  .j.d...|._.|.S.)
-00002ee0: 024e 2901 da0b 6163 7469 6f6e 5f74 7970  .N)...action_typ
-00002ef0: 6529 0672 9600 0000 72d3 0000 0072 d400  e).r....r....r..
-00002f00: 0000 7297 0000 0072 0b00 0000 da06 6163  ..r....r......ac
-00002f10: 7469 6f6e 7213 0000 0072 1200 0000 7212  tionr....r....r.
-00002f20: 0000 0072 1500 0000 da09 5f5f 656e 7465  ...r......__ente
-00002f30: 725f 5f52 0100 0073 0a00 0000 0601 0601  r__R...s........
-00002f40: 0801 0e01 0401 7a13 4d69 6e69 4368 6169  ......z.MiniChai
-00002f50: 6e2e 5f5f 656e 7465 725f 5fda 0474 7970  n.__enter__..typ
-00002f60: 65da 0965 7863 6570 7469 6f6e da09 7472  e..exception..tr
-00002f70: 6163 6562 6163 6b4e 6304 0000 0000 0000  acebackNc.......
-00002f80: 0000 0000 0004 0000 0002 0000 0043 0000  .............C..
-00002f90: 0073 2c00 0000 7c00 6a00 a001 a100 0100  .s,...|.j.......
-00002fa0: 7402 7403 6a04 8301 7c00 5f04 6900 7403  t.t.j...|._.i.t.
-00002fb0: 5f04 6900 7403 5f05 6401 7403 5f06 6400  _.i.t._.d.t._.d.
-00002fc0: 5300 7210 0000 0029 0772 dc00 0000 da06  S.r....).r......
-00002fd0: 6669 6e69 7368 7288 0000 0072 9600 0000  finishr....r....
-00002fe0: 72d3 0000 0072 d400 0000 7297 0000 0029  r....r....r....)
-00002ff0: 0472 1400 0000 72de 0000 0072 df00 0000  .r....r....r....
-00003000: 72e0 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
-00003010: 1500 0000 da08 5f5f 6578 6974 5f5f 5901  ......__exit__Y.
-00003020: 0000 730a 0000 000a 060c 0106 0106 010a  ..s.............
-00003030: 017a 124d 696e 6943 6861 696e 2e5f 5f65  .z.MiniChain.__e
-00003040: 7869 745f 5f29 0272 0e00 0000 72da 0000  xit__).r....r...
-00003050: 0029 0c72 2900 0000 722a 0000 0072 2b00  .).r)...r*...r+.
-00003060: 0000 7270 0000 0072 2d00 0000 7237 0000  ..rp...r-...r7..
-00003070: 0072 dd00 0000 72de 0000 0072 0900 0000  .r....r....r....
-00003080: da0d 4261 7365 4578 6365 7074 696f 6e72  ..BaseExceptionr
-00003090: 0300 0000 72e2 0000 0072 1200 0000 7212  ....r....r....r.
-000030a0: 0000 0072 1200 0000 7215 0000 0072 da00  ...r....r....r..
-000030b0: 0000 4801 0000 731a 0000 0008 0004 010e  ..H...s.........
-000030c0: 050a 0402 0702 0202 fe06 0302 fd06 0402  ................
-000030d0: fc02 050e fb72 da00 0000 6301 0000 0000  .....r....c.....
-000030e0: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
-000030f0: 0000 0073 0800 0000 7400 7c00 8301 5300  ...s....t.|...S.
-00003100: 2901 7a65 0a20 2020 2049 6e69 7469 616c  ).ze.    Initial
-00003110: 697a 6520 6120 6368 6169 6e2e 204c 6f67  ize a chain. Log
-00003120: 7320 746f 207b 6e61 6d65 7d2e 6c6f 672e  s to {name}.log.
-00003130: 2052 6574 7572 6e73 2061 2060 4d69 6e69   Returns a `Mini
-00003140: 4368 6169 6e60 2074 6861 740a 2020 2020  Chain` that.    
-00003150: 686f 6c64 7320 4c4c 4d20 6261 636b 656e  holds LLM backen
-00003160: 6473 2e2e 0a20 2020 2029 0172 da00 0000  ds...    ).r....
-00003170: 72d8 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
-00003180: 1500 0000 da0b 7374 6172 745f 6368 6169  ......start_chai
-00003190: 6e66 0100 0073 0200 0000 0805 72e4 0000  nf...s......r...
-000031a0: 0029 2972 5200 0000 7278 0000 0072 3a00  .))rR...rx...r:.
-000031b0: 0000 da0b 6461 7461 636c 6173 7365 7372  ....dataclassesr
-000031c0: 0200 0000 da05 7479 7065 7372 0300 0000  ......typesr....
-000031d0: da06 7479 7069 6e67 7204 0000 0072 0500  ..typingr....r..
-000031e0: 0000 7206 0000 0072 0700 0000 7208 0000  ..r....r....r...
-000031f0: 0072 0900 0000 720a 0000 00da 0667 7261  .r....r......gra
-00003200: 6469 6f72 2400 0000 da05 656c 696f 7472  dior$.....eliotr
-00003210: 0b00 0000 720c 0000 0072 9400 0000 720d  ....r....r....r.
-00003220: 0000 0072 3000 0000 7233 0000 0072 4000  ...r0...r3...r@.
-00003230: 0000 725c 0000 0072 7100 0000 7280 0000  ..r\...rq...r...
-00003240: 0072 8c00 0000 72a7 0000 0072 b400 0000  .r....r....r....
-00003250: 72b6 0000 0072 c800 0000 7295 0000 0072  r....r....r....r
-00003260: cc00 0000 72cf 0000 0072 9600 0000 722d  ....r....r....r-
-00003270: 0000 0072 d900 0000 72da 0000 0072 e400  ...r....r....r..
-00003280: 0000 7212 0000 0072 1200 0000 7212 0000  ..r....r....r...
-00003290: 0072 1500 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-000032a0: 0100 0000 733e 0000 0008 0008 0108 010c  ....s>..........
-000032b0: 010c 0124 0108 0210 0104 0208 010e 0310  ...$............
-000032c0: 1510 0510 1410 2c10 1c10 2410 1410 2610  ......,...$...&.
-000032d0: 1710 0510 0f10 0f02 1110 0102 0710 010e  ................
-000032e0: 0612 070e 0416 1e                        .......
+00000080: 0100 6400 6405 6c0f 6d10 5a10 6d11 5a11  ..d.d.l.m.Z.m.Z.
+00000090: 0100 6508 7238 6400 6401 6c12 5a12 4700  ..e.r8d.d.l.Z.G.
+000000a0: 6406 6407 8400 6407 8302 5a13 4700 6408  d.d...d...Z.G.d.
+000000b0: 6409 8400 6409 6513 8303 5a14 4700 640a  d...d.e...Z.G.d.
+000000c0: 640b 8400 640b 6513 8303 5a15 4700 640c  d...d.e...Z.G.d.
+000000d0: 640d 8400 640d 6513 8303 5a16 4700 640e  d...d.e...Z.G.d.
+000000e0: 640f 8400 640f 6513 8303 5a17 4700 6410  d...d.e...Z.G.d.
+000000f0: 6411 8400 6411 6513 8303 5a18 4700 6412  d...d.e...Z.G.d.
+00000100: 6413 8400 6413 6513 8303 5a19 4700 6414  d...d.e...Z.G.d.
+00000110: 6415 8400 6415 6519 8303 5a1a 4700 6416  d...d.e...Z.G.d.
+00000120: 6417 8400 6417 6519 8303 5a1b 4700 6418  d...d.e...Z.G.d.
+00000130: 6419 8400 6419 6513 8303 5a1c 4700 641a  d...d.e...Z.G.d.
+00000140: 641b 8400 641b 651c 8303 5a1d 4700 641c  d...d.e...Z.G.d.
+00000150: 641d 8400 641d 651c 8303 5a1e 4700 641e  d...d.e...Z.G.d.
+00000160: 641f 8400 641f 6513 8303 5a1f 6504 4700  d...d.e...Z.e.G.
+00000170: 6420 6421 8400 6421 8302 8301 5a20 6504  d d!..d!....Z e.
+00000180: 4700 6422 6423 8400 6423 8302 8301 5a21  G.d"d#..d#....Z!
+00000190: 4700 6424 6425 8400 6425 8302 5a22 6426  G.d$d%..d%..Z"d&
+000001a0: 6523 6427 6401 6604 6428 6429 8404 5a24  e#d'd.f.d(d)..Z$
+000001b0: 4700 642a 642b 8400 642b 8302 5a25 6426  G.d*d+..d+..Z%d&
+000001c0: 6523 6427 6525 6604 642c 642d 8404 5a26  e#d'e%f.d,d-..Z&
+000001d0: 6401 5300 292e e900 0000 004e 2901 da09  d.S.)......N)...
+000001e0: 6461 7461 636c 6173 7329 01da 0d54 7261  dataclass)...Tra
+000001f0: 6365 6261 636b 5479 7065 2907 da0d 5459  cebackType)...TY
+00000200: 5045 5f43 4845 434b 494e 47da 0341 6e79  PE_CHECKING..Any
+00000210: da04 4469 6374 da08 4974 6572 6174 6f72  ..Dict..Iterator
+00000220: da04 4c69 7374 da08 4f70 7469 6f6e 616c  ..List..Optional
+00000230: da05 5475 706c 6529 02da 0c73 7461 7274  ..Tuple)...start
+00000240: 5f61 6374 696f 6eda 0774 6f5f 6669 6c65  _action..to_file
+00000250: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000260: 0005 0000 0040 0000 0073 6800 0000 6500  .....@...sh...e.
+00000270: 5a01 6400 5a02 6503 6401 6504 6602 6402  Z.d.Z.e.d.e.f.d.
+00000280: 6403 8404 8301 5a05 6404 6504 6401 6504  d.....Z.d.e.d.e.
+00000290: 6604 6405 6406 8404 5a06 6404 6504 6401  f.d.d...Z.d.e.d.
+000002a0: 6507 6504 1900 6604 6407 6408 8404 5a08  e.e...f.d.d...Z.
+000002b0: 6404 6504 6401 6504 6604 6409 640a 8404  d.e.d.e.f.d.d...
+000002c0: 5a09 640b 640c 8400 5a0a 640d 640e 8400  Z.d.d...Z.d.d...
+000002d0: 5a0b 640f 5300 2910 da07 4261 636b 656e  Z.d.S.)...Backen
+000002e0: 64da 0672 6574 7572 6e63 0100 0000 0000  d..returnc......
+000002f0: 0000 0000 0000 0100 0000 0100 0000 4300  ..............C.
+00000300: 0000 f304 0000 0064 0153 00a9 024e da00  .......d.S...N..
+00000310: a900 a901 da04 7365 6c66 7212 0000 0072  ......selfr....r
+00000320: 1200 0000 fa55 2f68 6f6d 652f 7372 7573  .....U/home/srus
+00000330: 682f 5072 6f6a 6563 7473 2f4d 696e 6943  h/Projects/MiniC
+00000340: 6861 696e 2f76 656e 762f 6c69 622f 7079  hain/venv/lib/py
+00000350: 7468 6f6e 332e 3130 2f73 6974 652d 7061  thon3.10/site-pa
+00000360: 636b 6167 6573 2f6d 696e 6963 6861 696e  ckages/minichain
+00000370: 2f62 6163 6b65 6e64 2e70 79da 0b64 6573  /backend.py..des
+00000380: 6372 6970 7469 6f6e 0f00 0000 7302 0000  cription....s...
+00000390: 0004 027a 1342 6163 6b65 6e64 2e64 6573  ...z.Backend.des
+000003a0: 6372 6970 7469 6f6e da07 7265 7175 6573  cription..reques
+000003b0: 7463 0200 0000 0000 0000 0000 0000 0200  tc..............
+000003c0: 0000 0100 0000 4300 0000 7304 0000 0074  ......C...s....t
+000003d0: 0082 01a9 014e 2901 da13 4e6f 7449 6d70  .....N)...NotImp
+000003e0: 6c65 6d65 6e74 6564 4572 726f 72a9 0272  lementedError..r
+000003f0: 1400 0000 7217 0000 0072 1200 0000 7212  ....r....r....r.
+00000400: 0000 0072 1500 0000 da03 7275 6e13 0000  ...r......run...
+00000410: 00f3 0200 0000 0401 7a0b 4261 636b 656e  ........z.Backen
+00000420: 642e 7275 6e63 0200 0000 0000 0000 0000  d.runc..........
+00000430: 0000 0200 0000 0300 0000 6300 0000 7312  ..........c...s.
+00000440: 0000 0081 007c 00a0 007c 01a1 0156 0001  .....|...|...V..
+00000450: 0064 0053 0072 1800 0000 a901 721b 0000  .d.S.r......r...
+00000460: 0072 1a00 0000 7212 0000 0072 1200 0000  .r....r....r....
+00000470: 7215 0000 00da 0a72 756e 5f73 7472 6561  r......run_strea
+00000480: 6d16 0000 0073 0400 0000 0280 1001 7a12  m....s........z.
+00000490: 4261 636b 656e 642e 7275 6e5f 7374 7265  Backend.run_stre
+000004a0: 616d 6302 0000 0000 0000 0000 0000 0002  amc.............
+000004b0: 0000 0003 0000 00c3 0000 0073 0c00 0000  ...........s....
+000004c0: 8101 7c00 a000 7c01 a101 5300 7218 0000  ..|...|...S.r...
+000004d0: 0072 1d00 0000 721a 0000 0072 1200 0000  .r....r....r....
+000004e0: 7212 0000 0072 1500 0000 da04 6172 756e  r....r......arun
+000004f0: 1900 0000 7304 0000 0002 800a 017a 0c42  ....s........z.B
+00000500: 6163 6b65 6e64 2e61 7275 6e63 0200 0000  ackend.arunc....
+00000510: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+00000520: 4300 0000 f30c 0000 007c 016a 0064 0164  C........|.j.d.d
+00000530: 028d 0153 00a9 034e 4629 01da 0a73 686f  ...S...NF)...sho
+00000540: 775f 6c61 6265 6ca9 01da 0754 6578 7462  w_label....Textb
+00000550: 6f78 a902 7214 0000 00da 0267 7272 1200  ox..r......grr..
+00000560: 0000 7212 0000 0072 1500 0000 da0c 5f62  ..r....r......_b
+00000570: 6c6f 636b 5f69 6e70 7574 1c00 0000 f302  lock_input......
+00000580: 0000 000c 017a 1442 6163 6b65 6e64 2e5f  .....z.Backend._
+00000590: 626c 6f63 6b5f 696e 7075 7463 0200 0000  block_inputc....
+000005a0: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+000005b0: 4300 0000 7220 0000 0072 2100 0000 7223  C...r ...r!...r#
+000005c0: 0000 0072 2500 0000 7212 0000 0072 1200  ...r%...r....r..
+000005d0: 0000 7215 0000 00da 0d5f 626c 6f63 6b5f  ..r......_block_
+000005e0: 6f75 7470 7574 1f00 0000 7228 0000 007a  output....r(...z
+000005f0: 1542 6163 6b65 6e64 2e5f 626c 6f63 6b5f  .Backend._block_
+00000600: 6f75 7470 7574 4e29 0cda 085f 5f6e 616d  outputN)...__nam
+00000610: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
+00000620: 0c5f 5f71 7561 6c6e 616d 655f 5fda 0870  .__qualname__..p
+00000630: 726f 7065 7274 79da 0373 7472 7216 0000  roperty..strr...
+00000640: 0072 1b00 0000 7207 0000 0072 1e00 0000  .r....r....r....
+00000650: 721f 0000 0072 2700 0000 7229 0000 0072  r....r'...r)...r
+00000660: 1200 0000 7212 0000 0072 1200 0000 7215  ....r....r....r.
+00000670: 0000 0072 0d00 0000 0e00 0000 7310 0000  ...r........s...
+00000680: 0008 0002 0110 0112 0316 0312 0308 030c  ................
+00000690: 0372 0d00 0000 6300 0000 0000 0000 0000  .r....c.........
+000006a0: 0000 0000 0000 0004 0000 0040 0000 00f3  ...........@....
+000006b0: 1e00 0000 6500 5a01 6400 5a02 6401 6503  ....e.Z.d.Z.d.e.
+000006c0: 6402 6503 6604 6403 6404 8404 5a04 6405  d.e.f.d.d...Z.d.
+000006d0: 5300 2906 da02 4964 7217 0000 0072 0e00  S.)...Idr....r..
+000006e0: 0000 6302 0000 0000 0000 0000 0000 0002  ..c.............
+000006f0: 0000 0001 0000 0043 0000 0073 0400 0000  .......C...s....
+00000700: 7c01 5300 7218 0000 0072 1200 0000 721a  |.S.r....r....r.
+00000710: 0000 0072 1200 0000 7212 0000 0072 1500  ...r....r....r..
+00000720: 0000 721b 0000 0024 0000 0072 1c00 0000  ..r....$...r....
+00000730: 7a06 4964 2e72 756e 4ea9 0572 2a00 0000  z.Id.runN..r*...
+00000740: 722b 0000 0072 2c00 0000 722e 0000 0072  r+...r,...r....r
+00000750: 1b00 0000 7212 0000 0072 1200 0000 7212  ....r....r....r.
+00000760: 0000 0072 1500 0000 7230 0000 0023 0000  ...r....r0...#..
+00000770: 00f3 0400 0000 0800 1601 7230 0000 0063  ..........r0...c
+00000780: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000790: 0500 0000 4000 0000 7358 0000 0065 005a  ....@...sX...e.Z
+000007a0: 0164 005a 0267 0066 0164 0165 0365 0419  .d.Z.g.f.d.e.e..
+000007b0: 0066 0264 0264 0384 055a 0564 0465 0464  .f.d.d...Z.d.e.d
+000007c0: 0565 0466 0464 0664 0784 045a 0664 0465  .e.f.d.d...Z.d.e
+000007d0: 0464 0565 0765 0419 0066 0464 0864 0984  .d.e.e...f.d.d..
+000007e0: 045a 0864 0565 0466 0264 0a64 0b84 045a  .Z.d.e.f.d.d...Z
+000007f0: 0964 0c53 0029 0dda 044d 6f63 6bda 0761  .d.S.)...Mock..a
+00000800: 6e73 7765 7273 6302 0000 0000 0000 0000  nswersc.........
+00000810: 0000 0002 0000 0002 0000 0043 0000 0073  ...........C...s
+00000820: 1000 0000 6401 7c00 5f00 7c01 7c00 5f01  ....d.|._.|.|._.
+00000830: 6400 5300 2902 4ee9 ffff ffff 2902 da01  d.S.).N.....)...
+00000840: 6972 3400 0000 2902 7214 0000 0072 3400  ir4...).r....r4.
+00000850: 0000 7212 0000 0072 1200 0000 7215 0000  ..r....r....r...
+00000860: 00da 085f 5f69 6e69 745f 5f29 0000 0073  ...__init__)...s
+00000870: 0400 0000 0601 0a01 7a0d 4d6f 636b 2e5f  ........z.Mock._
+00000880: 5f69 6e69 745f 5f72 1700 0000 720e 0000  _init__r....r...
+00000890: 0063 0200 0000 0000 0000 0000 0000 0200  .c..............
+000008a0: 0000 0400 0000 4300 0000 7324 0000 007c  ......C...s$...|
+000008b0: 0004 006a 0064 0137 0002 005f 007c 006a  ...j.d.7..._.|.j
+000008c0: 017c 006a 0074 027c 006a 0183 0116 0019  .|.j.t.|.j......
+000008d0: 0053 0029 024e e901 0000 0029 0372 3600  .S.).N.....).r6.
+000008e0: 0000 7234 0000 00da 036c 656e 721a 0000  ..r4.....lenr...
+000008f0: 0072 1200 0000 7212 0000 0072 1500 0000  .r....r....r....
+00000900: 721b 0000 002d 0000 0073 0400 0000 0e01  r....-...s......
+00000910: 1601 7a08 4d6f 636b 2e72 756e 6302 0000  ..z.Mock.runc...
+00000920: 0000 0000 0000 0000 0004 0000 0004 0000  ................
+00000930: 0063 0000 0073 4400 0000 8100 7c00 0400  .c...sD.....|...
+00000940: 6a00 6401 3700 0200 5f00 7c00 6a01 7c00  j.d.7..._.|.j.|.
+00000950: 6a00 7402 7c00 6a01 8301 1600 1900 7d02  j.t.|.j.......}.
+00000960: 7c02 4400 5d0a 7d03 7c03 5600 0100 7403  |.D.].}.|.V...t.
+00000970: a004 6402 a101 0100 7115 6400 5300 2903  ..d.....q.d.S.).
+00000980: 4e72 3800 0000 679a 9999 9999 99b9 3f29  Nr8...g.......?)
+00000990: 0572 3600 0000 7234 0000 0072 3900 0000  .r6...r4...r9...
+000009a0: da04 7469 6d65 da05 736c 6565 7029 0472  ..time..sleep).r
+000009b0: 1400 0000 7217 0000 00da 0672 6573 756c  ....r......resul
+000009c0: 74da 0163 7212 0000 0072 1200 0000 7215  t..cr....r....r.
+000009d0: 0000 0072 1e00 0000 3100 0000 730e 0000  ...r....1...s...
+000009e0: 0002 800e 0116 0108 0106 010c 0104 fe7a  ...............z
+000009f0: 0f4d 6f63 6b2e 7275 6e5f 7374 7265 616d  .Mock.run_stream
+00000a00: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00000a10: 0002 0000 0043 0000 00f3 0c00 0000 6401  .....C........d.
+00000a20: 7c00 6a00 9b00 9d02 5300 2902 4e7a 0f4d  |.j.....S.).Nz.M
+00000a30: 6f63 6b65 6420 4261 636b 656e 6420 2901  ocked Backend ).
+00000a40: 7234 0000 0072 1300 0000 7212 0000 0072  r4...r....r....r
+00000a50: 1200 0000 7215 0000 00da 085f 5f72 6570  ....r......__rep
+00000a60: 725f 5f38 0000 0072 2800 0000 7a0d 4d6f  r__8...r(...z.Mo
+00000a70: 636b 2e5f 5f72 6570 725f 5f4e 290a 722a  ck.__repr__N).r*
+00000a80: 0000 0072 2b00 0000 722c 0000 0072 0800  ...r+...r,...r..
+00000a90: 0000 722e 0000 0072 3700 0000 721b 0000  ..r....r7...r...
+00000aa0: 0072 0700 0000 721e 0000 0072 3f00 0000  .r....r....r?...
+00000ab0: 7212 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
+00000ac0: 1500 0000 7233 0000 0028 0000 0073 0a00  ....r3...(...s..
+00000ad0: 0000 0800 1601 1204 1604 1207 7233 0000  ............r3..
+00000ae0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00000af0: 0000 0400 0000 4000 0000 7336 0000 0065  ......@...s6...e
+00000b00: 005a 0164 005a 0264 0a64 0364 0484 045a  .Z.d.Z.d.d.d...Z
+00000b10: 0364 0565 0464 0165 0466 0464 0664 0784  .d.e.d.e.f.d.d..
+00000b20: 045a 0564 0165 0466 0264 0864 0984 045a  .Z.d.e.f.d.d...Z
+00000b30: 0664 0253 0029 0bda 0647 6f6f 676c 6572  .d.S.)...Googler
+00000b40: 0e00 0000 4e63 0100 0000 0000 0000 0000  ....Nc..........
+00000b50: 0000 0100 0000 0100 0000 4300 0000 7304  ..........C...s.
+00000b60: 0000 0064 0053 0072 1800 0000 7212 0000  ...d.S.r....r...
+00000b70: 0072 1300 0000 7212 0000 0072 1200 0000  .r....r....r....
+00000b80: 7215 0000 0072 3700 0000 3d00 0000 721c  r....r7...=...r.
+00000b90: 0000 007a 0f47 6f6f 676c 652e 5f5f 696e  ...z.Google.__in
+00000ba0: 6974 5f5f 7217 0000 0063 0200 0000 0000  it__r....c......
+00000bb0: 0000 0000 0000 0800 0000 0700 0000 4300  ..............C.
+00000bc0: 0000 731a 0100 0064 0164 026c 006d 017d  ..s....d.d.l.m.}
+00000bd0: 0201 0074 026a 03a0 0464 03a1 017d 037c  ...t.j...d...}.|
+00000be0: 0373 124a 0064 0483 0182 017c 037c 005f  .s.J.d.....|.|._
+00000bf0: 057c 006a 0564 057c 0164 0664 0764 0864  .|.j.d.|.d.d.d.d
+00000c00: 099c 067d 047c 027c 0483 017d 057c 05a0  ...}.|.|...}.|..
+00000c10: 06a1 007d 0664 0a7c 06a0 07a1 0076 0072  ...}.d.|.....v.r
+00000c20: 3f64 0b7c 0664 0a19 00a0 07a1 0076 0072  ?d.|.d.......v.r
+00000c30: 3f7c 0664 0a19 0064 0b19 007d 0774 087c  ?|.d...d...}.t.|
+00000c40: 0783 0153 0064 0a7c 06a0 07a1 0076 0072  ...S.d.|.....v.r
+00000c50: 5764 0c7c 0664 0a19 00a0 07a1 0076 0072  Wd.|.d.......v.r
+00000c60: 577c 0664 0a19 0064 0c19 007d 0774 087c  W|.d...d...}.t.|
+00000c70: 0783 0153 0064 0a7c 06a0 07a1 0076 0072  ...S.d.|.....v.r
+00000c80: 7164 0d7c 0664 0a19 00a0 07a1 0076 0072  qd.|.d.......v.r
+00000c90: 717c 0664 0a19 0064 0d19 0064 0119 007d  q|.d...d...d...}
+00000ca0: 0774 087c 0783 0153 0064 0c7c 0664 0e19  .t.|...S.d.|.d..
+00000cb0: 0064 0119 00a0 07a1 0076 0072 877c 0664  .d.......v.r.|.d
+00000cc0: 0e19 0064 0119 0064 0c19 007d 0774 087c  ...d...d...}.t.|
+00000cd0: 0783 0153 0064 0f7d 0774 087c 0783 0153  ...S.d.}.t.|...S
+00000ce0: 0029 104e 7201 0000 0029 01da 0c47 6f6f  .).Nr....)...Goo
+00000cf0: 676c 6553 6561 7263 68da 0853 4552 505f  gleSearch..SERP_
+00000d00: 4b45 597a 3f4e 6565 6420 6120 5345 5250  KEYz?Need a SERP
+00000d10: 5f4b 4559 2e20 4765 7420 6f6e 6520 6865  _KEY. Get one he
+00000d20: 7265 2068 7474 7073 3a2f 2f73 6572 7061  re https://serpa
+00000d30: 7069 2e63 6f6d 2f75 7365 7273 2f77 656c  pi.com/users/wel
+00000d40: 636f 6d65 da06 676f 6f67 6c65 7a0a 676f  come..googlez.go
+00000d50: 6f67 6c65 2e63 6f6d da02 7573 da02 656e  ogle.com..us..en
+00000d60: 2906 da07 6170 695f 6b65 79da 0665 6e67  )...api_key..eng
+00000d70: 696e 65da 0171 da0d 676f 6f67 6c65 5f64  ine..q..google_d
+00000d80: 6f6d 6169 6eda 0267 6cda 0268 6cda 0a61  omain..gl..hl..a
+00000d90: 6e73 7765 725f 626f 78da 0661 6e73 7765  nswer_box..answe
+00000da0: 72da 0773 6e69 7070 6574 da19 736e 6970  r..snippet..snip
+00000db0: 7065 745f 6869 6768 6c69 6768 7465 645f  pet_highlighted_
+00000dc0: 776f 7264 73da 0f6f 7267 616e 6963 5f72  words..organic_r
+00000dd0: 6573 756c 7473 7211 0000 0029 09da 0773  esultsr....)...s
+00000de0: 6572 7061 7069 7241 0000 00da 026f 73da  erpapirA.....os.
+00000df0: 0765 6e76 6972 6f6e da03 6765 74da 0b73  .environ..get..s
+00000e00: 6572 7061 7069 5f6b 6579 da08 6765 745f  erpapi_key..get_
+00000e10: 6469 6374 da04 6b65 7973 722e 0000 0029  dict..keysr....)
+00000e20: 0872 1400 0000 7217 0000 0072 4100 0000  .r....r....rA...
+00000e30: 7255 0000 00da 0670 6172 616d 73da 0673  rU.....params..s
+00000e40: 6561 7263 68da 0372 6573 da05 746f 7265  earch..res..tore
+00000e50: 7472 1200 0000 7212 0000 0072 1500 0000  tr....r....r....
+00000e60: 721b 0000 0040 0000 0073 4200 0000 0c01  r....@...sB.....
+00000e70: 0c02 0202 04ff 0202 04fe 0603 0403 0201  ................
+00000e80: 0201 0201 0201 0201 06fa 0809 0801 1c02  ................
+00000e90: 0c01 080c 1cf5 0c01 080a 0af8 02ff 0e02  ................
+00000ea0: 02fe 1004 0805 14fc 1001 0803 04ff 0801  ................
+00000eb0: 7a0a 476f 6f67 6c65 2e72 756e 6301 0000  z.Google.runc...
+00000ec0: 0000 0000 0000 0000 0001 0000 0001 0000  ................
+00000ed0: 0043 0000 0072 0f00 0000 2902 4e7a 1547  .C...r....).Nz.G
+00000ee0: 6f6f 676c 6520 5365 6172 6368 2042 6163  oogle Search Bac
+00000ef0: 6b65 6e64 7212 0000 0072 1300 0000 7212  kendr....r....r.
+00000f00: 0000 0072 1200 0000 7215 0000 0072 3f00  ...r....r....r?.
+00000f10: 0000 6400 0000 721c 0000 007a 0f47 6f6f  ..d...r....z.Goo
+00000f20: 676c 652e 5f5f 7265 7072 5f5f 2902 720e  gle.__repr__).r.
+00000f30: 0000 004e 2907 722a 0000 0072 2b00 0000  ...N).r*...r+...
+00000f40: 722c 0000 0072 3700 0000 722e 0000 0072  r,...r7...r....r
+00000f50: 1b00 0000 723f 0000 0072 1200 0000 7212  ....r?...r....r.
+00000f60: 0000 0072 1200 0000 7215 0000 0072 4000  ...r....r....r@.
+00000f70: 0000 3c00 0000 7308 0000 0008 000a 0112  ..<...s.........
+00000f80: 0312 2472 4000 0000 6300 0000 0000 0000  ..$r@...c.......
+00000f90: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
+00000fa0: 0073 4000 0000 6500 5a01 6400 5a02 6401  .s@...e.Z.d.Z.d.
+00000fb0: 5a03 6402 6403 8400 5a04 6404 6405 8400  Z.d.d...Z.d.d...
+00000fc0: 5a05 6406 6506 6407 6506 6604 6408 6409  Z.d.e.d.e.f.d.d.
+00000fd0: 8404 5a07 6407 6506 6602 640a 640b 8404  ..Z.d.e.f.d.d...
+00000fe0: 5a08 640c 5300 290d da06 5079 7468 6f6e  Z.d.S.)...Python
+00000ff0: 7a30 4578 6563 7574 6573 2050 7974 686f  z0Executes Pytho
+00001000: 6e20 636f 6d6d 616e 6473 2061 6e64 2072  n commands and r
+00001010: 6574 7572 6e73 2074 6865 206f 7574 7075  eturns the outpu
+00001020: 742e 6302 0000 0000 0000 0000 0000 0002  t.c.............
+00001030: 0000 0002 0000 0043 0000 00f3 0800 0000  .......C........
+00001040: 7c01 a000 a100 5300 7218 0000 00a9 01da  |.....S.r.......
+00001050: 0443 6f64 6572 2500 0000 7212 0000 0072  .Coder%...r....r
+00001060: 1200 0000 7215 0000 0072 2700 0000 6b00  ....r....r'...k.
+00001070: 0000 f302 0000 0008 017a 1350 7974 686f  .........z.Pytho
+00001080: 6e2e 5f62 6c6f 636b 5f69 6e70 7574 6302  n._block_inputc.
+00001090: 0000 0000 0000 0000 0000 0002 0000 0002  ................
+000010a0: 0000 0043 0000 0072 5d00 0000 7218 0000  ...C...r]...r...
+000010b0: 0072 5e00 0000 7225 0000 0072 1200 0000  .r^...r%...r....
+000010c0: 7212 0000 0072 1500 0000 7229 0000 006e  r....r....r)...n
+000010d0: 0000 0072 6000 0000 7a14 5079 7468 6f6e  ...r`...z.Python
+000010e0: 2e5f 626c 6f63 6b5f 6f75 7470 7574 7217  ._block_outputr.
+000010f0: 0000 0072 0e00 0000 6302 0000 0000 0000  ...r....c.......
+00001100: 0000 0000 0007 0000 0008 0000 0043 0000  .............C..
+00001110: 0073 8800 0000 6401 6402 6c00 6d01 7d02  .s....d.d.l.m.}.
+00001120: 0100 6401 6403 6c02 6d03 7d03 0100 7c01  ..d.d.l.m.}...|.
+00001130: a004 a100 7d04 7c04 a005 6404 a101 7223  ....}.|...d...r#
+00001140: 6405 a006 7c04 a004 a100 a007 6405 a101  d...|.......d...
+00001150: 6406 6407 8502 1900 a101 7d04 7c03 8300  d.d.......}.|...
+00001160: 7d05 7c02 7c05 8301 8f0c 0100 7408 7c04  }.|.|.......t.|.
+00001170: 8301 0100 5700 6408 0400 0400 8303 0100  ....W.d.........
+00001180: 6e08 3100 7339 7701 0100 0100 0100 5900  n.1.s9w.......Y.
+00001190: 0100 7c05 a009 a100 7d06 7c06 5300 2909  ..|.....}.|.S.).
+000011a0: fa25 5275 6e20 636f 6d6d 616e 6473 2061  .%Run commands a
+000011b0: 6e64 2072 6574 7572 6e20 6669 6e61 6c20  nd return final 
+000011c0: 6f75 7470 7574 2e72 0100 0000 2901 da0f  output.r....)...
+000011d0: 7265 6469 7265 6374 5f73 7464 6f75 7429  redirect_stdout)
+000011e0: 01da 0853 7472 696e 6749 4f7a 0360 6060  ...StringIOz.```
+000011f0: da01 0a72 3800 0000 7235 0000 004e 290a  ...r8...r5...N).
+00001200: da0a 636f 6e74 6578 746c 6962 7262 0000  ..contextlibrb..
+00001210: 00da 0269 6f72 6300 0000 da05 7374 7269  ...iorc.....stri
+00001220: 70da 0a73 7461 7274 7377 6974 68da 046a  p..startswith..j
+00001230: 6f69 6eda 0573 706c 6974 da04 6578 6563  oin..split..exec
+00001240: da08 6765 7476 616c 7565 2907 7214 0000  ..getvalue).r...
+00001250: 0072 1700 0000 7262 0000 0072 6300 0000  .r....rb...rc...
+00001260: da01 70da 0166 da01 7372 1200 0000 7212  ..p..f..sr....r.
+00001270: 0000 0072 1500 0000 721b 0000 0071 0000  ...r....r....q..
+00001280: 0073 1600 0000 0c02 0c01 0802 0a01 1c01  .s..............
+00001290: 0602 0a01 0a01 1cff 0802 0401 7a0a 5079  ............z.Py
+000012a0: 7468 6f6e 2e72 756e 6301 0000 0000 0000  thon.runc.......
+000012b0: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
+000012c0: 0072 0f00 0000 2902 4e7a 0e50 7974 686f  .r....).Nz.Pytho
+000012d0: 6e2d 4261 636b 656e 6472 1200 0000 7213  n-Backendr....r.
+000012e0: 0000 0072 1200 0000 7212 0000 0072 1500  ...r....r....r..
+000012f0: 0000 723f 0000 0080 0000 0072 1c00 0000  ..r?.......r....
+00001300: 7a0f 5079 7468 6f6e 2e5f 5f72 6570 725f  z.Python.__repr_
+00001310: 5f4e 2909 722a 0000 0072 2b00 0000 722c  _N).r*...r+...r,
+00001320: 0000 00da 075f 5f64 6f63 5f5f 7227 0000  .....__doc__r'..
+00001330: 0072 2900 0000 722e 0000 0072 1b00 0000  .r)...r....r....
+00001340: 723f 0000 0072 1200 0000 7212 0000 0072  r?...r....r....r
+00001350: 1200 0000 7215 0000 0072 5c00 0000 6800  ....r....r\...h.
+00001360: 0000 730c 0000 0008 0004 0108 0208 0312  ..s.............
+00001370: 0312 0f72 5c00 0000 6300 0000 0000 0000  ...r\...c.......
+00001380: 0000 0000 0000 0000 0005 0000 0040 0000  .............@..
+00001390: 0073 5400 0000 6500 5a01 6400 5a02 6401  .sT...e.Z.d.Z.d.
+000013a0: 5a03 6402 6403 8400 5a04 6404 6405 8400  Z.d.d...Z.d.d...
+000013b0: 5a05 6412 6407 6506 6408 6506 6604 6409  Z.d.d.e.d.e.f.d.
+000013c0: 640a 8405 5a07 640b 6508 640c 6508 6604  d...Z.d.e.d.e.f.
+000013d0: 640d 640e 8404 5a09 640c 6508 6602 640f  d.d...Z.d.e.f.d.
+000013e0: 6410 8404 5a0a 6411 5300 2913 da04 4261  d...Z.d.S.)...Ba
+000013f0: 7368 7a2e 4578 6563 7574 6573 2062 6173  shz.Executes bas
+00001400: 6820 636f 6d6d 616e 6473 2061 6e64 2072  h commands and r
+00001410: 6574 7572 6e73 2074 6865 206f 7574 7075  eturns the outpu
+00001420: 742e 6302 0000 0000 0000 0000 0000 0002  t.c.............
+00001430: 0000 0002 0000 0043 0000 0072 5d00 0000  .......C...r]...
+00001440: 7218 0000 0072 5e00 0000 7225 0000 0072  r....r^...r%...r
+00001450: 1200 0000 7212 0000 0072 1500 0000 7227  ....r....r....r'
+00001460: 0000 0087 0000 0072 6000 0000 7a11 4261  .......r`...z.Ba
+00001470: 7368 2e5f 626c 6f63 6b5f 696e 7075 7463  sh._block_inputc
+00001480: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00001490: 0200 0000 4300 0000 725d 0000 0072 1800  ....C...r]...r..
+000014a0: 0000 725e 0000 0072 2500 0000 7212 0000  ..r^...r%...r...
+000014b0: 0072 1200 0000 7215 0000 0072 2900 0000  .r....r....r)...
+000014c0: 8a00 0000 7260 0000 007a 1242 6173 682e  ....r`...z.Bash.
+000014d0: 5f62 6c6f 636b 5f6f 7574 7075 7446 da0e  _block_outputF..
+000014e0: 7374 7269 705f 6e65 776c 696e 6573 da11  strip_newlines..
+000014f0: 7265 7475 726e 5f65 7272 5f6f 7574 7075  return_err_outpu
+00001500: 7463 0300 0000 0000 0000 0000 0000 0300  tc..............
+00001510: 0000 0200 0000 4300 0000 7310 0000 007c  ......C...s....|
+00001520: 017c 005f 007c 027c 005f 0164 0153 0029  .|._.|.|._.d.S.)
+00001530: 027a 2349 6e69 7469 616c 697a 6520 7769  .z#Initialize wi
+00001540: 7468 2073 7472 6970 7069 6e67 206e 6577  th stripping new
+00001550: 6c69 6e65 732e 4e29 0272 7200 0000 7273  lines.N).rr...rs
+00001560: 0000 0029 0372 1400 0000 7272 0000 0072  ...).r....rr...r
+00001570: 7300 0000 7212 0000 0072 1200 0000 7215  s...r....r....r.
+00001580: 0000 0072 3700 0000 8d00 0000 7304 0000  ...r7.......s...
+00001590: 0006 020a 017a 0d42 6173 682e 5f5f 696e  .....z.Bash.__in
+000015a0: 6974 5f5f 7217 0000 0072 0e00 0000 6302  it__r....r....c.
+000015b0: 0000 0000 0000 0000 0000 0004 0000 000a  ................
+000015c0: 0000 0043 0000 0073 8400 0000 7a11 7400  ...C...s....z.t.
+000015d0: 6a01 7c01 6401 6401 7400 6a02 7400 6a03  j.|.d.d.t.j.t.j.
+000015e0: 6402 8d05 6a04 a005 a100 7d02 5700 6e27  d...j.....}.W.n'
+000015f0: 0400 7400 6a06 7938 0100 7d03 0100 7a1a  ..t.j.y8..}...z.
+00001600: 7c00 6a07 722a 7408 7c03 6a04 a005 a100  |.j.r*t.|.j.....
+00001610: 8301 5700 0600 5900 6403 7d03 7e03 5300  ..W...Y.d.}.~.S.
+00001620: 7408 7c03 8301 5700 0600 5900 6403 7d03  t.|...W...Y.d.}.
+00001630: 7e03 5300 6403 7d03 7e03 7701 7700 7c00  ~.S.d.}.~.w.w.|.
+00001640: 6a09 7240 7c02 a00a a100 7d02 7c02 5300  j.r@|.....}.|.S.
+00001650: 2904 7261 0000 0054 2904 da05 7368 656c  ).ra...T)...shel
+00001660: 6cda 0563 6865 636b da06 7374 646f 7574  l..check..stdout
+00001670: da06 7374 6465 7272 4e29 0bda 0a73 7562  ..stderrN)...sub
+00001680: 7072 6f63 6573 7372 1b00 0000 da04 5049  processr......PI
+00001690: 5045 da06 5354 444f 5554 7276 0000 00da  PE..STDOUTrv....
+000016a0: 0664 6563 6f64 65da 1243 616c 6c65 6450  .decode..CalledP
+000016b0: 726f 6365 7373 4572 726f 7272 7300 0000  rocessErrorrs...
+000016c0: 722e 0000 0072 7200 0000 7267 0000 0029  r....rr...rg...)
+000016d0: 0472 1400 0000 7217 0000 00da 066f 7574  .r....r......out
+000016e0: 7075 74da 0565 7272 6f72 7212 0000 0072  put..errorr....r
+000016f0: 1200 0000 7215 0000 0072 1b00 0000 9200  ....r....r......
+00001700: 0000 7326 0000 0002 0204 0102 0102 0102  ..s&............
+00001710: 0104 0104 0104 fb06 0606 fa10 0706 011a  ................
+00001720: 0114 0108 8002 fd06 0408 0104 017a 0842  .............z.B
+00001730: 6173 682e 7275 6e63 0100 0000 0000 0000  ash.runc........
+00001740: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
+00001750: 720f 0000 0029 024e 7a0c 4261 7368 2d42  r....).Nz.Bash-B
+00001760: 6163 6b65 6e64 7212 0000 0072 1300 0000  ackendr....r....
+00001770: 7212 0000 0072 1200 0000 7215 0000 0072  r....r....r....r
+00001780: 3f00 0000 a400 0000 721c 0000 007a 0d42  ?.......r....z.B
+00001790: 6173 682e 5f5f 7265 7072 5f5f 4e29 0246  ash.__repr__N).F
+000017a0: 4629 0b72 2a00 0000 722b 0000 0072 2c00  F).r*...r+...r,.
+000017b0: 0000 7270 0000 0072 2700 0000 7229 0000  ..rp...r'...r)..
+000017c0: 00da 0462 6f6f 6c72 3700 0000 722e 0000  ...boolr7...r...
+000017d0: 0072 1b00 0000 723f 0000 0072 1200 0000  .r....r?...r....
+000017e0: 7212 0000 0072 1200 0000 7215 0000 0072  r....r....r....r
+000017f0: 7100 0000 8400 0000 730e 0000 0008 0004  q.......s.......
+00001800: 0108 0208 0314 0312 0512 1272 7100 0000  ...........rq...
+00001810: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00001820: 000b 0000 0040 0000 0073 4a00 0000 6500  .....@...sJ...e.
+00001830: 5a01 6400 5a02 0901 0902 0903 0904 640e  Z.d.Z.........d.
+00001840: 6405 6503 6406 6504 6407 6505 6408 6506  d.e.d.e.d.e.d.e.
+00001850: 6507 6503 1900 1900 6409 6404 660a 640a  e.e.....d.d.f.d.
+00001860: 640b 8405 5a08 6409 6503 6602 640c 640d  d...Z.d.e.f.d.d.
+00001870: 8404 5a09 6404 5300 290f da0a 4f70 656e  ..Z.d.S.)...Open
+00001880: 4149 4261 7365 fa0d 6770 742d 332e 352d  AIBase..gpt-3.5-
+00001890: 7475 7262 6fe9 0001 0000 e700 0000 0000  turbo...........
+000018a0: 0000 004e da05 6d6f 6465 6cda 0a6d 6178  ...N..model..max
+000018b0: 5f74 6f6b 656e 73da 0b74 656d 7065 7261  _tokens..tempera
+000018c0: 7475 7265 da04 7374 6f70 720e 0000 0063  ture..stopr....c
+000018d0: 0500 0000 0000 0000 0000 0000 0500 0000  ................
+000018e0: 0500 0000 4300 0000 7320 0000 007c 017c  ....C...s ...|.|
+000018f0: 005f 007c 047c 005f 0174 027c 017c 027c  ._.|.|._.t.|.|.|
+00001900: 0364 018d 037c 005f 0364 0053 0029 024e  .d...|._.d.S.).N
+00001910: 2903 7284 0000 0072 8500 0000 7286 0000  ).r....r....r...
+00001920: 0029 0472 8400 0000 7287 0000 00da 0464  .).r....r......d
+00001930: 6963 74da 076f 7074 696f 6e73 2905 7214  ict..options).r.
+00001940: 0000 0072 8400 0000 7285 0000 0072 8600  ...r....r....r..
+00001950: 0000 7287 0000 0072 1200 0000 7212 0000  ..r....r....r...
+00001960: 0072 1500 0000 7237 0000 00a9 0000 0073  .r....r7.......s
+00001970: 0e00 0000 0607 0601 0201 0201 0201 0201  ................
+00001980: 0cfd 7a13 4f70 656e 4149 4261 7365 2e5f  ..z.OpenAIBase._
+00001990: 5f69 6e69 745f 5f63 0100 0000 0000 0000  _init__c........
+000019a0: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
+000019b0: 723e 0000 0029 024e 7a0f 4f70 656e 4149  r>...).Nz.OpenAI
+000019c0: 2042 6163 6b65 6e64 2029 0172 8900 0000   Backend ).r....
+000019d0: 7213 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
+000019e0: 1500 0000 723f 0000 00b8 0000 0072 2800  ....r?.......r(.
+000019f0: 0000 7a13 4f70 656e 4149 4261 7365 2e5f  ..z.OpenAIBase._
+00001a00: 5f72 6570 725f 5f29 0472 8100 0000 7282  _repr__).r....r.
+00001a10: 0000 0072 8300 0000 4e29 0a72 2a00 0000  ...r....N).r*...
+00001a20: 722b 0000 0072 2c00 0000 722e 0000 00da  r+...r,...r.....
+00001a30: 0369 6e74 da05 666c 6f61 7472 0900 0000  .int..floatr....
+00001a40: 7208 0000 0072 3700 0000 723f 0000 0072  r....r7...r?...r
+00001a50: 1200 0000 7212 0000 0072 1200 0000 7215  ....r....r....r.
+00001a60: 0000 0072 8000 0000 a800 0000 7322 0000  ...r........s"..
+00001a70: 0008 0002 0302 0102 0102 0104 fb02 0202  ................
+00001a80: fe02 0302 fd02 0402 fc0a 0502 fb02 060a  ................
+00001a90: fa12 0f72 8000 0000 6300 0000 0000 0000  ...r....c.......
+00001aa0: 0000 0000 0000 0000 0005 0000 0040 0000  .............@..
+00001ab0: 0073 3400 0000 6500 5a01 6400 5a02 6401  .s4...e.Z.d.Z.d.
+00001ac0: 6503 6402 6503 6604 6403 6404 8404 5a04  e.d.e.f.d.d...Z.
+00001ad0: 6405 6503 6402 6505 6503 1900 6604 6406  d.e.d.e.e...f.d.
+00001ae0: 6407 8404 5a06 6408 5300 2909 da06 4f70  d...Z.d.S.)...Op
+00001af0: 656e 4149 7217 0000 0072 0e00 0000 6302  enAIr....r....c.
+00001b00: 0000 0000 0000 0000 0000 0005 0000 0006  ................
+00001b10: 0000 0043 0000 0073 5200 0000 6401 6400  ...C...sR...d.d.
+00001b20: 6c00 7d02 6402 6403 6802 7d03 7c02 6a01  l.}.d.d.h.}.|.j.
+00001b30: 7c00 6a02 7c03 7600 7211 6404 6e01 6405  |.j.|.v.r.d.n.d.
+00001b40: 7c00 6a03 6406 1900 6407 7404 6a05 9b00  |.j.d...d.t.j...
+00001b50: 6408 8d04 7d02 7c02 6a06 7c01 7c00 6a07  d...}.|.j.|.|.j.
+00001b60: 6409 8d02 7d04 7408 7c04 8301 5300 290a  d...}.t.|...S.).
+00001b70: 4e72 0100 0000 7a05 6770 742d 3472 8100  Nr....z.gpt-4r..
+00001b80: 0000 da0a 6f70 656e 6169 6368 6174 da06  ....openaichat..
+00001b90: 6f70 656e 6169 7285 0000 00da 0673 716c  openair......sql
+00001ba0: 6974 6529 04da 0b63 6c69 656e 745f 6e61  ite)...client_na
+00001bb0: 6d65 7285 0000 00da 0a63 6163 6865 5f6e  mer......cache_n
+00001bc0: 616d 65da 1063 6163 6865 5f63 6f6e 6e65  ame..cache_conne
+00001bd0: 6374 696f 6e29 01da 0e73 746f 705f 7365  ction)...stop_se
+00001be0: 7175 656e 6365 7329 09da 086d 616e 6966  quences)...manif
+00001bf0: 6573 74da 084d 616e 6966 6573 7472 8400  est..Manifestr..
+00001c00: 0000 7289 0000 00da 104d 696e 6963 6861  ..r......Minicha
+00001c10: 696e 436f 6e74 6578 74da 046e 616d 6572  inContext..namer
+00001c20: 1b00 0000 7287 0000 0072 2e00 0000 2905  ....r....r....).
+00001c30: 7214 0000 0072 1700 0000 7294 0000 00da  r....r....r.....
+00001c40: 0463 6861 74da 0361 6e73 7212 0000 0072  .chat..ansr....r
+00001c50: 1200 0000 7215 0000 0072 1b00 0000 bd00  ....r....r......
+00001c60: 0000 731a 0000 0008 0108 0204 0110 0108  ..s.............
+00001c70: 0102 0106 0106 fc04 0702 0104 0106 fe08  ................
+00001c80: 047a 0a4f 7065 6e41 492e 7275 6eda 0670  .z.OpenAI.run..p
+00001c90: 726f 6d70 7463 0200 0000 0000 0000 0000  romptc..........
+00001ca0: 0000 0500 0000 0600 0000 6300 0000 7380  ..........c...s.
+00001cb0: 0000 0081 0064 0164 006c 007d 0274 016a  .....d.d.l.}.t.j
+00001cc0: 02a0 0364 02a1 017c 005f 047c 006a 0473  ...d...|._.|.j.s
+00001cd0: 134a 0064 0383 0182 017c 006a 047c 025f  .J.d.....|.j.|._
+00001ce0: 047c 026a 056a 067c 006a 0764 047c 0164  .|.j.j.|.j.d.|.d
+00001cf0: 059c 0267 0164 067c 006a 0864 078d 0444  ...g.d.|.j.d...D
+00001d00: 005d 167d 037c 0364 0819 0064 0119 00a0  .].}.|.d...d....
+00001d10: 0364 0969 00a1 02a0 0364 0aa1 017d 047c  .d.i.....d...}.|
+00001d20: 0464 0075 0172 3d7c 0456 0001 0071 2764  .d.u.r=|.V...q'd
+00001d30: 0053 0029 0b4e 7201 0000 00da 0e4f 5045  .S.).Nr......OPE
+00001d40: 4e41 495f 4150 495f 4b45 59fa 3c4e 6565  NAI_API_KEY.<Nee
+00001d50: 6420 616e 204f 5045 4e41 495f 4150 495f  d an OPENAI_API_
+00001d60: 4b45 592e 2047 6574 206f 6e65 2068 6572  KEY. Get one her
+00001d70: 6520 6874 7470 733a 2f2f 6f70 656e 6169  e https://openai
+00001d80: 2e63 6f6d 2f61 7069 2fda 0475 7365 7229  .com/api/..user)
+00001d90: 02da 0472 6f6c 65da 0763 6f6e 7465 6e74  ...role..content
+00001da0: 5429 0472 8400 0000 da08 6d65 7373 6167  T).r......messag
+00001db0: 6573 da06 7374 7265 616d 7287 0000 00da  es..streamr.....
+00001dc0: 0763 686f 6963 6573 da05 6465 6c74 6172  .choices..deltar
+00001dd0: 9f00 0000 2909 728e 0000 0072 5200 0000  ....).r....rR...
+00001de0: 7253 0000 0072 5400 0000 7246 0000 00da  rS...rT...rF....
+00001df0: 0e43 6861 7443 6f6d 706c 6574 696f 6eda  .ChatCompletion.
+00001e00: 0663 7265 6174 6572 8400 0000 7287 0000  .creater....r...
+00001e10: 0029 0572 1400 0000 729a 0000 0072 8e00  .).r....r....r..
+00001e20: 0000 da05 6368 756e 6b72 9f00 0000 7212  ....chunkr....r.
+00001e30: 0000 0072 1200 0000 7215 0000 0072 1e00  ...r....r....r..
+00001e40: 0000 ce00 0000 7326 0000 0002 8008 010e  ......s&........
+00001e50: 0204 0204 ff02 0204 fe08 0306 0204 010a  ................
+00001e60: 0102 0104 010a fc1a 0608 0106 0102 8004  ................
+00001e70: f87a 114f 7065 6e41 492e 7275 6e5f 7374  .z.OpenAI.run_st
+00001e80: 7265 616d 4e29 0772 2a00 0000 722b 0000  reamN).r*...r+..
+00001e90: 0072 2c00 0000 722e 0000 0072 1b00 0000  .r,...r....r....
+00001ea0: 7207 0000 0072 1e00 0000 7212 0000 0072  r....r....r....r
+00001eb0: 1200 0000 7212 0000 0072 1500 0000 728c  ....r....r....r.
+00001ec0: 0000 00bc 0000 0073 0600 0000 0800 1201  .......s........
+00001ed0: 1a11 728c 0000 0063 0000 0000 0000 0000  ..r....c........
+00001ee0: 0000 0000 0000 0000 0700 0000 0000 0000  ................
+00001ef0: 7346 0000 0065 005a 0164 005a 0264 0164  sF...e.Z.d.Z.d.d
+00001f00: 0284 005a 0364 0d64 0465 0464 0565 0564  ...Z.d.d.e.d.e.d
+00001f10: 0664 0766 0687 0066 0164 0864 0984 0d5a  .d.f...f.d.d...Z
+00001f20: 0664 0a65 0464 0665 0466 0464 0b64 0c84  .d.e.d.e.f.d.d..
+00001f30: 045a 0787 0004 005a 0853 0029 0eda 0b4f  .Z.....Z.S.)...O
+00001f40: 7065 6e41 4945 6d62 6564 6302 0000 0000  penAIEmbedc.....
+00001f50: 0000 0000 0000 0002 0000 0003 0000 0043  ...............C
+00001f60: 0000 0072 2000 0000 2903 4eda 0945 6d62  ...r ...).N..Emb
+00001f70: 6564 6469 6e67 2901 da05 6c61 6265 6c72  edding)...labelr
+00001f80: 2300 0000 7225 0000 0072 1200 0000 7212  #...r%...r....r.
+00001f90: 0000 0072 1500 0000 7229 0000 00e3 0000  ...r....r)......
+00001fa0: 0072 2800 0000 7a19 4f70 656e 4149 456d  .r(...z.OpenAIEm
+00001fb0: 6265 642e 5f62 6c6f 636b 5f6f 7574 7075  bed._block_outpu
+00001fc0: 74fa 1674 6578 742d 656d 6265 6464 696e  t..text-embeddin
+00001fd0: 672d 6164 612d 3030 3272 8400 0000 da06  g-ada-002r......
+00001fe0: 6b77 6172 6773 720e 0000 004e 6302 0000  kwargsr....Nc...
+00001ff0: 0000 0000 0000 0000 0003 0000 0004 0000  ................
+00002000: 000b 0000 0073 1800 0000 7400 8300 6a01  .....s....t...j.
+00002010: 7c01 6601 6900 7c02 a401 8e01 0100 6400  |.f.i.|.......d.
+00002020: 5300 7218 0000 0029 02da 0573 7570 6572  S.r....)...super
+00002030: 7237 0000 0029 0372 1400 0000 7284 0000  r7...).r....r...
+00002040: 0072 ab00 0000 a901 da09 5f5f 636c 6173  .r........__clas
+00002050: 735f 5f72 1200 0000 7215 0000 0072 3700  s__r....r....r7.
+00002060: 0000 e600 0000 f302 0000 0018 017a 144f  .............z.O
+00002070: 7065 6e41 4945 6d62 6564 2e5f 5f69 6e69  penAIEmbed.__ini
+00002080: 745f 5f72 1700 0000 6302 0000 0000 0000  t__r....c.......
+00002090: 0000 0000 0004 0000 0004 0000 0043 0000  .............C..
+000020a0: 0073 4e00 0000 6401 6400 6c00 7d02 7401  .sN...d.d.l.}.t.
+000020b0: 6a02 a003 6402 a101 7c00 5f04 7c00 6a04  j...d...|._.|.j.
+000020c0: 7312 4a00 6403 8301 8201 7c00 6a04 7c02  s.J.d.....|.j.|.
+000020d0: 5f04 7c02 6a05 6a06 7c00 6a07 7c01 6404  _.|.j.j.|.j.|.d.
+000020e0: 8d02 7d03 7c03 6405 1900 6401 1900 6406  ..}.|.d...d...d.
+000020f0: 1900 5300 2907 4e72 0100 0000 729b 0000  ..S.).Nr....r...
+00002100: 0072 9c00 0000 2902 7247 0000 00da 0569  .r....).rG.....i
+00002110: 6e70 7574 da04 6461 7461 da09 656d 6265  nput..data..embe
+00002120: 6464 696e 6729 0872 8e00 0000 7252 0000  dding).r....rR..
+00002130: 0072 5300 0000 7254 0000 0072 4600 0000  .rS...rT...rF...
+00002140: 72a8 0000 0072 a500 0000 7284 0000 0029  r....r....r....)
+00002150: 0472 1400 0000 7217 0000 0072 8e00 0000  .r....r....r....
+00002160: 7299 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
+00002170: 1500 0000 721b 0000 00e9 0000 0073 1800  ....r........s..
+00002180: 0000 0801 0e02 0402 04ff 0202 04fe 0803  ................
+00002190: 0602 0401 0201 06fe 1004 7a0f 4f70 656e  ..........z.Open
+000021a0: 4149 456d 6265 642e 7275 6e29 0172 aa00  AIEmbed.run).r..
+000021b0: 0000 2909 722a 0000 0072 2b00 0000 722c  ..).r*...r+...r,
+000021c0: 0000 0072 2900 0000 722e 0000 0072 0500  ...r)...r....r..
+000021d0: 0000 7237 0000 0072 1b00 0000 da0d 5f5f  ..r7...r......__
+000021e0: 636c 6173 7363 656c 6c5f 5f72 1200 0000  classcell__r....
+000021f0: 7212 0000 0072 ad00 0000 7215 0000 0072  r....r....r....r
+00002200: a700 0000 e200 0000 7308 0000 0008 0008  ........s.......
+00002210: 011c 031a 0372 a700 0000 6300 0000 0000  .....r....c.....
+00002220: 0000 0000 0000 0000 0000 0005 0000 0040  ...............@
+00002230: 0000 0073 2000 0000 6500 5a01 6400 5a02  ...s ...e.Z.d.Z.
+00002240: 6407 6402 6503 6403 6404 6604 6405 6406  d.d.e.d.d.f.d.d.
+00002250: 8405 5a04 6404 5300 2908 da0f 4875 6767  ..Z.d.S.)...Hugg
+00002260: 696e 6746 6163 6542 6173 65da 0467 7074  ingFaceBase..gpt
+00002270: 3272 8400 0000 720e 0000 004e 6302 0000  2r....r....Nc...
+00002280: 0000 0000 0000 0000 0002 0000 0002 0000  ................
+00002290: 0043 0000 0073 0a00 0000 7c01 7c00 5f00  .C...s....|.|._.
+000022a0: 6400 5300 7218 0000 0029 0172 8400 0000  d.S.r....).r....
+000022b0: 2902 7214 0000 0072 8400 0000 7212 0000  ).r....r....r...
+000022c0: 0072 1200 0000 7215 0000 0072 3700 0000  .r....r....r7...
+000022d0: fa00 0000 7302 0000 000a 017a 1848 7567  ....s......z.Hug
+000022e0: 6769 6e67 4661 6365 4261 7365 2e5f 5f69  gingFaceBase.__i
+000022f0: 6e69 745f 5f29 0172 b500 0000 2905 722a  nit__).r....).r*
+00002300: 0000 0072 2b00 0000 722c 0000 0072 2e00  ...r+...r,...r..
+00002310: 0000 7237 0000 0072 1200 0000 7212 0000  ..r7...r....r...
+00002320: 0072 1200 0000 7215 0000 0072 b400 0000  .r....r....r....
+00002330: f900 0000 7304 0000 0008 0018 0172 b400  ....s........r..
+00002340: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00002350: 0000 0004 0000 0040 0000 0072 2f00 0000  .......@...r/...
+00002360: 2906 da0b 4875 6767 696e 6746 6163 6572  )...HuggingFacer
+00002370: 1700 0000 720e 0000 0063 0200 0000 0000  ....r....c......
+00002380: 0000 0000 0000 0400 0000 0500 0000 4300  ..............C.
+00002390: 0000 f34c 0000 0064 0164 026c 006d 017d  ...L...d.d.l.m.}
+000023a0: 0201 0074 026a 03a0 0464 03a1 017c 005f  ...t.j...d...|._
+000023b0: 057c 006a 0573 144a 0064 0483 0182 017c  .|.j.s.J.d.....|
+000023c0: 027c 006a 057c 006a 0664 0564 068d 037c  .|.j.|.j.d.d...|
+000023d0: 005f 077c 006a 077c 0164 078d 017d 037c  ._.|.j.|.d...}.|
+000023e0: 0353 0029 084e 7201 0000 00a9 01da 0c49  .S.).Nr........I
+000023f0: 6e66 6572 656e 6365 4170 69da 0648 465f  nferenceApi..HF_
+00002400: 4b45 59fa 344e 6565 6420 616e 2048 465f  KEY.4Need an HF_
+00002410: 4b45 592e 2047 6574 206f 6e65 2068 6572  KEY. Get one her
+00002420: 6520 6874 7470 733a 2f2f 6875 6767 696e  e https://huggin
+00002430: 6766 6163 652e 636f 2f7a 0f74 6578 742d  gface.co/z.text-
+00002440: 6765 6e65 7261 7469 6f6e a903 da05 746f  generation....to
+00002450: 6b65 6eda 0772 6570 6f5f 6964 da04 7461  ken..repo_id..ta
+00002460: 736b a901 da06 696e 7075 7473 a908 da1d  sk....inputs....
+00002470: 6875 6767 696e 6766 6163 655f 6875 622e  huggingface_hub.
+00002480: 696e 6665 7265 6e63 655f 6170 6972 b900  inference_apir..
+00002490: 0000 7252 0000 0072 5300 0000 7254 0000  ..rR...rS...rT..
+000024a0: 0072 4600 0000 7284 0000 00da 0663 6c69  .rF...r......cli
+000024b0: 656e 74a9 0472 1400 0000 7217 0000 0072  ent..r....r....r
+000024c0: b900 0000 da08 7265 7370 6f6e 7365 7212  ......responser.
+000024d0: 0000 0072 1200 0000 7215 0000 0072 1b00  ...r....r....r..
+000024e0: 0000 ff00 0000 f310 0000 000c 020e 020e  ................
+000024f0: 0102 020a 0108 ff0c 0304 017a 0f48 7567  ...........z.Hug
+00002500: 6769 6e67 4661 6365 2e72 756e 4e72 3100  gingFace.runNr1.
+00002510: 0000 7212 0000 0072 1200 0000 7212 0000  ..r....r....r...
+00002520: 0072 1500 0000 72b6 0000 00fe 0000 0072  .r....r........r
+00002530: 3200 0000 72b6 0000 0063 0000 0000 0000  2...r....c......
+00002540: 0000 0000 0000 0000 0000 0400 0000 4000  ..............@.
+00002550: 0000 722f 0000 0029 06da 1048 7567 6769  ..r/...)...Huggi
+00002560: 6e67 4661 6365 456d 6265 6472 1700 0000  ngFaceEmbedr....
+00002570: 720e 0000 0063 0200 0000 0000 0000 0000  r....c..........
+00002580: 0000 0400 0000 0500 0000 4300 0000 72b7  ..........C...r.
+00002590: 0000 0029 084e 7201 0000 0072 b800 0000  ...).Nr....r....
+000025a0: 72ba 0000 0072 bb00 0000 7a12 6665 6174  r....r....z.feat
+000025b0: 7572 652d 6578 7472 6163 7469 6f6e 72bc  ure-extractionr.
+000025c0: 0000 0072 c000 0000 72c2 0000 0072 c500  ...r....r....r..
+000025d0: 0000 7212 0000 0072 1200 0000 7215 0000  ..r....r....r...
+000025e0: 0072 1b00 0000 0e01 0000 72c7 0000 007a  .r........r....z
+000025f0: 1448 7567 6769 6e67 4661 6365 456d 6265  .HuggingFaceEmbe
+00002600: 642e 7275 6e4e 7231 0000 0072 1200 0000  d.runNr1...r....
+00002610: 7212 0000 0072 1200 0000 7215 0000 0072  r....r....r....r
+00002620: c800 0000 0d01 0000 7232 0000 0072 c800  ........r2...r..
+00002630: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00002640: 0000 0004 0000 0040 0000 0073 2800 0000  .......@...s(...
+00002650: 6500 5a01 6400 5a02 640a 6405 6406 8404  e.Z.d.Z.d.d.d...
+00002660: 5a03 6407 6504 6403 6504 6604 6408 6409  Z.d.e.d.e.f.d.d.
+00002670: 8404 5a05 6404 5300 290b 7295 0000 0072  ..Z.d.S.).r....r
+00002680: c400 0000 fa11 6d61 6e69 6665 7374 2e4d  ......manifest.M
+00002690: 616e 6966 6573 7472 0e00 0000 4e63 0200  anifestr....Nc..
+000026a0: 0000 0000 0000 0000 0000 0200 0000 0200  ................
+000026b0: 0000 4300 0000 730a 0000 007c 017c 005f  ..C...s....|.|._
+000026c0: 0064 0153 0029 027a 4443 6c69 656e 7420  .d.S.).zDClient 
+000026d0: 6672 6f6d 205b 4d61 6e69 6665 7374 2d4d  from [Manifest-M
+000026e0: 4c5d 2868 7474 7073 3a2f 2f67 6974 6875  L](https://githu
+000026f0: 622e 636f 6d2f 4861 7a79 5265 7365 6172  b.com/HazyResear
+00002700: 6368 2f6d 616e 6966 6573 7429 2e4e 2901  ch/manifest).N).
+00002710: 72c4 0000 0029 0272 1400 0000 72c4 0000  r....).r....r...
+00002720: 0072 1200 0000 7212 0000 0072 1500 0000  .r....r....r....
+00002730: 7237 0000 001d 0100 0073 0200 0000 0a02  r7.......s......
+00002740: 7a11 4d61 6e69 6665 7374 2e5f 5f69 6e69  z.Manifest.__ini
+00002750: 745f 5f72 1700 0000 6302 0000 0000 0000  t__r....c.......
+00002760: 0000 0000 0003 0000 0008 0000 0043 0000  .............C..
+00002770: 0073 4600 0000 7a06 6401 6400 6c00 7d02  .sF...z.d.d.l.}.
+00002780: 5700 6e0b 0400 7401 7911 0100 0100 0100  W.n...t.y.......
+00002790: 7401 6402 8301 8201 7700 7402 7c00 6a03  t.d.....w.t.|.j.
+000027a0: 7c02 6a04 8302 731d 4a00 6403 8301 8201  |.j...s.J.d.....
+000027b0: 7c00 6a03 a005 7c01 a101 5300 2904 4e72  |.j...|...S.).Nr
+000027c0: 0100 0000 7a36 6070 6970 2069 6e73 7461  ....z6`pip insta
+000027d0: 6c6c 206d 616e 6966 6573 742d 6d6c 6020  ll manifest-ml` 
+000027e0: 746f 2075 7365 2074 6865 204d 616e 6966  to use the Manif
+000027f0: 6573 7420 4261 636b 656e 642e 7a2e 436c  est Backend.z.Cl
+00002800: 6965 6e74 206d 7573 7420 6265 2061 2060  ient must be a `
+00002810: 6d61 6e69 6665 7374 2e4d 616e 6966 6573  manifest.Manifes
+00002820: 7460 2069 6e73 7461 6e63 652e 2906 7294  t` instance.).r.
+00002830: 0000 00da 0b49 6d70 6f72 7445 7272 6f72  .....ImportError
+00002840: da0a 6973 696e 7374 616e 6365 72c4 0000  ..isinstancer...
+00002850: 0072 9500 0000 721b 0000 0029 0372 1400  .r....r....).r..
+00002860: 0000 7217 0000 0072 9400 0000 7212 0000  ..r....r....r...
+00002870: 0072 1200 0000 7215 0000 0072 1b00 0000  .r....r....r....
+00002880: 2101 0000 7316 0000 0002 010c 010c 0108  !...s...........
+00002890: 0102 ff02 0208 0106 ff02 0204 fe0c 047a  ...............z
+000028a0: 0c4d 616e 6966 6573 742e 7275 6e29 0472  .Manifest.run).r
+000028b0: c400 0000 72c9 0000 0072 0e00 0000 4e29  ....r....r....N)
+000028c0: 0672 2a00 0000 722b 0000 0072 2c00 0000  .r*...r+...r,...
+000028d0: 7237 0000 0072 2e00 0000 721b 0000 0072  r7...r....r....r
+000028e0: 1200 0000 7212 0000 0072 1200 0000 7215  ....r....r....r.
+000028f0: 0000 0072 9500 0000 1c01 0000 7306 0000  ...r........s...
+00002900: 0008 000a 0116 0472 9500 0000 6300 0000  .......r....c...
+00002910: 0000 0000 0000 0000 0000 0000 0003 0000  ................
+00002920: 0040 0000 0073 4200 0000 6500 5a01 6400  .@...sB...e.Z.d.
+00002930: 5a02 5500 6401 5a03 6504 6505 6402 3c00  Z.U.d.Z.e.e.d.<.
+00002940: 6401 5a06 6507 6504 1900 6505 6403 3c00  d.Z.e.e...e.d.<.
+00002950: 6401 5a08 6504 6505 6404 3c00 6405 5a09  d.Z.e.e.d.<.d.Z.
+00002960: 650a 6505 6406 3c00 6407 5300 2908 da06  e.e.d.<.d.S.)...
+00002970: 5275 6e4c 6f67 7211 0000 0072 1700 0000  RunLogr....r....
+00002980: 72c6 0000 0072 7d00 0000 7201 0000 00da  r....r}...r.....
+00002990: 0764 796e 616d 6963 4e29 0b72 2a00 0000  .dynamicN).r*...
+000029a0: 722b 0000 0072 2c00 0000 7217 0000 0072  r+...r,...r....r
+000029b0: 2e00 0000 da0f 5f5f 616e 6e6f 7461 7469  ......__annotati
+000029c0: 6f6e 735f 5f72 c600 0000 7209 0000 0072  ons__r....r....r
+000029d0: 7d00 0000 72cd 0000 0072 8a00 0000 7212  }...r....r....r.
+000029e0: 0000 0072 1200 0000 7212 0000 0072 1500  ...r....r....r..
+000029f0: 0000 72cc 0000 002d 0100 0073 0a00 0000  ..r....-...s....
+00002a00: 0a00 0c02 1001 0c01 1001 72cc 0000 0063  ..........r....c
+00002a10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002a20: 0300 0000 4000 0000 7334 0000 0065 005a  ....@...s4...e.Z
+00002a30: 0164 005a 0255 0064 015a 0365 0465 0564  .d.Z.U.d.Z.e.e.d
+00002a40: 023c 0065 0683 005a 0765 0665 0564 033c  .<.e...Z.e.e.d.<
+00002a50: 0064 015a 0865 0465 0564 043c 0064 0553  .d.Z.e.e.d.<.d.S
+00002a60: 0029 06da 0a50 726f 6d70 7453 6e61 7072  .)...PromptSnapr
+00002a70: 1100 0000 da06 696e 7075 745f da07 7275  ......input_..ru
+00002a80: 6e5f 6c6f 6772 7d00 0000 4e29 0972 2a00  n_logr}...N).r*.
+00002a90: 0000 722b 0000 0072 2c00 0000 72d0 0000  ..r+...r,...r...
+00002aa0: 0072 0500 0000 72ce 0000 0072 cc00 0000  .r....r....r....
+00002ab0: 72d1 0000 0072 7d00 0000 7212 0000 0072  r....r}...r....r
+00002ac0: 1200 0000 7212 0000 0072 1500 0000 72cf  ....r....r....r.
+00002ad0: 0000 0035 0100 0073 0800 0000 0a00 0c02  ...5...s........
+00002ae0: 0e01 1001 72cf 0000 0063 0000 0000 0000  ....r....c......
+00002af0: 0000 0000 0000 0000 0000 0400 0000 4000  ..............@.
+00002b00: 0000 735a 0000 0065 005a 0164 005a 0255  ..sZ...e.Z.d.Z.U
+00002b10: 0064 015a 0365 0465 0564 023c 0069 005a  .d.Z.e.e.d.<.i.Z
+00002b20: 0665 0765 0865 0465 0466 0219 0065 0965  .e.e.e.e.f...e.e
+00002b30: 0a19 0066 0219 0065 0564 033c 0069 005a  ...f...e.d.<.i.Z
+00002b40: 0b65 0765 0465 0466 0219 0065 0564 043c  .e.e.e.f...e.d.<
+00002b50: 0064 055a 0c65 0d65 0564 063c 0064 0753  .d.Z.e.e.d.<.d.S
+00002b60: 0029 0872 9600 0000 7201 0000 00da 0369  .).r....r......i
+00002b70: 645f da0c 7072 6f6d 7074 5f73 746f 7265  d_..prompt_store
+00002b80: da0c 7072 6f6d 7074 5f63 6f75 6e74 7211  ..prompt_countr.
+00002b90: 0000 0072 9700 0000 4e29 0e72 2a00 0000  ...r....N).r*...
+00002ba0: 722b 0000 0072 2c00 0000 72d2 0000 0072  r+...r,...r....r
+00002bb0: 8a00 0000 72ce 0000 0072 d300 0000 7206  ....r....r....r.
+00002bc0: 0000 0072 0a00 0000 7208 0000 0072 cf00  ...r....r....r..
+00002bd0: 0000 72d4 0000 0072 9700 0000 722e 0000  ..r....r....r...
+00002be0: 0072 1200 0000 7212 0000 0072 1200 0000  .r....r....r....
+00002bf0: 7215 0000 0072 9600 0000 3c01 0000 730a  r....r....<...s.
+00002c00: 0000 000a 000c 0120 0114 0110 0172 9600  ....... .....r..
+00002c10: 0000 7297 0000 0072 0e00 0000 6301 0000  ..r....r....c...
+00002c20: 0000 0000 0000 0000 0001 0000 0004 0000  ................
+00002c30: 0043 0000 0073 1800 0000 7400 7401 7c00  .C...s....t.t.|.
+00002c40: 9b00 6401 9d02 6402 8302 8301 0100 6400  ..d...d.......d.
+00002c50: 5300 a903 4e7a 042e 6c6f 67da 0177 2902  S...Nz..log..w).
+00002c60: 720c 0000 00da 046f 7065 6ea9 0172 9700  r......open..r..
+00002c70: 0000 7212 0000 0072 1200 0000 7215 0000  ..r....r....r...
+00002c80: 00da 1173 6574 5f6d 696e 6963 6861 696e  ...set_minichain
+00002c90: 5f6c 6f67 4301 0000 72af 0000 0072 d900  _logC...r....r..
+00002ca0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00002cb0: 0000 0008 0000 0040 0000 0073 4a00 0000  .......@...sJ...
+00002cc0: 6500 5a01 6400 5a02 6401 5a03 6402 6504  e.Z.d.Z.d.Z.d.e.
+00002cd0: 6602 6403 6404 8404 5a05 640e 6406 6407  f.d.d...Z.d.d.d.
+00002ce0: 8404 5a06 6408 6507 6409 6508 6509 1900  ..Z.d.e.d.e.e...
+00002cf0: 640a 6508 650a 1900 6405 640b 6608 640c  d.e.e...d.d.f.d.
+00002d00: 640d 8404 5a0b 640b 5300 290f da09 4d69  d...Z.d.S.)...Mi
+00002d10: 6e69 4368 6169 6e7a 800a 2020 2020 4d69  niChainz..    Mi
+00002d20: 6e69 4368 6169 6e20 7365 7373 696f 6e20  niChain session 
+00002d30: 6f62 6a65 6374 2077 6974 6820 6261 636b  object with back
+00002d40: 656e 6473 2e20 4d61 6b65 2062 6163 6b65  ends. Make backe
+00002d50: 6e64 2062 7920 6361 6c6c 696e 670a 2020  nd by calling.  
+00002d60: 2020 606d 696e 6963 6861 696e 2e4f 7065    `minichain.Ope
+00002d70: 6e41 4928 2960 2077 6974 6820 6172 6773  nAI()` with args
+00002d80: 2066 6f72 2060 4f70 656e 4149 6020 636c   for `OpenAI` cl
+00002d90: 6173 732e 0a20 2020 2072 9700 0000 6302  ass..    r....c.
+00002da0: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00002db0: 0000 0043 0000 0073 1e00 0000 7400 7401  ...C...s....t.t.
+00002dc0: 7c01 9b00 6401 9d02 6402 8302 8301 0100  |...d...d.......
+00002dd0: 7c01 7c00 5f02 6400 5300 72d5 0000 0029  |.|._.d.S.r....)
+00002de0: 0372 0c00 0000 72d7 0000 0072 9700 0000  .r....r....r....
+00002df0: 2902 7214 0000 0072 9700 0000 7212 0000  ).r....r....r...
+00002e00: 0072 1200 0000 7215 0000 0072 3700 0000  .r....r....r7...
+00002e10: 4d01 0000 7304 0000 0014 010a 017a 124d  M...s........z.M
+00002e20: 696e 6943 6861 696e 2e5f 5f69 6e69 745f  iniChain.__init_
+00002e30: 5f72 0e00 0000 6301 0000 0000 0000 0000  _r....c.........
+00002e40: 0000 0001 0000 0003 0000 0043 0000 0073  ...........C...s
+00002e50: 2600 0000 6900 7400 5f01 6900 7400 5f02  &...i.t._.i.t._.
+00002e60: 7c00 6a03 7400 5f03 7404 7c00 6a03 6401  |.j.t._.t.|.j.d.
+00002e70: 8d01 7c00 5f05 7c00 5300 2902 4e29 01da  ..|._.|.S.).N)..
+00002e80: 0b61 6374 696f 6e5f 7479 7065 2906 7296  .action_type).r.
+00002e90: 0000 0072 d300 0000 72d4 0000 0072 9700  ...r....r....r..
+00002ea0: 0000 720b 0000 00da 0661 6374 696f 6e72  ..r......actionr
+00002eb0: 1300 0000 7212 0000 0072 1200 0000 7215  ....r....r....r.
+00002ec0: 0000 00da 095f 5f65 6e74 6572 5f5f 5101  .....__enter__Q.
+00002ed0: 0000 730a 0000 0006 0106 0108 010e 0104  ..s.............
+00002ee0: 017a 134d 696e 6943 6861 696e 2e5f 5f65  .z.MiniChain.__e
+00002ef0: 6e74 6572 5f5f da04 7479 7065 da09 6578  nter__..type..ex
+00002f00: 6365 7074 696f 6eda 0974 7261 6365 6261  ception..traceba
+00002f10: 636b 4e63 0400 0000 0000 0000 0000 0000  ckNc............
+00002f20: 0400 0000 0200 0000 4300 0000 732c 0000  ........C...s,..
+00002f30: 007c 006a 00a0 01a1 0001 0074 0274 036a  .|.j.......t.t.j
+00002f40: 0483 017c 005f 0469 0074 035f 0469 0074  ...|._.i.t._.i.t
+00002f50: 035f 0564 0174 035f 0664 0053 0072 1000  ._.d.t._.d.S.r..
+00002f60: 0000 2907 72dc 0000 00da 0666 696e 6973  ..).r......finis
+00002f70: 6872 8800 0000 7296 0000 0072 d300 0000  hr....r....r....
+00002f80: 72d4 0000 0072 9700 0000 2904 7214 0000  r....r....).r...
+00002f90: 0072 de00 0000 72df 0000 0072 e000 0000  .r....r....r....
+00002fa0: 7212 0000 0072 1200 0000 7215 0000 00da  r....r....r.....
+00002fb0: 085f 5f65 7869 745f 5f58 0100 0073 0a00  .__exit__X...s..
+00002fc0: 0000 0a06 0c01 0601 0601 0a01 7a12 4d69  ............z.Mi
+00002fd0: 6e69 4368 6169 6e2e 5f5f 6578 6974 5f5f  niChain.__exit__
+00002fe0: 2902 720e 0000 0072 da00 0000 290c 722a  ).r....r....).r*
+00002ff0: 0000 0072 2b00 0000 722c 0000 0072 7000  ...r+...r,...rp.
+00003000: 0000 722e 0000 0072 3700 0000 72dd 0000  ..r....r7...r...
+00003010: 0072 de00 0000 7209 0000 00da 0d42 6173  .r....r......Bas
+00003020: 6545 7863 6570 7469 6f6e 7203 0000 0072  eExceptionr....r
+00003030: e200 0000 7212 0000 0072 1200 0000 7212  ....r....r....r.
+00003040: 0000 0072 1500 0000 72da 0000 0047 0100  ...r....r....G..
+00003050: 0073 1a00 0000 0800 0401 0e05 0a04 0207  .s..............
+00003060: 0202 02fe 0603 02fd 0604 02fc 0205 0efb  ................
+00003070: 72da 0000 0063 0100 0000 0000 0000 0000  r....c..........
+00003080: 0000 0100 0000 0200 0000 4300 0000 7308  ..........C...s.
+00003090: 0000 0074 007c 0083 0153 0029 017a 650a  ...t.|...S.).ze.
+000030a0: 2020 2020 496e 6974 6961 6c69 7a65 2061      Initialize a
+000030b0: 2063 6861 696e 2e20 4c6f 6773 2074 6f20   chain. Logs to 
+000030c0: 7b6e 616d 657d 2e6c 6f67 2e20 5265 7475  {name}.log. Retu
+000030d0: 726e 7320 6120 604d 696e 6943 6861 696e  rns a `MiniChain
+000030e0: 6020 7468 6174 0a20 2020 2068 6f6c 6473  ` that.    holds
+000030f0: 204c 4c4d 2062 6163 6b65 6e64 732e 2e0a   LLM backends...
+00003100: 2020 2020 2901 72da 0000 0072 d800 0000      ).r....r....
+00003110: 7212 0000 0072 1200 0000 7215 0000 00da  r....r....r.....
+00003120: 0b73 7461 7274 5f63 6861 696e 6501 0000  .start_chaine...
+00003130: 7302 0000 0008 0572 e400 0000 2927 7252  s......r....)'rR
+00003140: 0000 0072 7800 0000 723a 0000 00da 0b64  ...rx...r:.....d
+00003150: 6174 6163 6c61 7373 6573 7202 0000 00da  ataclassesr.....
+00003160: 0574 7970 6573 7203 0000 00da 0674 7970  .typesr......typ
+00003170: 696e 6772 0400 0000 7205 0000 0072 0600  ingr....r....r..
+00003180: 0000 7207 0000 0072 0800 0000 7209 0000  ..r....r....r...
+00003190: 0072 0a00 0000 da05 656c 696f 7472 0b00  .r......eliotr..
+000031a0: 0000 720c 0000 0072 9400 0000 720d 0000  ..r....r....r...
+000031b0: 0072 3000 0000 7233 0000 0072 4000 0000  .r0...r3...r@...
+000031c0: 725c 0000 0072 7100 0000 7280 0000 0072  r\...rq...r....r
+000031d0: 8c00 0000 72a7 0000 0072 b400 0000 72b6  ....r....r....r.
+000031e0: 0000 0072 c800 0000 7295 0000 0072 cc00  ...r....r....r..
+000031f0: 0000 72cf 0000 0072 9600 0000 722e 0000  ..r....r....r...
+00003200: 0072 d900 0000 72da 0000 0072 e400 0000  .r....r....r....
+00003210: 7212 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
+00003220: 1500 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+00003230: 0000 733c 0000 0008 0008 0108 010c 010c  ..s<............
+00003240: 0124 0110 0204 0208 010e 0310 1510 0510  .$..............
+00003250: 1410 2c10 1c10 2410 1410 2610 1710 0510  ..,...$...&.....
+00003260: 0f10 0f02 1110 0102 0710 010e 0612 070e  ................
+00003270: 0416 1e                                  ...
```

### ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/__pycache__/gradio.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 21:30:57 2023 UTC, .py size: 11605 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 110c 3f64 552d 0000  o.........?dU-..
+00000000: 6f0d 0d0a 0000 0000 2ce6 3f64 8c2d 0000  o.......,.?d.-..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0019 0000 0040 0000 0073 de01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 0100 6400  d.l.m.Z.m.Z...d.
 00000050: 6403 6c05 6d06 5a06 6d07 5a07 6d08 5a08  d.l.m.Z.m.Z.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c  m.Z.m.Z.m.Z.m.Z.
 00000070: 0100 6400 6401 6c0d 5a0e 6400 6404 6c0f  ..d.d.l.Z.d.d.l.
@@ -606,17 +606,17 @@
 000025d0: 72a3 0000 0072 8800 0000 72a4 0000 0072  r....r....r....r
 000025e0: a500 0000 72a6 0000 0072 4200 0000 da04  ....r....rB.....
 000025f0: 6465 6d6f da09 7175 6572 795f 6274 6e72  demo..query_btnr
 00002600: b200 0000 72bc 0000 0072 1700 0000 72ba  ....r....r....r.
 00002610: 0000 0072 1800 0000 da04 7368 6f77 0b01  ...r......show..
 00002620: 0000 733a 0000 0016 201e 0106 0206 020a  ..s:.... .......
 00002630: 0316 010a 0312 030e 010c 010a 010a 0204  ................
-00002640: 020a 0106 ff1c fe26 0b18 0416 0214 0e04  .......&........
-00002650: 0212 010a cb04 3702 fd0a cc04 3710 c904  ......7.....7...
-00002660: 3772 ca00 0000 2901 5429 2772 bf00 0000  7r....).T)'r....
+00002640: 020a 0106 ff1c fe26 0b18 0416 0214 0f04  .......&........
+00002650: 0212 010a ca04 3802 fd0a cb04 3810 c804  ......8.....8...
+00002660: 3872 ca00 0000 2901 5429 2772 bf00 0000  8r....).T)'r....
 00002670: 7289 0000 00da 0b64 6174 6163 6c61 7373  r......dataclass
 00002680: 6573 7202 0000 0072 0300 0000 da06 7479  esr....r......ty
 00002690: 7069 6e67 7204 0000 0072 0500 0000 7206  pingr....r....r.
 000026a0: 0000 0072 0700 0000 7208 0000 0072 0900  ...r....r....r..
 000026b0: 0000 720a 0000 00da 0667 7261 6469 6f72  ..r......gradior
 000026c0: 1500 0000 da0d 6772 6164 696f 2e62 6c6f  ......gradio.blo
 000026d0: 636b 7372 0b00 0000 da09 6d69 6e69 6368  cksr......minich
```

### ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/backend.py

```diff
@@ -1,15 +1,14 @@
 import os
 import subprocess
 import time
 from dataclasses import dataclass
 from types import TracebackType
 from typing import TYPE_CHECKING, Any, Dict, Iterator, List, Optional, Tuple
 
-import gradio as gr
 from eliot import start_action, to_file
 
 if TYPE_CHECKING:
     import manifest
 
 
 class Backend:
@@ -22,18 +21,18 @@
 
     def run_stream(self, request: str) -> Iterator[str]:
         yield self.run(request)
 
     async def arun(self, request: str) -> str:
         return self.run(request)
 
-    def block_input(self) -> gr.Blocks:
+    def _block_input(self, gr):  # type: ignore
         return gr.Textbox(show_label=False)
 
-    def block_output(self) -> gr.Blocks:
+    def _block_output(self, gr):  # type: ignore
         return gr.Textbox(show_label=False)
 
 
 class Id(Backend):
     def run(self, request: str) -> str:
         return request
 
@@ -101,18 +100,18 @@
     def __repr__(self) -> str:
         return "Google Search Backend"
 
 
 class Python(Backend):
     """Executes Python commands and returns the output."""
 
-    def block_input(self) -> gr.Blocks:
+    def _block_input(self, gr):  # type: ignore
         return gr.Code()
 
-    def block_output(self) -> gr.Blocks:
+    def _block_output(self, gr):  # type: ignore
         return gr.Code()
 
     def run(self, request: str) -> str:
         """Run commands and return final output."""
         from contextlib import redirect_stdout
         from io import StringIO
 
@@ -129,18 +128,18 @@
     def __repr__(self) -> str:
         return "Python-Backend"
 
 
 class Bash(Backend):
     """Executes bash commands and returns the output."""
 
-    def block_input(self) -> gr.Blocks:
+    def _block_input(self, gr):  # type: ignore
         return gr.Code()
 
-    def block_output(self) -> gr.Blocks:
+    def _block_output(self, gr):  # type: ignore
         return gr.Code()
 
     def __init__(self, strip_newlines: bool = False, return_err_output: bool = False):
         """Initialize with stripping newlines."""
         self.strip_newlines = strip_newlines
         self.return_err_output = return_err_output
 
@@ -221,15 +220,15 @@
         ):
             content = chunk["choices"][0].get("delta", {}).get("content")
             if content is not None:
                 yield content
 
 
 class OpenAIEmbed(OpenAIBase):
-    def block_output(self) -> gr.Blocks:
+    def _block_output(self, gr):  # type: ignore
         return gr.Textbox(label="Embedding")
 
     def __init__(self, model: str = "text-embedding-ada-002", **kwargs: Any) -> None:
         super().__init__(model, **kwargs)
 
     def run(self, request: str) -> str:
         import openai
```

### ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/gradio.py

```diff
@@ -85,25 +85,25 @@
     with gr.Accordion(
         label=f"👩  Prompt: {str(base_prompt._fn)}", elem_id="prompt", visible=False
     ) as accordion_in:
         for backend in base_prompt.backend:
             if bp.gradio_conf is not None:
                 prompt = bp.gradio_conf.block_input()
             elif hasattr(backend, "_block_input"):
-                prompt = backend._block_input(gr)
+                prompt: gr.Blocks = backend._block_input(gr)  # type: ignore
             else:
                 prompt = GradioConf().block_input()
             prompts.append(prompt)
 
     with gr.Accordion(label="💻", elem_id="response", visible=False) as accordion_out:
         for backend in base_prompt.backend:
             if bp.gradio_conf is not None:
                 result = bp.gradio_conf.block_output()
             elif hasattr(backend, "_block_output"):
-                result = backend._block_output(gr)
+                result: gr.Blocks = backend._block_output(gr)  # type: ignore
             else:
                 result = GradioConf().block_output()
             results.append(result)
 
         with gr.Accordion(label="...", open=False, visible=show_advanced):
             gr.Markdown(f"Backend: {base_prompt.backend}", elem_id="json")
             input = gr.JSON(elem_id="json", label="Input")
@@ -343,13 +343,14 @@
                 for output in prompt(**prompt_inputs).run_gen():
                     data[all_data] = dict(MinichainContext.prompt_store)
                     data[final_output] = output
                     yield constructor.fn(data)
                     if output is not None:
                         break
             yield constructor.fn(data)
+
         query_btn.click(run, inputs=constructor.inputs, outputs=constructor.outputs)
 
         if code:
             gr.Code(code, language="python", elem_id="inner")
 
     return demo
```

### Comparing `./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain-0.3.1.egg-info/PKG-INFO` & `./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain-0.3.2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minichain
-Version: 0.3.1
+Version: 0.3.2
 Summary: A tiny library for large language models
 Home-page: https://github.com/srush/minichain
 Author: Sasha Rush
 Author-email: srush.research@gmail.com
 License: MIT
 Project-URL: Documentation, https://srush.github.io/minichain
 Project-URL: Source Code, https://github.com/srush/minichain
```

### Comparing `./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain-0.3.1.egg-info/SOURCES.txt` & `./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain-0.3.2.egg-info/SOURCES.txt`

 * *Files identical despite different names*


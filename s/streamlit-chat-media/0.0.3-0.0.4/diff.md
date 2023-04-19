# Comparing `tmp/streamlit-chat-media-0.0.3.tar.gz` & `tmp/streamlit-chat-media-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-chat-media-0.0.3.tar", last modified: Tue Mar 28 19:55:44 2023, max compression
+gzip compressed data, was "streamlit-chat-media-0.0.4.tar", last modified: Wed Apr 19 09:06:06 2023, max compression
```

## Comparing `streamlit-chat-media-0.0.3.tar` & `streamlit-chat-media-0.0.4.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxrwxr-x   0 alino     (1000) alino     (1000)        0 2023-03-28 19:55:44.153236 streamlit-chat-media-0.0.3/
--rw-rw-r--   0 alino     (1000) alino     (1000)     1064 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/LICENSE
--rw-rw-r--   0 alino     (1000) alino     (1000)       56 2023-03-28 15:21:06.000000 streamlit-chat-media-0.0.3/MANIFEST.in
--rw-rw-r--   0 alino     (1000) alino     (1000)     4183 2023-03-28 19:55:44.149236 streamlit-chat-media-0.0.3/PKG-INFO
--rw-rw-r--   0 alino     (1000) alino     (1000)     3687 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/README.md
--rw-rw-r--   0 alino     (1000) alino     (1000)       38 2023-03-28 19:55:44.153236 streamlit-chat-media-0.0.3/setup.cfg
--rw-rw-r--   0 alino     (1000) alino     (1000)      953 2023-03-28 19:54:37.000000 streamlit-chat-media-0.0.3/setup.py
-drwxrwxr-x   0 alino     (1000) alino     (1000)        0 2023-03-28 19:55:44.133236 streamlit-chat-media-0.0.3/streamlit_chat_media/
--rw-rw-r--   0 alino     (1000) alino     (1000)     3485 2023-03-28 15:21:37.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/__init__.py
-drwxrwxr-x   0 alino     (1000) alino     (1000)        0 2023-03-28 19:55:44.133236 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/
-drwxrwxr-x   0 alino     (1000) alino     (1000)        0 2023-03-28 19:55:44.137236 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/
--rw-rw-r--   0 alino     (1000) alino     (1000)     1150 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/asset-manifest.json
--rw-rw-r--   0 alino     (1000) alino     (1000)   197459 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/bootstrap.min.css
--rw-rw-r--   0 alino     (1000) alino     (1000)   646432 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/bootstrap.min.css.map
--rw-rw-r--   0 alino     (1000) alino     (1000)     2209 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/index.html
--rw-rw-r--   0 alino     (1000) alino     (1000)     8091 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/precache-manifest.c29a79fbc77e2c50510d007756686dac.js
--rw-rw-r--   0 alino     (1000) alino     (1000)     1183 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/service-worker.js
-drwxrwxr-x   0 alino     (1000) alino     (1000)        0 2023-03-28 19:55:44.133236 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/
-drwxrwxr-x   0 alino     (1000) alino     (1000)        0 2023-03-28 19:55:44.137236 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/css/
--rw-rw-r--   0 alino     (1000) alino     (1000)    25275 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/css/2.95a91b17.chunk.css
--rw-rw-r--   0 alino     (1000) alino     (1000)    30768 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/css/2.95a91b17.chunk.css.map
-drwxrwxr-x   0 alino     (1000) alino     (1000)        0 2023-03-28 19:55:44.141236 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/js/
--rw-rw-r--   0 alino     (1000) alino     (1000)  1608806 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/js/2.e1848dfc.chunk.js
--rw-rw-r--   0 alino     (1000) alino     (1000)     2015 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/js/2.e1848dfc.chunk.js.LICENSE.txt
--rw-rw-r--   0 alino     (1000) alino     (1000)  5402535 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/js/2.e1848dfc.chunk.js.map
--rw-rw-r--   0 alino     (1000) alino     (1000)     2073 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/js/main.87350243.chunk.js
--rw-rw-r--   0 alino     (1000) alino     (1000)     5399 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/js/main.87350243.chunk.js.map
--rw-rw-r--   0 alino     (1000) alino     (1000)     1598 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/js/runtime-main.11ec9aca.js
--rw-rw-r--   0 alino     (1000) alino     (1000)     8317 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/js/runtime-main.11ec9aca.js.map
-drwxrwxr-x   0 alino     (1000) alino     (1000)        0 2023-03-28 19:55:44.149236 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/
--rw-rw-r--   0 alino     (1000) alino     (1000)    33516 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_AMS-Regular.10824af7.woff
--rw-rw-r--   0 alino     (1000) alino     (1000)    63632 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_AMS-Regular.56573229.ttf
--rw-rw-r--   0 alino     (1000) alino     (1000)    28076 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_AMS-Regular.66c67820.woff2
--rw-rw-r--   0 alino     (1000) alino     (1000)    12368 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Caligraphic-Bold.497bf407.ttf
--rw-rw-r--   0 alino     (1000) alino     (1000)     6912 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Caligraphic-Bold.a9e9b095.woff2
--rw-rw-r--   0 alino     (1000) alino     (1000)     7716 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Caligraphic-Bold.de2ba279.woff
--rw-rw-r--   0 alino     (1000) alino     (1000)     6908 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Caligraphic-Regular.08d95d99.woff2
--rw-rw-r--   0 alino     (1000) alino     (1000)     7656 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Caligraphic-Regular.a25140fb.woff
--rw-rw-r--   0 alino     (1000) alino     (1000)    12344 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Caligraphic-Regular.e6fb499f.ttf
--rw-rw-r--   0 alino     (1000) alino     (1000)    13296 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Fraktur-Bold.40934fc0.woff
--rw-rw-r--   0 alino     (1000) alino     (1000)    11348 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Fraktur-Bold.796f3797.woff2
--rw-rw-r--   0 alino     (1000) alino     (1000)    19584 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Fraktur-Bold.b9d7c449.ttf
--rw-rw-r--   0 alino     (1000) alino     (1000)    19572 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Fraktur-Regular.97a699d8.ttf
--rw-rw-r--   0 alino     (1000) alino     (1000)    13208 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Fraktur-Regular.e435cda5.woff
--rw-rw-r--   0 alino     (1000) alino     (1000)    11316 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Fraktur-Regular.f9e6a99f.woff2
--rw-rw-r--   0 alino     (1000) alino     (1000)    29912 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-Bold.4cdba646.woff
--rw-rw-r--   0 alino     (1000) alino     (1000)    51336 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-Bold.8e431f7e.ttf
--rw-rw-r--   0 alino     (1000) alino     (1000)    25324 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-Bold.a9382e25.woff2
--rw-rw-r--   0 alino     (1000) alino     (1000)    32968 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-BoldItalic.52fb39b0.ttf
--rw-rw-r--   0 alino     (1000) alino     (1000)    19412 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-BoldItalic.5f875f98.woff
--rw-rw-r--   0 alino     (1000) alino     (1000)    16780 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-BoldItalic.d8737343.woff2
--rw-rw-r--   0 alino     (1000) alino     (1000)    33580 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-Italic.39349e0a.ttf
--rw-rw-r--   0 alino     (1000) alino     (1000)    16988 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-Italic.65297062.woff2
--rw-rw-r--   0 alino     (1000) alino     (1000)    19676 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-Italic.8ffd28f6.woff
--rw-rw-r--   0 alino     (1000) alino     (1000)    53580 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-Regular.818582da.ttf
--rw-rw-r--   0 alino     (1000) alino     (1000)    30772 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-Regular.f1cdb692.woff
--rw-rw-r--   0 alino     (1000) alino     (1000)    26272 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-Regular.f8a7f19f.woff2
--rw-rw-r--   0 alino     (1000) alino     (1000)    16400 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Math-BoldItalic.1320454d.woff2
--rw-rw-r--   0 alino     (1000) alino     (1000)    18668 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Math-BoldItalic.48155e43.woff
--rw-rw-r--   0 alino     (1000) alino     (1000)    31196 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Math-BoldItalic.6589c4f1.ttf
--rw-rw-r--   0 alino     (1000) alino     (1000)    16440 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Math-Italic.d8b7a801.woff2
--rw-rw-r--   0 alino     (1000) alino     (1000)    18748 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Math-Italic.ed7aea12.woff
--rw-rw-r--   0 alino     (1000) alino     (1000)    31308 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Math-Italic.fe5ed587.ttf
--rw-rw-r--   0 alino     (1000) alino     (1000)    14408 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_SansSerif-Bold.0e897d27.woff
--rw-rw-r--   0 alino     (1000) alino     (1000)    12216 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_SansSerif-Bold.ad546b47.woff2
--rw-rw-r--   0 alino     (1000) alino     (1000)    24504 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_SansSerif-Bold.f2ac7312.ttf
--rw-rw-r--   0 alino     (1000) alino     (1000)    12028 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_SansSerif-Italic.e934cbc8.woff2
--rw-rw-r--   0 alino     (1000) alino     (1000)    14112 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_SansSerif-Italic.ef725de5.woff
--rw-rw-r--   0 alino     (1000) alino     (1000)    22364 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_SansSerif-Italic.f60b4a34.ttf
--rw-rw-r--   0 alino     (1000) alino     (1000)    10344 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_SansSerif-Regular.1ac3ed6e.woff2
--rw-rw-r--   0 alino     (1000) alino     (1000)    19436 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_SansSerif-Regular.3243452e.ttf
--rw-rw-r--   0 alino     (1000) alino     (1000)    12316 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_SansSerif-Regular.5f8637ee.woff
--rw-rw-r--   0 alino     (1000) alino     (1000)     9644 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Script-Regular.1b3161eb.woff2
--rw-rw-r--   0 alino     (1000) alino     (1000)    16648 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Script-Regular.a189c37d.ttf
--rw-rw-r--   0 alino     (1000) alino     (1000)    10588 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Script-Regular.a82fa2a7.woff
--rw-rw-r--   0 alino     (1000) alino     (1000)    12228 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Size1-Regular.0d8d9204.ttf
--rw-rw-r--   0 alino     (1000) alino     (1000)     6496 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Size1-Regular.4788ba5b.woff
--rw-rw-r--   0 alino     (1000) alino     (1000)     5468 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Size1-Regular.82ef26dc.woff2
--rw-rw-r--   0 alino     (1000) alino     (1000)    11508 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Size2-Regular.1fdda0e5.ttf
--rw-rw-r--   0 alino     (1000) alino     (1000)     5208 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Size2-Regular.95a1da91.woff2
--rw-rw-r--   0 alino     (1000) alino     (1000)     6188 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Size2-Regular.b0628bfd.woff
--rw-rw-r--   0 alino     (1000) alino     (1000)     4420 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Size3-Regular.4de844d4.woff
--rw-rw-r--   0 alino     (1000) alino     (1000)     3624 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Size3-Regular.9108a400.woff2
--rw-rw-r--   0 alino     (1000) alino     (1000)     7588 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Size3-Regular.963af864.ttf
--rw-rw-r--   0 alino     (1000) alino     (1000)    10364 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Size4-Regular.27a23ee6.ttf
--rw-rw-r--   0 alino     (1000) alino     (1000)     5980 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Size4-Regular.3045a61f.woff
--rw-rw-r--   0 alino     (1000) alino     (1000)     4928 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Size4-Regular.61522cd3.woff2
--rw-rw-r--   0 alino     (1000) alino     (1000)    16028 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Typewriter-Regular.0e046058.woff
--rw-rw-r--   0 alino     (1000) alino     (1000)    27556 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Typewriter-Regular.6bf42875.ttf
--rw-rw-r--   0 alino     (1000) alino     (1000)    13568 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Typewriter-Regular.b8b8393d.woff2
-drwxrwxr-x   0 alino     (1000) alino     (1000)        0 2023-03-28 19:55:44.133236 streamlit-chat-media-0.0.3/streamlit_chat_media.egg-info/
--rw-rw-r--   0 alino     (1000) alino     (1000)     4183 2023-03-28 19:55:44.000000 streamlit-chat-media-0.0.3/streamlit_chat_media.egg-info/PKG-INFO
--rw-rw-r--   0 alino     (1000) alino     (1000)     6322 2023-03-28 19:55:44.000000 streamlit-chat-media-0.0.3/streamlit_chat_media.egg-info/SOURCES.txt
--rw-rw-r--   0 alino     (1000) alino     (1000)        1 2023-03-28 19:55:44.000000 streamlit-chat-media-0.0.3/streamlit_chat_media.egg-info/dependency_links.txt
--rw-rw-r--   0 alino     (1000) alino     (1000)       16 2023-03-28 19:55:44.000000 streamlit-chat-media-0.0.3/streamlit_chat_media.egg-info/requires.txt
--rw-rw-r--   0 alino     (1000) alino     (1000)       21 2023-03-28 19:55:44.000000 streamlit-chat-media-0.0.3/streamlit_chat_media.egg-info/top_level.txt
+drwxrwxr-x   0 alino     (1000) alino     (1000)        0 2023-04-19 09:06:06.691706 streamlit-chat-media-0.0.4/
+-rw-rw-r--   0 alino     (1000) alino     (1000)     1064 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/LICENSE
+-rw-rw-r--   0 alino     (1000) alino     (1000)       56 2023-03-28 15:21:06.000000 streamlit-chat-media-0.0.4/MANIFEST.in
+-rw-rw-r--   0 alino     (1000) alino     (1000)     4183 2023-04-19 09:06:06.691706 streamlit-chat-media-0.0.4/PKG-INFO
+-rw-rw-r--   0 alino     (1000) alino     (1000)     3687 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/README.md
+-rw-rw-r--   0 alino     (1000) alino     (1000)       38 2023-04-19 09:06:06.691706 streamlit-chat-media-0.0.4/setup.cfg
+-rw-rw-r--   0 alino     (1000) alino     (1000)      953 2023-04-19 09:02:19.000000 streamlit-chat-media-0.0.4/setup.py
+drwxrwxr-x   0 alino     (1000) alino     (1000)        0 2023-04-19 09:06:06.631707 streamlit-chat-media-0.0.4/streamlit_chat_media/
+-rw-rw-r--   0 alino     (1000) alino     (1000)     3485 2023-03-28 15:21:37.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/__init__.py
+drwxrwxr-x   0 alino     (1000) alino     (1000)        0 2023-04-19 09:06:06.631707 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/
+drwxrwxr-x   0 alino     (1000) alino     (1000)        0 2023-04-19 09:06:06.675706 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/
+-rw-rw-r--   0 alino     (1000) alino     (1000)     1150 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/asset-manifest.json
+-rw-rw-r--   0 alino     (1000) alino     (1000)   197459 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/bootstrap.min.css
+-rw-rw-r--   0 alino     (1000) alino     (1000)   646432 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/bootstrap.min.css.map
+-rw-rw-r--   0 alino     (1000) alino     (1000)     2209 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/index.html
+-rw-rw-r--   0 alino     (1000) alino     (1000)     8091 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/precache-manifest.c29a79fbc77e2c50510d007756686dac.js
+-rw-rw-r--   0 alino     (1000) alino     (1000)     1183 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/service-worker.js
+drwxrwxr-x   0 alino     (1000) alino     (1000)        0 2023-04-19 09:06:06.631707 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/
+drwxrwxr-x   0 alino     (1000) alino     (1000)        0 2023-04-19 09:06:06.675706 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/css/
+-rw-rw-r--   0 alino     (1000) alino     (1000)    25275 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/css/2.95a91b17.chunk.css
+-rw-rw-r--   0 alino     (1000) alino     (1000)    30768 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/css/2.95a91b17.chunk.css.map
+drwxrwxr-x   0 alino     (1000) alino     (1000)        0 2023-04-19 09:06:06.683706 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/js/
+-rw-rw-r--   0 alino     (1000) alino     (1000)  1608806 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/js/2.e1848dfc.chunk.js
+-rw-rw-r--   0 alino     (1000) alino     (1000)     2015 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/js/2.e1848dfc.chunk.js.LICENSE.txt
+-rw-rw-r--   0 alino     (1000) alino     (1000)  5402535 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/js/2.e1848dfc.chunk.js.map
+-rw-rw-r--   0 alino     (1000) alino     (1000)     2073 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/js/main.87350243.chunk.js
+-rw-rw-r--   0 alino     (1000) alino     (1000)     5399 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/js/main.87350243.chunk.js.map
+-rw-rw-r--   0 alino     (1000) alino     (1000)     1598 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/js/runtime-main.11ec9aca.js
+-rw-rw-r--   0 alino     (1000) alino     (1000)     8317 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/js/runtime-main.11ec9aca.js.map
+drwxrwxr-x   0 alino     (1000) alino     (1000)        0 2023-04-19 09:06:06.691706 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/
+-rw-rw-r--   0 alino     (1000) alino     (1000)    33516 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_AMS-Regular.10824af7.woff
+-rw-rw-r--   0 alino     (1000) alino     (1000)    63632 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_AMS-Regular.56573229.ttf
+-rw-rw-r--   0 alino     (1000) alino     (1000)    28076 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_AMS-Regular.66c67820.woff2
+-rw-rw-r--   0 alino     (1000) alino     (1000)    12368 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Caligraphic-Bold.497bf407.ttf
+-rw-rw-r--   0 alino     (1000) alino     (1000)     6912 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Caligraphic-Bold.a9e9b095.woff2
+-rw-rw-r--   0 alino     (1000) alino     (1000)     7716 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Caligraphic-Bold.de2ba279.woff
+-rw-rw-r--   0 alino     (1000) alino     (1000)     6908 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Caligraphic-Regular.08d95d99.woff2
+-rw-rw-r--   0 alino     (1000) alino     (1000)     7656 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Caligraphic-Regular.a25140fb.woff
+-rw-rw-r--   0 alino     (1000) alino     (1000)    12344 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Caligraphic-Regular.e6fb499f.ttf
+-rw-rw-r--   0 alino     (1000) alino     (1000)    13296 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Fraktur-Bold.40934fc0.woff
+-rw-rw-r--   0 alino     (1000) alino     (1000)    11348 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Fraktur-Bold.796f3797.woff2
+-rw-rw-r--   0 alino     (1000) alino     (1000)    19584 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Fraktur-Bold.b9d7c449.ttf
+-rw-rw-r--   0 alino     (1000) alino     (1000)    19572 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Fraktur-Regular.97a699d8.ttf
+-rw-rw-r--   0 alino     (1000) alino     (1000)    13208 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Fraktur-Regular.e435cda5.woff
+-rw-rw-r--   0 alino     (1000) alino     (1000)    11316 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Fraktur-Regular.f9e6a99f.woff2
+-rw-rw-r--   0 alino     (1000) alino     (1000)    29912 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-Bold.4cdba646.woff
+-rw-rw-r--   0 alino     (1000) alino     (1000)    51336 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-Bold.8e431f7e.ttf
+-rw-rw-r--   0 alino     (1000) alino     (1000)    25324 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-Bold.a9382e25.woff2
+-rw-rw-r--   0 alino     (1000) alino     (1000)    32968 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-BoldItalic.52fb39b0.ttf
+-rw-rw-r--   0 alino     (1000) alino     (1000)    19412 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-BoldItalic.5f875f98.woff
+-rw-rw-r--   0 alino     (1000) alino     (1000)    16780 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-BoldItalic.d8737343.woff2
+-rw-rw-r--   0 alino     (1000) alino     (1000)    33580 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-Italic.39349e0a.ttf
+-rw-rw-r--   0 alino     (1000) alino     (1000)    16988 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-Italic.65297062.woff2
+-rw-rw-r--   0 alino     (1000) alino     (1000)    19676 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-Italic.8ffd28f6.woff
+-rw-rw-r--   0 alino     (1000) alino     (1000)    53580 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-Regular.818582da.ttf
+-rw-rw-r--   0 alino     (1000) alino     (1000)    30772 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-Regular.f1cdb692.woff
+-rw-rw-r--   0 alino     (1000) alino     (1000)    26272 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-Regular.f8a7f19f.woff2
+-rw-rw-r--   0 alino     (1000) alino     (1000)    16400 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Math-BoldItalic.1320454d.woff2
+-rw-rw-r--   0 alino     (1000) alino     (1000)    18668 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Math-BoldItalic.48155e43.woff
+-rw-rw-r--   0 alino     (1000) alino     (1000)    31196 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Math-BoldItalic.6589c4f1.ttf
+-rw-rw-r--   0 alino     (1000) alino     (1000)    16440 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Math-Italic.d8b7a801.woff2
+-rw-rw-r--   0 alino     (1000) alino     (1000)    18748 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Math-Italic.ed7aea12.woff
+-rw-rw-r--   0 alino     (1000) alino     (1000)    31308 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Math-Italic.fe5ed587.ttf
+-rw-rw-r--   0 alino     (1000) alino     (1000)    14408 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_SansSerif-Bold.0e897d27.woff
+-rw-rw-r--   0 alino     (1000) alino     (1000)    12216 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_SansSerif-Bold.ad546b47.woff2
+-rw-rw-r--   0 alino     (1000) alino     (1000)    24504 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_SansSerif-Bold.f2ac7312.ttf
+-rw-rw-r--   0 alino     (1000) alino     (1000)    12028 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_SansSerif-Italic.e934cbc8.woff2
+-rw-rw-r--   0 alino     (1000) alino     (1000)    14112 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_SansSerif-Italic.ef725de5.woff
+-rw-rw-r--   0 alino     (1000) alino     (1000)    22364 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_SansSerif-Italic.f60b4a34.ttf
+-rw-rw-r--   0 alino     (1000) alino     (1000)    10344 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_SansSerif-Regular.1ac3ed6e.woff2
+-rw-rw-r--   0 alino     (1000) alino     (1000)    19436 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_SansSerif-Regular.3243452e.ttf
+-rw-rw-r--   0 alino     (1000) alino     (1000)    12316 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_SansSerif-Regular.5f8637ee.woff
+-rw-rw-r--   0 alino     (1000) alino     (1000)     9644 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Script-Regular.1b3161eb.woff2
+-rw-rw-r--   0 alino     (1000) alino     (1000)    16648 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Script-Regular.a189c37d.ttf
+-rw-rw-r--   0 alino     (1000) alino     (1000)    10588 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Script-Regular.a82fa2a7.woff
+-rw-rw-r--   0 alino     (1000) alino     (1000)    12228 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Size1-Regular.0d8d9204.ttf
+-rw-rw-r--   0 alino     (1000) alino     (1000)     6496 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Size1-Regular.4788ba5b.woff
+-rw-rw-r--   0 alino     (1000) alino     (1000)     5468 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Size1-Regular.82ef26dc.woff2
+-rw-rw-r--   0 alino     (1000) alino     (1000)    11508 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Size2-Regular.1fdda0e5.ttf
+-rw-rw-r--   0 alino     (1000) alino     (1000)     5208 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Size2-Regular.95a1da91.woff2
+-rw-rw-r--   0 alino     (1000) alino     (1000)     6188 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Size2-Regular.b0628bfd.woff
+-rw-rw-r--   0 alino     (1000) alino     (1000)     4420 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Size3-Regular.4de844d4.woff
+-rw-rw-r--   0 alino     (1000) alino     (1000)     3624 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Size3-Regular.9108a400.woff2
+-rw-rw-r--   0 alino     (1000) alino     (1000)     7588 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Size3-Regular.963af864.ttf
+-rw-rw-r--   0 alino     (1000) alino     (1000)    10364 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Size4-Regular.27a23ee6.ttf
+-rw-rw-r--   0 alino     (1000) alino     (1000)     5980 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Size4-Regular.3045a61f.woff
+-rw-rw-r--   0 alino     (1000) alino     (1000)     4928 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Size4-Regular.61522cd3.woff2
+-rw-rw-r--   0 alino     (1000) alino     (1000)    16028 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Typewriter-Regular.0e046058.woff
+-rw-rw-r--   0 alino     (1000) alino     (1000)    27556 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Typewriter-Regular.6bf42875.ttf
+-rw-rw-r--   0 alino     (1000) alino     (1000)    13568 2023-03-13 09:56:49.000000 streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Typewriter-Regular.b8b8393d.woff2
+drwxrwxr-x   0 alino     (1000) alino     (1000)        0 2023-04-19 09:06:06.675706 streamlit-chat-media-0.0.4/streamlit_chat_media.egg-info/
+-rw-rw-r--   0 alino     (1000) alino     (1000)     4183 2023-04-19 09:06:06.000000 streamlit-chat-media-0.0.4/streamlit_chat_media.egg-info/PKG-INFO
+-rw-rw-r--   0 alino     (1000) alino     (1000)     6322 2023-04-19 09:06:06.000000 streamlit-chat-media-0.0.4/streamlit_chat_media.egg-info/SOURCES.txt
+-rw-rw-r--   0 alino     (1000) alino     (1000)        1 2023-04-19 09:06:06.000000 streamlit-chat-media-0.0.4/streamlit_chat_media.egg-info/dependency_links.txt
+-rw-rw-r--   0 alino     (1000) alino     (1000)       16 2023-04-19 09:06:06.000000 streamlit-chat-media-0.0.4/streamlit_chat_media.egg-info/requires.txt
+-rw-rw-r--   0 alino     (1000) alino     (1000)       21 2023-04-19 09:06:06.000000 streamlit-chat-media-0.0.4/streamlit_chat_media.egg-info/top_level.txt
```

### Comparing `streamlit-chat-media-0.0.3/LICENSE` & `streamlit-chat-media-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/PKG-INFO` & `streamlit-chat-media-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-chat-media
-Version: 0.0.3
+Version: 0.0.4
 Summary: A streamlit component, to make chatbots with media support
 Home-page: https://github.com/AI-Yash/st-chat
 Author: Intelligenza Artificiale Italia
 Author-email: ceo@intelligenzaartificialeitalia.net
 Keywords: chat streamlit streamlit-component
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `streamlit-chat-media-0.0.3/README.md` & `streamlit-chat-media-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/setup.py` & `streamlit-chat-media-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 setuptools.setup(
     name="streamlit-chat-media",
-    version="0.0.3",
+    version="0.0.4",
     author="Intelligenza Artificiale Italia",
     author_email="ceo@intelligenzaartificialeitalia.net",
     description="A streamlit component, to make chatbots with media support",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/AI-Yash/st-chat",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/__init__.py` & `streamlit-chat-media-0.0.4/streamlit_chat_media/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/asset-manifest.json` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/bootstrap.min.css` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/bootstrap.min.css.map` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/index.html` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/precache-manifest.c29a79fbc77e2c50510d007756686dac.js` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/precache-manifest.c29a79fbc77e2c50510d007756686dac.js`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/service-worker.js` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/service-worker.js`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/css/2.95a91b17.chunk.css` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/css/2.95a91b17.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/css/2.95a91b17.chunk.css.map` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/css/2.95a91b17.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/js/2.e1848dfc.chunk.js` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/js/2.e1848dfc.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/js/2.e1848dfc.chunk.js.LICENSE.txt` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/js/2.e1848dfc.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/js/2.e1848dfc.chunk.js.map` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/js/2.e1848dfc.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/js/main.87350243.chunk.js` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/js/main.87350243.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/js/main.87350243.chunk.js.map` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/js/main.87350243.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/js/runtime-main.11ec9aca.js` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/js/runtime-main.11ec9aca.js`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/js/runtime-main.11ec9aca.js.map` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/js/runtime-main.11ec9aca.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_AMS-Regular.10824af7.woff` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_AMS-Regular.10824af7.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_AMS-Regular.56573229.ttf` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_AMS-Regular.56573229.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_AMS-Regular.66c67820.woff2` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_AMS-Regular.66c67820.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Caligraphic-Bold.497bf407.ttf` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Caligraphic-Bold.497bf407.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Caligraphic-Bold.a9e9b095.woff2` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Caligraphic-Bold.a9e9b095.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Caligraphic-Bold.de2ba279.woff` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Caligraphic-Bold.de2ba279.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Caligraphic-Regular.08d95d99.woff2` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Caligraphic-Regular.08d95d99.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Caligraphic-Regular.a25140fb.woff` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Caligraphic-Regular.a25140fb.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Caligraphic-Regular.e6fb499f.ttf` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Caligraphic-Regular.e6fb499f.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Fraktur-Bold.40934fc0.woff` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Fraktur-Bold.40934fc0.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Fraktur-Bold.796f3797.woff2` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Fraktur-Bold.796f3797.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Fraktur-Bold.b9d7c449.ttf` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Fraktur-Bold.b9d7c449.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Fraktur-Regular.97a699d8.ttf` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Fraktur-Regular.97a699d8.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Fraktur-Regular.e435cda5.woff` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Fraktur-Regular.e435cda5.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Fraktur-Regular.f9e6a99f.woff2` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Fraktur-Regular.f9e6a99f.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-Bold.4cdba646.woff` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-Bold.4cdba646.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-Bold.8e431f7e.ttf` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-Bold.8e431f7e.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-Bold.a9382e25.woff2` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-Bold.a9382e25.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-BoldItalic.52fb39b0.ttf` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-BoldItalic.52fb39b0.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-BoldItalic.5f875f98.woff` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-BoldItalic.5f875f98.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-BoldItalic.d8737343.woff2` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-BoldItalic.d8737343.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-Italic.39349e0a.ttf` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-Italic.39349e0a.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-Italic.65297062.woff2` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-Italic.65297062.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-Italic.8ffd28f6.woff` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-Italic.8ffd28f6.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-Regular.818582da.ttf` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-Regular.818582da.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-Regular.f1cdb692.woff` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-Regular.f1cdb692.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-Regular.f8a7f19f.woff2` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Main-Regular.f8a7f19f.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Math-BoldItalic.1320454d.woff2` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Math-BoldItalic.1320454d.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Math-BoldItalic.48155e43.woff` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Math-BoldItalic.48155e43.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Math-BoldItalic.6589c4f1.ttf` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Math-BoldItalic.6589c4f1.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Math-Italic.d8b7a801.woff2` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Math-Italic.d8b7a801.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Math-Italic.ed7aea12.woff` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Math-Italic.ed7aea12.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Math-Italic.fe5ed587.ttf` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Math-Italic.fe5ed587.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_SansSerif-Bold.0e897d27.woff` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_SansSerif-Bold.0e897d27.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_SansSerif-Bold.ad546b47.woff2` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_SansSerif-Bold.ad546b47.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_SansSerif-Bold.f2ac7312.ttf` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_SansSerif-Bold.f2ac7312.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_SansSerif-Italic.e934cbc8.woff2` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_SansSerif-Italic.e934cbc8.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_SansSerif-Italic.ef725de5.woff` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_SansSerif-Italic.ef725de5.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_SansSerif-Italic.f60b4a34.ttf` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_SansSerif-Italic.f60b4a34.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_SansSerif-Regular.1ac3ed6e.woff2` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_SansSerif-Regular.1ac3ed6e.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_SansSerif-Regular.3243452e.ttf` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_SansSerif-Regular.3243452e.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_SansSerif-Regular.5f8637ee.woff` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_SansSerif-Regular.5f8637ee.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Script-Regular.1b3161eb.woff2` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Script-Regular.1b3161eb.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Script-Regular.a189c37d.ttf` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Script-Regular.a189c37d.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Script-Regular.a82fa2a7.woff` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Script-Regular.a82fa2a7.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Size1-Regular.0d8d9204.ttf` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Size1-Regular.0d8d9204.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Size1-Regular.4788ba5b.woff` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Size1-Regular.4788ba5b.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Size1-Regular.82ef26dc.woff2` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Size1-Regular.82ef26dc.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Size2-Regular.1fdda0e5.ttf` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Size2-Regular.1fdda0e5.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Size2-Regular.95a1da91.woff2` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Size2-Regular.95a1da91.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Size2-Regular.b0628bfd.woff` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Size2-Regular.b0628bfd.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Size3-Regular.4de844d4.woff` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Size3-Regular.4de844d4.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Size3-Regular.9108a400.woff2` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Size3-Regular.9108a400.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Size3-Regular.963af864.ttf` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Size3-Regular.963af864.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Size4-Regular.27a23ee6.ttf` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Size4-Regular.27a23ee6.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Size4-Regular.3045a61f.woff` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Size4-Regular.3045a61f.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Size4-Regular.61522cd3.woff2` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Size4-Regular.61522cd3.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Typewriter-Regular.0e046058.woff` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Typewriter-Regular.0e046058.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Typewriter-Regular.6bf42875.ttf` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Typewriter-Regular.6bf42875.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media/frontend/build/static/media/KaTeX_Typewriter-Regular.b8b8393d.woff2` & `streamlit-chat-media-0.0.4/streamlit_chat_media/frontend/build/static/media/KaTeX_Typewriter-Regular.b8b8393d.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media.egg-info/PKG-INFO` & `streamlit-chat-media-0.0.4/streamlit_chat_media.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-chat-media
-Version: 0.0.3
+Version: 0.0.4
 Summary: A streamlit component, to make chatbots with media support
 Home-page: https://github.com/AI-Yash/st-chat
 Author: Intelligenza Artificiale Italia
 Author-email: ceo@intelligenzaartificialeitalia.net
 Keywords: chat streamlit streamlit-component
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `streamlit-chat-media-0.0.3/streamlit_chat_media.egg-info/SOURCES.txt` & `streamlit-chat-media-0.0.4/streamlit_chat_media.egg-info/SOURCES.txt`

 * *Files identical despite different names*


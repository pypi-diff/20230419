# Comparing `tmp/xiaogpt-1.40.tar.gz` & `tmp/xiaogpt-1.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiaogpt-1.40.tar", last modified: Fri Apr  7 11:13:57 2023, max compression
+gzip compressed data, was "xiaogpt-1.41.tar", last modified: Wed Apr 19 13:22:54 2023, max compression
```

## Comparing `xiaogpt-1.40.tar` & `xiaogpt-1.41.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1063 2023-04-07 11:13:49.171552 xiaogpt-1.40/LICENSE
--rw-r--r--   0        0        0    10532 2023-04-07 11:13:49.171552 xiaogpt-1.40/README.md
--rw-r--r--   0        0        0      911 2023-04-07 11:13:57.739975 xiaogpt-1.40/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-07 11:13:49.171552 xiaogpt-1.40/xiaogpt/__init__.py
--rw-r--r--   0        0        0       61 2023-04-07 11:13:49.171552 xiaogpt-1.40/xiaogpt/__main__.py
--rw-r--r--   0        0        0      189 2023-04-07 11:13:49.171552 xiaogpt-1.40/xiaogpt/bot/__init__.py
--rw-r--r--   0        0        0      218 2023-04-07 11:13:49.171552 xiaogpt-1.40/xiaogpt/bot/base_bot.py
--rw-r--r--   0        0        0     2325 2023-04-07 11:13:49.171552 xiaogpt-1.40/xiaogpt/bot/chatgptapi_bot.py
--rw-r--r--   0        0        0     1386 2023-04-07 11:13:49.171552 xiaogpt-1.40/xiaogpt/bot/gpt3_bot.py
--rw-r--r--   0        0        0     1732 2023-04-07 11:13:49.171552 xiaogpt-1.40/xiaogpt/bot/newbing_bot.py
--rw-r--r--   0        0        0     3000 2023-04-07 11:13:49.171552 xiaogpt-1.40/xiaogpt/cli.py
--rw-r--r--   0        0        0     4771 2023-04-07 11:13:49.171552 xiaogpt-1.40/xiaogpt/config.py
--rw-r--r--   0        0        0     1991 2023-04-07 11:13:49.171552 xiaogpt-1.40/xiaogpt/utils.py
--rw-r--r--   0        0        0    18767 2023-04-07 11:13:49.171552 xiaogpt-1.40/xiaogpt/xiaogpt.py
--rw-r--r--   0        0        0    11110 1970-01-01 00:00:00.000000 xiaogpt-1.40/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-04-19 13:22:43.233904 xiaogpt-1.41/LICENSE
+-rw-r--r--   0        0        0    11110 2023-04-19 13:22:43.233904 xiaogpt-1.41/README.md
+-rw-r--r--   0        0        0      911 2023-04-19 13:22:54.113975 xiaogpt-1.41/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-19 13:22:43.237905 xiaogpt-1.41/xiaogpt/__init__.py
+-rw-r--r--   0        0        0       61 2023-04-19 13:22:43.237905 xiaogpt-1.41/xiaogpt/__main__.py
+-rw-r--r--   0        0        0      189 2023-04-19 13:22:43.237905 xiaogpt-1.41/xiaogpt/bot/__init__.py
+-rw-r--r--   0        0        0      218 2023-04-19 13:22:43.237905 xiaogpt-1.41/xiaogpt/bot/base_bot.py
+-rw-r--r--   0        0        0     2895 2023-04-19 13:22:43.237905 xiaogpt-1.41/xiaogpt/bot/chatgptapi_bot.py
+-rw-r--r--   0        0        0     1386 2023-04-19 13:22:43.237905 xiaogpt-1.41/xiaogpt/bot/gpt3_bot.py
+-rw-r--r--   0        0        0     1732 2023-04-19 13:22:43.237905 xiaogpt-1.41/xiaogpt/bot/newbing_bot.py
+-rw-r--r--   0        0        0     3415 2023-04-19 13:22:43.237905 xiaogpt-1.41/xiaogpt/cli.py
+-rw-r--r--   0        0        0     5263 2023-04-19 13:22:43.237905 xiaogpt-1.41/xiaogpt/config.py
+-rw-r--r--   0        0        0     1991 2023-04-19 13:22:43.237905 xiaogpt-1.41/xiaogpt/utils.py
+-rw-r--r--   0        0        0    19359 2023-04-19 13:22:43.237905 xiaogpt-1.41/xiaogpt/xiaogpt.py
+-rw-r--r--   0        0        0    11688 1970-01-01 00:00:00.000000 xiaogpt-1.41/PKG-INFO
```

### Comparing `xiaogpt-1.40/LICENSE` & `xiaogpt-1.41/LICENSE`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.40/README.md` & `xiaogpt-1.41/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -134,14 +134,16 @@
 | start_conversation    | 开始持续对话关键词                                | `开始持续对话`                      |
 | end_conversation      | 结束持续对话关键词                                | `结束持续对话`                      |
 | stream                | 使用流式响应，获得更快的响应                      | `false`                             |
 | proxy                 | 支持 HTTP 代理，传入 http proxy URL               | ""                                  |
 | gpt_options           | OpenAI API 的参数字典                             | `{}`                                |
 | bing_cookie_path      | NewBing使用的cookie路径，参考[这里]获取           | 也可通过环境变量 `COOKIE_FILE` 设置 |
 | bing_cookies          | NewBing使用的cookie字典，参考[这里]获取           |                                     |
+| deployment_id         | Azure OpenAI 服务的 deployment ID                 |                                     |
+| localhost             | 是否通过本地服务器加载EdgeTTS的音频输出           | `true`                              |
 
 [这里]: https://github.com/acheong08/EdgeGPT#getting-authentication-required
 
 ## 注意
 
 1. 请开启小爱同学的蓝牙
 2. 如果要更改提示词和 PROMPT 在代码最上面自行更改
@@ -211,17 +213,20 @@
 
 ```shell
 docker run -v <your-config-dir>:/config yihong0618/xiaogpt -p 9527:9527 -e XIAOGPT_HOSTNAME=<your ip> --config=/config/config.json
 ```
 
 注意端口必须映射为与容器内一致，XIAOGPT_HOSTNAME 需要设置为宿主机的 IP 地址，否则小爱无法正常播放语音。
 
+如果不想使用本地的HTTP服务器，可以将配置中的 `localhost` 设置为 `false`，这样 Edge TTS 会通过一个网络上的三方服务器加载输出音频文件，但是这样会导致响应速度变慢。
+
 ## 推荐的 fork
 
 - [MIGPT](https://github.com/Afool4U/MIGPT) -> 基于 API 流式对话的低延迟版MIGPT
+- [XiaoBot](https://github.com/longbai/xiaobot) -> Go语言版本的Fork, 带支持不同平台的UI
 
 ## 感谢
 
 - [xiaomi](https://www.mi.com/)
 - [PDM](https://pdm.fming.dev/latest/)
 - @[Yonsm](https://github.com/Yonsm) 的 [MiService](https://github.com/Yonsm/MiService)
 - @[pjq](https://github.com/pjq) 给了这个项目非常多的帮助
```

### Comparing `xiaogpt-1.40/pyproject.toml` & `xiaogpt-1.41/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "openai",
     "aiohttp",
     "rich",
     "edge-tts>=6.1.3",
     "EdgeGPT",
 ]
 dynamic = []
-version = "1.40"
+version = "1.41"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/yihong0618/xiaogpt"
```

### Comparing `xiaogpt-1.40/xiaogpt/bot/gpt3_bot.py` & `xiaogpt-1.41/xiaogpt/bot/gpt3_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.40/xiaogpt/bot/newbing_bot.py` & `xiaogpt-1.41/xiaogpt/bot/newbing_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.40/xiaogpt/cli.py` & `xiaogpt-1.41/xiaogpt/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -109,14 +109,28 @@
     )
     # args to change api_base
     parser.add_argument(
         "--api_base",
         dest="api_base",
         help="specify base url other than the OpenAI's official API address",
     )
+    parser.add_argument(
+        "--no-localhost",
+        dest="localhost",
+        action="store_false",
+        default=None,
+        help="serve Edge TTS output files via internet. "
+        "This is useful when running in a container",
+    )
+
+    parser.add_argument(
+        "--deployment_id",
+        dest="deployment_id",
+        help="specify deployment id, only used when api_base points to azure",
+    )
 
     options = parser.parse_args()
     config = Config.from_options(options)
 
     miboy = MiGPT(config)
     loop = asyncio.get_event_loop()
     loop.run_until_complete(miboy.run_forever())
```

### Comparing `xiaogpt-1.40/xiaogpt/config.py` & `xiaogpt-1.41/xiaogpt/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -64,20 +64,22 @@
     keyword: Iterable[str] = KEY_WORD
     change_prompt_keyword: Iterable[str] = CHANGE_PROMPT_KEY_WORD
     prompt: str = PROMPT
     mute_xiaoai: bool = False
     bot: str = "chatgpt"
     cookie: str = ""
     api_base: str | None = None
+    deployment_id: str | None = None
     use_command: bool = False
     verbose: bool = False
     start_conversation: str = "开始持续对话"
     end_conversation: str = "结束持续对话"
     stream: bool = False
     enable_edge_tts: bool = False
+    localhost: bool = True
     edge_tts_voice: str = "zh-CN-XiaoxiaoNeural"
     gpt_options: dict[str, Any] = field(default_factory=dict)
     bing_cookie_path: str = ""
     bing_cookies: dict | None = None
 
     def __post_init__(self) -> None:
         if self.proxy:
@@ -86,14 +88,23 @@
             if not (self.bing_cookie_path or self.bing_cookies):
                 raise Exception(
                     "New bing bot needs bing_cookie_path or bing_cookies, read this: "
                     "https://github.com/acheong08/EdgeGPT#getting-authentication-required"
                 )
         elif not self.openai_key:
             raise Exception("Using GPT api needs openai API key, please google how to")
+        if (
+            self.api_base
+            and self.api_base.endswith(("openai.azure.com", "openai.azure.com/"))
+            and not self.deployment_id
+        ):
+            raise Exception(
+                "Using Azure OpenAI needs deployment_id, read this: "
+                "https://learn.microsoft.com/en-us/azure/cognitive-services/openai/how-to/chatgpt?pivots=programming-language-chat-completions"
+            )
 
     @property
     def tts_command(self) -> str:
         return HARDWARE_COMMAND_DICT.get(self.hardware, DEFAULT_COMMAND)[0]
 
     @property
     def wakeup_command(self) -> str:
```

### Comparing `xiaogpt-1.40/xiaogpt/utils.py` & `xiaogpt-1.41/xiaogpt/utils.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.40/xiaogpt/xiaogpt.py` & `xiaogpt-1.41/xiaogpt/xiaogpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 #!/usr/bin/env python3
 import asyncio
 import functools
 import http.server
+import io
 import json
 import logging
 import os
 import random
 import re
+import shutil
 import socket
 import socketserver
 import tempfile
 import threading
 import time
 from pathlib import Path
 
@@ -74,14 +76,16 @@
         self.parent_id = None
         self.mina_service = None
         self.miio_service = None
         self.in_conversation = False
         self.polling_event = asyncio.Event()
         self.new_record_event = asyncio.Event()
         self.temp_dir = None
+        if self.config.enable_edge_tts:
+            self.temp_dir = tempfile.TemporaryDirectory(prefix="xiaogpt-tts-")
 
         # setup logger
         self.log = logging.getLogger("xiaogpt")
         self.log.setLevel(logging.DEBUG if config.verbose else logging.INFO)
         self.log.addHandler(RichHandler())
         self.log.debug(config)
 
@@ -101,15 +105,15 @@
                     await asyncio.sleep(1 - d)
 
     async def init_all_data(self, session):
         await self.login_miboy(session)
         await self._init_data_hardware()
         session.cookie_jar.update_cookies(self.get_cookie())
         self.cookie_jar = session.cookie_jar
-        if self.config.enable_edge_tts:
+        if self.config.enable_edge_tts and self.config.localhost:
             self.start_http_server()
 
     async def login_miboy(self, session):
         account = MiAccount(
             session,
             self.config.account,
             self.config.password,
@@ -181,15 +185,18 @@
         if self._chatbot is None:
             if self.config.bot == "gpt3":
                 self._chatbot = GPT3Bot(
                     self.config.openai_key, self.config.api_base, self.config.proxy
                 )
             elif self.config.bot == "chatgptapi":
                 self._chatbot = ChatGPTBot(
-                    self.config.openai_key, self.config.api_base, self.config.proxy
+                    self.config.openai_key,
+                    self.config.api_base,
+                    self.config.proxy,
+                    self.config.deployment_id,
                 )
             elif self.config.bot == "newbing":
                 self._chatbot = NewBingBot(
                     bing_cookie_path=self.config.bing_cookie_path,
                     bing_cookies=self.config.bing_cookies,
                     proxy=self.config.proxy,
                 )
@@ -289,51 +296,59 @@
             await asyncio.sleep(1)
 
     def start_http_server(self):
         # set the port range
         port_range = range(8050, 8090)
         # get a random port from the range
         self.port = int(os.getenv("XIAOGPT_PORT", random.choice(port_range)))
-        self.temp_dir = tempfile.TemporaryDirectory(prefix="xiaogpt-tts-")
         # create the server
         handler = functools.partial(HTTPRequestHandler, directory=self.temp_dir.name)
         httpd = ThreadedHTTPServer(("", self.port), handler)
         # start the server in a new thread
         server_thread = threading.Thread(target=httpd.serve_forever)
         server_thread.daemon = True
         server_thread.start()
 
         self.hostname = get_hostname()
         self.log.info(f"Serving on {self.hostname}:{self.port}")
 
+    async def get_file_url(self, stream):
+        if self.config.localhost:
+            with tempfile.NamedTemporaryFile(
+                "wb", suffix=".mp3", delete=False, dir=self.temp_dir.name
+            ) as f:
+                shutil.copyfileobj(stream, f)
+                return f"http://{self.hostname}:{self.port}/{os.path.basename(f.name)}"
+        async with ClientSession("https://transfer.sh") as session:
+            resp = await session.put(
+                "/edge_tts.mp3", data=stream, proxy=self.config.proxy
+            )
+            return (await resp.text()).strip()
+
     async def text2mp3(self, text, tts_lang):
         communicate = edge_tts.Communicate(text, tts_lang)
         duration = 0
-        with tempfile.NamedTemporaryFile(
-            "wb", suffix=".mp3", delete=False, dir=self.temp_dir.name
-        ) as f:
-            async for chunk in communicate.stream():
-                if chunk["type"] == "audio":
-                    f.write(chunk["data"])
-                elif chunk["type"] == "WordBoundary":
-                    duration = (chunk["offset"] + chunk["duration"]) / 1e7
-            if duration == 0:
-                raise RuntimeError(f"Failed to get tts from edge with voice={tts_lang}")
-            return (
-                f"http://{self.hostname}:{self.port}/{os.path.basename(f.name)}",
-                duration,
-            )
+        stream = io.BytesIO()
+        async for chunk in communicate.stream():
+            if chunk["type"] == "audio":
+                stream.write(chunk["data"])
+            elif chunk["type"] == "WordBoundary":
+                duration = (chunk["offset"] + chunk["duration"]) / 1e7
+        if duration == 0:
+            raise RuntimeError(f"Failed to get tts from edge with voice={tts_lang}")
+        stream.seek(0)
+        return (await self.get_file_url(stream), duration)
 
     async def edge_tts(self, text_stream, tts_lang):
         async def run_tts(text_stream, tts_lang, queue):
             async for text in text_stream:
                 try:
                     url, duration = await self.text2mp3(text, tts_lang)
-                except Exception as e:
-                    self.log.error(e)
+                except Exception:
+                    self.log.exception("haha")
                     continue
                 await queue.put((url, duration))
 
         queue = asyncio.Queue()
         self.log.debug("Edge TTS with voice=%s", tts_lang)
         task = asyncio.create_task(run_tts(text_stream, tts_lang, queue))
         task.add_done_callback(lambda _: queue.put_nowait(EOF))
```

### Comparing `xiaogpt-1.40/PKG-INFO` & `xiaogpt-1.41/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xiaogpt
-Version: 1.40
+Version: 1.41
 Summary: Play ChatGPT with xiaomi AI speaker
 Author-Email: yihong0618 <zouzou0208@gmail.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Homepage, https://github.com/yihong0618/xiaogpt
@@ -153,14 +153,16 @@
 | start_conversation    | 开始持续对话关键词                                | `开始持续对话`                      |
 | end_conversation      | 结束持续对话关键词                                | `结束持续对话`                      |
 | stream                | 使用流式响应，获得更快的响应                      | `false`                             |
 | proxy                 | 支持 HTTP 代理，传入 http proxy URL               | ""                                  |
 | gpt_options           | OpenAI API 的参数字典                             | `{}`                                |
 | bing_cookie_path      | NewBing使用的cookie路径，参考[这里]获取           | 也可通过环境变量 `COOKIE_FILE` 设置 |
 | bing_cookies          | NewBing使用的cookie字典，参考[这里]获取           |                                     |
+| deployment_id         | Azure OpenAI 服务的 deployment ID                 |                                     |
+| localhost             | 是否通过本地服务器加载EdgeTTS的音频输出           | `true`                              |
 
 [这里]: https://github.com/acheong08/EdgeGPT#getting-authentication-required
 
 ## 注意
 
 1. 请开启小爱同学的蓝牙
 2. 如果要更改提示词和 PROMPT 在代码最上面自行更改
@@ -230,17 +232,20 @@
 
 ```shell
 docker run -v <your-config-dir>:/config yihong0618/xiaogpt -p 9527:9527 -e XIAOGPT_HOSTNAME=<your ip> --config=/config/config.json
 ```
 
 注意端口必须映射为与容器内一致，XIAOGPT_HOSTNAME 需要设置为宿主机的 IP 地址，否则小爱无法正常播放语音。
 
+如果不想使用本地的HTTP服务器，可以将配置中的 `localhost` 设置为 `false`，这样 Edge TTS 会通过一个网络上的三方服务器加载输出音频文件，但是这样会导致响应速度变慢。
+
 ## 推荐的 fork
 
 - [MIGPT](https://github.com/Afool4U/MIGPT) -> 基于 API 流式对话的低延迟版MIGPT
+- [XiaoBot](https://github.com/longbai/xiaobot) -> Go语言版本的Fork, 带支持不同平台的UI
 
 ## 感谢
 
 - [xiaomi](https://www.mi.com/)
 - [PDM](https://pdm.fming.dev/latest/)
 - @[Yonsm](https://github.com/Yonsm) 的 [MiService](https://github.com/Yonsm/MiService)
 - @[pjq](https://github.com/pjq) 给了这个项目非常多的帮助
```


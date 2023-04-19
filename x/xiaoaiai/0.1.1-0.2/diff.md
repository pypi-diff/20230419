# Comparing `tmp/xiaoaiai-0.1.1.tar.gz` & `tmp/xiaoaiai-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiaoaiai-0.1.1.tar", last modified: Wed Apr 19 11:37:22 2023, max compression
+gzip compressed data, was "xiaoaiai-0.2.tar", last modified: Wed Apr 19 07:41:31 2023, max compression
```

## Comparing `xiaoaiai-0.1.1.tar` & `xiaoaiai-0.2.tar`

### file list

```diff
@@ -1,29 +1,17 @@
--rw-r--r--   0        0        0    48745 2023-04-16 03:22:28.128312 xiaoaiai-0.1.1/ChatGPT/src/revChatGPT/V1.py
--rw-r--r--   0        0        0    23905 2023-04-16 03:11:20.930403 xiaoaiai-0.1.1/ChatGPT/src/revChatGPT/V3.py
--rw-r--r--   0        0        0      923 2023-04-16 03:11:20.931409 xiaoaiai-0.1.1/ChatGPT/src/revChatGPT/__init__.py
--rw-r--r--   0        0        0     1781 2023-04-16 03:11:20.932405 xiaoaiai-0.1.1/ChatGPT/src/revChatGPT/__main__.py
--rw-r--r--   0        0        0     1902 2023-04-10 16:17:01.479787 xiaoaiai-0.1.1/ChatGPT/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0        0        0     5224 2023-04-10 16:17:01.480787 xiaoaiai-0.1.1/ChatGPT/src/revChatGPT/typings.py
--rw-r--r--   0        0        0     2759 2023-04-10 16:17:01.480787 xiaoaiai-0.1.1/ChatGPT/src/revChatGPT/utils.py
--rw-r--r--   0        0        0     1084 2023-04-09 13:37:09.371338 xiaoaiai-0.1.1/LICENSE
--rw-r--r--   0        0        0    11057 2023-04-19 11:15:31.029364 xiaoaiai-0.1.1/README.md
--rw-r--r--   0        0        0      918 2023-04-19 11:37:22.530612 xiaoaiai-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       65 2023-04-09 13:37:09.385334 xiaoaiai-0.1.1/xiaoai/__main__.py
--rw-r--r--   0        0        0       76 2023-04-19 11:23:36.189150 xiaoaiai-0.1.1/xiaoai/cli.py
--rw-r--r--   0        0        0        0 2023-04-09 13:37:09.384335 xiaoaiai-0.1.1/xiaogpt/__init__.py
--rw-r--r--   0        0        0       65 2023-04-09 13:37:09.385334 xiaoaiai-0.1.1/xiaogpt/__main__.py
--rw-r--r--   0        0        0      194 2023-04-09 13:37:09.387334 xiaoaiai-0.1.1/xiaogpt/bot/__init__.py
--rw-r--r--   0        0        0      229 2023-04-09 13:37:09.389338 xiaoaiai-0.1.1/xiaogpt/bot/base_bot.py
--rw-r--r--   0        0        0     2431 2023-04-11 16:27:10.293600 xiaoaiai-0.1.1/xiaogpt/bot/chatgptapi_bot.py
--rw-r--r--   0        0        0     1477 2023-04-11 16:27:10.304602 xiaoaiai-0.1.1/xiaogpt/bot/gpt3_bot.py
--rw-r--r--   0        0        0     2670 2023-04-16 07:37:14.766010 xiaoaiai-0.1.1/xiaogpt/bot/newbing_acheongbot.py
--rw-r--r--   0        0        0     1826 2023-04-11 16:27:10.282598 xiaoaiai-0.1.1/xiaogpt/bot/newbing_bot.py
--rw-r--r--   0        0        0     2296 2023-04-12 12:30:28.200588 xiaoaiai-0.1.1/xiaogpt/bot/revchatgpt_bot.py
--rw-r--r--   0        0        0      599 2023-04-16 07:53:35.887546 xiaoaiai-0.1.1/xiaogpt/bot/stringcontain.py
--rw-r--r--   0        0        0     3515 2023-04-19 11:20:45.756797 xiaoaiai-0.1.1/xiaogpt/cli.py
--rw-r--r--   0        0        0     5121 2023-04-19 11:15:31.038296 xiaoaiai-0.1.1/xiaogpt/config.py
--rw-r--r--   0        0        0     2571 2023-04-16 06:44:38.538674 xiaoaiai-0.1.1/xiaogpt/testwindow.py
--rw-r--r--   0        0        0    12851 2023-04-16 08:07:14.535519 xiaoaiai-0.1.1/xiaogpt/toast.py
--rw-r--r--   0        0        0     2667 2023-04-16 06:10:47.636348 xiaoaiai-0.1.1/xiaogpt/utils.py
--rw-r--r--   0        0        0    32505 2023-04-19 11:20:45.769736 xiaoaiai-0.1.1/xiaogpt/xiaogpt.py
--rw-r--r--   0        0        0    11381 1970-01-01 00:00:00.000000 xiaoaiai-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-04-19 07:41:21.345111 xiaoaiai-0.2/LICENSE
+-rw-r--r--   0        0        0    10817 2023-04-19 07:41:21.345111 xiaoaiai-0.2/README.md
+-rw-r--r--   0        0        0      895 2023-04-19 07:41:31.601407 xiaoaiai-0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-19 07:41:21.349111 xiaoaiai-0.2/xiaogpt/__init__.py
+-rw-r--r--   0        0        0       61 2023-04-19 07:41:21.349111 xiaoaiai-0.2/xiaogpt/__main__.py
+-rw-r--r--   0        0        0      189 2023-04-19 07:41:21.349111 xiaoaiai-0.2/xiaogpt/bot/__init__.py
+-rw-r--r--   0        0        0      218 2023-04-19 07:41:21.349111 xiaoaiai-0.2/xiaogpt/bot/base_bot.py
+-rw-r--r--   0        0        0     2364 2023-04-19 07:41:21.349111 xiaoaiai-0.2/xiaogpt/bot/chatgptapi_bot.py
+-rw-r--r--   0        0        0     1426 2023-04-19 07:41:21.349111 xiaoaiai-0.2/xiaogpt/bot/gpt3_bot.py
+-rw-r--r--   0        0        0     2354 2023-04-19 07:41:21.349111 xiaoaiai-0.2/xiaogpt/bot/newbing_acheongbot.py
+-rw-r--r--   0        0        0     1766 2023-04-19 07:41:21.349111 xiaoaiai-0.2/xiaogpt/bot/newbing_bot.py
+-rw-r--r--   0        0        0     2217 2023-04-19 07:41:21.349111 xiaoaiai-0.2/xiaogpt/bot/revchatgpt_bot.py
+-rw-r--r--   0        0        0     3347 2023-04-19 07:41:21.349111 xiaoaiai-0.2/xiaogpt/cli.py
+-rw-r--r--   0        0        0     4986 2023-04-19 07:41:21.349111 xiaoaiai-0.2/xiaogpt/config.py
+-rw-r--r--   0        0        0     1991 2023-04-19 07:41:21.349111 xiaoaiai-0.2/xiaogpt/utils.py
+-rw-r--r--   0        0        0    25622 2023-04-19 07:41:21.349111 xiaoaiai-0.2/xiaogpt/xiaogpt.py
+-rw-r--r--   0        0        0    11379 1970-01-01 00:00:00.000000 xiaoaiai-0.2/PKG-INFO
```

### Comparing `xiaoaiai-0.1.1/README.md` & `xiaoaiai-0.2/README.md`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,240 +1,240 @@
-# xiaogpt
-
-[![PyPI](https://img.shields.io/pypi/v/xiaogpt?style=flat-square)](https://pypi.org/project/xiaogpt)
-[![Docker Image Version (latest by date)](https://img.shields.io/docker/v/yihong0618/xiaogpt?color=%23086DCD&label=docker%20image)](https://hub.docker.com/r/yihong0618/xiaogpt)
-
-
-https://user-images.githubusercontent.com/15976103/226803357-72f87a41-a15b-409e-94f5-e2d262eecd53.mp4
-
-
-Play ChatGPT with Xiaomi AI Speaker
-
-![image](https://user-images.githubusercontent.com/15976103/220028375-c193a859-48a1-4270-95b6-ef540e54a621.png)
-![image](https://user-images.githubusercontent.com/15976103/226802344-9c71f543-b73c-4a47-8703-4c200c434dec.png)
-
-## 支持的 AI 类型
-
-- GPT3
-- ChatGPT
-- New Bing
-
-## 一点原理
-
-[不用 root 使用小爱同学和 ChatGPT 交互折腾记](https://github.com/yihong0618/gitblog/issues/258)
-
-## 准备
-
-1. ChatGPT id
-2. 小爱音响
-3. 能正常联网的环境或 proxy
-4. python3.8+
-
-## 使用
-
-- `pip install -U --force-reinstall xiaogpt`
-- 参考我 fork 的 [MiService](https://github.com/yihong0618/MiService) 项目 README 并在本地 terminal 跑 `micli list` 拿到你音响的 DID 成功 **别忘了设置 export MI_DID=xxx** 这个 MI_DID 用
-- run `xiaogpt --hardware ${your_hardware} --use_chatgpt_api` hardware 你看小爱屁股上有型号，输入进来，如果在屁股上找不到或者型号不对，可以用 `micli mina` 找到型号
-- 跑起来之后就可以问小爱同学问题了，“帮我"开头的问题，会发送一份给 ChatGPT 然后小爱同学用 tts 回答
-- 如果上面不可用，可以尝试用手机抓包，https://userprofile.mina.mi.com/device_profile/v2/conversation 找到 cookie 利用 `--cookie '${cookie}'` cookie 别忘了用单引号包裹
-- 默认用目前 ubus, 如果你的设备不支持 ubus 可以使用 `--use_command` 来使用 command 来 tts
-- 使用 `--mute_xiaoai` 选项，可以快速停掉小爱的回答
-- 使用 `--account ${account} --password ${password}`
-- 如果有能力可以自行替换唤醒词，也可以去掉唤醒词
-- 使用 `--use_chatgpt_api` 的 api 那样可以更流畅的对话，速度特别快，达到了对话的体验, [openai api](https://platform.openai.com/account/api-keys), 命令 `--use_chatgpt_api`
-- 使用 gpt-3 的 api 那样可以更流畅的对话，速度快, 请 google 如何用 [openai api](https://platform.openai.com/account/api-keys) 命令 --use_gpt3
-- 如果你遇到了墙需要用 Cloudflare Workers 替换 api_base 请使用 `--api_base ${url}` 来替换。  **请注意，此处你输入的api应该是'`https://xxxx/v1`'的字样，域名需要用引号包裹**
-- 可以跟小爱说 `开始持续对话` 自动进入持续对话状态，`结束持续对话` 结束持续对话状态。
-- 可以使用 `--enable_edge_tts` 来获取更好的 tts 能力
-
-e.g.
-
-```shell
-export OPENAI_API_KEY=${your_api_key}
-xiaogpt --hardware LX06 --use_chatgpt_api
-# or
-xiaogpt --hardware LX06 --cookie ${cookie} --use_chatgpt_api
-# 如果你想直接输入账号密码
-xiaogpt --hardware LX06 --account ${your_xiaomi_account} --password ${your_password} --use_chatgpt_api
-# 如果你想 mute 小米的回答
-xiaogpt --hardware LX06  --mute_xiaoai --use_chatgpt_api
-# 使用流式响应，获得更快的响应
-xiaogpt --hardware LX06  --mute_xiaoai --stream
-# 如果你想使用 gpt3 ai
-export OPENAI_API_KEY=${your_api_key}
-xiaogpt --hardware LX06  --mute_xiaoai --use_gpt3
-# 如果你想用 edge-tts
-xiaogpt --hardware LX06 --cookie ${cookie} --use_chatgpt_api --enable_edge_tts
-```
-使用 git clone 运行
-
-```shell
-export OPENAI_API_KEY=${your_api_key}
-python3 loznxiaoai.py --hardware LX06
-# or
-python3 loznxiaoai.py --hardware LX06 --cookie ${cookie}
-# 如果你想直接输入账号密码
-python3 loznxiaoai.py --hardware LX06 --account ${your_xiaomi_account} --password ${your_password} --use_chatgpt_api
-# 如果你想 mute 小米的回答
-python3 loznxiaoai.py --hardware LX06  --mute_xiaoai
-# 使用流式响应，获得更快的响应
-python3 loznxiaoai.py --hardware LX06  --mute_xiaoai --stream
-# 如果你想使用 gpt3 ai
-export OPENAI_API_KEY=${your_api_key}
-python3 loznxiaoai.py --hardware LX06  --mute_xiaoai --use_gpt3
-```
-
-## config.json
-如果想通过单一配置文件启动也是可以的, 可以通过 `--config` 参数指定配置文件, config 文件必须是合法的 JSON 格式
-参数优先级
-- cli args > default > config
-
-```shell
-python3 loznxiaoai.py --config xiao_config.json
-# or
-xiaogpt --config xiao_config.json
-```
-或者
-```shell
-cp xiao_config.json.example xiao_config.json
-python3 loznxiaoai.py
-```
-
-若要指定 OpenAI 的模型参数，如 model, temporature, top_p, 请在config.json中指定：
-
-```json
-{
-    ...
-    "gpt_options": {
-        "temperature": 0.9,
-        "top_p": 0.9,
-    }
-}
-```
-
-具体参数作用请参考 [Open AI API 文档](https://platform.openai.com/docs/api-reference/chat/create)。
-## 配置项说明
-
-| 参数                  | 说明                                              | 默认值                              |
-| --------------------- | ------------------------------------------------- | ----------------------------------- |
-| hardware              | 设备型号                                          |                                     |
-| account               | 小爱账户                                          |                                     |
-| password              | 小爱账户密码                                      |                                     |
-| openai_key            | openai的apikey                                    |                                     |
-| cookie                | 小爱账户cookie （如果用上面密码登录可以不填）     |                                     |
-| mi_did                | 设备did                                           |                                     |
-| use_command           | 使用 MI command 与小爱交互                        | `false`                             |
-| mute_xiaoai           | 快速停掉小爱自己的回答                            | `true`                              |
-| verbose               | 是否打印详细日志                                  | `false`                             |
-| bot                   | 使用的 bot 类型，目前支持gpt3,chatgptapi和newbing | `chatgptapi`                        |
-| enable_edge_tts       | 使用Edge TTS                                      | `false`                             |
-| edge_tts_voice        | Edge TTS 的嗓音                                   | `zh-CN-XiaoxiaoNeural`              |
-| prompt                | 自定义prompt                                      | `请用100字以内回答`                 |
-| keyword               | 自定义请求词列表                                  | `["请问"]`                          |
-| change_prompt_keyword | 更改提示词触发列表                                | `["更改提示词"]`                    |
-| start_conversation    | 开始持续对话关键词                                | `开始持续对话`                      |
-| end_conversation      | 结束持续对话关键词                                | `结束持续对话`                      |
-| stream                | 使用流式响应，获得更快的响应                      | `false`                             |
-| proxy                 | 支持 HTTP 代理，传入 http proxy URL               | ""                                  |
-| gpt_options           | OpenAI API 的参数字典                             | `{}`                                |
-| bing_cookie_path      | NewBing使用的cookie路径，参考[这里]获取           | 也可通过环境变量 `COOKIE_FILE` 设置 |
-| bing_cookies          | NewBing使用的cookie字典，参考[这里]获取           |                                     |
-
-[这里]: https://github.com/acheong08/EdgeGPT#getting-authentication-required
-
-## 注意
-
-1. 请开启小爱同学的蓝牙
-2. 如果要更改提示词和 PROMPT 在代码最上面自行更改
-3. 目前已知 LX04 和 L05B L05C 可能需要使用 `--use_command`
-
-## QA
-
-1. 用破解么？不用
-2. 你做这玩意也没用啊？确实。。。但是挺好玩的，有用对你来说没用，对我们来说不一定呀
-3. 想把它变得更好？PR Issue always welcome.
-4. 还有问题？提 Issuse 哈哈
-
-## 视频教程
-https://www.youtube.com/watch?v=K4YA8YwzOOA
-
-## Docker
-
-### 常规用法
-X86/ARM Docker Image: `yihong0618/xiaogpt`
-
-```shell
-docker run -e OPENAI_API_KEY=<your-openapi-key> yihong0618/xiaogpt <命令行参数>
-```
-
-如
-
-```shell
-docker run -e OPENAI_API_KEY=<your-openapi-key> yihong0618/xiaogpt --account=<your-xiaomi-account> --password=<your-xiaomi-password> --hardware=<your-xiaomi-hardware> --use_chatgpt_api
-```
-
-### 使用配置文件
-xiaogpt的配置文件可通过指定volume /config，以及指定参数--config来处理，如
-```shell
-docker run -v <your-config-dir>:/config yihong0618/xiaogpt --config=/config/config.json
-```
-
-### 本地编译Docker Image
-```shell
- docker build -t xiaogpt .
-```
-如果需要在Apple M1/M2上编译x86
-```shell
- docker buildx build --platform=linux/amd64 -t xiaogpt-x86 .
-```
-
-### Add edge-tts
-edge-tts提供了类似微软tts的能力
-- https://github.com/rany2/edge-tts
-
-#### Usage
-你可以通过参数`enable_edge_tts`, 来启用它
-```json
-{
-  "enable_edge_tts": true,
-  "edge_tts_voice": "zh-CN-XiaoxiaoNeural"
-}
-```
-
-查看更多语言支持, 从中选择一个
-```shell
-edge-tts --list-voices
-```
-
-#### 在容器中使用edge-tts
-
-由于 Edge TTS 启动了一个本地的 HTTP 服务，所以需要将容器的端口映射到宿主机上，并且指定本地机器的 hostname:
-
-```shell
-docker run -v <your-config-dir>:/config yihong0618/xiaogpt -p 9527:9527 -e XIAOGPT_HOSTNAME=<your ip> --config=/config/config.json
-```
-
-注意端口必须映射为与容器内一致，XIAOGPT_HOSTNAME 需要设置为宿主机的 IP 地址，否则小爱无法正常播放语音。
-
-## 推荐的 fork
-
-- [MIGPT](https://github.com/Afool4U/MIGPT) -> 基于 API 流式对话的低延迟版MIGPT
-- [XiaoBot](https://github.com/longbai/xiaobot) -> Go语言版本的Fork, 带支持不同平台的UI
-
-## 感谢
-
-- [xiaomi](https://www.mi.com/)
-- [PDM](https://pdm.fming.dev/latest/)
-- @[Yonsm](https://github.com/Yonsm) 的 [MiService](https://github.com/Yonsm/MiService)
-- @[pjq](https://github.com/pjq) 给了这个项目非常多的帮助
-- @[frostming](https://github.com/frostming) 重构了一些代码，支持了`持续会话功能`
-
-## 赞赏
-
-谢谢就够了
-## 编译发布
-```
-pip install --upgrade build twine
-python -m build
-twine upload dist/*
-```
-参考 https://blog.csdn.net/u010214511/article/details/126909523
+# xiaogpt
+
+[![PyPI](https://img.shields.io/pypi/v/xiaogpt?style=flat-square)](https://pypi.org/project/xiaogpt)
+[![Docker Image Version (latest by date)](https://img.shields.io/docker/v/yihong0618/xiaogpt?color=%23086DCD&label=docker%20image)](https://hub.docker.com/r/yihong0618/xiaogpt)
+
+
+https://user-images.githubusercontent.com/15976103/226803357-72f87a41-a15b-409e-94f5-e2d262eecd53.mp4
+
+
+Play ChatGPT with Xiaomi AI Speaker
+
+![image](https://user-images.githubusercontent.com/15976103/220028375-c193a859-48a1-4270-95b6-ef540e54a621.png)
+![image](https://user-images.githubusercontent.com/15976103/226802344-9c71f543-b73c-4a47-8703-4c200c434dec.png)
+
+## 支持的 AI 类型
+
+- GPT3
+- ChatGPT
+- New Bing
+
+## 一点原理
+
+[不用 root 使用小爱同学和 ChatGPT 交互折腾记](https://github.com/yihong0618/gitblog/issues/258)
+
+## 准备
+
+1. ChatGPT id
+2. 小爱音响
+3. 能正常联网的环境或 proxy
+4. python3.8+
+
+## 使用
+
+- `pip install -U --force-reinstall xiaogpt`
+- 参考我 fork 的 [MiService](https://github.com/yihong0618/MiService) 项目 README 并在本地 terminal 跑 `micli list` 拿到你音响的 DID 成功 **别忘了设置 export MI_DID=xxx** 这个 MI_DID 用
+- run `xiaogpt --hardware ${your_hardware} --use_chatgpt_api` hardware 你看小爱屁股上有型号，输入进来，如果在屁股上找不到或者型号不对，可以用 `micli mina` 找到型号
+- 跑起来之后就可以问小爱同学问题了，“帮我"开头的问题，会发送一份给 ChatGPT 然后小爱同学用 tts 回答
+- 如果上面不可用，可以尝试用手机抓包，https://userprofile.mina.mi.com/device_profile/v2/conversation 找到 cookie 利用 `--cookie '${cookie}'` cookie 别忘了用单引号包裹
+- 默认用目前 ubus, 如果你的设备不支持 ubus 可以使用 `--use_command` 来使用 command 来 tts
+- 使用 `--mute_xiaoai` 选项，可以快速停掉小爱的回答
+- 使用 `--account ${account} --password ${password}`
+- 如果有能力可以自行替换唤醒词，也可以去掉唤醒词
+- 使用 `--use_chatgpt_api` 的 api 那样可以更流畅的对话，速度特别快，达到了对话的体验, [openai api](https://platform.openai.com/account/api-keys), 命令 `--use_chatgpt_api`
+- 使用 gpt-3 的 api 那样可以更流畅的对话，速度快, 请 google 如何用 [openai api](https://platform.openai.com/account/api-keys) 命令 --use_gpt3
+- 如果你遇到了墙需要用 Cloudflare Workers 替换 api_base 请使用 `--api_base ${url}` 来替换。  **请注意，此处你输入的api应该是'`https://xxxx/v1`'的字样，域名需要用引号包裹**
+- 可以跟小爱说 `开始持续对话` 自动进入持续对话状态，`结束持续对话` 结束持续对话状态。
+- 可以使用 `--enable_edge_tts` 来获取更好的 tts 能力
+
+e.g.
+
+```shell
+export OPENAI_API_KEY=${your_api_key}
+xiaogpt --hardware LX06 --use_chatgpt_api
+# or
+xiaogpt --hardware LX06 --cookie ${cookie} --use_chatgpt_api
+# 如果你想直接输入账号密码
+xiaogpt --hardware LX06 --account ${your_xiaomi_account} --password ${your_password} --use_chatgpt_api
+# 如果你想 mute 小米的回答
+xiaogpt --hardware LX06  --mute_xiaoai --use_chatgpt_api
+# 使用流式响应，获得更快的响应
+xiaogpt --hardware LX06  --mute_xiaoai --stream
+# 如果你想使用 gpt3 ai
+export OPENAI_API_KEY=${your_api_key}
+xiaogpt --hardware LX06  --mute_xiaoai --use_gpt3
+# 如果你想用 edge-tts
+xiaogpt --hardware LX06 --cookie ${cookie} --use_chatgpt_api --enable_edge_tts
+```
+使用 git clone 运行
+
+```shell
+export OPENAI_API_KEY=${your_api_key}
+python3 loznxiaoai.py --hardware LX06
+# or
+python3 loznxiaoai.py --hardware LX06 --cookie ${cookie}
+# 如果你想直接输入账号密码
+python3 loznxiaoai.py --hardware LX06 --account ${your_xiaomi_account} --password ${your_password} --use_chatgpt_api
+# 如果你想 mute 小米的回答
+python3 loznxiaoai.py --hardware LX06  --mute_xiaoai
+# 使用流式响应，获得更快的响应
+python3 loznxiaoai.py --hardware LX06  --mute_xiaoai --stream
+# 如果你想使用 gpt3 ai
+export OPENAI_API_KEY=${your_api_key}
+python3 loznxiaoai.py --hardware LX06  --mute_xiaoai --use_gpt3
+```
+
+## config.json
+如果想通过单一配置文件启动也是可以的, 可以通过 `--config` 参数指定配置文件, config 文件必须是合法的 JSON 格式
+参数优先级
+- cli args > default > config
+
+```shell
+python3 loznxiaoai.py --config xiao_config.json
+# or
+xiaogpt --config xiao_config.json
+```
+或者
+```shell
+cp xiao_config.json.example xiao_config.json
+python3 loznxiaoai.py
+```
+
+若要指定 OpenAI 的模型参数，如 model, temporature, top_p, 请在config.json中指定：
+
+```json
+{
+    ...
+    "gpt_options": {
+        "temperature": 0.9,
+        "top_p": 0.9,
+    }
+}
+```
+
+具体参数作用请参考 [Open AI API 文档](https://platform.openai.com/docs/api-reference/chat/create)。
+## 配置项说明
+
+| 参数                  | 说明                                              | 默认值                              |
+| --------------------- | ------------------------------------------------- | ----------------------------------- |
+| hardware              | 设备型号                                          |                                     |
+| account               | 小爱账户                                          |                                     |
+| password              | 小爱账户密码                                      |                                     |
+| openai_key            | openai的apikey                                    |                                     |
+| cookie                | 小爱账户cookie （如果用上面密码登录可以不填）     |                                     |
+| mi_did                | 设备did                                           |                                     |
+| use_command           | 使用 MI command 与小爱交互                        | `false`                             |
+| mute_xiaoai           | 快速停掉小爱自己的回答                            | `true`                              |
+| verbose               | 是否打印详细日志                                  | `false`                             |
+| bot                   | 使用的 bot 类型，目前支持gpt3,chatgptapi和newbing | `chatgptapi`                        |
+| enable_edge_tts       | 使用Edge TTS                                      | `false`                             |
+| edge_tts_voice        | Edge TTS 的嗓音                                   | `zh-CN-XiaoxiaoNeural`              |
+| prompt                | 自定义prompt                                      | `请用100字以内回答`                 |
+| keyword               | 自定义请求词列表                                  | `["请问"]`                          |
+| change_prompt_keyword | 更改提示词触发列表                                | `["更改提示词"]`                    |
+| start_conversation    | 开始持续对话关键词                                | `开始持续对话`                      |
+| end_conversation      | 结束持续对话关键词                                | `结束持续对话`                      |
+| stream                | 使用流式响应，获得更快的响应                      | `false`                             |
+| proxy                 | 支持 HTTP 代理，传入 http proxy URL               | ""                                  |
+| gpt_options           | OpenAI API 的参数字典                             | `{}`                                |
+| bing_cookie_path      | NewBing使用的cookie路径，参考[这里]获取           | 也可通过环境变量 `COOKIE_FILE` 设置 |
+| bing_cookies          | NewBing使用的cookie字典，参考[这里]获取           |                                     |
+
+[这里]: https://github.com/acheong08/EdgeGPT#getting-authentication-required
+
+## 注意
+
+1. 请开启小爱同学的蓝牙
+2. 如果要更改提示词和 PROMPT 在代码最上面自行更改
+3. 目前已知 LX04 和 L05B L05C 可能需要使用 `--use_command`
+
+## QA
+
+1. 用破解么？不用
+2. 你做这玩意也没用啊？确实。。。但是挺好玩的，有用对你来说没用，对我们来说不一定呀
+3. 想把它变得更好？PR Issue always welcome.
+4. 还有问题？提 Issuse 哈哈
+
+## 视频教程
+https://www.youtube.com/watch?v=K4YA8YwzOOA
+
+## Docker
+
+### 常规用法
+X86/ARM Docker Image: `yihong0618/xiaogpt`
+
+```shell
+docker run -e OPENAI_API_KEY=<your-openapi-key> yihong0618/xiaogpt <命令行参数>
+```
+
+如
+
+```shell
+docker run -e OPENAI_API_KEY=<your-openapi-key> yihong0618/xiaogpt --account=<your-xiaomi-account> --password=<your-xiaomi-password> --hardware=<your-xiaomi-hardware> --use_chatgpt_api
+```
+
+### 使用配置文件
+xiaogpt的配置文件可通过指定volume /config，以及指定参数--config来处理，如
+```shell
+docker run -v <your-config-dir>:/config yihong0618/xiaogpt --config=/config/config.json
+```
+
+### 本地编译Docker Image
+```shell
+ docker build -t xiaogpt .
+```
+如果需要在Apple M1/M2上编译x86
+```shell
+ docker buildx build --platform=linux/amd64 -t xiaogpt-x86 .
+```
+
+### Add edge-tts
+edge-tts提供了类似微软tts的能力
+- https://github.com/rany2/edge-tts
+
+#### Usage
+你可以通过参数`enable_edge_tts`, 来启用它
+```json
+{
+  "enable_edge_tts": true,
+  "edge_tts_voice": "zh-CN-XiaoxiaoNeural"
+}
+```
+
+查看更多语言支持, 从中选择一个
+```shell
+edge-tts --list-voices
+```
+
+#### 在容器中使用edge-tts
+
+由于 Edge TTS 启动了一个本地的 HTTP 服务，所以需要将容器的端口映射到宿主机上，并且指定本地机器的 hostname:
+
+```shell
+docker run -v <your-config-dir>:/config yihong0618/xiaogpt -p 9527:9527 -e XIAOGPT_HOSTNAME=<your ip> --config=/config/config.json
+```
+
+注意端口必须映射为与容器内一致，XIAOGPT_HOSTNAME 需要设置为宿主机的 IP 地址，否则小爱无法正常播放语音。
+
+## 推荐的 fork
+
+- [MIGPT](https://github.com/Afool4U/MIGPT) -> 基于 API 流式对话的低延迟版MIGPT
+- [XiaoBot](https://github.com/longbai/xiaobot) -> Go语言版本的Fork, 带支持不同平台的UI
+
+## 感谢
+
+- [xiaomi](https://www.mi.com/)
+- [PDM](https://pdm.fming.dev/latest/)
+- @[Yonsm](https://github.com/Yonsm) 的 [MiService](https://github.com/Yonsm/MiService)
+- @[pjq](https://github.com/pjq) 给了这个项目非常多的帮助
+- @[frostming](https://github.com/frostming) 重构了一些代码，支持了`持续会话功能`
+
+## 赞赏
+
+谢谢就够了
+## 编译发布
+```
+pip install --upgrade build twine
+python -m build
+twine upload dist/*
+```
+参考 https://blog.csdn.net/u010214511/article/details/126909523
```

### Comparing `xiaoaiai-0.1.1/pyproject.toml` & `xiaoaiai-0.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -15,38 +15,37 @@
     "miservice_fork",
     "openai",
     "aiohttp",
     "rich",
     "edge-tts>=6.1.3",
     "EdgeGPT",
 ]
-version = "0.1.1"
+dynamic = []
+version = "0.2"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/qssq/xiaoai"
 
 [project.scripts]
-xiaogpt = "xiaoai.cli:main"
+xiaogpt = "xiaogpt.cli:main"
 
 [tool.pdm]
 autoexport = [
     { filename = "requirements.txt", without-hashes = true },
 ]
 
 [tool.pdm.version]
 source = "scm"
 
 [tool.pdm.build]
 includes = [
     "xiaogpt/",
-    "ChatGPT/src/",
-    "xiaoai/",
 ]
 
 [build-system]
 requires = [
     "pdm-backend>=2.0.0",
 ]
 build-backend = "pdm.backend"
```

### Comparing `xiaoaiai-0.1.1/xiaogpt/bot/chatgptapi_bot.py` & `xiaoaiai-0.2/xiaogpt/bot/chatgptapi_bot.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-import openai
-from rich import print
-
-from xiaogpt.bot.base_bot import BaseBot
-from xiaogpt.utils import split_sentences
-
-
-class ChatGPTBot(BaseBot):
-    def __init__(self, openai_key, api_base=None, proxy=None):
-        self.history = []
-        self.name: str = "查机批踢"
-        openai.api_key = openai_key
-        if api_base:
-            openai.api_base = api_base
-        if proxy:
-            openai.proxy = proxy
-    async def ask(self, query, **options):
-        ms = []
-        for h in self.history:
-            ms.append({"role": "user", "content": h[0]})
-            ms.append({"role": "assistant", "content": h[1]})
-        ms.append({"role": "user", "content": f"{query}"})
-        kwargs = {"model": "gpt-3.5-turbo", **options}
-        completion = await openai.ChatCompletion.acreate(messages=ms, **kwargs)
-        message = (
-            completion["choices"][0]
-            .get("message")
-            .get("content")
-            .encode("utf8")
-            .decode()
-        )
-        self.history.append([f"{query}", message])
-        # only keep 5 history
-        first_history = self.history.pop(0)
-        self.history = [first_history] + self.history[-5:]
-        print(message)
-        return message
-
-    async def ask_stream(self, query, **options):
-        ms = []
-        for h in self.history:
-            ms.append({"role": "user", "content": h[0]})
-            ms.append({"role": "assistant", "content": h[1]})
-        ms.append({"role": "user", "content": f"{query}"})
-        kwargs = {"model": "gpt-3.5-turbo", **options}
-        completion = await openai.ChatCompletion.acreate(
-            messages=ms, stream=True, **kwargs
-        )
-
-        async def text_gen():
-            async for event in completion:
-                chunk_message = event["choices"][0]["delta"]
-                if "content" not in chunk_message:
-                    continue
-                print(chunk_message["content"], end="")
-                yield chunk_message["content"]
-
-        message = ""
-        try:
-            async for sentence in split_sentences(text_gen()):
-                message += sentence
-                yield sentence
-        finally:
-            print()
-            self.history.append([f"{query}", message])
-            first_history = self.history.pop(0)
-            self.history = [first_history] + self.history[-5:]
+import openai
+from rich import print
+
+from xiaogpt.bot.base_bot import BaseBot
+from xiaogpt.utils import split_sentences
+
+
+class ChatGPTBot(BaseBot):
+    def __init__(self, openai_key, api_base=None, proxy=None):
+        self.history = []
+        self.name: str = "查机批踢"
+        openai.api_key = openai_key
+        if api_base:
+            openai.api_base = api_base
+        if proxy:
+            openai.proxy = proxy
+    async def ask(self, query, **options):
+        ms = []
+        for h in self.history:
+            ms.append({"role": "user", "content": h[0]})
+            ms.append({"role": "assistant", "content": h[1]})
+        ms.append({"role": "user", "content": f"{query}"})
+        kwargs = {"model": "gpt-3.5-turbo", **options}
+        completion = await openai.ChatCompletion.acreate(messages=ms, **kwargs)
+        message = (
+            completion["choices"][0]
+            .get("message")
+            .get("content")
+            .encode("utf8")
+            .decode()
+        )
+        self.history.append([f"{query}", message])
+        # only keep 5 history
+        first_history = self.history.pop(0)
+        self.history = [first_history] + self.history[-5:]
+        print(message)
+        return message
+
+    async def ask_stream(self, query, **options):
+        ms = []
+        for h in self.history:
+            ms.append({"role": "user", "content": h[0]})
+            ms.append({"role": "assistant", "content": h[1]})
+        ms.append({"role": "user", "content": f"{query}"})
+        kwargs = {"model": "gpt-3.5-turbo", **options}
+        completion = await openai.ChatCompletion.acreate(
+            messages=ms, stream=True, **kwargs
+        )
+
+        async def text_gen():
+            async for event in completion:
+                chunk_message = event["choices"][0]["delta"]
+                if "content" not in chunk_message:
+                    continue
+                print(chunk_message["content"], end="")
+                yield chunk_message["content"]
+
+        message = ""
+        try:
+            async for sentence in split_sentences(text_gen()):
+                message += sentence
+                yield sentence
+        finally:
+            print()
+            self.history.append([f"{query}", message])
+            first_history = self.history.pop(0)
+            self.history = [first_history] + self.history[-5:]
```

### Comparing `xiaoaiai-0.1.1/xiaogpt/bot/newbing_acheongbot.py` & `xiaoaiai-0.2/xiaogpt/bot/revchatgpt_bot.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-from __future__ import annotations
-
-import re
-
-import asyncio
-from EdgeGPT import Chatbot, ConversationStyle
-from xiaogpt.utils import split_sentences
-
-_reference_link_re = re.compile(r"\[\d+\]: .+?\n+")
-
-
-class NewBingAcheongBot:
-
-    def __init__(
-            self,
-            bing_cookie_path: str = "",
-            bing_cookies: dict | None = None,
-            proxy: str | None = None,
-    ):
-        self.history = []
-        self.name: str = "新必应"
-        if (not proxy == None and len(proxy) == 0):
-            proxy = None
-        self._bot = Chatbot(
-            cookiePath=bing_cookie_path, cookies=bing_cookies, proxy=proxy
-        )
-
-    # https: // github.com / acheong08 / EdgeGPT
-    @staticmethod
-    def clean_text(s):
-        s = s.replace("**", "")
-        s = _reference_link_re.sub("", s)
-        s = re.sub(r"\[[\^\d]+\]", "", s)
-        return s.strip()
-
-    async def ask(self, query, **options):
-        kwargs = {"conversation_style": ConversationStyle.balanced, **options}
-        # completion = await self._bot.ask(prompt=query, **kwargs)
-        try:
-            completion = await self._bot.ask(prompt=query, conversation_style=ConversationStyle.creative,
-                                             wss_link="wss://sydney.bing.com/sydney/ChatHub")
-            text = self.clean_text(completion["item"]["messages"][1]["text"])
-        except Exception as e:
-            print("提问失败," + query + "," + str(e))
-        print(text)
-        text = text.replace("你好，我是必应。", "") \
-            .replace("这里是必应", "") \
-            .replace("我是必应", "") \
-            .replace("必应", "").replace("。", "").replace("，", "")
-        return text
-
-        # await self._bot.close()
-
-    async def ask_stream(self, query, **options):
-        kwargs = {"conversation_style": ConversationStyle.balanced, **options}
-        completion = self._bot.ask_stream(prompt=query, **kwargs)
-
-        async def text_gen():
-            current = ""
-            async for final, resp in completion:
-                if final:
-                    break
-                text = self.clean_text(resp)
-                if text == current:
-                    continue
-                diff = text[len(current):]
-                print(diff, end="")
-                # if (not self.proyprint == None):
-                #     self.proyprint(diff)
-                yield diff
-                current = text
-
-        try:
-            async for sentence in split_sentences(text_gen()):
-                yield sentence
-        finally:
-            print()
+from __future__ import annotations
+
+import re
+
+from xiaogpt.utils import split_sentences
+
+_reference_link_re = re.compile(r"\[\d+\]: .+?\n+")
+
+
+class RevChatgpt:
+    def __init__(
+            self,
+            access_token: str | None = None,
+            proxy: str | None = None,
+    ):
+        self.history = []
+        self.name: str = "傻妞"
+        from ChatGPT.src.revChatGPT.V1 import Chatbot
+
+        # self._robot = Chatbot(config={
+        #     "email": "qssq521@gmail.com",
+        #     "password": "Luozheng123",
+        #     "proxy": "http://127.0.0.1:7890",
+        # })
+        self._robot: Chatbot = Chatbot(config={
+            "access_token": access_token,
+            "proxy": proxy
+        })
+        self.conversation_id: str = ""
+        self.parent_id: str = ""
+
+    @staticmethod
+    def clean_text(s):
+        s = s.replace("**", "")
+        s = _reference_link_re.sub("", s)
+        s = re.sub(r"\[[\^\d]+\]", "", s)
+        return s.strip()
+
+    async def ask(self, query, **options):
+        # prompt = input("Enter your want ask: ")
+        # print(prompt)
+        response = ""
+        for data in self._robot.ask(
+                prompt=query,
+                conversation_id=self.conversation_id,
+                parent_id=self.parent_id,
+        ):
+            response = data["message"]
+            self.conversation_id = data["conversation_id"]
+            self.parent_id = data["parent_id"]
+        return response
+
+    async def ask_stream(self, query, **options):
+        completion = self._robot.ask(
+            conversation_id=self.conversation_id,
+            parent_id=self.parent_id,
+            prompt=query
+        )
+
+        async def text_gen():
+            current = ""
+            async for final, resp in completion:
+                if final:
+                    break
+                text = self.clean_text(resp)
+                if text == current:
+                    continue
+                diff = text[len(current):]
+                print(diff, end="")
+                yield diff
+                current = text
+
+        try:
+            async for sentence in split_sentences(text_gen()):
+                yield sentence
+        finally:
+            print()
```

### Comparing `xiaoaiai-0.1.1/xiaogpt/config.py` & `xiaoaiai-0.2/xiaogpt/config.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,135 +1,135 @@
-from __future__ import annotations
-
-import argparse
-import json
-import os
-from dataclasses import dataclass, field
-from typing import Any, Iterable
-
-from xiaogpt.utils import validate_proxy
-
-LATEST_ASK_API = "https://userprofile.mina.mi.com/device_profile/v2/conversation?source=dialogu&hardware={hardware}&timestamp={timestamp}&limit=2"
-COOKIE_TEMPLATE = "deviceId={device_id}; serviceToken={service_token}; userId={user_id}"
-WAKEUP_KEYWORD = "小爱同学"
-
-HARDWARE_COMMAND_DICT = {
-    # hardware: (tts_command, wakeup_command)
-    "LX06": ("5-1", "5-5"),
-    "L05B": ("5-3", "5-4"),
-    "S12A": ("5-1", "5-5"),
-    "LX01": ("5-1", "5-5"),
-    "L06A": ("5-1", "5-5"),
-    "LX04": ("5-1", "5-4"),
-    "L05C": ("5-3", "5-4"),
-    "L17A": ("7-3", "7-4"),
-    "X08E": ("7-3", "7-4"),
-    "LX05A": ("5-1", "5-5"),  # 小爱红外版
-    "LX5A": ("5-1", "5-5"),  # 小爱红外版
-    "L07A": ("5-1", "5-5"),  # Redmi小爱音箱Play(l7a)
-    "L15A": ("7-3", "7-4"),
-    "X6A": ("7-3", "7-4"),  # 小米智能家庭屏6
-    # add more here
-}
-
-EDGE_TTS_DICT = {
-    "用英语": "en-US-AriaNeural",
-    "用日语": "ja-JP-NanamiNeural",
-    "用法语": "fr-BE-CharlineNeural",
-    "用韩语": "ko-KR-SunHiNeural",
-    "用德语": "de-AT-JonasNeural",
-    # add more here
-}
-
-DEFAULT_COMMAND = ("5-1", "5-5")
-
-KEY_WORD = ("帮我", "请回答")
-CHANGE_PROMPT_KEY_WORD = ("更改提示词",)
-PROMPT = "以下请用100字以内回答，请只回答文字不要带链接"
-# simulate_xiaoai_question
-MI_ASK_SIMULATE_DATA = {
-    "code": 0,
-    "message": "Success",
-    "data": '{"bitSet":[0,1,1],"records":[{"bitSet":[0,1,1,1,1],"answers":[{"bitSet":[0,1,1,1],"type":"TTS","tts":{"bitSet":[0,1],"text":"Fake Answer"}}],"time":1677851434593,"query":"Fake Question","requestId":"fada34f8fa0c3f408ee6761ec7391d85"}],"nextEndTime":1677849207387}',
-}
-
-
-@dataclass
-class Config:
-    hardware: str = "LX06"
-    test: bool = False
-    answerall:bool=False
-    account: str = os.getenv("MI_USER", "")
-    port: str = os.getenv("XIAOGPT_PORT", "")
-    password: str = os.getenv("MI_PASS", "")
-    openai_key: str = os.getenv("OPENAI_API_KEY", "")
-    proxy: str | None = None
-    mi_did: str = os.getenv("MI_DID", "")
-    keyword: Iterable[str] = KEY_WORD
-    change_prompt_keyword: Iterable[str] = CHANGE_PROMPT_KEY_WORD
-    prompt: str = PROMPT
-    mute_xiaoai: bool = False
-    bot: str = "newbing1"
-    cookie: str = ""
-    api_base: str | None = None
-    use_command: bool = False
-    verbose: bool = False
-    detailverbose: bool = False
-    start_conversation:  Iterable[str] = ("开始持续对话")
-    end_conversation:  Iterable[str] = ("结束持续对话")
-    access_token: str = ""
-    stream: bool = False
-    enable_edge_tts: bool = False
-    edge_tts_voice: str = "zh-CN-XiaoxiaoNeural"
-    gpt_options: dict[str, Any] = field(default_factory=dict)
-    bing_cookie_path: str = ""
-    bing_cookies: dict | None = None
-
-    def __post_init__(self) -> None:
-        if self.proxy:
-            validate_proxy(self.proxy)
-        if self.bot == "newbing":
-            if not (self.bing_cookie_path or self.bing_cookies):
-                raise Exception(
-                    "New bing bot needs bing_cookie_path or bing_cookies, read this: "
-                    "https://github.com/acheong08/EdgeGPT#getting-authentication-required"
-                )
-        elif not self.openai_key:
-            raise Exception("Using GPT api needs openai API key, please google how to")
-
-    @property
-    def tts_command(self) -> str:
-        return HARDWARE_COMMAND_DICT.get(self.hardware, DEFAULT_COMMAND)[0]
-
-    @property
-    def wakeup_command(self) -> str:
-        return HARDWARE_COMMAND_DICT.get(self.hardware, DEFAULT_COMMAND)[1]
-
-    @classmethod
-    def from_options(cls, options: argparse.Namespace) -> Config:
-        config = {}
-        if options.config and os.path.isfile(options.config):
-            config = cls.read_from_file(options.config)
-        for key, value in vars(options).items():
-            if value is not None and key in cls.__dataclass_fields__:
-                config[key] = value
-        return cls(**config)
-
-    @classmethod
-    def read_from_file(cls, config_path: str) -> dict:
-        result = {}
-        with open(config_path, "rb") as f:
-            config = json.load(f)
-            for key, value in config.items():
-                if value is not None and key in cls.__dataclass_fields__:
-                    if key == "keyword":
-                        if not isinstance(value, list):
-                            value = [value]
-                        value = [kw for kw in value if kw]
-                    elif key == "use_chatgpt_api":
-                        key, value = "bot", "chatgptapi"
-                    elif key == "use_gpt3":
-                        key, value = "bot", "gpt3"
-                    elif key == "use_newbing":
-                        key, value = "bot", "newbing"
-                    result[key] = value
-        return result
+from __future__ import annotations
+
+import argparse
+import json
+import os
+from dataclasses import dataclass, field
+from typing import Any, Iterable
+
+from xiaogpt.utils import validate_proxy
+
+LATEST_ASK_API = "https://userprofile.mina.mi.com/device_profile/v2/conversation?source=dialogu&hardware={hardware}&timestamp={timestamp}&limit=2"
+COOKIE_TEMPLATE = "deviceId={device_id}; serviceToken={service_token}; userId={user_id}"
+WAKEUP_KEYWORD = "小爱同学"
+
+HARDWARE_COMMAND_DICT = {
+    # hardware: (tts_command, wakeup_command)
+    "LX06": ("5-1", "5-5"),
+    "L05B": ("5-3", "5-4"),
+    "S12A": ("5-1", "5-5"),
+    "LX01": ("5-1", "5-5"),
+    "L06A": ("5-1", "5-5"),
+    "LX04": ("5-1", "5-4"),
+    "L05C": ("5-3", "5-4"),
+    "L17A": ("7-3", "7-4"),
+    "X08E": ("7-3", "7-4"),
+    "LX05A": ("5-1", "5-5"),  # 小爱红外版
+    "LX5A": ("5-1", "5-5"),  # 小爱红外版
+    "L07A": ("5-1", "5-5"),  # Redmi小爱音箱Play(l7a)
+    "L15A": ("7-3", "7-4"),
+    "X6A": ("7-3", "7-4"),  # 小米智能家庭屏6
+    # add more here
+}
+
+EDGE_TTS_DICT = {
+    "用英语": "en-US-AriaNeural",
+    "用日语": "ja-JP-NanamiNeural",
+    "用法语": "fr-BE-CharlineNeural",
+    "用韩语": "ko-KR-SunHiNeural",
+    "用德语": "de-AT-JonasNeural",
+    # add more here
+}
+
+DEFAULT_COMMAND = ("5-1", "5-5")
+
+KEY_WORD = ("帮我", "请回答")
+CHANGE_PROMPT_KEY_WORD = ("更改提示词",)
+PROMPT = "以下请用100字以内回答，请只回答文字不要带链接"
+# simulate_xiaoai_question
+MI_ASK_SIMULATE_DATA = {
+    "code": 0,
+    "message": "Success",
+    "data": '{"bitSet":[0,1,1],"records":[{"bitSet":[0,1,1,1,1],"answers":[{"bitSet":[0,1,1,1],"type":"TTS","tts":{"bitSet":[0,1],"text":"Fake Answer"}}],"time":1677851434593,"query":"Fake Question","requestId":"fada34f8fa0c3f408ee6761ec7391d85"}],"nextEndTime":1677849207387}',
+}
+
+
+@dataclass
+class Config:
+    hardware: str = "LX06"
+    test: bool = False
+    answerall:bool=False
+    account: str = os.getenv("MI_USER", "")
+    port: str = os.getenv("XIAOGPT_PORT", "")
+    password: str = os.getenv("MI_PASS", "")
+    openai_key: str = os.getenv("OPENAI_API_KEY", "")
+    proxy: str | None = None
+    mi_did: str = os.getenv("MI_DID", "")
+    keyword: Iterable[str] = KEY_WORD
+    change_prompt_keyword: Iterable[str] = CHANGE_PROMPT_KEY_WORD
+    prompt: str = PROMPT
+    mute_xiaoai: bool = False
+    bot: str = "newbing1"
+    cookie: str = ""
+    api_base: str | None = None
+    use_command: bool = False
+    verbose: bool = False
+    detailverbose: bool = False
+    start_conversation:  Iterable[str] = ("开始持续对话")
+    end_conversation:  Iterable[str] = ("结束持续对话")
+    access_token: str = ""
+    stream: bool = False
+    enable_edge_tts: bool = False
+    edge_tts_voice: str = "zh-CN-XiaoxiaoNeural"
+    gpt_options: dict[str, Any] = field(default_factory=dict)
+    bing_cookie_path: str = ""
+    bing_cookies: dict | None = None
+
+    def __post_init__(self) -> None:
+        if self.proxy:
+            validate_proxy(self.proxy)
+        if self.bot == "newbing":
+            if not (self.bing_cookie_path or self.bing_cookies):
+                raise Exception(
+                    "New bing bot needs bing_cookie_path or bing_cookies, read this: "
+                    "https://github.com/acheong08/EdgeGPT#getting-authentication-required"
+                )
+        elif not self.openai_key:
+            raise Exception("Using GPT api needs openai API key, please google how to")
+
+    @property
+    def tts_command(self) -> str:
+        return HARDWARE_COMMAND_DICT.get(self.hardware, DEFAULT_COMMAND)[0]
+
+    @property
+    def wakeup_command(self) -> str:
+        return HARDWARE_COMMAND_DICT.get(self.hardware, DEFAULT_COMMAND)[1]
+
+    @classmethod
+    def from_options(cls, options: argparse.Namespace) -> Config:
+        config = {}
+        if options.config and os.path.isfile(options.config):
+            config = cls.read_from_file(options.config)
+        for key, value in vars(options).items():
+            if value is not None and key in cls.__dataclass_fields__:
+                config[key] = value
+        return cls(**config)
+
+    @classmethod
+    def read_from_file(cls, config_path: str) -> dict:
+        result = {}
+        with open(config_path, "rb") as f:
+            config = json.load(f)
+            for key, value in config.items():
+                if value is not None and key in cls.__dataclass_fields__:
+                    if key == "keyword":
+                        if not isinstance(value, list):
+                            value = [value]
+                        value = [kw for kw in value if kw]
+                    elif key == "use_chatgpt_api":
+                        key, value = "bot", "chatgptapi"
+                    elif key == "use_gpt3":
+                        key, value = "bot", "gpt3"
+                    elif key == "use_newbing":
+                        key, value = "bot", "newbing"
+                    result[key] = value
+        return result
```

### Comparing `xiaoaiai-0.1.1/PKG-INFO` & `xiaoaiai-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xiaoaiai
-Version: 0.1.1
+Version: 0.2
 Summary: Play ChatGPT with xiaomi AI speaker
 Author-Email: lozn <qssq521@gmail.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Homepage, https://github.com/qssq/xiaoai
```


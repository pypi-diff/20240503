# Comparing `tmp/xiaogpt-2.64.tar.gz` & `tmp/xiaogpt-2.70.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiaogpt-2.64.tar", last modified: Thu Apr 25 02:23:43 2024, max compression
+gzip compressed data, was "xiaogpt-2.70.tar", last modified: Fri May  3 05:30:50 2024, max compression
```

## Comparing `xiaogpt-2.64.tar` & `xiaogpt-2.70.tar`

### file list

```diff
@@ -1,27 +1,30 @@
--rw-r--r--   0        0        0     1063 2024-04-25 02:23:36.228737 xiaogpt-2.64/LICENSE
--rw-r--r--   0        0        0    22689 2024-04-25 02:23:36.228737 xiaogpt-2.64/README.md
--rw-r--r--   0        0        0     3938 2024-04-25 02:23:43.912794 xiaogpt-2.64/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-25 02:23:36.228737 xiaogpt-2.64/xiaogpt/__init__.py
--rw-r--r--   0        0        0       61 2024-04-25 02:23:36.228737 xiaogpt-2.64/xiaogpt/__main__.py
--rw-r--r--   0        0        0     1006 2024-04-25 02:23:36.228737 xiaogpt-2.64/xiaogpt/bot/__init__.py
--rw-r--r--   0        0        0     1467 2024-04-25 02:23:36.228737 xiaogpt-2.64/xiaogpt/bot/base_bot.py
--rw-r--r--   0        0        0     3656 2024-04-25 02:23:36.228737 xiaogpt-2.64/xiaogpt/bot/chatgptapi_bot.py
--rw-r--r--   0        0        0     2773 2024-04-25 02:23:36.228737 xiaogpt-2.64/xiaogpt/bot/doubao_bot.py
--rw-r--r--   0        0        0     2516 2024-04-25 02:23:36.228737 xiaogpt-2.64/xiaogpt/bot/gemini_bot.py
--rw-r--r--   0        0        0     1825 2024-04-25 02:23:36.228737 xiaogpt-2.64/xiaogpt/bot/glm_bot.py
--rw-r--r--   0        0        0     1944 2024-04-25 02:23:36.228737 xiaogpt-2.64/xiaogpt/bot/langchain_bot.py
--rw-r--r--   0        0        0     2289 2024-04-25 02:23:36.228737 xiaogpt-2.64/xiaogpt/bot/newbing_bot.py
--rw-r--r--   0        0        0     3657 2024-04-25 02:23:36.228737 xiaogpt-2.64/xiaogpt/bot/qwen_bot.py
--rw-r--r--   0        0        0     4956 2024-04-25 02:23:36.228737 xiaogpt-2.64/xiaogpt/cli.py
--rw-r--r--   0        0        0     6560 2024-04-25 02:23:36.228737 xiaogpt-2.64/xiaogpt/config.py
--rw-r--r--   0        0        0     2616 2024-04-25 02:23:36.228737 xiaogpt-2.64/xiaogpt/langchain/callbacks.py
--rw-r--r--   0        0        0     1495 2024-04-25 02:23:36.228737 xiaogpt-2.64/xiaogpt/langchain/chain.py
--rw-r--r--   0        0        0     6372 2024-04-25 02:23:36.228737 xiaogpt-2.64/xiaogpt/langchain/examples/email/mail_box.py
--rw-r--r--   0        0        0     1561 2024-04-25 02:23:36.228737 xiaogpt-2.64/xiaogpt/langchain/examples/email/mail_summary_tools.py
--rw-r--r--   0        0        0      145 2024-04-25 02:23:36.228737 xiaogpt-2.64/xiaogpt/tts/__init__.py
--rw-r--r--   0        0        0     4656 2024-04-25 02:23:36.228737 xiaogpt-2.64/xiaogpt/tts/base.py
--rw-r--r--   0        0        0     1095 2024-04-25 02:23:36.228737 xiaogpt-2.64/xiaogpt/tts/mi.py
--rw-r--r--   0        0        0     1058 2024-04-25 02:23:36.228737 xiaogpt-2.64/xiaogpt/tts/tetos.py
--rw-r--r--   0        0        0     2072 2024-04-25 02:23:36.232737 xiaogpt-2.64/xiaogpt/utils.py
--rw-r--r--   0        0        0    15960 2024-04-25 02:23:36.232737 xiaogpt-2.64/xiaogpt/xiaogpt.py
--rw-r--r--   0        0        0    28654 1970-01-01 00:00:00.000000 xiaogpt-2.64/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-03 05:30:43.428077 xiaogpt-2.70/LICENSE
+-rw-r--r--   0        0        0    22452 2024-05-03 05:30:43.428077 xiaogpt-2.70/README.md
+-rw-r--r--   0        0        0     3987 2024-05-03 05:30:50.091982 xiaogpt-2.70/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/__init__.py
+-rw-r--r--   0        0        0       61 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/__main__.py
+-rw-r--r--   0        0        0     1252 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/bot/__init__.py
+-rw-r--r--   0        0        0     1467 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/bot/base_bot.py
+-rw-r--r--   0        0        0     3656 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/bot/chatgptapi_bot.py
+-rw-r--r--   0        0        0     2773 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/bot/doubao_bot.py
+-rw-r--r--   0        0        0     2516 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/bot/gemini_bot.py
+-rw-r--r--   0        0        0     1825 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/bot/glm_bot.py
+-rw-r--r--   0        0        0     1944 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/bot/langchain_bot.py
+-rw-r--r--   0        0        0      708 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/bot/llama_bot.py
+-rw-r--r--   0        0        0      822 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/bot/moonshot_bot.py
+-rw-r--r--   0        0        0     2289 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/bot/newbing_bot.py
+-rw-r--r--   0        0        0     3657 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/bot/qwen_bot.py
+-rw-r--r--   0        0        0      784 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/bot/yi_bot.py
+-rw-r--r--   0        0        0     5899 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/cli.py
+-rw-r--r--   0        0        0     7006 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/config.py
+-rw-r--r--   0        0        0     2616 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/langchain/callbacks.py
+-rw-r--r--   0        0        0     1495 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/langchain/chain.py
+-rw-r--r--   0        0        0     6372 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/langchain/examples/email/mail_box.py
+-rw-r--r--   0        0        0     1561 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/langchain/examples/email/mail_summary_tools.py
+-rw-r--r--   0        0        0      145 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/tts/__init__.py
+-rw-r--r--   0        0        0     4656 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/tts/base.py
+-rw-r--r--   0        0        0     1095 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/tts/mi.py
+-rw-r--r--   0        0        0     1058 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/tts/tetos.py
+-rw-r--r--   0        0        0     2072 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/utils.py
+-rw-r--r--   0        0        0    16525 2024-05-03 05:30:43.428077 xiaogpt-2.70/xiaogpt/xiaogpt.py
+-rw-r--r--   0        0        0    28501 1970-01-01 00:00:00.000000 xiaogpt-2.70/PKG-INFO
```

### Comparing `xiaogpt-2.64/LICENSE` & `xiaogpt-2.70/LICENSE`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.64/README.md` & `xiaogpt-2.70/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 # xiaogpt
 
 [![PyPI](https://img.shields.io/pypi/v/xiaogpt?style=flat-square)](https://pypi.org/project/xiaogpt)
 [![Docker Image Version (latest by date)](https://img.shields.io/docker/v/yihong0618/xiaogpt?color=%23086DCD&label=docker%20image)](https://hub.docker.com/r/yihong0618/xiaogpt)
 
-https://user-images.githubusercontent.com/15976103/226803357-72f87a41-a15b-409e-94f5-e2d262eecd53.mp4
+<https://user-images.githubusercontent.com/15976103/226803357-72f87a41-a15b-409e-94f5-e2d262eecd53.mp4>
 
 Play ChatGPT and other LLM with Xiaomi AI Speaker
 
 ![image](https://user-images.githubusercontent.com/15976103/220028375-c193a859-48a1-4270-95b6-ef540e54a621.png)
 ![image](https://user-images.githubusercontent.com/15976103/226802344-9c71f543-b73c-4a47-8703-4c200c434dec.png)
 
 ## 支持的 AI 类型
 
 - ChatGPT
 - New Bing
 - [ChatGLM](http://open.bigmodel.cn/)
 - [Gemini](https://makersuite.google.com/app/apikey)
 - [Doubao](https://console.volcengine.com/iam/keymanage/)
+- [Moonshot](https://platform.moonshot.cn/docs/api/chat#%E5%BF%AB%E9%80%9F%E5%BC%80%E5%A7%8B)
+- [01](https://platform.lingyiwanwu.com/apikeys)
+- [Llama3](https://console.groq.com/docs/quickstart)
 - [通义千问](https://help.aliyun.com/zh/dashscope/developer-reference/api-details)
 
 ## 获取小米音响DID
-| 系统和Shell   | Linux *sh                                      | Windows CMD用户                        | Windows PowerShell用户                         |
-| ------------- | ---------------------------------------------- | -------------------------------------- | ---------------------------------------------- |
+
+| 系统和Shell  | Linux *sh                                      | Windows CMD用户                        | Windows PowerShell用户                         |
+|------------|------------------------------------------------|----------------------------------------|------------------------------------------------|
 | 1、安装包     | `pip install miservice_fork`                   | `pip install miservice_fork`           | `pip install miservice_fork`                   |
 | 2、设置变量   | `export MI_USER=xxx` <br> `export MI_PASS=xxx` | `set MI_USER=xxx`<br>`set MI_PASS=xxx` | `$env:MI_USER="xxx"` <br> `$env:MI_PASS="xxx"` |
 | 3、取得MI_DID | `micli list`                                   | `micli list`                           | `micli list`                                   |
 | 4、设置MI_DID | `export MI_DID=xxx`                            | `set MI_DID=xxx`                       | `$env:MI_DID="xxx"`                            |
 
 - 注意不同shell 对环境变量的处理是不同的，尤其是powershell赋值时，可能需要双引号来包括值。
 - 如果获取did报错时，请更换一下无线网络，有很大概率解决问题。
@@ -43,21 +47,22 @@
 
 ## 使用
 
 - `pip install -U --force-reinstall xiaogpt[locked]`
 - 参考我 fork 的 [MiService](https://github.com/yihong0618/MiService) 项目 README 并在本地 terminal 跑 `micli list` 拿到你音响的 DID 成功 **别忘了设置 export MI_DID=xxx** 这个 MI_DID 用
 - run `xiaogpt --hardware ${your_hardware} --use_chatgpt_api` hardware 你看小爱屁股上有型号，输入进来，如果在屁股上找不到或者型号不对，可以用 `micli mina` 找到型号
 - 跑起来之后就可以问小爱同学问题了，“帮我"开头的问题，会发送一份给 ChatGPT 然后小爱同学用 tts 回答
-- 如果上面不可用，可以尝试用手机抓包，https://userprofile.mina.mi.com/device_profile/v2/conversation 找到 cookie 利用 `--cookie '${cookie}'` cookie 别忘了用单引号包裹
+- 如果上面不可用，可以尝试用手机抓包，<https://userprofile.mina.mi.com/device_profile/v2/conversation> 找到 cookie 利用 `--cookie '${cookie}'` cookie 别忘了用单引号包裹
 - 默认用目前 ubus, 如果你的设备不支持 ubus 可以使用 `--use_command` 来使用 command 来 tts
 - 使用 `--mute_xiaoai` 选项，可以快速停掉小爱的回答
 - 使用 `--account ${account} --password ${password}`
 - 如果有能力可以自行替换唤醒词，也可以去掉唤醒词
 - 使用 `--use_chatgpt_api` 的 api 那样可以更流畅的对话，速度特别快，达到了对话的体验, [openai api](https://platform.openai.com/account/api-keys), 命令 `--use_chatgpt_api`
 - 如果你遇到了墙需要用 Cloudflare Workers 替换 api_base 请使用 `--api_base ${url}` 来替换。 **请注意，此处你输入的api应该是'`https://xxxx/v1`'的字样，域名需要用引号包裹**
+- `--use_moonshot_api` and other models please refer below
 - 可以跟小爱说 `开始持续对话` 自动进入持续对话状态，`结束持续对话` 结束持续对话状态。
 - 可以使用 `--tts edge` 来获取更好的 tts 能力
 - 可以使用 `--tts openai` 来获取 openai tts 能力
 - 可以使用 `--tts azure --azure_tts_speech_key <your-speech-key>` 来获取 Azure TTS 能力
 - 可以使用 `--use_langchain` 替代 `--use_chatgpt_api` 来调用 LangChain（默认 chatgpt）服务，实现上网检索、数学运算..
 
 e.g.
@@ -75,19 +80,25 @@
 xiaogpt --hardware LX06  --mute_xiaoai --stream
 # 如果你想使用 google 的 gemini
 xiaogpt --hardware LX06  --mute_xiaoai --use_gemini --gemini_key ${gemini_key}
 # 如果你想使用自己的 google gemini 服务
 python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_gemini --gemini_key ${gemini_key} --gemini_api_domain ${gemini_api_domain}
 # 如果你想使用阿里的通义千问
 xiaogpt --hardware LX06  --mute_xiaoai --use_qwen --qwen_key ${qwen_key}
+# 如果你想使用 kimi
+xiaogpt --hardware LX06  --mute_xiaoai --use_moonshot_api --moonshot_api_key ${moonshot_api_key}
+# 如果你想使用 llama3
+xiaogpt --hardware LX06  --mute_xiaoai --use_llama --llama_api_key ${llama_api_key}
+# 如果你想使用 01
+xiaogpt --hardware LX06  --mute_xiaoai --use_yi_api --ti_api_key ${yi_api_key}
 # 如果你想使用豆包
-xiaogpt --hardware LX06  --mute_xiaoai --use_doubao --stream --volc_access_key xxxx --volc_secret_key xxx
-# 如果你想用 edge-tts
-xiaogpt --hardware LX06 --cookie ${cookie} --use_chatgpt_api --tts edge
-# 如果你想使用 LangChain + SerpApi 实现上网检索或其他本地服务（目前仅支持 stream 模式）
+
+
+
+
 export OPENAI_API_KEY=${your_api_key}
 export SERPAPI_API_KEY=${your_serpapi_key}
 xiaogpt --hardware Lx06 --use_langchain --mute_xiaoai --stream --openai_key ${your_api_key} --serpapi_api_key ${your_serpapi_key}
 ```
 
 使用 git clone 运行
 
@@ -106,16 +117,22 @@
 python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_glm --glm_key ${glm_key}
 # 如果你想使用 google 的 gemini
 python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_gemini --gemini_key ${gemini_key}
 # 如果你想使用自己的 google gemini 服务
 python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_gemini --gemini_key ${gemini_key} --gemini_api_domain ${gemini_api_domain}
 # 如果你想使用阿里的通义千问
 python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_qwen --qwen_key ${qwen_key}
+# 如果你想使用 kimi
+xiaogpt --hardware LX06  --mute_xiaoai --use_moonshot_api --moonshot_api_key ${moonshot_api_key}
+# 如果你想使用 01
+xiaogpt --hardware LX06  --mute_xiaoai --use_yi_api --ti_api_key ${yi_api_key}
 # 如果你想使用豆包
 python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_doubao --stream --volc_access_key xxxx --volc_secret_key xxx
+# 如果你想使用 llama3
+python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_llama --llama_api_key ${llama_api_key}
 # 如果你想使用 LangChain+SerpApi 实现上网检索或其他本地服务（目前仅支持 stream 模式）
 export OPENAI_API_KEY=${your_api_key}
 export SERPAPI_API_KEY=${your_serpapi_key}
 python3 xiaogpt.py --hardware Lx06 --use_langchain --mute_xiaoai --stream --openai_key ${your_api_key} --serpapi_api_key ${your_serpapi_key}
 ```
 
 ## config.json
@@ -151,23 +168,26 @@
 ```
 
 具体参数作用请参考 [Open AI API 文档](https://platform.openai.com/docs/api-reference/chat/create)。
 ChatGLM [文档](http://open.bigmodel.cn/doc/api#chatglm_130b)
 
 ## 配置项说明
 
-| 参数                  | 说明                                                                                        | 默认值                                                                                                    | 可选值                                                           |
-| --------------------- | ------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------- |
-| hardware              | 设备型号                                                                                    |                                                                                                           |                                                                  |
-| account               | 小爱账户                                                                                    |                                                                                                           |                                                                  |
-| password              | 小爱账户密码                                                                                |                                                                                                           |                                                                  |
-| openai_key            | openai的apikey                                                                              |                                                                                                           |                                                                  |
-| serpapi_api_key       | serpapi的key 参考 [SerpAPI](https://serpapi.com/)                                           |                                                                                                           |                                                                  |
-| glm_key               | chatglm 的 apikey                                                                           |                                                                                                           |                                                                  |
-| gemini_key            | gemini 的 apikey [参考](https://makersuite.google.com/app/apikey)                           |                                                                                                           |                                                                  |
+| 参数             | 说明                                                                                                       | 默认值 | 可选值 |
+|------------------|-----------------------------------------------------------------------------------------------------------|--------|--------|
+| hardware         | 设备型号                                                                                                   |        |        |
+| account          | 小爱账户                                                                                                   |        |        |
+| password         | 小爱账户密码                                                                                               |        |        |
+| openai_key       | openai的apikey                                                                                             |        |        |
+| moonshot_api_key | moonshot kimi 的 [apikey](https://platform.moonshot.cn/docs/api/chat#%E5%BF%AB%E9%80%9F%E5%BC%80%E5%A7%8B) |        |        |
+| yi_api_key       | 01 wanwu 的 [apikey](https://platform.lingyiwanwu.com/apikeys)                                             |        |        |
+| llama_api_key       | groq 的 llama3 [apikey](https://console.groq.com/docs/quickstart)                                             |        |        |
+| serpapi_api_key  | serpapi的key 参考 [SerpAPI](https://serpapi.com/)                                                          |        |        |
+| glm_key          | chatglm 的 apikey                                                                                          |        |        |
+| gemini_key       | gemini 的 apikey [参考](https://makersuite.google.com/app/apikey)                                          |        |        |
 | gemini_api_domain     | gemini 的自定义域名 [参考](https://github.com/antergone/palm-netlify-proxy)                 |                                                                                                           |
 | qwen_key              | qwen 的 apikey [参考](https://help.aliyun.com/zh/dashscope/developer-reference/api-details) |                                                                                                           |                                                                  |
 | cookie                | 小爱账户cookie （如果用上面密码登录可以不填）                                               |                                                                                                           |                                                                  |
 | mi_did                | 设备did                                                                                     |                                                                                                           |                                                                  |
 | use_command           | 使用 MI command 与小爱交互                                                                  | `false`                                                                                                   |                                                                  |
 | mute_xiaoai           | 快速停掉小爱自己的回答                                                                      | `true`                                                                                                    |                                                                  |
 | verbose               | 是否打印详细日志                                                                            | `false`                                                                                                   |                                                                  |
@@ -184,38 +204,38 @@
 | gpt_options           | OpenAI API 的参数字典                                                                       | `{}`                                                                                                      |                                                                  |
 | bing_cookie_path      | NewBing使用的cookie路径，参考[这里]获取                                                     | 也可通过环境变量 `COOKIE_FILE` 设置                                                                       |                                                                  |
 | bing_cookies          | NewBing使用的cookie字典，参考[这里]获取                                                     |                                                                                                           |                                                                  |
 | deployment_id         | Azure OpenAI 服务的 deployment ID                                                           | 参考这个[如何找到deployment_id](https://github.com/yihong0618/xiaogpt/issues/347#issuecomment-1784410784) |                                                                  |
 | api_base              | 如果需要替换默认的api,或者使用Azure OpenAI 服务                                             | 例如：`https://abc-def.openai.azure.com/`                                                                 |
 | volc_access_key       | 火山引擎的 access key 请在[这里](https://console.volcengine.com/iam/keymanage/)获取         |                                                                                                           |                                                                  |
 | volc_secret_key       | 火山引擎的 secret key 请在[这里](https://console.volcengine.com/iam/keymanage/)获取         |                                                                                                           |                                                                  |
-[这里]: https://github.com/acheong08/EdgeGPT#getting-authentication-required
+[这里]: <https://github.com/acheong08/EdgeGPT#getting-authentication-required>
 
 ## 注意
 
 1. 请开启小爱同学的蓝牙
 2. 如果要更改提示词和 PROMPT 在代码最上面自行更改
 3. 目前已知 LX04、X10A 和 L05B L05C 可能需要使用 `--use_command`，否则可能会出现终端能输出GPT的回复但小爱同学不回答GPT的情况。这几个型号也只支持小爱原本的 tts.
-4. 在wsl使用时, 需要设置代理为 http://wls的ip:port(vpn的代理端口), 否则会出现连接超时的情况, 详情 [报错： Error communicating with OpenAI](https://github.com/yihong0618/xiaogpt/issues/235)
+4. 在wsl使用时, 需要设置代理为 <http://wls的ip:port(vpn的代理端口)>, 否则会出现连接超时的情况, 详情 [报错： Error communicating with OpenAI](https://github.com/yihong0618/xiaogpt/issues/235)
 
 ## QA
 
 1. 用破解么？不用
 2. 你做这玩意也没用啊？确实。。。但是挺好玩的，有用对你来说没用，对我们来说不一定呀
 3. 想把它变得更好？PR Issue always welcome.
 4. 还有问题？提 Issue 哈哈
-5. Exception: Error https://api2.mina.mi.com/admin/v2/device_list?master=0&requestId=app_ios_xxx: Login failed [@KJZH001](https://github.com/KJZH001)<br>
+5. Exception: Error <https://api2.mina.mi.com/admin/v2/device_list?master=0&requestId=app_ios_xxx>: Login failed [@KJZH001](https://github.com/KJZH001)<br>
    这是由于小米风控导致，海外地区无法登录大陆的账户，请尝试cookie登录
    无法抓包的可以在本地部署完毕项目后再用户文件夹`C:\Users\用户名`下面找到.mi.token，然后扔到你无法登录的服务器去<br>
    若是linux则请放到当前用户的home文件夹，此时你可以重新执行先前的命令，不出意外即可正常登录（但cookie可能会过一段时间失效，需要重新获取）<br>
    详情请见 [https://github.com/yihong0618/xiaogpt/issues/332](https://github.com/yihong0618/xiaogpt/issues/332)
 
 ## 视频教程
 
-https://www.youtube.com/watch?v=K4YA8YwzOOA
+<https://www.youtube.com/watch?v=K4YA8YwzOOA>
 
 ## Docker
 
 ### 常规用法
 
 X86/ARM Docker Image: `yihong0618/xiaogpt`
```

### Comparing `xiaogpt-2.64/pyproject.toml` & `xiaogpt-2.70/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,18 @@
     "langchain>=0.0.343",
     "beautifulsoup4>=4.12.0",
     "google-search-results>=2.4.2",
     "google-generativeai",
     "numexpr>=2.8.6",
     "dashscope>=1.10.0",
     "tetos>=0.2.1",
+    "groq>=0.5.0",
 ]
 dynamic = []
-version = "2.64"
+version = "2.70"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/yihong0618/xiaogpt"
 
@@ -51,15 +52,15 @@
     "beautifulsoup4==4.12.3",
     "bingimagecreator==0.5.0",
     "cachetools==5.3.2",
     "certifi==2024.2.2",
     "charset-normalizer==3.3.2",
     "click==8.1.7",
     "colorama==0.4.6 ; platform_system == \"Windows\"",
-    "dashscope==1.17.1",
+    "dashscope==1.18.0",
     "dataclasses-json==0.6.3",
     "distro==1.9.0",
     "edge-tts==6.1.10",
     "edgegpt==0.1.26",
     "exceptiongroup==1.2.0 ; python_version < \"3.11\"",
     "frozenlist==1.4.1",
     "google-ai-generativelanguage==0.6.2",
@@ -69,39 +70,40 @@
     "google-auth==2.26.1",
     "google-auth-httplib2==0.2.0",
     "google-cloud-texttospeech==2.16.3",
     "google-generativeai==0.5.2",
     "google-search-results==2.4.2",
     "googleapis-common-protos==1.62.0",
     "greenlet==3.0.3 ; platform_machine == \"win32\" or platform_machine == \"WIN32\" or platform_machine == \"AMD64\" or platform_machine == \"amd64\" or platform_machine == \"x86_64\" or platform_machine == \"ppc64le\" or platform_machine == \"aarch64\"",
+    "groq==0.5.0",
     "grpcio==1.60.0",
     "grpcio-status==1.60.0",
     "h11==0.14.0",
     "httpcore==1.0.5",
     "httplib2==0.22.0",
     "httpx==0.27.0",
     "httpx[socks]==0.27.0",
     "idna==3.7",
     "jsonpatch==1.33",
     "jsonpointer==2.4",
-    "langchain==0.1.16",
-    "langchain-community==0.0.32",
-    "langchain-core==0.1.42",
+    "langchain==0.1.17",
+    "langchain-community==0.0.36",
+    "langchain-core==0.1.50",
     "langchain-text-splitters==0.0.1",
     "langsmith==0.1.45",
     "markdown-it-py==3.0.0",
     "marshmallow==3.20.1",
     "mdurl==0.1.2",
     "miservice-fork==2.4.3",
     "multidict==6.0.5",
     "mutagen==1.47.0",
     "mypy-extensions==1.0.0",
     "numexpr==2.10.0",
     "numpy==1.26.3",
-    "openai==1.23.2",
+    "openai==1.25.1",
     "orjson==3.10.0",
     "packaging==23.2",
     "prompt-toolkit==3.0.43",
     "proto-plus==1.23.0",
     "protobuf==4.25.1",
     "pyasn1==0.5.1",
     "pyasn1-modules==0.3.0",
@@ -125,15 +127,15 @@
     "typing-extensions==4.9.0",
     "typing-inspect==0.9.0",
     "uritemplate==4.1.1",
     "urllib3==2.1.0",
     "wcwidth==0.2.13",
     "websockets==12.0",
     "yarl==1.9.4",
-    "zhipuai==2.0.1",
+    "zhipuai==2.0.1.20240423.1",
 ]
 
 [tool.pdm]
 plugins = [
     "pdm-autoexport",
 ]
 autoexport = [
```

### Comparing `xiaogpt-2.64/xiaogpt/bot/__init__.py` & `xiaogpt-2.70/xiaogpt/bot/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,24 +4,30 @@
 from xiaogpt.bot.chatgptapi_bot import ChatGPTBot
 from xiaogpt.bot.doubao_bot import DoubaoBot
 from xiaogpt.bot.gemini_bot import GeminiBot
 from xiaogpt.bot.glm_bot import GLMBot
 from xiaogpt.bot.langchain_bot import LangChainBot
 from xiaogpt.bot.newbing_bot import NewBingBot
 from xiaogpt.bot.qwen_bot import QwenBot
+from xiaogpt.bot.moonshot_bot import MoonshotBot
+from xiaogpt.bot.yi_bot import YiBot
+from xiaogpt.bot.llama_bot import LlamaBot
 from xiaogpt.config import Config
 
 BOTS: dict[str, type[BaseBot]] = {
     "newbing": NewBingBot,
     "chatgptapi": ChatGPTBot,
     "glm": GLMBot,
     "gemini": GeminiBot,
     "qwen": QwenBot,
     "langchain": LangChainBot,
     "doubao": DoubaoBot,
+    "moonshot": MoonshotBot,
+    "yi": YiBot,
+    "llama": LlamaBot,
 }
 
 
 def get_bot(config: Config) -> BaseBot:
     try:
         return BOTS[config.bot].from_config(config)
     except KeyError:
@@ -29,12 +35,15 @@
 
 
 __all__ = [
     "ChatGPTBot",
     "NewBingBot",
     "GLMBot",
     "GeminiBot",
+    "MoonshotBot",
     "QwenBot",
     "get_bot",
     "LangChainBot",
     "DoubaoBot",
+    "YiBot",
+    "LlamaBot",
 ]
```

### Comparing `xiaogpt-2.64/xiaogpt/bot/base_bot.py` & `xiaogpt-2.70/xiaogpt/bot/base_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.64/xiaogpt/bot/chatgptapi_bot.py` & `xiaogpt-2.70/xiaogpt/bot/chatgptapi_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.64/xiaogpt/bot/doubao_bot.py` & `xiaogpt-2.70/xiaogpt/bot/doubao_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.64/xiaogpt/bot/gemini_bot.py` & `xiaogpt-2.70/xiaogpt/bot/gemini_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.64/xiaogpt/bot/glm_bot.py` & `xiaogpt-2.70/xiaogpt/bot/glm_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.64/xiaogpt/bot/langchain_bot.py` & `xiaogpt-2.70/xiaogpt/bot/langchain_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.64/xiaogpt/bot/newbing_bot.py` & `xiaogpt-2.70/xiaogpt/bot/newbing_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.64/xiaogpt/bot/qwen_bot.py` & `xiaogpt-2.70/xiaogpt/bot/qwen_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.64/xiaogpt/cli.py` & `xiaogpt-2.70/xiaogpt/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,14 +24,29 @@
     )
     parser.add_argument(
         "--openai_key",
         dest="openai_key",
         help="openai api key",
     )
     parser.add_argument(
+        "--moonshot_api_key",
+        dest="moonshot_api_key",
+        help="Moonshot api key",
+    )
+    parser.add_argument(
+        "--llama_api_key",
+        dest="llama_api_key",
+        help="llama(use groq) api key",
+    )
+    parser.add_argument(
+        "--yi_api_key",
+        dest="yi_api_key",
+        help="01wanwu api key",
+    )
+    parser.add_argument(
         "--glm_key",
         dest="glm_key",
         help="chatglm api key",
     )
     parser.add_argument(
         "--gemini_key",
         dest="gemini_key",
@@ -106,14 +121,28 @@
         "--use_chatgpt_api",
         dest="bot",
         action="store_const",
         const="chatgptapi",
         help="if use openai chatgpt api",
     )
     bot_group.add_argument(
+        "--use_moonshot_api",
+        dest="bot",
+        action="store_const",
+        const="moonshot",
+        help="if use moonshot api",
+    )
+    bot_group.add_argument(
+        "--use_yi_api",
+        dest="bot",
+        action="store_const",
+        const="yi",
+        help="if use yi api",
+    )
+    bot_group.add_argument(
         "--use_langchain",
         dest="bot",
         action="store_const",
         const="langchain",
         help="if use langchain",
     )
     bot_group.add_argument(
@@ -147,14 +176,21 @@
     bot_group.add_argument(
         "--use_doubao",
         dest="bot",
         action="store_const",
         const="doubao",
         help="if use doubao",
     )
+    bot_group.add_argument(
+        "--use_llama",  # use groq
+        dest="bot",
+        action="store_const",
+        const="llama",
+        help="if use groq llama3",
+    )
     parser.add_argument(
         "--bing_cookie_path",
         dest="bing_cookie_path",
         help="new bing cookies path if use new bing",
     )
     bot_group.add_argument(
         "--bot",
@@ -164,14 +200,17 @@
             "chatgptapi",
             "newbing",
             "glm",
             "gemini",
             "langchain",
             "qwen",
             "doubao",
+            "moonshot",
+            "yi",
+            "llama",
         ],
     )
     parser.add_argument(
         "--config",
         dest="config",
         help="config file path",
     )
```

### Comparing `xiaogpt-2.64/xiaogpt/config.py` & `xiaogpt-2.70/xiaogpt/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,29 +33,32 @@
     # add more here
 }
 
 DEFAULT_COMMAND = ("5-1", "5-5")
 
 KEY_WORD = ("帮我", "请")
 CHANGE_PROMPT_KEY_WORD = ("更改提示词",)
-PROMPT = "以下请用100字以内回答，请只回答文字不要带链接"
+PROMPT = "以下请用300字以内回答，请只回答文字不要带链接"
 # simulate_xiaoai_question
 MI_ASK_SIMULATE_DATA = {
     "code": 0,
     "message": "Success",
     "data": '{"bitSet":[0,1,1],"records":[{"bitSet":[0,1,1,1,1],"answers":[{"bitSet":[0,1,1,1],"type":"TTS","tts":{"bitSet":[0,1],"text":"Fake Answer"}}],"time":1677851434593,"query":"Fake Question","requestId":"fada34f8fa0c3f408ee6761ec7391d85"}],"nextEndTime":1677849207387}',
 }
 
 
 @dataclass
 class Config:
     hardware: str = "LX06"
     account: str = os.getenv("MI_USER", "")
     password: str = os.getenv("MI_PASS", "")
     openai_key: str = os.getenv("OPENAI_API_KEY", "")
+    moonshot_api_key: str = os.getenv("MOONSHOT_API_KEY", "")
+    yi_api_key: str = os.getenv("YI_API_KEY", "")
+    llama_api_key: str = os.getenv("GROQ_API_KEY", "")  # use groq
     glm_key: str = os.getenv("CHATGLM_KEY", "")
     gemini_key: str = os.getenv("GEMINI_KEY", "")  # keep the old rule
     qwen_key: str = os.getenv("DASHSCOPE_API_KEY", "")  # keep the old rule
     serpapi_api_key: str = os.getenv("SERPAPI_API_KEY", "")
     gemini_api_domain: str = os.getenv(
         "GEMINI_API_DOMAIN", ""
     )  # 自行部署的 Google Gemini 代理
@@ -153,14 +156,20 @@
                     key, value = "bot", "glm"
                 elif key == "use_gemini":
                     key, value = "bot", "gemini"
                 elif key == "use_qwen":
                     key, value = "bot", "qwen"
                 elif key == "use_doubao":
                     key, value = "bot", "doubao"
+                elif key == "use_moonshot":
+                    key, value = "bot", "moonshot"
+                elif key == "use_yi":
+                    key, value = "bot", "yi"
+                elif key == "use_llama":
+                    key, value = "bot", "llama"
                 elif key == "use_langchain":
                     key, value = "bot", "langchain"
                 elif key == "enable_edge_tts":
                     key, value = "tts", "edge"
                 if key in cls.__dataclass_fields__:
                     result[key] = value
         return result
```

### Comparing `xiaogpt-2.64/xiaogpt/langchain/callbacks.py` & `xiaogpt-2.70/xiaogpt/langchain/callbacks.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.64/xiaogpt/langchain/chain.py` & `xiaogpt-2.70/xiaogpt/langchain/chain.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.64/xiaogpt/langchain/examples/email/mail_box.py` & `xiaogpt-2.70/xiaogpt/langchain/examples/email/mail_box.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.64/xiaogpt/langchain/examples/email/mail_summary_tools.py` & `xiaogpt-2.70/xiaogpt/langchain/examples/email/mail_summary_tools.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.64/xiaogpt/tts/base.py` & `xiaogpt-2.70/xiaogpt/tts/base.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.64/xiaogpt/tts/mi.py` & `xiaogpt-2.70/xiaogpt/tts/mi.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.64/xiaogpt/tts/tetos.py` & `xiaogpt-2.70/xiaogpt/tts/tetos.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.64/xiaogpt/utils.py` & `xiaogpt-2.70/xiaogpt/utils.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.64/xiaogpt/xiaogpt.py` & `xiaogpt-2.70/xiaogpt/xiaogpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -374,22 +374,31 @@
                 print(new_record)
                 self._change_prompt(new_record.get("query", ""))
 
             if not self.need_ask_gpt(new_record):
                 self.log.debug("No new xiao ai record")
                 continue
 
-            # drop 帮我回答
+            # drop key words
             query = re.sub(rf"^({'|'.join(self.config.keyword)})", "", query)
+            # llama3 is not good at Chinese, so we need to add prompt in it.
+            if self.config.bot == "llama":
+                query = f"你是一个基于llama3 的智能助手，请你跟我对话时，一定使用中文，不要夹杂一些英文单词，甚至英语短语也不能随意使用，但类似于 llama3 这样的专属名词除外, 问题是：{query}"
 
             print("-" * 20)
             print("问题：" + query + "？")
             if not self.chatbot.has_history():
                 query = f"{query}，{self.config.prompt}"
-            query += "，并用本段话的language code作为开头，用|分隔，如：en-US|你好……"
+            # some model can not detect the language code, so we need to add it
+
+            if self.config.tts != "mi":  # mi only say Chinese
+                query += (
+                    "，并用本段话的language code作为开头，用|分隔，如：en-US|你好……"
+                )
+
             if self.config.mute_xiaoai:
                 await self.stop_if_xiaoai_is_playing()
             else:
                 # waiting for xiaoai speaker done
                 await asyncio.sleep(8)
             await self.do_tts(f"正在问{self.chatbot.name}请耐心等待")
             try:
```

### Comparing `xiaogpt-2.64/PKG-INFO` & `xiaogpt-2.70/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xiaogpt
-Version: 2.64
+Version: 2.70
 Summary: Play ChatGPT or other LLM with xiaomi AI speaker
 Author-Email: yihong0618 <zouzou0208@gmail.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Homepage, https://github.com/yihong0618/xiaogpt
@@ -19,29 +19,30 @@
 Requires-Dist: langchain>=0.0.343
 Requires-Dist: beautifulsoup4>=4.12.0
 Requires-Dist: google-search-results>=2.4.2
 Requires-Dist: google-generativeai
 Requires-Dist: numexpr>=2.8.6
 Requires-Dist: dashscope>=1.10.0
 Requires-Dist: tetos>=0.2.1
+Requires-Dist: groq>=0.5.0
 Requires-Dist: aiohttp==3.9.5; extra == "locked"
 Requires-Dist: aiosignal==1.3.1; extra == "locked"
 Requires-Dist: annotated-types==0.6.0; extra == "locked"
 Requires-Dist: anyio==4.3.0; extra == "locked"
 Requires-Dist: async-timeout==4.0.3; python_version < "3.11" and extra == "locked"
 Requires-Dist: attrs==23.2.0; extra == "locked"
 Requires-Dist: azure-cognitiveservices-speech==1.37.0; extra == "locked"
 Requires-Dist: beautifulsoup4==4.12.3; extra == "locked"
 Requires-Dist: bingimagecreator==0.5.0; extra == "locked"
 Requires-Dist: cachetools==5.3.2; extra == "locked"
 Requires-Dist: certifi==2024.2.2; extra == "locked"
 Requires-Dist: charset-normalizer==3.3.2; extra == "locked"
 Requires-Dist: click==8.1.7; extra == "locked"
 Requires-Dist: colorama==0.4.6; platform_system == "Windows" and extra == "locked"
-Requires-Dist: dashscope==1.17.1; extra == "locked"
+Requires-Dist: dashscope==1.18.0; extra == "locked"
 Requires-Dist: dataclasses-json==0.6.3; extra == "locked"
 Requires-Dist: distro==1.9.0; extra == "locked"
 Requires-Dist: edge-tts==6.1.10; extra == "locked"
 Requires-Dist: edgegpt==0.1.26; extra == "locked"
 Requires-Dist: exceptiongroup==1.2.0; python_version < "3.11" and extra == "locked"
 Requires-Dist: frozenlist==1.4.1; extra == "locked"
 Requires-Dist: google-ai-generativelanguage==0.6.2; extra == "locked"
@@ -51,39 +52,40 @@
 Requires-Dist: google-auth==2.26.1; extra == "locked"
 Requires-Dist: google-auth-httplib2==0.2.0; extra == "locked"
 Requires-Dist: google-cloud-texttospeech==2.16.3; extra == "locked"
 Requires-Dist: google-generativeai==0.5.2; extra == "locked"
 Requires-Dist: google-search-results==2.4.2; extra == "locked"
 Requires-Dist: googleapis-common-protos==1.62.0; extra == "locked"
 Requires-Dist: greenlet==3.0.3; (platform_machine == "win32" or platform_machine == "WIN32" or platform_machine == "AMD64" or platform_machine == "amd64" or platform_machine == "x86_64" or platform_machine == "ppc64le" or platform_machine == "aarch64") and extra == "locked"
+Requires-Dist: groq==0.5.0; extra == "locked"
 Requires-Dist: grpcio==1.60.0; extra == "locked"
 Requires-Dist: grpcio-status==1.60.0; extra == "locked"
 Requires-Dist: h11==0.14.0; extra == "locked"
 Requires-Dist: httpcore==1.0.5; extra == "locked"
 Requires-Dist: httplib2==0.22.0; extra == "locked"
 Requires-Dist: httpx==0.27.0; extra == "locked"
 Requires-Dist: httpx[socks]==0.27.0; extra == "locked"
 Requires-Dist: idna==3.7; extra == "locked"
 Requires-Dist: jsonpatch==1.33; extra == "locked"
 Requires-Dist: jsonpointer==2.4; extra == "locked"
-Requires-Dist: langchain==0.1.16; extra == "locked"
-Requires-Dist: langchain-community==0.0.32; extra == "locked"
-Requires-Dist: langchain-core==0.1.42; extra == "locked"
+Requires-Dist: langchain==0.1.17; extra == "locked"
+Requires-Dist: langchain-community==0.0.36; extra == "locked"
+Requires-Dist: langchain-core==0.1.50; extra == "locked"
 Requires-Dist: langchain-text-splitters==0.0.1; extra == "locked"
 Requires-Dist: langsmith==0.1.45; extra == "locked"
 Requires-Dist: markdown-it-py==3.0.0; extra == "locked"
 Requires-Dist: marshmallow==3.20.1; extra == "locked"
 Requires-Dist: mdurl==0.1.2; extra == "locked"
 Requires-Dist: miservice-fork==2.4.3; extra == "locked"
 Requires-Dist: multidict==6.0.5; extra == "locked"
 Requires-Dist: mutagen==1.47.0; extra == "locked"
 Requires-Dist: mypy-extensions==1.0.0; extra == "locked"
 Requires-Dist: numexpr==2.10.0; extra == "locked"
 Requires-Dist: numpy==1.26.3; extra == "locked"
-Requires-Dist: openai==1.23.2; extra == "locked"
+Requires-Dist: openai==1.25.1; extra == "locked"
 Requires-Dist: orjson==3.10.0; extra == "locked"
 Requires-Dist: packaging==23.2; extra == "locked"
 Requires-Dist: prompt-toolkit==3.0.43; extra == "locked"
 Requires-Dist: proto-plus==1.23.0; extra == "locked"
 Requires-Dist: protobuf==4.25.1; extra == "locked"
 Requires-Dist: pyasn1==0.5.1; extra == "locked"
 Requires-Dist: pyasn1-modules==0.3.0; extra == "locked"
@@ -107,42 +109,46 @@
 Requires-Dist: typing-extensions==4.9.0; extra == "locked"
 Requires-Dist: typing-inspect==0.9.0; extra == "locked"
 Requires-Dist: uritemplate==4.1.1; extra == "locked"
 Requires-Dist: urllib3==2.1.0; extra == "locked"
 Requires-Dist: wcwidth==0.2.13; extra == "locked"
 Requires-Dist: websockets==12.0; extra == "locked"
 Requires-Dist: yarl==1.9.4; extra == "locked"
-Requires-Dist: zhipuai==2.0.1; extra == "locked"
+Requires-Dist: zhipuai==2.0.1.20240423.1; extra == "locked"
 Provides-Extra: locked
 Description-Content-Type: text/markdown
 
 # xiaogpt
 
 [![PyPI](https://img.shields.io/pypi/v/xiaogpt?style=flat-square)](https://pypi.org/project/xiaogpt)
 [![Docker Image Version (latest by date)](https://img.shields.io/docker/v/yihong0618/xiaogpt?color=%23086DCD&label=docker%20image)](https://hub.docker.com/r/yihong0618/xiaogpt)
 
-https://user-images.githubusercontent.com/15976103/226803357-72f87a41-a15b-409e-94f5-e2d262eecd53.mp4
+<https://user-images.githubusercontent.com/15976103/226803357-72f87a41-a15b-409e-94f5-e2d262eecd53.mp4>
 
 Play ChatGPT and other LLM with Xiaomi AI Speaker
 
 ![image](https://user-images.githubusercontent.com/15976103/220028375-c193a859-48a1-4270-95b6-ef540e54a621.png)
 ![image](https://user-images.githubusercontent.com/15976103/226802344-9c71f543-b73c-4a47-8703-4c200c434dec.png)
 
 ## 支持的 AI 类型
 
 - ChatGPT
 - New Bing
 - [ChatGLM](http://open.bigmodel.cn/)
 - [Gemini](https://makersuite.google.com/app/apikey)
 - [Doubao](https://console.volcengine.com/iam/keymanage/)
+- [Moonshot](https://platform.moonshot.cn/docs/api/chat#%E5%BF%AB%E9%80%9F%E5%BC%80%E5%A7%8B)
+- [01](https://platform.lingyiwanwu.com/apikeys)
+- [Llama3](https://console.groq.com/docs/quickstart)
 - [通义千问](https://help.aliyun.com/zh/dashscope/developer-reference/api-details)
 
 ## 获取小米音响DID
-| 系统和Shell   | Linux *sh                                      | Windows CMD用户                        | Windows PowerShell用户                         |
-| ------------- | ---------------------------------------------- | -------------------------------------- | ---------------------------------------------- |
+
+| 系统和Shell  | Linux *sh                                      | Windows CMD用户                        | Windows PowerShell用户                         |
+|------------|------------------------------------------------|----------------------------------------|------------------------------------------------|
 | 1、安装包     | `pip install miservice_fork`                   | `pip install miservice_fork`           | `pip install miservice_fork`                   |
 | 2、设置变量   | `export MI_USER=xxx` <br> `export MI_PASS=xxx` | `set MI_USER=xxx`<br>`set MI_PASS=xxx` | `$env:MI_USER="xxx"` <br> `$env:MI_PASS="xxx"` |
 | 3、取得MI_DID | `micli list`                                   | `micli list`                           | `micli list`                                   |
 | 4、设置MI_DID | `export MI_DID=xxx`                            | `set MI_DID=xxx`                       | `$env:MI_DID="xxx"`                            |
 
 - 注意不同shell 对环境变量的处理是不同的，尤其是powershell赋值时，可能需要双引号来包括值。
 - 如果获取did报错时，请更换一下无线网络，有很大概率解决问题。
@@ -160,21 +166,22 @@
 
 ## 使用
 
 - `pip install -U --force-reinstall xiaogpt[locked]`
 - 参考我 fork 的 [MiService](https://github.com/yihong0618/MiService) 项目 README 并在本地 terminal 跑 `micli list` 拿到你音响的 DID 成功 **别忘了设置 export MI_DID=xxx** 这个 MI_DID 用
 - run `xiaogpt --hardware ${your_hardware} --use_chatgpt_api` hardware 你看小爱屁股上有型号，输入进来，如果在屁股上找不到或者型号不对，可以用 `micli mina` 找到型号
 - 跑起来之后就可以问小爱同学问题了，“帮我"开头的问题，会发送一份给 ChatGPT 然后小爱同学用 tts 回答
-- 如果上面不可用，可以尝试用手机抓包，https://userprofile.mina.mi.com/device_profile/v2/conversation 找到 cookie 利用 `--cookie '${cookie}'` cookie 别忘了用单引号包裹
+- 如果上面不可用，可以尝试用手机抓包，<https://userprofile.mina.mi.com/device_profile/v2/conversation> 找到 cookie 利用 `--cookie '${cookie}'` cookie 别忘了用单引号包裹
 - 默认用目前 ubus, 如果你的设备不支持 ubus 可以使用 `--use_command` 来使用 command 来 tts
 - 使用 `--mute_xiaoai` 选项，可以快速停掉小爱的回答
 - 使用 `--account ${account} --password ${password}`
 - 如果有能力可以自行替换唤醒词，也可以去掉唤醒词
 - 使用 `--use_chatgpt_api` 的 api 那样可以更流畅的对话，速度特别快，达到了对话的体验, [openai api](https://platform.openai.com/account/api-keys), 命令 `--use_chatgpt_api`
 - 如果你遇到了墙需要用 Cloudflare Workers 替换 api_base 请使用 `--api_base ${url}` 来替换。 **请注意，此处你输入的api应该是'`https://xxxx/v1`'的字样，域名需要用引号包裹**
+- `--use_moonshot_api` and other models please refer below
 - 可以跟小爱说 `开始持续对话` 自动进入持续对话状态，`结束持续对话` 结束持续对话状态。
 - 可以使用 `--tts edge` 来获取更好的 tts 能力
 - 可以使用 `--tts openai` 来获取 openai tts 能力
 - 可以使用 `--tts azure --azure_tts_speech_key <your-speech-key>` 来获取 Azure TTS 能力
 - 可以使用 `--use_langchain` 替代 `--use_chatgpt_api` 来调用 LangChain（默认 chatgpt）服务，实现上网检索、数学运算..
 
 e.g.
@@ -192,19 +199,25 @@
 xiaogpt --hardware LX06  --mute_xiaoai --stream
 # 如果你想使用 google 的 gemini
 xiaogpt --hardware LX06  --mute_xiaoai --use_gemini --gemini_key ${gemini_key}
 # 如果你想使用自己的 google gemini 服务
 python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_gemini --gemini_key ${gemini_key} --gemini_api_domain ${gemini_api_domain}
 # 如果你想使用阿里的通义千问
 xiaogpt --hardware LX06  --mute_xiaoai --use_qwen --qwen_key ${qwen_key}
+# 如果你想使用 kimi
+xiaogpt --hardware LX06  --mute_xiaoai --use_moonshot_api --moonshot_api_key ${moonshot_api_key}
+# 如果你想使用 llama3
+xiaogpt --hardware LX06  --mute_xiaoai --use_llama --llama_api_key ${llama_api_key}
+# 如果你想使用 01
+xiaogpt --hardware LX06  --mute_xiaoai --use_yi_api --ti_api_key ${yi_api_key}
 # 如果你想使用豆包
-xiaogpt --hardware LX06  --mute_xiaoai --use_doubao --stream --volc_access_key xxxx --volc_secret_key xxx
-# 如果你想用 edge-tts
-xiaogpt --hardware LX06 --cookie ${cookie} --use_chatgpt_api --tts edge
-# 如果你想使用 LangChain + SerpApi 实现上网检索或其他本地服务（目前仅支持 stream 模式）
+
+
+
+
 export OPENAI_API_KEY=${your_api_key}
 export SERPAPI_API_KEY=${your_serpapi_key}
 xiaogpt --hardware Lx06 --use_langchain --mute_xiaoai --stream --openai_key ${your_api_key} --serpapi_api_key ${your_serpapi_key}
 ```
 
 使用 git clone 运行
 
@@ -223,16 +236,22 @@
 python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_glm --glm_key ${glm_key}
 # 如果你想使用 google 的 gemini
 python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_gemini --gemini_key ${gemini_key}
 # 如果你想使用自己的 google gemini 服务
 python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_gemini --gemini_key ${gemini_key} --gemini_api_domain ${gemini_api_domain}
 # 如果你想使用阿里的通义千问
 python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_qwen --qwen_key ${qwen_key}
+# 如果你想使用 kimi
+xiaogpt --hardware LX06  --mute_xiaoai --use_moonshot_api --moonshot_api_key ${moonshot_api_key}
+# 如果你想使用 01
+xiaogpt --hardware LX06  --mute_xiaoai --use_yi_api --ti_api_key ${yi_api_key}
 # 如果你想使用豆包
 python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_doubao --stream --volc_access_key xxxx --volc_secret_key xxx
+# 如果你想使用 llama3
+python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_llama --llama_api_key ${llama_api_key}
 # 如果你想使用 LangChain+SerpApi 实现上网检索或其他本地服务（目前仅支持 stream 模式）
 export OPENAI_API_KEY=${your_api_key}
 export SERPAPI_API_KEY=${your_serpapi_key}
 python3 xiaogpt.py --hardware Lx06 --use_langchain --mute_xiaoai --stream --openai_key ${your_api_key} --serpapi_api_key ${your_serpapi_key}
 ```
 
 ## config.json
@@ -268,23 +287,26 @@
 ```
 
 具体参数作用请参考 [Open AI API 文档](https://platform.openai.com/docs/api-reference/chat/create)。
 ChatGLM [文档](http://open.bigmodel.cn/doc/api#chatglm_130b)
 
 ## 配置项说明
 
-| 参数                  | 说明                                                                                        | 默认值                                                                                                    | 可选值                                                           |
-| --------------------- | ------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------- |
-| hardware              | 设备型号                                                                                    |                                                                                                           |                                                                  |
-| account               | 小爱账户                                                                                    |                                                                                                           |                                                                  |
-| password              | 小爱账户密码                                                                                |                                                                                                           |                                                                  |
-| openai_key            | openai的apikey                                                                              |                                                                                                           |                                                                  |
-| serpapi_api_key       | serpapi的key 参考 [SerpAPI](https://serpapi.com/)                                           |                                                                                                           |                                                                  |
-| glm_key               | chatglm 的 apikey                                                                           |                                                                                                           |                                                                  |
-| gemini_key            | gemini 的 apikey [参考](https://makersuite.google.com/app/apikey)                           |                                                                                                           |                                                                  |
+| 参数             | 说明                                                                                                       | 默认值 | 可选值 |
+|------------------|-----------------------------------------------------------------------------------------------------------|--------|--------|
+| hardware         | 设备型号                                                                                                   |        |        |
+| account          | 小爱账户                                                                                                   |        |        |
+| password         | 小爱账户密码                                                                                               |        |        |
+| openai_key       | openai的apikey                                                                                             |        |        |
+| moonshot_api_key | moonshot kimi 的 [apikey](https://platform.moonshot.cn/docs/api/chat#%E5%BF%AB%E9%80%9F%E5%BC%80%E5%A7%8B) |        |        |
+| yi_api_key       | 01 wanwu 的 [apikey](https://platform.lingyiwanwu.com/apikeys)                                             |        |        |
+| llama_api_key       | groq 的 llama3 [apikey](https://console.groq.com/docs/quickstart)                                             |        |        |
+| serpapi_api_key  | serpapi的key 参考 [SerpAPI](https://serpapi.com/)                                                          |        |        |
+| glm_key          | chatglm 的 apikey                                                                                          |        |        |
+| gemini_key       | gemini 的 apikey [参考](https://makersuite.google.com/app/apikey)                                          |        |        |
 | gemini_api_domain     | gemini 的自定义域名 [参考](https://github.com/antergone/palm-netlify-proxy)                 |                                                                                                           |
 | qwen_key              | qwen 的 apikey [参考](https://help.aliyun.com/zh/dashscope/developer-reference/api-details) |                                                                                                           |                                                                  |
 | cookie                | 小爱账户cookie （如果用上面密码登录可以不填）                                               |                                                                                                           |                                                                  |
 | mi_did                | 设备did                                                                                     |                                                                                                           |                                                                  |
 | use_command           | 使用 MI command 与小爱交互                                                                  | `false`                                                                                                   |                                                                  |
 | mute_xiaoai           | 快速停掉小爱自己的回答                                                                      | `true`                                                                                                    |                                                                  |
 | verbose               | 是否打印详细日志                                                                            | `false`                                                                                                   |                                                                  |
@@ -301,38 +323,38 @@
 | gpt_options           | OpenAI API 的参数字典                                                                       | `{}`                                                                                                      |                                                                  |
 | bing_cookie_path      | NewBing使用的cookie路径，参考[这里]获取                                                     | 也可通过环境变量 `COOKIE_FILE` 设置                                                                       |                                                                  |
 | bing_cookies          | NewBing使用的cookie字典，参考[这里]获取                                                     |                                                                                                           |                                                                  |
 | deployment_id         | Azure OpenAI 服务的 deployment ID                                                           | 参考这个[如何找到deployment_id](https://github.com/yihong0618/xiaogpt/issues/347#issuecomment-1784410784) |                                                                  |
 | api_base              | 如果需要替换默认的api,或者使用Azure OpenAI 服务                                             | 例如：`https://abc-def.openai.azure.com/`                                                                 |
 | volc_access_key       | 火山引擎的 access key 请在[这里](https://console.volcengine.com/iam/keymanage/)获取         |                                                                                                           |                                                                  |
 | volc_secret_key       | 火山引擎的 secret key 请在[这里](https://console.volcengine.com/iam/keymanage/)获取         |                                                                                                           |                                                                  |
-[这里]: https://github.com/acheong08/EdgeGPT#getting-authentication-required
+[这里]: <https://github.com/acheong08/EdgeGPT#getting-authentication-required>
 
 ## 注意
 
 1. 请开启小爱同学的蓝牙
 2. 如果要更改提示词和 PROMPT 在代码最上面自行更改
 3. 目前已知 LX04、X10A 和 L05B L05C 可能需要使用 `--use_command`，否则可能会出现终端能输出GPT的回复但小爱同学不回答GPT的情况。这几个型号也只支持小爱原本的 tts.
-4. 在wsl使用时, 需要设置代理为 http://wls的ip:port(vpn的代理端口), 否则会出现连接超时的情况, 详情 [报错： Error communicating with OpenAI](https://github.com/yihong0618/xiaogpt/issues/235)
+4. 在wsl使用时, 需要设置代理为 <http://wls的ip:port(vpn的代理端口)>, 否则会出现连接超时的情况, 详情 [报错： Error communicating with OpenAI](https://github.com/yihong0618/xiaogpt/issues/235)
 
 ## QA
 
 1. 用破解么？不用
 2. 你做这玩意也没用啊？确实。。。但是挺好玩的，有用对你来说没用，对我们来说不一定呀
 3. 想把它变得更好？PR Issue always welcome.
 4. 还有问题？提 Issue 哈哈
-5. Exception: Error https://api2.mina.mi.com/admin/v2/device_list?master=0&requestId=app_ios_xxx: Login failed [@KJZH001](https://github.com/KJZH001)<br>
+5. Exception: Error <https://api2.mina.mi.com/admin/v2/device_list?master=0&requestId=app_ios_xxx>: Login failed [@KJZH001](https://github.com/KJZH001)<br>
    这是由于小米风控导致，海外地区无法登录大陆的账户，请尝试cookie登录
    无法抓包的可以在本地部署完毕项目后再用户文件夹`C:\Users\用户名`下面找到.mi.token，然后扔到你无法登录的服务器去<br>
    若是linux则请放到当前用户的home文件夹，此时你可以重新执行先前的命令，不出意外即可正常登录（但cookie可能会过一段时间失效，需要重新获取）<br>
    详情请见 [https://github.com/yihong0618/xiaogpt/issues/332](https://github.com/yihong0618/xiaogpt/issues/332)
 
 ## 视频教程
 
-https://www.youtube.com/watch?v=K4YA8YwzOOA
+<https://www.youtube.com/watch?v=K4YA8YwzOOA>
 
 ## Docker
 
 ### 常规用法
 
 X86/ARM Docker Image: `yihong0618/xiaogpt`
```


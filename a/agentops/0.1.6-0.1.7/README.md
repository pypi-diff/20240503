# Comparing `tmp/agentops-0.1.6.tar.gz` & `tmp/agentops-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentops-0.1.6.tar", last modified: Sat Apr 20 03:48:53 2024, max compression
+gzip compressed data, was "agentops-0.1.7.tar", last modified: Fri May  3 19:21:33 2024, max compression
```

## Comparing `agentops-0.1.6.tar` & `agentops-0.1.7.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:48:53.968020 agentops-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-20 03:48:49.000000 agentops-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6827 2024-04-20 03:48:53.968020 agentops-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-04-20 03:48:49.000000 agentops-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:48:53.964020 agentops-0.1.6/agentops/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3373 2024-04-20 03:48:49.000000 agentops-0.1.6/agentops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-20 03:48:49.000000 agentops-0.1.6/agentops/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    13264 2024-04-20 03:48:49.000000 agentops-0.1.6/agentops/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-04-20 03:48:49.000000 agentops-0.1.6/agentops/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-20 03:48:49.000000 agentops-0.1.6/agentops/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-20 03:48:49.000000 agentops-0.1.6/agentops/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     5979 2024-04-20 03:48:49.000000 agentops-0.1.6/agentops/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-04-20 03:48:49.000000 agentops-0.1.6/agentops/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-20 03:48:49.000000 agentops-0.1.6/agentops/host_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-04-20 03:48:49.000000 agentops-0.1.6/agentops/http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    21947 2024-04-20 03:48:49.000000 agentops-0.1.6/agentops/langchain_callback_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    12003 2024-04-20 03:48:49.000000 agentops-0.1.6/agentops/llm_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-20 03:48:49.000000 agentops-0.1.6/agentops/log_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-20 03:48:49.000000 agentops-0.1.6/agentops/meta_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-20 03:48:49.000000 agentops-0.1.6/agentops/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-04-20 03:48:49.000000 agentops-0.1.6/agentops/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:48:53.964020 agentops-0.1.6/agentops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6827 2024-04-20 03:48:53.000000 agentops-0.1.6/agentops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-20 03:48:53.000000 agentops-0.1.6/agentops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 03:48:53.000000 agentops-0.1.6/agentops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-20 03:48:53.000000 agentops-0.1.6/agentops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-20 03:48:53.000000 agentops-0.1.6/agentops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-20 03:48:49.000000 agentops-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 03:48:53.968020 agentops-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:48:53.964020 agentops-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-20 03:48:49.000000 agentops-0.1.6/tests/test_canary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-20 03:48:49.000000 agentops-0.1.6/tests/test_patcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-20 03:48:49.000000 agentops-0.1.6/tests/test_record_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-20 03:48:49.000000 agentops-0.1.6/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-20 03:48:49.000000 agentops-0.1.6/tests/test_teardown.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:21:33.291933 agentops-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-03 19:21:28.000000 agentops-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8706 2024-05-03 19:21:33.291933 agentops-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7774 2024-05-03 19:21:28.000000 agentops-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:21:33.287933 agentops-0.1.7/agentops/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4857 2024-05-03 19:21:28.000000 agentops-0.1.7/agentops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-03 19:21:28.000000 agentops-0.1.7/agentops/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14941 2024-05-03 19:21:28.000000 agentops-0.1.7/agentops/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-05-03 19:21:28.000000 agentops-0.1.7/agentops/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-03 19:21:28.000000 agentops-0.1.7/agentops/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-03 19:21:28.000000 agentops-0.1.7/agentops/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-05-03 19:21:28.000000 agentops-0.1.7/agentops/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-03 19:21:28.000000 agentops-0.1.7/agentops/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-03 19:21:28.000000 agentops-0.1.7/agentops/host_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-05-03 19:21:28.000000 agentops-0.1.7/agentops/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21947 2024-05-03 19:21:28.000000 agentops-0.1.7/agentops/langchain_callback_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14616 2024-05-03 19:21:28.000000 agentops-0.1.7/agentops/llm_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-03 19:21:28.000000 agentops-0.1.7/agentops/log_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-03 19:21:28.000000 agentops-0.1.7/agentops/meta_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-03 19:21:28.000000 agentops-0.1.7/agentops/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-05-03 19:21:28.000000 agentops-0.1.7/agentops/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:21:33.291933 agentops-0.1.7/agentops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8706 2024-05-03 19:21:33.000000 agentops-0.1.7/agentops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-03 19:21:33.000000 agentops-0.1.7/agentops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 19:21:33.000000 agentops-0.1.7/agentops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-03 19:21:33.000000 agentops-0.1.7/agentops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-03 19:21:33.000000 agentops-0.1.7/agentops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-03 19:21:28.000000 agentops-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 19:21:33.291933 agentops-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:21:33.287933 agentops-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-03 19:21:28.000000 agentops-0.1.7/tests/test_canary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-03 19:21:28.000000 agentops-0.1.7/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-03 19:21:28.000000 agentops-0.1.7/tests/test_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-05-03 19:21:28.000000 agentops-0.1.7/tests/test_record_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-05-03 19:21:28.000000 agentops-0.1.7/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-03 19:21:28.000000 agentops-0.1.7/tests/test_teardown.py
```

### Comparing `agentops-0.1.6/LICENSE` & `agentops-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `agentops-0.1.6/PKG-INFO` & `agentops-0.1.7/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,11 @@
-Metadata-Version: 2.1
-Name: agentops
-Version: 0.1.6
-Summary: Python SDK for developing AI agent evals and observability
-Author-email: Alex Reibman <areibman@gmail.com>, Shawn Qiu <siyangqiu@gmail.com>, Braelyn Boynton <bboynton97@gmail.com>, Howard Gil <howardbgil@gmail.com>
-Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
-Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests==2.31.0
-Requires-Dist: psutil==5.9.8
-Requires-Dist: packaging==23.2
-Provides-Extra: dev
-Requires-Dist: pytest==7.4.0; extra == "dev"
-Requires-Dist: requests_mock==1.11.0; extra == "dev"
-Provides-Extra: langchain
-Requires-Dist: langchain>=0.0.354; extra == "langchain"
-
 <div align="center">
-  <img src="logo.png" style="margin: 15px; max-width: 300px" width="50%" alt="Logo">
+  <a href="https://agentops.ai?ref=gh">
+    <img src="logo.png" style="margin: 15px; max-width: 300px" width="50%" alt="Logo">
+  </a>
 </div>
 <p align="center">
   <em>AI agents suck. We’re fixing that.</em>
 </p>
 
 <p align="center">
     <a href="https://pypi.org/project/agentops/" target="_blank">
@@ -34,44 +14,55 @@
     </a>
 </p>
 <p align="center">
 <a href="https://twitter.com/agentopsai/">🐦 Twitter</a>
 <span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
 <a href="https://discord.gg/JHPt4C7r">📢 Discord</a>
 <span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
-<a href="https://app.agentops.ai/?=gh">🖇️ AgentOps</a>
+<a href="https://app.agentops.ai/?ref=gh">🖇️ AgentOps</a>
 <span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
 <a href="https://docs.agentops.ai/introduction">📙 Documentation</a>
 </p>
 
-# AgentOps
-
-Build your next agent with benchmarks, observability, and replay analytics. AgentOps is the toolkit for evaluating and developing robust and reliable AI agents.
-
-You can sign up for AgentOps [here](https://app.agentops.ai).
+# AgentOps 🖇️
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) ![PyPI - Version](https://img.shields.io/pypi/v/agentops) <a href="https://pepy.tech/project/agentops">
   <img src="https://static.pepy.tech/badge/agentops/month"> <a href="https://twitter.com/agentopsai">
     <img src="https://img.shields.io/badge/follow-%40agentops-1DA1F2?logo=twitter&style=social" alt="AgentOps Twitter" /> 
   </a>
-<a href="https://discord.gg/mKW3ZhN9p2">
+  <a href="https://discord.gg/mKW3ZhN9p2">
     <img src="https://img.shields.io/badge/chat-on%20Discord-blueviolet" alt="Discord community channel" />
   </a>
-  <a href="mailto:investor@agentops.ai"><img src="https://img.shields.io/website?color=%23f26522&down_message=Y%20Combinator&label=Not%20Backed%20By&logo=ycombinator&style=flat-square&up_message=Y%20Combinator&url=https%3A%2F%2Fwww.ycombinator.com"></a>
-<a href="https://github.com/agentops-ai/agentops/issues">
+  <a href="mailto:investor@agentops.ai"><img src="https://img.shields.io/website?color=%23f26522&down_message=Y%20Combinator&label=Not%20Backed%20By&logo=ycombinator&style=flat-square&up_message=Y%20Combinator&url=https%3A%2F%2Fwww.ycombinator.com"/>
+  <a href="https://github.com/agentops-ai/agentops/issues">
     <img src="https://img.shields.io/github/commit-activity/m/agentops-ai/agentops" alt="git commit activity" />
   </a>
+
+
+AgentOps helps developers build, evaluate, and monitor AI agents. Tools to build agents from prototype to production.
+
+
+|||
+|------------------------------------------|----------------------------------------------------|
+| 📊 **Replay Analytics and Debugging** | Step-by-step agent execution graphs |
+| 💸 **LLM Cost Management**   | Track spend with LLM foundation model providers |
+| 🧪 **Agent Benchmarking** | Test your agents against 1,000+ evals |
+| 🔐 **Compliance and Security**            | Detect common prompt injection and data exfiltration exploits |
+| 🤝 **Framework Integrations**            | Easily plugs in with frameworks like CrewAI and LangChain |
+
 ## Quick Start ⌨️
 
-```pip install agentops```
+```python
+pip install agentops
+```
 
 ### Session replays in 3 lines of code
-Initialize the AgentOps client, and automatically get analytics on every LLM call.
+Initialize the AgentOps client and automatically get analytics on every LLM call.
 
-```python python
+```python
 import agentops
 
 # Beginning of program's code (i.e. main.py, __init__.py)
 agentops.init(<INSERT YOUR API KEY HERE>)
 
 ...
 # (optional: record specific functions)
@@ -80,46 +71,52 @@
     ...
 
 # End of program
 agentops.end_session('Success')
 # Woohoo You're done 🎉
 ```
 
-Refer to our [API documentation](http://docs.agentops.ai) for detailed instructions.
+All your sessions are available on the [AgentOps dashboard](https://app.agentops.ai?ref=gh). Refer to our [API documentation](http://docs.agentops.ai) for detailed instructions.
 
-## Time travel debugging 🔮
-(coming soon!)
 
-## Agent Arena 🥊
-(coming soon!)
+<details open>
+  <summary>Agent Dashboard</summary>
+  <a href="https://app.agentops.ai?ref=gh">
+   <img src="https://github.com/AgentOps-AI/agentops/assets/14807319/158e082a-9a7d-49b7-9b41-51a49a1f7d3d" style="width: 90%;" alt="Agent Dashboard"/>
+  </a>
+</details>
 
-## Evaluations Roadmap 🧭
+<details>
+  <summary>Session Analytics</summary>
+  <a href="https://app.agentops.ai?ref=gh">
+    <img src="https://github.com/AgentOps-AI/agentops/assets/14807319/d7228019-1488-40d3-852f-a61e998658ad" style="width: 90%;" alt="Session Analytics"/>
+  </a>
+</details>
 
-| Platform | Dashboard | Evals |
-|---|---|---|
-|✅ Python SDK | ✅ Multi-session and Cross-session metrics | ✅ Custom eval metrics |
-|🚧 Evaluation builder API | ✅ Custom event tag tracking | 🔜 Agent scorecards |
-|✅ [Javascript/Typescript SDK](https://github.com/AgentOps-AI/agentops-node) | ✅ Session replays| 🔜 Evaluation playground + leaderboard|
+<details>
+  <summary>Session Replays</summary>
+  <a href="https://app.agentops.ai?ref=gh">
+    <img src="https://github.com/AgentOps-AI/agentops/assets/14807319/561d59f3-c441-4066-914b-f6cfe32a598c" style="width: 90%;" alt="Session Replays"/>
+  </a>
+</details>
 
+## Integrations 🦾
 
-## Debugging Roadmap 🧭
+### CrewAI 🛶
 
-| Performance testing | Environments | LLM Testing | Reasoning and execution testing |
-|---|---|---|---|
-|✅ Event latency analysis | 🔜 Non-stationary environment testing | 🔜 LLM non-deterministic function detection | 🚧 Infinite loops and recursive thought detection |
-|✅ Agent workflow execution pricing | 🔜 Multi-modal environments | 🚧 Token limit overflow flags | 🔜 Faulty reasoning detection |
-|🚧 Success validators (external) | 🔜 Execution containers | 🔜 Context limit overflow flags | 🔜 Generative code validators |
-|🔜 Agent controllers/skill tests | ✅ Honeypot and prompt injection detection ([PromptArmor](https://promptarmor.com)) | 🔜 API bill tracking | 🔜 Error breakpoint analysis |
-|🔜 Information context constraint testing | 🔜 Anti-agent roadblocks (i.e. Captchas) | 🔜 CI/CD integration checks | |
-|🔜 Regression testing | 🔜 Multi-agent framework visualization | | |
+Build Crew agents with observability with only 2 lines of code. Simply set an `AGENTOPS_API_KEY` in your environment, and your crews will get automatic monitoring on the AgentOps dashboard.
+
+AgentOps is officially supported on Crew's latest rc branch: `crewai==0.28.9rc1`
+
+* [AgentOps integration example](https://docs.agentops.ai/v1/integrations/crewai)
+* [Offical CrewAI documentation](https://docs.crewai.com/how-to/AgentOps-Observability)
 
-## Callback handlers ↩️
 
-### Langchain
-AgentOps works seemlessly with applications built using Langchain. To use the handler, install Langchain as an optional dependency:
+### Langchain 🦜🔗
+AgentOps works seamlessly with applications built using Langchain. To use the handler, install Langchain as an optional dependency:
 ```shell
 pip install agentops[langchain]
 ```
 
 To use the handler, import and set
 
 ```python
@@ -141,18 +138,45 @@
                          verbose=True,
                          callbacks=[handler], # You must pass in a callback handler to record your agent
                          handle_parsing_errors=True)
 ```
 
 Check out the [Langchain Examples Notebook](./examples/langchain_examples.ipynb) for more details including Async handlers.
 
-### LlamaIndex 
+### LlamaIndex 🦙
 (Coming Soon)
 
 
+
+## Time travel debugging 🔮
+(coming soon!)
+
+## Agent Arena 🥊
+(coming soon!)
+
+## Evaluations Roadmap 🧭
+
+| Platform | Dashboard | Evals |
+|---|---|---|
+|✅ Python SDK | ✅ Multi-session and Cross-session metrics | ✅ Custom eval metrics |
+|🚧 Evaluation builder API | ✅ Custom event tag tracking | 🔜 Agent scorecards |
+|✅ [Javascript/Typescript SDK](https://github.com/AgentOps-AI/agentops-node) | ✅ Session replays| 🔜 Evaluation playground + leaderboard|
+
+
+## Debugging Roadmap 🧭
+
+| Performance testing | Environments | LLM Testing | Reasoning and execution testing |
+|---|---|---|---|
+|✅ Event latency analysis | 🔜 Non-stationary environment testing | 🔜 LLM non-deterministic function detection | 🚧 Infinite loops and recursive thought detection |
+|✅ Agent workflow execution pricing | 🔜 Multi-modal environments | 🚧 Token limit overflow flags | 🔜 Faulty reasoning detection |
+|🚧 Success validators (external) | 🔜 Execution containers | 🔜 Context limit overflow flags | 🔜 Generative code validators |
+|🔜 Agent controllers/skill tests | ✅ Honeypot and prompt injection detection ([PromptArmor](https://promptarmor.com)) | 🔜 API bill tracking | 🔜 Error breakpoint analysis |
+|🔜 Information context constraint testing | 🔜 Anti-agent roadblocks (i.e. Captchas) | 🔜 CI/CD integration checks | |
+|🔜 Regression testing | 🔜 Multi-agent framework visualization | | |
+
 ### Why AgentOps? 🤔
 
-Our mission is to bring your agent from protype to production.
+Our mission is to bring your agent from prototype to production.
 
 Agent developers often work with little to no visibility into agent testing performance. This means their agents never leave the lab. We're changing that. 
 
 AgentOps is the easiest way to evaluate, grade, and test agents. Is there a feature you'd like to see AgentOps cover? Just raise it in the issues tab, and we'll work on adding it to the roadmap.
```

#### html2text {}

```diff
@@ -1,75 +1,75 @@
-Metadata-Version: 2.1 Name: agentops Version: 0.1.6 Summary: Python SDK for
-developing AI agent evals and observability Author-email: Alex Reibman
-gmail.com>, Shawn Qiu
-gmail.com>, Braelyn Boynton
-gmail.com>, Howard Gil
-gmail.com> Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
-Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues Classifier:
-Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
-License Classifier: Operating System :: OS Independent Requires-Python: >=3.7
-Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-requests==2.31.0 Requires-Dist: psutil==5.9.8 Requires-Dist: packaging==23.2
-Provides-Extra: dev Requires-Dist: pytest==7.4.0; extra == "dev" Requires-Dist:
-requests_mock==1.11.0; extra == "dev" Provides-Extra: langchain Requires-Dist:
-langchain>=0.0.354; extra == "langchain"
-                                    [Logo]
+                                    _[_L_o_g_o_]
                      AAII aaggeennttss ssuucckk.. WWee?â??rree ffiixxiinngg tthhaatt..
                                _[_P_y_t_h_o_n_]_[_V_e_r_s_i_o_n_]
     _ð___¦_ _T_w_i_t_t_e_r   â¢   _ð___¢_ _D_i_s_c_o_r_d   â¢   _ð____ï_¸__ _A_g_e_n_t_O_p_s   â¢   _ð___
                                  _D_o_c_u_m_e_n_t_a_t_i_o_n
-# AgentOps Build your next agent with benchmarks, observability, and replay
-analytics. AgentOps is the toolkit for evaluating and developing robust and
-reliable AI agents. You can sign up for AgentOps [here](https://
-app.agentops.ai). [![License: MIT](https://img.shields.io/badge/License-MIT-
+# AgentOps ðï¸ [![License: MIT](https://img.shields.io/badge/License-MIT-
 yellow.svg)](https://opensource.org/licenses/MIT) ![PyPI - Version](https://
 img.shields.io/pypi/v/agentops) _[_h_t_t_p_s_:_/_/_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_a_g_e_n_t_o_p_s_/_m_o_n_t_h_]
 _[_A_g_e_n_t_O_p_s_ _T_w_i_t_t_e_r_]_[_D_i_s_c_o_r_d_ _c_o_m_m_u_n_i_t_y_ _c_h_a_n_n_e_l_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _w_e_b_s_i_t_e_?_c_o_l_o_r_=_%_2_3_f_2_6_5_2_2_&_d_o_w_n___m_e_s_s_a_g_e_=_Y_%_2_0_C_o_m_b_i_n_a_t_o_r_&_l_a_b_e_l_=_N_o_t_%_2_0_B_a_c_k_e_d_%_2_0_B_y_&_l_o_g_o_=_y_c_o_m_b_i_n_a_t_o_r_&_s_t_y_l_e_=_f_l_a_t_-
 _s_q_u_a_r_e_&_u_p___m_e_s_s_a_g_e_=_Y_%_2_0_C_o_m_b_i_n_a_t_o_r_&_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_w_w_w_._y_c_o_m_b_i_n_a_t_o_r_._c_o_m_]_[_g_i_t
-_c_o_m_m_i_t_ _a_c_t_i_v_i_t_y_]_#_#_ _Q_u_i_c_k_ _S_t_a_r_t_ _â__¨_ï_¸__ _`_`_`_p_i_p_ _i_n_s_t_a_l_l_ _a_g_e_n_t_o_p_s_`_`_`_ _#_#_#_ _S_e_s_s_i_o_n
-_r_e_p_l_a_y_s_ _i_n_ _3_ _l_i_n_e_s_ _o_f_ _c_o_d_e_ _I_n_i_t_i_a_l_i_z_e_ _t_h_e_ _A_g_e_n_t_O_p_s_ _c_l_i_e_n_t_,_ _a_n_d_ _a_u_t_o_m_a_t_i_c_a_l_l_y
-_g_e_t_ _a_n_a_l_y_t_i_c_s_ _o_n_ _e_v_e_r_y_ _L_L_M_ _c_a_l_l_._ _`_`_`_p_y_t_h_o_n_ _p_y_t_h_o_n_ _i_m_p_o_r_t_ _a_g_e_n_t_o_p_s_ _#_ _B_e_g_i_n_n_i_n_g
-_o_f_ _p_r_o_g_r_a_m_'_s_ _c_o_d_e_ _(_i_._e_._ _m_a_i_n_._p_y_,_ _____i_n_i_t_____._p_y_)_ _a_g_e_n_t_o_p_s_._i_n_i_t_(_)_ _._._._ _#_ _(_o_p_t_i_o_n_a_l_:
-_r_e_c_o_r_d_ _s_p_e_c_i_f_i_c_ _f_u_n_c_t_i_o_n_s_)_ _@_a_g_e_n_t_o_p_s_._r_e_c_o_r_d___f_u_n_c_t_i_o_n_(_'_s_a_m_p_l_e_ _f_u_n_c_t_i_o_n_ _b_e_i_n_g
-_r_e_c_o_r_d_'_)_ _d_e_f_ _s_a_m_p_l_e___f_u_n_c_t_i_o_n_(_._._._)_:_ _._._._ _#_ _E_n_d_ _o_f_ _p_r_o_g_r_a_m_ _a_g_e_n_t_o_p_s_._e_n_d___s_e_s_s_i_o_n
-_(_'_S_u_c_c_e_s_s_'_)_ _#_ _W_o_o_h_o_o_ _Y_o_u_'_r_e_ _d_o_n_e_ _ð____ _`_`_`_ _R_e_f_e_r_ _t_o_ _o_u_r_ _[_A_P_I_ _d_o_c_u_m_e_n_t_a_t_i_o_n_]
-_(_h_t_t_p_:_/_/_d_o_c_s_._a_g_e_n_t_o_p_s_._a_i_)_ _f_o_r_ _d_e_t_a_i_l_e_d_ _i_n_s_t_r_u_c_t_i_o_n_s_._ _#_#_ _T_i_m_e_ _t_r_a_v_e_l_ _d_e_b_u_g_g_i_n_g
-_ð___®_ _(_c_o_m_i_n_g_ _s_o_o_n_!_)_ _#_#_ _A_g_e_n_t_ _A_r_e_n_a_ _ð__¥__ _(_c_o_m_i_n_g_ _s_o_o_n_!_)_ _#_#_ _E_v_a_l_u_a_t_i_o_n_s_ _R_o_a_d_m_a_p
-_ð__§_­_ _|_ _P_l_a_t_f_o_r_m_ _|_ _D_a_s_h_b_o_a_r_d_ _|_ _E_v_a_l_s_ _|_ _|_-_-_-_|_-_-_-_|_-_-_-_|_ _|_â___ _P_y_t_h_o_n_ _S_D_K_ _|_ _â__
-_M_u_l_t_i_-_s_e_s_s_i_o_n_ _a_n_d_ _C_r_o_s_s_-_s_e_s_s_i_o_n_ _m_e_t_r_i_c_s_ _|_ _â___ _C_u_s_t_o_m_ _e_v_a_l_ _m_e_t_r_i_c_s_ _|_ _|_ð___§
-_E_v_a_l_u_a_t_i_o_n_ _b_u_i_l_d_e_r_ _A_P_I_ _|_ _â___ _C_u_s_t_o_m_ _e_v_e_n_t_ _t_a_g_ _t_r_a_c_k_i_n_g_Â_ _|_ _ð____ _A_g_e_n_t_ _s_c_o_r_e_c_a_r_d_s
-_|_ _|_â___ _[_J_a_v_a_s_c_r_i_p_t_/_T_y_p_e_s_c_r_i_p_t_ _S_D_K_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_A_g_e_n_t_O_p_s_-_A_I_/_a_g_e_n_t_o_p_s_-
-_n_o_d_e_)_ _|_ _â___ _S_e_s_s_i_o_n_ _r_e_p_l_a_y_s_|_ _ð____ _E_v_a_l_u_a_t_i_o_n_ _p_l_a_y_g_r_o_u_n_d_ _+_ _l_e_a_d_e_r_b_o_a_r_d_|_ _#_#
-_D_e_b_u_g_g_i_n_g_ _R_o_a_d_m_a_p_ _ð__§_­_ _|_ _P_e_r_f_o_r_m_a_n_c_e_ _t_e_s_t_i_n_g_ _|_ _E_n_v_i_r_o_n_m_e_n_t_s_ _|_ _L_L_M_ _T_e_s_t_i_n_g_ _|
-_R_e_a_s_o_n_i_n_g_ _a_n_d_ _e_x_e_c_u_t_i_o_n_ _t_e_s_t_i_n_g_ _|_ _|_-_-_-_|_-_-_-_|_-_-_-_|_-_-_-_|_ _|_â___ _E_v_e_n_t_ _l_a_t_e_n_c_y_ _a_n_a_l_y_s_i_s
-_|_ _ð____ _N_o_n_-_s_t_a_t_i_o_n_a_r_y_ _e_n_v_i_r_o_n_m_e_n_t_ _t_e_s_t_i_n_g_ _|_ _ð____ _L_L_M_ _n_o_n_-_d_e_t_e_r_m_i_n_i_s_t_i_c_ _f_u_n_c_t_i_o_n
-_d_e_t_e_c_t_i_o_n_ _|_ _ð___§_ _I_n_f_i_n_i_t_e_ _l_o_o_p_s_ _a_n_d_ _r_e_c_u_r_s_i_v_e_ _t_h_o_u_g_h_t_ _d_e_t_e_c_t_i_o_n_ _|_ _|_â___ _A_g_e_n_t
-_w_o_r_k_f_l_o_w_ _e_x_e_c_u_t_i_o_n_ _p_r_i_c_i_n_g_ _|_ _ð____ _M_u_l_t_i_-_m_o_d_a_l_ _e_n_v_i_r_o_n_m_e_n_t_s_ _|_ _ð___§_ _T_o_k_e_n_ _l_i_m_i_t
-_o_v_e_r_f_l_o_w_ _f_l_a_g_s_ _|_ _ð____ _F_a_u_l_t_y_ _r_e_a_s_o_n_i_n_g_ _d_e_t_e_c_t_i_o_n_ _|_ _|_ð___§_ _S_u_c_c_e_s_s_ _v_a_l_i_d_a_t_o_r_s_ 
-_(_e_x_t_e_r_n_a_l_)_ _|_ _ð____ _E_x_e_c_u_t_i_o_n_ _c_o_n_t_a_i_n_e_r_s_ _|_ _ð____ _C_o_n_t_e_x_t_ _l_i_m_i_t_ _o_v_e_r_f_l_o_w_ _f_l_a_g_s_ _|
-_ð____ _G_e_n_e_r_a_t_i_v_e_ _c_o_d_e_ _v_a_l_i_d_a_t_o_r_s_ _|_ _|_ð____ _A_g_e_n_t_ _c_o_n_t_r_o_l_l_e_r_s_/_s_k_i_l_l_ _t_e_s_t_s_ _|_ _â__
-_H_o_n_e_y_p_o_t_ _a_n_d_ _p_r_o_m_p_t_ _i_n_j_e_c_t_i_o_n_ _d_e_t_e_c_t_i_o_n_ _(_[_P_r_o_m_p_t_A_r_m_o_r_]_(_h_t_t_p_s_:_/_/
-_p_r_o_m_p_t_a_r_m_o_r_._c_o_m_)_)_ _|_ _ð____ _A_P_I_ _b_i_l_l_ _t_r_a_c_k_i_n_g_ _|_ _ð____ _E_r_r_o_r_ _b_r_e_a_k_p_o_i_n_t_ _a_n_a_l_y_s_i_s_ _|
-_|_ð____ _I_n_f_o_r_m_a_t_i_o_n_ _c_o_n_t_e_x_t_ _c_o_n_s_t_r_a_i_n_t_ _t_e_s_t_i_n_g_ _|_ _ð____ _A_n_t_i_-_a_g_e_n_t_ _r_o_a_d_b_l_o_c_k_s_ _(_i_._e_.
-_C_a_p_t_c_h_a_s_)_ _|_ _ð____ _C_I_/_C_D_ _i_n_t_e_g_r_a_t_i_o_n_ _c_h_e_c_k_s_ _|_ _|_ _|_ð____ _R_e_g_r_e_s_s_i_o_n_ _t_e_s_t_i_n_g_ _|_ _ð___
-_M_u_l_t_i_-_a_g_e_n_t_ _f_r_a_m_e_w_o_r_k_ _v_i_s_u_a_l_i_z_a_t_i_o_n_ _|_ _|_ _|_ _#_#_ _C_a_l_l_b_a_c_k_ _h_a_n_d_l_e_r_s_ _â__©_ï_¸__ _#_#_#
-_L_a_n_g_c_h_a_i_n_ _A_g_e_n_t_O_p_s_ _w_o_r_k_s_ _s_e_e_m_l_e_s_s_l_y_ _w_i_t_h_ _a_p_p_l_i_c_a_t_i_o_n_s_ _b_u_i_l_t_ _u_s_i_n_g_ _L_a_n_g_c_h_a_i_n_._ _T_o
-_u_s_e_ _t_h_e_ _h_a_n_d_l_e_r_,_ _i_n_s_t_a_l_l_ _L_a_n_g_c_h_a_i_n_ _a_s_ _a_n_ _o_p_t_i_o_n_a_l_ _d_e_p_e_n_d_e_n_c_y_:_ _`_`_`_s_h_e_l_l_ _p_i_p
-_i_n_s_t_a_l_l_ _a_g_e_n_t_o_p_s_[_l_a_n_g_c_h_a_i_n_]_ _`_`_`_ _T_o_ _u_s_e_ _t_h_e_ _h_a_n_d_l_e_r_,_ _i_m_p_o_r_t_ _a_n_d_ _s_e_t_ _`_`_`_p_y_t_h_o_n
-_i_m_p_o_r_t_ _o_s_ _f_r_o_m_ _l_a_n_g_c_h_a_i_n_._c_h_a_t___m_o_d_e_l_s_ _i_m_p_o_r_t_ _C_h_a_t_O_p_e_n_A_I_ _f_r_o_m_ _l_a_n_g_c_h_a_i_n_._a_g_e_n_t_s
-_i_m_p_o_r_t_ _i_n_i_t_i_a_l_i_z_e___a_g_e_n_t_,_ _A_g_e_n_t_T_y_p_e_ _f_r_o_m_ _a_g_e_n_t_o_p_s_._l_a_n_g_c_h_a_i_n___c_a_l_l_b_a_c_k___h_a_n_d_l_e_r
-_i_m_p_o_r_t_ _L_a_n_g_c_h_a_i_n_C_a_l_l_b_a_c_k_H_a_n_d_l_e_r_ _A_G_E_N_T_O_P_S___A_P_I___K_E_Y_ _=_ _o_s_._e_n_v_i_r_o_n
-_[_'_A_G_E_N_T_O_P_S___A_P_I___K_E_Y_'_]_ _h_a_n_d_l_e_r_ _=_ _L_a_n_g_c_h_a_i_n_C_a_l_l_b_a_c_k_H_a_n_d_l_e_r
-_(_a_p_i___k_e_y_=_A_G_E_N_T_O_P_S___A_P_I___K_E_Y_,_ _t_a_g_s_=_[_'_L_a_n_g_c_h_a_i_n_ _E_x_a_m_p_l_e_'_]_)_ _l_l_m_ _=_ _C_h_a_t_O_p_e_n_A_I
-_(_o_p_e_n_a_i___a_p_i___k_e_y_=_O_P_E_N_A_I___A_P_I___K_E_Y_,_ _c_a_l_l_b_a_c_k_s_=_[_h_a_n_d_l_e_r_]_,_ _m_o_d_e_l_=_'_g_p_t_-_3_._5_-_t_u_r_b_o_'_)
-_a_g_e_n_t_ _=_ _i_n_i_t_i_a_l_i_z_e___a_g_e_n_t_(_t_o_o_l_s_,_ _l_l_m_,
+_c_o_m_m_i_t_ _a_c_t_i_v_i_t_y_]_A_g_e_n_t_O_p_s_ _h_e_l_p_s_ _d_e_v_e_l_o_p_e_r_s_ _b_u_i_l_d_,_ _e_v_a_l_u_a_t_e_,_ _a_n_d_ _m_o_n_i_t_o_r_ _A_I
+_a_g_e_n_t_s_._ _T_o_o_l_s_ _t_o_ _b_u_i_l_d_ _a_g_e_n_t_s_ _f_r_o_m_ _p_r_o_t_o_t_y_p_e_ _t_o_ _p_r_o_d_u_c_t_i_o_n_._ _|_|_|_ _|_-_-_-_-_-_-_-_-_-_-_-_-_-_-
+_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_|_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-
+_-_-_|_ _|_ _ð____ _*_*_R_e_p_l_a_y_ _A_n_a_l_y_t_i_c_s_ _a_n_d_ _D_e_b_u_g_g_i_n_g_*_*_ _|_ _S_t_e_p_-_b_y_-_s_t_e_p_ _a_g_e_n_t_ _e_x_e_c_u_t_i_o_n
+_g_r_a_p_h_s_ _|_ _|_ _ð___¸_ _*_*_L_L_M_ _C_o_s_t_ _M_a_n_a_g_e_m_e_n_t_*_*_ _|_ _T_r_a_c_k_ _s_p_e_n_d_ _w_i_t_h_ _L_L_M_ _f_o_u_n_d_a_t_i_o_n_ _m_o_d_e_l
+_p_r_o_v_i_d_e_r_s_ _|_ _|_ _ð__§_ª_ _*_*_A_g_e_n_t_ _B_e_n_c_h_m_a_r_k_i_n_g_*_*_ _|_ _T_e_s_t_ _y_o_u_r_ _a_g_e_n_t_s_ _a_g_a_i_n_s_t_ _1_,_0_0_0_+
+_e_v_a_l_s_ _|_ _|_ _ð____ _*_*_C_o_m_p_l_i_a_n_c_e_ _a_n_d_ _S_e_c_u_r_i_t_y_*_*_ _|_ _D_e_t_e_c_t_ _c_o_m_m_o_n_ _p_r_o_m_p_t_ _i_n_j_e_c_t_i_o_n_ _a_n_d
+_d_a_t_a_ _e_x_f_i_l_t_r_a_t_i_o_n_ _e_x_p_l_o_i_t_s_ _|_ _|_ _ð__¤__ _*_*_F_r_a_m_e_w_o_r_k_ _I_n_t_e_g_r_a_t_i_o_n_s_*_*_ _|_ _E_a_s_i_l_y_ _p_l_u_g_s
+_i_n_ _w_i_t_h_ _f_r_a_m_e_w_o_r_k_s_ _l_i_k_e_ _C_r_e_w_A_I_ _a_n_d_ _L_a_n_g_C_h_a_i_n_ _|_ _#_#_ _Q_u_i_c_k_ _S_t_a_r_t_ _â__¨_ï_¸__ _`_`_`_p_y_t_h_o_n
+_p_i_p_ _i_n_s_t_a_l_l_ _a_g_e_n_t_o_p_s_ _`_`_`_ _#_#_#_ _S_e_s_s_i_o_n_ _r_e_p_l_a_y_s_ _i_n_ _3_ _l_i_n_e_s_ _o_f_ _c_o_d_e_ _I_n_i_t_i_a_l_i_z_e_ _t_h_e
+_A_g_e_n_t_O_p_s_ _c_l_i_e_n_t_ _a_n_d_ _a_u_t_o_m_a_t_i_c_a_l_l_y_ _g_e_t_ _a_n_a_l_y_t_i_c_s_ _o_n_ _e_v_e_r_y_ _L_L_M_ _c_a_l_l_._ _`_`_`_p_y_t_h_o_n
+_i_m_p_o_r_t_ _a_g_e_n_t_o_p_s_ _#_ _B_e_g_i_n_n_i_n_g_ _o_f_ _p_r_o_g_r_a_m_'_s_ _c_o_d_e_ _(_i_._e_._ _m_a_i_n_._p_y_,_ _____i_n_i_t_____._p_y_)
+_a_g_e_n_t_o_p_s_._i_n_i_t_(_)_ _._._._ _#_ _(_o_p_t_i_o_n_a_l_:_ _r_e_c_o_r_d_ _s_p_e_c_i_f_i_c_ _f_u_n_c_t_i_o_n_s_)
+_@_a_g_e_n_t_o_p_s_._r_e_c_o_r_d___f_u_n_c_t_i_o_n_(_'_s_a_m_p_l_e_ _f_u_n_c_t_i_o_n_ _b_e_i_n_g_ _r_e_c_o_r_d_'_)_ _d_e_f_ _s_a_m_p_l_e___f_u_n_c_t_i_o_n
+_(_._._._)_:_ _._._._ _#_ _E_n_d_ _o_f_ _p_r_o_g_r_a_m_ _a_g_e_n_t_o_p_s_._e_n_d___s_e_s_s_i_o_n_(_'_S_u_c_c_e_s_s_'_)_ _#_ _W_o_o_h_o_o_ _Y_o_u_'_r_e
+_d_o_n_e_ _ð____ _`_`_`_ _A_l_l_ _y_o_u_r_ _s_e_s_s_i_o_n_s_ _a_r_e_ _a_v_a_i_l_a_b_l_e_ _o_n_ _t_h_e_ _[_A_g_e_n_t_O_p_s_ _d_a_s_h_b_o_a_r_d_]
+_(_h_t_t_p_s_:_/_/_a_p_p_._a_g_e_n_t_o_p_s_._a_i_?_r_e_f_=_g_h_)_._ _R_e_f_e_r_ _t_o_ _o_u_r_ _[_A_P_I_ _d_o_c_u_m_e_n_t_a_t_i_o_n_]_(_h_t_t_p_:_/_/
+_d_o_c_s_._a_g_e_n_t_o_p_s_._a_i_)_ _f_o_r_ _d_e_t_a_i_l_e_d_ _i_n_s_t_r_u_c_t_i_o_n_s_._ _A_g_e_n_t_ _D_a_s_h_b_o_a_r_d_ _[_A_g_e_n_t
+_D_a_s_h_b_o_a_r_d_]_S_e_s_s_i_o_n_ _A_n_a_l_y_t_i_c_s_ _[_S_e_s_s_i_o_n_ _A_n_a_l_y_t_i_c_s_]_S_e_s_s_i_o_n_ _R_e_p_l_a_y_s_ _[_S_e_s_s_i_o_n
+_R_e_p_l_a_y_s_]_#_#_ _I_n_t_e_g_r_a_t_i_o_n_s_ _ð__¦_¾_ _#_#_#_ _C_r_e_w_A_I_ _ð___¶_ _B_u_i_l_d_ _C_r_e_w_ _a_g_e_n_t_s_ _w_i_t_h
+_o_b_s_e_r_v_a_b_i_l_i_t_y_ _w_i_t_h_ _o_n_l_y_ _2_ _l_i_n_e_s_ _o_f_ _c_o_d_e_._ _S_i_m_p_l_y_ _s_e_t_ _a_n_ _`_A_G_E_N_T_O_P_S___A_P_I___K_E_Y_`_ _i_n
+_y_o_u_r_ _e_n_v_i_r_o_n_m_e_n_t_,_ _a_n_d_ _y_o_u_r_ _c_r_e_w_s_ _w_i_l_l_ _g_e_t_ _a_u_t_o_m_a_t_i_c_ _m_o_n_i_t_o_r_i_n_g_ _o_n_ _t_h_e_ _A_g_e_n_t_O_p_s
+_d_a_s_h_b_o_a_r_d_._ _A_g_e_n_t_O_p_s_ _i_s_ _o_f_f_i_c_i_a_l_l_y_ _s_u_p_p_o_r_t_e_d_ _o_n_ _C_r_e_w_'_s_ _l_a_t_e_s_t_ _r_c_ _b_r_a_n_c_h_:
+_`_c_r_e_w_a_i_=_=_0_._2_8_._9_r_c_1_`_ _*_ _[_A_g_e_n_t_O_p_s_ _i_n_t_e_g_r_a_t_i_o_n_ _e_x_a_m_p_l_e_]_(_h_t_t_p_s_:_/_/_d_o_c_s_._a_g_e_n_t_o_p_s_._a_i_/
+_v_1_/_i_n_t_e_g_r_a_t_i_o_n_s_/_c_r_e_w_a_i_)_ _*_ _[_O_f_f_i_c_a_l_ _C_r_e_w_A_I_ _d_o_c_u_m_e_n_t_a_t_i_o_n_]_(_h_t_t_p_s_:_/_/
+_d_o_c_s_._c_r_e_w_a_i_._c_o_m_/_h_o_w_-_t_o_/_A_g_e_n_t_O_p_s_-_O_b_s_e_r_v_a_b_i_l_i_t_y_)_ _#_#_#_ _L_a_n_g_c_h_a_i_n_ _ð__¦__ð____ _A_g_e_n_t_O_p_s
+_w_o_r_k_s_ _s_e_a_m_l_e_s_s_l_y_ _w_i_t_h_ _a_p_p_l_i_c_a_t_i_o_n_s_ _b_u_i_l_t_ _u_s_i_n_g_ _L_a_n_g_c_h_a_i_n_._ _T_o_ _u_s_e_ _t_h_e_ _h_a_n_d_l_e_r_,
+_i_n_s_t_a_l_l_ _L_a_n_g_c_h_a_i_n_ _a_s_ _a_n_ _o_p_t_i_o_n_a_l_ _d_e_p_e_n_d_e_n_c_y_:_ _`_`_`_s_h_e_l_l_ _p_i_p_ _i_n_s_t_a_l_l_ _a_g_e_n_t_o_p_s
+_[_l_a_n_g_c_h_a_i_n_]_ _`_`_`_ _T_o_ _u_s_e_ _t_h_e_ _h_a_n_d_l_e_r_,_ _i_m_p_o_r_t_ _a_n_d_ _s_e_t_ _`_`_`_p_y_t_h_o_n_ _i_m_p_o_r_t_ _o_s_ _f_r_o_m
+_l_a_n_g_c_h_a_i_n_._c_h_a_t___m_o_d_e_l_s_ _i_m_p_o_r_t_ _C_h_a_t_O_p_e_n_A_I_ _f_r_o_m_ _l_a_n_g_c_h_a_i_n_._a_g_e_n_t_s_ _i_m_p_o_r_t
+_i_n_i_t_i_a_l_i_z_e___a_g_e_n_t_,_ _A_g_e_n_t_T_y_p_e_ _f_r_o_m_ _a_g_e_n_t_o_p_s_._l_a_n_g_c_h_a_i_n___c_a_l_l_b_a_c_k___h_a_n_d_l_e_r_ _i_m_p_o_r_t
+_L_a_n_g_c_h_a_i_n_C_a_l_l_b_a_c_k_H_a_n_d_l_e_r_ _A_G_E_N_T_O_P_S___A_P_I___K_E_Y_ _=_ _o_s_._e_n_v_i_r_o_n_[_'_A_G_E_N_T_O_P_S___A_P_I___K_E_Y_'_]
+_h_a_n_d_l_e_r_ _=_ _L_a_n_g_c_h_a_i_n_C_a_l_l_b_a_c_k_H_a_n_d_l_e_r_(_a_p_i___k_e_y_=_A_G_E_N_T_O_P_S___A_P_I___K_E_Y_,_ _t_a_g_s_=_[_'_L_a_n_g_c_h_a_i_n
+_E_x_a_m_p_l_e_'_]_)_ _l_l_m_ _=_ _C_h_a_t_O_p_e_n_A_I_(_o_p_e_n_a_i___a_p_i___k_e_y_=_O_P_E_N_A_I___A_P_I___K_E_Y_,_ _c_a_l_l_b_a_c_k_s_=_[_h_a_n_d_l_e_r_]_,
+_m_o_d_e_l_=_'_g_p_t_-_3_._5_-_t_u_r_b_o_'_)_ _a_g_e_n_t_ _=_ _i_n_i_t_i_a_l_i_z_e___a_g_e_n_t_(_t_o_o_l_s_,_ _l_l_m_,
 _a_g_e_n_t_=_A_g_e_n_t_T_y_p_e_._C_H_A_T___Z_E_R_O___S_H_O_T___R_E_A_C_T___D_E_S_C_R_I_P_T_I_O_N_,_ _v_e_r_b_o_s_e_=_T_r_u_e_,_ _c_a_l_l_b_a_c_k_s_=
 _[_h_a_n_d_l_e_r_]_,_ _#_ _Y_o_u_ _m_u_s_t_ _p_a_s_s_ _i_n_ _a_ _c_a_l_l_b_a_c_k_ _h_a_n_d_l_e_r_ _t_o_ _r_e_c_o_r_d_ _y_o_u_r_ _a_g_e_n_t
 _h_a_n_d_l_e___p_a_r_s_i_n_g___e_r_r_o_r_s_=_T_r_u_e_)_ _`_`_`_ _C_h_e_c_k_ _o_u_t_ _t_h_e_ _[_L_a_n_g_c_h_a_i_n_ _E_x_a_m_p_l_e_s_ _N_o_t_e_b_o_o_k_]_(_._/
 _e_x_a_m_p_l_e_s_/_l_a_n_g_c_h_a_i_n___e_x_a_m_p_l_e_s_._i_p_y_n_b_)_ _f_o_r_ _m_o_r_e_ _d_e_t_a_i_l_s_ _i_n_c_l_u_d_i_n_g_ _A_s_y_n_c_ _h_a_n_d_l_e_r_s_.
-_#_#_#_ _L_l_a_m_a_I_n_d_e_x_ _(_C_o_m_i_n_g_ _S_o_o_n_)_ _#_#_#_ _W_h_y_ _A_g_e_n_t_O_p_s_?_ _ð__¤__ _O_u_r_ _m_i_s_s_i_o_n_ _i_s_ _t_o_ _b_r_i_n_g
-_y_o_u_r_ _a_g_e_n_t_ _f_r_o_m_ _p_r_o_t_y_p_e_ _t_o_ _p_r_o_d_u_c_t_i_o_n_._ _A_g_e_n_t_ _d_e_v_e_l_o_p_e_r_s_ _o_f_t_e_n_ _w_o_r_k_ _w_i_t_h_ _l_i_t_t_l_e
-_t_o_ _n_o_ _v_i_s_i_b_i_l_i_t_y_ _i_n_t_o_ _a_g_e_n_t_ _t_e_s_t_i_n_g_ _p_e_r_f_o_r_m_a_n_c_e_._ _T_h_i_s_ _m_e_a_n_s_ _t_h_e_i_r_ _a_g_e_n_t_s_ _n_e_v_e_r
-_l_e_a_v_e_ _t_h_e_ _l_a_b_._ _W_e_'_r_e_ _c_h_a_n_g_i_n_g_ _t_h_a_t_._ _A_g_e_n_t_O_p_s_ _i_s_ _t_h_e_ _e_a_s_i_e_s_t_ _w_a_y_ _t_o_ _e_v_a_l_u_a_t_e_,
-_g_r_a_d_e_,_ _a_n_d_ _t_e_s_t_ _a_g_e_n_t_s_._ _I_s_ _t_h_e_r_e_ _a_ _f_e_a_t_u_r_e_ _y_o_u_'_d_ _l_i_k_e_ _t_o_ _s_e_e_ _A_g_e_n_t_O_p_s_ _c_o_v_e_r_?
-_J_u_s_t_ _r_a_i_s_e_ _i_t_ _i_n_ _t_h_e_ _i_s_s_u_e_s_ _t_a_b_,_ _a_n_d_ _w_e_'_l_l_ _w_o_r_k_ _o_n_ _a_d_d_i_n_g_ _i_t_ _t_o_ _t_h_e_ _r_o_a_d_m_a_p_.
+_#_#_#_ _L_l_a_m_a_I_n_d_e_x_ _ð__¦__ _(_C_o_m_i_n_g_ _S_o_o_n_)_ _#_#_ _T_i_m_e_ _t_r_a_v_e_l_ _d_e_b_u_g_g_i_n_g_ _ð___®_ _(_c_o_m_i_n_g_ _s_o_o_n_!_)
+_#_#_ _A_g_e_n_t_ _A_r_e_n_a_ _ð__¥__ _(_c_o_m_i_n_g_ _s_o_o_n_!_)_ _#_#_ _E_v_a_l_u_a_t_i_o_n_s_ _R_o_a_d_m_a_p_ _ð__§_­_ _|_ _P_l_a_t_f_o_r_m_ _|
+_D_a_s_h_b_o_a_r_d_ _|_ _E_v_a_l_s_ _|_ _|_-_-_-_|_-_-_-_|_-_-_-_|_ _|_â___ _P_y_t_h_o_n_ _S_D_K_ _|_ _â___ _M_u_l_t_i_-_s_e_s_s_i_o_n_ _a_n_d
+_C_r_o_s_s_-_s_e_s_s_i_o_n_ _m_e_t_r_i_c_s_ _|_ _â___ _C_u_s_t_o_m_ _e_v_a_l_ _m_e_t_r_i_c_s_ _|_ _|_ð___§_ _E_v_a_l_u_a_t_i_o_n_ _b_u_i_l_d_e_r_ _A_P_I
+_|_ _â___ _C_u_s_t_o_m_ _e_v_e_n_t_ _t_a_g_ _t_r_a_c_k_i_n_g_Â_ _|_ _ð____ _A_g_e_n_t_ _s_c_o_r_e_c_a_r_d_s_ _|_ _|_â___ _[_J_a_v_a_s_c_r_i_p_t_/
+_T_y_p_e_s_c_r_i_p_t_ _S_D_K_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_A_g_e_n_t_O_p_s_-_A_I_/_a_g_e_n_t_o_p_s_-_n_o_d_e_)_ _|_ _â___ _S_e_s_s_i_o_n
+_r_e_p_l_a_y_s_|_ _ð____ _E_v_a_l_u_a_t_i_o_n_ _p_l_a_y_g_r_o_u_n_d_ _+_ _l_e_a_d_e_r_b_o_a_r_d_|_ _#_#_ _D_e_b_u_g_g_i_n_g_ _R_o_a_d_m_a_p_ _ð__§_­_ _|
+_P_e_r_f_o_r_m_a_n_c_e_ _t_e_s_t_i_n_g_ _|_ _E_n_v_i_r_o_n_m_e_n_t_s_ _|_ _L_L_M_ _T_e_s_t_i_n_g_ _|_ _R_e_a_s_o_n_i_n_g_ _a_n_d_ _e_x_e_c_u_t_i_o_n
+_t_e_s_t_i_n_g_ _|_ _|_-_-_-_|_-_-_-_|_-_-_-_|_-_-_-_|_ _|_â___ _E_v_e_n_t_ _l_a_t_e_n_c_y_ _a_n_a_l_y_s_i_s_ _|_ _ð____ _N_o_n_-_s_t_a_t_i_o_n_a_r_y
+_e_n_v_i_r_o_n_m_e_n_t_ _t_e_s_t_i_n_g_ _|_ _ð____ _L_L_M_ _n_o_n_-_d_e_t_e_r_m_i_n_i_s_t_i_c_ _f_u_n_c_t_i_o_n_ _d_e_t_e_c_t_i_o_n_ _|_ _ð___§
+_I_n_f_i_n_i_t_e_ _l_o_o_p_s_ _a_n_d_ _r_e_c_u_r_s_i_v_e_ _t_h_o_u_g_h_t_ _d_e_t_e_c_t_i_o_n_ _|_ _|_â___ _A_g_e_n_t_ _w_o_r_k_f_l_o_w_ _e_x_e_c_u_t_i_o_n
+_p_r_i_c_i_n_g_ _|_ _ð____ _M_u_l_t_i_-_m_o_d_a_l_ _e_n_v_i_r_o_n_m_e_n_t_s_ _|_ _ð___§_ _T_o_k_e_n_ _l_i_m_i_t_ _o_v_e_r_f_l_o_w_ _f_l_a_g_s_ _|
+_ð____ _F_a_u_l_t_y_ _r_e_a_s_o_n_i_n_g_ _d_e_t_e_c_t_i_o_n_ _|_ _|_ð___§_ _S_u_c_c_e_s_s_ _v_a_l_i_d_a_t_o_r_s_ _(_e_x_t_e_r_n_a_l_)_ _|_ _ð___
+_E_x_e_c_u_t_i_o_n_ _c_o_n_t_a_i_n_e_r_s_ _|_ _ð____ _C_o_n_t_e_x_t_ _l_i_m_i_t_ _o_v_e_r_f_l_o_w_ _f_l_a_g_s_ _|_ _ð____ _G_e_n_e_r_a_t_i_v_e_ _c_o_d_e
+_v_a_l_i_d_a_t_o_r_s_ _|_ _|_ð____ _A_g_e_n_t_ _c_o_n_t_r_o_l_l_e_r_s_/_s_k_i_l_l_ _t_e_s_t_s_ _|_ _â___ _H_o_n_e_y_p_o_t_ _a_n_d_ _p_r_o_m_p_t
+_i_n_j_e_c_t_i_o_n_ _d_e_t_e_c_t_i_o_n_ _(_[_P_r_o_m_p_t_A_r_m_o_r_]_(_h_t_t_p_s_:_/_/_p_r_o_m_p_t_a_r_m_o_r_._c_o_m_)_)_ _|_ _ð____ _A_P_I_ _b_i_l_l
+_t_r_a_c_k_i_n_g_ _|_ _ð____ _E_r_r_o_r_ _b_r_e_a_k_p_o_i_n_t_ _a_n_a_l_y_s_i_s_ _|_ _|_ð____ _I_n_f_o_r_m_a_t_i_o_n_ _c_o_n_t_e_x_t
+_c_o_n_s_t_r_a_i_n_t_ _t_e_s_t_i_n_g_ _|_ _ð____ _A_n_t_i_-_a_g_e_n_t_ _r_o_a_d_b_l_o_c_k_s_ _(_i_._e_._ _C_a_p_t_c_h_a_s_)_ _|_ _ð____ _C_I_/_C_D
+_i_n_t_e_g_r_a_t_i_o_n_ _c_h_e_c_k_s_ _|_ _|_ _|_ð____ _R_e_g_r_e_s_s_i_o_n_ _t_e_s_t_i_n_g_ _|_ _ð____ _M_u_l_t_i_-_a_g_e_n_t_ _f_r_a_m_e_w_o_r_k
+_v_i_s_u_a_l_i_z_a_t_i_o_n_ _|_ _|_ _|_ _#_#_#_ _W_h_y_ _A_g_e_n_t_O_p_s_?_ _ð__¤__ _O_u_r_ _m_i_s_s_i_o_n_ _i_s_ _t_o_ _b_r_i_n_g_ _y_o_u_r_ _a_g_e_n_t
+_f_r_o_m_ _p_r_o_t_o_t_y_p_e_ _t_o_ _p_r_o_d_u_c_t_i_o_n_._ _A_g_e_n_t_ _d_e_v_e_l_o_p_e_r_s_ _o_f_t_e_n_ _w_o_r_k_ _w_i_t_h_ _l_i_t_t_l_e_ _t_o_ _n_o
+_v_i_s_i_b_i_l_i_t_y_ _i_n_t_o_ _a_g_e_n_t_ _t_e_s_t_i_n_g_ _p_e_r_f_o_r_m_a_n_c_e_._ _T_h_i_s_ _m_e_a_n_s_ _t_h_e_i_r_ _a_g_e_n_t_s_ _n_e_v_e_r_ _l_e_a_v_e
+_t_h_e_ _l_a_b_._ _W_e_'_r_e_ _c_h_a_n_g_i_n_g_ _t_h_a_t_._ _A_g_e_n_t_O_p_s_ _i_s_ _t_h_e_ _e_a_s_i_e_s_t_ _w_a_y_ _t_o_ _e_v_a_l_u_a_t_e_,_ _g_r_a_d_e_,
+_a_n_d_ _t_e_s_t_ _a_g_e_n_t_s_._ _I_s_ _t_h_e_r_e_ _a_ _f_e_a_t_u_r_e_ _y_o_u_'_d_ _l_i_k_e_ _t_o_ _s_e_e_ _A_g_e_n_t_O_p_s_ _c_o_v_e_r_?_ _J_u_s_t
+_r_a_i_s_e_ _i_t_ _i_n_ _t_h_e_ _i_s_s_u_e_s_ _t_a_b_,_ _a_n_d_ _w_e_'_l_l_ _w_o_r_k_ _o_n_ _a_d_d_i_n_g_ _i_t_ _t_o_ _t_h_e_ _r_o_a_d_m_a_p_.
```

### Comparing `agentops-0.1.6/README.md` & `agentops-0.1.7/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,33 @@
+Metadata-Version: 2.1
+Name: agentops
+Version: 0.1.7
+Summary: Python SDK for developing AI agent evals and observability
+Author-email: Alex Reibman <areibman@gmail.com>, Shawn Qiu <siyangqiu@gmail.com>, Braelyn Boynton <bboynton97@gmail.com>, Howard Gil <howardbgil@gmail.com>
+Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
+Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests==2.31.0
+Requires-Dist: psutil==5.9.8
+Requires-Dist: packaging==23.2
+Provides-Extra: dev
+Requires-Dist: pytest==7.4.0; extra == "dev"
+Requires-Dist: requests_mock==1.11.0; extra == "dev"
+Provides-Extra: langchain
+Requires-Dist: langchain>=0.0.354; extra == "langchain"
+
 <div align="center">
-  <img src="logo.png" style="margin: 15px; max-width: 300px" width="50%" alt="Logo">
+  <a href="https://agentops.ai?ref=gh">
+    <img src="logo.png" style="margin: 15px; max-width: 300px" width="50%" alt="Logo">
+  </a>
 </div>
 <p align="center">
   <em>AI agents suck. We’re fixing that.</em>
 </p>
 
 <p align="center">
     <a href="https://pypi.org/project/agentops/" target="_blank">
@@ -12,44 +36,55 @@
     </a>
 </p>
 <p align="center">
 <a href="https://twitter.com/agentopsai/">🐦 Twitter</a>
 <span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
 <a href="https://discord.gg/JHPt4C7r">📢 Discord</a>
 <span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
-<a href="https://app.agentops.ai/?=gh">🖇️ AgentOps</a>
+<a href="https://app.agentops.ai/?ref=gh">🖇️ AgentOps</a>
 <span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
 <a href="https://docs.agentops.ai/introduction">📙 Documentation</a>
 </p>
 
-# AgentOps
-
-Build your next agent with benchmarks, observability, and replay analytics. AgentOps is the toolkit for evaluating and developing robust and reliable AI agents.
-
-You can sign up for AgentOps [here](https://app.agentops.ai).
+# AgentOps 🖇️
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) ![PyPI - Version](https://img.shields.io/pypi/v/agentops) <a href="https://pepy.tech/project/agentops">
   <img src="https://static.pepy.tech/badge/agentops/month"> <a href="https://twitter.com/agentopsai">
     <img src="https://img.shields.io/badge/follow-%40agentops-1DA1F2?logo=twitter&style=social" alt="AgentOps Twitter" /> 
   </a>
-<a href="https://discord.gg/mKW3ZhN9p2">
+  <a href="https://discord.gg/mKW3ZhN9p2">
     <img src="https://img.shields.io/badge/chat-on%20Discord-blueviolet" alt="Discord community channel" />
   </a>
-  <a href="mailto:investor@agentops.ai"><img src="https://img.shields.io/website?color=%23f26522&down_message=Y%20Combinator&label=Not%20Backed%20By&logo=ycombinator&style=flat-square&up_message=Y%20Combinator&url=https%3A%2F%2Fwww.ycombinator.com"></a>
-<a href="https://github.com/agentops-ai/agentops/issues">
+  <a href="mailto:investor@agentops.ai"><img src="https://img.shields.io/website?color=%23f26522&down_message=Y%20Combinator&label=Not%20Backed%20By&logo=ycombinator&style=flat-square&up_message=Y%20Combinator&url=https%3A%2F%2Fwww.ycombinator.com"/>
+  <a href="https://github.com/agentops-ai/agentops/issues">
     <img src="https://img.shields.io/github/commit-activity/m/agentops-ai/agentops" alt="git commit activity" />
   </a>
+
+
+AgentOps helps developers build, evaluate, and monitor AI agents. Tools to build agents from prototype to production.
+
+
+|||
+|------------------------------------------|----------------------------------------------------|
+| 📊 **Replay Analytics and Debugging** | Step-by-step agent execution graphs |
+| 💸 **LLM Cost Management**   | Track spend with LLM foundation model providers |
+| 🧪 **Agent Benchmarking** | Test your agents against 1,000+ evals |
+| 🔐 **Compliance and Security**            | Detect common prompt injection and data exfiltration exploits |
+| 🤝 **Framework Integrations**            | Easily plugs in with frameworks like CrewAI and LangChain |
+
 ## Quick Start ⌨️
 
-```pip install agentops```
+```python
+pip install agentops
+```
 
 ### Session replays in 3 lines of code
-Initialize the AgentOps client, and automatically get analytics on every LLM call.
+Initialize the AgentOps client and automatically get analytics on every LLM call.
 
-```python python
+```python
 import agentops
 
 # Beginning of program's code (i.e. main.py, __init__.py)
 agentops.init(<INSERT YOUR API KEY HERE>)
 
 ...
 # (optional: record specific functions)
@@ -58,46 +93,52 @@
     ...
 
 # End of program
 agentops.end_session('Success')
 # Woohoo You're done 🎉
 ```
 
-Refer to our [API documentation](http://docs.agentops.ai) for detailed instructions.
+All your sessions are available on the [AgentOps dashboard](https://app.agentops.ai?ref=gh). Refer to our [API documentation](http://docs.agentops.ai) for detailed instructions.
 
-## Time travel debugging 🔮
-(coming soon!)
 
-## Agent Arena 🥊
-(coming soon!)
+<details open>
+  <summary>Agent Dashboard</summary>
+  <a href="https://app.agentops.ai?ref=gh">
+   <img src="https://github.com/AgentOps-AI/agentops/assets/14807319/158e082a-9a7d-49b7-9b41-51a49a1f7d3d" style="width: 90%;" alt="Agent Dashboard"/>
+  </a>
+</details>
 
-## Evaluations Roadmap 🧭
+<details>
+  <summary>Session Analytics</summary>
+  <a href="https://app.agentops.ai?ref=gh">
+    <img src="https://github.com/AgentOps-AI/agentops/assets/14807319/d7228019-1488-40d3-852f-a61e998658ad" style="width: 90%;" alt="Session Analytics"/>
+  </a>
+</details>
 
-| Platform | Dashboard | Evals |
-|---|---|---|
-|✅ Python SDK | ✅ Multi-session and Cross-session metrics | ✅ Custom eval metrics |
-|🚧 Evaluation builder API | ✅ Custom event tag tracking | 🔜 Agent scorecards |
-|✅ [Javascript/Typescript SDK](https://github.com/AgentOps-AI/agentops-node) | ✅ Session replays| 🔜 Evaluation playground + leaderboard|
+<details>
+  <summary>Session Replays</summary>
+  <a href="https://app.agentops.ai?ref=gh">
+    <img src="https://github.com/AgentOps-AI/agentops/assets/14807319/561d59f3-c441-4066-914b-f6cfe32a598c" style="width: 90%;" alt="Session Replays"/>
+  </a>
+</details>
 
+## Integrations 🦾
 
-## Debugging Roadmap 🧭
+### CrewAI 🛶
 
-| Performance testing | Environments | LLM Testing | Reasoning and execution testing |
-|---|---|---|---|
-|✅ Event latency analysis | 🔜 Non-stationary environment testing | 🔜 LLM non-deterministic function detection | 🚧 Infinite loops and recursive thought detection |
-|✅ Agent workflow execution pricing | 🔜 Multi-modal environments | 🚧 Token limit overflow flags | 🔜 Faulty reasoning detection |
-|🚧 Success validators (external) | 🔜 Execution containers | 🔜 Context limit overflow flags | 🔜 Generative code validators |
-|🔜 Agent controllers/skill tests | ✅ Honeypot and prompt injection detection ([PromptArmor](https://promptarmor.com)) | 🔜 API bill tracking | 🔜 Error breakpoint analysis |
-|🔜 Information context constraint testing | 🔜 Anti-agent roadblocks (i.e. Captchas) | 🔜 CI/CD integration checks | |
-|🔜 Regression testing | 🔜 Multi-agent framework visualization | | |
+Build Crew agents with observability with only 2 lines of code. Simply set an `AGENTOPS_API_KEY` in your environment, and your crews will get automatic monitoring on the AgentOps dashboard.
+
+AgentOps is officially supported on Crew's latest rc branch: `crewai==0.28.9rc1`
+
+* [AgentOps integration example](https://docs.agentops.ai/v1/integrations/crewai)
+* [Offical CrewAI documentation](https://docs.crewai.com/how-to/AgentOps-Observability)
 
-## Callback handlers ↩️
 
-### Langchain
-AgentOps works seemlessly with applications built using Langchain. To use the handler, install Langchain as an optional dependency:
+### Langchain 🦜🔗
+AgentOps works seamlessly with applications built using Langchain. To use the handler, install Langchain as an optional dependency:
 ```shell
 pip install agentops[langchain]
 ```
 
 To use the handler, import and set
 
 ```python
@@ -119,18 +160,45 @@
                          verbose=True,
                          callbacks=[handler], # You must pass in a callback handler to record your agent
                          handle_parsing_errors=True)
 ```
 
 Check out the [Langchain Examples Notebook](./examples/langchain_examples.ipynb) for more details including Async handlers.
 
-### LlamaIndex 
+### LlamaIndex 🦙
 (Coming Soon)
 
 
+
+## Time travel debugging 🔮
+(coming soon!)
+
+## Agent Arena 🥊
+(coming soon!)
+
+## Evaluations Roadmap 🧭
+
+| Platform | Dashboard | Evals |
+|---|---|---|
+|✅ Python SDK | ✅ Multi-session and Cross-session metrics | ✅ Custom eval metrics |
+|🚧 Evaluation builder API | ✅ Custom event tag tracking | 🔜 Agent scorecards |
+|✅ [Javascript/Typescript SDK](https://github.com/AgentOps-AI/agentops-node) | ✅ Session replays| 🔜 Evaluation playground + leaderboard|
+
+
+## Debugging Roadmap 🧭
+
+| Performance testing | Environments | LLM Testing | Reasoning and execution testing |
+|---|---|---|---|
+|✅ Event latency analysis | 🔜 Non-stationary environment testing | 🔜 LLM non-deterministic function detection | 🚧 Infinite loops and recursive thought detection |
+|✅ Agent workflow execution pricing | 🔜 Multi-modal environments | 🚧 Token limit overflow flags | 🔜 Faulty reasoning detection |
+|🚧 Success validators (external) | 🔜 Execution containers | 🔜 Context limit overflow flags | 🔜 Generative code validators |
+|🔜 Agent controllers/skill tests | ✅ Honeypot and prompt injection detection ([PromptArmor](https://promptarmor.com)) | 🔜 API bill tracking | 🔜 Error breakpoint analysis |
+|🔜 Information context constraint testing | 🔜 Anti-agent roadblocks (i.e. Captchas) | 🔜 CI/CD integration checks | |
+|🔜 Regression testing | 🔜 Multi-agent framework visualization | | |
+
 ### Why AgentOps? 🤔
 
-Our mission is to bring your agent from protype to production.
+Our mission is to bring your agent from prototype to production.
 
 Agent developers often work with little to no visibility into agent testing performance. This means their agents never leave the lab. We're changing that. 
 
 AgentOps is the easiest way to evaluate, grade, and test agents. Is there a feature you'd like to see AgentOps cover? Just raise it in the issues tab, and we'll work on adding it to the roadmap.
```

#### html2text {}

```diff
@@ -1,61 +1,89 @@
-                                    [Logo]
+Metadata-Version: 2.1 Name: agentops Version: 0.1.7 Summary: Python SDK for
+developing AI agent evals and observability Author-email: Alex Reibman
+gmail.com>, Shawn Qiu
+gmail.com>, Braelyn Boynton
+gmail.com>, Howard Gil
+gmail.com> Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
+Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues Classifier:
+Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
+License Classifier: Operating System :: OS Independent Requires-Python: >=3.10
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+requests==2.31.0 Requires-Dist: psutil==5.9.8 Requires-Dist: packaging==23.2
+Provides-Extra: dev Requires-Dist: pytest==7.4.0; extra == "dev" Requires-Dist:
+requests_mock==1.11.0; extra == "dev" Provides-Extra: langchain Requires-Dist:
+langchain>=0.0.354; extra == "langchain"
+                                    _[_L_o_g_o_]
                      AAII aaggeennttss ssuucckk.. WWee?â??rree ffiixxiinngg tthhaatt..
                                _[_P_y_t_h_o_n_]_[_V_e_r_s_i_o_n_]
     _ð___¦_ _T_w_i_t_t_e_r   â¢   _ð___¢_ _D_i_s_c_o_r_d   â¢   _ð____ï_¸__ _A_g_e_n_t_O_p_s   â¢   _ð___
                                  _D_o_c_u_m_e_n_t_a_t_i_o_n
-# AgentOps Build your next agent with benchmarks, observability, and replay
-analytics. AgentOps is the toolkit for evaluating and developing robust and
-reliable AI agents. You can sign up for AgentOps [here](https://
-app.agentops.ai). [![License: MIT](https://img.shields.io/badge/License-MIT-
+# AgentOps ðï¸ [![License: MIT](https://img.shields.io/badge/License-MIT-
 yellow.svg)](https://opensource.org/licenses/MIT) ![PyPI - Version](https://
 img.shields.io/pypi/v/agentops) _[_h_t_t_p_s_:_/_/_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_a_g_e_n_t_o_p_s_/_m_o_n_t_h_]
 _[_A_g_e_n_t_O_p_s_ _T_w_i_t_t_e_r_]_[_D_i_s_c_o_r_d_ _c_o_m_m_u_n_i_t_y_ _c_h_a_n_n_e_l_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _w_e_b_s_i_t_e_?_c_o_l_o_r_=_%_2_3_f_2_6_5_2_2_&_d_o_w_n___m_e_s_s_a_g_e_=_Y_%_2_0_C_o_m_b_i_n_a_t_o_r_&_l_a_b_e_l_=_N_o_t_%_2_0_B_a_c_k_e_d_%_2_0_B_y_&_l_o_g_o_=_y_c_o_m_b_i_n_a_t_o_r_&_s_t_y_l_e_=_f_l_a_t_-
 _s_q_u_a_r_e_&_u_p___m_e_s_s_a_g_e_=_Y_%_2_0_C_o_m_b_i_n_a_t_o_r_&_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_w_w_w_._y_c_o_m_b_i_n_a_t_o_r_._c_o_m_]_[_g_i_t
-_c_o_m_m_i_t_ _a_c_t_i_v_i_t_y_]_#_#_ _Q_u_i_c_k_ _S_t_a_r_t_ _â__¨_ï_¸__ _`_`_`_p_i_p_ _i_n_s_t_a_l_l_ _a_g_e_n_t_o_p_s_`_`_`_ _#_#_#_ _S_e_s_s_i_o_n
-_r_e_p_l_a_y_s_ _i_n_ _3_ _l_i_n_e_s_ _o_f_ _c_o_d_e_ _I_n_i_t_i_a_l_i_z_e_ _t_h_e_ _A_g_e_n_t_O_p_s_ _c_l_i_e_n_t_,_ _a_n_d_ _a_u_t_o_m_a_t_i_c_a_l_l_y
-_g_e_t_ _a_n_a_l_y_t_i_c_s_ _o_n_ _e_v_e_r_y_ _L_L_M_ _c_a_l_l_._ _`_`_`_p_y_t_h_o_n_ _p_y_t_h_o_n_ _i_m_p_o_r_t_ _a_g_e_n_t_o_p_s_ _#_ _B_e_g_i_n_n_i_n_g
-_o_f_ _p_r_o_g_r_a_m_'_s_ _c_o_d_e_ _(_i_._e_._ _m_a_i_n_._p_y_,_ _____i_n_i_t_____._p_y_)_ _a_g_e_n_t_o_p_s_._i_n_i_t_(_)_ _._._._ _#_ _(_o_p_t_i_o_n_a_l_:
-_r_e_c_o_r_d_ _s_p_e_c_i_f_i_c_ _f_u_n_c_t_i_o_n_s_)_ _@_a_g_e_n_t_o_p_s_._r_e_c_o_r_d___f_u_n_c_t_i_o_n_(_'_s_a_m_p_l_e_ _f_u_n_c_t_i_o_n_ _b_e_i_n_g
-_r_e_c_o_r_d_'_)_ _d_e_f_ _s_a_m_p_l_e___f_u_n_c_t_i_o_n_(_._._._)_:_ _._._._ _#_ _E_n_d_ _o_f_ _p_r_o_g_r_a_m_ _a_g_e_n_t_o_p_s_._e_n_d___s_e_s_s_i_o_n
-_(_'_S_u_c_c_e_s_s_'_)_ _#_ _W_o_o_h_o_o_ _Y_o_u_'_r_e_ _d_o_n_e_ _ð____ _`_`_`_ _R_e_f_e_r_ _t_o_ _o_u_r_ _[_A_P_I_ _d_o_c_u_m_e_n_t_a_t_i_o_n_]
-_(_h_t_t_p_:_/_/_d_o_c_s_._a_g_e_n_t_o_p_s_._a_i_)_ _f_o_r_ _d_e_t_a_i_l_e_d_ _i_n_s_t_r_u_c_t_i_o_n_s_._ _#_#_ _T_i_m_e_ _t_r_a_v_e_l_ _d_e_b_u_g_g_i_n_g
-_ð___®_ _(_c_o_m_i_n_g_ _s_o_o_n_!_)_ _#_#_ _A_g_e_n_t_ _A_r_e_n_a_ _ð__¥__ _(_c_o_m_i_n_g_ _s_o_o_n_!_)_ _#_#_ _E_v_a_l_u_a_t_i_o_n_s_ _R_o_a_d_m_a_p
-_ð__§_­_ _|_ _P_l_a_t_f_o_r_m_ _|_ _D_a_s_h_b_o_a_r_d_ _|_ _E_v_a_l_s_ _|_ _|_-_-_-_|_-_-_-_|_-_-_-_|_ _|_â___ _P_y_t_h_o_n_ _S_D_K_ _|_ _â__
-_M_u_l_t_i_-_s_e_s_s_i_o_n_ _a_n_d_ _C_r_o_s_s_-_s_e_s_s_i_o_n_ _m_e_t_r_i_c_s_ _|_ _â___ _C_u_s_t_o_m_ _e_v_a_l_ _m_e_t_r_i_c_s_ _|_ _|_ð___§
-_E_v_a_l_u_a_t_i_o_n_ _b_u_i_l_d_e_r_ _A_P_I_ _|_ _â___ _C_u_s_t_o_m_ _e_v_e_n_t_ _t_a_g_ _t_r_a_c_k_i_n_g_Â_ _|_ _ð____ _A_g_e_n_t_ _s_c_o_r_e_c_a_r_d_s
-_|_ _|_â___ _[_J_a_v_a_s_c_r_i_p_t_/_T_y_p_e_s_c_r_i_p_t_ _S_D_K_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_A_g_e_n_t_O_p_s_-_A_I_/_a_g_e_n_t_o_p_s_-
-_n_o_d_e_)_ _|_ _â___ _S_e_s_s_i_o_n_ _r_e_p_l_a_y_s_|_ _ð____ _E_v_a_l_u_a_t_i_o_n_ _p_l_a_y_g_r_o_u_n_d_ _+_ _l_e_a_d_e_r_b_o_a_r_d_|_ _#_#
-_D_e_b_u_g_g_i_n_g_ _R_o_a_d_m_a_p_ _ð__§_­_ _|_ _P_e_r_f_o_r_m_a_n_c_e_ _t_e_s_t_i_n_g_ _|_ _E_n_v_i_r_o_n_m_e_n_t_s_ _|_ _L_L_M_ _T_e_s_t_i_n_g_ _|
-_R_e_a_s_o_n_i_n_g_ _a_n_d_ _e_x_e_c_u_t_i_o_n_ _t_e_s_t_i_n_g_ _|_ _|_-_-_-_|_-_-_-_|_-_-_-_|_-_-_-_|_ _|_â___ _E_v_e_n_t_ _l_a_t_e_n_c_y_ _a_n_a_l_y_s_i_s
-_|_ _ð____ _N_o_n_-_s_t_a_t_i_o_n_a_r_y_ _e_n_v_i_r_o_n_m_e_n_t_ _t_e_s_t_i_n_g_ _|_ _ð____ _L_L_M_ _n_o_n_-_d_e_t_e_r_m_i_n_i_s_t_i_c_ _f_u_n_c_t_i_o_n
-_d_e_t_e_c_t_i_o_n_ _|_ _ð___§_ _I_n_f_i_n_i_t_e_ _l_o_o_p_s_ _a_n_d_ _r_e_c_u_r_s_i_v_e_ _t_h_o_u_g_h_t_ _d_e_t_e_c_t_i_o_n_ _|_ _|_â___ _A_g_e_n_t
-_w_o_r_k_f_l_o_w_ _e_x_e_c_u_t_i_o_n_ _p_r_i_c_i_n_g_ _|_ _ð____ _M_u_l_t_i_-_m_o_d_a_l_ _e_n_v_i_r_o_n_m_e_n_t_s_ _|_ _ð___§_ _T_o_k_e_n_ _l_i_m_i_t
-_o_v_e_r_f_l_o_w_ _f_l_a_g_s_ _|_ _ð____ _F_a_u_l_t_y_ _r_e_a_s_o_n_i_n_g_ _d_e_t_e_c_t_i_o_n_ _|_ _|_ð___§_ _S_u_c_c_e_s_s_ _v_a_l_i_d_a_t_o_r_s_ 
-_(_e_x_t_e_r_n_a_l_)_ _|_ _ð____ _E_x_e_c_u_t_i_o_n_ _c_o_n_t_a_i_n_e_r_s_ _|_ _ð____ _C_o_n_t_e_x_t_ _l_i_m_i_t_ _o_v_e_r_f_l_o_w_ _f_l_a_g_s_ _|
-_ð____ _G_e_n_e_r_a_t_i_v_e_ _c_o_d_e_ _v_a_l_i_d_a_t_o_r_s_ _|_ _|_ð____ _A_g_e_n_t_ _c_o_n_t_r_o_l_l_e_r_s_/_s_k_i_l_l_ _t_e_s_t_s_ _|_ _â__
-_H_o_n_e_y_p_o_t_ _a_n_d_ _p_r_o_m_p_t_ _i_n_j_e_c_t_i_o_n_ _d_e_t_e_c_t_i_o_n_ _(_[_P_r_o_m_p_t_A_r_m_o_r_]_(_h_t_t_p_s_:_/_/
-_p_r_o_m_p_t_a_r_m_o_r_._c_o_m_)_)_ _|_ _ð____ _A_P_I_ _b_i_l_l_ _t_r_a_c_k_i_n_g_ _|_ _ð____ _E_r_r_o_r_ _b_r_e_a_k_p_o_i_n_t_ _a_n_a_l_y_s_i_s_ _|
-_|_ð____ _I_n_f_o_r_m_a_t_i_o_n_ _c_o_n_t_e_x_t_ _c_o_n_s_t_r_a_i_n_t_ _t_e_s_t_i_n_g_ _|_ _ð____ _A_n_t_i_-_a_g_e_n_t_ _r_o_a_d_b_l_o_c_k_s_ _(_i_._e_.
-_C_a_p_t_c_h_a_s_)_ _|_ _ð____ _C_I_/_C_D_ _i_n_t_e_g_r_a_t_i_o_n_ _c_h_e_c_k_s_ _|_ _|_ _|_ð____ _R_e_g_r_e_s_s_i_o_n_ _t_e_s_t_i_n_g_ _|_ _ð___
-_M_u_l_t_i_-_a_g_e_n_t_ _f_r_a_m_e_w_o_r_k_ _v_i_s_u_a_l_i_z_a_t_i_o_n_ _|_ _|_ _|_ _#_#_ _C_a_l_l_b_a_c_k_ _h_a_n_d_l_e_r_s_ _â__©_ï_¸__ _#_#_#
-_L_a_n_g_c_h_a_i_n_ _A_g_e_n_t_O_p_s_ _w_o_r_k_s_ _s_e_e_m_l_e_s_s_l_y_ _w_i_t_h_ _a_p_p_l_i_c_a_t_i_o_n_s_ _b_u_i_l_t_ _u_s_i_n_g_ _L_a_n_g_c_h_a_i_n_._ _T_o
-_u_s_e_ _t_h_e_ _h_a_n_d_l_e_r_,_ _i_n_s_t_a_l_l_ _L_a_n_g_c_h_a_i_n_ _a_s_ _a_n_ _o_p_t_i_o_n_a_l_ _d_e_p_e_n_d_e_n_c_y_:_ _`_`_`_s_h_e_l_l_ _p_i_p
-_i_n_s_t_a_l_l_ _a_g_e_n_t_o_p_s_[_l_a_n_g_c_h_a_i_n_]_ _`_`_`_ _T_o_ _u_s_e_ _t_h_e_ _h_a_n_d_l_e_r_,_ _i_m_p_o_r_t_ _a_n_d_ _s_e_t_ _`_`_`_p_y_t_h_o_n
-_i_m_p_o_r_t_ _o_s_ _f_r_o_m_ _l_a_n_g_c_h_a_i_n_._c_h_a_t___m_o_d_e_l_s_ _i_m_p_o_r_t_ _C_h_a_t_O_p_e_n_A_I_ _f_r_o_m_ _l_a_n_g_c_h_a_i_n_._a_g_e_n_t_s
-_i_m_p_o_r_t_ _i_n_i_t_i_a_l_i_z_e___a_g_e_n_t_,_ _A_g_e_n_t_T_y_p_e_ _f_r_o_m_ _a_g_e_n_t_o_p_s_._l_a_n_g_c_h_a_i_n___c_a_l_l_b_a_c_k___h_a_n_d_l_e_r
-_i_m_p_o_r_t_ _L_a_n_g_c_h_a_i_n_C_a_l_l_b_a_c_k_H_a_n_d_l_e_r_ _A_G_E_N_T_O_P_S___A_P_I___K_E_Y_ _=_ _o_s_._e_n_v_i_r_o_n
-_[_'_A_G_E_N_T_O_P_S___A_P_I___K_E_Y_'_]_ _h_a_n_d_l_e_r_ _=_ _L_a_n_g_c_h_a_i_n_C_a_l_l_b_a_c_k_H_a_n_d_l_e_r
-_(_a_p_i___k_e_y_=_A_G_E_N_T_O_P_S___A_P_I___K_E_Y_,_ _t_a_g_s_=_[_'_L_a_n_g_c_h_a_i_n_ _E_x_a_m_p_l_e_'_]_)_ _l_l_m_ _=_ _C_h_a_t_O_p_e_n_A_I
-_(_o_p_e_n_a_i___a_p_i___k_e_y_=_O_P_E_N_A_I___A_P_I___K_E_Y_,_ _c_a_l_l_b_a_c_k_s_=_[_h_a_n_d_l_e_r_]_,_ _m_o_d_e_l_=_'_g_p_t_-_3_._5_-_t_u_r_b_o_'_)
-_a_g_e_n_t_ _=_ _i_n_i_t_i_a_l_i_z_e___a_g_e_n_t_(_t_o_o_l_s_,_ _l_l_m_,
+_c_o_m_m_i_t_ _a_c_t_i_v_i_t_y_]_A_g_e_n_t_O_p_s_ _h_e_l_p_s_ _d_e_v_e_l_o_p_e_r_s_ _b_u_i_l_d_,_ _e_v_a_l_u_a_t_e_,_ _a_n_d_ _m_o_n_i_t_o_r_ _A_I
+_a_g_e_n_t_s_._ _T_o_o_l_s_ _t_o_ _b_u_i_l_d_ _a_g_e_n_t_s_ _f_r_o_m_ _p_r_o_t_o_t_y_p_e_ _t_o_ _p_r_o_d_u_c_t_i_o_n_._ _|_|_|_ _|_-_-_-_-_-_-_-_-_-_-_-_-_-_-
+_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_|_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-
+_-_-_|_ _|_ _ð____ _*_*_R_e_p_l_a_y_ _A_n_a_l_y_t_i_c_s_ _a_n_d_ _D_e_b_u_g_g_i_n_g_*_*_ _|_ _S_t_e_p_-_b_y_-_s_t_e_p_ _a_g_e_n_t_ _e_x_e_c_u_t_i_o_n
+_g_r_a_p_h_s_ _|_ _|_ _ð___¸_ _*_*_L_L_M_ _C_o_s_t_ _M_a_n_a_g_e_m_e_n_t_*_*_ _|_ _T_r_a_c_k_ _s_p_e_n_d_ _w_i_t_h_ _L_L_M_ _f_o_u_n_d_a_t_i_o_n_ _m_o_d_e_l
+_p_r_o_v_i_d_e_r_s_ _|_ _|_ _ð__§_ª_ _*_*_A_g_e_n_t_ _B_e_n_c_h_m_a_r_k_i_n_g_*_*_ _|_ _T_e_s_t_ _y_o_u_r_ _a_g_e_n_t_s_ _a_g_a_i_n_s_t_ _1_,_0_0_0_+
+_e_v_a_l_s_ _|_ _|_ _ð____ _*_*_C_o_m_p_l_i_a_n_c_e_ _a_n_d_ _S_e_c_u_r_i_t_y_*_*_ _|_ _D_e_t_e_c_t_ _c_o_m_m_o_n_ _p_r_o_m_p_t_ _i_n_j_e_c_t_i_o_n_ _a_n_d
+_d_a_t_a_ _e_x_f_i_l_t_r_a_t_i_o_n_ _e_x_p_l_o_i_t_s_ _|_ _|_ _ð__¤__ _*_*_F_r_a_m_e_w_o_r_k_ _I_n_t_e_g_r_a_t_i_o_n_s_*_*_ _|_ _E_a_s_i_l_y_ _p_l_u_g_s
+_i_n_ _w_i_t_h_ _f_r_a_m_e_w_o_r_k_s_ _l_i_k_e_ _C_r_e_w_A_I_ _a_n_d_ _L_a_n_g_C_h_a_i_n_ _|_ _#_#_ _Q_u_i_c_k_ _S_t_a_r_t_ _â__¨_ï_¸__ _`_`_`_p_y_t_h_o_n
+_p_i_p_ _i_n_s_t_a_l_l_ _a_g_e_n_t_o_p_s_ _`_`_`_ _#_#_#_ _S_e_s_s_i_o_n_ _r_e_p_l_a_y_s_ _i_n_ _3_ _l_i_n_e_s_ _o_f_ _c_o_d_e_ _I_n_i_t_i_a_l_i_z_e_ _t_h_e
+_A_g_e_n_t_O_p_s_ _c_l_i_e_n_t_ _a_n_d_ _a_u_t_o_m_a_t_i_c_a_l_l_y_ _g_e_t_ _a_n_a_l_y_t_i_c_s_ _o_n_ _e_v_e_r_y_ _L_L_M_ _c_a_l_l_._ _`_`_`_p_y_t_h_o_n
+_i_m_p_o_r_t_ _a_g_e_n_t_o_p_s_ _#_ _B_e_g_i_n_n_i_n_g_ _o_f_ _p_r_o_g_r_a_m_'_s_ _c_o_d_e_ _(_i_._e_._ _m_a_i_n_._p_y_,_ _____i_n_i_t_____._p_y_)
+_a_g_e_n_t_o_p_s_._i_n_i_t_(_)_ _._._._ _#_ _(_o_p_t_i_o_n_a_l_:_ _r_e_c_o_r_d_ _s_p_e_c_i_f_i_c_ _f_u_n_c_t_i_o_n_s_)
+_@_a_g_e_n_t_o_p_s_._r_e_c_o_r_d___f_u_n_c_t_i_o_n_(_'_s_a_m_p_l_e_ _f_u_n_c_t_i_o_n_ _b_e_i_n_g_ _r_e_c_o_r_d_'_)_ _d_e_f_ _s_a_m_p_l_e___f_u_n_c_t_i_o_n
+_(_._._._)_:_ _._._._ _#_ _E_n_d_ _o_f_ _p_r_o_g_r_a_m_ _a_g_e_n_t_o_p_s_._e_n_d___s_e_s_s_i_o_n_(_'_S_u_c_c_e_s_s_'_)_ _#_ _W_o_o_h_o_o_ _Y_o_u_'_r_e
+_d_o_n_e_ _ð____ _`_`_`_ _A_l_l_ _y_o_u_r_ _s_e_s_s_i_o_n_s_ _a_r_e_ _a_v_a_i_l_a_b_l_e_ _o_n_ _t_h_e_ _[_A_g_e_n_t_O_p_s_ _d_a_s_h_b_o_a_r_d_]
+_(_h_t_t_p_s_:_/_/_a_p_p_._a_g_e_n_t_o_p_s_._a_i_?_r_e_f_=_g_h_)_._ _R_e_f_e_r_ _t_o_ _o_u_r_ _[_A_P_I_ _d_o_c_u_m_e_n_t_a_t_i_o_n_]_(_h_t_t_p_:_/_/
+_d_o_c_s_._a_g_e_n_t_o_p_s_._a_i_)_ _f_o_r_ _d_e_t_a_i_l_e_d_ _i_n_s_t_r_u_c_t_i_o_n_s_._ _A_g_e_n_t_ _D_a_s_h_b_o_a_r_d_ _[_A_g_e_n_t
+_D_a_s_h_b_o_a_r_d_]_S_e_s_s_i_o_n_ _A_n_a_l_y_t_i_c_s_ _[_S_e_s_s_i_o_n_ _A_n_a_l_y_t_i_c_s_]_S_e_s_s_i_o_n_ _R_e_p_l_a_y_s_ _[_S_e_s_s_i_o_n
+_R_e_p_l_a_y_s_]_#_#_ _I_n_t_e_g_r_a_t_i_o_n_s_ _ð__¦_¾_ _#_#_#_ _C_r_e_w_A_I_ _ð___¶_ _B_u_i_l_d_ _C_r_e_w_ _a_g_e_n_t_s_ _w_i_t_h
+_o_b_s_e_r_v_a_b_i_l_i_t_y_ _w_i_t_h_ _o_n_l_y_ _2_ _l_i_n_e_s_ _o_f_ _c_o_d_e_._ _S_i_m_p_l_y_ _s_e_t_ _a_n_ _`_A_G_E_N_T_O_P_S___A_P_I___K_E_Y_`_ _i_n
+_y_o_u_r_ _e_n_v_i_r_o_n_m_e_n_t_,_ _a_n_d_ _y_o_u_r_ _c_r_e_w_s_ _w_i_l_l_ _g_e_t_ _a_u_t_o_m_a_t_i_c_ _m_o_n_i_t_o_r_i_n_g_ _o_n_ _t_h_e_ _A_g_e_n_t_O_p_s
+_d_a_s_h_b_o_a_r_d_._ _A_g_e_n_t_O_p_s_ _i_s_ _o_f_f_i_c_i_a_l_l_y_ _s_u_p_p_o_r_t_e_d_ _o_n_ _C_r_e_w_'_s_ _l_a_t_e_s_t_ _r_c_ _b_r_a_n_c_h_:
+_`_c_r_e_w_a_i_=_=_0_._2_8_._9_r_c_1_`_ _*_ _[_A_g_e_n_t_O_p_s_ _i_n_t_e_g_r_a_t_i_o_n_ _e_x_a_m_p_l_e_]_(_h_t_t_p_s_:_/_/_d_o_c_s_._a_g_e_n_t_o_p_s_._a_i_/
+_v_1_/_i_n_t_e_g_r_a_t_i_o_n_s_/_c_r_e_w_a_i_)_ _*_ _[_O_f_f_i_c_a_l_ _C_r_e_w_A_I_ _d_o_c_u_m_e_n_t_a_t_i_o_n_]_(_h_t_t_p_s_:_/_/
+_d_o_c_s_._c_r_e_w_a_i_._c_o_m_/_h_o_w_-_t_o_/_A_g_e_n_t_O_p_s_-_O_b_s_e_r_v_a_b_i_l_i_t_y_)_ _#_#_#_ _L_a_n_g_c_h_a_i_n_ _ð__¦__ð____ _A_g_e_n_t_O_p_s
+_w_o_r_k_s_ _s_e_a_m_l_e_s_s_l_y_ _w_i_t_h_ _a_p_p_l_i_c_a_t_i_o_n_s_ _b_u_i_l_t_ _u_s_i_n_g_ _L_a_n_g_c_h_a_i_n_._ _T_o_ _u_s_e_ _t_h_e_ _h_a_n_d_l_e_r_,
+_i_n_s_t_a_l_l_ _L_a_n_g_c_h_a_i_n_ _a_s_ _a_n_ _o_p_t_i_o_n_a_l_ _d_e_p_e_n_d_e_n_c_y_:_ _`_`_`_s_h_e_l_l_ _p_i_p_ _i_n_s_t_a_l_l_ _a_g_e_n_t_o_p_s
+_[_l_a_n_g_c_h_a_i_n_]_ _`_`_`_ _T_o_ _u_s_e_ _t_h_e_ _h_a_n_d_l_e_r_,_ _i_m_p_o_r_t_ _a_n_d_ _s_e_t_ _`_`_`_p_y_t_h_o_n_ _i_m_p_o_r_t_ _o_s_ _f_r_o_m
+_l_a_n_g_c_h_a_i_n_._c_h_a_t___m_o_d_e_l_s_ _i_m_p_o_r_t_ _C_h_a_t_O_p_e_n_A_I_ _f_r_o_m_ _l_a_n_g_c_h_a_i_n_._a_g_e_n_t_s_ _i_m_p_o_r_t
+_i_n_i_t_i_a_l_i_z_e___a_g_e_n_t_,_ _A_g_e_n_t_T_y_p_e_ _f_r_o_m_ _a_g_e_n_t_o_p_s_._l_a_n_g_c_h_a_i_n___c_a_l_l_b_a_c_k___h_a_n_d_l_e_r_ _i_m_p_o_r_t
+_L_a_n_g_c_h_a_i_n_C_a_l_l_b_a_c_k_H_a_n_d_l_e_r_ _A_G_E_N_T_O_P_S___A_P_I___K_E_Y_ _=_ _o_s_._e_n_v_i_r_o_n_[_'_A_G_E_N_T_O_P_S___A_P_I___K_E_Y_'_]
+_h_a_n_d_l_e_r_ _=_ _L_a_n_g_c_h_a_i_n_C_a_l_l_b_a_c_k_H_a_n_d_l_e_r_(_a_p_i___k_e_y_=_A_G_E_N_T_O_P_S___A_P_I___K_E_Y_,_ _t_a_g_s_=_[_'_L_a_n_g_c_h_a_i_n
+_E_x_a_m_p_l_e_'_]_)_ _l_l_m_ _=_ _C_h_a_t_O_p_e_n_A_I_(_o_p_e_n_a_i___a_p_i___k_e_y_=_O_P_E_N_A_I___A_P_I___K_E_Y_,_ _c_a_l_l_b_a_c_k_s_=_[_h_a_n_d_l_e_r_]_,
+_m_o_d_e_l_=_'_g_p_t_-_3_._5_-_t_u_r_b_o_'_)_ _a_g_e_n_t_ _=_ _i_n_i_t_i_a_l_i_z_e___a_g_e_n_t_(_t_o_o_l_s_,_ _l_l_m_,
 _a_g_e_n_t_=_A_g_e_n_t_T_y_p_e_._C_H_A_T___Z_E_R_O___S_H_O_T___R_E_A_C_T___D_E_S_C_R_I_P_T_I_O_N_,_ _v_e_r_b_o_s_e_=_T_r_u_e_,_ _c_a_l_l_b_a_c_k_s_=
 _[_h_a_n_d_l_e_r_]_,_ _#_ _Y_o_u_ _m_u_s_t_ _p_a_s_s_ _i_n_ _a_ _c_a_l_l_b_a_c_k_ _h_a_n_d_l_e_r_ _t_o_ _r_e_c_o_r_d_ _y_o_u_r_ _a_g_e_n_t
 _h_a_n_d_l_e___p_a_r_s_i_n_g___e_r_r_o_r_s_=_T_r_u_e_)_ _`_`_`_ _C_h_e_c_k_ _o_u_t_ _t_h_e_ _[_L_a_n_g_c_h_a_i_n_ _E_x_a_m_p_l_e_s_ _N_o_t_e_b_o_o_k_]_(_._/
 _e_x_a_m_p_l_e_s_/_l_a_n_g_c_h_a_i_n___e_x_a_m_p_l_e_s_._i_p_y_n_b_)_ _f_o_r_ _m_o_r_e_ _d_e_t_a_i_l_s_ _i_n_c_l_u_d_i_n_g_ _A_s_y_n_c_ _h_a_n_d_l_e_r_s_.
-_#_#_#_ _L_l_a_m_a_I_n_d_e_x_ _(_C_o_m_i_n_g_ _S_o_o_n_)_ _#_#_#_ _W_h_y_ _A_g_e_n_t_O_p_s_?_ _ð__¤__ _O_u_r_ _m_i_s_s_i_o_n_ _i_s_ _t_o_ _b_r_i_n_g
-_y_o_u_r_ _a_g_e_n_t_ _f_r_o_m_ _p_r_o_t_y_p_e_ _t_o_ _p_r_o_d_u_c_t_i_o_n_._ _A_g_e_n_t_ _d_e_v_e_l_o_p_e_r_s_ _o_f_t_e_n_ _w_o_r_k_ _w_i_t_h_ _l_i_t_t_l_e
-_t_o_ _n_o_ _v_i_s_i_b_i_l_i_t_y_ _i_n_t_o_ _a_g_e_n_t_ _t_e_s_t_i_n_g_ _p_e_r_f_o_r_m_a_n_c_e_._ _T_h_i_s_ _m_e_a_n_s_ _t_h_e_i_r_ _a_g_e_n_t_s_ _n_e_v_e_r
-_l_e_a_v_e_ _t_h_e_ _l_a_b_._ _W_e_'_r_e_ _c_h_a_n_g_i_n_g_ _t_h_a_t_._ _A_g_e_n_t_O_p_s_ _i_s_ _t_h_e_ _e_a_s_i_e_s_t_ _w_a_y_ _t_o_ _e_v_a_l_u_a_t_e_,
-_g_r_a_d_e_,_ _a_n_d_ _t_e_s_t_ _a_g_e_n_t_s_._ _I_s_ _t_h_e_r_e_ _a_ _f_e_a_t_u_r_e_ _y_o_u_'_d_ _l_i_k_e_ _t_o_ _s_e_e_ _A_g_e_n_t_O_p_s_ _c_o_v_e_r_?
-_J_u_s_t_ _r_a_i_s_e_ _i_t_ _i_n_ _t_h_e_ _i_s_s_u_e_s_ _t_a_b_,_ _a_n_d_ _w_e_'_l_l_ _w_o_r_k_ _o_n_ _a_d_d_i_n_g_ _i_t_ _t_o_ _t_h_e_ _r_o_a_d_m_a_p_.
+_#_#_#_ _L_l_a_m_a_I_n_d_e_x_ _ð__¦__ _(_C_o_m_i_n_g_ _S_o_o_n_)_ _#_#_ _T_i_m_e_ _t_r_a_v_e_l_ _d_e_b_u_g_g_i_n_g_ _ð___®_ _(_c_o_m_i_n_g_ _s_o_o_n_!_)
+_#_#_ _A_g_e_n_t_ _A_r_e_n_a_ _ð__¥__ _(_c_o_m_i_n_g_ _s_o_o_n_!_)_ _#_#_ _E_v_a_l_u_a_t_i_o_n_s_ _R_o_a_d_m_a_p_ _ð__§_­_ _|_ _P_l_a_t_f_o_r_m_ _|
+_D_a_s_h_b_o_a_r_d_ _|_ _E_v_a_l_s_ _|_ _|_-_-_-_|_-_-_-_|_-_-_-_|_ _|_â___ _P_y_t_h_o_n_ _S_D_K_ _|_ _â___ _M_u_l_t_i_-_s_e_s_s_i_o_n_ _a_n_d
+_C_r_o_s_s_-_s_e_s_s_i_o_n_ _m_e_t_r_i_c_s_ _|_ _â___ _C_u_s_t_o_m_ _e_v_a_l_ _m_e_t_r_i_c_s_ _|_ _|_ð___§_ _E_v_a_l_u_a_t_i_o_n_ _b_u_i_l_d_e_r_ _A_P_I
+_|_ _â___ _C_u_s_t_o_m_ _e_v_e_n_t_ _t_a_g_ _t_r_a_c_k_i_n_g_Â_ _|_ _ð____ _A_g_e_n_t_ _s_c_o_r_e_c_a_r_d_s_ _|_ _|_â___ _[_J_a_v_a_s_c_r_i_p_t_/
+_T_y_p_e_s_c_r_i_p_t_ _S_D_K_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_A_g_e_n_t_O_p_s_-_A_I_/_a_g_e_n_t_o_p_s_-_n_o_d_e_)_ _|_ _â___ _S_e_s_s_i_o_n
+_r_e_p_l_a_y_s_|_ _ð____ _E_v_a_l_u_a_t_i_o_n_ _p_l_a_y_g_r_o_u_n_d_ _+_ _l_e_a_d_e_r_b_o_a_r_d_|_ _#_#_ _D_e_b_u_g_g_i_n_g_ _R_o_a_d_m_a_p_ _ð__§_­_ _|
+_P_e_r_f_o_r_m_a_n_c_e_ _t_e_s_t_i_n_g_ _|_ _E_n_v_i_r_o_n_m_e_n_t_s_ _|_ _L_L_M_ _T_e_s_t_i_n_g_ _|_ _R_e_a_s_o_n_i_n_g_ _a_n_d_ _e_x_e_c_u_t_i_o_n
+_t_e_s_t_i_n_g_ _|_ _|_-_-_-_|_-_-_-_|_-_-_-_|_-_-_-_|_ _|_â___ _E_v_e_n_t_ _l_a_t_e_n_c_y_ _a_n_a_l_y_s_i_s_ _|_ _ð____ _N_o_n_-_s_t_a_t_i_o_n_a_r_y
+_e_n_v_i_r_o_n_m_e_n_t_ _t_e_s_t_i_n_g_ _|_ _ð____ _L_L_M_ _n_o_n_-_d_e_t_e_r_m_i_n_i_s_t_i_c_ _f_u_n_c_t_i_o_n_ _d_e_t_e_c_t_i_o_n_ _|_ _ð___§
+_I_n_f_i_n_i_t_e_ _l_o_o_p_s_ _a_n_d_ _r_e_c_u_r_s_i_v_e_ _t_h_o_u_g_h_t_ _d_e_t_e_c_t_i_o_n_ _|_ _|_â___ _A_g_e_n_t_ _w_o_r_k_f_l_o_w_ _e_x_e_c_u_t_i_o_n
+_p_r_i_c_i_n_g_ _|_ _ð____ _M_u_l_t_i_-_m_o_d_a_l_ _e_n_v_i_r_o_n_m_e_n_t_s_ _|_ _ð___§_ _T_o_k_e_n_ _l_i_m_i_t_ _o_v_e_r_f_l_o_w_ _f_l_a_g_s_ _|
+_ð____ _F_a_u_l_t_y_ _r_e_a_s_o_n_i_n_g_ _d_e_t_e_c_t_i_o_n_ _|_ _|_ð___§_ _S_u_c_c_e_s_s_ _v_a_l_i_d_a_t_o_r_s_ _(_e_x_t_e_r_n_a_l_)_ _|_ _ð___
+_E_x_e_c_u_t_i_o_n_ _c_o_n_t_a_i_n_e_r_s_ _|_ _ð____ _C_o_n_t_e_x_t_ _l_i_m_i_t_ _o_v_e_r_f_l_o_w_ _f_l_a_g_s_ _|_ _ð____ _G_e_n_e_r_a_t_i_v_e_ _c_o_d_e
+_v_a_l_i_d_a_t_o_r_s_ _|_ _|_ð____ _A_g_e_n_t_ _c_o_n_t_r_o_l_l_e_r_s_/_s_k_i_l_l_ _t_e_s_t_s_ _|_ _â___ _H_o_n_e_y_p_o_t_ _a_n_d_ _p_r_o_m_p_t
+_i_n_j_e_c_t_i_o_n_ _d_e_t_e_c_t_i_o_n_ _(_[_P_r_o_m_p_t_A_r_m_o_r_]_(_h_t_t_p_s_:_/_/_p_r_o_m_p_t_a_r_m_o_r_._c_o_m_)_)_ _|_ _ð____ _A_P_I_ _b_i_l_l
+_t_r_a_c_k_i_n_g_ _|_ _ð____ _E_r_r_o_r_ _b_r_e_a_k_p_o_i_n_t_ _a_n_a_l_y_s_i_s_ _|_ _|_ð____ _I_n_f_o_r_m_a_t_i_o_n_ _c_o_n_t_e_x_t
+_c_o_n_s_t_r_a_i_n_t_ _t_e_s_t_i_n_g_ _|_ _ð____ _A_n_t_i_-_a_g_e_n_t_ _r_o_a_d_b_l_o_c_k_s_ _(_i_._e_._ _C_a_p_t_c_h_a_s_)_ _|_ _ð____ _C_I_/_C_D
+_i_n_t_e_g_r_a_t_i_o_n_ _c_h_e_c_k_s_ _|_ _|_ _|_ð____ _R_e_g_r_e_s_s_i_o_n_ _t_e_s_t_i_n_g_ _|_ _ð____ _M_u_l_t_i_-_a_g_e_n_t_ _f_r_a_m_e_w_o_r_k
+_v_i_s_u_a_l_i_z_a_t_i_o_n_ _|_ _|_ _|_ _#_#_#_ _W_h_y_ _A_g_e_n_t_O_p_s_?_ _ð__¤__ _O_u_r_ _m_i_s_s_i_o_n_ _i_s_ _t_o_ _b_r_i_n_g_ _y_o_u_r_ _a_g_e_n_t
+_f_r_o_m_ _p_r_o_t_o_t_y_p_e_ _t_o_ _p_r_o_d_u_c_t_i_o_n_._ _A_g_e_n_t_ _d_e_v_e_l_o_p_e_r_s_ _o_f_t_e_n_ _w_o_r_k_ _w_i_t_h_ _l_i_t_t_l_e_ _t_o_ _n_o
+_v_i_s_i_b_i_l_i_t_y_ _i_n_t_o_ _a_g_e_n_t_ _t_e_s_t_i_n_g_ _p_e_r_f_o_r_m_a_n_c_e_._ _T_h_i_s_ _m_e_a_n_s_ _t_h_e_i_r_ _a_g_e_n_t_s_ _n_e_v_e_r_ _l_e_a_v_e
+_t_h_e_ _l_a_b_._ _W_e_'_r_e_ _c_h_a_n_g_i_n_g_ _t_h_a_t_._ _A_g_e_n_t_O_p_s_ _i_s_ _t_h_e_ _e_a_s_i_e_s_t_ _w_a_y_ _t_o_ _e_v_a_l_u_a_t_e_,_ _g_r_a_d_e_,
+_a_n_d_ _t_e_s_t_ _a_g_e_n_t_s_._ _I_s_ _t_h_e_r_e_ _a_ _f_e_a_t_u_r_e_ _y_o_u_'_d_ _l_i_k_e_ _t_o_ _s_e_e_ _A_g_e_n_t_O_p_s_ _c_o_v_e_r_?_ _J_u_s_t
+_r_a_i_s_e_ _i_t_ _i_n_ _t_h_e_ _i_s_s_u_e_s_ _t_a_b_,_ _a_n_d_ _w_e_'_l_l_ _w_o_r_k_ _o_n_ _a_d_d_i_n_g_ _i_t_ _t_o_ _t_h_e_ _r_o_a_d_m_a_p_.
```

### Comparing `agentops-0.1.6/agentops/__init__.py` & `agentops-0.1.7/agentops/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 
 def init(api_key: Optional[str] = None,
          parent_key: Optional[str] = None,
          endpoint: Optional[str] = None,
          max_wait_time: Optional[int] = None,
          max_queue_size: Optional[int] = None,
          tags: Optional[List[str]] = None,
-         override=True,
+         override: Optional[bool] = None,  # Deprecated
+         instrument_llm_calls=True,
          auto_start_session=True,
          inherited_session_id: Optional[str] = None
          ):
     """
         Initializes the AgentOps singleton pattern.
 
         Args:
@@ -33,55 +34,97 @@
             endpoint (str, optional): The endpoint for the AgentOps service. If none is provided, key will
                 be read from the AGENTOPS_API_ENDPOINT environment variable. Defaults to 'https://api.agentops.ai'.
             max_wait_time (int, optional): The maximum time to wait in milliseconds before flushing the queue.
                 Defaults to 30,000 (30 seconds)
             max_queue_size (int, optional): The maximum size of the event queue. Defaults to 100.
             tags (List[str], optional): Tags for the sessions that can be used for grouping or
                 sorting later (e.g. ["GPT-4"]).
-            override (bool): Whether to override and LLM calls to emit as events.
+            override (bool, optional): [Deprecated] Use `instrument_llm_calls` instead. Whether to instrument LLM calls and emit LLMEvents..
+            instrument_llm_calls (bool): Whether to instrument LLM calls and emit LLMEvents..
             auto_start_session (bool): Whether to start a session automatically when the client is created.
             inherited_session_id (optional, str): Init Agentops with an existing Session
         Attributes:
-        """
+    """
     set_logging_level_info()
     c = Client(api_key=api_key,
                parent_key=parent_key,
                endpoint=endpoint,
                max_wait_time=max_wait_time,
                max_queue_size=max_queue_size,
                tags=tags,
                override=override,
+               instrument_llm_calls=instrument_llm_calls,
                auto_start_session=auto_start_session,
                inherited_session_id=inherited_session_id
                )
-    
+
     return inherited_session_id or c.current_session_id
 
 
 def end_session(end_state: str,
                 end_state_reason: Optional[str] = None,
                 video: Optional[str] = None):
+    """
+        End the current session with the AgentOps service.
+
+        Args:
+            end_state (str): The final state of the session. Options: Success, Fail, or Indeterminate.
+            end_state_reason (str, optional): The reason for ending the session.
+            video (str, optional): URL to a video recording of the session
+    """
     Client().end_session(end_state, end_state_reason, video)
 
 
 def start_session(tags: Optional[List[str]] = None, config: Optional[Configuration] = None, inherited_session_id: Optional[str] = None):
+    """
+        Start a new session for recording events.
+
+        Args:
+            tags (List[str], optional): Tags that can be used for grouping or sorting later.
+                e.g. ["test_run"].
+            config: (Configuration, optional): Client configuration object
+    """
     return Client().start_session(tags, config, inherited_session_id)
 
 
 def record(event: Event | ErrorEvent):
+    """
+        Record an event with the AgentOps service.
+
+        Args:
+            event (Event): The event to record.
+    """
     Client().record(event)
 
 
 def add_tags(tags: List[str]):
+    """
+        Append to session tags at runtime. 
+
+        Args:
+            tags (List[str]): The list of tags to append.
+    """
     Client().add_tags(tags)
 
 
 def set_tags(tags: List[str]):
+    """
+        Replace session tags at runtime. 
+
+        Args:
+            tags (List[str]): The list of tags to set.
+    """
     Client().set_tags(tags)
 
 
 def get_api_key() -> str:
     return Client().api_key
 
 
 def set_parent_key(parent_key):
+    """
+        Set the parent API key which has visibility to projects it is parent to.
+
+        Args:
+            parent_key (str): The API key of the parent organization to set.
+    """
     Client().set_parent_key(parent_key)
```

### Comparing `agentops-0.1.6/agentops/agent.py` & `agentops-0.1.7/agentops/agent.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.6/agentops/client.py` & `agentops-0.1.7/agentops/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,122 +1,154 @@
 """
-AgentOps client module that provides a client class with public interfaces and configuration.
+    AgentOps client module that provides a client class with public interfaces and configuration.
 
-Classes:
-    Client: Provides methods to interact with the AgentOps service.
+    Classes:
+        Client: Provides methods to interact with the AgentOps service.
 """
-
+import os
 from .event import ActionEvent, ErrorEvent, Event
 from .enums import EndState
 from .helpers import get_ISO_time, singleton, check_call_stack_for_agent_id
 from .session import Session
 from .worker import Worker
 from .host_env import get_host_env
 from uuid import uuid4
 from typing import Optional, List
 import traceback
 from .log_config import logger, set_logging_level_info
+from decimal import Decimal
 import inspect
 import atexit
 import signal
 import sys
 import threading
 
+
 from .meta_client import MetaClient
 from .config import Configuration, ConfigurationError
 from .llm_tracker import LlmTracker
 
 
 @singleton
 class Client(metaclass=MetaClient):
     """
-    Client for AgentOps service.
+        Client for AgentOps service.
 
-    Args:
+        Args:
 
-        api_key (str, optional): API Key for AgentOps services. If none is provided, key will 
-            be read from the AGENTOPS_API_KEY environment variable.
-        parent_key (str, optional): Organization key to give visibility of all user sessions the user's organization. If none is provided, key will 
-            be read from the AGENTOPS_PARENT_KEY environment variable.
-        endpoint (str, optional): The endpoint for the AgentOps service. If none is provided, key will 
-            be read from the AGENTOPS_API_ENDPOINT environment variable. Defaults to 'https://api.agentops.ai'.
-        max_wait_time (int, optional): The maximum time to wait in milliseconds before flushing the queue. 
-            Defaults to 30,000 (30 seconds)
-        max_queue_size (int, optional): The maximum size of the event queue. Defaults to 100.
-        tags (List[str], optional): Tags for the sessions that can be used for grouping or 
-            sorting later (e.g. ["GPT-4"]).
-        override (bool): Whether to override and LLM calls to emit as events.
-        auto_start_session (bool): Whether to start a session automatically when the client is created.
-        inherited_session_id (optional, str): Init Agentops with an existing Session
-    Attributes:
-        _session (Session, optional): A Session is a grouping of events (e.g. a run of your agent).
-        _worker (Worker, optional): A Worker manages the event queue and sends session updates to the AgentOps api server
+            api_key (str, optional): API Key for AgentOps services. If none is provided, key will
+                be read from the AGENTOPS_API_KEY environment variable.
+            parent_key (str, optional): Organization key to give visibility of all user sessions the user's organization. If none is provided, key will
+                be read from the AGENTOPS_PARENT_KEY environment variable.
+            endpoint (str, optional): The endpoint for the AgentOps service. If none is provided, key will
+                be read from the AGENTOPS_API_ENDPOINT environment variable. Defaults to 'https://api.agentops.ai'.
+            max_wait_time (int, optional): The maximum time to wait in milliseconds before flushing the queue.
+                Defaults to 30,000 (30 seconds)
+            max_queue_size (int, optional): The maximum size of the event queue. Defaults to 100.
+            tags (List[str], optional): Tags for the sessions that can be used for grouping or
+                sorting later (e.g. ["GPT-4"]).
+            override (bool, optional): [Deprecated] Use `instrument_llm_calls` instead. Whether to instrument LLM calls and emit LLMEvents..
+            instrument_llm_calls (bool): Whether to instrument LLM calls and emit LLMEvents..
+            auto_start_session (bool): Whether to start a session automatically when the client is created.
+            inherited_session_id (optional, str): Init Agentops with an existing Session
+        Attributes:
+            _session (Session, optional): A Session is a grouping of events (e.g. a run of your agent).
+            _worker (Worker, optional): A Worker manages the event queue and sends session updates to the AgentOps api server
     """
 
     def __init__(self,
                  api_key: Optional[str] = None,
                  parent_key: Optional[str] = None,
                  endpoint: Optional[str] = None,
                  max_wait_time: Optional[int] = None,
                  max_queue_size: Optional[int] = None,
                  tags: Optional[List[str]] = None,
-                 override=True,
+                 override: Optional[bool] = None,  # Deprecated
+                 instrument_llm_calls=True,
                  auto_start_session=True,
                  inherited_session_id: Optional[str] = None
                  ):
 
+        if override is not None:
+            logger.warning("🖇 AgentOps: The 'override' parameter is deprecated. Use 'instrument_llm_calls' instead.",
+                           DeprecationWarning, stacklevel=2)
+            instrument_llm_calls = instrument_llm_calls or override
+
         self._session = None
         self._worker = None
-        self._tags = tags
+        self._tags_for_future_session = None
+
+        self._env_data_opt_out = os.getenv('AGENTOPS_ENV_DATA_OPT_OUT') and os.getenv('AGENTOPS_ENV_DATA_OPT_OUT').lower() == 'true'
 
         try:
             self.config = Configuration(api_key=api_key,
                                         parent_key=parent_key,
                                         endpoint=endpoint,
                                         max_wait_time=max_wait_time,
                                         max_queue_size=max_queue_size)
         except ConfigurationError:
             return
 
         self._handle_unclean_exits()
 
         if auto_start_session:
             self.start_session(tags, self.config, inherited_session_id)
+        else:
+            self._tags_for_future_session = tags
 
-        if override:
-            if 'openai' in sys.modules:
-                self.llm_tracker = LlmTracker(self)
-                self.llm_tracker.override_api('openai')
+        if instrument_llm_calls:
+            self.llm_tracker = LlmTracker(self)
+            self.llm_tracker.override_api()
 
     def add_tags(self, tags: List[str]):
-        if self._tags is not None:
-            self._tags.extend(tags)
+        """
+            Append to session tags at runtime.
+
+            Args:
+                tags (List[str]): The list of tags to append.
+        """
+        if self._session.tags is not None:
+            for tag in tags:
+                if tag not in self._session.tags:
+                    self._session.tags.append(tag)
         else:
-            self._tags = tags
+            self._session.tags = tags
 
         if self._session is not None:
-            self._session.tags = self._tags
             self._worker.update_session(self._session)
 
     def set_tags(self, tags: List[str]):
-        self._tags = tags
+        """
+            Replace session tags at runtime.
+
+            Args:
+                tags (List[str]): The list of tags to set.
+        """
+        self._tags_for_future_session = tags
 
         if self._session is not None:
             self._session.tags = tags
             self._worker.update_session(self._session)
 
     def record(self, event: Event | ErrorEvent):
         """
-        Record an event with the AgentOps service.
+            Record an event with the AgentOps service.
 
-        Args:
-            event (Event): The event to record.
+            Args:
+                event (Event): The event to record.
         """
-
+        if not event.end_timestamp or event.init_timestamp == event.end_timestamp:
+            event.end_timestamp = get_ISO_time()
         if self._session is not None and not self._session.has_ended:
+            if isinstance(event, ErrorEvent):
+                if event.trigger_event:
+                    event.trigger_event_id = event.trigger_event.id
+                    event.trigger_event_type = event.trigger_event.event_type
+                    self._worker.add_event(event.trigger_event.__dict__)
+                    event.trigger_event = None  # removes trigger_event from serialization
             self._worker.add_event(event.__dict__)
         else:
             logger.warning(
                 "🖇 AgentOps: Cannot record event - no current session")
 
     def _record_event_sync(self, func, event_name, *args, **kwargs):
         init_time = get_ISO_time()
@@ -140,17 +172,14 @@
 
             # If the function returns multiple values, record them all in the same event
             if isinstance(returns, tuple):
                 returns = list(returns)
 
             event.returns = returns
             event.end_timestamp = get_ISO_time()
-            # TODO: If func excepts this will never get called
-            # the dev loses all the useful stuff in ActionEvent they would need for debugging
-            # we should either record earlier or have Error post the supplied event to supabase
             self.record(event)
 
         except Exception as e:
             self.record(ErrorEvent(trigger_event=event, exception=e))
 
             # Re-raise the exception
             raise
@@ -179,82 +208,81 @@
 
             # If the function returns multiple values, record them all in the same event
             if isinstance(returns, tuple):
                 returns = list(returns)
 
             event.returns = returns
             event.end_timestamp = get_ISO_time()
-            # TODO: If func excepts this will never get called
-            # the dev loses all the useful stuff in ActionEvent they would need for debugging
-            # we should either record earlier or have Error post the supplied event to supabase
             self.record(event)
 
         except Exception as e:
             self.record(ErrorEvent(trigger_event=event, exception=e))
 
             # Re-raise the exception
             raise
 
         return returns
 
     def start_session(self, tags: Optional[List[str]] = None, config: Optional[Configuration] = None, inherited_session_id: Optional[str] = None):
         """
-        Start a new session for recording events.
+            Start a new session for recording events.
 
-        Args:
-            tags (List[str], optional): Tags that can be used for grouping or sorting later.
-                e.g. ["test_run"].
-            config: (Configuration, optional): Client configuration object
-            inherited_session_id (optional, str): assign session id to match existing Session
+            Args:
+                tags (List[str], optional): Tags that can be used for grouping or sorting later.
+                    e.g. ["test_run"].
+                config: (Configuration, optional): Client configuration object
+                inherited_session_id (optional, str): assign session id to match existing Session
         """
         set_logging_level_info()
-        
+
         if self._session is not None:
             return logger.warning("🖇 AgentOps: Cannot start session - session already started")
 
         if not config and not self.config:
             return logger.warning("🖇 AgentOps: Cannot start session - missing configuration")
 
-        self._session = Session(inherited_session_id or uuid4(), tags or self._tags, host_env=get_host_env())
+        self._session = Session(inherited_session_id or uuid4(), tags or self._tags_for_future_session, host_env=get_host_env(self._env_data_opt_out))
         self._worker = Worker(config or self.config)
         start_session_result = self._worker.start_session(self._session)
         if not start_session_result:
             self._session = None
             return logger.warning("🖇 AgentOps: Cannot start session")
 
         logger.info('View info on this session at https://app.agentops.ai/drilldown?session_id={}'
-                     .format(self._session.session_id))
+                    .format(self._session.session_id))
 
         return self._session.session_id
 
     def end_session(self,
                     end_state: str,
                     end_state_reason: Optional[str] = None,
                     video: Optional[str] = None):
         """
-        End the current session with the AgentOps service.
+            End the current session with the AgentOps service.
 
-        Args:
-            end_state (str): The final state of the session. Options: Success, Fail, or Indeterminate.
-            end_state_reason (str, optional): The reason for ending the session.
-            video (str, optional): The video screen recording of the session
+            Args:
+                end_state (str): The final state of the session. Options: Success, Fail, or Indeterminate.
+                end_state_reason (str, optional): The reason for ending the session.
+                video (str, optional): The video screen recording of the session
         """
         if self._session is None or self._session.has_ended:
             return logger.warning("🖇 AgentOps: Cannot end session - no current session")
 
         if not any(end_state == state.value for state in EndState):
             return logger.warning("🖇 AgentOps: Invalid end_state. Please use one of the EndState enums")
 
         self._session.video = video
         self._session.end_session(end_state, end_state_reason)
         token_cost = self._worker.end_session(self._session)
         if token_cost == 'unknown':
             print('🖇 AgentOps: Could not determine cost of run.')
         else:
-            print('🖇 AgentOps: This run cost ${:.6f}'.format(float(token_cost)))
+            token_cost_d = Decimal(token_cost)
+            print('🖇 AgentOps: This run cost ${}'.format('{:.2f}'.format(
+                token_cost_d) if token_cost_d == 0 else '{:.6f}'.format(token_cost_d)))
         self._session = None
         self._worker = None
 
     def create_agent(self, agent_id: str, name: str):
         if self._worker:
             self._worker.create_agent(agent_id, name)
 
@@ -263,36 +291,36 @@
             # Only run cleanup function if session is created
             if self._session is not None:
                 self.end_session(end_state=end_state,
                                  end_state_reason=end_state_reason)
 
         def signal_handler(signum, frame):
             """
-            Signal handler for SIGINT (Ctrl+C) and SIGTERM. Ends the session and exits the program.
+                Signal handler for SIGINT (Ctrl+C) and SIGTERM. Ends the session and exits the program.
 
-            Args:
-                signum (int): The signal number.
-                frame: The current stack frame.
+                Args:
+                    signum (int): The signal number.
+                    frame: The current stack frame.
             """
             signal_name = 'SIGINT' if signum == signal.SIGINT else 'SIGTERM'
             logger.info(
                 f'🖇 AgentOps: {signal_name} detected. Ending session...')
             self.end_session(end_state='Fail',
                              end_state_reason=f'Signal {signal_name} detected')
             sys.exit(0)
 
         def handle_exception(exc_type, exc_value, exc_traceback):
             """
-            Handle uncaught exceptions before they result in program termination.
+                Handle uncaught exceptions before they result in program termination.
 
-            Args:
-                exc_type (Type[BaseException]): The type of the exception.
-                exc_value (BaseException): The exception instance.
-                exc_traceback (TracebackType): A traceback object encapsulating the call stack at the 
-                                               point where the exception originally occurred.
+                Args:
+                    exc_type (Type[BaseException]): The type of the exception.
+                    exc_value (BaseException): The exception instance.
+                    exc_traceback (TracebackType): A traceback object encapsulating the call stack at the
+                                                point where the exception originally occurred.
             """
             formatted_traceback = ''.join(traceback.format_exception(exc_type, exc_value,
                                                                      exc_traceback))
 
             self.end_session(end_state='Fail',
                              end_state_reason=f"{str(exc_value)}: {formatted_traceback}")
 
@@ -311,14 +339,20 @@
     def current_session_id(self):
         return self._session.session_id if self._session else None
 
     @property
     def api_key(self):
         return self.config.api_key
 
-    def set_parent_key(self, parent_key):
+    def set_parent_key(self, parent_key: str):
+        """
+            Set the parent API key which has visibility to projects it is parent to.
+
+            Args:
+                parent_key (str): The API key of the parent organization to set.
+        """
         if self._worker:
             self._worker.config.parent_key = parent_key
 
     @property
     def parent_key(self):
         return self.config.parent_key
```

### Comparing `agentops-0.1.6/agentops/config.py` & `agentops-0.1.7/agentops/config.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.6/agentops/decorators.py` & `agentops-0.1.7/agentops/decorators.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.6/agentops/enums.py` & `agentops-0.1.7/agentops/enums.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.6/agentops/event.py` & `agentops-0.1.7/agentops/event.py`

 * *Files 6% similar despite different names*

```diff
@@ -131,15 +131,11 @@
     code: Optional[str] = None
     details: Optional[str] = None
     logs: Optional[str] = field(default_factory=traceback.format_exc)
     timestamp: str = field(default_factory=get_ISO_time)
 
     def __post_init__(self):
         self.event_type = EventType.ERROR.value
-        if self.trigger_event:
-            self.trigger_event_id = self.trigger_event.id
-            self.trigger_event_type = self.trigger_event.event_type
-            self.trigger_event = None  # removes trigger_event from serialization
         if self.exception:
             self.error_type = self.error_type or type(self.exception).__name__
             self.details = self.details or str(self.exception)
             self.exception = None  # removes exception from serialization
```

### Comparing `agentops-0.1.6/agentops/helpers.py` & `agentops-0.1.7/agentops/helpers.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.6/agentops/host_env.py` & `agentops-0.1.7/agentops/host_env.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,59 @@
 import platform
 import psutil
 import socket
 from .helpers import get_agentops_version
 
 
 def get_sdk_details():
-    return {
-        "AgentOps SDK Version": get_agentops_version(),
-        "Python Version": platform.python_version(),
-    }
+    try:
+        return {
+            "AgentOps SDK Version": get_agentops_version(),
+            "Python Version": platform.python_version(),
+        }
+    except:
+        return {}
 
 
 def get_os_details():
-    return {
-        "Hostname": socket.gethostname(),
-        "OS": platform.system(),
-        "OS Version": platform.version(),
-        "OS Release": platform.release()
-    }
+    try:
+        return {
+            "Hostname": socket.gethostname(),
+            "OS": platform.system(),
+            "OS Version": platform.version(),
+            "OS Release": platform.release()
+        }
+    except:
+        return {}
 
 
 def get_cpu_details():
-    return {
-        "Physical cores": psutil.cpu_count(logical=False),
-        "Total cores": psutil.cpu_count(logical=True),
-        # "Max Frequency": f"{psutil.cpu_freq().max:.2f}Mhz", # Fails right now
-        "CPU Usage": f"{psutil.cpu_percent()}%"
-    }
+    try:
+        return {
+            "Physical cores": psutil.cpu_count(logical=False),
+            "Total cores": psutil.cpu_count(logical=True),
+            # "Max Frequency": f"{psutil.cpu_freq().max:.2f}Mhz", # Fails right now
+            "CPU Usage": f"{psutil.cpu_percent()}%"
+        }
+    except:
+        return {}
 
 
 def get_ram_details():
-    ram_info = psutil.virtual_memory()
-    return {
-        "Total": f"{ram_info.total / (1024**3):.2f} GB",
-        "Available": f"{ram_info.available / (1024**3):.2f} GB",
-        "Used": f"{ram_info.used / (1024**3):.2f} GB",
-        "Percentage": f"{ram_info.percent}%"
-    }
+    try:
+        ram_info = psutil.virtual_memory()
+        return {
+            "Total": f"{ram_info.total / (1024 ** 3):.2f} GB",
+            "Available": f"{ram_info.available / (1024 ** 3):.2f} GB",
+            "Used": f"{ram_info.used / (1024 ** 3):.2f} GB",
+            "Percentage": f"{ram_info.percent}%"
+        }
+    except:
+        return {}
+
 
 
 def get_disk_details():
     partitions = psutil.disk_partitions()
     disk_info = {}
     for partition in partitions:
         usage = psutil.disk_usage(partition.mountpoint)
@@ -50,15 +63,21 @@
             "Used": f"{usage.used / (1024**3):.2f} GB",
             "Free": f"{usage.free / (1024**3):.2f} GB",
             "Percentage": f"{usage.percent}%"
         }
     return disk_info
 
 
-def get_host_env():
-    return {
-        "SDK": get_sdk_details(),
-        "OS": get_os_details(),
-        "CPU": get_cpu_details(),
-        "RAM": get_ram_details(),
-        "Disk": get_disk_details(),
-    }
+def get_host_env(opt_out: bool = False):
+    if opt_out:
+        return {
+            "SDK": get_sdk_details(),
+            "OS": get_os_details()
+        }
+    else:
+        return {
+            "SDK": get_sdk_details(),
+            "OS": get_os_details(),
+            "CPU": get_cpu_details(),
+            "RAM": get_ram_details(),
+            "Disk": get_disk_details(),
+        }
```

### Comparing `agentops-0.1.6/agentops/http_client.py` & `agentops-0.1.7/agentops/http_client.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.6/agentops/langchain_callback_handler.py` & `agentops-0.1.7/agentops/langchain_callback_handler.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.6/agentops/llm_tracker.py` & `agentops-0.1.7/agentops/llm_tracker.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,71 +1,81 @@
 import functools
 import sys
 from importlib import import_module
-from packaging.version import parse
+from importlib.metadata import version
+from packaging.version import Version, parse
 from .log_config import logger
 from .event import LLMEvent, ErrorEvent
 from .helpers import get_ISO_time, check_call_stack_for_agent_id
 import inspect
+import pprint
 
 
 class LlmTracker:
     SUPPORTED_APIS = {
+        'litellm': {'1.3.1': ("openai_chat_completions.completion",)},
         'openai': {
             '1.0.0': (
                 "chat.completions.create",
             ),
             '0.0.0':
                 (
                 "ChatCompletion.create",
                 "ChatCompletion.acreate",
             ),
         }
     }
 
     def __init__(self, client):
         self.client = client
-        self.completion = ""
-        self.llm_event: LLMEvent = None
 
     def _handle_response_v0_openai(self, response, kwargs, init_timestamp):
         """Handle responses for OpenAI versions <v1.0.0"""
 
-        self.completion = ""
-        self.llm_event = None
+        self.llm_event = LLMEvent(
+            init_timestamp=init_timestamp,
+            params=kwargs
+        )
 
         def handle_stream_chunk(chunk):
-            self.llm_event = LLMEvent(
-                init_timestamp=init_timestamp,
-                params=kwargs
-            )
+            # NOTE: prompt/completion usage not returned in response when streaming
+            # We take the first ChatCompletionChunk and accumulate the deltas from all subsequent chunks to build one full chat completion
+            if self.llm_event.returns == None:
+                self.llm_event.returns = chunk
 
             try:
-                # NOTE: prompt/completion usage not returned in response when streaming
-                model = chunk['model']
-                choices = chunk['choices']
-                token = choices[0]['delta'].get('content', '')
-                finish_reason = choices[0]['finish_reason']
-                if token:
-                    self.completion += token
-
-                if finish_reason:
-                    self.llm_event.agent_id = check_call_stack_for_agent_id()
-                    self.llm_event.prompt = kwargs["messages"]
-                    self.llm_event.completion = {"role": "assistant", "content": self.completion}
-                    self.llm_event.returns = {"finish_reason": finish_reason, "content": self.completion}
-                    self.llm_event.model = model
+                accumulated_delta = self.llm_event.returns['choices'][0]['delta']
+                self.llm_event.agent_id = check_call_stack_for_agent_id()
+                self.llm_event.model = chunk['model']
+                self.llm_event.prompt = kwargs["messages"]
+                choice = chunk['choices'][0]  # NOTE: We assume for completion only choices[0] is relevant
+
+                if choice['delta'].get('content'):
+                    accumulated_delta['content'] += choice['delta'].content
+
+                if choice['delta'].get('role'):
+                    accumulated_delta['role'] = choice['delta'].get('role')
+
+                if choice['finish_reason']:
+                    # Streaming is done. Record LLMEvent
+                    self.llm_event.returns.choices[0]['finish_reason'] = choice['finish_reason']
+                    self.llm_event.completion = {
+                        "role": accumulated_delta['role'], "content": accumulated_delta['content']}
                     self.llm_event.end_timestamp = get_ISO_time()
 
                     self.client.record(self.llm_event)
             except Exception as e:
                 self.client.record(ErrorEvent(trigger_event=self.llm_event, exception=e))
-                # TODO: This error is specific to only one path of failure. Should be more generic or have different logger for different paths
+                kwargs_str = pprint.pformat(kwargs)
+                chunk = pprint.pformat(chunk)
                 logger.warning(
-                    f"🖇 AgentOps: Unable to parse a chunk for LLM call {kwargs} - skipping upload to AgentOps")
+                    f"🖇 AgentOps: Unable to parse a chunk for LLM call. Skipping upload to AgentOps\n"
+                    f"chunk:\n {chunk}\n"
+                    f"kwargs:\n {kwargs_str}\n"
+                )
 
         # if the response is a generator, decorate the generator
         if inspect.isasyncgen(response):
             async def async_generator():
                 async for chunk in response:
                     handle_stream_chunk(chunk)
 
@@ -78,79 +88,93 @@
                     handle_stream_chunk(chunk)
 
                     yield chunk
             return generator()
 
         self.llm_event = LLMEvent(
             init_timestamp=init_timestamp,
-            params=kwargs
+            params=kwargs,
+            returns=response
         )
         # v0.0.0 responses are dicts
         try:
             self.llm_event.agent_id = check_call_stack_for_agent_id()
             self.llm_event.prompt = kwargs["messages"]
             self.llm_event.prompt_tokens = response['usage']['prompt_tokens']
             self.llm_event.completion = {"role": "assistant", "content": response['choices'][0]['message']['content']}
             self.llm_event.completion_tokens = response['usage']['completion_tokens']
-            self.llm_event.returns = {"content": response['choices'][0]['message']['content']}
             self.llm_event.model = response["model"]
             self.llm_event.end_timestamp = get_ISO_time()
 
             self.client.record(self.llm_event)
         except Exception as e:
             self.client.record(ErrorEvent(trigger_event=self.llm_event, exception=e))
-            # TODO: This error is specific to only one path of failure. Should be more generic or have different logger for different paths
+            kwargs_str = pprint.pformat(kwargs)
+            response = pprint.pformat(response)
             logger.warning(
-                f"🖇 AgentOps: Unable to parse a chunk for LLM call {kwargs} - skipping upload to AgentOps")
+                f"🖇 AgentOps: Unable to parse response for LLM call. Skipping upload to AgentOps\n"
+                f"response:\n {response}\n"
+                f"kwargs:\n {kwargs_str}\n"
+            )
 
         return response
 
     def _handle_response_v1_openai(self, response, kwargs, init_timestamp):
         """Handle responses for OpenAI versions >v1.0.0"""
         from openai import Stream, AsyncStream
         from openai.types.chat import ChatCompletionChunk
         from openai.resources import AsyncCompletions
 
-        self.completion = ""
-        self.llm_event = None
+        self.llm_event = LLMEvent(
+            init_timestamp=init_timestamp,
+            params=kwargs
+        )
 
         def handle_stream_chunk(chunk: ChatCompletionChunk):
-
-            self.llm_event = LLMEvent(
-                init_timestamp=init_timestamp,
-                params=kwargs
-            )
+            # NOTE: prompt/completion usage not returned in response when streaming
+            # We take the first ChatCompletionChunk and accumulate the deltas from all subsequent chunks to build one full chat completion
+            if self.llm_event.returns == None:
+                self.llm_event.returns = chunk
 
             try:
-                # NOTE: prompt/completion usage not returned in response when streaming
-                model = chunk.model
-                choices = chunk.choices
-                token = choices[0].delta.content
-                finish_reason = choices[0].finish_reason
-                function_call = choices[0].delta.function_call
-                tool_calls = choices[0].delta.tool_calls
-                role = choices[0].delta.role
-                if token:
-                    self.completion += token
-
-                if finish_reason:
-                    self.llm_event.agent_id = check_call_stack_for_agent_id()
-                    self.llm_event.prompt = kwargs["messages"]
-                    self.llm_event.completion = {"role": "assistant", "content": self.completion}
-                    self.llm_event.returns = {"finish_reason": finish_reason, "content": self.completion,
-                                              "function_call": function_call, "tool_calls": tool_calls, "role": role}
-                    self.llm_event.model = model
+                accumulated_delta = self.llm_event.returns.choices[0].delta
+                self.llm_event.agent_id = check_call_stack_for_agent_id()
+                self.llm_event.model = chunk.model
+                self.llm_event.prompt = kwargs["messages"]
+                choice = chunk.choices[0]  # NOTE: We assume for completion only choices[0] is relevant
+
+                if choice.delta.content:
+                    accumulated_delta.content += choice.delta.content
+
+                if choice.delta.role:
+                    accumulated_delta.role = choice.delta.role
+
+                if choice.delta.tool_calls:
+                    accumulated_delta.tool_calls = choice.delta.tool_calls
+
+                if choice.delta.function_call:
+                    accumulated_delta.function_call = choice.delta.function_call
+
+                if choice.finish_reason:
+                    # Streaming is done. Record LLMEvent
+                    self.llm_event.returns.choices[0].finish_reason = choice.finish_reason
+                    self.llm_event.completion = {"role": accumulated_delta.role, "content": accumulated_delta.content,
+                                                 "function_call": accumulated_delta.function_call, "tool_calls": accumulated_delta.tool_calls}
                     self.llm_event.end_timestamp = get_ISO_time()
 
                     self.client.record(self.llm_event)
             except Exception as e:
                 self.client.record(ErrorEvent(trigger_event=self.llm_event, exception=e))
-                # TODO: This error is specific to only one path of failure. Should be more generic or have different logger for different paths
+                kwargs_str = pprint.pformat(kwargs)
+                chunk = pprint.pformat(chunk)
                 logger.warning(
-                    f"🖇 AgentOps: Unable to parse a chunk for LLM call {kwargs} - skipping upload to AgentOps")
+                    f"🖇 AgentOps: Unable to parse a chunk for LLM call. Skipping upload to AgentOps\n"
+                    f"chunk:\n {chunk}\n"
+                    f"kwargs:\n {kwargs_str}\n"
+                )
 
         # if the response is a generator, decorate the generator
         if isinstance(response, Stream):
             def generator():
                 for chunk in response:
                     handle_stream_chunk(chunk)
                     yield chunk
@@ -174,63 +198,93 @@
 
         self.llm_event = LLMEvent(
             init_timestamp=init_timestamp,
             params=kwargs
         )
         # v1.0.0+ responses are objects
         try:
+            self.llm_event.returns = response.model_dump()
             self.llm_event.agent_id = check_call_stack_for_agent_id()
             self.llm_event.prompt = kwargs["messages"]
             self.llm_event.prompt_tokens = response.usage.prompt_tokens
             self.llm_event.completion = response.choices[0].message.model_dump()
             self.llm_event.completion_tokens = response.usage.completion_tokens
-            self.llm_event.returns = response.model_dump()
             self.llm_event.model = response.model
 
             self.client.record(self.llm_event)
         except Exception as e:
             self.client.record(ErrorEvent(trigger_event=self.llm_event, exception=e))
-            # TODO: This error is specific to only one path of failure. Should be more generic or have different logger for different paths
+            kwargs_str = pprint.pformat(kwargs)
+            response = pprint.pformat(response)
             logger.warning(
-                f"🖇 AgentOps: Unable to parse a chunk for LLM call {kwargs} - skipping upload to AgentOps")
+                f"🖇 AgentOps: Unable to parse response for LLM call. Skipping upload to AgentOps\n"
+                f"response:\n {response}\n"
+                f"kwargs:\n {kwargs_str}\n"
+            )
 
         return response
 
     def override_openai_v1_completion(self):
         from openai.resources.chat import completions
 
         # Store the original method
         original_create = completions.Completions.create
 
-        # Define the patched function
         def patched_function(*args, **kwargs):
             init_timestamp = get_ISO_time()
             # Call the original function with its original arguments
             result = original_create(*args, **kwargs)
             return self._handle_response_v1_openai(result, kwargs, init_timestamp)
 
       # Override the original method with the patched one
         completions.Completions.create = patched_function
 
     def override_openai_v1_async_completion(self):
         from openai.resources.chat import completions
 
         # Store the original method
         original_create = completions.AsyncCompletions.create
-        # Define the patched function
 
         async def patched_function(*args, **kwargs):
             # Call the original function with its original arguments
             init_timestamp = get_ISO_time()
             result = await original_create(*args, **kwargs)
             return self._handle_response_v1_openai(result, kwargs, init_timestamp)
 
         # Override the original method with the patched one
         completions.AsyncCompletions.create = patched_function
 
+    def override_litellm_completion(self):
+        import litellm
+
+        original_create = litellm.completion
+
+        def patched_function(*args, **kwargs):
+            init_timestamp = get_ISO_time()
+            result = original_create(*args, **kwargs)
+            # Note: litellm calls all LLM APIs using the OpenAI format
+            return self._handle_response_v1_openai(result, kwargs, init_timestamp)
+
+        litellm.completion = patched_function
+
+    def override_litellm_async_completion(self):
+        import litellm
+
+        original_create = litellm.acompletion
+
+        async def patched_function(*args, **kwargs):
+            # Call the original function with its original arguments
+            init_timestamp = get_ISO_time()
+            result = await original_create(*args, **kwargs)
+            # Note: litellm calls all LLM APIs using the OpenAI format
+            return self._handle_response_v1_openai(result, kwargs, init_timestamp)
+
+        # Override the original method with the patched one
+        litellm.acompletion = patched_function
+
     def _override_method(self, api, method_path, module):
         def handle_response(result, kwargs, init_timestamp):
             if api == "openai":
                 return self._handle_response_v0_openai(result, kwargs, init_timestamp)
             return result
 
         def wrap_method(original_method):
@@ -256,28 +310,35 @@
 
         if len(method_parts) == 1:
             setattr(module, method_parts[0], new_method)
         else:
             parent = functools.reduce(getattr, method_parts[:-1], module)
             setattr(parent, method_parts[-1], new_method)
 
-    def override_api(self, api):
+    def override_api(self):
         """
         Overrides key methods of the specified API to record events.
         """
-        if api in sys.modules:
-            if api not in self.SUPPORTED_APIS:
-                raise ValueError(f"Unsupported API: {api}")
-
-            module = import_module(api)
-            if api == 'openai':
-                # Patch openai v1.0.0+ methods
-                if hasattr(module, '__version__'):
-                    module_version = parse(module.__version__)
-                    if module_version >= parse('1.0.0'):
-                        self.override_openai_v1_completion()
-                        self.override_openai_v1_async_completion()
-                        return
-
-                # Patch openai <v1.0.0 methods
-                for method_path in self.SUPPORTED_APIS['openai']['0.0.0']:
-                    self._override_method(api, method_path, module)
+
+        for api in self.SUPPORTED_APIS:
+            if api in sys.modules:
+                module = import_module(api)
+                if api == 'litellm':
+                    module_version = version(api)
+                    if Version(module_version) >= parse('1.3.1'):
+                        self.override_litellm_completion()
+                        self.override_litellm_async_completion()
+                    else:
+                        logger.warning(f'🖇 AgentOps: Only litellm>=1.3.1 supported. v{module_version} found.')
+                    return  # If using an abstraction like litellm, do not patch the underlying LLM APIs
+
+                if api == 'openai':
+                    # Patch openai v1.0.0+ methods
+                    if hasattr(module, '__version__'):
+                        module_version = parse(module.__version__)
+                        if module_version >= parse('1.0.0'):
+                            self.override_openai_v1_completion()
+                            self.override_openai_v1_async_completion()
+                        else:
+                            # Patch openai <v1.0.0 methods
+                            for method_path in self.SUPPORTED_APIS['openai']['0.0.0']:
+                                self._override_method(api, method_path, module)
```

### Comparing `agentops-0.1.6/agentops/meta_client.py` & `agentops-0.1.7/agentops/meta_client.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.6/agentops/session.py` & `agentops-0.1.7/agentops/session.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.6/agentops/worker.py` & `agentops-0.1.7/agentops/worker.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.6/agentops.egg-info/PKG-INFO` & `agentops-0.1.7/agentops.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: agentops
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python SDK for developing AI agent evals and observability
 Author-email: Alex Reibman <areibman@gmail.com>, Shawn Qiu <siyangqiu@gmail.com>, Braelyn Boynton <bboynton97@gmail.com>, Howard Gil <howardbgil@gmail.com>
 Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
 Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.31.0
 Requires-Dist: psutil==5.9.8
 Requires-Dist: packaging==23.2
 Provides-Extra: dev
 Requires-Dist: pytest==7.4.0; extra == "dev"
 Requires-Dist: requests_mock==1.11.0; extra == "dev"
 Provides-Extra: langchain
 Requires-Dist: langchain>=0.0.354; extra == "langchain"
 
 <div align="center">
-  <img src="logo.png" style="margin: 15px; max-width: 300px" width="50%" alt="Logo">
+  <a href="https://agentops.ai?ref=gh">
+    <img src="logo.png" style="margin: 15px; max-width: 300px" width="50%" alt="Logo">
+  </a>
 </div>
 <p align="center">
   <em>AI agents suck. We’re fixing that.</em>
 </p>
 
 <p align="center">
     <a href="https://pypi.org/project/agentops/" target="_blank">
@@ -34,44 +36,55 @@
     </a>
 </p>
 <p align="center">
 <a href="https://twitter.com/agentopsai/">🐦 Twitter</a>
 <span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
 <a href="https://discord.gg/JHPt4C7r">📢 Discord</a>
 <span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
-<a href="https://app.agentops.ai/?=gh">🖇️ AgentOps</a>
+<a href="https://app.agentops.ai/?ref=gh">🖇️ AgentOps</a>
 <span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
 <a href="https://docs.agentops.ai/introduction">📙 Documentation</a>
 </p>
 
-# AgentOps
-
-Build your next agent with benchmarks, observability, and replay analytics. AgentOps is the toolkit for evaluating and developing robust and reliable AI agents.
-
-You can sign up for AgentOps [here](https://app.agentops.ai).
+# AgentOps 🖇️
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) ![PyPI - Version](https://img.shields.io/pypi/v/agentops) <a href="https://pepy.tech/project/agentops">
   <img src="https://static.pepy.tech/badge/agentops/month"> <a href="https://twitter.com/agentopsai">
     <img src="https://img.shields.io/badge/follow-%40agentops-1DA1F2?logo=twitter&style=social" alt="AgentOps Twitter" /> 
   </a>
-<a href="https://discord.gg/mKW3ZhN9p2">
+  <a href="https://discord.gg/mKW3ZhN9p2">
     <img src="https://img.shields.io/badge/chat-on%20Discord-blueviolet" alt="Discord community channel" />
   </a>
-  <a href="mailto:investor@agentops.ai"><img src="https://img.shields.io/website?color=%23f26522&down_message=Y%20Combinator&label=Not%20Backed%20By&logo=ycombinator&style=flat-square&up_message=Y%20Combinator&url=https%3A%2F%2Fwww.ycombinator.com"></a>
-<a href="https://github.com/agentops-ai/agentops/issues">
+  <a href="mailto:investor@agentops.ai"><img src="https://img.shields.io/website?color=%23f26522&down_message=Y%20Combinator&label=Not%20Backed%20By&logo=ycombinator&style=flat-square&up_message=Y%20Combinator&url=https%3A%2F%2Fwww.ycombinator.com"/>
+  <a href="https://github.com/agentops-ai/agentops/issues">
     <img src="https://img.shields.io/github/commit-activity/m/agentops-ai/agentops" alt="git commit activity" />
   </a>
+
+
+AgentOps helps developers build, evaluate, and monitor AI agents. Tools to build agents from prototype to production.
+
+
+|||
+|------------------------------------------|----------------------------------------------------|
+| 📊 **Replay Analytics and Debugging** | Step-by-step agent execution graphs |
+| 💸 **LLM Cost Management**   | Track spend with LLM foundation model providers |
+| 🧪 **Agent Benchmarking** | Test your agents against 1,000+ evals |
+| 🔐 **Compliance and Security**            | Detect common prompt injection and data exfiltration exploits |
+| 🤝 **Framework Integrations**            | Easily plugs in with frameworks like CrewAI and LangChain |
+
 ## Quick Start ⌨️
 
-```pip install agentops```
+```python
+pip install agentops
+```
 
 ### Session replays in 3 lines of code
-Initialize the AgentOps client, and automatically get analytics on every LLM call.
+Initialize the AgentOps client and automatically get analytics on every LLM call.
 
-```python python
+```python
 import agentops
 
 # Beginning of program's code (i.e. main.py, __init__.py)
 agentops.init(<INSERT YOUR API KEY HERE>)
 
 ...
 # (optional: record specific functions)
@@ -80,46 +93,52 @@
     ...
 
 # End of program
 agentops.end_session('Success')
 # Woohoo You're done 🎉
 ```
 
-Refer to our [API documentation](http://docs.agentops.ai) for detailed instructions.
+All your sessions are available on the [AgentOps dashboard](https://app.agentops.ai?ref=gh). Refer to our [API documentation](http://docs.agentops.ai) for detailed instructions.
 
-## Time travel debugging 🔮
-(coming soon!)
 
-## Agent Arena 🥊
-(coming soon!)
+<details open>
+  <summary>Agent Dashboard</summary>
+  <a href="https://app.agentops.ai?ref=gh">
+   <img src="https://github.com/AgentOps-AI/agentops/assets/14807319/158e082a-9a7d-49b7-9b41-51a49a1f7d3d" style="width: 90%;" alt="Agent Dashboard"/>
+  </a>
+</details>
 
-## Evaluations Roadmap 🧭
+<details>
+  <summary>Session Analytics</summary>
+  <a href="https://app.agentops.ai?ref=gh">
+    <img src="https://github.com/AgentOps-AI/agentops/assets/14807319/d7228019-1488-40d3-852f-a61e998658ad" style="width: 90%;" alt="Session Analytics"/>
+  </a>
+</details>
 
-| Platform | Dashboard | Evals |
-|---|---|---|
-|✅ Python SDK | ✅ Multi-session and Cross-session metrics | ✅ Custom eval metrics |
-|🚧 Evaluation builder API | ✅ Custom event tag tracking | 🔜 Agent scorecards |
-|✅ [Javascript/Typescript SDK](https://github.com/AgentOps-AI/agentops-node) | ✅ Session replays| 🔜 Evaluation playground + leaderboard|
+<details>
+  <summary>Session Replays</summary>
+  <a href="https://app.agentops.ai?ref=gh">
+    <img src="https://github.com/AgentOps-AI/agentops/assets/14807319/561d59f3-c441-4066-914b-f6cfe32a598c" style="width: 90%;" alt="Session Replays"/>
+  </a>
+</details>
 
+## Integrations 🦾
 
-## Debugging Roadmap 🧭
+### CrewAI 🛶
 
-| Performance testing | Environments | LLM Testing | Reasoning and execution testing |
-|---|---|---|---|
-|✅ Event latency analysis | 🔜 Non-stationary environment testing | 🔜 LLM non-deterministic function detection | 🚧 Infinite loops and recursive thought detection |
-|✅ Agent workflow execution pricing | 🔜 Multi-modal environments | 🚧 Token limit overflow flags | 🔜 Faulty reasoning detection |
-|🚧 Success validators (external) | 🔜 Execution containers | 🔜 Context limit overflow flags | 🔜 Generative code validators |
-|🔜 Agent controllers/skill tests | ✅ Honeypot and prompt injection detection ([PromptArmor](https://promptarmor.com)) | 🔜 API bill tracking | 🔜 Error breakpoint analysis |
-|🔜 Information context constraint testing | 🔜 Anti-agent roadblocks (i.e. Captchas) | 🔜 CI/CD integration checks | |
-|🔜 Regression testing | 🔜 Multi-agent framework visualization | | |
+Build Crew agents with observability with only 2 lines of code. Simply set an `AGENTOPS_API_KEY` in your environment, and your crews will get automatic monitoring on the AgentOps dashboard.
+
+AgentOps is officially supported on Crew's latest rc branch: `crewai==0.28.9rc1`
+
+* [AgentOps integration example](https://docs.agentops.ai/v1/integrations/crewai)
+* [Offical CrewAI documentation](https://docs.crewai.com/how-to/AgentOps-Observability)
 
-## Callback handlers ↩️
 
-### Langchain
-AgentOps works seemlessly with applications built using Langchain. To use the handler, install Langchain as an optional dependency:
+### Langchain 🦜🔗
+AgentOps works seamlessly with applications built using Langchain. To use the handler, install Langchain as an optional dependency:
 ```shell
 pip install agentops[langchain]
 ```
 
 To use the handler, import and set
 
 ```python
@@ -141,18 +160,45 @@
                          verbose=True,
                          callbacks=[handler], # You must pass in a callback handler to record your agent
                          handle_parsing_errors=True)
 ```
 
 Check out the [Langchain Examples Notebook](./examples/langchain_examples.ipynb) for more details including Async handlers.
 
-### LlamaIndex 
+### LlamaIndex 🦙
 (Coming Soon)
 
 
+
+## Time travel debugging 🔮
+(coming soon!)
+
+## Agent Arena 🥊
+(coming soon!)
+
+## Evaluations Roadmap 🧭
+
+| Platform | Dashboard | Evals |
+|---|---|---|
+|✅ Python SDK | ✅ Multi-session and Cross-session metrics | ✅ Custom eval metrics |
+|🚧 Evaluation builder API | ✅ Custom event tag tracking | 🔜 Agent scorecards |
+|✅ [Javascript/Typescript SDK](https://github.com/AgentOps-AI/agentops-node) | ✅ Session replays| 🔜 Evaluation playground + leaderboard|
+
+
+## Debugging Roadmap 🧭
+
+| Performance testing | Environments | LLM Testing | Reasoning and execution testing |
+|---|---|---|---|
+|✅ Event latency analysis | 🔜 Non-stationary environment testing | 🔜 LLM non-deterministic function detection | 🚧 Infinite loops and recursive thought detection |
+|✅ Agent workflow execution pricing | 🔜 Multi-modal environments | 🚧 Token limit overflow flags | 🔜 Faulty reasoning detection |
+|🚧 Success validators (external) | 🔜 Execution containers | 🔜 Context limit overflow flags | 🔜 Generative code validators |
+|🔜 Agent controllers/skill tests | ✅ Honeypot and prompt injection detection ([PromptArmor](https://promptarmor.com)) | 🔜 API bill tracking | 🔜 Error breakpoint analysis |
+|🔜 Information context constraint testing | 🔜 Anti-agent roadblocks (i.e. Captchas) | 🔜 CI/CD integration checks | |
+|🔜 Regression testing | 🔜 Multi-agent framework visualization | | |
+
 ### Why AgentOps? 🤔
 
-Our mission is to bring your agent from protype to production.
+Our mission is to bring your agent from prototype to production.
 
 Agent developers often work with little to no visibility into agent testing performance. This means their agents never leave the lab. We're changing that. 
 
 AgentOps is the easiest way to evaluate, grade, and test agents. Is there a feature you'd like to see AgentOps cover? Just raise it in the issues tab, and we'll work on adding it to the roadmap.
```

#### html2text {}

```diff
@@ -1,75 +1,89 @@
-Metadata-Version: 2.1 Name: agentops Version: 0.1.6 Summary: Python SDK for
+Metadata-Version: 2.1 Name: agentops Version: 0.1.7 Summary: Python SDK for
 developing AI agent evals and observability Author-email: Alex Reibman
 gmail.com>, Shawn Qiu
 gmail.com>, Braelyn Boynton
 gmail.com>, Howard Gil
 gmail.com> Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
 Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
-License Classifier: Operating System :: OS Independent Requires-Python: >=3.7
+License Classifier: Operating System :: OS Independent Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 requests==2.31.0 Requires-Dist: psutil==5.9.8 Requires-Dist: packaging==23.2
 Provides-Extra: dev Requires-Dist: pytest==7.4.0; extra == "dev" Requires-Dist:
 requests_mock==1.11.0; extra == "dev" Provides-Extra: langchain Requires-Dist:
 langchain>=0.0.354; extra == "langchain"
-                                    [Logo]
+                                    _[_L_o_g_o_]
                      AAII aaggeennttss ssuucckk.. WWee?â??rree ffiixxiinngg tthhaatt..
                                _[_P_y_t_h_o_n_]_[_V_e_r_s_i_o_n_]
     _ð___¦_ _T_w_i_t_t_e_r   â¢   _ð___¢_ _D_i_s_c_o_r_d   â¢   _ð____ï_¸__ _A_g_e_n_t_O_p_s   â¢   _ð___
                                  _D_o_c_u_m_e_n_t_a_t_i_o_n
-# AgentOps Build your next agent with benchmarks, observability, and replay
-analytics. AgentOps is the toolkit for evaluating and developing robust and
-reliable AI agents. You can sign up for AgentOps [here](https://
-app.agentops.ai). [![License: MIT](https://img.shields.io/badge/License-MIT-
+# AgentOps ðï¸ [![License: MIT](https://img.shields.io/badge/License-MIT-
 yellow.svg)](https://opensource.org/licenses/MIT) ![PyPI - Version](https://
 img.shields.io/pypi/v/agentops) _[_h_t_t_p_s_:_/_/_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_a_g_e_n_t_o_p_s_/_m_o_n_t_h_]
 _[_A_g_e_n_t_O_p_s_ _T_w_i_t_t_e_r_]_[_D_i_s_c_o_r_d_ _c_o_m_m_u_n_i_t_y_ _c_h_a_n_n_e_l_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _w_e_b_s_i_t_e_?_c_o_l_o_r_=_%_2_3_f_2_6_5_2_2_&_d_o_w_n___m_e_s_s_a_g_e_=_Y_%_2_0_C_o_m_b_i_n_a_t_o_r_&_l_a_b_e_l_=_N_o_t_%_2_0_B_a_c_k_e_d_%_2_0_B_y_&_l_o_g_o_=_y_c_o_m_b_i_n_a_t_o_r_&_s_t_y_l_e_=_f_l_a_t_-
 _s_q_u_a_r_e_&_u_p___m_e_s_s_a_g_e_=_Y_%_2_0_C_o_m_b_i_n_a_t_o_r_&_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_w_w_w_._y_c_o_m_b_i_n_a_t_o_r_._c_o_m_]_[_g_i_t
-_c_o_m_m_i_t_ _a_c_t_i_v_i_t_y_]_#_#_ _Q_u_i_c_k_ _S_t_a_r_t_ _â__¨_ï_¸__ _`_`_`_p_i_p_ _i_n_s_t_a_l_l_ _a_g_e_n_t_o_p_s_`_`_`_ _#_#_#_ _S_e_s_s_i_o_n
-_r_e_p_l_a_y_s_ _i_n_ _3_ _l_i_n_e_s_ _o_f_ _c_o_d_e_ _I_n_i_t_i_a_l_i_z_e_ _t_h_e_ _A_g_e_n_t_O_p_s_ _c_l_i_e_n_t_,_ _a_n_d_ _a_u_t_o_m_a_t_i_c_a_l_l_y
-_g_e_t_ _a_n_a_l_y_t_i_c_s_ _o_n_ _e_v_e_r_y_ _L_L_M_ _c_a_l_l_._ _`_`_`_p_y_t_h_o_n_ _p_y_t_h_o_n_ _i_m_p_o_r_t_ _a_g_e_n_t_o_p_s_ _#_ _B_e_g_i_n_n_i_n_g
-_o_f_ _p_r_o_g_r_a_m_'_s_ _c_o_d_e_ _(_i_._e_._ _m_a_i_n_._p_y_,_ _____i_n_i_t_____._p_y_)_ _a_g_e_n_t_o_p_s_._i_n_i_t_(_)_ _._._._ _#_ _(_o_p_t_i_o_n_a_l_:
-_r_e_c_o_r_d_ _s_p_e_c_i_f_i_c_ _f_u_n_c_t_i_o_n_s_)_ _@_a_g_e_n_t_o_p_s_._r_e_c_o_r_d___f_u_n_c_t_i_o_n_(_'_s_a_m_p_l_e_ _f_u_n_c_t_i_o_n_ _b_e_i_n_g
-_r_e_c_o_r_d_'_)_ _d_e_f_ _s_a_m_p_l_e___f_u_n_c_t_i_o_n_(_._._._)_:_ _._._._ _#_ _E_n_d_ _o_f_ _p_r_o_g_r_a_m_ _a_g_e_n_t_o_p_s_._e_n_d___s_e_s_s_i_o_n
-_(_'_S_u_c_c_e_s_s_'_)_ _#_ _W_o_o_h_o_o_ _Y_o_u_'_r_e_ _d_o_n_e_ _ð____ _`_`_`_ _R_e_f_e_r_ _t_o_ _o_u_r_ _[_A_P_I_ _d_o_c_u_m_e_n_t_a_t_i_o_n_]
-_(_h_t_t_p_:_/_/_d_o_c_s_._a_g_e_n_t_o_p_s_._a_i_)_ _f_o_r_ _d_e_t_a_i_l_e_d_ _i_n_s_t_r_u_c_t_i_o_n_s_._ _#_#_ _T_i_m_e_ _t_r_a_v_e_l_ _d_e_b_u_g_g_i_n_g
-_ð___®_ _(_c_o_m_i_n_g_ _s_o_o_n_!_)_ _#_#_ _A_g_e_n_t_ _A_r_e_n_a_ _ð__¥__ _(_c_o_m_i_n_g_ _s_o_o_n_!_)_ _#_#_ _E_v_a_l_u_a_t_i_o_n_s_ _R_o_a_d_m_a_p
-_ð__§_­_ _|_ _P_l_a_t_f_o_r_m_ _|_ _D_a_s_h_b_o_a_r_d_ _|_ _E_v_a_l_s_ _|_ _|_-_-_-_|_-_-_-_|_-_-_-_|_ _|_â___ _P_y_t_h_o_n_ _S_D_K_ _|_ _â__
-_M_u_l_t_i_-_s_e_s_s_i_o_n_ _a_n_d_ _C_r_o_s_s_-_s_e_s_s_i_o_n_ _m_e_t_r_i_c_s_ _|_ _â___ _C_u_s_t_o_m_ _e_v_a_l_ _m_e_t_r_i_c_s_ _|_ _|_ð___§
-_E_v_a_l_u_a_t_i_o_n_ _b_u_i_l_d_e_r_ _A_P_I_ _|_ _â___ _C_u_s_t_o_m_ _e_v_e_n_t_ _t_a_g_ _t_r_a_c_k_i_n_g_Â_ _|_ _ð____ _A_g_e_n_t_ _s_c_o_r_e_c_a_r_d_s
-_|_ _|_â___ _[_J_a_v_a_s_c_r_i_p_t_/_T_y_p_e_s_c_r_i_p_t_ _S_D_K_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_A_g_e_n_t_O_p_s_-_A_I_/_a_g_e_n_t_o_p_s_-
-_n_o_d_e_)_ _|_ _â___ _S_e_s_s_i_o_n_ _r_e_p_l_a_y_s_|_ _ð____ _E_v_a_l_u_a_t_i_o_n_ _p_l_a_y_g_r_o_u_n_d_ _+_ _l_e_a_d_e_r_b_o_a_r_d_|_ _#_#
-_D_e_b_u_g_g_i_n_g_ _R_o_a_d_m_a_p_ _ð__§_­_ _|_ _P_e_r_f_o_r_m_a_n_c_e_ _t_e_s_t_i_n_g_ _|_ _E_n_v_i_r_o_n_m_e_n_t_s_ _|_ _L_L_M_ _T_e_s_t_i_n_g_ _|
-_R_e_a_s_o_n_i_n_g_ _a_n_d_ _e_x_e_c_u_t_i_o_n_ _t_e_s_t_i_n_g_ _|_ _|_-_-_-_|_-_-_-_|_-_-_-_|_-_-_-_|_ _|_â___ _E_v_e_n_t_ _l_a_t_e_n_c_y_ _a_n_a_l_y_s_i_s
-_|_ _ð____ _N_o_n_-_s_t_a_t_i_o_n_a_r_y_ _e_n_v_i_r_o_n_m_e_n_t_ _t_e_s_t_i_n_g_ _|_ _ð____ _L_L_M_ _n_o_n_-_d_e_t_e_r_m_i_n_i_s_t_i_c_ _f_u_n_c_t_i_o_n
-_d_e_t_e_c_t_i_o_n_ _|_ _ð___§_ _I_n_f_i_n_i_t_e_ _l_o_o_p_s_ _a_n_d_ _r_e_c_u_r_s_i_v_e_ _t_h_o_u_g_h_t_ _d_e_t_e_c_t_i_o_n_ _|_ _|_â___ _A_g_e_n_t
-_w_o_r_k_f_l_o_w_ _e_x_e_c_u_t_i_o_n_ _p_r_i_c_i_n_g_ _|_ _ð____ _M_u_l_t_i_-_m_o_d_a_l_ _e_n_v_i_r_o_n_m_e_n_t_s_ _|_ _ð___§_ _T_o_k_e_n_ _l_i_m_i_t
-_o_v_e_r_f_l_o_w_ _f_l_a_g_s_ _|_ _ð____ _F_a_u_l_t_y_ _r_e_a_s_o_n_i_n_g_ _d_e_t_e_c_t_i_o_n_ _|_ _|_ð___§_ _S_u_c_c_e_s_s_ _v_a_l_i_d_a_t_o_r_s_ 
-_(_e_x_t_e_r_n_a_l_)_ _|_ _ð____ _E_x_e_c_u_t_i_o_n_ _c_o_n_t_a_i_n_e_r_s_ _|_ _ð____ _C_o_n_t_e_x_t_ _l_i_m_i_t_ _o_v_e_r_f_l_o_w_ _f_l_a_g_s_ _|
-_ð____ _G_e_n_e_r_a_t_i_v_e_ _c_o_d_e_ _v_a_l_i_d_a_t_o_r_s_ _|_ _|_ð____ _A_g_e_n_t_ _c_o_n_t_r_o_l_l_e_r_s_/_s_k_i_l_l_ _t_e_s_t_s_ _|_ _â__
-_H_o_n_e_y_p_o_t_ _a_n_d_ _p_r_o_m_p_t_ _i_n_j_e_c_t_i_o_n_ _d_e_t_e_c_t_i_o_n_ _(_[_P_r_o_m_p_t_A_r_m_o_r_]_(_h_t_t_p_s_:_/_/
-_p_r_o_m_p_t_a_r_m_o_r_._c_o_m_)_)_ _|_ _ð____ _A_P_I_ _b_i_l_l_ _t_r_a_c_k_i_n_g_ _|_ _ð____ _E_r_r_o_r_ _b_r_e_a_k_p_o_i_n_t_ _a_n_a_l_y_s_i_s_ _|
-_|_ð____ _I_n_f_o_r_m_a_t_i_o_n_ _c_o_n_t_e_x_t_ _c_o_n_s_t_r_a_i_n_t_ _t_e_s_t_i_n_g_ _|_ _ð____ _A_n_t_i_-_a_g_e_n_t_ _r_o_a_d_b_l_o_c_k_s_ _(_i_._e_.
-_C_a_p_t_c_h_a_s_)_ _|_ _ð____ _C_I_/_C_D_ _i_n_t_e_g_r_a_t_i_o_n_ _c_h_e_c_k_s_ _|_ _|_ _|_ð____ _R_e_g_r_e_s_s_i_o_n_ _t_e_s_t_i_n_g_ _|_ _ð___
-_M_u_l_t_i_-_a_g_e_n_t_ _f_r_a_m_e_w_o_r_k_ _v_i_s_u_a_l_i_z_a_t_i_o_n_ _|_ _|_ _|_ _#_#_ _C_a_l_l_b_a_c_k_ _h_a_n_d_l_e_r_s_ _â__©_ï_¸__ _#_#_#
-_L_a_n_g_c_h_a_i_n_ _A_g_e_n_t_O_p_s_ _w_o_r_k_s_ _s_e_e_m_l_e_s_s_l_y_ _w_i_t_h_ _a_p_p_l_i_c_a_t_i_o_n_s_ _b_u_i_l_t_ _u_s_i_n_g_ _L_a_n_g_c_h_a_i_n_._ _T_o
-_u_s_e_ _t_h_e_ _h_a_n_d_l_e_r_,_ _i_n_s_t_a_l_l_ _L_a_n_g_c_h_a_i_n_ _a_s_ _a_n_ _o_p_t_i_o_n_a_l_ _d_e_p_e_n_d_e_n_c_y_:_ _`_`_`_s_h_e_l_l_ _p_i_p
-_i_n_s_t_a_l_l_ _a_g_e_n_t_o_p_s_[_l_a_n_g_c_h_a_i_n_]_ _`_`_`_ _T_o_ _u_s_e_ _t_h_e_ _h_a_n_d_l_e_r_,_ _i_m_p_o_r_t_ _a_n_d_ _s_e_t_ _`_`_`_p_y_t_h_o_n
-_i_m_p_o_r_t_ _o_s_ _f_r_o_m_ _l_a_n_g_c_h_a_i_n_._c_h_a_t___m_o_d_e_l_s_ _i_m_p_o_r_t_ _C_h_a_t_O_p_e_n_A_I_ _f_r_o_m_ _l_a_n_g_c_h_a_i_n_._a_g_e_n_t_s
-_i_m_p_o_r_t_ _i_n_i_t_i_a_l_i_z_e___a_g_e_n_t_,_ _A_g_e_n_t_T_y_p_e_ _f_r_o_m_ _a_g_e_n_t_o_p_s_._l_a_n_g_c_h_a_i_n___c_a_l_l_b_a_c_k___h_a_n_d_l_e_r
-_i_m_p_o_r_t_ _L_a_n_g_c_h_a_i_n_C_a_l_l_b_a_c_k_H_a_n_d_l_e_r_ _A_G_E_N_T_O_P_S___A_P_I___K_E_Y_ _=_ _o_s_._e_n_v_i_r_o_n
-_[_'_A_G_E_N_T_O_P_S___A_P_I___K_E_Y_'_]_ _h_a_n_d_l_e_r_ _=_ _L_a_n_g_c_h_a_i_n_C_a_l_l_b_a_c_k_H_a_n_d_l_e_r
-_(_a_p_i___k_e_y_=_A_G_E_N_T_O_P_S___A_P_I___K_E_Y_,_ _t_a_g_s_=_[_'_L_a_n_g_c_h_a_i_n_ _E_x_a_m_p_l_e_'_]_)_ _l_l_m_ _=_ _C_h_a_t_O_p_e_n_A_I
-_(_o_p_e_n_a_i___a_p_i___k_e_y_=_O_P_E_N_A_I___A_P_I___K_E_Y_,_ _c_a_l_l_b_a_c_k_s_=_[_h_a_n_d_l_e_r_]_,_ _m_o_d_e_l_=_'_g_p_t_-_3_._5_-_t_u_r_b_o_'_)
-_a_g_e_n_t_ _=_ _i_n_i_t_i_a_l_i_z_e___a_g_e_n_t_(_t_o_o_l_s_,_ _l_l_m_,
+_c_o_m_m_i_t_ _a_c_t_i_v_i_t_y_]_A_g_e_n_t_O_p_s_ _h_e_l_p_s_ _d_e_v_e_l_o_p_e_r_s_ _b_u_i_l_d_,_ _e_v_a_l_u_a_t_e_,_ _a_n_d_ _m_o_n_i_t_o_r_ _A_I
+_a_g_e_n_t_s_._ _T_o_o_l_s_ _t_o_ _b_u_i_l_d_ _a_g_e_n_t_s_ _f_r_o_m_ _p_r_o_t_o_t_y_p_e_ _t_o_ _p_r_o_d_u_c_t_i_o_n_._ _|_|_|_ _|_-_-_-_-_-_-_-_-_-_-_-_-_-_-
+_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_|_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-
+_-_-_|_ _|_ _ð____ _*_*_R_e_p_l_a_y_ _A_n_a_l_y_t_i_c_s_ _a_n_d_ _D_e_b_u_g_g_i_n_g_*_*_ _|_ _S_t_e_p_-_b_y_-_s_t_e_p_ _a_g_e_n_t_ _e_x_e_c_u_t_i_o_n
+_g_r_a_p_h_s_ _|_ _|_ _ð___¸_ _*_*_L_L_M_ _C_o_s_t_ _M_a_n_a_g_e_m_e_n_t_*_*_ _|_ _T_r_a_c_k_ _s_p_e_n_d_ _w_i_t_h_ _L_L_M_ _f_o_u_n_d_a_t_i_o_n_ _m_o_d_e_l
+_p_r_o_v_i_d_e_r_s_ _|_ _|_ _ð__§_ª_ _*_*_A_g_e_n_t_ _B_e_n_c_h_m_a_r_k_i_n_g_*_*_ _|_ _T_e_s_t_ _y_o_u_r_ _a_g_e_n_t_s_ _a_g_a_i_n_s_t_ _1_,_0_0_0_+
+_e_v_a_l_s_ _|_ _|_ _ð____ _*_*_C_o_m_p_l_i_a_n_c_e_ _a_n_d_ _S_e_c_u_r_i_t_y_*_*_ _|_ _D_e_t_e_c_t_ _c_o_m_m_o_n_ _p_r_o_m_p_t_ _i_n_j_e_c_t_i_o_n_ _a_n_d
+_d_a_t_a_ _e_x_f_i_l_t_r_a_t_i_o_n_ _e_x_p_l_o_i_t_s_ _|_ _|_ _ð__¤__ _*_*_F_r_a_m_e_w_o_r_k_ _I_n_t_e_g_r_a_t_i_o_n_s_*_*_ _|_ _E_a_s_i_l_y_ _p_l_u_g_s
+_i_n_ _w_i_t_h_ _f_r_a_m_e_w_o_r_k_s_ _l_i_k_e_ _C_r_e_w_A_I_ _a_n_d_ _L_a_n_g_C_h_a_i_n_ _|_ _#_#_ _Q_u_i_c_k_ _S_t_a_r_t_ _â__¨_ï_¸__ _`_`_`_p_y_t_h_o_n
+_p_i_p_ _i_n_s_t_a_l_l_ _a_g_e_n_t_o_p_s_ _`_`_`_ _#_#_#_ _S_e_s_s_i_o_n_ _r_e_p_l_a_y_s_ _i_n_ _3_ _l_i_n_e_s_ _o_f_ _c_o_d_e_ _I_n_i_t_i_a_l_i_z_e_ _t_h_e
+_A_g_e_n_t_O_p_s_ _c_l_i_e_n_t_ _a_n_d_ _a_u_t_o_m_a_t_i_c_a_l_l_y_ _g_e_t_ _a_n_a_l_y_t_i_c_s_ _o_n_ _e_v_e_r_y_ _L_L_M_ _c_a_l_l_._ _`_`_`_p_y_t_h_o_n
+_i_m_p_o_r_t_ _a_g_e_n_t_o_p_s_ _#_ _B_e_g_i_n_n_i_n_g_ _o_f_ _p_r_o_g_r_a_m_'_s_ _c_o_d_e_ _(_i_._e_._ _m_a_i_n_._p_y_,_ _____i_n_i_t_____._p_y_)
+_a_g_e_n_t_o_p_s_._i_n_i_t_(_)_ _._._._ _#_ _(_o_p_t_i_o_n_a_l_:_ _r_e_c_o_r_d_ _s_p_e_c_i_f_i_c_ _f_u_n_c_t_i_o_n_s_)
+_@_a_g_e_n_t_o_p_s_._r_e_c_o_r_d___f_u_n_c_t_i_o_n_(_'_s_a_m_p_l_e_ _f_u_n_c_t_i_o_n_ _b_e_i_n_g_ _r_e_c_o_r_d_'_)_ _d_e_f_ _s_a_m_p_l_e___f_u_n_c_t_i_o_n
+_(_._._._)_:_ _._._._ _#_ _E_n_d_ _o_f_ _p_r_o_g_r_a_m_ _a_g_e_n_t_o_p_s_._e_n_d___s_e_s_s_i_o_n_(_'_S_u_c_c_e_s_s_'_)_ _#_ _W_o_o_h_o_o_ _Y_o_u_'_r_e
+_d_o_n_e_ _ð____ _`_`_`_ _A_l_l_ _y_o_u_r_ _s_e_s_s_i_o_n_s_ _a_r_e_ _a_v_a_i_l_a_b_l_e_ _o_n_ _t_h_e_ _[_A_g_e_n_t_O_p_s_ _d_a_s_h_b_o_a_r_d_]
+_(_h_t_t_p_s_:_/_/_a_p_p_._a_g_e_n_t_o_p_s_._a_i_?_r_e_f_=_g_h_)_._ _R_e_f_e_r_ _t_o_ _o_u_r_ _[_A_P_I_ _d_o_c_u_m_e_n_t_a_t_i_o_n_]_(_h_t_t_p_:_/_/
+_d_o_c_s_._a_g_e_n_t_o_p_s_._a_i_)_ _f_o_r_ _d_e_t_a_i_l_e_d_ _i_n_s_t_r_u_c_t_i_o_n_s_._ _A_g_e_n_t_ _D_a_s_h_b_o_a_r_d_ _[_A_g_e_n_t
+_D_a_s_h_b_o_a_r_d_]_S_e_s_s_i_o_n_ _A_n_a_l_y_t_i_c_s_ _[_S_e_s_s_i_o_n_ _A_n_a_l_y_t_i_c_s_]_S_e_s_s_i_o_n_ _R_e_p_l_a_y_s_ _[_S_e_s_s_i_o_n
+_R_e_p_l_a_y_s_]_#_#_ _I_n_t_e_g_r_a_t_i_o_n_s_ _ð__¦_¾_ _#_#_#_ _C_r_e_w_A_I_ _ð___¶_ _B_u_i_l_d_ _C_r_e_w_ _a_g_e_n_t_s_ _w_i_t_h
+_o_b_s_e_r_v_a_b_i_l_i_t_y_ _w_i_t_h_ _o_n_l_y_ _2_ _l_i_n_e_s_ _o_f_ _c_o_d_e_._ _S_i_m_p_l_y_ _s_e_t_ _a_n_ _`_A_G_E_N_T_O_P_S___A_P_I___K_E_Y_`_ _i_n
+_y_o_u_r_ _e_n_v_i_r_o_n_m_e_n_t_,_ _a_n_d_ _y_o_u_r_ _c_r_e_w_s_ _w_i_l_l_ _g_e_t_ _a_u_t_o_m_a_t_i_c_ _m_o_n_i_t_o_r_i_n_g_ _o_n_ _t_h_e_ _A_g_e_n_t_O_p_s
+_d_a_s_h_b_o_a_r_d_._ _A_g_e_n_t_O_p_s_ _i_s_ _o_f_f_i_c_i_a_l_l_y_ _s_u_p_p_o_r_t_e_d_ _o_n_ _C_r_e_w_'_s_ _l_a_t_e_s_t_ _r_c_ _b_r_a_n_c_h_:
+_`_c_r_e_w_a_i_=_=_0_._2_8_._9_r_c_1_`_ _*_ _[_A_g_e_n_t_O_p_s_ _i_n_t_e_g_r_a_t_i_o_n_ _e_x_a_m_p_l_e_]_(_h_t_t_p_s_:_/_/_d_o_c_s_._a_g_e_n_t_o_p_s_._a_i_/
+_v_1_/_i_n_t_e_g_r_a_t_i_o_n_s_/_c_r_e_w_a_i_)_ _*_ _[_O_f_f_i_c_a_l_ _C_r_e_w_A_I_ _d_o_c_u_m_e_n_t_a_t_i_o_n_]_(_h_t_t_p_s_:_/_/
+_d_o_c_s_._c_r_e_w_a_i_._c_o_m_/_h_o_w_-_t_o_/_A_g_e_n_t_O_p_s_-_O_b_s_e_r_v_a_b_i_l_i_t_y_)_ _#_#_#_ _L_a_n_g_c_h_a_i_n_ _ð__¦__ð____ _A_g_e_n_t_O_p_s
+_w_o_r_k_s_ _s_e_a_m_l_e_s_s_l_y_ _w_i_t_h_ _a_p_p_l_i_c_a_t_i_o_n_s_ _b_u_i_l_t_ _u_s_i_n_g_ _L_a_n_g_c_h_a_i_n_._ _T_o_ _u_s_e_ _t_h_e_ _h_a_n_d_l_e_r_,
+_i_n_s_t_a_l_l_ _L_a_n_g_c_h_a_i_n_ _a_s_ _a_n_ _o_p_t_i_o_n_a_l_ _d_e_p_e_n_d_e_n_c_y_:_ _`_`_`_s_h_e_l_l_ _p_i_p_ _i_n_s_t_a_l_l_ _a_g_e_n_t_o_p_s
+_[_l_a_n_g_c_h_a_i_n_]_ _`_`_`_ _T_o_ _u_s_e_ _t_h_e_ _h_a_n_d_l_e_r_,_ _i_m_p_o_r_t_ _a_n_d_ _s_e_t_ _`_`_`_p_y_t_h_o_n_ _i_m_p_o_r_t_ _o_s_ _f_r_o_m
+_l_a_n_g_c_h_a_i_n_._c_h_a_t___m_o_d_e_l_s_ _i_m_p_o_r_t_ _C_h_a_t_O_p_e_n_A_I_ _f_r_o_m_ _l_a_n_g_c_h_a_i_n_._a_g_e_n_t_s_ _i_m_p_o_r_t
+_i_n_i_t_i_a_l_i_z_e___a_g_e_n_t_,_ _A_g_e_n_t_T_y_p_e_ _f_r_o_m_ _a_g_e_n_t_o_p_s_._l_a_n_g_c_h_a_i_n___c_a_l_l_b_a_c_k___h_a_n_d_l_e_r_ _i_m_p_o_r_t
+_L_a_n_g_c_h_a_i_n_C_a_l_l_b_a_c_k_H_a_n_d_l_e_r_ _A_G_E_N_T_O_P_S___A_P_I___K_E_Y_ _=_ _o_s_._e_n_v_i_r_o_n_[_'_A_G_E_N_T_O_P_S___A_P_I___K_E_Y_'_]
+_h_a_n_d_l_e_r_ _=_ _L_a_n_g_c_h_a_i_n_C_a_l_l_b_a_c_k_H_a_n_d_l_e_r_(_a_p_i___k_e_y_=_A_G_E_N_T_O_P_S___A_P_I___K_E_Y_,_ _t_a_g_s_=_[_'_L_a_n_g_c_h_a_i_n
+_E_x_a_m_p_l_e_'_]_)_ _l_l_m_ _=_ _C_h_a_t_O_p_e_n_A_I_(_o_p_e_n_a_i___a_p_i___k_e_y_=_O_P_E_N_A_I___A_P_I___K_E_Y_,_ _c_a_l_l_b_a_c_k_s_=_[_h_a_n_d_l_e_r_]_,
+_m_o_d_e_l_=_'_g_p_t_-_3_._5_-_t_u_r_b_o_'_)_ _a_g_e_n_t_ _=_ _i_n_i_t_i_a_l_i_z_e___a_g_e_n_t_(_t_o_o_l_s_,_ _l_l_m_,
 _a_g_e_n_t_=_A_g_e_n_t_T_y_p_e_._C_H_A_T___Z_E_R_O___S_H_O_T___R_E_A_C_T___D_E_S_C_R_I_P_T_I_O_N_,_ _v_e_r_b_o_s_e_=_T_r_u_e_,_ _c_a_l_l_b_a_c_k_s_=
 _[_h_a_n_d_l_e_r_]_,_ _#_ _Y_o_u_ _m_u_s_t_ _p_a_s_s_ _i_n_ _a_ _c_a_l_l_b_a_c_k_ _h_a_n_d_l_e_r_ _t_o_ _r_e_c_o_r_d_ _y_o_u_r_ _a_g_e_n_t
 _h_a_n_d_l_e___p_a_r_s_i_n_g___e_r_r_o_r_s_=_T_r_u_e_)_ _`_`_`_ _C_h_e_c_k_ _o_u_t_ _t_h_e_ _[_L_a_n_g_c_h_a_i_n_ _E_x_a_m_p_l_e_s_ _N_o_t_e_b_o_o_k_]_(_._/
 _e_x_a_m_p_l_e_s_/_l_a_n_g_c_h_a_i_n___e_x_a_m_p_l_e_s_._i_p_y_n_b_)_ _f_o_r_ _m_o_r_e_ _d_e_t_a_i_l_s_ _i_n_c_l_u_d_i_n_g_ _A_s_y_n_c_ _h_a_n_d_l_e_r_s_.
-_#_#_#_ _L_l_a_m_a_I_n_d_e_x_ _(_C_o_m_i_n_g_ _S_o_o_n_)_ _#_#_#_ _W_h_y_ _A_g_e_n_t_O_p_s_?_ _ð__¤__ _O_u_r_ _m_i_s_s_i_o_n_ _i_s_ _t_o_ _b_r_i_n_g
-_y_o_u_r_ _a_g_e_n_t_ _f_r_o_m_ _p_r_o_t_y_p_e_ _t_o_ _p_r_o_d_u_c_t_i_o_n_._ _A_g_e_n_t_ _d_e_v_e_l_o_p_e_r_s_ _o_f_t_e_n_ _w_o_r_k_ _w_i_t_h_ _l_i_t_t_l_e
-_t_o_ _n_o_ _v_i_s_i_b_i_l_i_t_y_ _i_n_t_o_ _a_g_e_n_t_ _t_e_s_t_i_n_g_ _p_e_r_f_o_r_m_a_n_c_e_._ _T_h_i_s_ _m_e_a_n_s_ _t_h_e_i_r_ _a_g_e_n_t_s_ _n_e_v_e_r
-_l_e_a_v_e_ _t_h_e_ _l_a_b_._ _W_e_'_r_e_ _c_h_a_n_g_i_n_g_ _t_h_a_t_._ _A_g_e_n_t_O_p_s_ _i_s_ _t_h_e_ _e_a_s_i_e_s_t_ _w_a_y_ _t_o_ _e_v_a_l_u_a_t_e_,
-_g_r_a_d_e_,_ _a_n_d_ _t_e_s_t_ _a_g_e_n_t_s_._ _I_s_ _t_h_e_r_e_ _a_ _f_e_a_t_u_r_e_ _y_o_u_'_d_ _l_i_k_e_ _t_o_ _s_e_e_ _A_g_e_n_t_O_p_s_ _c_o_v_e_r_?
-_J_u_s_t_ _r_a_i_s_e_ _i_t_ _i_n_ _t_h_e_ _i_s_s_u_e_s_ _t_a_b_,_ _a_n_d_ _w_e_'_l_l_ _w_o_r_k_ _o_n_ _a_d_d_i_n_g_ _i_t_ _t_o_ _t_h_e_ _r_o_a_d_m_a_p_.
+_#_#_#_ _L_l_a_m_a_I_n_d_e_x_ _ð__¦__ _(_C_o_m_i_n_g_ _S_o_o_n_)_ _#_#_ _T_i_m_e_ _t_r_a_v_e_l_ _d_e_b_u_g_g_i_n_g_ _ð___®_ _(_c_o_m_i_n_g_ _s_o_o_n_!_)
+_#_#_ _A_g_e_n_t_ _A_r_e_n_a_ _ð__¥__ _(_c_o_m_i_n_g_ _s_o_o_n_!_)_ _#_#_ _E_v_a_l_u_a_t_i_o_n_s_ _R_o_a_d_m_a_p_ _ð__§_­_ _|_ _P_l_a_t_f_o_r_m_ _|
+_D_a_s_h_b_o_a_r_d_ _|_ _E_v_a_l_s_ _|_ _|_-_-_-_|_-_-_-_|_-_-_-_|_ _|_â___ _P_y_t_h_o_n_ _S_D_K_ _|_ _â___ _M_u_l_t_i_-_s_e_s_s_i_o_n_ _a_n_d
+_C_r_o_s_s_-_s_e_s_s_i_o_n_ _m_e_t_r_i_c_s_ _|_ _â___ _C_u_s_t_o_m_ _e_v_a_l_ _m_e_t_r_i_c_s_ _|_ _|_ð___§_ _E_v_a_l_u_a_t_i_o_n_ _b_u_i_l_d_e_r_ _A_P_I
+_|_ _â___ _C_u_s_t_o_m_ _e_v_e_n_t_ _t_a_g_ _t_r_a_c_k_i_n_g_Â_ _|_ _ð____ _A_g_e_n_t_ _s_c_o_r_e_c_a_r_d_s_ _|_ _|_â___ _[_J_a_v_a_s_c_r_i_p_t_/
+_T_y_p_e_s_c_r_i_p_t_ _S_D_K_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_A_g_e_n_t_O_p_s_-_A_I_/_a_g_e_n_t_o_p_s_-_n_o_d_e_)_ _|_ _â___ _S_e_s_s_i_o_n
+_r_e_p_l_a_y_s_|_ _ð____ _E_v_a_l_u_a_t_i_o_n_ _p_l_a_y_g_r_o_u_n_d_ _+_ _l_e_a_d_e_r_b_o_a_r_d_|_ _#_#_ _D_e_b_u_g_g_i_n_g_ _R_o_a_d_m_a_p_ _ð__§_­_ _|
+_P_e_r_f_o_r_m_a_n_c_e_ _t_e_s_t_i_n_g_ _|_ _E_n_v_i_r_o_n_m_e_n_t_s_ _|_ _L_L_M_ _T_e_s_t_i_n_g_ _|_ _R_e_a_s_o_n_i_n_g_ _a_n_d_ _e_x_e_c_u_t_i_o_n
+_t_e_s_t_i_n_g_ _|_ _|_-_-_-_|_-_-_-_|_-_-_-_|_-_-_-_|_ _|_â___ _E_v_e_n_t_ _l_a_t_e_n_c_y_ _a_n_a_l_y_s_i_s_ _|_ _ð____ _N_o_n_-_s_t_a_t_i_o_n_a_r_y
+_e_n_v_i_r_o_n_m_e_n_t_ _t_e_s_t_i_n_g_ _|_ _ð____ _L_L_M_ _n_o_n_-_d_e_t_e_r_m_i_n_i_s_t_i_c_ _f_u_n_c_t_i_o_n_ _d_e_t_e_c_t_i_o_n_ _|_ _ð___§
+_I_n_f_i_n_i_t_e_ _l_o_o_p_s_ _a_n_d_ _r_e_c_u_r_s_i_v_e_ _t_h_o_u_g_h_t_ _d_e_t_e_c_t_i_o_n_ _|_ _|_â___ _A_g_e_n_t_ _w_o_r_k_f_l_o_w_ _e_x_e_c_u_t_i_o_n
+_p_r_i_c_i_n_g_ _|_ _ð____ _M_u_l_t_i_-_m_o_d_a_l_ _e_n_v_i_r_o_n_m_e_n_t_s_ _|_ _ð___§_ _T_o_k_e_n_ _l_i_m_i_t_ _o_v_e_r_f_l_o_w_ _f_l_a_g_s_ _|
+_ð____ _F_a_u_l_t_y_ _r_e_a_s_o_n_i_n_g_ _d_e_t_e_c_t_i_o_n_ _|_ _|_ð___§_ _S_u_c_c_e_s_s_ _v_a_l_i_d_a_t_o_r_s_ _(_e_x_t_e_r_n_a_l_)_ _|_ _ð___
+_E_x_e_c_u_t_i_o_n_ _c_o_n_t_a_i_n_e_r_s_ _|_ _ð____ _C_o_n_t_e_x_t_ _l_i_m_i_t_ _o_v_e_r_f_l_o_w_ _f_l_a_g_s_ _|_ _ð____ _G_e_n_e_r_a_t_i_v_e_ _c_o_d_e
+_v_a_l_i_d_a_t_o_r_s_ _|_ _|_ð____ _A_g_e_n_t_ _c_o_n_t_r_o_l_l_e_r_s_/_s_k_i_l_l_ _t_e_s_t_s_ _|_ _â___ _H_o_n_e_y_p_o_t_ _a_n_d_ _p_r_o_m_p_t
+_i_n_j_e_c_t_i_o_n_ _d_e_t_e_c_t_i_o_n_ _(_[_P_r_o_m_p_t_A_r_m_o_r_]_(_h_t_t_p_s_:_/_/_p_r_o_m_p_t_a_r_m_o_r_._c_o_m_)_)_ _|_ _ð____ _A_P_I_ _b_i_l_l
+_t_r_a_c_k_i_n_g_ _|_ _ð____ _E_r_r_o_r_ _b_r_e_a_k_p_o_i_n_t_ _a_n_a_l_y_s_i_s_ _|_ _|_ð____ _I_n_f_o_r_m_a_t_i_o_n_ _c_o_n_t_e_x_t
+_c_o_n_s_t_r_a_i_n_t_ _t_e_s_t_i_n_g_ _|_ _ð____ _A_n_t_i_-_a_g_e_n_t_ _r_o_a_d_b_l_o_c_k_s_ _(_i_._e_._ _C_a_p_t_c_h_a_s_)_ _|_ _ð____ _C_I_/_C_D
+_i_n_t_e_g_r_a_t_i_o_n_ _c_h_e_c_k_s_ _|_ _|_ _|_ð____ _R_e_g_r_e_s_s_i_o_n_ _t_e_s_t_i_n_g_ _|_ _ð____ _M_u_l_t_i_-_a_g_e_n_t_ _f_r_a_m_e_w_o_r_k
+_v_i_s_u_a_l_i_z_a_t_i_o_n_ _|_ _|_ _|_ _#_#_#_ _W_h_y_ _A_g_e_n_t_O_p_s_?_ _ð__¤__ _O_u_r_ _m_i_s_s_i_o_n_ _i_s_ _t_o_ _b_r_i_n_g_ _y_o_u_r_ _a_g_e_n_t
+_f_r_o_m_ _p_r_o_t_o_t_y_p_e_ _t_o_ _p_r_o_d_u_c_t_i_o_n_._ _A_g_e_n_t_ _d_e_v_e_l_o_p_e_r_s_ _o_f_t_e_n_ _w_o_r_k_ _w_i_t_h_ _l_i_t_t_l_e_ _t_o_ _n_o
+_v_i_s_i_b_i_l_i_t_y_ _i_n_t_o_ _a_g_e_n_t_ _t_e_s_t_i_n_g_ _p_e_r_f_o_r_m_a_n_c_e_._ _T_h_i_s_ _m_e_a_n_s_ _t_h_e_i_r_ _a_g_e_n_t_s_ _n_e_v_e_r_ _l_e_a_v_e
+_t_h_e_ _l_a_b_._ _W_e_'_r_e_ _c_h_a_n_g_i_n_g_ _t_h_a_t_._ _A_g_e_n_t_O_p_s_ _i_s_ _t_h_e_ _e_a_s_i_e_s_t_ _w_a_y_ _t_o_ _e_v_a_l_u_a_t_e_,_ _g_r_a_d_e_,
+_a_n_d_ _t_e_s_t_ _a_g_e_n_t_s_._ _I_s_ _t_h_e_r_e_ _a_ _f_e_a_t_u_r_e_ _y_o_u_'_d_ _l_i_k_e_ _t_o_ _s_e_e_ _A_g_e_n_t_O_p_s_ _c_o_v_e_r_?_ _J_u_s_t
+_r_a_i_s_e_ _i_t_ _i_n_ _t_h_e_ _i_s_s_u_e_s_ _t_a_b_,_ _a_n_d_ _w_e_'_l_l_ _w_o_r_k_ _o_n_ _a_d_d_i_n_g_ _i_t_ _t_o_ _t_h_e_ _r_o_a_d_m_a_p_.
```

### Comparing `agentops-0.1.6/agentops.egg-info/SOURCES.txt` & `agentops-0.1.7/agentops.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -19,11 +19,12 @@
 agentops/worker.py
 agentops.egg-info/PKG-INFO
 agentops.egg-info/SOURCES.txt
 agentops.egg-info/dependency_links.txt
 agentops.egg-info/requires.txt
 agentops.egg-info/top_level.txt
 tests/test_canary.py
+tests/test_events.py
 tests/test_patcher.py
 tests/test_record_function.py
 tests/test_session.py
 tests/test_teardown.py
```

### Comparing `agentops-0.1.6/pyproject.toml` & `agentops-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "agentops"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   { name="Alex Reibman", email="areibman@gmail.com" },
   { name="Shawn Qiu", email="siyangqiu@gmail.com" },
   { name="Braelyn Boynton", email="bboynton97@gmail.com" },
   { name="Howard Gil", email="howardbgil@gmail.com" }
 ]
 description = "Python SDK for developing AI agent evals and observability"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "requests==2.31.0",
```

### Comparing `agentops-0.1.6/tests/test_canary.py` & `agentops-0.1.7/tests/test_canary.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.6/tests/test_patcher.py` & `agentops-0.1.7/tests/test_patcher.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.6/tests/test_record_function.py` & `agentops-0.1.7/tests/test_record_function.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.6/tests/test_session.py` & `agentops-0.1.7/tests/test_session.py`

 * *Files 16% similar despite different names*

```diff
@@ -44,14 +44,33 @@
         # We should have 3 requests (additional end session)
         assert len(mock_req.request_history) == 3
         assert mock_req.last_request.headers['X-Agentops-Auth'] == self.api_key
         request_json = mock_req.last_request.json()
         assert request_json['session']['end_state'] == end_state
         assert request_json['session']['tags'] == None
 
+    def test_add_tags(self, mock_req):
+        # Arrange
+        tags = ['GPT-4']
+        agentops.start_session(tags=tags, config=self.config)
+        agentops.add_tags(['test-tag', 'dupe-tag'])
+        agentops.add_tags(['dupe-tag'])
+
+        # Act
+        end_state = 'Success'
+        agentops.end_session(end_state)
+        time.sleep(0.15)
+
+        # Assert 3 requests, 1 for session init, 1 for event, 1 for end session
+        assert mock_req.last_request.headers['X-Agentops-Auth'] == self.api_key
+        request_json = mock_req.last_request.json()
+        assert request_json['session']['end_state'] == end_state
+        assert request_json['session']['tags'] == ['GPT-4', 'test-tag', 'dupe-tag']
+
+
     def test_tags(self, mock_req):
         # Arrange
         tags = ['GPT-4']
         agentops.start_session(tags=tags, config=self.config)
 
         # Act
         agentops.record(ActionEvent(self.event_type))
```

### Comparing `agentops-0.1.6/tests/test_teardown.py` & `agentops-0.1.7/tests/test_teardown.py`

 * *Files identical despite different names*


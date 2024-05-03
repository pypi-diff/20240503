# Comparing `tmp/qai_agent-0.5.2.2.tar.gz` & `tmp/qai_agent-0.5.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qai_agent-0.5.2.2.tar", max compression
+gzip compressed data, was "qai_agent-0.5.2.3.tar", max compression
```

## Comparing `qai_agent-0.5.2.2.tar` & `qai_agent-0.5.2.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0       13 2024-05-02 06:52:44.114033 qai_agent-0.5.2.2/README.md
--rw-r--r--   0        0        0     1922 2024-05-02 16:09:05.869587 qai_agent-0.5.2.2/pyproject.toml
--rw-r--r--   0        0        0     1227 2024-05-02 06:52:44.117744 qai_agent-0.5.2.2/src/qai/agent/__init__.py
--rw-r--r--   0        0        0    10173 2024-05-02 06:52:44.123828 qai_agent-0.5.2.2/src/qai/agent/agents/campaign/campaign.py
--rw-r--r--   0        0        0     3164 2024-05-02 06:52:44.120615 qai_agent-0.5.2.2/src/qai/agent/agents/conversation.py
--rw-r--r--   0        0        0    13254 2024-05-02 06:52:44.122385 qai_agent-0.5.2.2/src/qai/agent/agents/email.py
--rw-r--r--   0        0        0     3389 2024-05-02 06:52:44.120375 qai_agent-0.5.2.2/src/qai/agent/agents/example_agent.py
--rw-r--r--   0        0        0     3505 2024-05-02 06:52:44.118310 qai_agent-0.5.2.2/src/qai/agent/agents/find_agent.py
--rw-r--r--   0        0        0    11013 2024-05-02 06:52:44.120971 qai_agent-0.5.2.2/src/qai/agent/agents/sql_query.py
--rw-r--r--   0        0        0        0 2024-05-02 06:52:44.118819 qai_agent-0.5.2.2/src/qai/agent/agents/tools/__init__.py
--rw-r--r--   0        0        0     1399 2024-05-02 06:52:44.118768 qai_agent-0.5.2.2/src/qai/agent/agents/tools/outreach.py
--rw-r--r--   0        0        0        0 2024-05-02 06:52:44.124088 qai_agent-0.5.2.2/src/qai/agent/agents/worker/__init__.py
--rw-r--r--   0        0        0     3166 2024-05-02 06:52:44.131675 qai_agent-0.5.2.2/src/qai/agent/basic.py
--rw-r--r--   0        0        0        0 2024-05-02 06:52:44.132044 qai_agent-0.5.2.2/src/qai/agent/data/__init__.py
--rw-r--r--   0        0        0     1284 2024-05-02 06:52:44.131968 qai_agent-0.5.2.2/src/qai/agent/data/state_codes.py
--rw-r--r--   0        0        0     1322 2024-05-02 06:52:44.117542 qai_agent-0.5.2.2/src/qai/agent/llama_index/llm_program.py
--rw-r--r--   0        0        0      170 2024-05-02 06:52:44.116688 qai_agent-0.5.2.2/src/qai/agent/models.py
--rw-r--r--   0        0        0     3312 2024-05-02 06:52:44.116889 qai_agent-0.5.2.2/src/qai/agent/qaibot.py
--rw-r--r--   0        0        0     3403 2024-05-02 06:52:44.117981 qai_agent-0.5.2.2/src/qai/agent/serve.py
--rw-r--r--   0        0        0     1270 2024-05-02 06:52:44.130644 qai_agent-0.5.2.2/src/qai/agent/sessions/qai_session.py
--rw-r--r--   0        0        0        0 2024-05-02 06:52:44.115489 qai_agent-0.5.2.2/src/qai/agent/tools/__init__.py
--rw-r--r--   0        0        0      423 2024-05-02 06:52:44.115702 qai_agent-0.5.2.2/src/qai/agent/tools/types.py
--rw-r--r--   0        0        0     4497 2024-05-02 06:52:44.117132 qai_agent-0.5.2.2/src/qai/agent/tools.py
--rw-r--r--   0        0        0       56 2024-05-02 06:52:44.126120 qai_agent-0.5.2.2/src/qai/agent/utils/__init__.py
--rw-r--r--   0        0        0      397 2024-05-02 06:52:44.128007 qai_agent-0.5.2.2/src/qai/agent/utils/db_utils.py
--rw-r--r--   0        0        0     8150 2024-05-02 06:52:44.125814 qai_agent-0.5.2.2/src/qai/agent/utils/distribute.py
--rw-r--r--   0        0        0     3636 2024-05-02 06:52:44.127769 qai_agent-0.5.2.2/src/qai/agent/utils/utils.py
--rw-r--r--   0        0        0     1861 1970-01-01 00:00:00.000000 qai_agent-0.5.2.2/PKG-INFO
+-rw-r--r--   0        0        0       13 2024-05-02 06:52:44.114033 qai_agent-0.5.2.3/README.md
+-rw-r--r--   0        0        0     1922 2024-05-02 17:50:45.353244 qai_agent-0.5.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1227 2024-05-02 06:52:44.117744 qai_agent-0.5.2.3/src/qai/agent/__init__.py
+-rw-r--r--   0        0        0    10255 2024-05-02 17:49:36.927262 qai_agent-0.5.2.3/src/qai/agent/agents/campaign/campaign.py
+-rw-r--r--   0        0        0     3164 2024-05-02 06:52:44.120615 qai_agent-0.5.2.3/src/qai/agent/agents/conversation.py
+-rw-r--r--   0        0        0    13254 2024-05-02 17:42:04.131721 qai_agent-0.5.2.3/src/qai/agent/agents/email.py
+-rw-r--r--   0        0        0     3389 2024-05-02 06:52:44.120375 qai_agent-0.5.2.3/src/qai/agent/agents/example_agent.py
+-rw-r--r--   0        0        0     3505 2024-05-02 06:52:44.118310 qai_agent-0.5.2.3/src/qai/agent/agents/find_agent.py
+-rw-r--r--   0        0        0    11013 2024-05-02 06:52:44.120971 qai_agent-0.5.2.3/src/qai/agent/agents/sql_query.py
+-rw-r--r--   0        0        0        0 2024-05-02 06:52:44.118819 qai_agent-0.5.2.3/src/qai/agent/agents/tools/__init__.py
+-rw-r--r--   0        0        0     1399 2024-05-02 06:52:44.118768 qai_agent-0.5.2.3/src/qai/agent/agents/tools/outreach.py
+-rw-r--r--   0        0        0        0 2024-05-02 06:52:44.124088 qai_agent-0.5.2.3/src/qai/agent/agents/worker/__init__.py
+-rw-r--r--   0        0        0     3166 2024-05-02 06:52:44.131675 qai_agent-0.5.2.3/src/qai/agent/basic.py
+-rw-r--r--   0        0        0        0 2024-05-02 06:52:44.132044 qai_agent-0.5.2.3/src/qai/agent/data/__init__.py
+-rw-r--r--   0        0        0     1284 2024-05-02 06:52:44.131968 qai_agent-0.5.2.3/src/qai/agent/data/state_codes.py
+-rw-r--r--   0        0        0     1322 2024-05-02 06:52:44.117542 qai_agent-0.5.2.3/src/qai/agent/llama_index/llm_program.py
+-rw-r--r--   0        0        0      170 2024-05-02 06:52:44.116688 qai_agent-0.5.2.3/src/qai/agent/models.py
+-rw-r--r--   0        0        0     3312 2024-05-02 06:52:44.116889 qai_agent-0.5.2.3/src/qai/agent/qaibot.py
+-rw-r--r--   0        0        0     3403 2024-05-02 06:52:44.117981 qai_agent-0.5.2.3/src/qai/agent/serve.py
+-rw-r--r--   0        0        0     1270 2024-05-02 06:52:44.130644 qai_agent-0.5.2.3/src/qai/agent/sessions/qai_session.py
+-rw-r--r--   0        0        0        0 2024-05-02 06:52:44.115489 qai_agent-0.5.2.3/src/qai/agent/tools/__init__.py
+-rw-r--r--   0        0        0      423 2024-05-02 06:52:44.115702 qai_agent-0.5.2.3/src/qai/agent/tools/types.py
+-rw-r--r--   0        0        0     4497 2024-05-02 06:52:44.117132 qai_agent-0.5.2.3/src/qai/agent/tools.py
+-rw-r--r--   0        0        0       56 2024-05-02 06:52:44.126120 qai_agent-0.5.2.3/src/qai/agent/utils/__init__.py
+-rw-r--r--   0        0        0      397 2024-05-02 06:52:44.128007 qai_agent-0.5.2.3/src/qai/agent/utils/db_utils.py
+-rw-r--r--   0        0        0     8150 2024-05-02 17:32:18.845999 qai_agent-0.5.2.3/src/qai/agent/utils/distribute.py
+-rw-r--r--   0        0        0     3636 2024-05-02 06:52:44.127769 qai_agent-0.5.2.3/src/qai/agent/utils/utils.py
+-rw-r--r--   0        0        0     1861 1970-01-01 00:00:00.000000 qai_agent-0.5.2.3/PKG-INFO
```

### Comparing `qai_agent-0.5.2.2/pyproject.toml` & `qai_agent-0.5.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.poetry]
 authors = ["parnell <152523161+leeparnell@users.noreply.github.com>"]
 description = "Qai Agents for the Qai AI Platform"
 name = "qai-agent"
 packages = [{from = "src", include = "qai"}]
 readme = "README.md"
-version = "0.5.2.2"
+version = "0.5.2.3"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
 install = "^1.3.5"
 llama-index-agent-openai = "^0.2.3"
 llama-index-core = "^0.10.30"
 llama-index-embeddings-huggingface = "^0.2.0"
```

### Comparing `qai_agent-0.5.2.2/src/qai/agent/__init__.py` & `qai_agent-0.5.2.3/src/qai/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.2/src/qai/agent/agents/campaign/campaign.py` & `qai_agent-0.5.2.3/src/qai/agent/agents/campaign/campaign.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,15 @@
         return "Campaign is starting to be created, it can be found in the campaign tab."
 
 
 @dataclass
 class CampaignResponse(AgentChatResponse):
     completed: bool = False
     emails: List[EmailModel] = None
+    sequence_id: str = None
 
 
 class CampaignAgent(OpenAIAgent):
     """
     An agent that generates a campaign for a list of people and companies.
     """
 
@@ -193,17 +194,18 @@
                 assistant_message += "\n    People"
             ## Purposefully not using companies as we don't really need them
             if not noutreach:
                 assistant_message += "\n    Outreach types"
         message += assistant_message
         response: AgentChatResponse = super().chat(message, chat_history, tool_choice)
         completed = response.sources and response.sources[0].tool_name == "create_campaign"
-        setattr(response, "completed", completed)
         emails = None
         sequence_id = str(uuid.uuid4())
+        setattr(response, "completed", completed)
+        setattr(response, "sequence_id", sequence_id)
 
         if completed:
             emails = self.email_agent.create_emails(
                 sequence_id, self.from_person, self.from_company, self.people, self.companies
             )
         setattr(response, "emails", emails)
         print(f"campaignagent::Chat completed={completed}  response: {response} emails: {emails}")
```

### Comparing `qai_agent-0.5.2.2/src/qai/agent/agents/conversation.py` & `qai_agent-0.5.2.3/src/qai/agent/agents/conversation.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.2/src/qai/agent/agents/email.py` & `qai_agent-0.5.2.3/src/qai/agent/agents/email.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.2/src/qai/agent/agents/example_agent.py` & `qai_agent-0.5.2.3/src/qai/agent/agents/example_agent.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.2/src/qai/agent/agents/find_agent.py` & `qai_agent-0.5.2.3/src/qai/agent/agents/find_agent.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.2/src/qai/agent/agents/sql_query.py` & `qai_agent-0.5.2.3/src/qai/agent/agents/sql_query.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.2/src/qai/agent/agents/tools/outreach.py` & `qai_agent-0.5.2.3/src/qai/agent/agents/tools/outreach.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.2/src/qai/agent/basic.py` & `qai_agent-0.5.2.3/src/qai/agent/basic.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.2/src/qai/agent/data/state_codes.py` & `qai_agent-0.5.2.3/src/qai/agent/data/state_codes.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.2/src/qai/agent/llama_index/llm_program.py` & `qai_agent-0.5.2.3/src/qai/agent/llama_index/llm_program.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.2/src/qai/agent/qaibot.py` & `qai_agent-0.5.2.3/src/qai/agent/qaibot.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.2/src/qai/agent/serve.py` & `qai_agent-0.5.2.3/src/qai/agent/serve.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.2/src/qai/agent/sessions/qai_session.py` & `qai_agent-0.5.2.3/src/qai/agent/sessions/qai_session.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.2/src/qai/agent/tools.py` & `qai_agent-0.5.2.3/src/qai/agent/tools.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.2/src/qai/agent/utils/distribute.py` & `qai_agent-0.5.2.3/src/qai/agent/utils/distribute.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.2/src/qai/agent/utils/utils.py` & `qai_agent-0.5.2.3/src/qai/agent/utils/utils.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.2/PKG-INFO` & `qai_agent-0.5.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qai-agent
-Version: 0.5.2.2
+Version: 0.5.2.3
 Summary: Qai Agents for the Qai AI Platform
 Author: parnell
 Author-email: 152523161+leeparnell@users.noreply.github.com
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: install (>=1.3.5,<2.0.0)
```


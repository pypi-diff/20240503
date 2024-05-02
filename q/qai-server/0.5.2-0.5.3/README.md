# Comparing `tmp/qai_server-0.5.2.tar.gz` & `tmp/qai_server-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qai_server-0.5.2.tar", max compression
+gzip compressed data, was "qai_server-0.5.3.tar", max compression
```

## Comparing `qai_server-0.5.2.tar` & `qai_server-0.5.3.tar`

### file list

```diff
@@ -1,10 +1,13 @@
--rw-r--r--   0        0        0       17 2024-04-19 20:20:41.923099 qai_server-0.5.2/README.md
--rw-r--r--   0        0        0     1181 2024-05-02 06:17:30.435562 qai_server-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     1168 2024-04-30 20:35:10.418212 qai_server-0.5.2/src/qai/server/__init__.py
--rw-r--r--   0        0        0      159 2024-04-19 22:02:46.638364 qai_server-0.5.2/src/qai/server/config.py
--rw-r--r--   0        0        0     2249 2024-04-29 04:11:00.509739 qai_server-0.5.2/src/qai/server/mock_responses.py
--rw-r--r--   0        0        0     3064 2024-05-01 03:39:19.096752 qai_server-0.5.2/src/qai/server/models.py
--rw-r--r--   0        0        0     5876 2024-05-01 03:45:06.872714 qai_server-0.5.2/src/qai/server/serve.py
--rw-r--r--   0        0        0        0 2024-04-19 21:43:15.360059 qai_server-0.5.2/src/qai/server/tools/__init__.py
--rw-r--r--   0        0        0     2870 2024-04-30 19:58:26.080497 qai_server-0.5.2/src/qai/server/tools/security.py
--rw-r--r--   0        0        0     1055 1970-01-01 00:00:00.000000 qai_server-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1449 2024-05-02 21:57:55.615342 qai_server-0.5.3/README.md
+-rw-r--r--   0        0        0     1217 2024-05-02 21:59:55.785558 qai_server-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     1168 2024-05-02 06:52:44.104059 qai_server-0.5.3/src/qai/server/__init__.py
+-rw-r--r--   0        0        0       60 2024-05-02 21:39:36.863227 qai_server-0.5.3/src/qai/server/config.py
+-rw-r--r--   0        0        0       46 2024-05-02 21:15:14.308413 qai_server-0.5.3/src/qai/server/mock/__init__.py
+-rw-r--r--   0        0        0      769 2024-05-02 21:40:51.512429 qai_server-0.5.3/src/qai/server/mock/mock_functions.py
+-rw-r--r--   0        0        0     2249 2024-05-02 20:49:56.058745 qai_server-0.5.3/src/qai/server/mock/mock_responses.py
+-rw-r--r--   0        0        0      781 2024-05-02 21:26:23.357307 qai_server-0.5.3/src/qai/server/mock/mockable.py
+-rw-r--r--   0        0        0     3064 2024-05-02 06:52:44.103836 qai_server-0.5.3/src/qai/server/models.py
+-rw-r--r--   0        0        0     5050 2024-05-02 21:47:47.687832 qai_server-0.5.3/src/qai/server/serve.py
+-rw-r--r--   0        0        0        0 2024-05-02 06:52:44.102448 qai_server-0.5.3/src/qai/server/tools/__init__.py
+-rw-r--r--   0        0        0     2285 2024-05-02 21:43:22.021661 qai_server-0.5.3/src/qai/server/tools/security.py
+-rw-r--r--   0        0        0     2546 1970-01-01 00:00:00.000000 qai_server-0.5.3/PKG-INFO
```

### Comparing `qai_server-0.5.2/pyproject.toml` & `qai_server-0.5.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -4,27 +4,28 @@
 
 [tool.poetry]
 authors = ["parnell <152523161+leeparnell@users.noreply.github.com>"]
 description = ""
 name = "qai-server"
 packages = [{from = "src", include = "qai"}]
 readme = "README.md"
-version = "0.5.2"
+version = "0.5.3"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
 beautifulsoup4 = "^4.12.2"
 dataclasses-json = "^0.6.4"
 flask = "^3.0.3"
 flask-pydantic = "^0.12.0"
 ftfy = "^6.1.1"
 gunicorn = "^22.0.0"
 html2text = "^2020.1.16"
 llama-index = "^0.10.33"
-qai-agent = "^0.5.0"
+mysql-connector-python = "^8.4.0"
+qai-agent = "^0.5.2.3"
 qai-chat = "^0.5.1"
 torch = [
   {markers = "sys_platform == 'darwin' and platform_machine == 'arm64'", source = "pypi", version = "^2.3.0"},
   {platform = "darwin", source = "pypi", version = "^2.3.0"},
   {platform = "linux", source = "pytorch-cpu-src", version = "=2.3.0+cpu"},
   {platform = "win32", source = "pytorch-cpu-src", version = "=2.3.0+cpu"}
 ]
```

### Comparing `qai_server-0.5.2/src/qai/server/__init__.py` & `qai_server-0.5.3/src/qai/server/__init__.py`

 * *Files identical despite different names*

### Comparing `qai_server-0.5.2/src/qai/server/mock_responses.py` & `qai_server-0.5.3/src/qai/server/mock/mock_responses.py`

 * *Files identical despite different names*

### Comparing `qai_server-0.5.2/src/qai/server/models.py` & `qai_server-0.5.3/src/qai/server/models.py`

 * *Files identical despite different names*

### Comparing `qai_server-0.5.2/src/qai/server/serve.py` & `qai_server-0.5.3/src/qai/server/serve.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 import uuid
 from pprint import pformat
 
 from flask import jsonify, request
 from flask_pydantic import validate
 from pi_log import logs
-from qai.agent.agents.campaign.campaign import (
-    CampaignAgent,
-    CampaignResponse,
-    CampaignToolSpec,
-)
+from qai.agent.agents.campaign.campaign import CampaignAgent, CampaignResponse
 from qai.chat.chat import company_query
 from qai.chat.db.chroma.chroma import Chroma
 
 from qai.server import VERSION, create_app
 from qai.server.config import cfg
+from qai.server.mock import mockable
 from qai.server.models import CampaignInputModel, CompanyChatbotModel
 
-app = create_app(cfg)  ## app should be created before importing other modules
+## app should be created before importing other modules that require cfg
+app = create_app(cfg) 
 
-from qai.server.tools.security import requires, token_required
+from qai.server.tools.security import token_required
 
 log = logs.getLogger(__name__)
 logs.set_app_level("debug")
 default_not_found_message = "Sorry, I don't know the answer to that question."
 
 chat_session = {}
 
@@ -31,22 +29,19 @@
 def heartbeat():
     log.debug(f"serve::heartbeat")
     return jsonify({"status": "OK"}), 200
 
 
 @app.route("/set_config", methods=["GET", "POST"])
 @token_required
-@requires(["key", "value"])
-def set_config():
+def set_config(key: str, value: str):
     """
     Set a configuration value
     """
     in_data = request.get_json()
-    key = in_data.get("key")
-    value = in_data.get("value")
     log.debug(f"serve::set_config, in_data={in_data}")
     old = app.cfg[key]
     app.cfg[key] = value
     return jsonify({"old": old, "new": value}), 200
 
 
 @app.route("/set_loglevel/<level>", methods=["GET", "POST"])
@@ -111,25 +106,24 @@
     }
     in_data["response"] = pformat(d)
     return jsonify(in_data), 200
 
 
 @app.route("/", methods=["GET", "POST"])
 @token_required
+@mockable(CompanyChatbotModel)
 @validate(body=CompanyChatbotModel)
 def company_chat():
     """
     Query the company chatbot
     """
     model = CompanyChatbotModel(**request.get_json())
 
-    log.debug(f"serve::query, in_data={model}")
+    log.debug(f"company_chat(), in_data={model}")
 
-    if model.mock:
-        return {"response": "Mocked Response"}, 200
     try:
         response = company_query(
             query=model.query,
             user_id=model.user_id,
             company_name=model.company_name,
             company_id=model.company_id,
             model_cfg=app.cfg.model,
@@ -138,72 +132,54 @@
     except Exception as e:
         return {"response": str(e)}, 500
     response = {"response": str(response)}
     return jsonify(response), 200
 
 
 @app.route("/campaign", methods=["GET", "POST"])
-@token_required
+@mockable(CampaignInputModel)
 @validate(body=CampaignInputModel)
+@token_required
 def campaign():
     """
     Do a campaign query
     """
     model = CampaignInputModel(**request.get_json())
-    log.debug(f"#### campaign : model={model}", flush=True)
+    log.debug(f"campaign() : model={model}")
     if not model.id:
         model.id = uuid.uuid4().hex
-    from qai.agent.basic import BasicQuery, QueryType
-
-    from qai.server.mock_responses import (
-        campaign_response,
-        company_response,
-        people_response,
-    )
 
-    if model.mock:
-        basic_query = BasicQuery()
-        result = basic_query.query(model.query)
-        if result == QueryType.campaign:
-            return jsonify(campaign_response), 200
-        elif result == QueryType.company:
-            return jsonify(company_response), 200
-        elif result == QueryType.people:
-            return jsonify(people_response), 200
-        else:
-            return jsonify(campaign_response), 200
+    agent: CampaignAgent
+    if model.user_id in chat_session:
+        agent = chat_session[model.user_id]
     else:
-        agent : CampaignAgent 
-        if model.user_id in chat_session:
-            agent = chat_session[model.user_id]
-        else:
-
-            agent = CampaignAgent.create(**model.to_params())
-            
-            # chat_session[model.user_id] = agent ### TODO
-        if model.uploaded_data:
-            ## convert list of dict to dict of dict
-            uploaded_data = {d["name"]: d for d in model.uploaded_data}
-            agent.people = uploaded_data
-        response: CampaignResponse = agent.chat(model.query)
-        js = {}
-        js["actions"] = [
-            {
-                "action": "text",
-                "response": response.response,
-            }
-        ]
-        if response.emails:
-            emails = []
-            for em in response.emails:
-
-                e_js = em.dict()
-                e_js.update(
-                    {"type": "email_sequence_draft", "sequence_id": model.id, "title": em.subject}
-                )
-                js["actions"].append(e_js)
+        agent = CampaignAgent.create(**model.to_params())
+
+    if model.uploaded_data:
+        ## convert list of dict to dict of dict
+        uploaded_data = {d["name"]: d for d in model.uploaded_data}
+        agent.people = uploaded_data
+    response: CampaignResponse = agent.chat(model.query)
+    js = {}
+    js["actions"] = [
+        {
+            "action": "text",
+            "response": response.response,
+        }
+    ]
+    if response.emails:
+        for em in response.emails:
+            e_js = em.dict()
+            e_js.update(
+                {
+                    "type": "email_sequence_draft",
+                    "sequence_id": response.sequence_id,
+                    "title": em.subject,
+                }
+            )
+            js["actions"].append(e_js)
 
-        return jsonify(js), 200
+    return jsonify(js), 200
 
 
 if __name__ == "__main__":
     app.run(host="0.0.0.0", debug=True)
```

### Comparing `qai_server-0.5.2/src/qai/server/tools/security.py` & `qai_server-0.5.3/src/qai/server/tools/security.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,63 +1,46 @@
 import functools
+from logging import getLogger
 
 from flask import current_app as app
 from flask import request
 
+log = getLogger(__name__)
+
 
 def token_required(func):
     """
     Decorator to check for a valid token
     """
+
     @functools.wraps(func)
     def decorated_function(*args, **kwargs):
         try:
             server_config = app.cfg.server
         except AttributeError:
             raise AttributeError(
                 f"Error! No server config. set server.allowed_tokens in config file."
             )
 
         try:
-            # print("### server_config.allowed_tokens", server_config, flush=True)
             allowed_tokens = set(server_config.allowed_tokens)
         except AttributeError:
             raise AttributeError(
                 f"Error! No allowed tokens in config. set server.allowed_tokens in config file. "
             )
         ## Get and remove token from request, we don't want to be printing this
         token = request.get_json().pop("token", "")
         if token not in allowed_tokens:
-            print(f"Error! Invalid token <{token}> === {allowed_tokens}", flush=True)
+            log.error(f"Error! Invalid token <{token}> === {allowed_tokens}")
             raise Exception("Error! Invalid token")
         return func(*args, **kwargs)
 
     return decorated_function
 
 
-class requires:
-    """
-    Decorator to check for required variables in the request
-    """
-    def __init__(self, vars: list[str] = []):
-        self.vars = vars
-
-    def __call__(self, func):
-        @functools.wraps(func)
-        def decorated_function(*args, **kwargs):
-
-            # for arg in self.vars:
-            #     print(f"checking for {arg}", flush=True)
-            # for k, v in kwargs.items():
-            #     print(f"checking for {k}={v}", flush=True)
-            return func(*args, **kwargs)
-
-        return decorated_function
-
-
 def check_variable_exists(variables, in_data) -> bool:
     """
     Check if a variable exists in the request
     Args:
         variables: str or list of str
         in_data: dict
     Returns:
```


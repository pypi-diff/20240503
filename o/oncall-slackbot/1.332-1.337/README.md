# Comparing `tmp/oncall-slackbot-1.332.tar.gz` & `tmp/oncall-slackbot-1.337.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oncall-slackbot-1.332.tar", last modified: Wed Feb 23 20:44:21 2022, max compression
+gzip compressed data, was "oncall-slackbot-1.337.tar", last modified: Fri May  3 01:11:19 2024, max compression
```

## Comparing `oncall-slackbot-1.332.tar` & `oncall-slackbot-1.337.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 20:44:21.277460 oncall-slackbot-1.332/
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-02-23 20:44:19.000000 oncall-slackbot-1.332/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-02-23 20:44:19.000000 oncall-slackbot-1.332/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      715 2022-02-23 20:44:21.277460 oncall-slackbot-1.332/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2754 2022-02-23 20:44:19.000000 oncall-slackbot-1.332/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 20:44:21.277460 oncall-slackbot-1.332/oncall_slackbot/
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-02-23 20:44:21.000000 oncall-slackbot-1.332/oncall_slackbot/VERSION
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-23 20:44:19.000000 oncall-slackbot-1.332/oncall_slackbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14544 2022-02-23 20:44:19.000000 oncall-slackbot-1.332/oncall_slackbot/bot.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 20:44:21.277460 oncall-slackbot-1.332/oncall_slackbot/integrations/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-23 20:44:19.000000 oncall-slackbot-1.332/oncall_slackbot/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 20:44:21.277460 oncall-slackbot-1.332/oncall_slackbot/integrations/nlp/
--rw-r--r--   0 runner    (1001) docker     (121)      657 2022-02-23 20:44:19.000000 oncall-slackbot-1.332/oncall_slackbot/integrations/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1711 2022-02-23 20:44:19.000000 oncall-slackbot-1.332/oncall_slackbot/integrations/nlp/spacy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1925 2022-02-23 20:44:19.000000 oncall-slackbot-1.332/oncall_slackbot/integrations/pagerduty.py
--rw-r--r--   0 runner    (1001) docker     (121)     1868 2022-02-23 20:44:19.000000 oncall-slackbot-1.332/oncall_slackbot/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 20:44:21.277460 oncall-slackbot-1.332/oncall_slackbot/plugins/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-23 20:44:19.000000 oncall-slackbot-1.332/oncall_slackbot/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2000 2022-02-23 20:44:19.000000 oncall-slackbot-1.332/oncall_slackbot/plugins/blocks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1413 2022-02-23 20:44:19.000000 oncall-slackbot-1.332/oncall_slackbot/plugins/hello.py
--rw-r--r--   0 runner    (1001) docker     (121)      954 2022-02-23 20:44:19.000000 oncall-slackbot-1.332/oncall_slackbot/plugins/nlp.py
--rw-r--r--   0 runner    (1001) docker     (121)     2783 2022-02-23 20:44:19.000000 oncall-slackbot-1.332/oncall_slackbot/plugins/oncall.py
--rw-r--r--   0 runner    (1001) docker     (121)     1106 2022-02-23 20:44:19.000000 oncall-slackbot-1.332/oncall_slackbot/plugins/upload.py
--rw-r--r--   0 runner    (1001) docker     (121)     2061 2022-02-23 20:44:19.000000 oncall-slackbot-1.332/oncall_slackbot/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     5943 2022-02-23 20:44:19.000000 oncall-slackbot-1.332/oncall_slackbot/slackclient.py
--rw-r--r--   0 runner    (1001) docker     (121)     1796 2022-02-23 20:44:19.000000 oncall-slackbot-1.332/oncall_slackbot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 20:44:21.277460 oncall-slackbot-1.332/oncall_slackbot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      715 2022-02-23 20:44:21.000000 oncall-slackbot-1.332/oncall_slackbot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      804 2022-02-23 20:44:21.000000 oncall-slackbot-1.332/oncall_slackbot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-23 20:44:21.000000 oncall-slackbot-1.332/oncall_slackbot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-02-23 20:44:21.000000 oncall-slackbot-1.332/oncall_slackbot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-02-23 20:44:21.000000 oncall-slackbot-1.332/oncall_slackbot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-02-23 20:44:21.281460 oncall-slackbot-1.332/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1965 2022-02-23 20:44:19.000000 oncall-slackbot-1.332/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:11:19.907071 oncall-slackbot-1.337/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-03 01:11:13.000000 oncall-slackbot-1.337/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-03 01:11:13.000000 oncall-slackbot-1.337/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-03 01:11:19.907071 oncall-slackbot-1.337/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-05-03 01:11:13.000000 oncall-slackbot-1.337/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:11:19.907071 oncall-slackbot-1.337/oncall_slackbot/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-03 01:11:18.000000 oncall-slackbot-1.337/oncall_slackbot/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:11:13.000000 oncall-slackbot-1.337/oncall_slackbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15230 2024-05-03 01:11:13.000000 oncall-slackbot-1.337/oncall_slackbot/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:11:19.907071 oncall-slackbot-1.337/oncall_slackbot/integrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:11:13.000000 oncall-slackbot-1.337/oncall_slackbot/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:11:19.907071 oncall-slackbot-1.337/oncall_slackbot/integrations/nlp/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-03 01:11:13.000000 oncall-slackbot-1.337/oncall_slackbot/integrations/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-03 01:11:13.000000 oncall-slackbot-1.337/oncall_slackbot/integrations/nlp/spacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-03 01:11:13.000000 oncall-slackbot-1.337/oncall_slackbot/integrations/pagerduty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-03 01:11:13.000000 oncall-slackbot-1.337/oncall_slackbot/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:11:19.907071 oncall-slackbot-1.337/oncall_slackbot/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:11:13.000000 oncall-slackbot-1.337/oncall_slackbot/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-03 01:11:13.000000 oncall-slackbot-1.337/oncall_slackbot/plugins/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-03 01:11:13.000000 oncall-slackbot-1.337/oncall_slackbot/plugins/hello.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-03 01:11:13.000000 oncall-slackbot-1.337/oncall_slackbot/plugins/nlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-03 01:11:13.000000 oncall-slackbot-1.337/oncall_slackbot/plugins/oncall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-03 01:11:13.000000 oncall-slackbot-1.337/oncall_slackbot/plugins/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-03 01:11:13.000000 oncall-slackbot-1.337/oncall_slackbot/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5991 2024-05-03 01:11:13.000000 oncall-slackbot-1.337/oncall_slackbot/slackclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-03 01:11:13.000000 oncall-slackbot-1.337/oncall_slackbot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:11:19.907071 oncall-slackbot-1.337/oncall_slackbot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-03 01:11:19.000000 oncall-slackbot-1.337/oncall_slackbot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-03 01:11:19.000000 oncall-slackbot-1.337/oncall_slackbot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 01:11:19.000000 oncall-slackbot-1.337/oncall_slackbot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-03 01:11:19.000000 oncall-slackbot-1.337/oncall_slackbot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-03 01:11:19.000000 oncall-slackbot-1.337/oncall_slackbot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-03 01:11:13.000000 oncall-slackbot-1.337/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-03 01:11:19.907071 oncall-slackbot-1.337/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-03 01:11:13.000000 oncall-slackbot-1.337/setup.py
```

### Comparing `oncall-slackbot-1.332/LICENSE.txt` & `oncall-slackbot-1.337/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `oncall-slackbot-1.332/PKG-INFO` & `oncall-slackbot-1.337/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: oncall-slackbot
-Version: 1.332
+Version: 1.337
 Summary: Slackbot made specifically to handle on-call requests
 Home-page: http://github.com/bluesliverx/oncall-slackbot
 Author: Brian Saville
 Author-email: bksaville@gmail.com
 License: MIT
 Description: UNKNOWN
 Platform: Any
```

### Comparing `oncall-slackbot-1.332/README.md` & `oncall-slackbot-1.337/README.md`

 * *Files identical despite different names*

### Comparing `oncall-slackbot-1.332/oncall_slackbot/bot.py` & `oncall-slackbot-1.337/oncall_slackbot/bot.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,40 +14,44 @@
 from oncall_slackbot.integrations import nlp
 
 logger = logging.getLogger(__name__)
 
 
 class Bot:
     def __init__(self):
-        alias_regex = ''
-        if getattr(settings, 'ALIASES', None):
-            logger.info('using aliases %s', settings.ALIASES)
-            alias_regex = '|(?P<alias>{})'.format('|'.join([re.escape(s) for s in settings.ALIASES.split(',')]))
+        alias_regex = ""
+        if getattr(settings, "ALIASES", None):
+            logger.info("using aliases %s", settings.ALIASES)
+            alias_regex = "|(?P<alias>{})".format(
+                "|".join([re.escape(s) for s in settings.ALIASES.split(",")])
+            )
 
         self.at_message_matcher = re.compile(
-            fr'^(?:\<@(?P<atuser>\w+)\>:?|(?P<username>\w+):{alias_regex}) ?(?P<text>[\s\S]*)$'
+            rf"^(?:\<@(?P<atuser>\w+)\>:?|(?P<username>\w+):{alias_regex}) ?(?P<text>[\s\S]*)$"
         )
 
         self._pool = WorkerPool(self.dispatch_msg)
 
         # pylint: disable=no-member
         self._client = SlackClient(
             settings.API_TOKEN,
-            timeout=settings.TIMEOUT if hasattr(settings, 'TIMEOUT') else None,
-            bot_icon=settings.BOT_ICON if hasattr(settings, 'BOT_ICON') else None,
-            bot_emoji=settings.BOT_EMOJI if hasattr(settings, 'BOT_EMOJI') else None,
-            rtm_handlers=[self.handle_message]
+            timeout=settings.TIMEOUT if hasattr(settings, "TIMEOUT") else None,
+            bot_icon=settings.BOT_ICON if hasattr(settings, "BOT_ICON") else None,
+            bot_emoji=settings.BOT_EMOJI if hasattr(settings, "BOT_EMOJI") else None,
+            rtm_handlers=[self.handle_message],
         )
 
         errors_to = settings.ERRORS_TO
         self._errors_to = None
         if errors_to:
             self._errors_to = self._client.find_channel_by_name(errors_to)
             if not self._errors_to:
-                raise ValueError('Could not find errors_to recipient {!r}'.format(errors_to))
+                raise ValueError(
+                    "Could not find errors_to recipient {!r}".format(errors_to)
+                )
 
         self._plugins = PluginsManager()
 
     def dispatch_msg(self, msg):
         if len(msg) > 2:
             override_match_text = msg[2]
         else:
@@ -65,153 +69,167 @@
             # NOTE: This isn't really ideal as respond_to could respond with something when nlp_respond_to did not
             #   but it is a stop-gap that should work most of the time since most won't be combining nlp with non-nlp
             #   plugins I would imagine
             # if (category == 'respond_to' and not msg.get('nlp_label')) or \
             #         (category == 'nlp_label_respond_to' and msg.get('nlp_label')):
             #     if not self._dispatch_msg_handler_override('default_reply', msg, override_match_text):
             #         self._default_reply(msg)
-            if category == 'respond_to':
-                if not self._dispatch_msg_handler('default_reply', msg):
+            if category == "respond_to":
+                if not self._dispatch_msg_handler("default_reply", msg):
                     self._default_reply(msg)
 
     def _dispatch_msg_handler(self, category, msg, override_match_text=None):
         responded = False
-        match_text = override_match_text or msg.get('text', None)
+        match_text = override_match_text or msg.get("text", None)
         for func, args in self._plugins.get_plugins(category, match_text):
             if func:
                 responded = True
                 try:
                     func(Message(self._client, msg), *args)
                 except Exception:  # pylint: disable=broad-except
-                    logger.exception('failed to handle message %s with plugin "%s"', msg['text'], func.__name__)
-                    reply = f'[{func.__name__}] I had a problem handling "{msg["text"]}"\n'
-                    _tb = f'```\n{traceback.format_exc()}\n```'
+                    logger.exception(
+                        'failed to handle message %s with plugin "%s"',
+                        msg["text"],
+                        func.__name__,
+                    )
+                    reply = (
+                        f'[{func.__name__}] I had a problem handling "{msg["text"]}"\n'
+                    )
+                    _tb = f"```\n{traceback.format_exc()}\n```"
                     if self._errors_to:
-                        self._client.rtm_send_message(msg['channel'], reply)
-                        self._client.rtm_send_message(self._errors_to, f'{reply}\n{_tb}')
+                        self._client.rtm_send_message(msg["channel"], reply)
+                        self._client.rtm_send_message(
+                            self._errors_to, f"{reply}\n{_tb}"
+                        )
                     else:
-                        self._client.rtm_send_message(msg['channel'], f'{reply}\n{_tb}')
+                        self._client.rtm_send_message(msg["channel"], f"{reply}\n{_tb}")
         return responded
 
     def filter_text(self, msg):
-        full_text = msg.get('text', '') or ''
-        channel = msg['channel']
+        full_text = msg.get("text", "") or ""
+        channel = msg["channel"]
         bot_name = self._get_bot_name()
         bot_id = self._get_bot_id()
         _msg = self.at_message_matcher.match(full_text)
 
-        if channel[0] == 'C' or channel[0] == 'G':
+        if channel[0] == "C" or channel[0] == "G":
             if not _msg:
                 return None
 
             matches = _msg.groupdict()
 
-            atuser = matches.get('atuser')
-            username = matches.get('username')
-            text = matches.get('text')
-            alias = matches.get('alias')
+            atuser = matches.get("atuser")
+            username = matches.get("username")
+            text = matches.get("text")
+            alias = matches.get("alias")
 
             if alias:
                 atuser = bot_id
 
             if atuser != bot_id and username != bot_name:
                 # a channel message at other user
                 return None
 
-            logger.debug('got an AT message: %s', text)
-            msg['text'] = text
+            logger.debug("got an AT message: %s", text)
+            msg["text"] = text
         else:
             if _msg:
-                msg['text'] = _msg.groupdict().get('text', None)
+                msg["text"] = _msg.groupdict().get("text", None)
         return msg
 
     def _get_bot_id(self):
-        return self._client.login_data['self']['id']
+        return self._client.login_data["self"]["id"]
 
     def _get_bot_name(self):
-        return self._client.login_data['self']['name']
+        return self._client.login_data["self"]["name"]
 
     def _on_new_message(self, msg):
         # ignore edits
-        subtype = msg.get('subtype', '')
-        if subtype == 'message_changed':
+        subtype = msg.get("subtype", "")
+        if subtype == "message_changed":
             return
 
         botname = self._get_bot_name()
         try:
-            msguser = self._client.users.get(msg['user'])
-            username = msguser['name']
+            msguser = self._client.users.get(msg["user"])
+            username = msguser["name"]
         except (KeyError, TypeError):
-            if 'username' in msg:
-                username = msg['username']
-            elif 'bot_profile' in msg and 'name' in msg['bot_profile']:
-                username = msg['bot_profile']['name']
+            if "username" in msg:
+                username = msg["username"]
+            elif "bot_profile" in msg and "name" in msg["bot_profile"]:
+                username = msg["bot_profile"]["name"]
             else:
                 return
 
-        if username in [botname, 'slackbot']:
+        if username in [botname, "slackbot"]:
             return
 
         msg_respond_to = self.filter_text(msg)
         if msg_respond_to:
-            self._pool.add_task(('respond_to', msg_respond_to))
+            self._pool.add_task(("respond_to", msg_respond_to))
         else:
-            self._pool.add_task(('listen_to', msg))
+            self._pool.add_task(("listen_to", msg))
 
     def _default_reply(self, msg):
         _default_reply = settings.DEFAULT_REPLY
         if _default_reply is None:
-            _default_reply = [f"Bad command \"{msg['text']}\", You can ask me one of the following questions:\n"]
+            _default_reply = [
+                f"Bad command \"{msg['text']}\", You can ask me one of the following questions:\n"
+            ]
             _default_reply += [
                 f'    • `{p.pattern}` {v.__doc__ or ""}'
-                for p, v in self._plugins.commands['respond_to'].items()
+                for p, v in self._plugins.commands["respond_to"].items()
             ]
-            _default_reply = '\n'.join(_default_reply)
+            _default_reply = "\n".join(_default_reply)
 
         _msg = Message(self._client, msg)
         _msg.reply(_default_reply)
 
     def handle_message(self, event: str):
         event = json.loads(event)
-        event_type = event.get('type')
-        if event_type == 'message':
+        event_type = event.get("type")
+        if event_type == "message":
             self._on_new_message(event)
-        elif event_type in ['channel_created', 'channel_rename',
-                            'group_joined', 'group_rename',
-                            'im_created']:
-            channel = [event['channel']]
+        elif event_type in [
+            "channel_created",
+            "channel_rename",
+            "group_joined",
+            "group_rename",
+            "im_created",
+        ]:
+            channel = [event["channel"]]
             self._client.parse_channel_data(channel)
-        elif event_type in ['team_join', 'user_change']:
-            user = [event['user']]
+        elif event_type in ["team_join", "user_change"]:
+            user = [event["user"]]
             self._client.parse_user_data(user)
 
     def run(self):
         self._plugins.init_plugins()
         self._pool.start()
         if not self._client.connected:
             self._client.rtm_connect()
 
-        logger.info('connected to slack RTM api')
+        logger.info("connected to slack RTM api")
         self._client.start()
 
 
 def respond_to(matchstr, flags=0):
     def wrapper(func):
-        PluginsManager.commands['respond_to'][
-            re.compile(matchstr, flags)] = func
-        logger.info('registered respond_to plugin "%s" to "%s"', func.__name__, matchstr)
+        PluginsManager.commands["respond_to"][re.compile(matchstr, flags)] = func
+        logger.info(
+            'registered respond_to plugin "%s" to "%s"', func.__name__, matchstr
+        )
         return func
 
     return wrapper
 
 
 def listen_to(matchstr, flags=0):
     def wrapper(func):
-        PluginsManager.commands['listen_to'][
-            re.compile(matchstr, flags)] = func
+        PluginsManager.commands["listen_to"][re.compile(matchstr, flags)] = func
         logger.info('registered listen_to plugin "%s" to "%s"', func.__name__, matchstr)
         return func
 
     return wrapper
 
 
 # def default_reply(matchstr=r'^.*$', flags=0):
@@ -219,203 +237,235 @@
     """
     Decorator declaring the wrapped function to the default reply hanlder.
 
     May be invoked as a simple, argument-less decorator (i.e. ``@default_reply``) or
     with arguments customizing its behavior (e.g. ``@default_reply(matchstr='pattern')``).
     """
     invoked = bool(not args or kwargs)
-    matchstr = kwargs.pop('matchstr', r'^.*$')
-    flags = kwargs.pop('flags', 0)
+    matchstr = kwargs.pop("matchstr", r"^.*$")
+    flags = kwargs.pop("flags", 0)
 
     if not invoked:
         func = args[0]
 
     def wrapper(func):
-        PluginsManager.commands['default_reply'][
-            re.compile(matchstr, flags)] = func
-        logger.info('registered default_reply plugin "%s" to "%s"', func.__name__,
-                    matchstr)
+        PluginsManager.commands["default_reply"][re.compile(matchstr, flags)] = func
+        logger.info(
+            'registered default_reply plugin "%s" to "%s"', func.__name__, matchstr
+        )
         return func
 
     return wrapper if invoked else wrapper(func)
 
 
 def unicode_compact(func):
     """
     Make sure the first parameter of the decorated method to be a unicode
     object.
     """
 
     @wraps(func)
     def wrapped(self, text, *a, **kw):
         if not isinstance(text, str):
-            text = text.decode('utf-8')
+            text = text.decode("utf-8")
         return func(self, text, *a, **kw)
 
     return wrapped
 
 
 class Message:
     def __init__(self, slackclient, body):
         self._client = slackclient
         self._body = body
         self._plugins = PluginsManager()
 
     def _get_user_id(self):
-        if 'user' in self._body:
-            return self._body['user']
+        if "user" in self._body:
+            return self._body["user"]
 
-        return self._client.find_user_by_name(self._body['username'])
+        return self._client.find_user_by_name(self._body["username"])
 
     @unicode_compact
     def _gen_at_message(self, text):
-        text = '<@{}>: {}'.format(self._get_user_id(), text)
+        text = "<@{}>: {}".format(self._get_user_id(), text)
         return text
 
     @unicode_compact
     def gen_reply(self, text):
-        chan = self._body['channel']
-        if chan.startswith('C') or chan.startswith('G'):
+        chan = self._body["channel"]
+        if chan.startswith("C") or chan.startswith("G"):
             return self._gen_at_message(text)
         return text
 
     # pylint: disable=too-many-arguments
     @unicode_compact
-    def reply_webapi(self, text, attachments=None, blocks=None, as_user=True, in_thread=None):
+    def reply_webapi(
+        self, text, attachments=None, blocks=None, as_user=True, in_thread=None
+    ):
         """
-            Send a reply to the sender using Web API
+        Send a reply to the sender using Web API
 
-            (This function supports formatted message
-            when using a bot integration)
+        (This function supports formatted message
+        when using a bot integration)
 
-            If the message was sent in a thread, answer in a thread per default.
+        If the message was sent in a thread, answer in a thread per default.
         """
         if in_thread is None:
-            in_thread = 'thread_ts' in self.body
+            in_thread = "thread_ts" in self.body
 
         if in_thread:
-            self.send_webapi(text, attachments=attachments, blocks=blocks, as_user=as_user, thread_ts=self.thread_ts)
+            self.send_webapi(
+                text,
+                attachments=attachments,
+                blocks=blocks,
+                as_user=as_user,
+                thread_ts=self.thread_ts,
+            )
         else:
             text = self.gen_reply(text)
-            self.send_webapi(text, attachments=attachments, blocks=blocks, as_user=as_user)
+            self.send_webapi(
+                text, attachments=attachments, blocks=blocks, as_user=as_user
+            )
 
     # pylint: disable=too-many-arguments
     @unicode_compact
-    def send_webapi(self, text, attachments=None, blocks=None, as_user=True, thread_ts=None):
-        """
-            Send a reply using Web API
-            (This function supports formatted message
-            when using a bot integration)
+    def send_webapi(
+        self, text, attachments=None, blocks=None, as_user=True, thread_ts=None
+    ):
+        """
+        Send a reply using Web API
+        (This function supports formatted message
+        when using a bot integration)
         """
         self._client.send_message(
-            self._body['channel'],
+            self._body["channel"],
             text,
             attachments=attachments,
             blocks=blocks,
             as_user=as_user,
-            thread_ts=thread_ts)
+            thread_ts=thread_ts,
+        )
 
     @unicode_compact
     def reply(self, text, in_thread=None):
         """
-            Send a reply to the sender using RTM API
+        Send a reply to the sender using RTM API
 
-            (This function doesn't supports formatted message
-            when using a bot integration)
+        (This function doesn't supports formatted message
+        when using a bot integration)
 
-            If the message was send in a thread, answer in a thread per default.
+        If the message was send in a thread, answer in a thread per default.
         """
         if in_thread is None:
-            in_thread = 'thread_ts' in self.body
+            in_thread = "thread_ts" in self.body
 
         if in_thread:
             self.send(text, thread_ts=self.thread_ts)
         else:
             text = self.gen_reply(text)
             self.send(text)
 
     @unicode_compact
     def direct_reply(self, text):
         """
-            Send a reply via direct message using RTM API
+        Send a reply via direct message using RTM API
 
         """
         channel_id = self._client.open_dm_channel(self._get_user_id())
         self._client.rtm_send_message(channel_id, text)
 
     @unicode_compact
     def send(self, text, thread_ts=None):
         """
-            Send a reply using RTM API
+        Send a reply using RTM API
 
-            (This function doesn't supports formatted message
-            when using a bot integration)
+        (This function doesn't supports formatted message
+        when using a bot integration)
         """
-        self._client.rtm_send_message(self._body['channel'], text, thread_ts=thread_ts)
+        self._client.rtm_send_message(self._body["channel"], text, thread_ts=thread_ts)
 
     def react(self, emojiname):
         """
-           React to a message using the web api
+        React to a message using the web api
         """
         self._client.react_to_message(
             emojiname=emojiname,
-            channel=self._body['channel'],
-            timestamp=self._body['ts'])
+            channel=self._body["channel"],
+            timestamp=self._body["ts"],
+        )
 
     @property
     def channel(self):
-        return self._client.get_channel(self._body['channel'])
+        return self._client.get_channel(self._body["channel"])
 
     @property
     def body(self):
         return self._body
 
     @property
     def user(self):
-        return self._client.get_user(self._body['user'])
+        return self._client.get_user(self._body["user"])
 
     @property
     def thread_ts(self):
         try:
-            thread_ts = self.body['thread_ts']
+            thread_ts = self.body["thread_ts"]
         except KeyError:
-            thread_ts = self.body['ts']
+            thread_ts = self.body["ts"]
 
         return thread_ts
 
     def docs_reply(self):
         reply = [
-            f'    • `{v.__name__}` {v.__doc__}'
-            for _, v in self._plugins.commands['respond_to'].items()
+            f"    • `{v.__name__}` {v.__doc__}"
+            for _, v in self._plugins.commands["respond_to"].items()
         ]
-        return '\n'.join(reply)
+        return "\n".join(reply)
 
 
 def nlp_label_respond_to(match_label, flags=0):
     def wrapper(func):
         if nlp.is_backend_present():
-            PluginsManager.commands['nlp_label_respond_to'][re.compile(match_label, flags)] = func
-            logger.info('registered nlp_label_respond_to plugin "%s" to "%s"', func.__name__, match_label)
+            PluginsManager.commands["nlp_label_respond_to"][
+                re.compile(match_label, flags)
+            ] = func
+            logger.info(
+                'registered nlp_label_respond_to plugin "%s" to "%s"',
+                func.__name__,
+                match_label,
+            )
         else:
-            logger.warning('no NLP backend is configured to handle nlp_label_respond_to for "%s"', func.__name__)
+            logger.warning(
+                'no NLP backend is configured to handle nlp_label_respond_to for "%s"',
+                func.__name__,
+            )
         return func
 
     return wrapper
 
 
 def nlp_label_listen_to(match_label, flags=0):
     def wrapper(func):
         if nlp.is_backend_present():
-            PluginsManager.commands['nlp_label_listen_to'][re.compile(match_label, flags)] = func
-            logger.info('registered nlp_label_listen_to plugin "%s" to "%s"', func.__name__, match_label)
+            PluginsManager.commands["nlp_label_listen_to"][
+                re.compile(match_label, flags)
+            ] = func
+            logger.info(
+                'registered nlp_label_listen_to plugin "%s" to "%s"',
+                func.__name__,
+                match_label,
+            )
         else:
-            logger.warning('no NLP backend is configured to handle nlp_label_listen_to for "%s"', func.__name__)
+            logger.warning(
+                'no NLP backend is configured to handle nlp_label_listen_to for "%s"',
+                func.__name__,
+            )
         return func
 
     return wrapper
 
 
 if nlp.is_backend_present():
-    if 'nlp_label_respond_to' not in PluginsManager.commands:
-        PluginsManager.commands['nlp_label_respond_to'] = {}
-    if 'nlp_label_listen_to' not in PluginsManager.commands:
-        PluginsManager.commands['nlp_label_listen_to'] = {}
+    if "nlp_label_respond_to" not in PluginsManager.commands:
+        PluginsManager.commands["nlp_label_respond_to"] = {}
+    if "nlp_label_listen_to" not in PluginsManager.commands:
+        PluginsManager.commands["nlp_label_listen_to"] = {}
```

### Comparing `oncall-slackbot-1.332/oncall_slackbot/integrations/nlp/__init__.py` & `oncall-slackbot-1.337/oncall_slackbot/integrations/nlp/__init__.py`

 * *Files identical despite different names*

### Comparing `oncall-slackbot-1.332/oncall_slackbot/integrations/nlp/spacy.py` & `oncall-slackbot-1.337/oncall_slackbot/integrations/nlp/spacy.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,33 +14,33 @@
 
 def is_configured() -> bool:
     return not not settings.SPACY_MODEL  # pylint: disable=unneeded-not
 
 
 def _initialize_textcat(nlp: Language) -> None:
     # Ensure that the text categorizer is added to the pipeline
-    if 'textcat' not in nlp.pipe_names:
-        LOGGER.info('Adding the text categorizer to the spacy nlp pipeline')
+    if "textcat" not in nlp.pipe_names:
+        LOGGER.info("Adding the text categorizer to the spacy nlp pipeline")
 
         # nlp.create_pipe works for built-ins that are registered with spaCy
         textcat = nlp.create_pipe(
-            'textcat', config={'exclusive_classes': True, 'architecture': 'simple_cnn'}
+            "textcat", config={"exclusive_classes": True, "architecture": "simple_cnn"}
         )
         nlp.add_pipe(textcat, last=True)
 
 
 def _get_nlp() -> Optional[Language]:
     global _NLP  # pylint: disable=global-statement
     if not is_configured():
         return None
     if not _NLP:
-        LOGGER.debug('Loading spacy model from %s', settings.SPACY_MODEL)
+        LOGGER.debug("Loading spacy model from %s", settings.SPACY_MODEL)
         _NLP = spacy.load(settings.SPACY_MODEL)
         _initialize_textcat(_NLP)
-        LOGGER.info('Initialized spacy nlp backend from model %s', settings.SPACY_MODEL)
+        LOGGER.info("Initialized spacy nlp backend from model %s", settings.SPACY_MODEL)
     return _NLP
 
 
 def get_doc(message_text: str) -> Optional[Doc]:
     if not message_text:
         return None
     nlp = _get_nlp()
```

### Comparing `oncall-slackbot-1.332/oncall_slackbot/integrations/pagerduty.py` & `oncall-slackbot-1.337/oncall_slackbot/integrations/pagerduty.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,44 +21,50 @@
         return None
     return PagerDuty(settings.PAGERDUTY_TOKEN)
 
 
 def get_user_name(user: User) -> Optional[str]:
     if not settings.PAGERDUTY_USERNAME_EMAIL_DOMAIN:
         return None
-    email_suffix = f'@{settings.PAGERDUTY_USERNAME_EMAIL_DOMAIN}'
+    email_suffix = f"@{settings.PAGERDUTY_USERNAME_EMAIL_DOMAIN}"
     if not user.email.endswith(email_suffix):
         return None
-    return user.email.replace(email_suffix, '')
+    return user.email.replace(email_suffix, "")
 
 
 def get_schedule_id():
     return settings.PAGERDUTY_SCHEDULE_ID
 
 
-def get_humanized_datetime(datetime_string: str, dest_time_zone_str: Optional[str] = None) -> str:
-    parsed = datetime.strptime(datetime_string, '%Y-%m-%dT%H:%M:%SZ').replace(tzinfo=UTC)
+def get_humanized_datetime(
+    datetime_string: str, dest_time_zone_str: Optional[str] = None
+) -> str:
+    parsed = datetime.strptime(datetime_string, "%Y-%m-%dT%H:%M:%SZ").replace(
+        tzinfo=UTC
+    )
     if dest_time_zone_str:
         dest_time_zone = timezone(dest_time_zone_str)
         parsed = parsed.astimezone(dest_time_zone)
     else:
         dest_time_zone = UTC
     result = humanize.naturaldate(parsed)
-    if result != 'today':
+    if result != "today":
         return result
     return humanize.naturaltime(datetime.now(dest_time_zone) - parsed)
 
 
 def get_current_oncall() -> Optional[Oncall]:
     client = _get_client()
     if not client:
-        LOGGER.debug('Pager duty settings are not configured, cannot retrieve current on call')
+        LOGGER.debug(
+            "Pager duty settings are not configured, cannot retrieve current on call"
+        )
         return None
 
-    oncalls = client.oncalls.list(include=['users'], schedule_ids=[get_schedule_id()])
+    oncalls = client.oncalls.list(include=["users"], schedule_ids=[get_schedule_id()])
     current_oncall = None
     for oncall in oncalls:
         current_oncall = oncall
         break
     if not current_oncall:
         return None
     return current_oncall
```

### Comparing `oncall-slackbot-1.332/oncall_slackbot/manager.py` & `oncall-slackbot-1.337/oncall_slackbot/manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,54 +10,51 @@
 logger = logging.getLogger(__name__)
 
 
 class PluginsManager:
     def __init__(self):
         pass
 
-    commands = {
-        'respond_to': {},
-        'listen_to': {},
-        'default_reply': {}
-    }
+    commands = {"respond_to": {}, "listen_to": {}, "default_reply": {}}
 
     def init_plugins(self):
-        if hasattr(settings, 'PLUGINS'):
+        if hasattr(settings, "PLUGINS"):
             plugins = settings.PLUGINS
         else:
-            plugins = 'slackbot.plugins'
+            plugins = "slackbot.plugins"
 
         for plugin in plugins:
             self._load_plugins(plugin)
 
     @staticmethod
     def _load_plugins(plugin):
         logger.info('loading plugin "%s"', plugin)
         path_name = importlib_find(plugin)
         try:
             path_name = path_name.submodule_search_locations[0]
         except TypeError:
             path_name = path_name.origin
 
         module_list = [plugin]
-        if not path_name.endswith('.py'):
-            module_list = glob('{}/[!_]*.py'.format(path_name))
-            module_list = ['.'.join((plugin, os.path.split(f)[-1][:-3])) for f
-                           in module_list]
+        if not path_name.endswith(".py"):
+            module_list = glob("{}/[!_]*.py".format(path_name))
+            module_list = [
+                ".".join((plugin, os.path.split(f)[-1][:-3])) for f in module_list
+            ]
         for module in module_list:
             try:
                 import_module(module)
             except Exception:  # pylint: disable=broad-except
                 # TODO Better exception handling
-                logger.exception('Failed to import %s', module)
+                logger.exception("Failed to import %s", module)
 
     def get_plugins(self, category, text):
         has_matching_plugin = False
         if text is None:
-            text = ''
+            text = ""
         for matcher in self.commands[category]:
             match = matcher.search(text)
             if match:
                 has_matching_plugin = True
                 yield self.commands[category][matcher], match.groups()
 
         if not has_matching_plugin:
```

### Comparing `oncall-slackbot-1.332/oncall_slackbot/plugins/blocks.py` & `oncall-slackbot-1.337/oncall_slackbot/plugins/blocks.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,66 +1,59 @@
 # -*- coding: utf-8 -*-
 
 from oncall_slackbot.bot import respond_to
 
 
-@respond_to('^reply blocks$')
+@respond_to("^reply blocks$")
 def reply_blocks(message):
-    message.reply_webapi('hello there!', blocks=[
-        {
-            "type": "section",
-            "text": {
-                "type": "mrkdwn",
-                "text": "You have a new request:\n*<fakeLink.toEmployeeProfile.com|Fred Enriquez - New device request>*"
-            }
-        },
-        {
-            "type": "section",
-            "fields": [
-                {
+    message.reply_webapi(
+        "hello there!",
+        blocks=[
+            {
+                "type": "section",
+                "text": {
                     "type": "mrkdwn",
-                    "text": "*Type:*\nComputer (laptop)"
+                    "text": "You have a new request:\n*<fakeLink.toEmployeeProfile.com|Fred Enriquez - New device request>*",
                 },
-                {
-                    "type": "mrkdwn",
-                    "text": "*When:*\nSubmitted Aut 10"
-                },
-                {
-                    "type": "mrkdwn",
-                    "text": "*Last Update:*\nMar 10, 2015 (3 years, 5 months)"
-                },
-                {
-                    "type": "mrkdwn",
-                    "text": "*Reason:*\nAll vowel keys aren't working."
-                },
-                {
-                    "type": "mrkdwn",
-                    "text": "*Specs:*\n\"Cheetah Pro 15\" - Fast, really fast\""
-                }
-            ]
-        },
-        {
-            "type": "actions",
-            "elements": [
-                {
-                    "type": "button",
-                    "text": {
-                        "type": "plain_text",
-                        "emoji": True,
-                        "text": "Approve"
+            },
+            {
+                "type": "section",
+                "fields": [
+                    {"type": "mrkdwn", "text": "*Type:*\nComputer (laptop)"},
+                    {"type": "mrkdwn", "text": "*When:*\nSubmitted Aut 10"},
+                    {
+                        "type": "mrkdwn",
+                        "text": "*Last Update:*\nMar 10, 2015 (3 years, 5 months)",
                     },
-                    "style": "primary",
-                    "value": "click_me_123"
-                },
-                {
-                    "type": "button",
-                    "text": {
-                        "type": "plain_text",
-                        "emoji": True,
-                        "text": "Deny"
+                    {
+                        "type": "mrkdwn",
+                        "text": "*Reason:*\nAll vowel keys aren't working.",
+                    },
+                    {
+                        "type": "mrkdwn",
+                        "text": '*Specs:*\n"Cheetah Pro 15" - Fast, really fast"',
+                    },
+                ],
+            },
+            {
+                "type": "actions",
+                "elements": [
+                    {
+                        "type": "button",
+                        "text": {
+                            "type": "plain_text",
+                            "emoji": True,
+                            "text": "Approve",
+                        },
+                        "style": "primary",
+                        "value": "click_me_123",
+                    },
+                    {
+                        "type": "button",
+                        "text": {"type": "plain_text", "emoji": True, "text": "Deny"},
+                        "style": "danger",
+                        "value": "click_me_123",
                     },
-                    "style": "danger",
-                    "value": "click_me_123"
-                }
-            ]
-        }
-    ])
+                ],
+            },
+        ],
+    )
```

### Comparing `oncall-slackbot-1.332/oncall_slackbot/plugins/nlp.py` & `oncall-slackbot-1.337/oncall_slackbot/plugins/nlp.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,23 +7,26 @@
 LOGGER = logging.getLogger(__name__)
 
 
 class OnCallMessage(Message):
     """
     Overrides a message to add support for nlp label.
     """
+
     @property
     def nlp_label(self):
-        return self._body.get('nlp_label')
+        return self._body.get("nlp_label")
 
 
-@nlp_label_listen_to(r'^test')
-def process_nlp(message: OnCallMessage):
+@nlp_label_listen_to(r"^test")
+def process_nlp_test(message: OnCallMessage):
     # You don't have to process the doc with spacy again, but you can if you want to retrieve more information
-    doc = spacy.get_doc(message.body['text'])
-    message.reply(f'Message has a test-prefixed nlp label of "{message.nlp_label}", '
-                  f'{list((token.text, token.pos_, token.dep_) for token in doc)}')
+    doc = spacy.get_doc(message.body["text"])
+    message.reply(
+        f'Message has a test-prefixed nlp label of "{message.nlp_label}", '
+        f"{list((token.text, token.pos_, token.dep_) for token in doc)}"
+    )
 
 
-@nlp_label_respond_to(r'^ignore$')
-def process_nlp(message: OnCallMessage):
-    message.reply('This message has a nlp label that signifies it is ignored')
+@nlp_label_respond_to(r"^ignore$")
+def process_nlp_ignore(message: OnCallMessage):
+    message.reply("This message has a nlp label that signifies it is ignored")
```

### Comparing `oncall-slackbot-1.332/oncall_slackbot/plugins/oncall.py` & `oncall-slackbot-1.337/oncall_slackbot/plugins/oncall.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,69 +5,81 @@
 from typing import Optional
 from pygerduty.v2 import ContactMethod  # pylint: disable=import-error
 from oncall_slackbot.bot import listen_to, Message
 from oncall_slackbot.integrations import pagerduty
 
 LOGGER = logging.getLogger(__name__)
 CONTACT_METHOD_EMOTICON_BY_TYPE = {
-    'email_contact_method': ':email:',
-    'phone_contact_method': ':slack_call:',
+    "email_contact_method": ":email:",
+    "phone_contact_method": ":slack_call:",
     # Do not show anything for push or SMS notifications, since they duplicate the phone contact
-    'sms_contact_method': None,
-    'push_notification_contact_method': None,
+    "sms_contact_method": None,
+    "push_notification_contact_method": None,
 }
 
 
-def _get_contact_method_message(contact_method: ContactMethod, add_label: bool) -> Optional[str]:
+def _get_contact_method_message(
+    contact_method: ContactMethod, add_label: bool
+) -> Optional[str]:
     emoticon = CONTACT_METHOD_EMOTICON_BY_TYPE.get(contact_method.type)
-    if not emoticon or (hasattr(contact_method, 'enabled') and not contact_method.enabled):
+    if not emoticon or (
+        hasattr(contact_method, "enabled") and not contact_method.enabled
+    ):
         return None
-    label = ''
+    label = ""
     if add_label:
-        label = f' ({contact_method.label})'
-    return f'{emoticon} {contact_method.address}{label}'
+        label = f" ({contact_method.label})"
+    return f"{emoticon} {contact_method.address}{label}"
 
 
-@listen_to(r'who is (?:currently )?on(?:-| |)call', re.IGNORECASE)
+@listen_to(r"who is (?:currently )?on(?:-| |)call", re.IGNORECASE)
 def who_is_on_call(message: Message):
     if not pagerduty.is_configured():
-        LOGGER.debug('Pager duty settings are not configured, cannot retrieve current on call')
+        LOGGER.debug(
+            "Pager duty settings are not configured, cannot retrieve current on call"
+        )
         return
 
     current_oncall = pagerduty.get_current_oncall()
     if not current_oncall:
-        message.reply(f'No current on-call information found for schedule {pagerduty.get_schedule_id()}')
+        message.reply(
+            f"No current on-call information found for schedule {pagerduty.get_schedule_id()}"
+        )
         return
 
     # Build up contact methods string
     contact_method_messages = []
     user_name = pagerduty.get_user_name(current_oncall.user)
     if user_name:
-        contact_method_messages.append(f':slack: @{user_name}')
-    contact_methods = current_oncall.user.contact_methods.list(time_zone='MDT')
+        contact_method_messages.append(f":slack: @{user_name}")
+    contact_methods = current_oncall.user.contact_methods.list(time_zone="MDT")
     for contact_method in contact_methods:
         # Only add label if there is no user name
-        contact_method_message = _get_contact_method_message(contact_method, not user_name)
+        contact_method_message = _get_contact_method_message(
+            contact_method, not user_name
+        )
         if contact_method_message:
             contact_method_messages.append(contact_method_message)
 
     # Get formatted end time
-    end_time = pagerduty.get_humanized_datetime(current_oncall.end, current_oncall.user.time_zone)
-
-    message.reply_webapi(f'{current_oncall.user.name} is currently on call', in_thread=True, blocks=[
-        {
-            "type": "section",
-            "text": {
-                "type": "mrkdwn",
-                "text":
-                    f'*<{current_oncall.user.html_url}|{current_oncall.user.name}>* is on call '
-                    f'<{current_oncall.schedule.html_url}|until {end_time}>'
-            }
-        },
-        {
-            "type": "section",
-            "text": {
-                "type": "mrkdwn",
-                "text": '\n'.join(contact_method_messages)
-            }
-        },
-    ])
+    end_time = pagerduty.get_humanized_datetime(
+        current_oncall.end, current_oncall.user.time_zone
+    )
+
+    message.reply_webapi(
+        f"{current_oncall.user.name} is currently on call",
+        in_thread=True,
+        blocks=[
+            {
+                "type": "section",
+                "text": {
+                    "type": "mrkdwn",
+                    "text": f"*<{current_oncall.user.html_url}|{current_oncall.user.name}>* is on call "
+                    f"<{current_oncall.schedule.html_url}|until {end_time}>",
+                },
+            },
+            {
+                "type": "section",
+                "text": {"type": "mrkdwn", "text": "\n".join(contact_method_messages)},
+            },
+        ],
+    )
```

### Comparing `oncall-slackbot-1.332/oncall_slackbot/plugins/upload.py` & `oncall-slackbot-1.337/oncall_slackbot/plugins/upload.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # -*- coding: utf-8 -*-
 
 import os
 from oncall_slackbot.bot import respond_to
 from oncall_slackbot.utils import download_file, create_tmp_file
 
 
-@respond_to(r'upload \<?(.*)\>?')
+@respond_to(r"upload \<?(.*)\>?")
 def upload(message, thing):
     # message.channel.upload_file(slack_filename, local_filename, initial_comment='')
-    if thing == 'favicon':
-        url = 'https://slack.com/favicon.ico'
-        message.reply(f'uploading {url}')
+    if thing == "favicon":
+        url = "https://slack.com/favicon.ico"
+        message.reply(f"uploading {url}")
         with create_tmp_file() as tmpf:
             download_file(url, tmpf)
-            message.channel.upload_file(url, tmpf, f'downloaded from {url}')
-    elif thing == 'slack.png':
-        message.reply('uploading slack.png')
+            message.channel.upload_file(url, tmpf, f"downloaded from {url}")
+    elif thing == "slack.png":
+        message.reply("uploading slack.png")
         cwd = os.path.abspath(os.path.dirname(__file__))
-        fname = os.path.join(cwd, '../../tests/functional/slack.png')
+        fname = os.path.join(cwd, "../../tests/functional/slack.png")
         message.channel.upload_file(thing, fname)
 
 
-@respond_to('send_string_content')
+@respond_to("send_string_content")
 def upload_content(message):
     # message.channel.upload_content(slack_filename, content, initial_comment='')
     content = "你好! here's some data\nthat will appear\nas a plain text snippet"
-    message.channel.upload_content('content.txt', content)
+    message.channel.upload_content("content.txt", content)
```

### Comparing `oncall-slackbot-1.332/oncall_slackbot/settings.py` & `oncall-slackbot-1.337/oncall_slackbot/settings.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,73 +3,73 @@
 import os
 # pylint: disable=wildcard-import,unused-wildcard-import
 
 DEBUG = False
 
 ERRORS_TO = None
 
-'''
+"""
 Setup timeout for slacker API requests (e.g. uploading a file).
-'''
+"""
 TIMEOUT = 100
 
 # API_TOKEN = '###token###'
 
-'''
+"""
 Setup a comma delimited list of aliases that the bot will respond to.
 
 Example: if you set ALIASES='!,$' then a bot which would respond to:
 'botname hello'
 will now also respond to
 '$ hello'
-'''
-ALIASES = ''
+"""
+ALIASES = ""
 
-'''
+"""
 If you use Slack Web API to send messages (with
 send_webapi(text, as_user=False) or reply_webapi(text, as_user=False)),
 you can customize the bot logo by providing Icon or Emoji. If you use Slack
 RTM API to send messages (with send() or reply()), or if as_user is True
 (default), the used icon comes from bot settings and Icon or Emoji has no
 effect.
-'''
+"""
 # BOT_ICON = 'http://lorempixel.com/64/64/abstract/7/'
 # BOT_EMOJI = ':godmode:'
 
 # Specify a different reply when the bot is messaged with no matching cmd
 DEFAULT_REPLY = None
 
 
-'''
+"""
 Pager duty configuration, these are optional but both must be specified in
 order to enable pager duty integration.
-'''
+"""
 PAGERDUTY_TOKEN = None
 PAGERDUTY_SCHEDULE_ID = None
 
 
-'''
+"""
 (Optional, only works if pager duty is configured) Configures the email domain used to determine user names from emails.
 For example, emails of the form 'myuser@example.com' should configure this property with a value of 'example.com'
 (exclude the @ prefix). This would result in 'myuser' being set as the user name.
-'''
+"""
 PAGERDUTY_USERNAME_EMAIL_DOMAIN = None
 
 
-'''
+"""
 Spacy configuration, this is optional
-'''
+"""
 SPACY_MODEL = None
 
 PLUGINS = [
-    'oncall_slackbot.plugins',
+    "oncall_slackbot.plugins",
 ]
 
 for key in os.environ:
-    if key[:9] == 'SLACKBOT_':
+    if key[:9] == "SLACKBOT_":
         name = key[9:]
         globals()[name] = os.environ[key]
 
 # pylint: disable=unused-wildcard-import
 try:
     from slackbot_settings import *
 except ImportError:
```

### Comparing `oncall-slackbot-1.332/oncall_slackbot/slackclient.py` & `oncall-slackbot-1.337/oncall_slackbot/slackclient.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,31 +11,41 @@
 
 logger = logging.getLogger(__name__)
 
 
 # pylint: disable=too-many-instance-attributes
 class SlackClient:
     # pylint: disable=too-many-arguments
-    def __init__(self, token, timeout=None, bot_icon=None, bot_emoji=None, connect=True,
-                 rtm_start_args=None, rtm_handlers=None):
+    def __init__(
+        self,
+        token,
+        timeout=None,
+        bot_icon=None,
+        bot_emoji=None,
+        connect=True,
+        rtm_start_args=None,
+        rtm_handlers=None,
+    ):
         self.token = token
         self.bot_icon = bot_icon
         self.bot_emoji = bot_emoji
         self.username = None
         self.domain = None
         self.login_data = None
         self.users = {}
         self.channels = {}
         self.connected = False
         self.rtm_start_args = rtm_start_args
 
         if timeout is None:
             self.rtm = RTMClient(token=self.token)
         else:
-            self.rtm = RTMClient(token=self.token, timeout=timeout, on_message_listeners=rtm_handlers)
+            self.rtm = RTMClient(
+                token=self.token, timeout=timeout, on_message_listeners=rtm_handlers
+            )
 
         rate_limit_handler = RateLimitErrorRetryHandler(max_retry_count=100)
         # Enable rate limited error retries
         self.rtm.web_client.retry_handlers.append(rate_limit_handler)
 
         if connect:
             self.rtm_connect()
@@ -48,131 +58,133 @@
         self.parse_slack_login_data(reply)
         self.connected = True
 
     def reconnect(self):
         while True:
             try:
                 self.rtm_connect()
-                logger.warning('reconnected to slack rtm websocket')
+                logger.warning("reconnected to slack rtm websocket")
                 return
             except Exception as exc:  # pylint: disable=broad-except
-                logger.exception('failed to reconnect: %s', exc)
+                logger.exception("failed to reconnect: %s", exc)
                 time.sleep(5)
 
     def parse_slack_login_data(self, login_data):
         self.login_data = login_data
-        self.domain = self.login_data['team']['domain']
-        self.username = self.login_data['self']['name']
+        self.domain = self.login_data["team"]["domain"]
+        self.username = self.login_data["self"]["name"]
 
-        logger.debug('Getting users')
+        logger.debug("Getting users")
         for page in self.rtm.web_client.users_list(limit=200):
-            self.parse_user_data(page['members'])
-        logger.debug('Getting channels')
+            self.parse_user_data(page["members"])
+        logger.debug("Getting channels")
         for page in self.rtm.web_client.conversations_list(
-                exclude_archived=True,
-                types="public_channel,private_channel",
-                limit=1000
+            exclude_archived=True, types="public_channel,private_channel", limit=1000
         ):
-            self.parse_channel_data(page['channels'])
+            self.parse_channel_data(page["channels"])
 
     def parse_channel_data(self, channel_data):
-        logger.debug('Adding %d users', len(channel_data))
-        self.channels.update({c['id']: c for c in channel_data})
+        logger.debug("Adding %d users", len(channel_data))
+        self.channels.update({c["id"]: c for c in channel_data})
 
     def parse_user_data(self, user_data):
-        logger.debug('Adding %d users', len(user_data))
-        self.users.update({u['id']: u for u in user_data})
+        logger.debug("Adding %d users", len(user_data))
+        self.users.update({u["id"]: u for u in user_data})
 
     def send_to_rtm(self, data):
         """Send (data) directly to the RTMClient."""
         data = json.dumps(data)
         self.rtm.send(data)
 
     def rtm_send_message(self, channel, message, attachments=None, thread_ts=None):
         message_json = {
-            'type': 'message',
-            'channel': channel,
-            'text': message,
-            'attachments': attachments,
-            'thread_ts': thread_ts,
-            }
+            "type": "message",
+            "channel": channel,
+            "text": message,
+            "attachments": attachments,
+            "thread_ts": thread_ts,
+        }
         self.send_to_rtm(message_json)
 
     def upload_file(self, channel, fname, fpath, comment):
         fname = fname or os.path.basename(fpath)
         self.rtm.web_client.files_upload(
-            file=fpath,
-            channels=channel,
-            filename=fname,
-            initial_comment=comment)
+            file=fpath, channels=channel, filename=fname, initial_comment=comment
+        )
 
     def upload_content(self, channel, fname, content, comment):
         self.rtm.web_client.files_upload(
-            channels=channel,
-            content=content,
-            filename=fname,
-            initial_comment=comment)
+            channels=channel, content=content, filename=fname, initial_comment=comment
+        )
 
     # pylint: disable=too-many-arguments
-    def send_message(self, channel, message, attachments=None, blocks=None, as_user=True, thread_ts=None):
+    def send_message(
+        self,
+        channel,
+        message,
+        attachments=None,
+        blocks=None,
+        as_user=True,
+        thread_ts=None,
+    ):
         self.rtm.web_client.chat_postMessage(
             channel=channel,
             text=message,
-            username=self.login_data['self']['name'],
+            username=self.login_data["self"]["name"],
             icon_url=self.bot_icon,
             icon_emoji=self.bot_emoji,
             attachments=attachments,
             blocks=blocks,
             as_user=as_user,
-            thread_ts=thread_ts)
+            thread_ts=thread_ts,
+        )
 
     def get_channel(self, channel_id):
         return Channel(self, self.channels[channel_id])
 
     def open_dm_channel(self, user_id):
         return self.rtm.web_client.conversations_open(users=[user_id])["channel"]["id"]
 
     def find_channel_by_name(self, channel_name):
         for channel_id, channel in self.channels.items():
             try:
-                name = channel['name']
+                name = channel["name"]
             except KeyError:
-                name = self.users[channel['user']]['name']
+                name = self.users[channel["user"]]["name"]
             if name == channel_name:
                 return channel_id
         return None
 
     def get_user(self, user_id):
         return self.users.get(user_id)
 
     def find_user_by_name(self, username):
         for userid, user in self.users.items():
-            if user['name'] == username:
+            if user["name"] == username:
                 return userid
         return None
 
     def react_to_message(self, emojiname, channel, timestamp):
         self.rtm.web_client.reactions_add(
-            name=emojiname,
-            channel=channel,
-            timestamp=timestamp)
+            name=emojiname, channel=channel, timestamp=timestamp
+        )
 
 
 class SlackConnectionError(Exception):
     pass
 
 
 class Channel:
     def __init__(self, slackclient, body):
         self._body = body
         self._client = slackclient
 
     def __eq__(self, compare_str):
-        name = self._body['name']
-        cid = self._body['id']
+        name = self._body["name"]
+        cid = self._body["id"]
         return compare_str in [name, f"#{name}", cid]
 
-    def upload_file(self, fname, fpath, initial_comment=''):
-        self._client.upload_file(self._body['id'], fname, fpath, initial_comment)
+    def upload_file(self, fname, fpath, initial_comment=""):
+        self._client.upload_file(self._body["id"], fname, fpath, initial_comment)
 
-    def upload_content(self, fname, content, initial_comment=''):
-        self._client.upload_content(self._body['id'], fname, content, initial_comment)
+    def upload_content(self, fname, content, initial_comment=""):
+        self._client.upload_content(self._body["id"], fname, content, initial_comment)
```

### Comparing `oncall-slackbot-1.332/oncall_slackbot/utils.py` & `oncall-slackbot-1.337/oncall_slackbot/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 import queue
 from contextlib import contextmanager
 import requests
 
 logger = logging.getLogger(__name__)
 
 
-def download_file(url, fpath, token=''):
-    logger.debug('starting to fetch %s', url)
+def download_file(url, fpath, token=""):
+    logger.debug("starting to fetch %s", url)
     headers = {"Authorization": f"Bearer {token}"} if token else None
     req = requests.get(url, stream=True, headers=headers)
-    with open(fpath, 'wb') as file_handle:
-        for chunk in req.iter_content(chunk_size=1024*64):
+    with open(fpath, "wb") as file_handle:
+        for chunk in req.iter_content(chunk_size=1024 * 64):
             if chunk:  # filter out keep-alive new chunks
                 file_handle.write(chunk)
                 file_handle.flush()
-    logger.debug('fetch %s', fpath)
+    logger.debug("fetch %s", fpath)
     return fpath
 
 
 @contextmanager
-def create_tmp_file(content=''):
+def create_tmp_file(content=""):
     _fd, name = tempfile.mkstemp()
     try:
         if content:
             os.write(_fd, content)
         yield name
     finally:
         os.close(_fd)
@@ -54,18 +54,18 @@
             msg = self.queue.get()
             self.func(msg)
 
 
 def get_http_proxy(environ):
     proxy, proxy_port, no_proxy = None, None, None
 
-    if 'http_proxy' in environ:
-        http_proxy = environ['http_proxy']
-        prefix = 'http://'
+    if "http_proxy" in environ:
+        http_proxy = environ["http_proxy"]
+        prefix = "http://"
         if http_proxy.startswith(prefix):
-            http_proxy = http_proxy[len(prefix):]
-        proxy, proxy_port = http_proxy.split(':')
+            http_proxy = http_proxy[len(prefix) :]
+        proxy, proxy_port = http_proxy.split(":")
 
-    if 'no_proxy' in environ:
-        no_proxy = environ['no_proxy']
+    if "no_proxy" in environ:
+        no_proxy = environ["no_proxy"]
 
     return proxy, proxy_port, no_proxy
```

### Comparing `oncall-slackbot-1.332/oncall_slackbot.egg-info/PKG-INFO` & `oncall-slackbot-1.337/oncall_slackbot.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: oncall-slackbot
-Version: 1.332
+Version: 1.337
 Summary: Slackbot made specifically to handle on-call requests
 Home-page: http://github.com/bluesliverx/oncall-slackbot
 Author: Brian Saville
 Author-email: bksaville@gmail.com
 License: MIT
 Description: UNKNOWN
 Platform: Any
```

### Comparing `oncall-slackbot-1.332/oncall_slackbot.egg-info/SOURCES.txt` & `oncall-slackbot-1.337/oncall_slackbot.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE.txt
 MANIFEST.in
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 oncall_slackbot/VERSION
 oncall_slackbot/__init__.py
 oncall_slackbot/bot.py
 oncall_slackbot/manager.py
 oncall_slackbot/settings.py
```

### Comparing `oncall-slackbot-1.332/setup.py` & `oncall-slackbot-1.337/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import os
 import subprocess
 from setuptools import setup, find_packages
 
 
-MAJOR_VERSION = '1'
+MAJOR_VERSION = "1"
 
-version_file = os.path.join(os.path.dirname(__file__), 'oncall_slackbot/VERSION')
+version_file = os.path.join(os.path.dirname(__file__), "oncall_slackbot/VERSION")
 if os.path.exists(version_file):
     # Read version from file
-    with open(version_file, 'r', encoding='utf8') as fobj:
+    with open(version_file, "r", encoding="utf8") as fobj:
         version = fobj.read().strip()
 else:
     # Generate the version and store it in the file
     # pylint: disable=subprocess-run-check
-    result = subprocess.run('git rev-list --count HEAD', shell=True, capture_output=True, encoding='utf8')
+    result = subprocess.run(
+        "git rev-list --count HEAD", shell=True, capture_output=True, encoding="utf8"
+    )
     commit_count = result.stdout.strip()
-    version = f'{MAJOR_VERSION}.{commit_count}'
-    print(f'Setting version to {version} and writing to {version_file}')
-    with open(version_file, 'w', encoding='utf8') as fobj:
+    version = f"{MAJOR_VERSION}.{commit_count}"
+    print(f"Setting version to {version} and writing to {version_file}")
+    with open(version_file, "w", encoding="utf8") as fobj:
         fobj.write(version)
 
 install_requires = (
     'pygerduty>=0.38.2',
     'pytz>=2019.3',
     'humanize>=3.14.0',
     'spacy==2.2.3',
@@ -29,28 +31,30 @@
 )  # yapf: disable
 
 excludes = (
     '*test*',
     '*local_settings*',
 )  # yapf: disable
 
-setup(name='oncall-slackbot',
-      version=version,
-      license='MIT',
-      description='Slackbot made specifically to handle on-call requests',
-      author='Brian Saville',
-      author_email='bksaville@gmail.com',
-      url='http://github.com/bluesliverx/oncall-slackbot',
-      platforms=['Any'],
-      packages=find_packages(exclude=excludes),
-      install_requires=install_requires,
-      classifiers=['Development Status :: 4 - Beta',
-                   'License :: OSI Approved :: MIT License',
-                   'Operating System :: OS Independent',
-                   'Programming Language :: Python',
-                   'Programming Language :: Python :: 3',
-                   'Programming Language :: Python :: 3.4',
-                   'Programming Language :: Python :: 3.5',
-                   'Programming Language :: Python :: 3.6',
-                   'Programming Language :: Python :: 3.7',
-                   ]
-      )
+setup(
+    name="oncall-slackbot",
+    version=version,
+    license="MIT",
+    description="Slackbot made specifically to handle on-call requests",
+    author="Brian Saville",
+    author_email="bksaville@gmail.com",
+    url="http://github.com/bluesliverx/oncall-slackbot",
+    platforms=["Any"],
+    packages=find_packages(exclude=excludes),
+    install_requires=install_requires,
+    classifiers=[
+        "Development Status :: 4 - Beta",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.4",
+        "Programming Language :: Python :: 3.5",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+    ],
+)
```


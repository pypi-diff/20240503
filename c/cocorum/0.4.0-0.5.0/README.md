# Comparing `tmp/cocorum-0.4.0.tar.gz` & `tmp/cocorum-0.5.0.tar.gz`

## Comparing `cocorum-0.4.0.tar` & `cocorum-0.5.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0   343002 2020-02-02 00:00:00.000000 cocorum-0.4.0/cocorum_icon.png
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 cocorum-0.4.0/requirements.txt
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 cocorum-0.4.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0    18441 2020-02-02 00:00:00.000000 cocorum-0.4.0/src/cocorum/__init__.py
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 cocorum-0.4.0/src/cocorum/localvars.py
--rw-r--r--   0        0        0    13155 2020-02-02 00:00:00.000000 cocorum-0.4.0/src/cocorum/ssechat.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 cocorum-0.4.0/src/cocorum/utils.py
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 cocorum-0.4.0/LICENSE.txt
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 cocorum-0.4.0/README.md
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 cocorum-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 cocorum-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0   343002 2020-02-02 00:00:00.000000 cocorum-0.5.0/cocorum_icon.png
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 cocorum-0.5.0/requirements.txt
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 cocorum-0.5.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0    19903 2020-02-02 00:00:00.000000 cocorum-0.5.0/src/cocorum/__init__.py
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 cocorum-0.5.0/src/cocorum/localvars.py
+-rw-r--r--   0        0        0    13806 2020-02-02 00:00:00.000000 cocorum-0.5.0/src/cocorum/ssechat.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 cocorum-0.5.0/src/cocorum/utils.py
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 cocorum-0.5.0/LICENSE.txt
+-rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 cocorum-0.5.0/README.md
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 cocorum-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 cocorum-0.5.0/PKG-INFO
```

### Comparing `cocorum-0.4.0/cocorum_icon.png` & `cocorum-0.5.0/cocorum_icon.png`

 * *Files identical despite different names*

### Comparing `cocorum-0.4.0/.github/workflows/python-publish.yml` & `cocorum-0.5.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `cocorum-0.4.0/src/cocorum/__init__.py` & `cocorum-0.5.0/src/cocorum/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,62 @@
 #!/usr/bin/env python3
-"""Cocorum: a Python wrapper for the Rumble.com API
+"""An unofficial Python wrapper for the Rumble.com APIs
 
+A Python wrapper for the Rumble Live Stream API v1.0 (beta), with some quality of life additions, such as:
+- Automatic refresh when past the refresh_rate delay when querying any non_static property.
+- All timespamps are parsed to seconds since Epoch, UTC timezone.
+- Chat has new_messages and new_rants properties that return only messages and rants since the last time they were read.
+
+Note, you are only expected to create a RumbleAPI() and / or ssechat.SSEChat() object, and work with everything through them.
+
+Most attributes that are not added features have the same name as the direct JSON counterparts, with the exception of adding prefixes to some things that have the same name in the JSON as Python builtin functions. For example, thing/id in JSON is thing.thing_id in this Python wrapper.
+
+Example usage:
+```
+from cocorum import RumbleAPI
+from cocorum.localvars import *
+
+api = RumbleAPI(API_URL, refresh_rate = 10)
+
+print(api.username)
+print(api.latest_follower)
+
+if api.latest_subscriber:
+    print(api.latest_subscriber, "subscribed for $" + str(api.latest_subscriber.amount_dollars))
+
+#RumbleLivestream objects returned by RumbleAPI properties are deep: When queried, they will pull new information via their parent RumbleAPI object.
+livestream = api.latest_livestream #None if there is no stream running
+
+if livestream:
+    if livestream.visibility != STREAM_VIS_PUBLIC:
+        print("Stream is not public.")
+    message = livestream.chat.latest_message #None if there are no messages yet
+    if message:
+        print(message.username, "said", message)
+```
 S.D.G."""
 
 import time
 import calendar
 import requests
 
 from .localvars import *
-from .utils import *
+from . import utils
 
-class RumbleAPISubObj():
+class APISubObj():
     """Abstract class for a Rumble API object"""
     def __init__(self, json):
         """Pass the JSON block for a single Rumble API subobject"""
         self._json = json
 
     def __getitem__(self, key):
         """Get a key from the JSON"""
         return self._json[key]
 
-class RumbleUserAction(RumbleAPISubObj):
+class UserAction(APISubObj):
     """Abstract class for Rumble user actions"""
     def __init__(self, json):
         """Pass the JSON block for a single Rumble user action"""
         super().__init__(json)
         self.__profile_pic = None
 
     def __eq__(self, other):
@@ -55,30 +87,30 @@
     def profile_pic(self):
         """The user's profile picture as a bytes string"""
         if not self.profile_pic_url: #The profile picture is blank
             return b''
 
         if not self.__profile_pic: #We never queried the profile pic before
             #TODO make this timeout assignable
-            response = requests.get(self.profile_pic_url, DEFAULT_TIMEOUT)
+            response = requests.get(self.profile_pic_url, timeout = DEFAULT_TIMEOUT)
             if response.status_code != 200:
                 raise Exception("Status code " + str(response.status_code))
 
             self.__profile_pic = response.content
 
         return self.__profile_pic
 
-class RumbleFollower(RumbleUserAction):
+class Follower(UserAction):
     """Rumble follower"""
     @property
     def followed_on(self):
         """When the follower followed, in seconds since Epoch UTC"""
-        return parse_timestamp(self["followed_on"])
+        return utils.parse_timestamp(self["followed_on"])
 
-class RumbleSubscriber(RumbleUserAction):
+class Subscriber(UserAction):
     """Rumble subscriber"""
     def __eq__(self, other):
         """Is this subscriber equal to another"""
         #Check if the compared string is our username
         if isinstance(other, str):
             return self.username == other
 
@@ -109,17 +141,17 @@
     def amount_dollars(self):
         """The subscription amount in dollars"""
         return self["amount_dollars"]
 
     @property
     def subscribed_on(self):
         """When the subscriber subscribed, in seconds since Epoch UTC"""
-        return parse_timestamp(self["subscribed_on"])
+        return utils.parse_timestamp(self["subscribed_on"])
 
-class RumbleStreamCategory(RumbleAPISubObj):
+class StreamCategory(APISubObj):
     """Category of a Rumble stream"""
 
     @property
     def slug(self):
         """Return the category's slug, AKA it's ID"""
         return self["slug"]
 
@@ -138,22 +170,22 @@
         if hasattr(other, "slug"):
             return self.slug == other.slug
 
     def __str__(self):
         """The category in string form"""
         return self.title
 
-class RumbleLivestream():
+class Livestream():
     """Rumble livestream"""
     def __init__(self, json, api):
         """Pass the JSON block of a single Rumble livestream"""
         self._json = json
         self.api = api
         self.is_disappeared = False #The livestream is in the API listing
-        self.__chat = RumbleLiveChat(self)
+        self.__chat = LiveChat(self)
 
     def __eq__(self, other):
         """Is this stream equal to another"""
         #Check if the compared string is our stream ID
         if isinstance(other, str):
             return self.stream_id == other #or self.title == other
 
@@ -187,25 +219,25 @@
     def stream_id(self):
         """The livestream ID"""
         return self["id"]
 
     @property
     def stream_id_b10(self):
         """The livestream chat ID (stream ID in base 10)"""
-        return stream_id_36_to_10(self.stream_id)
+        return utils.stream_id_36_to_10(self.stream_id)
 
     @property
     def title(self):
         """The title of the livestream"""
         return self["title"]
 
     @property
     def created_on(self):
         """When the livestream was created, in seconds since the Epock UTC"""
-        return parse_timestamp(self["created_on"])
+        return utils.parse_timestamp(self["created_on"])
 
     @property
     def is_live(self):
         """Is the stream live?"""
         return self["is_live"] and not self.is_disappeared
 
     @property
@@ -213,15 +245,15 @@
         """TODO"""
         return self["visibility"]
 
     @property
     def categories(self):
         """A list of our categories"""
         data = self["categories"].copy().values()
-        return [RumbleStreamCategory(json_block) for json_block in data]
+        return [StreamCategory(json_block) for json_block in data]
 
     @property
     def likes(self):
         """Number of likes on the stream"""
         return self["likes"]
 
     @property
@@ -243,15 +275,15 @@
         return self["watching_now"]
 
     @property
     def chat(self):
         """The livestream chat"""
         return self.__chat
 
-class RumbleChatMessage(RumbleUserAction):
+class ChatMessage(UserAction):
     """A single message in a Rumble livestream chat"""
     def __eq__(self, other):
         """Is this message equal to another"""
         #Check if the compared string is our message
         if isinstance(other, str):
             return self.text == other
 
@@ -275,22 +307,22 @@
     def text(self):
         """The message text"""
         return self["text"]
 
     @property
     def created_on(self):
         """When the message was created, in seconds since Epoch UTC"""
-        return parse_timestamp(self["created_on"])
+        return utils.parse_timestamp(self["created_on"])
 
     @property
     def badges(self):
         """The user's badges"""
         return tuple(self["badges"].values())
 
-class RumbleRant(RumbleChatMessage):
+class Rant(ChatMessage):
     """A single rant in a Rumble livestream chat"""
     def __eq__(self, other):
         """Is this category equal to another"""
         #Check if the compared string is our message
         if isinstance(other, str):
             return self.text == other
 
@@ -323,15 +355,15 @@
         return self["amount_cents"]
 
     @property
     def amount_dollars(self):
         """The rant amount in dollars"""
         return self["amount_dollars"]
 
-class RumbleLiveChat():
+class LiveChat():
     """Reference for chat of a Rumble livestream"""
     def __init__(self, stream):
         """Pass the JSON block of a single Rumble livestream"""
         self.stream = stream
         self.api = stream.api
         self.last_newmessage_time = 0 #Last time we were checked for "new" messages
         self.last_newrant_time = 0 #Last time we were checked for "new" rants
@@ -341,21 +373,21 @@
         return self.stream["chat"][key]
 
     @property
     def latest_message(self):
         """The latest chat message"""
         if not self["latest_message"]:
             return None #No-one has chatted on this stream yet
-        return RumbleChatMessage(self["latest_message"])
+        return ChatMessage(self["latest_message"])
 
     @property
     def recent_messages(self):
         """Recent chat messages"""
         data = self["recent_messages"].copy()
-        return [RumbleChatMessage(json_block) for json_block in data]
+        return [ChatMessage(json_block) for json_block in data]
 
     @property
     def new_messages(self):
         """Chat messages that are newer than the last time this was referenced"""
         rem = self.recent_messages.copy()
         rem.sort(key = lambda x: x.created_on) #Sort the messages so the newest ones are last
 
@@ -371,21 +403,21 @@
         return rem[i:]
 
     @property
     def latest_rant(self):
         """The latest chat rant"""
         if not self["latest_rant"]:
             return None #No-one has ranted on this stream yet
-        return RumbleRant(self["latest_rant"])
+        return Rant(self["latest_rant"])
 
     @property
     def recent_rants(self):
         """Recent chat rants"""
         data = self["recent_rants"].copy()
-        return [RumbleRant(json_block) for json_block in data]
+        return [Rant(json_block) for json_block in data]
 
     @property
     def new_rants(self):
         """Chat rants that are newer than the last time this was referenced"""
         rera = self.recent_rants.copy()
         rera.sort(key = lambda x: x.created_on) #Sort the rants so the newest ones are last
 
@@ -452,15 +484,15 @@
         #Update livestream references' JSONs in-place
         for json in self._json["livestreams"]:
             try:
                 #Update the JSON of the stored livestream
                 self.__livestreams[json["id"]]._json = json
 
             except KeyError: #The livestream has not been stored yet
-                self.__livestreams[json["id"]] = RumbleLivestream(json, self)
+                self.__livestreams[json["id"]] = Livestream(json, self)
 
     @property
     def api_type(self):
         """Type of API URL in use, user or channel"""
         return self["type"]
 
     @property
@@ -494,21 +526,21 @@
         return self["followers"]["num_followers_total"]
 
     @property
     def latest_follower(self):
         """The latest follower of this user or channel"""
         if not self["followers"]["latest_follower"]:
             return None #No-one has followed this user or channel yet
-        return RumbleFollower(self["followers"]["latest_follower"])
+        return Follower(self["followers"]["latest_follower"])
 
     @property
     def recent_followers(self):
         """A list (technically a shallow generator object) of recent followers"""
         data = self["followers"]["recent_followers"].copy()
-        return [RumbleFollower(json_block) for json_block in data]
+        return [Follower(json_block) for json_block in data]
 
     @property
     def num_subscribers(self):
         """The number of subscribers of this user or channel"""
         return self["subscribers"]["num_subscribers"]
 
     @property
@@ -517,21 +549,21 @@
         return self["subscribers"]["num_subscribers_total"]
 
     @property
     def latest_subscriber(self):
         """The latest subscriber of this user or channel"""
         if not self["subscribers"]["latest_subscriber"]:
             return None #No-one has subscribed to this user or channel yet
-        return RumbleSubscriber(self["subscribers"]["latest_subscriber"])
+        return Subscriber(self["subscribers"]["latest_subscriber"])
 
     @property
     def recent_subscribers(self):
         """A list (technically a shallow generator object) of recent subscribers"""
         data = self["subscribers"]["recent_subscribers"].copy()
-        return [RumbleSubscriber(json_block) for json_block in data]
+        return [Subscriber(json_block) for json_block in data]
 
     @property
     def livestreams(self):
         """A dictionairy of our livestreams"""
         self.check_refresh()
         return self.__livestreams
```

### Comparing `cocorum-0.4.0/src/cocorum/localvars.py` & `cocorum-0.5.0/src/cocorum/localvars.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 #!/usr/bin/env python3
 """Cocorum local variable definitions
 
+This submodule provides absolute variable definitions for Cocorum.
+
 S.D.G."""
 
 #Rumble timestamp format, not including the 6 TODO characters at the end
 TIMESTAMP_FORMAT = "%Y-%m-%dT%H:%M:%S"
 
 #Headers for the Rumble Live Stream API request (currently must fake a User-Agent string)
 HEADERS = {"User-Agent" : "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/51.0.2704.103 Safari/537.36"}
@@ -13,15 +15,15 @@
 STATIC_KEYS = [
     "user_id",
     "username",
     "channel_id",
     "channel_name",
     ]
 
-#Keys of the API JSON stream object that should not change unless the API URL changes, and so do not trigger a refresh
+#Keys of the API JSON stream object that should not trigger a refresh
 STATIC_KEYS_STREAM = [
     "id",
     "created_on"
     ]
 
 #API types, under JSON["type"]
 API_TYPE_USER = "user"
```

### Comparing `cocorum-0.4.0/src/cocorum/ssechat.py` & `cocorum-0.5.0/src/cocorum/ssechat.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,33 @@
 #!/usr/bin/env python3
-"""Rumble SSE chat display client
+"""SSE chat display client
 
+This part of cocorum is not part of the official Rumble Live Stream API, but may provide a more reliable method of ensuring all chat messages are received.
+
+Example usage:
+```
+from cocorum import ssechat
+
+chat = ssechat.SSEChat(stream_id = STREAM_ID) #Stream ID can be base 10 or 36
+chat.clear_mailbox() #Erase messages that were still visible before we connected
+
+msg = True
+while msg:
+    msg = chat.next_chat_message() #Hangs until a new message arrives
+    print(msg.user.username, ":", msg)
+
+print("Chat has closed.")
+```
 S.D.G."""
 
 import json #For parsing SSE message data
 import requests
 import sseclient
 from .localvars import *
-from .utils import *
+from . import utils
 
 class SSEChatObject():
     """Object in SSE chat API"""
     def __init__(self, jsondata, chat):
         """Pass the object JSON, and the parent SSEChat object"""
         self._jsondata = jsondata
         self.chat = chat
@@ -213,15 +229,15 @@
     def message_id(self):
         """The unique numerical ID of the chat message"""
         return self["id"]
 
     @property
     def time(self):
         """The time the message was sent on, in seconds since the Epoch UTC"""
-        return parse_timestamp(self["time"])
+        return utils.parse_timestamp(self["time"])
 
     @property
     def user_id(self):
         """The numerical ID of the user who posted the message"""
         return self["user_id"]
 
     @property
@@ -270,22 +286,22 @@
         return self["rant"]["duration"]
 
     @property
     def rant_expires_on(self):
         """When the rant expires, returns message creation time if message is not a rant"""
         if not self.is_rant:
             return self.time
-        return parse_timestamp(self["rant"]["expires_on"])
+        return utils.parse_timestamp(self["rant"]["expires_on"])
 
-class SSEChatAPI():
+class SSEChat():
     """Access the Rumble SSE chat api"""
     def __init__(self, stream_id):
-        self.stream_id = stream_id_ensure_b36(stream_id)
+        self.stream_id = utils.stream_id_ensure_b36(stream_id)
 
-        self.mailbox = [] #A mailbox if you will
+        self.__mailbox = [] #A mailbox if you will
         self.users = {} #Dictionary of users by user ID
         self.channels = {} #Dictionary of channels by channel ID
         self.badges = {}
 
         #Connect to the API
         self.url = SSE_CHAT_URL.format(stream_id_b10 = self.stream_id_b10)
         self.client = sseclient.SSEClient(self.url)
@@ -323,15 +339,19 @@
         self.rants_enabled = jsondata["data"]["config"]["rants"]["enable"]
         #subscription TODO
         #rant levels TODO
         self.message_length_max = jsondata["data"]["config"]["message_length_max"]
 
     def update_mailbox(self, jsondata):
         """Parse chat messages from an SSE data JSON"""
-        self.mailbox += [SSEChatMessage(message_json, self) for message_json in jsondata["data"]["messages"]]
+        self.__mailbox += [SSEChatMessage(message_json, self) for message_json in jsondata["data"]["messages"]]
+
+    def clear_mailbox(self):
+        """Delete anything in the mailbox"""
+        self.__mailbox = []
 
     def update_users(self, jsondata):
         """Update our dictionary of users from an SSE data JSON"""
         for user_json in jsondata["data"]["users"]:
             try:
                 self.users[user_json["id"]]._jsondata = user_json #Update an existing user's JSON
             except KeyError: #User is new
@@ -348,24 +368,24 @@
     def load_badges(self, jsondata):
         """Create our dictionary of badges given a dictionary of badges"""
         self.badges = {badge_slug : SSEChatUserBadge(badge_slug, jsondata["data"]["config"]["badges"][badge_slug], self) for badge_slug in jsondata["data"]["config"]["badges"].keys()}
 
     @property
     def stream_id_b10(self):
         """The chat ID in user"""
-        return stream_id_36_to_10(self.stream_id)
+        return utils.stream_id_36_to_10(self.stream_id)
 
     def next_chat_message(self):
         """Return the next chat message (parsing any additional data), waits for it to come in, returns None if chat closed"""
-        if not self.mailbox: #We don't already have messages
+        if not self.__mailbox: #We don't already have messages
             jsondata = self.next_jsondata()
             if not jsondata: #The chat has closed or a blank event
                 return
             if jsondata["type"] != "messages":
                 raise ValueError("API did not send a messages message")
 
             #Parse messages, users, and channels
             self.update_mailbox(jsondata)
             self.update_users(jsondata)
             self.update_channels(jsondata)
 
-        return self.mailbox.pop(0) #Return the first message in the mailbox, and then remove it from there
+        return self.__mailbox.pop(0) #Return the first message in the mailbox, and then remove it from there
```

### Comparing `cocorum-0.4.0/src/cocorum/utils.py` & `cocorum-0.5.0/src/cocorum/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 #!/usr/bin/env python3
 """Rumble API utilities
 
+This submodule provides some utilities for working with the APIs:
+- Timestamp parsing
+- Converting stream IDs from base 36 to base 10 and vice versa
+- Ensuring a stream ID is one of those two bases, converting if necessary
+
 S.D.G."""
 
 import calendar
 import time
 from .localvars import *
 
 def parse_timestamp(timestamp):
```

### Comparing `cocorum-0.4.0/LICENSE.txt` & `cocorum-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cocorum-0.4.0/README.md` & `cocorum-0.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <h1><img src="cocorum_icon.png" alt="" width="64"/> Cocorum: Rumble Live Stream API Python Wrapper</h1>
-A Python wrapper for the Rumble Live Stream API v1.0 (beta), with some quality of live additions, such as:
+A Python wrapper for the Rumble Live Stream API v1.0 (beta), with some quality of life additions, such as:
 - Automatic refresh when past the refresh_rate delay when querying any non_static property.
 - All timespamps are parsed to seconds since Epoch, UTC timezone.
 - Chat has new_messages and new_rants properties that return only messages and rants since the last time they were read.
 
 ## Usage:
-I tried to document the wrapper well, so the help function should work. Note, you are only expected to create a RumbleAPI object, and work with everything through that.
+I tried to document the wrapper well, so help("cocorum") should work. Note, you are only expected to create a RumbleAPI() and / or ssechat.SSEChat() object, and work with everything through them.
 
 Most attributes that are not added features have the same name as the direct JSON counterparts, with the exception of adding prefixes to some things that have the same name in the JSON as Python builtin functions. For example, thing/id in JSON is thing.thing_id in this Python wrapper.
 
 ```
 from cocorum import RumbleAPI
 from cocorum.localvars import *
 
@@ -35,15 +35,15 @@
 ## Experimental SSE chat submodule
 This part of cocorum is not part of the official Rumble Live Stream API, but may provide a more reliable method of ensuring all chat messages are received.
 
 ```
 from cocorum import ssechat
 
 chat = ssechat.SSEChat(stream_id = STREAM_ID) #Stream ID can be base 10 or 36
-#Do chat.mailbox = [] here to erase messages that were still visible before we connected
+chat.clear_mailbox() #Erase messages that were still visible before we connected
 
 msg = True
 while msg:
     msg = chat.next_chat_message() #Hangs until a new message arrives
     print(msg.user.username, ":", msg)
 
 print("Chat has closed.")
```

### Comparing `cocorum-0.4.0/pyproject.toml` & `cocorum-0.5.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cocorum"
-version = "0.4.0"
+version = "0.5.0"
 keywords = ["rumble", "api", "wrapper", "livestream"]
 authors = [
   { name="Wilbur Jaywright", email="zargulthewizard@outlook.com" },
 ]
 description = "An unofficial Python wrapper for the Rumble Live Stream API v1.0 (beta)"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `cocorum-0.4.0/PKG-INFO` & `cocorum-0.5.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cocorum
-Version: 0.4.0
+Version: 0.5.0
 Summary: An unofficial Python wrapper for the Rumble Live Stream API v1.0 (beta)
 Project-URL: Homepage, https://github.com/thelabcat/rumble-api-wrapper-py
 Project-URL: Issues, https://github.com/thelabcat/rumble-api-wrapper-py/issues
 Project-URL: Rumble Live Stream API docs, https://rumblefaq.groovehq.com/help/how-to-use-rumble-s-live-stream-api
 Author-email: Wilbur Jaywright <zargulthewizard@outlook.com>
 License-File: LICENSE.txt
 Keywords: api,livestream,rumble,wrapper
@@ -14,21 +14,21 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: requests
 Requires-Dist: sseclient
 Description-Content-Type: text/markdown
 
 <h1><img src="cocorum_icon.png" alt="" width="64"/> Cocorum: Rumble Live Stream API Python Wrapper</h1>
-A Python wrapper for the Rumble Live Stream API v1.0 (beta), with some quality of live additions, such as:
+A Python wrapper for the Rumble Live Stream API v1.0 (beta), with some quality of life additions, such as:
 - Automatic refresh when past the refresh_rate delay when querying any non_static property.
 - All timespamps are parsed to seconds since Epoch, UTC timezone.
 - Chat has new_messages and new_rants properties that return only messages and rants since the last time they were read.
 
 ## Usage:
-I tried to document the wrapper well, so the help function should work. Note, you are only expected to create a RumbleAPI object, and work with everything through that.
+I tried to document the wrapper well, so help("cocorum") should work. Note, you are only expected to create a RumbleAPI() and / or ssechat.SSEChat() object, and work with everything through them.
 
 Most attributes that are not added features have the same name as the direct JSON counterparts, with the exception of adding prefixes to some things that have the same name in the JSON as Python builtin functions. For example, thing/id in JSON is thing.thing_id in this Python wrapper.
 
 ```
 from cocorum import RumbleAPI
 from cocorum.localvars import *
 
@@ -54,15 +54,15 @@
 ## Experimental SSE chat submodule
 This part of cocorum is not part of the official Rumble Live Stream API, but may provide a more reliable method of ensuring all chat messages are received.
 
 ```
 from cocorum import ssechat
 
 chat = ssechat.SSEChat(stream_id = STREAM_ID) #Stream ID can be base 10 or 36
-#Do chat.mailbox = [] here to erase messages that were still visible before we connected
+chat.clear_mailbox() #Erase messages that were still visible before we connected
 
 msg = True
 while msg:
     msg = chat.next_chat_message() #Hangs until a new message arrives
     print(msg.user.username, ":", msg)
 
 print("Chat has closed.")
```


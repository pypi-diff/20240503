# Comparing `tmp/cocorum-0.3.0.tar.gz` & `tmp/cocorum-0.4.0.tar.gz`

## Comparing `cocorum-0.3.0.tar` & `cocorum-0.4.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 cocorum-0.3.0/requirements.txt
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 cocorum-0.3.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0    18392 2020-02-02 00:00:00.000000 cocorum-0.3.0/src/cocorum/__init__.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 cocorum-0.3.0/src/cocorum/localvars.py
--rw-r--r--   0        0        0    13714 2020-02-02 00:00:00.000000 cocorum-0.3.0/src/cocorum/ssechat.py
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 cocorum-0.3.0/src/cocorum/utils.py
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 cocorum-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 cocorum-0.3.0/README.md
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 cocorum-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 cocorum-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0   343002 2020-02-02 00:00:00.000000 cocorum-0.4.0/cocorum_icon.png
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 cocorum-0.4.0/requirements.txt
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 cocorum-0.4.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0    18441 2020-02-02 00:00:00.000000 cocorum-0.4.0/src/cocorum/__init__.py
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 cocorum-0.4.0/src/cocorum/localvars.py
+-rw-r--r--   0        0        0    13155 2020-02-02 00:00:00.000000 cocorum-0.4.0/src/cocorum/ssechat.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 cocorum-0.4.0/src/cocorum/utils.py
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 cocorum-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 cocorum-0.4.0/README.md
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 cocorum-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 cocorum-0.4.0/PKG-INFO
```

### Comparing `cocorum-0.3.0/.github/workflows/python-publish.yml` & `cocorum-0.4.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `cocorum-0.3.0/src/cocorum/__init__.py` & `cocorum-0.4.0/src/cocorum/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,18 +54,18 @@
     @property
     def profile_pic(self):
         """The user's profile picture as a bytes string"""
         if not self.profile_pic_url: #The profile picture is blank
             return b''
 
         if not self.__profile_pic: #We never queried the profile pic before
-            response = requests.get(self.profile_pic_url)
+            #TODO make this timeout assignable
+            response = requests.get(self.profile_pic_url, DEFAULT_TIMEOUT)
             if response.status_code != 200:
-                #TODO make this timeout assignable
-                raise Exception("Status code " + str(response.status_code), DEFAULT_TIMEOUT)
+                raise Exception("Status code " + str(response.status_code))
 
             self.__profile_pic = response.content
 
         return self.__profile_pic
 
 class RumbleFollower(RumbleUserAction):
     """Rumble follower"""
@@ -86,15 +86,15 @@
         if isinstance(other, (int, float)):
             return self.amount_cents == other
 
         #Check if the compared object's username matches our own, if it has one
         if hasattr(other, "username"):
             #Check if the compared object's cost amout matches our own, if it has one
             if hasattr(other, "amount_cents"):
-                self.amount_cents == other.amount_cents
+                return self.amount_cents == other.amount_cents
 
             #Other object has no amount_cents attribute
             return self.username == other.username
 
     @property
     def user(self):
         """AFAIK this is being deprecated, use username instead"""
@@ -155,23 +155,23 @@
         """Is this stream equal to another"""
         #Check if the compared string is our stream ID
         if isinstance(other, str):
             return self.stream_id == other #or self.title == other
 
         #check if the compared number is our chat ID (linked to stream ID)
         if isinstance(other, (int, float)):
-            return self.chat_id == other
+            return self.stream_id_b10 == other
 
         #Check if the compared object has the same stream ID
         if hasattr(other, "stream_id"):
             return self.stream_id == other.stream_id
 
         #Check if the compared object has the same chat ID
-        if hasattr(other, "chat_id"):
-            return self.stream_id == other.chat_id
+        if hasattr(other, "stream_id_b10"):
+            return self.stream_id_b10 == other.stream_id_b10
 
     def __str__(self):
         """The livestream in string form"""
         return self.stream_id
 
     def __getitem__(self, key):
         """Return a key from the JSON, refreshing if necessary"""
@@ -185,17 +185,17 @@
 
     @property
     def stream_id(self):
         """The livestream ID"""
         return self["id"]
 
     @property
-    def chat_id(self):
-        """The livestream chat ID"""
-        return id_stream_to_chat(self.stream_id)
+    def stream_id_b10(self):
+        """The livestream chat ID (stream ID in base 10)"""
+        return stream_id_36_to_10(self.stream_id)
 
     @property
     def title(self):
         """The title of the livestream"""
         return self["title"]
 
     @property
@@ -334,15 +334,15 @@
         self.stream = stream
         self.api = stream.api
         self.last_newmessage_time = 0 #Last time we were checked for "new" messages
         self.last_newrant_time = 0 #Last time we were checked for "new" rants
 
     def __getitem__(self, key):
         """Return a key from the stream's chat JSON"""
-        return self.stream._json["chat"][key]
+        return self.stream["chat"][key]
 
     @property
     def latest_message(self):
         """The latest chat message"""
         if not self["latest_message"]:
             return None #No-one has chatted on this stream yet
         return RumbleChatMessage(self["latest_message"])
```

### Comparing `cocorum-0.3.0/src/cocorum/localvars.py` & `cocorum-0.4.0/src/cocorum/localvars.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,16 +34,16 @@
 
 #Base URL to Rumble's website, for URLs that are relative to it
 RUMBLE_BASE_URL = "https://rumble.com"
 
 #Numerical base that the stream ID is in
 STREAM_ID_BASE = "0123456789abcdefghijklmnopqrstuvwxyz"
 
-#Rumble's SSE chat display URL for a stream, format this string with a chat_id
-SSE_CHAT_URL = "https://web7.rumble.com/chat/api/chat/{chat_id}/stream"
+#Rumble's SSE chat display URL for a stream, format this string with a stream_id_b10
+SSE_CHAT_URL = "https://web7.rumble.com/chat/api/chat/{stream_id_b10}/stream"
 
 #Size of chat badge icons to retrieve, only valid one has long been the string 48
 BADGE_ICON_SIZE = "48"
 
 #How long to wait before giving up on a network request, in seconds
 DEFAULT_TIMEOUT = 20
```

### Comparing `cocorum-0.3.0/src/cocorum/ssechat.py` & `cocorum-0.4.0/src/cocorum/ssechat.py`

 * *Files 4% similar despite different names*

```diff
@@ -274,33 +274,24 @@
         """When the rant expires, returns message creation time if message is not a rant"""
         if not self.is_rant:
             return self.time
         return parse_timestamp(self["rant"]["expires_on"])
 
 class SSEChatAPI():
     """Access the Rumble SSE chat api"""
-    def __init__(self, chat_id = None, stream_id = None):
-        if stream_id: #Stream ID as provided by the API
-            self.chat_id = id_stream_to_chat(stream_id)
-            if chat_id and self.chat_id != chat_id:
-                raise ValueError("Stream ID and chat ID were both specified but they do not match")
-        elif chat_id: #Chat ID as it appears in the popout URL
-            self.chat_id = chat_id
-        else:
-            raise ValueError("Must specify either stream_id or chat_id")
-
-        self.__stream_id = stream_id
+    def __init__(self, stream_id):
+        self.stream_id = stream_id_ensure_b36(stream_id)
 
         self.mailbox = [] #A mailbox if you will
         self.users = {} #Dictionary of users by user ID
         self.channels = {} #Dictionary of channels by channel ID
         self.badges = {}
 
         #Connect to the API
-        self.url = SSE_CHAT_URL.format(chat_id = self.chat_id)
+        self.url = SSE_CHAT_URL.format(stream_id_b10 = self.stream_id_b10)
         self.client = sseclient.SSEClient(self.url)
         self.chat_running = True
         self.parse_init_data(self.next_jsondata())
 
     def next_jsondata(self):
         """Wait for the next message from the SSE and parse the JSON"""
         if not self.chat_running: #Do not try to query a new message if chat is closed
@@ -355,20 +346,17 @@
                 self.channels.update({channel_json["id"] : SSEChatChannel(channel_json, self)})
 
     def load_badges(self, jsondata):
         """Create our dictionary of badges given a dictionary of badges"""
         self.badges = {badge_slug : SSEChatUserBadge(badge_slug, jsondata["data"]["config"]["badges"][badge_slug], self) for badge_slug in jsondata["data"]["config"]["badges"].keys()}
 
     @property
-    def stream_id(self):
-        """If we don't know our stream ID, figure it out from the chat ID"""
-        if not self.__stream_id:
-            self.__stream_id = id_chat_to_stream(self.chat_id)
-
-        return self.__stream_id
+    def stream_id_b10(self):
+        """The chat ID in user"""
+        return stream_id_36_to_10(self.stream_id)
 
     def next_chat_message(self):
         """Return the next chat message (parsing any additional data), waits for it to come in, returns None if chat closed"""
         if not self.mailbox: #We don't already have messages
             jsondata = self.next_jsondata()
             if not jsondata: #The chat has closed or a blank event
                 return
```

### Comparing `cocorum-0.3.0/LICENSE.txt` & `cocorum-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cocorum-0.3.0/README.md` & `cocorum-0.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Cocorum: Rumble Live Stream API Python Wrapper
+<h1><img src="cocorum_icon.png" alt="" width="64"/> Cocorum: Rumble Live Stream API Python Wrapper</h1>
 A Python wrapper for the Rumble Live Stream API v1.0 (beta), with some quality of live additions, such as:
 - Automatic refresh when past the refresh_rate delay when querying any non_static property.
 - All timespamps are parsed to seconds since Epoch, UTC timezone.
 - Chat has new_messages and new_rants properties that return only messages and rants since the last time they were read.
 
 ## Usage:
 I tried to document the wrapper well, so the help function should work. Note, you are only expected to create a RumbleAPI object, and work with everything through that.
@@ -29,20 +29,20 @@
         print("Stream is not public.")
     message = livestream.chat.latest_message #None if there are no messages yet
     if message:
         print(message.username, "said", message)
 ```
 
 ## Experimental SSE chat submodule
-This part of cocorum is not part of the official Rumble Livestream API, but may provide a more reliable method of ensuring all chat messages are received.
+This part of cocorum is not part of the official Rumble Live Stream API, but may provide a more reliable method of ensuring all chat messages are received.
 
 ```
 from cocorum import ssechat
 
-chat = ssechat.SSEChat(chat_id = CHAT_ID)
+chat = ssechat.SSEChat(stream_id = STREAM_ID) #Stream ID can be base 10 or 36
 #Do chat.mailbox = [] here to erase messages that were still visible before we connected
 
 msg = True
 while msg:
     msg = chat.next_chat_message() #Hangs until a new message arrives
     print(msg.user.username, ":", msg)
```

### Comparing `cocorum-0.3.0/pyproject.toml` & `cocorum-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cocorum"
-version = "0.3.0"
+version = "0.4.0"
 keywords = ["rumble", "api", "wrapper", "livestream"]
 authors = [
   { name="Wilbur Jaywright", email="zargulthewizard@outlook.com" },
 ]
 description = "An unofficial Python wrapper for the Rumble Live Stream API v1.0 (beta)"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `cocorum-0.3.0/PKG-INFO` & `cocorum-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cocorum
-Version: 0.3.0
+Version: 0.4.0
 Summary: An unofficial Python wrapper for the Rumble Live Stream API v1.0 (beta)
 Project-URL: Homepage, https://github.com/thelabcat/rumble-api-wrapper-py
 Project-URL: Issues, https://github.com/thelabcat/rumble-api-wrapper-py/issues
 Project-URL: Rumble Live Stream API docs, https://rumblefaq.groovehq.com/help/how-to-use-rumble-s-live-stream-api
 Author-email: Wilbur Jaywright <zargulthewizard@outlook.com>
 License-File: LICENSE.txt
 Keywords: api,livestream,rumble,wrapper
@@ -13,15 +13,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: requests
 Requires-Dist: sseclient
 Description-Content-Type: text/markdown
 
-# Cocorum: Rumble Live Stream API Python Wrapper
+<h1><img src="cocorum_icon.png" alt="" width="64"/> Cocorum: Rumble Live Stream API Python Wrapper</h1>
 A Python wrapper for the Rumble Live Stream API v1.0 (beta), with some quality of live additions, such as:
 - Automatic refresh when past the refresh_rate delay when querying any non_static property.
 - All timespamps are parsed to seconds since Epoch, UTC timezone.
 - Chat has new_messages and new_rants properties that return only messages and rants since the last time they were read.
 
 ## Usage:
 I tried to document the wrapper well, so the help function should work. Note, you are only expected to create a RumbleAPI object, and work with everything through that.
@@ -48,20 +48,20 @@
         print("Stream is not public.")
     message = livestream.chat.latest_message #None if there are no messages yet
     if message:
         print(message.username, "said", message)
 ```
 
 ## Experimental SSE chat submodule
-This part of cocorum is not part of the official Rumble Livestream API, but may provide a more reliable method of ensuring all chat messages are received.
+This part of cocorum is not part of the official Rumble Live Stream API, but may provide a more reliable method of ensuring all chat messages are received.
 
 ```
 from cocorum import ssechat
 
-chat = ssechat.SSEChat(chat_id = CHAT_ID)
+chat = ssechat.SSEChat(stream_id = STREAM_ID) #Stream ID can be base 10 or 36
 #Do chat.mailbox = [] here to erase messages that were still visible before we connected
 
 msg = True
 while msg:
     msg = chat.next_chat_message() #Hangs until a new message arrives
     print(msg.user.username, ":", msg)
```


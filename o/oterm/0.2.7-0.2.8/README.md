# Comparing `tmp/oterm-0.2.7.tar.gz` & `tmp/oterm-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oterm-0.2.7.tar", max compression
+gzip compressed data, was "oterm-0.2.8.tar", max compression
```

## Comparing `oterm-0.2.7.tar` & `oterm-0.2.8.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0     1064 2024-04-22 06:47:10.868047 oterm-0.2.7/LICENSE
--rw-r--r--   0        0        0     3798 2024-04-22 06:47:10.868047 oterm-0.2.7/README.md
--rw-r--r--   0        0        0        0 2024-04-22 06:47:10.868047 oterm-0.2.7/oterm/__init__.py
--rw-r--r--   0        0        0        0 2024-04-22 06:47:10.868047 oterm-0.2.7/oterm/app/__init__.py
--rw-r--r--   0        0        0     7156 2024-04-22 06:47:10.868047 oterm-0.2.7/oterm/app/chat_edit.py
--rw-r--r--   0        0        0     1593 2024-04-22 06:47:10.868047 oterm-0.2.7/oterm/app/chat_export.py
--rw-r--r--   0        0        0      734 2024-04-22 06:47:10.868047 oterm-0.2.7/oterm/app/chat_rename.py
--rw-r--r--   0        0        0     2313 2024-04-22 06:47:10.868047 oterm-0.2.7/oterm/app/image_browser.py
--rw-r--r--   0        0        0     3244 2024-04-22 06:47:10.868047 oterm-0.2.7/oterm/app/oterm.py
--rw-r--r--   0        0        0     3239 2024-04-22 06:47:10.868047 oterm-0.2.7/oterm/app/oterm.tcss
--rw-r--r--   0        0        0     1058 2024-04-22 06:47:10.872047 oterm-0.2.7/oterm/app/prompt_history.py
--rw-r--r--   0        0        0     1947 2024-04-22 06:47:10.872047 oterm-0.2.7/oterm/app/splash.py
--rw-r--r--   0        0        0       46 2024-04-22 06:47:10.872047 oterm-0.2.7/oterm/app/widgets/__init__.py
--rw-r--r--   0        0        0     9680 2024-04-22 06:47:10.872047 oterm-0.2.7/oterm/app/widgets/chat.py
--rw-r--r--   0        0        0     1823 2024-04-22 06:47:10.872047 oterm-0.2.7/oterm/app/widgets/image.py
--rw-r--r--   0        0        0      627 2024-04-22 06:47:10.872047 oterm-0.2.7/oterm/app/widgets/monkey.py
--rw-r--r--   0        0        0     5569 2024-04-22 06:47:10.872047 oterm-0.2.7/oterm/app/widgets/prompt.py
--rw-r--r--   0        0        0      879 2024-04-22 06:47:10.872047 oterm-0.2.7/oterm/app/widgets/text_area.py
--rw-r--r--   0        0        0        0 2024-04-22 06:47:10.872047 oterm-0.2.7/oterm/cli/__init__.py
--rw-r--r--   0        0        0      724 2024-04-22 06:47:10.872047 oterm-0.2.7/oterm/cli/oterm.py
--rw-r--r--   0        0        0     3131 2024-04-22 06:47:10.872047 oterm-0.2.7/oterm/config.py
--rw-r--r--   0        0        0     2181 2024-04-22 06:47:10.872047 oterm-0.2.7/oterm/ollama.py
--rw-r--r--   0        0        0        0 2024-04-22 06:47:10.872047 oterm-0.2.7/oterm/store/__init__.py
--rw-r--r--   0        0        0      892 2024-04-22 06:47:10.872047 oterm-0.2.7/oterm/store/chat.py
--rw-r--r--   0        0        0      572 2024-04-22 06:47:10.872047 oterm-0.2.7/oterm/store/setup.py
--rw-r--r--   0        0        0     5769 2024-04-22 06:47:10.872047 oterm-0.2.7/oterm/store/store.py
--rw-r--r--   0        0        0      359 2024-04-22 06:47:10.872047 oterm-0.2.7/oterm/store/upgrades/__init__.py
--rw-r--r--   0        0        0      574 2024-04-22 06:47:10.872047 oterm-0.2.7/oterm/store/upgrades/v0_1_11.py
--rw-r--r--   0        0        0      514 2024-04-22 06:47:10.872047 oterm-0.2.7/oterm/store/upgrades/v0_1_6.py
--rw-r--r--   0        0        0      522 2024-04-22 06:47:10.872047 oterm-0.2.7/oterm/store/upgrades/v0_2_0.py
--rw-r--r--   0        0        0      533 2024-04-22 06:47:10.872047 oterm-0.2.7/oterm/store/upgrades/v0_2_4.py
--rw-r--r--   0        0        0     1408 2024-04-22 06:47:10.872047 oterm-0.2.7/oterm/utils.py
--rw-r--r--   0        0        0     2040 2024-04-22 06:47:10.872047 oterm-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     5242 1970-01-01 00:00:00.000000 oterm-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-03 12:41:59.688509 oterm-0.2.8/LICENSE
+-rw-r--r--   0        0        0     3798 2024-05-03 12:41:59.688509 oterm-0.2.8/README.md
+-rw-r--r--   0        0        0        0 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/app/__init__.py
+-rw-r--r--   0        0        0     7948 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/app/chat_edit.py
+-rw-r--r--   0        0        0     1593 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/app/chat_export.py
+-rw-r--r--   0        0        0      734 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/app/chat_rename.py
+-rw-r--r--   0        0        0     2313 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/app/image_browser.py
+-rw-r--r--   0        0        0     3428 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/app/oterm.py
+-rw-r--r--   0        0        0     3323 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/app/oterm.tcss
+-rw-r--r--   0        0        0     1058 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/app/prompt_history.py
+-rw-r--r--   0        0        0     1947 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/app/splash.py
+-rw-r--r--   0        0        0       46 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/app/widgets/__init__.py
+-rw-r--r--   0        0        0    10087 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/app/widgets/chat.py
+-rw-r--r--   0        0        0     1823 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/app/widgets/image.py
+-rw-r--r--   0        0        0      627 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/app/widgets/monkey.py
+-rw-r--r--   0        0        0     5569 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/app/widgets/prompt.py
+-rw-r--r--   0        0        0      879 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/app/widgets/text_area.py
+-rw-r--r--   0        0        0        0 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/cli/__init__.py
+-rw-r--r--   0        0        0      724 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/cli/oterm.py
+-rw-r--r--   0        0        0     3131 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/config.py
+-rw-r--r--   0        0        0     2295 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/ollama.py
+-rw-r--r--   0        0        0        0 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/store/__init__.py
+-rw-r--r--   0        0        0      967 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/store/chat.py
+-rw-r--r--   0        0        0      608 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/store/setup.py
+-rw-r--r--   0        0        0     5988 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/store/store.py
+-rw-r--r--   0        0        0      469 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/store/upgrades/__init__.py
+-rw-r--r--   0        0        0      574 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/store/upgrades/v0_1_11.py
+-rw-r--r--   0        0        0      514 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/store/upgrades/v0_1_6.py
+-rw-r--r--   0        0        0      522 2024-05-03 12:41:59.688509 oterm-0.2.8/oterm/store/upgrades/v0_2_0.py
+-rw-r--r--   0        0        0      533 2024-05-03 12:41:59.692510 oterm-0.2.8/oterm/store/upgrades/v0_2_4.py
+-rw-r--r--   0        0        0      535 2024-05-03 12:41:59.692510 oterm-0.2.8/oterm/store/upgrades/v0_2_8.py
+-rw-r--r--   0        0        0     1408 2024-05-03 12:41:59.692510 oterm-0.2.8/oterm/utils.py
+-rw-r--r--   0        0        0     2040 2024-05-03 12:41:59.692510 oterm-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     5242 1970-01-01 00:00:00.000000 oterm-0.2.8/PKG-INFO
```

### Comparing `oterm-0.2.7/LICENSE` & `oterm-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `oterm-0.2.7/README.md` & `oterm-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `oterm-0.2.7/oterm/app/chat_edit.py` & `oterm-0.2.8/oterm/app/chat_edit.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from rich.text import Text
 from textual.app import ComposeResult
 from textual.containers import Container, Horizontal, Vertical
 from textual.css.query import NoMatches
 from textual.reactive import reactive
 from textual.screen import ModalScreen
-from textual.widgets import Button, Checkbox, Label, OptionList, Pretty
+from textual.widgets import Button, Checkbox, Input, Label, OptionList, Pretty
 
 from oterm.app.widgets.text_area import TextArea
 from oterm.ollama import OllamaLLM
 
 
 class ChatEdit(ModalScreen[str]):
     models = []
@@ -23,30 +23,33 @@
     bytes: reactive[int] = reactive(0)
     model_info: dict[str, str] = {}
     system: reactive[str] = reactive("")
     params: reactive[list[tuple[str, str]]] = reactive([])
     json_format: reactive[bool] = reactive(False)
     edit_mode: reactive[bool] = reactive(False)
     last_highlighted_index = None
+    keep_alive: reactive[int] = reactive(5)
 
     BINDINGS = [
         ("escape", "cancel", "Cancel"),
         ("enter", "save", "Save"),
     ]
 
     def _return_chat_meta(self) -> None:
         model = f"{self.model_name}:{self.tag}"
         system = self.query_one(".system", TextArea).text
         system = system if system != self.model_info.get("system", "") else None
         jsn = self.query_one(".json-format", Checkbox).value
+        keep_alive = int(self.query_one(".keep-alive", Input).value)
         result = json.dumps(
             {
                 "name": model,
                 "system": system,
                 "format": "json" if jsn else "",
+                "keep_alive": keep_alive,
             }
         )
         self.dismiss(result)
 
     def _parse_model_params(self, parameter_text: str) -> list[tuple[str, Any]]:
         lines = parameter_text.split("\n")
         params = []
@@ -160,14 +163,21 @@
     def watch_json_format(self, jsn: bool) -> None:
         try:
             widget = self.query_one(".json-format", Checkbox)
             widget.value = jsn
         except NoMatches:
             pass
 
+    def watch_keep_alive(self, keep_alive: int) -> None:
+        try:
+            widget = self.query_one(".keep-alive", Input)
+            widget.value = str(keep_alive)
+        except NoMatches:
+            pass
+
     def watch_edit_mode(self, edit_mode: bool) -> None:
         try:
             widget = self.query_one("#model-select", OptionList)
             widget.disabled = edit_mode
         except NoMatches:
             pass
 
@@ -183,16 +193,26 @@
                         yield Label("", classes="tag")
                         yield Label("", classes="size")
                 with Vertical():
                     yield Label("System:", classes="title")
                     yield TextArea("", classes="system log")
                     yield Label("Parameters:", classes="title")
                     yield Pretty("", classes="parameters")
-                    yield Label("Format", classes="title")
-                    yield Checkbox("JSON output", value=False, classes="json-format")
+                    with Horizontal():
+                        yield Checkbox(
+                            "JSON output",
+                            value=False,
+                            classes="json-format",
+                            button_first=False,
+                        )
+                        with Horizontal():
+                            yield Label(
+                                "Keep-alive (min)", classes="title keep-alive-label"
+                            )
+                            yield Input(classes="keep-alive", value="5")
 
             with Horizontal(classes="button-container"):
                 yield Button(
                     "Save",
                     id="save-btn",
                     name="save",
                     disabled=True,
```

### Comparing `oterm-0.2.7/oterm/app/chat_export.py` & `oterm-0.2.8/oterm/app/chat_export.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.7/oterm/app/chat_rename.py` & `oterm-0.2.8/oterm/app/chat_rename.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.7/oterm/app/image_browser.py` & `oterm-0.2.8/oterm/app/image_browser.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.7/oterm/app/oterm.py` & `oterm-0.2.8/oterm/app/oterm.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,33 +27,36 @@
 
     async def action_quit(self) -> None:
         return self.exit()
 
     def action_new_chat(self) -> None:
         async def on_model_select(model_info: str) -> None:
             model: dict = json.loads(model_info)
+            print(model)
             tabs = self.query_one(TabbedContent)
             tab_count = tabs.tab_count
             name = f"chat #{tab_count+1} - {model['name']}"
             id = await self.store.save_chat(
                 id=None,
                 name=name,
                 model=model["name"],
                 context="[]",
                 system=model["system"],
                 format=model["format"],
+                keep_alive=model["keep_alive"],
             )
             pane = TabPane(name, id=f"chat-{id}")
             pane.compose_add_child(
                 ChatContainer(
                     db_id=id,
                     chat_name=name,
                     model=model["name"],
                     system=model["system"],
                     format=model["format"],
+                    keep_alive=model["keep_alive"],
                     messages=[],
                 )
             )
             await tabs.add_pane(pane)
             tabs.active = f"chat-{id}"
 
         self.push_screen(ChatEdit(), on_model_select)
@@ -62,26 +65,27 @@
         self.store = await Store.create()
         self.dark = appConfig.get("theme") == "dark"
         saved_chats = await self.store.get_chats()  # type: ignore
         if not saved_chats:
             self.action_new_chat()
         else:
             tabs = self.query_one(TabbedContent)
-            for id, name, model, context, system, format in saved_chats:
+            for id, name, model, context, system, format, keep_alive in saved_chats:
                 messages = await self.store.get_messages(id)
                 pane = TabPane(name, id=f"chat-{id}")
                 await pane.mount(
                     ChatContainer(
                         db_id=id,
                         chat_name=name,
                         model=model,
                         context=context,
                         messages=messages,  # type: ignore
                         system=system,
                         format=format,
+                        keep_alive=keep_alive,
                     )
                 )
                 tabs.add_pane(pane)
         await self.push_screen(SplashScreen())
 
     @on(TabbedContent.TabActivated)
     async def on_tab_activated(self, event: TabbedContent.TabActivated) -> None:
```

### Comparing `oterm-0.2.7/oterm/app/oterm.tcss` & `oterm-0.2.8/oterm/app/oterm.tcss`

 * *Files 3% similar despite different names*

```diff
@@ -211,8 +211,16 @@
 
 MarkdownFence {
     max-height: 50;
 }
 
 Button.icon {
     min-width: 5;
+}
+
+Input.keep-alive {
+    width: 10;
+}
+
+Label.keep-alive-label {
+    margin-top: 1;
 }
```

### Comparing `oterm-0.2.7/oterm/app/prompt_history.py` & `oterm-0.2.8/oterm/app/prompt_history.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.7/oterm/app/splash.py` & `oterm-0.2.8/oterm/app/splash.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.7/oterm/app/widgets/chat.py` & `oterm-0.2.8/oterm/app/widgets/chat.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 
 class ChatContainer(Widget):
     ollama = OllamaLLM()
     messages: reactive[list[tuple[Author, str]]] = reactive([])
     chat_name: str
     system: str | None
     format: Literal["", "json"]
+    keep_alive: int = 5
     images: list[tuple[Path, str]] = []
 
     BINDINGS = [
         Binding("ctrl+e", "edit_chat", "edit", priority=True),
         Binding("ctrl+s", "export", "export", priority=True),
         ("ctrl+r", "rename_chat", "rename"),
         ("ctrl+x", "forget_chat", "forget"),
@@ -58,28 +59,31 @@
         db_id: int,
         chat_name: str,
         model: str = "nous-hermes:13b",
         context: list[int] = [],
         messages: list[tuple[Author, str]] = [],
         system: str | None = None,
         format: Literal["", "json"] = "",
+        keep_alive: int = 5,
         **kwargs,
     ) -> None:
         super().__init__(*children, **kwargs)
         self.ollama = OllamaLLM(
             model=model,
             context=context,
             system=system,
             format=format,
+            keep_alive=keep_alive,
         )  # We do this to reset the context
         self.chat_name = chat_name
         self.db_id = db_id
         self.messages = messages
         self.system = system
         self.format = format
+        self.keep_alive = keep_alive
         self.loaded = False
 
     def on_mount(self) -> None:
         self.query_one("#prompt").focus()
 
     async def load_messages(self) -> None:
         if self.loaded:
@@ -112,25 +116,26 @@
             user_chat_item.author = Author.USER
             message_container.mount(user_chat_item)
 
             response_chat_item = ChatItem()
             response_chat_item.author = Author.OLLAMA
             message_container.mount(response_chat_item)
             loading = LoadingIndicator()
-            message_container.mount(loading)
+            await message_container.mount(loading)
             message_container.scroll_end()
 
             try:
                 response = ""
                 async for text in self.ollama.stream(
                     message, [img for _, img in self.images]
                 ):
                     response = text
                     response_chat_item.text = text
-                    message_container.scroll_end()
+                    if message_container.can_view(response_chat_item):
+                        message_container.scroll_end()
                 self.messages.append((Author.OLLAMA, response))
                 self.images = []
 
                 # Save to db
                 await self.app.store.save_context(  # type: ignore
                     id=self.db_id,
                     context=json.dumps(self.ollama.context),
@@ -160,38 +165,43 @@
             self.inference_task.cancel()
 
     async def action_edit_chat(self) -> None:
         async def on_model_select(model_info: str) -> None:
             model: dict = json.loads(model_info)
             self.system = model.get("system")
             self.format = model.get("format", "")
+            self.keep_alive = model.get("keep_alive", 5)
+
             await self.app.store.edit_chat(
                 id=self.db_id,
                 name=self.chat_name,
                 system=model["system"],
                 format=model["format"],
+                keep_alive=model["keep_alive"],
             )
-            _, _, _, context, _, _ = await self.app.store.get_chat(self.db_id)
+            _, _, _, context, _, _, _ = await self.app.store.get_chat(self.db_id)
             self.ollama = OllamaLLM(
                 model=model["name"],
                 context=context,
                 system=model["system"],
                 format=model["format"],
+                keep_alive=model["keep_alive"],
             )
 
         screen = ChatEdit()
         screen.model_name = self.ollama.model
 
         await self.app.push_screen(screen, on_model_select)
         screen.edit_mode = True
         screen.select_model(self.ollama.model)
 
         if self.system:
             screen.system = self.system
         screen.json_format = self.format == "json"
+        screen.keep_alive = self.keep_alive
 
     async def action_export(self) -> None:
         screen = ChatExport()
         screen.chat_id = self.db_id
         screen.file_name = f"{slugify(self.chat_name)}.md"
         self.app.push_screen(screen)
```

### Comparing `oterm-0.2.7/oterm/app/widgets/image.py` & `oterm-0.2.8/oterm/app/widgets/image.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.7/oterm/app/widgets/monkey.py` & `oterm-0.2.8/oterm/app/widgets/monkey.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.7/oterm/app/widgets/prompt.py` & `oterm-0.2.8/oterm/app/widgets/prompt.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.7/oterm/app/widgets/text_area.py` & `oterm-0.2.8/oterm/app/widgets/text_area.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.7/oterm/cli/oterm.py` & `oterm-0.2.8/oterm/cli/oterm.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.7/oterm/config.py` & `oterm-0.2.8/oterm/config.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.7/oterm/ollama.py` & `oterm-0.2.8/oterm/ollama.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,31 +8,34 @@
 class OllamaLLM:
     def __init__(
         self,
         model="nous-hermes:13b",
         system: str | None = None,
         context: list[int] = [],
         format: Literal["", "json"] = "",
+        keep_alive: int = 5,
     ):
         self.model = model
         self.system = system
         self.context = context
         self.format = format
+        self.keep_alive = keep_alive
 
     async def completion(self, prompt: str, images: list[str] = []) -> str:
         client = AsyncClient(
             host=envConfig.OLLAMA_URL, verify=envConfig.OTERM_VERIFY_SSL
         )
         response: dict = await client.generate(
             model=self.model,
             prompt=prompt,
             context=self.context,
             system=self.system,  # type: ignore
             format=self.format,  # type: ignore
             images=images,
+            keep_alive=f"{self.keep_alive}m",
         )
         self.context = response.get("context", [])
         return response.get("response", "")
 
     async def stream(
         self, prompt: str, images: list[str] = []
     ) -> AsyncGenerator[str, Any]:
@@ -43,28 +46,25 @@
             model=self.model,
             prompt=prompt,
             context=self.context,
             system=self.system,  # type: ignore
             format=self.format,  # type: ignore
             images=images,
             stream=True,
+            keep_alive=f"{self.keep_alive}m",
         )
         text = ""
         async for response in stream:
             text = text + response.get("response", "")
             if "context" in response:
                 self.context = response.get("context")
             yield text
 
     @staticmethod
     def list() -> Mapping[str, Any]:
-        client = Client(
-            host=envConfig.OLLAMA_URL, verify=envConfig.OTERM_VERIFY_SSL
-        )
+        client = Client(host=envConfig.OLLAMA_URL, verify=envConfig.OTERM_VERIFY_SSL)
         return client.list()
 
     @staticmethod
     def show(model: str) -> Mapping[str, Any]:
-        client = Client(
-            host=envConfig.OLLAMA_URL, verify=envConfig.OTERM_VERIFY_SSL
-        )
+        client = Client(host=envConfig.OLLAMA_URL, verify=envConfig.OTERM_VERIFY_SSL)
         return client.show(model)
```

### Comparing `oterm-0.2.7/oterm/store/setup.py` & `oterm-0.2.8/oterm/store/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 CREATE TABLE IF NOT EXISTS "chat" (
 	"id"		INTEGER,
 	"name"		TEXT,
 	"model"		TEXT NOT NULL,
 	"context"	TEXT NOT NULL,
 	"system"	TEXT,
 	"format"	TEXT,
+    "keep_alive" INTEGER DEFAULT 5,
 	PRIMARY KEY("id" AUTOINCREMENT)
 );
 
 -- name: create_message_table
 CREATE TABLE IF NOT EXISTS "message" (
 	"chat_id"	INTEGER NOT NULL,
 	"author"	TEXT NOT NULL,
```

### Comparing `oterm-0.2.7/oterm/store/store.py` & `oterm-0.2.8/oterm/store/store.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,24 +58,26 @@
         self,
         id: int | None,
         name: str,
         model: str,
         context: str,
         system: str | None,
         format: Literal["", "json"],
+        keep_alive: int,
     ) -> int:
         async with aiosqlite.connect(self.db_path) as connection:
             res: list[tuple[int]] = await chat_queries.save_chat(  # type: ignore
                 connection,
                 id=id,
                 name=name,
                 model=model,
                 context=context,
                 system=system,
                 format=format,
+                keep_alive=keep_alive,
             )
 
             await connection.commit()
             return res[0][0]
 
     async def save_context(self, id: int, context: str) -> None:
         async with aiosqlite.connect(self.db_path) as connection:
@@ -92,47 +94,53 @@
                 connection,
                 id=id,
                 name=name,
             )
             await connection.commit()
 
     async def edit_chat(
-        self, id: int, name: str, system: str | None, format: Literal["", "json"]
+        self,
+        id: int,
+        name: str,
+        system: str | None,
+        format: Literal["", "json"],
+        keep_alive: int,
     ) -> None:
         async with aiosqlite.connect(self.db_path) as connection:
             await chat_queries.edit_chat(  # type: ignore
                 connection,
                 id=id,
                 name=name,
                 system=system,
                 format=format,
+                keep_alive=keep_alive,
             )
             await connection.commit()
 
     async def get_chats(
         self,
-    ) -> list[tuple[int, str, str, list[int], str | None, Literal["", "json"]]]:
+    ) -> list[tuple[int, str, str, list[int], str | None, Literal["", "json"], int]]:
         async with aiosqlite.connect(self.db_path) as connection:
             chats = await chat_queries.get_chats(connection)  # type: ignore
             chats = [
-                (id, name, model, json.loads(context), system, format)
-                for id, name, model, context, system, format in chats
+                (id, name, model, json.loads(context), system, format, keep_alive)
+                for id, name, model, context, system, format, keep_alive in chats
             ]
             return chats
 
     async def get_chat(
         self, id
-    ) -> tuple[int, str, str, list[int], str | None, Literal["", "json"]] | None:
+    ) -> tuple[int, str, str, list[int], str | None, Literal["", "json"], int] | None:
         async with aiosqlite.connect(self.db_path) as connection:
             chat = await chat_queries.get_chat(connection, id=id)  # type: ignore
             if chat:
                 chat = chat[0]
-                id, name, model, context, system, format = chat
+                id, name, model, context, system, format, keep_alive = chat
                 context = json.loads(context)
-                return id, name, model, context, system, format
+                return id, name, model, context, system, format, keep_alive
 
     async def delete_chat(self, id: int) -> None:
         async with aiosqlite.connect(self.db_path) as connection:
             await chat_queries.delete_chat(connection, id=id)  # type: ignore
             await connection.commit()
 
     async def save_message(self, chat_id: int, author: str, text: str) -> None:
```

### Comparing `oterm-0.2.7/oterm/store/upgrades/v0_1_11.py` & `oterm-0.2.8/oterm/store/upgrades/v0_1_11.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.7/oterm/store/upgrades/v0_1_6.py` & `oterm-0.2.8/oterm/store/upgrades/v0_1_6.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.7/oterm/store/upgrades/v0_2_0.py` & `oterm-0.2.8/oterm/store/upgrades/v0_2_0.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.7/oterm/store/upgrades/v0_2_4.py` & `oterm-0.2.8/oterm/store/upgrades/v0_2_4.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.7/oterm/utils.py` & `oterm-0.2.8/oterm/utils.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.7/pyproject.toml` & `oterm-0.2.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oterm"
-version = "0.2.7"
+version = "0.2.8"
 description = "A text-based terminal client for Ollama."
 authors = ["Yiorgis Gozadinos <ggozadinos@gmail.com>"]
 homepage = "https://github.com/ggozad/oterm"
 repository = "https://github.com/ggozad/oterm"
 license = "MIT"
 readme = "README.md"
 classifiers = [
```

### Comparing `oterm-0.2.7/PKG-INFO` & `oterm-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oterm
-Version: 0.2.7
+Version: 0.2.8
 Summary: A text-based terminal client for Ollama.
 Home-page: https://github.com/ggozad/oterm
 License: MIT
 Author: Yiorgis Gozadinos
 Author-email: ggozadinos@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```


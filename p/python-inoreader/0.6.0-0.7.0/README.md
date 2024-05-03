# Comparing `tmp/python-inoreader-0.6.0.tar.gz` & `tmp/python_inoreader-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-inoreader-0.6.0.tar", last modified: Fri Mar 22 10:18:29 2024, max compression
+gzip compressed data, was "python_inoreader-0.7.0.tar", last modified: Fri May  3 11:17:38 2024, max compression
```

## Comparing `python-inoreader-0.6.0.tar` & `python_inoreader-0.7.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 10:18:29.860854 python-inoreader-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-03-22 10:18:29.856854 python-inoreader-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-03-22 10:18:23.000000 python-inoreader-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 10:18:29.856854 python-inoreader-0.6.0/inoreader/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-22 10:18:23.000000 python-inoreader-0.6.0/inoreader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-03-22 10:18:23.000000 python-inoreader-0.6.0/inoreader/article.py
--rw-r--r--   0 runner    (1001) docker     (127)    10972 2024-03-22 10:18:23.000000 python-inoreader-0.6.0/inoreader/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-03-22 10:18:23.000000 python-inoreader-0.6.0/inoreader/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-03-22 10:18:23.000000 python-inoreader-0.6.0/inoreader/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-22 10:18:23.000000 python-inoreader-0.6.0/inoreader/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-03-22 10:18:23.000000 python-inoreader-0.6.0/inoreader/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    21870 2024-03-22 10:18:23.000000 python-inoreader-0.6.0/inoreader/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-03-22 10:18:23.000000 python-inoreader-0.6.0/inoreader/sim.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-03-22 10:18:23.000000 python-inoreader-0.6.0/inoreader/subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-03-22 10:18:23.000000 python-inoreader-0.6.0/inoreader/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-03-22 10:18:23.000000 python-inoreader-0.6.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 10:18:29.856854 python-inoreader-0.6.0/python_inoreader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-03-22 10:18:29.000000 python-inoreader-0.6.0/python_inoreader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-03-22 10:18:29.000000 python-inoreader-0.6.0/python_inoreader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 10:18:29.000000 python-inoreader-0.6.0/python_inoreader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-22 10:18:29.000000 python-inoreader-0.6.0/python_inoreader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-22 10:18:29.000000 python-inoreader-0.6.0/python_inoreader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-22 10:18:29.000000 python-inoreader-0.6.0/python_inoreader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 10:18:29.860854 python-inoreader-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:17:38.012538 python_inoreader-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-03 11:17:38.012538 python_inoreader-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-03 11:17:29.000000 python_inoreader-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:17:38.012538 python_inoreader-0.7.0/inoreader/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-03 11:17:29.000000 python_inoreader-0.7.0/inoreader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-03 11:17:29.000000 python_inoreader-0.7.0/inoreader/article.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10436 2024-05-03 11:17:29.000000 python_inoreader-0.7.0/inoreader/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-03 11:17:29.000000 python_inoreader-0.7.0/inoreader/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-03 11:17:29.000000 python_inoreader-0.7.0/inoreader/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-03 11:17:29.000000 python_inoreader-0.7.0/inoreader/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-03 11:17:29.000000 python_inoreader-0.7.0/inoreader/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22407 2024-05-03 11:17:29.000000 python_inoreader-0.7.0/inoreader/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-05-03 11:17:29.000000 python_inoreader-0.7.0/inoreader/sim.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-03 11:17:29.000000 python_inoreader-0.7.0/inoreader/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-03 11:17:29.000000 python_inoreader-0.7.0/inoreader/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-03 11:17:29.000000 python_inoreader-0.7.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:17:38.012538 python_inoreader-0.7.0/python_inoreader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-03 11:17:38.000000 python_inoreader-0.7.0/python_inoreader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-03 11:17:38.000000 python_inoreader-0.7.0/python_inoreader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 11:17:38.000000 python_inoreader-0.7.0/python_inoreader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-03 11:17:38.000000 python_inoreader-0.7.0/python_inoreader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-03 11:17:38.000000 python_inoreader-0.7.0/python_inoreader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-03 11:17:38.000000 python_inoreader-0.7.0/python_inoreader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 11:17:38.012538 python_inoreader-0.7.0/setup.cfg
```

### Comparing `python-inoreader-0.6.0/PKG-INFO` & `python_inoreader-0.7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-inoreader
-Version: 0.6.0
+Version: 0.7.0
 Summary: Python wrapper of Inoreader API
 Author-email: Linusp <linusp1024@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Linusp/python-inoreader
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `python-inoreader-0.6.0/README.md` & `python_inoreader-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `python-inoreader-0.6.0/inoreader/article.py` & `python_inoreader-0.7.0/inoreader/article.py`

 * *Files identical despite different names*

### Comparing `python-inoreader-0.6.0/inoreader/client.py` & `python_inoreader-0.7.0/inoreader/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -139,100 +139,87 @@
         self.check_token()
 
         url = urljoin(BASE_URL, self.SUBSCRIPTION_LIST_PATH)
         response = self.parse_response(self.session.get(url, proxies=self.proxies))
         for item in response["subscriptions"]:
             yield Subscription.from_json(item)
 
-    def get_stream_contents(self, stream_id, c="", limit=None):
-        fetched_count = 0
-        stop = False
-        while not stop:
-            articles, c = self.__get_stream_contents(stream_id, c)
-            for a in articles:
-                try:
-                    yield Article.from_json(a)
-                    fetched_count += 1
-                except Exception as e:
-                    print(e)
-                    continue
-                if limit and fetched_count >= limit:
-                    stop = True
-                    break
-            if c is None:
-                break
-
-    def __get_stream_contents(self, stream_id, continuation=""):
+    def __get_stream_contents(
+        self, stream_id=None, n=50, r=None, ot=None, xt=None, it=None, c=None
+    ):
+        """reference: https://www.inoreader.com/developers/stream-contents"""
         self.check_token()
 
-        url = urljoin(BASE_URL, self.STREAM_CONTENTS_PATH + quote_plus(stream_id))
-        params = {"n": 50, "r": "", "c": continuation, "output": "json"}  # default 20, max 1000
+        url = urljoin(BASE_URL, self.STREAM_CONTENTS_PATH)
+        if stream_id:
+            url = urljoin(url, quote_plus(stream_id))
+
+        params = {"n": n, "r": r, "ot": ot, "xt": xt, "it": it, "c": c}
+        params = {arg: val for arg, val in params.items() if val is not None}
         response = self.parse_response(self.session.post(url, params=params, proxies=self.proxies))
         if "continuation" in response:
             return response["items"], response["continuation"]
         else:
             return response["items"], None
 
-    def fetch_articles(self, folder=None, tags=None, unread=True, starred=False, limit=None):
+    def fetch_articles(
+        self, stream_id=None, folder=None, tags=None, unread=True, starred=False, limit=None, n=50
+    ):
         self.check_token()
 
-        url = urljoin(BASE_URL, self.STREAM_CONTENTS_PATH)
-        if folder:
-            url = urljoin(url, quote_plus(self.GENERAL_TAG_TEMPLATE.format(folder)))
+        if not stream_id and folder:
+            stream_id = self.GENERAL_TAG_TEMPLATE.format(folder)
 
-        params = {"c": str(uuid4())}
+        params = {"stream_id": stream_id, "n": n, "c": str(uuid4())}
         if unread:
             params["xt"] = self.READ_TAG
 
         if starred:
             params["it"] = self.STARRED_TAG
 
         fetched_count = 0
-        response = self.parse_response(self.session.post(url, params=params, proxies=self.proxies))
-        for data in response["items"]:
+        items, continuation = self.__get_stream_contents(**params)
+        for data in items:
             categories = {
                 category.split("/")[-1]
                 for category in data.get("categories", [])
                 if category.find("label") > 0
             }
             if tags and not categories.issuperset(set(tags)):
                 continue
 
             yield Article.from_json(data)
             fetched_count += 1
             if limit and fetched_count >= limit:
                 break
 
-        continuation = response.get("continuation")
         while continuation and (not limit or fetched_count < limit):
             params["c"] = continuation
-            response = self.parse_response(
-                self.session.post(url, params=params, proxies=self.proxies)
-            )
-            for data in response["items"]:
+            items, continuation = self.__get_stream_contents(**params)
+            for data in items:
                 categories = {
                     category.split("/")[-1]
                     for category in data.get("categories", [])
                     if category.find("label") > 0
                 }
                 if tags and not categories.issuperset(set(tags)):
                     continue
                 yield Article.from_json(data)
                 fetched_count += 1
                 if limit and fetched_count >= limit:
                     break
 
-            continuation = response.get("continuation")
-
-    def fetch_unread(self, folder=None, tags=None, limit=None):
-        for article in self.fetch_articles(folder=folder, tags=tags, unread=True):
+    def fetch_unread(self, folder=None, tags=None, limit=None, n=None):
+        for article in self.fetch_articles(folder=folder, tags=tags, unread=True, n=n):
             yield article
 
-    def fetch_starred(self, folder=None, tags=None, limit=None):
-        for article in self.fetch_articles(folder=folder, tags=tags, unread=False, starred=True):
+    def fetch_starred(self, folder=None, tags=None, limit=None, n=None):
+        for article in self.fetch_articles(
+            folder=folder, tags=tags, unread=False, starred=True, n=n
+        ):
             yield article
 
     def add_general_label(self, articles, label):
         self.check_token()
 
         url = urljoin(BASE_URL, self.EDIT_TAG_PATH)
         for start in range(0, len(articles), 10):
```

### Comparing `python-inoreader-0.6.0/inoreader/config.py` & `python_inoreader-0.7.0/inoreader/config.py`

 * *Files identical despite different names*

### Comparing `python-inoreader-0.6.0/inoreader/filter.py` & `python_inoreader-0.7.0/inoreader/filter.py`

 * *Files identical despite different names*

### Comparing `python-inoreader-0.6.0/inoreader/main.py` & `python_inoreader-0.7.0/inoreader/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,30 +196,33 @@
 
     print(tabulate(output_info, headers="firstrow", tablefmt="github"))
 
 
 @main.command("fetch-unread")
 @click.option("-f", "--folder", required=True, help="Folder which articles belong to")
 @click.option("-t", "--tags", help="Tag(s) for filtering, separate with comma")
+@click.option(
+    "--batch-size", type=int, default=50, help="Maximum number of articles per API request"
+)
 @click.option("-o", "--outfile", required=True, help="Filename to save articles")
 @click.option(
     "--out-format",
     type=click.Choice(["json", "csv", "plain", "markdown", "org-mode"]),
     default="json",
     help="Format of output file, default: json",
 )
 @catch_error
-def fetch_unread(folder, tags, outfile, out_format):
+def fetch_unread(folder, tags, batch_size, outfile, out_format):
     """Fetch unread articles"""
     client = get_client()
 
     tag_list = [] if not tags else tags.split(",")
     fout = codecs.open(outfile, mode="w", encoding="utf-8")
     writer = csv.writer(fout, delimiter=",") if out_format == "csv" else None
-    for idx, article in enumerate(client.fetch_unread(folder=folder, tags=tag_list)):
+    for idx, article in enumerate(client.fetch_unread(folder=folder, tags=tag_list, n=batch_size)):
         if idx > 0 and (idx % 10) == 0:
             LOGGER.info("fetched %d articles", idx)
         title = article.title
         text = article.text
         link = article.link
         if out_format == "json":
             print(
@@ -387,33 +390,39 @@
 
     if outfile:
         fout.close()
 
 
 @main.command("fetch-articles")
 @click.option("-i", "--stream-id", required=True, help="Stream ID which you want to fetch")
+@click.option(
+    "--batch-size", type=int, default=50, help="Maximum number of articles per API request"
+)
+@click.option("--only-unread", is_flag=True, help="Fetch unread articles only")
 @click.option("-o", "--outfile", required=True, help="Filename to save results")
 @click.option(
     "--out-format",
     type=click.Choice(["json", "csv", "plain", "markdown", "org-mode"]),
     default="json",
     help="Format of output, default: json",
 )
 @catch_error
-def fetch_articles(outfile, stream_id, out_format):
+def fetch_articles(outfile, stream_id, batch_size, only_unread, out_format):
     """Fetch articles by stream id"""
     client = get_client()
 
     fout = codecs.open(outfile, mode="w", encoding="utf-8")
     writer = None
     if out_format == "csv":
         writer = csv.DictWriter(fout, ["title", "content"], delimiter=",", quoting=csv.QUOTE_ALL)
         writer.writeheader()
 
-    for idx, article in enumerate(client.get_stream_contents(stream_id)):
+    for idx, article in enumerate(
+        client.fetch_articles(stream_id=stream_id, n=batch_size, unread=only_unread)
+    ):
         if idx > 0 and (idx % 10) == 0:
             LOGGER.info("fetched %d articles", idx)
 
         title = article.title
         text = article.text
         if out_format == "json":
             print(json.dumps({"title": title, "content": text}, ensure_ascii=False), file=fout)
@@ -466,29 +475,32 @@
     apply_action(matched_articles, client, "mark_as_read", None)
 
 
 @main.command("fetch-starred")
 @click.option("-f", "--folder", help="Folder which articles belong to")
 @click.option("-t", "--tags", help="Tag(s) for filtering, separate with comma")
 @click.option(
+    "--batch-size", type=int, default=50, help="Maximum number of articles per API request"
+)
+@click.option(
     "-o", "--outfile", help="Filename to save articles, required when output format is `csv`"
 )
 @click.option(
     "-d", "--outdir", help="Directory to save articles, required when output format is not `csv`"
 )
 @click.option("-l", "--limit", type=int)
 @click.option("--save-image", is_flag=True)
 @click.option(
     "--out-format",
     type=click.Choice(["json", "csv", "markdown", "org-mode"]),
     default="json",
     help="Format of output file, default: json",
 )
 @catch_error
-def fetch_starred(folder, tags, outfile, outdir, limit, save_image, out_format):
+def fetch_starred(folder, tags, batch_size, outfile, outdir, limit, save_image, out_format):
     """Fetch starred articles"""
     client = get_client()
 
     if out_format == "csv" and not outfile:
         click.secho("`outfile` is required!", fg="red")
         return -1
     elif out_format != "csv" and not outdir:
@@ -502,15 +514,15 @@
         )
     elif not os.path.exists(outdir):
         os.makedirs(outdir)
 
     tag_list = [] if not tags else tags.split(",")
     url_to_image = {}
     fetched_count = 0
-    for article in client.fetch_starred(folder=folder, tags=tag_list, limit=limit):
+    for article in client.fetch_starred(folder=folder, tags=tag_list, limit=limit, n=batch_size):
         if limit and fetched_count >= limit:
             break
 
         fetched_count += 1
         title = article.title
         text = article.text
         link = article.link
```

### Comparing `python-inoreader-0.6.0/inoreader/sim.py` & `python_inoreader-0.7.0/inoreader/sim.py`

 * *Files identical despite different names*

### Comparing `python-inoreader-0.6.0/inoreader/subscription.py` & `python_inoreader-0.7.0/inoreader/subscription.py`

 * *Files identical despite different names*

### Comparing `python-inoreader-0.6.0/inoreader/utils.py` & `python_inoreader-0.7.0/inoreader/utils.py`

 * *Files identical despite different names*

### Comparing `python-inoreader-0.6.0/pyproject.toml` & `python_inoreader-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "python-inoreader"
-version = "0.6.0"
+version = "0.7.0"
 description = "Python wrapper of Inoreader API"
 authors = [
     {name = "Linusp", email = "linusp1024@gmail.com"},
 ]
 dependencies = [
     "lxml",
     "requests",
```

### Comparing `python-inoreader-0.6.0/python_inoreader.egg-info/PKG-INFO` & `python_inoreader-0.7.0/python_inoreader.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-inoreader
-Version: 0.6.0
+Version: 0.7.0
 Summary: Python wrapper of Inoreader API
 Author-email: Linusp <linusp1024@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Linusp/python-inoreader
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```


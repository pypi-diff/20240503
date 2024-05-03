# Comparing `tmp/flet_route-0.3.2.tar.gz` & `tmp/flet_route-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_route-0.3.2.tar", last modified: Sat Sep  9 04:20:48 2023, max compression
+gzip compressed data, was "flet_route-0.3.3.tar", last modified: Fri May  3 12:50:49 2024, max compression
```

## Comparing `flet_route-0.3.2.tar` & `flet_route-0.3.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 saurabh   (1000) saurabh   (1000)        0 2023-09-09 04:20:48.529850 flet_route-0.3.2/
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)     1072 2023-06-16 04:23:36.000000 flet_route-0.3.2/LICENSE
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)     1355 2023-09-09 04:20:48.529850 flet_route-0.3.2/PKG-INFO
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)      834 2023-06-18 15:43:54.000000 flet_route-0.3.2/README.md
-drwxr-xr-x   0 saurabh   (1000) saurabh   (1000)        0 2023-09-09 04:20:48.526851 flet_route-0.3.2/cli/
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)       25 2023-06-16 05:00:09.000000 flet_route-0.3.2/cli/__init__.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)     2642 2023-06-18 15:00:26.000000 flet_route-0.3.2/cli/ac_class_contents.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)     2217 2023-06-18 14:43:18.000000 flet_route-0.3.2/cli/ac_func_contents.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)     2381 2023-06-18 14:11:32.000000 flet_route-0.3.2/cli/class_contents.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)     2181 2023-06-18 14:34:00.000000 flet_route-0.3.2/cli/cli.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)     2025 2023-06-18 14:50:39.000000 flet_route-0.3.2/cli/func_contents.py
-drwxr-xr-x   0 saurabh   (1000) saurabh   (1000)        0 2023-09-09 04:20:48.527850 flet_route-0.3.2/flet_route/
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)      128 2023-06-16 04:23:36.000000 flet_route-0.3.2/flet_route/__init__.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)      646 2023-06-16 04:23:36.000000 flet_route-0.3.2/flet_route/basket.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)      854 2023-06-16 04:23:36.000000 flet_route-0.3.2/flet_route/not_found_view.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)      716 2023-06-16 04:23:36.000000 flet_route-0.3.2/flet_route/params.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)     7412 2023-09-09 04:11:05.000000 flet_route-0.3.2/flet_route/routing.py
-drwxr-xr-x   0 saurabh   (1000) saurabh   (1000)        0 2023-09-09 04:20:48.528850 flet_route-0.3.2/flet_route.egg-info/
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)     1355 2023-09-09 04:20:48.000000 flet_route-0.3.2/flet_route.egg-info/PKG-INFO
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)      467 2023-09-09 04:20:48.000000 flet_route-0.3.2/flet_route.egg-info/SOURCES.txt
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)        1 2023-09-09 04:20:48.000000 flet_route-0.3.2/flet_route.egg-info/dependency_links.txt
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)       44 2023-09-09 04:20:48.000000 flet_route-0.3.2/flet_route.egg-info/entry_points.txt
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)       25 2023-09-09 04:20:48.000000 flet_route-0.3.2/flet_route.egg-info/requires.txt
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)       15 2023-09-09 04:20:48.000000 flet_route-0.3.2/flet_route.egg-info/top_level.txt
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)       38 2023-09-09 04:20:48.529850 flet_route-0.3.2/setup.cfg
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)      936 2023-09-09 04:11:37.000000 flet_route-0.3.2/setup.py
+drwxr-xr-x   0 saurabh   (1000) saurabh   (1000)        0 2024-05-03 12:50:49.271341 flet_route-0.3.3/
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)     1072 2023-06-16 04:23:36.000000 flet_route-0.3.3/LICENSE
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)     1355 2024-05-03 12:50:49.270341 flet_route-0.3.3/PKG-INFO
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)      834 2023-06-18 15:43:54.000000 flet_route-0.3.3/README.md
+drwxr-xr-x   0 saurabh   (1000) saurabh   (1000)        0 2024-05-03 12:50:49.268341 flet_route-0.3.3/cli/
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)       25 2023-06-16 05:00:09.000000 flet_route-0.3.3/cli/__init__.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)     2498 2024-05-03 12:23:40.000000 flet_route-0.3.3/cli/ac_class_contents.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)     2092 2024-05-03 12:22:05.000000 flet_route-0.3.3/cli/ac_func_contents.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)     2381 2023-06-18 14:11:32.000000 flet_route-0.3.3/cli/class_contents.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)     2181 2023-06-18 14:34:00.000000 flet_route-0.3.3/cli/cli.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)     2025 2023-06-18 14:50:39.000000 flet_route-0.3.3/cli/func_contents.py
+drwxr-xr-x   0 saurabh   (1000) saurabh   (1000)        0 2024-05-03 12:50:49.269341 flet_route-0.3.3/flet_route/
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)      128 2023-06-16 04:23:36.000000 flet_route-0.3.3/flet_route/__init__.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)      646 2023-06-16 04:23:36.000000 flet_route-0.3.3/flet_route/basket.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)      873 2024-05-03 12:27:02.000000 flet_route-0.3.3/flet_route/not_found_view.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)      716 2023-06-16 04:23:36.000000 flet_route-0.3.3/flet_route/params.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)     7364 2024-05-03 11:51:34.000000 flet_route-0.3.3/flet_route/routing.py
+drwxr-xr-x   0 saurabh   (1000) saurabh   (1000)        0 2024-05-03 12:50:49.270341 flet_route-0.3.3/flet_route.egg-info/
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)     1355 2024-05-03 12:50:49.000000 flet_route-0.3.3/flet_route.egg-info/PKG-INFO
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)      467 2024-05-03 12:50:49.000000 flet_route-0.3.3/flet_route.egg-info/SOURCES.txt
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)        1 2024-05-03 12:50:49.000000 flet_route-0.3.3/flet_route.egg-info/dependency_links.txt
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)       44 2024-05-03 12:50:49.000000 flet_route-0.3.3/flet_route.egg-info/entry_points.txt
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)       25 2024-05-03 12:50:49.000000 flet_route-0.3.3/flet_route.egg-info/requires.txt
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)       15 2024-05-03 12:50:49.000000 flet_route-0.3.3/flet_route.egg-info/top_level.txt
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)       38 2024-05-03 12:50:49.271341 flet_route-0.3.3/setup.cfg
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)      937 2024-05-03 12:46:52.000000 flet_route-0.3.3/setup.py
```

### Comparing `flet_route-0.3.2/LICENSE` & `flet_route-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flet_route-0.3.2/PKG-INFO` & `flet_route-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet_route
-Version: 0.3.2
+Version: 0.3.3
 Summary: This makes it easy to manage multiple views with dynamic routing.
 Home-page: https://github.com/saurabhwadekar/flet_route
 Author: Saurabh Wadekar [ INDIA ]
 Maintainer: Saurabh Wadekar
 Maintainer-email: saurabhwadekar420@gmail.com
 License: MIT
 Keywords: flet,routing,flet_route,routes,flet app,flet-route,flet simple routing
```

### Comparing `flet_route-0.3.2/README.md` & `flet_route-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `flet_route-0.3.2/cli/ac_class_contents.py` & `flet_route-0.3.3/cli/ac_class_contents.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
     Routing(
         page = page,
         app_routes = app_routes,
         middleware = AppBasedMiddleware().call_me,
         async_is = True
     )
-    await page.go_async(page.route)
+    page.go(page.route)
 
 ft.app(target=main)
 
 """
 
 ROUTES = """from flet_route import path
 from middlewares.url_middleware import UrlBasedMiddleware
@@ -35,51 +35,45 @@
 INDEX_VIEW = """import flet as ft
 from flet_route import Params,Basket
 
 class IndexView:
     def __init__(self):
         ...
 
-    async def go_next_view(self,e):
-        await self.page.go_async("/next_view/10")
-
     async def view(self,page:ft.page,params:Params,basket:Basket):
         self.page = page
         print(params)
         print(basket)
 
         return ft.View(
             "/",
             controls=[
                 ft.Text("This Is Index View"),
-                ft.ElevatedButton("Go Next View", on_click= self.go_next_view),
+                ft.ElevatedButton("Go Next View", on_click= lambda _: self.page.go("/next_view/10")),
             ]
         )
 """
 
 NEXT_VIEW = """import flet as ft
 from flet_route import Params,Basket
 
 class NextView:
     def __init__(self):
         ...
 
-    async def go_index_view(self,e):
-        await self.page.go_async("/")
-
     async def view(self,page:ft.page,params:Params,basket:Basket):
         self.page = page
         print(params)
         print(basket)
 
         return ft.View(
             "/next_view/:my_id",
             controls=[
                 ft.Text("This Is Next View"),
-                ft.ElevatedButton("Go Index View", on_click= self.go_index_view),
+                ft.ElevatedButton("Go Index View", on_click= lambda _: self.page.go("/")),
             ]
         )
 """
 
 APP_BASED_MIDDLEWARE = """import flet as ft
 from flet_route import Params,Basket
```

### Comparing `flet_route-0.3.2/cli/ac_func_contents.py` & `flet_route-0.3.3/cli/func_contents.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 
 MAIN = """import flet as ft
 from flet_route import Routing
 from routes import app_routes
 from middlewares.app_middleware import AppBasedMiddleware
 
-async def main(page: ft.Page):
+def main(page: ft.Page):
 
     Routing(
         page = page,
         app_routes = app_routes,
-        middleware = AppBasedMiddleware,
-        async_is = True
+        middleware = AppBasedMiddleware
     )
-    await page.go_async(page.route)
+    page.go(page.route)
 
 ft.app(target=main)
 
 """
 
 ROUTES = """from flet_route import path
 from middlewares.url_middleware import UrlBasedMiddleware
@@ -31,61 +30,53 @@
 ]
 
 """
 
 INDEX_VIEW = """import flet as ft
 from flet_route import Params,Basket
 
-async def IndexView(page:ft.Page,params:Params,basket:Basket):
+def IndexView(page:ft.Page,params:Params,basket:Basket):
     print(params)
     print(basket)
 
-    async def go_next_view(e):
-        await page.go_async("/next_view/10")
-        
     return ft.View(
         "/",
         controls=[
             ft.Text("This Is Index View"),
-            ft.ElevatedButton("Go Next View", on_click= go_next_view ),
+            ft.ElevatedButton("Go Next View", on_click=lambda _: page.go("/next_view/10")),
         ]
     )
-
 """
 
 NEXT_VIEW = """import flet as ft
 from flet_route import Params,Basket
 
-async def NextView(page:ft.Page,params:Params,basket:Basket):
+def NextView(page:ft.Page,params:Params,basket:Basket):
     print(params)
     print(basket)
     
-    async def go_index_view(e):
-        await page.go_async("/")
-
     return ft.View(
         "/next_view/:my_id",
         controls=[
             ft.Text("This Is Next View"),
-            ft.ElevatedButton("Go Index View", on_click= go_index_view),
+            ft.ElevatedButton("Go Index View", on_click=lambda _: page.go("/")),
         ]
     )
-
 """
 
 APP_BASED_MIDDLEWARE = """import flet as ft
 from flet_route import Params,Basket
 
-async def AppBasedMiddleware(page:ft.Page,params:Params,basket:Basket):
+def AppBasedMiddleware(page:ft.Page,params:Params,basket:Basket):
 
     print("App Based Middleware Called")
     #page.route = "/another_view" # If you want to change the route for some reason, use page.route
 """
 
 URL_BASED_MIDDLEWARE = """import flet as ft
 from flet_route import Params,Basket
 
-async def UrlBasedMiddleware(page:ft.Page,params:Params,basket:Basket):
+def UrlBasedMiddleware(page:ft.Page,params:Params,basket:Basket):
 
     print("Url Based Middleware Called")
     #page.route = "/another_view" # If you want to change the route for some reason, use page.route
 """
```

### Comparing `flet_route-0.3.2/cli/class_contents.py` & `flet_route-0.3.3/cli/class_contents.py`

 * *Files identical despite different names*

### Comparing `flet_route-0.3.2/cli/cli.py` & `flet_route-0.3.3/cli/cli.py`

 * *Files identical despite different names*

### Comparing `flet_route-0.3.2/cli/func_contents.py` & `flet_route-0.3.3/cli/ac_func_contents.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 
 MAIN = """import flet as ft
 from flet_route import Routing
 from routes import app_routes
 from middlewares.app_middleware import AppBasedMiddleware
 
-def main(page: ft.Page):
+async def main(page: ft.Page):
 
     Routing(
         page = page,
         app_routes = app_routes,
-        middleware = AppBasedMiddleware
+        middleware = AppBasedMiddleware,
+        async_is = True
     )
     page.go(page.route)
 
 ft.app(target=main)
 
 """
 
@@ -30,53 +31,55 @@
 ]
 
 """
 
 INDEX_VIEW = """import flet as ft
 from flet_route import Params,Basket
 
-def IndexView(page:ft.Page,params:Params,basket:Basket):
+async def IndexView(page:ft.Page,params:Params,basket:Basket):
     print(params)
     print(basket)
-
+        
     return ft.View(
         "/",
         controls=[
             ft.Text("This Is Index View"),
-            ft.ElevatedButton("Go Next View", on_click=lambda _: page.go("/next_view/10")),
+            ft.ElevatedButton("Go Next View", on_click= lambda _: page.go("/next_view/10")),
         ]
     )
+
 """
 
 NEXT_VIEW = """import flet as ft
 from flet_route import Params,Basket
 
-def NextView(page:ft.Page,params:Params,basket:Basket):
+async def NextView(page:ft.Page,params:Params,basket:Basket):
     print(params)
     print(basket)
     
     return ft.View(
         "/next_view/:my_id",
         controls=[
             ft.Text("This Is Next View"),
-            ft.ElevatedButton("Go Index View", on_click=lambda _: page.go("/")),
+            ft.ElevatedButton("Go Index View", on_click= lambda _: page.go("/")),
         ]
     )
+
 """
 
 APP_BASED_MIDDLEWARE = """import flet as ft
 from flet_route import Params,Basket
 
-def AppBasedMiddleware(page:ft.Page,params:Params,basket:Basket):
+async def AppBasedMiddleware(page:ft.Page,params:Params,basket:Basket):
 
     print("App Based Middleware Called")
     #page.route = "/another_view" # If you want to change the route for some reason, use page.route
 """
 
 URL_BASED_MIDDLEWARE = """import flet as ft
 from flet_route import Params,Basket
 
-def UrlBasedMiddleware(page:ft.Page,params:Params,basket:Basket):
+async def UrlBasedMiddleware(page:ft.Page,params:Params,basket:Basket):
 
     print("Url Based Middleware Called")
     #page.route = "/another_view" # If you want to change the route for some reason, use page.route
 """
```

### Comparing `flet_route-0.3.2/flet_route/basket.py` & `flet_route-0.3.3/flet_route/basket.py`

 * *Files identical despite different names*

### Comparing `flet_route-0.3.2/flet_route/params.py` & `flet_route-0.3.3/flet_route/params.py`

 * *Files identical despite different names*

### Comparing `flet_route-0.3.2/flet_route/routing.py` & `flet_route-0.3.3/flet_route/routing.py`

 * *Files 3% similar despite different names*

```diff
@@ -160,27 +160,27 @@
                     await self.__middleware(  # call main middleware
                         page=self.page,
                         params=self.__params,
                         basket=self.__basket
                     )
                 # if chnge route using main midellware recall change route
                 if self.page.route != route_str(route=route):
-                    await self.page.go_async(self.page.route)
+                    self.page.go(self.page.route)
                     return
 
                 if url[3] != None:
                     await url[3](  # call url middleware
                         page=self.page,
                         params=self.__params,
                         basket=self.__basket
                     )
 
                 # if chnge route using url midellware recall change route
                 if self.page.route != route_str(route=route):
-                    await self.page.go_async(self.page.route)
+                    self.page.go(self.page.route)
                     return
 
                 if url[1]:
                     self.page.views.clear()
                 view = await url[2](
                     page=self.page,
                     params=self.__params,
@@ -199,13 +199,13 @@
             self.page.views.append(
                 await self.not_found_view(
                     page=self.page,
                     params=self.__params,
                     basket=self.__basket
                 )
             )
-        await self.page.update_async()
+        self.page.update()
 
     async def view_pop_async(self, view):
         self.page.views.pop()
         top_view = self.page.views[-1]
-        await self.page.go_async(top_view.route)
+        self.page.go(top_view.route)
```

### Comparing `flet_route-0.3.2/flet_route.egg-info/PKG-INFO` & `flet_route-0.3.3/flet_route.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: flet-route
-Version: 0.3.2
+Name: flet_route
+Version: 0.3.3
 Summary: This makes it easy to manage multiple views with dynamic routing.
 Home-page: https://github.com/saurabhwadekar/flet_route
 Author: Saurabh Wadekar [ INDIA ]
 Maintainer: Saurabh Wadekar
 Maintainer-email: saurabhwadekar420@gmail.com
 License: MIT
 Keywords: flet,routing,flet_route,routes,flet app,flet-route,flet simple routing
```

### Comparing `flet_route-0.3.2/setup.py` & `flet_route-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name = "flet_route",
-    version = "0.3.2",
+    version = "0.3.3",
     author="Saurabh Wadekar [ INDIA ]",
     packages=["flet_route","cli"],
     license="MIT",
     maintainer="Saurabh Wadekar",
     maintainer_email="saurabhwadekar420@gmail.com",
     keywords=["flet","routing","flet_route","routes","flet app","flet-route","flet simple routing"],
     description="This makes it easy to manage multiple views with dynamic routing.",
@@ -23,8 +23,8 @@
         "repath",
         "flet",
     ],
     entry_points= {
         'console_scripts': 
         ['flet-route=cli:make_app']
     }, 
-)
+)
```


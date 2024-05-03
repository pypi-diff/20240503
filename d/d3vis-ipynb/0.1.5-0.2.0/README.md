# Comparing `tmp/d3vis_ipynb-0.1.5.tar.gz` & `tmp/d3vis_ipynb-0.2.0.tar.gz`

## Comparing `d3vis_ipynb-0.1.5.tar` & `d3vis_ipynb-0.2.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/D3vis_ipynb.json
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/MANIFEST.in
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/RELEASE.md
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/install.json
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/setup.cfg
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/setup.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/d3vis_ipynb/__init__.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/d3vis_ipynb/_version.py
--rw-r--r--   0        0        0     5728 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/d3vis_ipynb/embedding.py
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/d3vis_ipynb/web.py
--rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/d3vis_ipynb/widgets.py
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/d3vis_ipynb/labextension/package.json
--rw-r--r--   0        0        0    27996 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/d3vis_ipynb/labextension/static/363.d9832b540bc5aa86432a.js
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/d3vis_ipynb/labextension/static/493.053b071a46f0bcccaab9.js
--rw-r--r--   0        0        0   282230 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/d3vis_ipynb/labextension/static/693.c8409ce8329f6703470f.js
--rw-r--r--   0        0        0     6790 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/d3vis_ipynb/labextension/static/remoteEntry.0a6c310552f16e38d4c2.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/d3vis_ipynb/labextension/static/style.js
--rw-r--r--   0        0        0    35163 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/d3vis_ipynb/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0    93818 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/d3vis_ipynb/nbextension/index.js
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/js/README.md
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/js/amd-public-path.js
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/js/package.json
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/js/webpack.config.js
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/js/webpack.exports.config.js
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/js/css/widget.css
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/js/lib/extension.js
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/js/lib/index.js
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/js/lib/labplugin.js
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/js/lib/web-dev.js
--rw-r--r--   0        0        0    12874 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/js/lib/widgets.js
--rw-r--r--   0        0        0     9311 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/js/lib/graphs/barplot.js
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/js/lib/graphs/histogramplot.js
--rw-r--r--   0        0        0     3987 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/js/lib/graphs/linearhistplot.js
--rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/js/lib/graphs/rangeslider.js
--rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/js/lib/graphs/scatterplot.js
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/js/lib/tools/lasso.js
--rw-r--r--   0        0        0     5894 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/js/lib/wrappers/embedding.wrapper.js
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/.gitignore
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/LICENSE.txt
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/README.md
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.0/D3vis_ipynb.json
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.0/MANIFEST.in
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.0/RELEASE.md
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.0/install.json
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.0/setup.cfg
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.0/setup.py
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.0/d3vis_ipynb/__init__.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.0/d3vis_ipynb/_version.py
+-rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.0/d3vis_ipynb/custom.py
+-rw-r--r--   0        0        0     5728 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.0/d3vis_ipynb/embedding.py
+-rw-r--r--   0        0        0     7336 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.0/d3vis_ipynb/widgets.py
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.0/d3vis_ipynb/labextension/package.json
+-rw-r--r--   0        0        0    27903 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.0/d3vis_ipynb/labextension/static/363.5fe76f6939929abf33b8.js
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.0/d3vis_ipynb/labextension/static/493.053b071a46f0bcccaab9.js
+-rw-r--r--   0        0        0   282230 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.0/d3vis_ipynb/labextension/static/693.c8409ce8329f6703470f.js
+-rw-r--r--   0        0        0     6790 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.0/d3vis_ipynb/labextension/static/remoteEntry.075b810a9929e45488a4.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.0/d3vis_ipynb/labextension/static/style.js
+-rw-r--r--   0        0        0    35163 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.0/d3vis_ipynb/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0    93725 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.0/d3vis_ipynb/nbextension/index.js
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.0/js/README.md
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.0/js/amd-public-path.js
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.0/js/package.json
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.0/js/webpack.config.js
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.0/js/webpack.exports.config.js
+-rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.0/js/css/widget.css
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.0/js/lib/extension.js
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.0/js/lib/index.js
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.0/js/lib/labplugin.js
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.0/js/lib/web-dev.js
+-rw-r--r--   0        0        0    13007 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.0/js/lib/widgets.js
+-rw-r--r--   0        0        0     9163 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.0/js/lib/graphs/barplot.js
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.0/js/lib/graphs/histogramplot.js
+-rw-r--r--   0        0        0     3987 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.0/js/lib/graphs/linearhistplot.js
+-rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.0/js/lib/graphs/rangeslider.js
+-rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.0/js/lib/graphs/scatterplot.js
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.0/js/lib/tools/lasso.js
+-rw-r--r--   0        0        0     5894 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.0/js/lib/wrappers/embedding.wrapper.js
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.0/README.md
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.0/PKG-INFO
```

### Comparing `d3vis_ipynb-0.1.5/RELEASE.md` & `d3vis_ipynb-0.2.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.5/setup.cfg` & `d3vis_ipynb-0.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.5/d3vis_ipynb/__init__.py` & `d3vis_ipynb-0.2.0/d3vis_ipynb/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 
 from ._version import __version__
+from .custom import CustomWidget
 from .embedding import Embedding
-from .web import WebWidget
 from .widgets import *
 
 if "google.colab.output" in sys.modules:
     sys.modules["google.colab.output"].enable_custom_widget_manager()
 
 
 def _jupyter_labextension_paths():
```

### Comparing `d3vis_ipynb-0.1.5/d3vis_ipynb/embedding.py` & `d3vis_ipynb-0.2.0/d3vis_ipynb/embedding.py`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.5/d3vis_ipynb/web.py` & `d3vis_ipynb-0.2.0/d3vis_ipynb/custom.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,58 @@
 import anywidget
 import urllib3
 
 
-class WebWidget(anywidget.AnyWidget):
+class CustomWidget(anywidget.AnyWidget):
     def readFromWeb(url):
         http = urllib3.PoolManager(cert_reqs="CERT_NONE")
         response = http.request("GET", url)
         text = response.data.decode("utf-8")
         return text
 
+    def readFromLocalFile(path):
+        text = ""
+        with open(path, "r") as file:
+            lines = file.readlines()
+            text = text.join(lines)
+        return text
+
+    def createWidgetFromLocalFile(
+        widgetCall: str, varList: list, updatableVars: list, filePath: str
+    ):
+        return CustomWidget._createWidget(
+            widgetCall, varList, updatableVars, filePath, CustomWidget.readFromLocalFile
+        )
+
     def createWidgetFromUrl(
         widgetCall: str, varList: list, updatableVars: list, jsUrl: str
     ):
+        return CustomWidget._createWidget(
+            widgetCall, varList, updatableVars, jsUrl, CustomWidget.readFromWeb
+        )
+
+    def _createWidget(
+        widgetCall: str, varList: list, updatableVars: list, string: str, fileReader
+    ):
         modelVars = ""
         modelChanges = ""
         for var in varList:
             newModelVar = "let " + var + ' = model.get("' + var + '");\n'
             modelVars += newModelVar
 
         for var in updatableVars:
             newModelChange = 'model.on("change:' + var + '", plotAfterInterval);\n'
             modelChanges += newModelChange
 
-        jsUrlStr = WebWidget.readFromWeb(jsUrl)
+        fileStr = fileReader(string)
         jsStr = """
         import * as d3 from "https://esm.sh/d3@7";
 
         function render({{ model, el }} ) {{
-            {jsUrlStr}
+            {fileStr}
             
             let timeout;
 
             function plotAfterInterval() {{
                 if (timeout) {{
                     clearTimeout(timeout);
                 }}
@@ -61,20 +82,14 @@
             window.addEventListener("resize", () => plotAfterInterval(this));
         }}
         
         
 
         export default {{ render }};
         """.format(
-            jsUrlStr=jsUrlStr,
+            fileStr=fileStr,
             modelVars=modelVars,
             widgetCall=widgetCall,
             modelChanges=modelChanges,
         )
 
         return jsStr
-
-    def linkData(self, widget, widgetAttr):
-        def callback(change):
-            self.data = getattr(widget, widgetAttr)
-
-        widget.observe(callback, names=[widgetAttr])
```

### Comparing `d3vis_ipynb-0.1.5/d3vis_ipynb/labextension/package.json` & `d3vis_ipynb-0.2.0/d3vis_ipynb/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9603365384615384%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.075b810a9929e45488a4.js'}}",*

 * * "'version'": "'0.2.0'"}*

```diff
@@ -16,15 +16,15 @@
         "lib/**/*.js",
         "dist/*.js",
         "css/*.css"
     ],
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.0a6c310552f16e38d4c2.js"
+            "load": "static/remoteEntry.075b810a9929e45488a4.js"
         },
         "extension": "lib/labplugin",
         "outputDir": "../d3vis_ipynb/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
@@ -54,9 +54,9 @@
         "export": "webpack --env export --config webpack.exports.config.js",
         "prepublish": "yarn run clean && yarn run build:prod",
         "start": "webpack serve --open --config webpack.exports.config.js",
         "start:export": "webpack serve --open --config webpack.exports.config.js --env export",
         "test": "echo \"Error: no test specified\" && exit 1",
         "watch": "webpack --watch --mode=development"
     },
-    "version": "0.1.5"
+    "version": "0.2.0"
 }
```

### Comparing `d3vis_ipynb-0.1.5/d3vis_ipynb/labextension/static/363.d9832b540bc5aa86432a.js` & `d3vis_ipynb-0.2.0/d3vis_ipynb/labextension/static/363.5fe76f6939929abf33b8.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -8,30 +8,30 @@
                 EmbeddingModel: () => C,
                 EmbeddingView: () => O,
                 HistogramPlotModel: () => D,
                 HistogramPlotView: () => j,
                 LinearHistPlotModel: () => M,
                 LinearHistPlotView: () => E,
                 RangeSliderModel: () => I,
-                RangeSliderView: () => B,
+                RangeSliderView: () => R,
                 ScatterPlotModel: () => L,
                 ScatterPlotView: () => A,
-                author: () => W.author,
-                dependencies: () => W.dependencies,
-                description: () => W.description,
-                devDependencies: () => W.devDependencies,
-                files: () => W.files,
-                jupyterlab: () => W.jupyterlab,
-                keywords: () => W.keywords,
-                license: () => W.license,
-                main: () => W.main,
-                name: () => W.name,
-                repository: () => W.repository,
-                scripts: () => W.scripts,
-                version: () => W.version
+                author: () => B.author,
+                dependencies: () => B.dependencies,
+                description: () => B.description,
+                devDependencies: () => B.devDependencies,
+                files: () => B.files,
+                jupyterlab: () => B.jupyterlab,
+                keywords: () => B.keywords,
+                license: () => B.license,
+                main: () => B.main,
+                name: () => B.name,
+                repository: () => B.repository,
+                scripts: () => B.scripts,
+                version: () => B.version
             });
             var a = n(801),
                 i = n(72),
                 o = n.n(i),
                 s = n(825),
                 r = n.n(s),
                 l = n(659),
@@ -156,37 +156,37 @@
                         ...super.defaults(),
                         _model_name: L.model_name,
                         _view_name: L.view_name,
                         _model_module: L.model_module,
                         _view_module: L.view_module,
                         _model_module_version: L.model_module_version,
                         _view_module_version: L.view_module_version,
-                        data: [],
+                        dataRecords: [],
                         x: String,
                         y: String,
                         hue: String,
                         elementId: String,
                         clickedValue: String,
-                        selectedValues: []
+                        selectedValuesRecords: []
                     }
                 }
                 static model_name = "ScatterplotModel";
                 static model_module = b.name;
                 static model_module_version = b.version;
                 static view_name = "ScatterplotView";
                 static view_module = b.name;
                 static view_module_version = b.version
             }
             class A extends a.DOMWidgetView {
                 timeout;
                 render() {
-                    k(this), this.model.on("change:data", (() => k(this)), this), this.model.on("change:x", (() => k(this)), this), this.model.on("change:y", (() => k(this)), this), this.model.on("change:hue", (() => k(this)), this), window.addEventListener("resize", (() => k(this)))
+                    k(this), this.model.on("change:dataRecords", (() => k(this)), this), this.model.on("change:x", (() => k(this)), this), this.model.on("change:y", (() => k(this)), this), this.model.on("change:hue", (() => k(this)), this), window.addEventListener("resize", (() => k(this)))
                 }
                 plot() {
-                    const e = this.model.get("data"),
+                    const e = this.model.get("dataRecords"),
                         t = this.model.get("x"),
                         n = this.model.get("y"),
                         a = this.model.get("hue"),
                         i = this.model.get("elementId");
                     let o = y,
                         s = this.el;
                     i && (s = document.getElementById(i), o = s.clientHeight);
@@ -270,29 +270,29 @@
                 setValue(e) {
                     this.model.set({
                         clickedValue: e
                     }), this.model.save_changes()
                 }
                 setSelectedValues(e) {
                     this.model.set({
-                        selectedValues: e
+                        selectedValuesRecords: e
                     }), this.model.save_changes()
                 }
             }
             class S extends a.DOMWidgetModel {
                 defaults() {
                     return {
                         ...super.defaults(),
                         _model_name: S.model_name,
                         _view_name: S.view_name,
                         _model_module: S.model_module,
                         _view_module: S.view_module,
                         _model_module_version: S.model_module_version,
                         _view_module_version: S.view_module_version,
-                        data: [],
+                        dataRecords: [],
                         x: String,
                         y: String,
                         hue: String,
                         elementId: String
                     }
                 }
                 static model_name = "BarplotModel";
@@ -301,30 +301,29 @@
                 static view_name = "BarplotView";
                 static view_module = b.name;
                 static view_module_version = b.version
             }
             class V extends a.DOMWidgetView {
                 timeout;
                 render() {
-                    k(this), this.model.on("change:data", (() => k(this)), this), this.model.on("change:x", (() => k(this)), this), this.model.on("change:y", (() => k(this)), this), this.model.on("change:hue", (() => k(this)), this), window.addEventListener("resize", (() => k(this)))
+                    k(this), this.model.on("change:dataRecords", (() => k(this)), this), this.model.on("change:x", (() => k(this)), this), this.model.on("change:y", (() => k(this)), this), this.model.on("change:hue", (() => k(this)), this), window.addEventListener("resize", (() => k(this)))
                 }
                 plot() {
-                    const e = this.model.get("data"),
+                    const e = this.model.get("dataRecords"),
                         t = this.model.get("x"),
                         n = this.model.get("y"),
                         a = this.model.get("hue"),
                         i = this.model.get("elementId");
-                    console.log("barplot"), console.log("elementId:"), console.log(i);
                     let o = y,
                         s = this.el;
                     i && (s = document.getElementById(i), o = s.clientHeight),
                         function(e, t, n, a, i, o, s, r) {
                             const l = o - r.left - r.right,
                                 d = s - r.top - r.bottom;
-                            console.log("element:"), console.log(i), console.log("width:"), console.log(o), console.log("height:"), console.log(s), _.select(i).selectAll("*").remove();
+                            _.select(i).selectAll("*").remove();
                             const c = _.select(i).append("svg").attr("width", o).attr("height", s).append("g").attr("transform", "translate(" + r.left + "," + r.top + ")");
                             a || (a = t);
                             const m = e.reduce(((e, t) => (e && -1 === e.indexOf(t[a]) && e.push(t[a]), e)), []),
                                 u = {},
                                 p = _.scaleOrdinal(_.schemeCategory10);
                             a == t ? function() {
                                 let a = e.reduce(((e, a) => {
@@ -480,15 +479,15 @@
                         ...super.defaults(),
                         _model_name: D.model_name,
                         _view_name: D.view_name,
                         _model_module: D.model_module,
                         _view_module: D.view_module,
                         _model_module_version: D.model_module_version,
                         _view_module_version: D.view_module_version,
-                        data: [],
+                        dataRecords: [],
                         x: String,
                         start: Number,
                         end: Number,
                         elementId: String
                     }
                 }
                 static model_name = "HistogramplotModel";
@@ -497,18 +496,18 @@
                 static view_name = "HistogramplotView";
                 static view_module = b.name;
                 static view_module_version = b.version
             }
             class j extends a.DOMWidgetView {
                 timeout;
                 render() {
-                    k(this), this.model.on("change:data", (() => k(this)), this), this.model.on("change:x", (() => k(this)), this), this.model.on("change:start", (() => k(this)), this), this.model.on("change:end", (() => k(this)), this), window.addEventListener("resize", (() => k(this)))
+                    k(this), this.model.on("change:dataRecords", (() => k(this)), this), this.model.on("change:x", (() => k(this)), this), this.model.on("change:start", (() => k(this)), this), this.model.on("change:end", (() => k(this)), this), window.addEventListener("resize", (() => k(this)))
                 }
                 plot() {
-                    const e = this.model.get("data"),
+                    const e = this.model.get("dataRecords"),
                         t = this.model.get("x"),
                         n = this.model.get("start"),
                         a = this.model.get("end"),
                         i = this.model.get("elementId");
                     let o = y,
                         s = this.el;
                     i && (s = document.getElementById(i), o = s.clientHeight),
@@ -563,28 +562,28 @@
                         n = this.model.get("grid_template_areas");
                     let a = this.model.get("style");
                     a || (a = "basic");
                     const i = document.createElement("div");
                     i.classList.add(a), i.style.display = "grid", i.style.gridTemplateAreas = n, i.style.gridTemplateRows = "repeat(" + e.length + ", 180px)", i.style.gridTemplateColumns = "repeat(" + e[0].length + ", 1fr)", i.style.width = "100%", t.forEach((e => {
                         const t = document.createElement("div");
                         t.setAttribute("id", e), t.style.gridArea = e, t.classList.add("dashboard-div"), i.appendChild(t)
-                    })), this.el.appendChild(i), console.log("Embedding:"), console.log(i)
+                    })), this.el.appendChild(i)
                 }
             }
             class I extends a.DOMWidgetModel {
                 defaults() {
                     return {
                         ...super.defaults(),
                         _model_name: I.model_name,
                         _view_name: I.view_name,
                         _model_module: I.model_module,
                         _view_module: I.view_module,
                         _model_module_version: I.model_module_version,
                         _view_module_version: I.view_module_version,
-                        data: [],
+                        dataRecords: [],
                         variable: String,
                         step: Number,
                         description: String,
                         minValue: Number,
                         maxValue: Number,
                         elementId: String
                     }
@@ -592,20 +591,20 @@
                 static model_name = "RangeSliderModel";
                 static model_module = b.name;
                 static model_module_version = b.version;
                 static view_name = "RangeSliderView";
                 static view_module = b.name;
                 static view_module_version = b.version
             }
-            class B extends a.DOMWidgetView {
+            class R extends a.DOMWidgetView {
                 render() {
-                    k(this), this.model.on("change:data", (() => k(this)), this), this.model.on("change:variable", (() => k(this)), this), this.model.on("change:step", (() => k(this)), this), this.model.on("change:description", (() => k(this)), this), window.addEventListener("resize", (() => k(this)))
+                    k(this), this.model.on("change:dataRecords", (() => k(this)), this), this.model.on("change:variable", (() => k(this)), this), this.model.on("change:step", (() => k(this)), this), this.model.on("change:description", (() => k(this)), this), window.addEventListener("resize", (() => k(this)))
                 }
                 plot() {
-                    const e = this.model.get("data"),
+                    const e = this.model.get("dataRecords"),
                         t = this.model.get("variable"),
                         n = this.model.get("step"),
                         a = this.model.get("description"),
                         i = this.model.get("elementId"),
                         o = this.model.get("minValue"),
                         s = this.model.get("maxValue");
                     let r = this.el;
@@ -651,25 +650,25 @@
                     this.model.set({
                         minValue: e
                     }), this.model.set({
                         maxValue: t
                     }), this.model.save_changes()
                 }
             }
-            var W = n(330)
+            var B = n(330)
         },
         930: (e, t, n) => {
             n.d(t, {
                 A: () => r
             });
             var a = n(601),
                 i = n.n(a),
                 o = n(314),
                 s = n.n(o)()(i());
-            s.push([e.id, '/***** EMBEDDING *****/\n.basic .dashboard-div {\n  border: 1px solid black;\n  text-align: center;\n}\n\n.dark .dashboard-div {\n  margin: 2px;\n  border-radius: 10px;\n  background-color: #262626;\n  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.5);\n}\n\n.glassmorphism .dashboard-div {\n  margin: 5px;\n  border-radius: 10px;\n  background: rgb(255, 254, 254);\n  border: 1px solid rgb(255, 255, 255);\n  backdrop-filter: blur(10px);\n  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);\n}\n\n.neumorphism .dashboard-div {\n  margin: 10px;\n  border-radius: 15px;\n  background-color: #e0e0e0;\n  box-shadow: 5px 5px 10px #bebebe, -5px -5px 10px #ffffff;\n}\n\n.minimalism .dashboard-div {\n  margin-bottom: 5px;\n}\n\n/***** RANGE SLIDER *****/\n.range_outside_container {\n  display: flex;\n  max-width: 500px;\n}\n\n.range_inside_container {\n  display: flex;\n  flex-direction: column;\n  width: 80%;\n}\n\n.range_description {\n  padding-right: 20px;\n}\n\n.range_value {\n  padding-left: 20px;\n  width: 80px;\n}\n\n.sliders_control {\n  position: relative;\n  min-height: 50px;\n}\n\ninput[type="range"]::-webkit-slider-thumb {\n  -webkit-appearance: none;\n  pointer-events: all;\n  width: 24px;\n  height: 24px;\n  background-color: #fff;\n  border-radius: 50%;\n  box-shadow: 0 0 0 1px #c6c6c6;\n  cursor: pointer;\n}\n\ninput[type="range"]::-moz-range-thumb {\n  -webkit-appearance: none;\n  pointer-events: all;\n  width: 24px;\n  height: 24px;\n  background-color: #fff;\n  border-radius: 50%;\n  box-shadow: 0 0 0 1px #c6c6c6;\n  cursor: pointer;\n}\n\ninput[type="range"]::-webkit-slider-thumb:hover {\n  background: #f7f7f7;\n}\n\ninput[type="range"]::-webkit-slider-thumb:active {\n  box-shadow: inset 0 0 3px #387bbe, 0 0 9px #387bbe;\n  -webkit-box-shadow: inset 0 0 3px #387bbe, 0 0 9px #387bbe;\n}\n\ninput[type="range"] {\n  -webkit-appearance: none;\n  appearance: none;\n  height: 10px;\n  width: 100%;\n  position: absolute;\n  background-color: #f79847;\n  pointer-events: none;\n}\n\n.top_slider {\n  height: 0 !important;\n  z-index: 1;\n  top: 5px;\n}\n', ""]);
+            s.push([e.id, '/***** EMBEDDING *****/\n.basic .dashboard-div {\n  border: 1px solid black;\n  text-align: center;\n}\n\n.dark .dashboard-div {\n  margin: 2px;\n  border-radius: 10px;\n  background-color: #262626;\n  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.5);\n}\n\n.glassmorphism .dashboard-div {\n  margin: 5px;\n  border-radius: 10px;\n  background: rgb(255, 254, 254);\n  border: 1px solid rgb(255, 255, 255);\n  backdrop-filter: blur(10px);\n  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);\n}\n\n.neumorphism .dashboard-div {\n  margin: 10px;\n  border-radius: 15px;\n  background-color: #e0e0e0;\n  box-shadow: 5px 5px 10px #bebebe, -5px -5px 10px #ffffff;\n}\n\n.minimalism .dashboard-div {\n  margin-bottom: 5px;\n}\n\n/***** RANGE SLIDER *****/\n.range_outside_container {\n  display: flex;\n  max-width: 500px;\n}\n\n.range_inside_container {\n  display: flex;\n  flex-direction: column;\n  width: 80%;\n}\n\n.range_description {\n  padding-right: 20px;\n}\n\n.range_value {\n  padding-left: 20px;\n  width: 80px;\n}\n\n.sliders_control {\n  position: relative;\n  min-height: 50px;\n}\n\ninput[type="range"]::-webkit-slider-thumb {\n  -webkit-appearance: none;\n  pointer-events: all;\n  width: 24px;\n  height: 24px;\n  background-color: #fff;\n  border: none !important;\n  border-radius: 50%;\n  box-shadow: 0 0 0 1px #c6c6c6;\n  cursor: pointer;\n}\n\ninput[type="range"]::-moz-range-thumb {\n  -webkit-appearance: none;\n  pointer-events: all;\n  width: 24px;\n  height: 24px;\n  background-color: #fff;\n  border-radius: 50%;\n  box-shadow: 0 0 0 1px #c6c6c6;\n  cursor: pointer;\n}\n\ninput[type="range"]::-webkit-slider-thumb:hover {\n  background: #f7f7f7;\n}\n\ninput[type="range"]::-webkit-slider-thumb:active {\n  box-shadow: inset 0 0 3px #387bbe, 0 0 9px #387bbe;\n  -webkit-box-shadow: inset 0 0 3px #387bbe, 0 0 9px #387bbe;\n}\n\ninput[type="range"] {\n  -webkit-appearance: none;\n  appearance: none;\n  height: 10px;\n  width: 100%;\n  position: absolute;\n  background-color: #f79847;\n  pointer-events: none;\n}\n\n.top_slider {\n  height: 0 !important;\n  z-index: 1;\n  top: 5px;\n}\n', ""]);
             const r = s
         },
         314: e => {
             e.exports = function(e) {
                 var t = [];
                 return t.toString = function() {
                     return this.map((function(t) {
@@ -829,11 +828,11 @@
                 else {
                     for (; t.firstChild;) t.removeChild(t.firstChild);
                     t.appendChild(document.createTextNode(e))
                 }
             }
         },
         330: e => {
-            e.exports = JSON.parse('{"name":"d3vis_ipynb","version":"0.1.5","description":"A Custom Jupyter Widget Library with visualizations created with D3.js.","author":"Daniel Adam Miranda","license":"BSD-3-Clause","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/H-IAAC/d3vis_ipynb.git"},"keywords":["jupyter","widgets","ipython","ipywidgets","jupyterlab-extension"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"scripts":{"clean":"rimraf dist/ && rimraf ../d3vis_ipynb/labextension/ && rimraf ../d3vis_ipynb/nbextension","prepublish":"yarn run clean && yarn run build:prod","build":"webpack --mode=development && yarn run build:labextension:dev","build:prod":"webpack --mode=production && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","watch":"webpack --watch --mode=development","start":"webpack serve --open --config webpack.exports.config.js","start:export":"webpack serve --open --config webpack.exports.config.js --env export","export":"webpack --env export --config webpack.exports.config.js","test":"echo \\"Error: no test specified\\" && exit 1"},"devDependencies":{"@jupyterlab/builder":"^4.0.6","html-webpack-plugin":"^5.6.0","rimraf":"^2.6.1","webpack":"^5","webpack-dev-server":"^5.0.2"},"dependencies":{"@jupyter-widgets/base":"^1.1 || ^2 || ^3 || ^4 || ^6","d3":"^7.9.0"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../d3vis_ipynb/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+            e.exports = JSON.parse('{"name":"d3vis_ipynb","version":"0.2.0","description":"A Custom Jupyter Widget Library with visualizations created with D3.js.","author":"Daniel Adam Miranda","license":"BSD-3-Clause","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/H-IAAC/d3vis_ipynb.git"},"keywords":["jupyter","widgets","ipython","ipywidgets","jupyterlab-extension"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"scripts":{"clean":"rimraf dist/ && rimraf ../d3vis_ipynb/labextension/ && rimraf ../d3vis_ipynb/nbextension","prepublish":"yarn run clean && yarn run build:prod","build":"webpack --mode=development && yarn run build:labextension:dev","build:prod":"webpack --mode=production && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","watch":"webpack --watch --mode=development","start":"webpack serve --open --config webpack.exports.config.js","start:export":"webpack serve --open --config webpack.exports.config.js --env export","export":"webpack --env export --config webpack.exports.config.js","test":"echo \\"Error: no test specified\\" && exit 1"},"devDependencies":{"@jupyterlab/builder":"^4.0.6","html-webpack-plugin":"^5.6.0","rimraf":"^2.6.1","webpack":"^5","webpack-dev-server":"^5.0.2"},"dependencies":{"@jupyter-widgets/base":"^1.1 || ^2 || ^3 || ^4 || ^6","d3":"^7.9.0"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../d3vis_ipynb/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
         }
     }
 ]);
```

### Comparing `d3vis_ipynb-0.1.5/d3vis_ipynb/labextension/static/493.053b071a46f0bcccaab9.js` & `d3vis_ipynb-0.2.0/d3vis_ipynb/labextension/static/493.053b071a46f0bcccaab9.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.5/d3vis_ipynb/labextension/static/693.c8409ce8329f6703470f.js` & `d3vis_ipynb-0.2.0/d3vis_ipynb/labextension/static/693.c8409ce8329f6703470f.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.5/d3vis_ipynb/labextension/static/remoteEntry.0a6c310552f16e38d4c2.js` & `d3vis_ipynb-0.2.0/d3vis_ipynb/labextension/static/remoteEntry.075b810a9929e45488a4.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, i, a, u, d, s, l, f, c, p, h, v, g, b, m, y, w = {
+    var e, r, t, n, o, i, a, u, d, s, l, f, p, c, h, v, g, b, m, y, w = {
             772: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(363).then((() => () => t(363))),
                         "./extension": () => Promise.all([t.e(363), t.e(493)]).then((() => () => t(493)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -42,19 +42,19 @@
         }), r
     }, E.d = (e, r) => {
         for (var t in r) E.o(r, t) && !E.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, E.f = {}, E.e = e => Promise.all(Object.keys(E.f).reduce(((r, t) => (E.f[t](e, r), r)), [])), E.u = e => e + "." + {
-        363: "d9832b540bc5aa86432a",
+        363: "5fe76f6939929abf33b8",
         493: "053b071a46f0bcccaab9",
         693: "c8409ce8329f6703470f"
     } [e] + ".js?v=" + {
-        363: "d9832b540bc5aa86432a",
+        363: "5fe76f6939929abf33b8",
         493: "053b071a46f0bcccaab9",
         693: "c8409ce8329f6703470f"
     } [e], E.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
@@ -70,19 +70,19 @@
                     if (l.getAttribute("src") == t || l.getAttribute("data-webpack") == r + o) {
                         a = l;
                         break
                     }
                 }
             a || (u = !0, (a = document.createElement("script")).charset = "utf-8", a.timeout = 120, E.nc && a.setAttribute("nonce", E.nc), a.setAttribute("data-webpack", r + o), a.src = t), e[t] = [n];
             var f = (r, n) => {
-                    a.onerror = a.onload = null, clearTimeout(c);
+                    a.onerror = a.onload = null, clearTimeout(p);
                     var o = e[t];
                     if (delete e[t], a.parentNode && a.parentNode.removeChild(a), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                c = setTimeout(f.bind(null, void 0, {
+                p = setTimeout(f.bind(null, void 0, {
                     type: "timeout",
                     target: a
                 }), 12e4);
             a.onerror = f.bind(null, a.onerror), a.onload = f.bind(null, a.onload), u && document.head.appendChild(a)
         }
     }, E.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
@@ -108,15 +108,15 @@
                         (!u || !u.loaded && (!n != !u.eager ? n : a > u.from)) && (o[r] = {
                             get: t,
                             from: a,
                             eager: !!n
                         })
                     },
                     d = [];
-                return "default" === t && (u("d3", "7.9.0", (() => E.e(693).then((() => () => E(693))))), u("d3vis_ipynb", "0.1.5", (() => E.e(363).then((() => () => E(363)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("d3", "7.9.0", (() => E.e(693).then((() => () => E(693))))), u("d3vis_ipynb", "0.2.0", (() => E.e(363).then((() => () => E(363)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         E.g.importScripts && (e = E.g.location + "");
         var r = E.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -187,42 +187,42 @@
                     d = !1, u--
                 } else {
                     if (u <= n || l < f != o) return !1;
                     d = !1
                 } else "s" != f && "n" != f && (d = !1, u--)
             }
         }
-        var c = [],
-            p = c.pop.bind(c);
+        var p = [],
+            c = p.pop.bind(p);
         for (a = 1; a < e.length; a++) {
             var h = e[a];
-            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? i(h, r) : !p())
+            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? i(h, r) : !c())
         }
-        return !!p()
+        return !!c()
     }, a = (e, r) => {
         var t = E.S[e];
         if (!t || !E.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
     }, d = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", s = (e, r, t, n) => {
         var o = u(e, t);
-        return i(n, o) || f(d(e, t, o, n)), c(e[t][o])
+        return i(n, o) || f(d(e, t, o, n)), p(e[t][o])
     }, l = (e, r, t) => {
         var o = e[r];
         return (r = Object.keys(o).reduce(((e, r) => !i(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
     }, f = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, c = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, n, o) {
+    }, p = e => (e.loaded = 1, e.get()), h = (c = e => function(r, t, n, o) {
         var i = E.I(r);
         return i && i.then ? i.then(e.bind(e, r, E.S[r], t, n, o)) : e(r, E.S[r], t, n, o)
-    })(((e, r, t, n) => (a(e, t), s(r, 0, t, n)))), v = p(((e, r, t, n, o) => {
+    })(((e, r, t, n) => (a(e, t), s(r, 0, t, n)))), v = c(((e, r, t, n, o) => {
         var i = r && E.o(r, t) && l(r, t, n);
-        return i ? c(i) : o()
+        return i ? p(i) : o()
     })), g = {}, b = {
         801: () => h("default", "@jupyter-widgets/base", [, [1, 6],
             [1, 4],
             [1, 3],
             [1, 2],
             [1, 1, 1], 1, 1, 1, 1
         ]),
```

### Comparing `d3vis_ipynb-0.1.5/d3vis_ipynb/labextension/static/third-party-licenses.json` & `d3vis_ipynb-0.2.0/d3vis_ipynb/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.5/d3vis_ipynb/nbextension/index.js` & `d3vis_ipynb-0.2.0/d3vis_ipynb/nbextension/index.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -5,15 +5,15 @@
                 n.d(e, {
                     A: () => s
                 });
                 var r = n(601),
                     i = n.n(r),
                     o = n(314),
                     a = n.n(o)()(i());
-                a.push([t.id, '/***** EMBEDDING *****/\n.basic .dashboard-div {\n  border: 1px solid black;\n  text-align: center;\n}\n\n.dark .dashboard-div {\n  margin: 2px;\n  border-radius: 10px;\n  background-color: #262626;\n  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.5);\n}\n\n.glassmorphism .dashboard-div {\n  margin: 5px;\n  border-radius: 10px;\n  background: rgb(255, 254, 254);\n  border: 1px solid rgb(255, 255, 255);\n  backdrop-filter: blur(10px);\n  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);\n}\n\n.neumorphism .dashboard-div {\n  margin: 10px;\n  border-radius: 15px;\n  background-color: #e0e0e0;\n  box-shadow: 5px 5px 10px #bebebe, -5px -5px 10px #ffffff;\n}\n\n.minimalism .dashboard-div {\n  margin-bottom: 5px;\n}\n\n/***** RANGE SLIDER *****/\n.range_outside_container {\n  display: flex;\n  max-width: 500px;\n}\n\n.range_inside_container {\n  display: flex;\n  flex-direction: column;\n  width: 80%;\n}\n\n.range_description {\n  padding-right: 20px;\n}\n\n.range_value {\n  padding-left: 20px;\n  width: 80px;\n}\n\n.sliders_control {\n  position: relative;\n  min-height: 50px;\n}\n\ninput[type="range"]::-webkit-slider-thumb {\n  -webkit-appearance: none;\n  pointer-events: all;\n  width: 24px;\n  height: 24px;\n  background-color: #fff;\n  border-radius: 50%;\n  box-shadow: 0 0 0 1px #c6c6c6;\n  cursor: pointer;\n}\n\ninput[type="range"]::-moz-range-thumb {\n  -webkit-appearance: none;\n  pointer-events: all;\n  width: 24px;\n  height: 24px;\n  background-color: #fff;\n  border-radius: 50%;\n  box-shadow: 0 0 0 1px #c6c6c6;\n  cursor: pointer;\n}\n\ninput[type="range"]::-webkit-slider-thumb:hover {\n  background: #f7f7f7;\n}\n\ninput[type="range"]::-webkit-slider-thumb:active {\n  box-shadow: inset 0 0 3px #387bbe, 0 0 9px #387bbe;\n  -webkit-box-shadow: inset 0 0 3px #387bbe, 0 0 9px #387bbe;\n}\n\ninput[type="range"] {\n  -webkit-appearance: none;\n  appearance: none;\n  height: 10px;\n  width: 100%;\n  position: absolute;\n  background-color: #f79847;\n  pointer-events: none;\n}\n\n.top_slider {\n  height: 0 !important;\n  z-index: 1;\n  top: 5px;\n}\n', ""]);
+                a.push([t.id, '/***** EMBEDDING *****/\n.basic .dashboard-div {\n  border: 1px solid black;\n  text-align: center;\n}\n\n.dark .dashboard-div {\n  margin: 2px;\n  border-radius: 10px;\n  background-color: #262626;\n  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.5);\n}\n\n.glassmorphism .dashboard-div {\n  margin: 5px;\n  border-radius: 10px;\n  background: rgb(255, 254, 254);\n  border: 1px solid rgb(255, 255, 255);\n  backdrop-filter: blur(10px);\n  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);\n}\n\n.neumorphism .dashboard-div {\n  margin: 10px;\n  border-radius: 15px;\n  background-color: #e0e0e0;\n  box-shadow: 5px 5px 10px #bebebe, -5px -5px 10px #ffffff;\n}\n\n.minimalism .dashboard-div {\n  margin-bottom: 5px;\n}\n\n/***** RANGE SLIDER *****/\n.range_outside_container {\n  display: flex;\n  max-width: 500px;\n}\n\n.range_inside_container {\n  display: flex;\n  flex-direction: column;\n  width: 80%;\n}\n\n.range_description {\n  padding-right: 20px;\n}\n\n.range_value {\n  padding-left: 20px;\n  width: 80px;\n}\n\n.sliders_control {\n  position: relative;\n  min-height: 50px;\n}\n\ninput[type="range"]::-webkit-slider-thumb {\n  -webkit-appearance: none;\n  pointer-events: all;\n  width: 24px;\n  height: 24px;\n  background-color: #fff;\n  border: none !important;\n  border-radius: 50%;\n  box-shadow: 0 0 0 1px #c6c6c6;\n  cursor: pointer;\n}\n\ninput[type="range"]::-moz-range-thumb {\n  -webkit-appearance: none;\n  pointer-events: all;\n  width: 24px;\n  height: 24px;\n  background-color: #fff;\n  border-radius: 50%;\n  box-shadow: 0 0 0 1px #c6c6c6;\n  cursor: pointer;\n}\n\ninput[type="range"]::-webkit-slider-thumb:hover {\n  background: #f7f7f7;\n}\n\ninput[type="range"]::-webkit-slider-thumb:active {\n  box-shadow: inset 0 0 3px #387bbe, 0 0 9px #387bbe;\n  -webkit-box-shadow: inset 0 0 3px #387bbe, 0 0 9px #387bbe;\n}\n\ninput[type="range"] {\n  -webkit-appearance: none;\n  appearance: none;\n  height: 10px;\n  width: 100%;\n  position: absolute;\n  background-color: #f79847;\n  pointer-events: none;\n}\n\n.top_slider {\n  height: 0 !important;\n  z-index: 1;\n  top: 5px;\n}\n', ""]);
                 const s = a
             },
             314: t => {
                 t.exports = function(t) {
                     var e = [];
                     return e.toString = function() {
                         return this.map((function(e) {
@@ -179,15 +179,15 @@
             55: t => {
                 t.exports = e
             },
             308: e => {
                 e.exports = t
             },
             330: t => {
-                t.exports = JSON.parse('{"name":"d3vis_ipynb","version":"0.1.5","description":"A Custom Jupyter Widget Library with visualizations created with D3.js.","author":"Daniel Adam Miranda","license":"BSD-3-Clause","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/H-IAAC/d3vis_ipynb.git"},"keywords":["jupyter","widgets","ipython","ipywidgets","jupyterlab-extension"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"scripts":{"clean":"rimraf dist/ && rimraf ../d3vis_ipynb/labextension/ && rimraf ../d3vis_ipynb/nbextension","prepublish":"yarn run clean && yarn run build:prod","build":"webpack --mode=development && yarn run build:labextension:dev","build:prod":"webpack --mode=production && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","watch":"webpack --watch --mode=development","start":"webpack serve --open --config webpack.exports.config.js","start:export":"webpack serve --open --config webpack.exports.config.js --env export","export":"webpack --env export --config webpack.exports.config.js","test":"echo \\"Error: no test specified\\" && exit 1"},"devDependencies":{"@jupyterlab/builder":"^4.0.6","html-webpack-plugin":"^5.6.0","rimraf":"^2.6.1","webpack":"^5","webpack-dev-server":"^5.0.2"},"dependencies":{"@jupyter-widgets/base":"^1.1 || ^2 || ^3 || ^4 || ^6","d3":"^7.9.0"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../d3vis_ipynb/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+                t.exports = JSON.parse('{"name":"d3vis_ipynb","version":"0.2.0","description":"A Custom Jupyter Widget Library with visualizations created with D3.js.","author":"Daniel Adam Miranda","license":"BSD-3-Clause","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/H-IAAC/d3vis_ipynb.git"},"keywords":["jupyter","widgets","ipython","ipywidgets","jupyterlab-extension"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"scripts":{"clean":"rimraf dist/ && rimraf ../d3vis_ipynb/labextension/ && rimraf ../d3vis_ipynb/nbextension","prepublish":"yarn run clean && yarn run build:prod","build":"webpack --mode=development && yarn run build:labextension:dev","build:prod":"webpack --mode=production && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","watch":"webpack --watch --mode=development","start":"webpack serve --open --config webpack.exports.config.js","start:export":"webpack serve --open --config webpack.exports.config.js --env export","export":"webpack --env export --config webpack.exports.config.js","test":"echo \\"Error: no test specified\\" && exit 1"},"devDependencies":{"@jupyterlab/builder":"^4.0.6","html-webpack-plugin":"^5.6.0","rimraf":"^2.6.1","webpack":"^5","webpack-dev-server":"^5.0.2"},"dependencies":{"@jupyter-widgets/base":"^1.1 || ^2 || ^3 || ^4 || ^6","d3":"^7.9.0"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../d3vis_ipynb/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
             }
         },
         r = {};
 
     function i(t) {
         var e = r[t];
         if (void 0 !== e) return e.exports;
@@ -219,37 +219,37 @@
         var t = i(308);
         const e = new URL(t.uri, document.location);
         e.pathname = e.pathname.slice(0, e.pathname.lastIndexOf("/") + 1), i.p = `${e.origin}${e.pathname}`
     })(), (() => {
         i.r(o), i.d(o, {
             BarPlotModel: () => Vi,
             BarPlotView: () => Li,
-            EmbeddingModel: () => qi,
-            EmbeddingView: () => Hi,
+            EmbeddingModel: () => Ri,
+            EmbeddingView: () => qi,
             HistogramPlotModel: () => Di,
             HistogramPlotView: () => Ii,
             LinearHistPlotModel: () => Ti,
             LinearHistPlotView: () => ji,
-            RangeSliderModel: () => zi,
-            RangeSliderView: () => Xi,
+            RangeSliderModel: () => Hi,
+            RangeSliderView: () => zi,
             ScatterPlotModel: () => Oi,
             ScatterPlotView: () => Pi,
-            author: () => Ri.author,
-            dependencies: () => Ri.dependencies,
-            description: () => Ri.description,
-            devDependencies: () => Ri.devDependencies,
-            files: () => Ri.files,
-            jupyterlab: () => Ri.jupyterlab,
-            keywords: () => Ri.keywords,
-            license: () => Ri.license,
-            main: () => Ri.main,
-            name: () => Ri.name,
-            repository: () => Ri.repository,
-            scripts: () => Ri.scripts,
-            version: () => Ri.version
+            author: () => Xi.author,
+            dependencies: () => Xi.dependencies,
+            description: () => Xi.description,
+            devDependencies: () => Xi.devDependencies,
+            files: () => Xi.files,
+            jupyterlab: () => Xi.jupyterlab,
+            keywords: () => Xi.keywords,
+            license: () => Xi.license,
+            main: () => Xi.main,
+            name: () => Xi.name,
+            repository: () => Xi.repository,
+            scripts: () => Xi.scripts,
+            version: () => Xi.version
         });
         var t = i(55),
             e = i(72),
             n = i.n(e),
             r = i(825),
             a = i.n(r),
             s = i(659),
@@ -454,21 +454,21 @@
             else {
                 let r = -1;
                 for (let i of t) null != (i = e(i, ++r, t)) && (n > i || void 0 === n && i >= i) && (n = i)
             }
             return n
         }
 
-        function q(t) {
+        function R(t) {
             return t
         }
-        var H = 1,
-            z = 2,
-            X = 3,
-            R = 4,
+        var q = 1,
+            H = 2,
+            z = 3,
+            X = 4,
             Y = 1e-6;
 
         function B(t) {
             return "translate(" + t + ",0)"
         }
 
         function F(t) {
@@ -491,41 +491,41 @@
             var n = [],
                 r = null,
                 i = null,
                 o = 6,
                 a = 6,
                 s = 3,
                 l = "undefined" != typeof window && window.devicePixelRatio > 1 ? 0 : .5,
-                u = t === H || t === R ? -1 : 1,
-                c = t === R || t === z ? "x" : "y",
-                h = t === H || t === X ? B : F;
+                u = t === q || t === X ? -1 : 1,
+                c = t === X || t === H ? "x" : "y",
+                h = t === q || t === z ? B : F;
 
             function f(f) {
                 var d = null == r ? e.ticks ? e.ticks.apply(e, n) : e.domain() : r,
-                    p = null == i ? e.tickFormat ? e.tickFormat.apply(e, n) : q : i,
+                    p = null == i ? e.tickFormat ? e.tickFormat.apply(e, n) : R : i,
                     m = Math.max(o, 0) + s,
                     _ = e.range(),
                     g = +_[0] + l,
                     v = +_[_.length - 1] + l,
                     y = (e.bandwidth ? U : W)(e.copy(), l),
                     w = f.selection ? f.selection() : f,
                     x = w.selectAll(".domain").data([null]),
                     b = w.selectAll(".tick").data(d, e).order(),
                     M = b.exit(),
                     k = b.enter().append("g").attr("class", "tick"),
                     A = b.select("line"),
                     E = b.select("text");
-                x = x.merge(x.enter().insert("path", ".tick").attr("class", "domain").attr("stroke", "currentColor")), b = b.merge(k), A = A.merge(k.append("line").attr("stroke", "currentColor").attr(c + "2", u * o)), E = E.merge(k.append("text").attr("fill", "currentColor").attr(c, u * m).attr("dy", t === H ? "0em" : t === X ? "0.71em" : "0.32em")), f !== w && (x = x.transition(f), b = b.transition(f), A = A.transition(f), E = E.transition(f), M = M.transition(f).attr("opacity", Y).attr("transform", (function(t) {
+                x = x.merge(x.enter().insert("path", ".tick").attr("class", "domain").attr("stroke", "currentColor")), b = b.merge(k), A = A.merge(k.append("line").attr("stroke", "currentColor").attr(c + "2", u * o)), E = E.merge(k.append("text").attr("fill", "currentColor").attr(c, u * m).attr("dy", t === q ? "0em" : t === z ? "0.71em" : "0.32em")), f !== w && (x = x.transition(f), b = b.transition(f), A = A.transition(f), E = E.transition(f), M = M.transition(f).attr("opacity", Y).attr("transform", (function(t) {
                     return isFinite(t = y(t)) ? h(t + l) : this.getAttribute("transform")
                 })), k.attr("opacity", Y).attr("transform", (function(t) {
                     var e = this.parentNode.__axis;
                     return h((e && isFinite(e = e(t)) ? e : y(t)) + l)
-                }))), M.remove(), x.attr("d", t === R || t === z ? a ? "M" + u * a + "," + g + "H" + l + "V" + v + "H" + u * a : "M" + l + "," + g + "V" + v : a ? "M" + g + "," + u * a + "V" + l + "H" + v + "V" + u * a : "M" + g + "," + l + "H" + v), b.attr("opacity", 1).attr("transform", (function(t) {
+                }))), M.remove(), x.attr("d", t === X || t === H ? a ? "M" + u * a + "," + g + "H" + l + "V" + v + "H" + u * a : "M" + l + "," + g + "V" + v : a ? "M" + g + "," + u * a + "V" + l + "H" + v + "V" + u * a : "M" + g + "," + l + "H" + v), b.attr("opacity", 1).attr("transform", (function(t) {
                     return h(y(t) + l)
-                })), A.attr(c + "2", u * o), E.attr(c, u * m).text(p), w.filter(G).attr("fill", "none").attr("font-size", 10).attr("font-family", "sans-serif").attr("text-anchor", t === z ? "start" : t === R ? "end" : "middle"), w.each((function() {
+                })), A.attr(c + "2", u * o), E.attr(c, u * m).text(p), w.filter(G).attr("fill", "none").attr("font-size", 10).attr("font-family", "sans-serif").attr("text-anchor", t === H ? "start" : t === X ? "end" : "middle"), w.each((function() {
                     this.__axis = y
                 }))
             }
             return f.scale = function(t) {
                 return arguments.length ? (e = t, f) : e
             }, f.ticks = function() {
                 return n = Array.from(arguments), f
@@ -545,19 +545,19 @@
                 return arguments.length ? (s = +t, f) : s
             }, f.offset = function(t) {
                 return arguments.length ? (l = +t, f) : l
             }, f
         }
 
         function Z(t) {
-            return J(X, t)
+            return J(z, t)
         }
 
         function K(t) {
-            return J(R, t)
+            return J(X, t)
         }
 
         function Q() {}
 
         function tt(t) {
             return null == t ? Q : function() {
                 return this.querySelector(t)
@@ -769,37 +769,37 @@
 
         function It(t) {
             return function() {
                 Lt(this, t)
             }
         }
 
-        function qt(t) {
+        function Rt(t) {
             return function() {
                 Dt(this, t)
             }
         }
 
-        function Ht(t, e) {
+        function qt(t, e) {
             return function() {
                 (e.apply(this, arguments) ? Lt : Dt)(this, t)
             }
         }
 
-        function zt() {
+        function Ht() {
             this.textContent = ""
         }
 
-        function Xt(t) {
+        function zt(t) {
             return function() {
                 this.textContent = t
             }
         }
 
-        function Rt(t) {
+        function Xt(t) {
             return function() {
                 var e = t.apply(this, arguments);
                 this.textContent = null == e ? "" : e
             }
         }
 
         function Yt() {
@@ -1084,18 +1084,18 @@
             classed: function(t, e) {
                 var n = Ot(t + "");
                 if (arguments.length < 2) {
                     for (var r = Pt(this.node()), i = -1, o = n.length; ++i < o;)
                         if (!r.contains(n[i])) return !1;
                     return !0
                 }
-                return this.each(("function" == typeof e ? Ht : e ? It : qt)(n, e))
+                return this.each(("function" == typeof e ? qt : e ? It : Rt)(n, e))
             },
             text: function(t) {
-                return arguments.length ? this.each(null == t ? zt : ("function" == typeof t ? Rt : Xt)(t)) : this.node().textContent
+                return arguments.length ? this.each(null == t ? Ht : ("function" == typeof t ? Xt : zt)(t)) : this.node().textContent
             },
             html: function(t) {
                 return arguments.length ? this.each(null == t ? Yt : ("function" == typeof t ? Ft : Bt)(t)) : this.node().innerHTML
             },
             raise: function() {
                 return this.each(Wt)
             },
@@ -1301,35 +1301,35 @@
             stop: function() {
                 this._call && (this._call = null, this._time = 1 / 0, Pe())
             }
         };
         var Le = _e("start", "end", "cancel", "interrupt"),
             De = [],
             Ie = 0,
-            qe = 3;
+            Re = 3;
 
-        function He(t, e, n, r, i, o) {
+        function qe(t, e, n, r, i, o) {
             var a = t.__transition;
             if (a) {
                 if (n in a) return
             } else t.__transition = {};
             ! function(t, e, n) {
                 var r, i = t.__transition;
 
                 function o(l) {
                     var u, c, h, f;
                     if (1 !== n.state) return s();
                     for (u in i)
                         if ((f = i[u]).name === n.name) {
-                            if (f.state === qe) return Ve(o);
+                            if (f.state === Re) return Ve(o);
                             4 === f.state ? (f.state = 6, f.timer.stop(), f.on.call("interrupt", t, t.__data__, f.index, f.group), delete i[u]) : +u < e && (f.state = 6, f.timer.stop(), f.on.call("cancel", t, t.__data__, f.index, f.group), delete i[u])
                         } if (Ve((function() {
-                            n.state === qe && (n.state = 4, n.timer.restart(a, n.delay, n.time), a(l))
+                            n.state === Re && (n.state = 4, n.timer.restart(a, n.delay, n.time), a(l))
                         })), n.state = 2, n.on.call("start", t, t.__data__, n.index, n.group), 2 === n.state) {
-                        for (n.state = qe, r = new Array(h = n.tween.length), u = 0, c = -1; u < h; ++u)(f = n.tween[u].value.call(t, t.__data__, n.index, n.group)) && (r[++c] = f);
+                        for (n.state = Re, r = new Array(h = n.tween.length), u = 0, c = -1; u < h; ++u)(f = n.tween[u].value.call(t, t.__data__, n.index, n.group)) && (r[++c] = f);
                         r.length = c + 1
                     }
                 }
 
                 function a(e) {
                     for (var i = e < n.duration ? n.ease.call(null, e / n.duration) : (n.timer.restart(s), n.state = 5, 1), o = -1, a = r.length; ++o < a;) r[o].call(t, i);
                     5 === n.state && (n.on.call("end", t, t.__data__, n.index, n.group), s())
@@ -1353,27 +1353,27 @@
                 duration: o.duration,
                 ease: o.ease,
                 timer: null,
                 state: Ie
             })
         }
 
-        function ze(t, e) {
-            var n = Re(t, e);
+        function He(t, e) {
+            var n = Xe(t, e);
             if (n.state > Ie) throw new Error("too late; already scheduled");
             return n
         }
 
-        function Xe(t, e) {
-            var n = Re(t, e);
-            if (n.state > qe) throw new Error("too late; already running");
+        function ze(t, e) {
+            var n = Xe(t, e);
+            if (n.state > Re) throw new Error("too late; already running");
             return n
         }
 
-        function Re(t, e) {
+        function Xe(t, e) {
             var n = t.__transition;
             if (!n || !(n = n[e])) throw new Error("transition not found");
             return n
         }
 
         function Ye(t, e) {
             return t = +t, e = +e,
@@ -1460,30 +1460,30 @@
             Ze = Ge((function(t) {
                 return null == t ? We : (Be || (Be = document.createElementNS("http://www.w3.org/2000/svg", "g")), Be.setAttribute("transform", t), (t = Be.transform.baseVal.consolidate()) ? Ue((t = t.matrix).a, t.b, t.c, t.d, t.e, t.f) : We)
             }), ", ", ")", ")");
 
         function Ke(t, e) {
             var n, r;
             return function() {
-                var i = Xe(this, t),
+                var i = ze(this, t),
                     o = i.tween;
                 if (o !== n)
                     for (var a = 0, s = (r = n = o).length; a < s; ++a)
                         if (r[a].name === e) {
                             (r = r.slice()).splice(a, 1);
                             break
                         } i.tween = r
             }
         }
 
         function Qe(t, e, n) {
             var r, i;
             if ("function" != typeof n) throw new Error;
             return function() {
-                var o = Xe(this, t),
+                var o = ze(this, t),
                     a = o.tween;
                 if (a !== r) {
                     i = (r = a).slice();
                     for (var s = {
                             name: e,
                             value: n
                         }, l = 0, u = i.length; l < u; ++l)
@@ -1495,19 +1495,19 @@
                 o.tween = i
             }
         }
 
         function tn(t, e, n) {
             var r = t._id;
             return t.each((function() {
-                    var t = Xe(this, r);
+                    var t = ze(this, r);
                     (t.value || (t.value = {}))[e] = n.apply(this, arguments)
                 })),
                 function(t) {
-                    return Re(t, r).value[e]
+                    return Xe(t, r).value[e]
                 }
         }
 
         function en(t, e, n) {
             t.prototype = e.prototype = n, n.constructor = t
         }
 
@@ -1846,15 +1846,15 @@
             var n = e - t;
             return n ? function(t, e) {
                 return function(n) {
                     return t + n * e
                 }
             }(t, n) : Dn(isNaN(t) ? e : t)
         }
-        const qn = function t(e) {
+        const Rn = function t(e) {
             var n = function(t) {
                 return 1 == (t = +t) ? In : function(e, n) {
                     return n - e ? function(t, e, n) {
                         return t = Math.pow(t, n), e = Math.pow(e, n) - t, n = 1 / n,
                             function(r) {
                                 return Math.pow(t + r * e, n)
                             }
@@ -1870,61 +1870,61 @@
                 return function(e) {
                     return t.r = r(e), t.g = i(e), t.b = o(e), t.opacity = a(e), t + ""
                 }
             }
             return r.gamma = t, r
         }(1);
 
-        function Hn(t) {
+        function qn(t) {
             return function(e) {
                 var n, r, i = e.length,
                     o = new Array(i),
                     a = new Array(i),
                     s = new Array(i);
                 for (n = 0; n < i; ++n) r = Mn(e[n]), o[n] = r.r || 0, a[n] = r.g || 0, s[n] = r.b || 0;
                 return o = t(o), a = t(a), s = t(s), r.opacity = 1,
                     function(t) {
                         return r.r = o(t), r.g = a(t), r.b = s(t), r + ""
                     }
             }
         }
-        Hn((function(t) {
+        qn((function(t) {
             var e = t.length - 1;
             return function(n) {
                 var r = n <= 0 ? n = 0 : n >= 1 ? (n = 1, e - 1) : Math.floor(n * e),
                     i = t[r],
                     o = t[r + 1],
                     a = r > 0 ? t[r - 1] : 2 * i - o,
                     s = r < e - 1 ? t[r + 2] : 2 * o - i;
                 return Ln((n - r / e) * e, a, i, o, s)
             }
-        })), Hn((function(t) {
+        })), qn((function(t) {
             var e = t.length;
             return function(n) {
                 var r = Math.floor(((n %= 1) < 0 ? ++n : n) * e),
                     i = t[(r + e - 1) % e],
                     o = t[r % e],
                     a = t[(r + 1) % e],
                     s = t[(r + 2) % e];
                 return Ln((n - r / e) * e, i, o, a, s)
             }
         }));
-        var zn = /[-+]?(?:\d+\.?\d*|\.?\d+)(?:[eE][-+]?\d+)?/g,
-            Xn = new RegExp(zn.source, "g");
+        var Hn = /[-+]?(?:\d+\.?\d*|\.?\d+)(?:[eE][-+]?\d+)?/g,
+            zn = new RegExp(Hn.source, "g");
 
-        function Rn(t, e) {
-            var n, r, i, o = zn.lastIndex = Xn.lastIndex = 0,
+        function Xn(t, e) {
+            var n, r, i, o = Hn.lastIndex = zn.lastIndex = 0,
                 a = -1,
                 s = [],
                 l = [];
             for (t += "", e += "";
-                (n = zn.exec(t)) && (r = Xn.exec(e));)(i = r.index) > o && (i = e.slice(o, i), s[a] ? s[a] += i : s[++a] = i), (n = n[0]) === (r = r[0]) ? s[a] ? s[a] += r : s[++a] = r : (s[++a] = null, l.push({
+                (n = Hn.exec(t)) && (r = zn.exec(e));)(i = r.index) > o && (i = e.slice(o, i), s[a] ? s[a] += i : s[++a] = i), (n = n[0]) === (r = r[0]) ? s[a] ? s[a] += r : s[++a] = r : (s[++a] = null, l.push({
                 i: a,
                 x: Ye(n, r)
-            })), o = Xn.lastIndex;
+            })), o = zn.lastIndex;
             return o < e.length && (i = e.slice(o), s[a] ? s[a] += i : s[++a] = i), s.length < 2 ? l[0] ? function(t) {
                 return function(e) {
                     return t(e) + ""
                 }
             }(l[0].x) : function(t) {
                 return function() {
                     return t
@@ -1933,15 +1933,15 @@
                 for (var n, r = 0; r < e; ++r) s[(n = l[r]).i] = n.x(t);
                 return s.join("")
             })
         }
 
         function Yn(t, e) {
             var n;
-            return ("number" == typeof e ? Ye : e instanceof wn ? qn : (n = wn(e)) ? (e = n, qn) : Rn)(t, e)
+            return ("number" == typeof e ? Ye : e instanceof wn ? Rn : (n = wn(e)) ? (e = n, Rn) : Xn)(t, e)
         }
 
         function Bn(t) {
             return function() {
                 this.removeAttribute(t)
             }
         }
@@ -2012,35 +2012,35 @@
                 }(t, i)), n
             }
             return i._value = e, i
         }
 
         function Qn(t, e) {
             return function() {
-                ze(this, t).delay = +e.apply(this, arguments)
+                He(this, t).delay = +e.apply(this, arguments)
             }
         }
 
         function tr(t, e) {
             return e = +e,
                 function() {
-                    ze(this, t).delay = e
+                    He(this, t).delay = e
                 }
         }
 
         function er(t, e) {
             return function() {
-                Xe(this, t).duration = +e.apply(this, arguments)
+                ze(this, t).duration = +e.apply(this, arguments)
             }
         }
 
         function nr(t, e) {
             return e = +e,
                 function() {
-                    Xe(this, t).duration = e
+                    ze(this, t).duration = e
                 }
         }
         var rr = ce.prototype.constructor;
 
         function ir(t) {
             return function() {
                 this.style.removeProperty(t)
@@ -2061,25 +2061,25 @@
         }.prototype = {
             constructor: ar,
             select: function(t) {
                 var e = this._name,
                     n = this._id;
                 "function" != typeof t && (t = tt(t));
                 for (var r = this._groups, i = r.length, o = new Array(i), a = 0; a < i; ++a)
-                    for (var s, l, u = r[a], c = u.length, h = o[a] = new Array(c), f = 0; f < c; ++f)(s = u[f]) && (l = t.call(s, s.__data__, f, u)) && ("__data__" in s && (l.__data__ = s.__data__), h[f] = l, He(h[f], e, n, f, h, Re(s, n)));
+                    for (var s, l, u = r[a], c = u.length, h = o[a] = new Array(c), f = 0; f < c; ++f)(s = u[f]) && (l = t.call(s, s.__data__, f, u)) && ("__data__" in s && (l.__data__ = s.__data__), h[f] = l, qe(h[f], e, n, f, h, Xe(s, n)));
                 return new ar(o, this._parents, e, n)
             },
             selectAll: function(t) {
                 var e = this._name,
                     n = this._id;
                 "function" != typeof t && (t = nt(t));
                 for (var r = this._groups, i = r.length, o = [], a = [], s = 0; s < i; ++s)
                     for (var l, u = r[s], c = u.length, h = 0; h < c; ++h)
                         if (l = u[h]) {
-                            for (var f, d = t.call(l, l.__data__, h, u), p = Re(l, n), m = 0, _ = d.length; m < _; ++m)(f = d[m]) && He(f, e, n, m, d, p);
+                            for (var f, d = t.call(l, l.__data__, h, u), p = Xe(l, n), m = 0, _ = d.length; m < _; ++m)(f = d[m]) && qe(f, e, n, m, d, p);
                             o.push(d), a.push(l)
                         } return new ar(o, a, e, n)
             },
             selectChild: lr.selectChild,
             selectChildren: lr.selectChildren,
             filter: function(t) {
                 "function" != typeof t && (t = rt(t));
@@ -2097,16 +2097,16 @@
             selection: function() {
                 return new rr(this._groups, this._parents)
             },
             transition: function() {
                 for (var t = this._name, e = this._id, n = sr(), r = this._groups, i = r.length, o = 0; o < i; ++o)
                     for (var a, s = r[o], l = s.length, u = 0; u < l; ++u)
                         if (a = s[u]) {
-                            var c = Re(a, e);
-                            He(a, t, n, u, s, {
+                            var c = Xe(a, e);
+                            qe(a, t, n, u, s, {
                                 time: c.time + c.delay + c.duration,
                                 delay: 0,
                                 duration: c.duration,
                                 ease: c.ease
                             })
                         } return new ar(r, this._parents, t, n)
             },
@@ -2114,21 +2114,21 @@
             nodes: lr.nodes,
             node: lr.node,
             size: lr.size,
             empty: lr.empty,
             each: lr.each,
             on: function(t, e) {
                 var n = this._id;
-                return arguments.length < 2 ? Re(this.node(), n).on.on(t) : this.each(function(t, e, n) {
+                return arguments.length < 2 ? Xe(this.node(), n).on.on(t) : this.each(function(t, e, n) {
                     var r, i, o = function(t) {
                         return (t + "").trim().split(/^|\s+/).every((function(t) {
                             var e = t.indexOf(".");
                             return e >= 0 && (t = t.slice(0, e)), !t || "start" === t
                         }))
-                    }(e) ? ze : Xe;
+                    }(e) ? He : ze;
                     return function() {
                         var a = o(this, t),
                             s = a.on;
                         s !== r && (i = (r = s).copy()).on(e, n), a.on = i
                     }
                 }(n, t, e))
             },
@@ -2162,15 +2162,15 @@
                             l = s + "";
                         return null == s && (this.style.removeProperty(t), l = s = $t(this, t)), a === l ? null : a === r && l === i ? o : (i = l, o = e(r = a, s))
                     }
                 }(t, r, tn(this, "style." + t, e))).each(function(t, e) {
                     var n, r, i, o, a = "style." + e,
                         s = "end." + a;
                     return function() {
-                        var l = Xe(this, t),
+                        var l = ze(this, t),
                             u = l.on,
                             c = null == l.value[a] ? o || (o = ir(e)) : void 0;
                         u === n && i === c || (r = (n = u).copy()).on(s, i = c), l.on = r
                     }
                 }(this._id, t)) : this.styleTween(t, function(t, e, n) {
                     var r, i, o = n + "";
                     return function() {
@@ -2238,44 +2238,44 @@
                         e && e.removeChild(this)
                     }
                 }(this._id))
             },
             tween: function(t, e) {
                 var n = this._id;
                 if (t += "", arguments.length < 2) {
-                    for (var r, i = Re(this.node(), n).tween, o = 0, a = i.length; o < a; ++o)
+                    for (var r, i = Xe(this.node(), n).tween, o = 0, a = i.length; o < a; ++o)
                         if ((r = i[o]).name === t) return r.value;
                     return null
                 }
                 return this.each((null == e ? Ke : Qe)(n, t, e))
             },
             delay: function(t) {
                 var e = this._id;
-                return arguments.length ? this.each(("function" == typeof t ? Qn : tr)(e, t)) : Re(this.node(), e).delay
+                return arguments.length ? this.each(("function" == typeof t ? Qn : tr)(e, t)) : Xe(this.node(), e).delay
             },
             duration: function(t) {
                 var e = this._id;
-                return arguments.length ? this.each(("function" == typeof t ? er : nr)(e, t)) : Re(this.node(), e).duration
+                return arguments.length ? this.each(("function" == typeof t ? er : nr)(e, t)) : Xe(this.node(), e).duration
             },
             ease: function(t) {
                 var e = this._id;
                 return arguments.length ? this.each(function(t, e) {
                     if ("function" != typeof e) throw new Error;
                     return function() {
-                        Xe(this, t).ease = e
+                        ze(this, t).ease = e
                     }
-                }(e, t)) : Re(this.node(), e).ease
+                }(e, t)) : Xe(this.node(), e).ease
             },
             easeVarying: function(t) {
                 if ("function" != typeof t) throw new Error;
                 return this.each(function(t, e) {
                     return function() {
                         var n = e.apply(this, arguments);
                         if ("function" != typeof n) throw new Error;
-                        Xe(this, t).ease = n
+                        ze(this, t).ease = n
                     }
                 }(this._id, t))
             },
             end: function() {
                 var t, e, n = this,
                     r = n._id,
                     i = n.size();
@@ -2285,15 +2285,15 @@
                         },
                         l = {
                             value: function() {
                                 0 == --i && o()
                             }
                         };
                     n.each((function() {
-                        var n = Xe(this, r),
+                        var n = ze(this, r),
                             i = n.on;
                         i !== t && ((e = (t = i).copy())._.cancel.push(s), e._.interrupt.push(s), e._.end.push(l)), n.on = e
                     })), 0 === i && o()
                 }))
             },
             [Symbol.iterator]: lr[Symbol.iterator]
         };
@@ -2322,15 +2322,15 @@
                     }
                 }(this, t)
             }))
         }, ce.prototype.transition = function(t) {
             var e, n;
             t instanceof ar ? (e = t._id, t = t._name) : (e = sr(), (n = ur).time = Se(), t = null == t ? null : t + "");
             for (var r = this._groups, i = r.length, o = 0; o < i; ++o)
-                for (var a, s = r[o], l = s.length, u = 0; u < l; ++u)(a = s[u]) && He(a, t, e, u, s, n || cr(a, e));
+                for (var a, s = r[o], l = s.length, u = 0; u < l; ++u)(a = s[u]) && qe(a, t, e, u, s, n || cr(a, e));
             return new ar(r, this._parents, t, e)
         };
         const {
             abs: hr,
             max: fr,
             min: dr
         } = Math;
@@ -2658,59 +2658,59 @@
                 for (n = 0; n < r; ++n) i[n] = t[n] * (1 - o) + e[n] * o;
                 return i
             }
         }
 
         function Ir(t, e) {
             var n, r, i = typeof e;
-            return null == e || "boolean" === i ? Dn(e) : ("number" === i ? Ye : "string" === i ? (n = wn(e)) ? (e = n, qn) : Rn : e instanceof wn ? qn : e instanceof Date ? Vr : (r = e, !ArrayBuffer.isView(r) || r instanceof DataView ? Array.isArray(e) ? Pr : "function" != typeof e.valueOf && "function" != typeof e.toString || isNaN(e) ? Lr : Ye : Dr))(t, e)
+            return null == e || "boolean" === i ? Dn(e) : ("number" === i ? Ye : "string" === i ? (n = wn(e)) ? (e = n, Rn) : Xn : e instanceof wn ? Rn : e instanceof Date ? Vr : (r = e, !ArrayBuffer.isView(r) || r instanceof DataView ? Array.isArray(e) ? Pr : "function" != typeof e.valueOf && "function" != typeof e.toString || isNaN(e) ? Lr : Ye : Dr))(t, e)
         }
 
-        function qr(t, e) {
+        function Rr(t, e) {
             return t = +t, e = +e,
                 function(n) {
                     return Math.round(t * (1 - n) + e * n)
                 }
         }
 
-        function Hr(t) {
+        function qr(t) {
             return +t
         }
-        var zr = [0, 1];
+        var Hr = [0, 1];
 
-        function Xr(t) {
+        function zr(t) {
             return t
         }
 
-        function Rr(t, e) {
+        function Xr(t, e) {
             return (e -= t = +t) ? function(n) {
                 return (n - t) / e
             } : (n = isNaN(e) ? NaN : .5, function() {
                 return n
             });
             var n
         }
 
         function Yr(t, e, n) {
             var r = t[0],
                 i = t[1],
                 o = e[0],
                 a = e[1];
-            return i < r ? (r = Rr(i, r), o = n(a, o)) : (r = Rr(r, i), o = n(o, a)),
+            return i < r ? (r = Xr(i, r), o = n(a, o)) : (r = Xr(r, i), o = n(o, a)),
                 function(t) {
                     return o(r(t))
                 }
         }
 
         function Br(t, e, n) {
             var r = Math.min(t.length, e.length) - 1,
                 i = new Array(r),
                 o = new Array(r),
                 a = -1;
-            for (t[r] < t[0] && (t = t.slice().reverse(), e = e.slice().reverse()); ++a < r;) i[a] = Rr(t[a], t[a + 1]), o[a] = n(e[a], e[a + 1]);
+            for (t[r] < t[0] && (t = t.slice().reverse(), e = e.slice().reverse()); ++a < r;) i[a] = Xr(t[a], t[a + 1]), o[a] = n(e[a], e[a + 1]);
             return function(e) {
                 var n = E(t, e, 1, r) - 1;
                 return o[n](i[n](e))
             }
         }
         var Fr, Wr = /^(?:(.)?([<>=^]))?([+\-( ])?([$#])?(0)?(\d+)?(,)?(\.\d+)?(~)?([a-z%])?$/i;
 
@@ -2785,48 +2785,48 @@
             return t
         }
         var ei, ni, ri, ii = Array.prototype.map,
             oi = ["y", "z", "a", "f", "p", "n", "µ", "m", "", "k", "M", "G", "T", "P", "E", "Z", "Y"];
 
         function ai() {
             var t = function() {
-                var t, e, n, r, i, o, a = zr,
-                    s = zr,
+                var t, e, n, r, i, o, a = Hr,
+                    s = Hr,
                     l = Ir,
-                    u = Xr;
+                    u = zr;
 
                 function c() {
                     var t, e, n, l = Math.min(a.length, s.length);
-                    return u !== Xr && (t = a[0], e = a[l - 1], t > e && (n = t, t = e, e = n), u = function(n) {
+                    return u !== zr && (t = a[0], e = a[l - 1], t > e && (n = t, t = e, e = n), u = function(n) {
                         return Math.max(t, Math.min(e, n))
                     }), r = l > 2 ? Br : Yr, i = o = null, h
                 }
 
                 function h(e) {
                     return null == e || isNaN(e = +e) ? n : (i || (i = r(a.map(t), s, l)))(t(u(e)))
                 }
                 return h.invert = function(n) {
                         return u(e((o || (o = r(s, a.map(t), Ye)))(n)))
                     }, h.domain = function(t) {
-                        return arguments.length ? (a = Array.from(t, Hr), c()) : a.slice()
+                        return arguments.length ? (a = Array.from(t, qr), c()) : a.slice()
                     }, h.range = function(t) {
                         return arguments.length ? (s = Array.from(t), c()) : s.slice()
                     }, h.rangeRound = function(t) {
-                        return s = Array.from(t), l = qr, c()
+                        return s = Array.from(t), l = Rr, c()
                     }, h.clamp = function(t) {
-                        return arguments.length ? (u = !!t || Xr, c()) : u !== Xr
+                        return arguments.length ? (u = !!t || zr, c()) : u !== zr
                     }, h.interpolate = function(t) {
                         return arguments.length ? (l = t, c()) : l
                     }, h.unknown = function(t) {
                         return arguments.length ? (n = t, h) : n
                     },
                     function(n, r) {
                         return t = n, e = r, c()
                     }
-            }()(Xr, Xr);
+            }()(zr, zr);
             return t.copy = function() {
                     return e = t, ai().domain(e.domain()).range(e.range()).interpolate(e.interpolate()).clamp(e.clamp()).unknown(e.unknown());
                     var e
                 }, Nr.apply(t, arguments),
                 function(t) {
                     var e = t.domain;
                     return t.ticks = function(t) {
@@ -3572,37 +3572,37 @@
                     ...super.defaults(),
                     _model_name: Oi.model_name,
                     _view_name: Oi.view_name,
                     _model_module: Oi.model_module,
                     _view_module: Oi.view_module,
                     _model_module_version: Oi.model_module_version,
                     _view_module_version: Oi.view_module_version,
-                    data: [],
+                    dataRecords: [],
                     x: String,
                     y: String,
                     hue: String,
                     elementId: String,
                     clickedValue: String,
-                    selectedValues: []
+                    selectedValuesRecords: []
                 }
             }
             static model_name = "ScatterplotModel";
             static model_module = Ni.name;
             static model_module_version = Ni.version;
             static view_name = "ScatterplotView";
             static view_module = Ni.name;
             static view_module_version = Ni.version
         }
         class Pi extends t.DOMWidgetView {
             timeout;
             render() {
-                Ci(this), this.model.on("change:data", (() => Ci(this)), this), this.model.on("change:x", (() => Ci(this)), this), this.model.on("change:y", (() => Ci(this)), this), this.model.on("change:hue", (() => Ci(this)), this), window.addEventListener("resize", (() => Ci(this)))
+                Ci(this), this.model.on("change:dataRecords", (() => Ci(this)), this), this.model.on("change:x", (() => Ci(this)), this), this.model.on("change:y", (() => Ci(this)), this), this.model.on("change:hue", (() => Ci(this)), this), window.addEventListener("resize", (() => Ci(this)))
             }
             plot() {
-                const t = this.model.get("data"),
+                const t = this.model.get("dataRecords"),
                     e = this.model.get("x"),
                     n = this.model.get("y"),
                     r = this.model.get("hue"),
                     i = this.model.get("elementId");
                 let o = Si,
                     a = this.el;
                 i && (a = document.getElementById(i), o = a.clientHeight);
@@ -3659,29 +3659,29 @@
             setValue(t) {
                 this.model.set({
                     clickedValue: t
                 }), this.model.save_changes()
             }
             setSelectedValues(t) {
                 this.model.set({
-                    selectedValues: t
+                    selectedValuesRecords: t
                 }), this.model.save_changes()
             }
         }
         class Vi extends t.DOMWidgetModel {
             defaults() {
                 return {
                     ...super.defaults(),
                     _model_name: Vi.model_name,
                     _view_name: Vi.view_name,
                     _model_module: Vi.model_module,
                     _view_module: Vi.view_module,
                     _model_module_version: Vi.model_module_version,
                     _view_module_version: Vi.view_module_version,
-                    data: [],
+                    dataRecords: [],
                     x: String,
                     y: String,
                     hue: String,
                     elementId: String
                 }
             }
             static model_name = "BarplotModel";
@@ -3690,30 +3690,29 @@
             static view_name = "BarplotView";
             static view_module = Ni.name;
             static view_module_version = Ni.version
         }
         class Li extends t.DOMWidgetView {
             timeout;
             render() {
-                Ci(this), this.model.on("change:data", (() => Ci(this)), this), this.model.on("change:x", (() => Ci(this)), this), this.model.on("change:y", (() => Ci(this)), this), this.model.on("change:hue", (() => Ci(this)), this), window.addEventListener("resize", (() => Ci(this)))
+                Ci(this), this.model.on("change:dataRecords", (() => Ci(this)), this), this.model.on("change:x", (() => Ci(this)), this), this.model.on("change:y", (() => Ci(this)), this), this.model.on("change:hue", (() => Ci(this)), this), window.addEventListener("resize", (() => Ci(this)))
             }
             plot() {
-                const t = this.model.get("data"),
+                const t = this.model.get("dataRecords"),
                     e = this.model.get("x"),
                     n = this.model.get("y"),
                     r = this.model.get("hue"),
                     i = this.model.get("elementId");
-                console.log("barplot"), console.log("elementId:"), console.log(i);
                 let o = Si,
                     a = this.el;
                 i && (a = document.getElementById(i), o = a.clientHeight),
                     function(t, e, n, r, i, o, a, s) {
                         const l = o - s.left - s.right,
                             u = a - s.top - s.bottom;
-                        console.log("element:"), console.log(i), console.log("width:"), console.log(o), console.log("height:"), console.log(a), mr(i).selectAll("*").remove();
+                        mr(i).selectAll("*").remove();
                         const c = mr(i).append("svg").attr("width", o).attr("height", a).append("g").attr("transform", "translate(" + s.left + "," + s.top + ")");
                         r || (r = e);
                         const h = t.reduce(((t, e) => (t && -1 === t.indexOf(e[r]) && t.push(e[r]), t)), []),
                             f = {},
                             d = jr(si);
                         r == e ? function() {
                             let r = t.reduce(((t, r) => {
@@ -3869,15 +3868,15 @@
                     ...super.defaults(),
                     _model_name: Di.model_name,
                     _view_name: Di.view_name,
                     _model_module: Di.model_module,
                     _view_module: Di.view_module,
                     _model_module_version: Di.model_module_version,
                     _view_module_version: Di.view_module_version,
-                    data: [],
+                    dataRecords: [],
                     x: String,
                     start: Number,
                     end: Number,
                     elementId: String
                 }
             }
             static model_name = "HistogramplotModel";
@@ -3886,18 +3885,18 @@
             static view_name = "HistogramplotView";
             static view_module = Ni.name;
             static view_module_version = Ni.version
         }
         class Ii extends t.DOMWidgetView {
             timeout;
             render() {
-                Ci(this), this.model.on("change:data", (() => Ci(this)), this), this.model.on("change:x", (() => Ci(this)), this), this.model.on("change:start", (() => Ci(this)), this), this.model.on("change:end", (() => Ci(this)), this), window.addEventListener("resize", (() => Ci(this)))
+                Ci(this), this.model.on("change:dataRecords", (() => Ci(this)), this), this.model.on("change:x", (() => Ci(this)), this), this.model.on("change:start", (() => Ci(this)), this), this.model.on("change:end", (() => Ci(this)), this), window.addEventListener("resize", (() => Ci(this)))
             }
             plot() {
-                const t = this.model.get("data"),
+                const t = this.model.get("dataRecords"),
                     e = this.model.get("x"),
                     n = this.model.get("start"),
                     r = this.model.get("end"),
                     i = this.model.get("elementId");
                 let o = Si,
                     a = this.el;
                 i && (a = document.getElementById(i), o = a.clientHeight),
@@ -3915,65 +3914,65 @@
                             m = K(d),
                             _ = L().thresholds(40).value((t => Math.round(10 * t[e]) / 10))(t),
                             g = mr(i).append("svg").attr("width", o).attr("height", a).append("g").attr("transform", "translate(" + s.left + "," + s.top + ")");
                         f.domain([c, h]), d.domain([0, D(_, (t => t.length))]), g.append("g").attr("transform", "translate(0," + u + ")").call(p).append("text").attr("x", l).attr("y", -6).style("text-anchor", "end"), g.append("g").call(m).append("text").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end"), g.append("g").attr("fill", "steelblue").selectAll().data(_).join("rect").attr("x", (t => f(t.x0) + 1)).attr("width", (t => f(t.x1) - f(t.x0) - 1)).attr("y", (t => d(t.length))).attr("height", (t => d(0) - d(t.length)))
                     }(t, e, n, r, a, a.clientWidth, o, $i)
             }
         }
-        class qi extends t.DOMWidgetModel {
+        class Ri extends t.DOMWidgetModel {
             defaults() {
                 return {
                     ...super.defaults(),
-                    _model_name: qi.model_name,
-                    _view_name: qi.view_name,
-                    _model_module: qi.model_module,
-                    _view_module: qi.view_module,
-                    _model_module_version: qi.model_module_version,
-                    _view_module_version: qi.view_module_version,
+                    _model_name: Ri.model_name,
+                    _view_name: Ri.view_name,
+                    _model_module: Ri.model_module,
+                    _view_module: Ri.view_module,
+                    _model_module_version: Ri.model_module_version,
+                    _view_module_version: Ri.view_module_version,
                     matrix: [],
                     grid_areas: [],
                     grid_template_areas: String,
                     style: String
                 }
             }
             static model_name = "EmbeddingModel";
             static model_module = Ni.name;
             static model_module_version = Ni.version;
             static view_name = "EmbeddingView";
             static view_module = Ni.name;
             static view_module_version = Ni.version
         }
-        class Hi extends t.DOMWidgetView {
+        class qi extends t.DOMWidgetView {
             render() {
                 this.value_changed()
             }
             value_changed() {
                 const t = this.model.get("matrix"),
                     e = this.model.get("grid_areas"),
                     n = this.model.get("grid_template_areas");
                 let r = this.model.get("style");
                 r || (r = "basic");
                 const i = document.createElement("div");
                 i.classList.add(r), i.style.display = "grid", i.style.gridTemplateAreas = n, i.style.gridTemplateRows = "repeat(" + t.length + ", 180px)", i.style.gridTemplateColumns = "repeat(" + t[0].length + ", 1fr)", i.style.width = "100%", e.forEach((t => {
                     const e = document.createElement("div");
                     e.setAttribute("id", t), e.style.gridArea = t, e.classList.add("dashboard-div"), i.appendChild(e)
-                })), this.el.appendChild(i), console.log("Embedding:"), console.log(i)
+                })), this.el.appendChild(i)
             }
         }
-        class zi extends t.DOMWidgetModel {
+        class Hi extends t.DOMWidgetModel {
             defaults() {
                 return {
                     ...super.defaults(),
-                    _model_name: zi.model_name,
-                    _view_name: zi.view_name,
-                    _model_module: zi.model_module,
-                    _view_module: zi.view_module,
-                    _model_module_version: zi.model_module_version,
-                    _view_module_version: zi.view_module_version,
-                    data: [],
+                    _model_name: Hi.model_name,
+                    _view_name: Hi.view_name,
+                    _model_module: Hi.model_module,
+                    _view_module: Hi.view_module,
+                    _model_module_version: Hi.model_module_version,
+                    _view_module_version: Hi.view_module_version,
+                    dataRecords: [],
                     variable: String,
                     step: Number,
                     description: String,
                     minValue: Number,
                     maxValue: Number,
                     elementId: String
                 }
@@ -3981,20 +3980,20 @@
             static model_name = "RangeSliderModel";
             static model_module = Ni.name;
             static model_module_version = Ni.version;
             static view_name = "RangeSliderView";
             static view_module = Ni.name;
             static view_module_version = Ni.version
         }
-        class Xi extends t.DOMWidgetView {
+        class zi extends t.DOMWidgetView {
             render() {
-                Ci(this), this.model.on("change:data", (() => Ci(this)), this), this.model.on("change:variable", (() => Ci(this)), this), this.model.on("change:step", (() => Ci(this)), this), this.model.on("change:description", (() => Ci(this)), this), window.addEventListener("resize", (() => Ci(this)))
+                Ci(this), this.model.on("change:dataRecords", (() => Ci(this)), this), this.model.on("change:variable", (() => Ci(this)), this), this.model.on("change:step", (() => Ci(this)), this), this.model.on("change:description", (() => Ci(this)), this), window.addEventListener("resize", (() => Ci(this)))
             }
             plot() {
-                const t = this.model.get("data"),
+                const t = this.model.get("dataRecords"),
                     e = this.model.get("variable"),
                     n = this.model.get("step"),
                     r = this.model.get("description"),
                     i = this.model.get("elementId"),
                     o = this.model.get("minValue"),
                     a = this.model.get("maxValue");
                 let s = this.el;
@@ -4040,10 +4039,10 @@
                 this.model.set({
                     minValue: t
                 }), this.model.set({
                     maxValue: e
                 }), this.model.save_changes()
             }
         }
-        var Ri = i(330)
+        var Xi = i(330)
     })(), o
 })()));
```

### Comparing `d3vis_ipynb-0.1.5/js/amd-public-path.js` & `d3vis_ipynb-0.2.0/js/amd-public-path.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.5/js/package.json` & `d3vis_ipynb-0.2.0/js/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.2.0'"}*

```diff
@@ -50,9 +50,9 @@
         "export": "webpack --env export --config webpack.exports.config.js",
         "prepublish": "yarn run clean && yarn run build:prod",
         "start": "webpack serve --open --config webpack.exports.config.js",
         "start:export": "webpack serve --open --config webpack.exports.config.js --env export",
         "test": "echo \"Error: no test specified\" && exit 1",
         "watch": "webpack --watch --mode=development"
     },
-    "version": "0.1.5"
+    "version": "0.2.0"
 }
```

### Comparing `d3vis_ipynb-0.1.5/js/webpack.config.js` & `d3vis_ipynb-0.2.0/js/webpack.config.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.5/js/webpack.exports.config.js` & `d3vis_ipynb-0.2.0/js/webpack.exports.config.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.5/js/css/widget.css` & `d3vis_ipynb-0.2.0/js/css/widget.css`

 * *Files 14% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 
 input[type="range"]::-webkit-slider-thumb {
   -webkit-appearance: none;
   pointer-events: all;
   width: 24px;
   height: 24px;
   background-color: #fff;
+  border: none !important;
   border-radius: 50%;
   box-shadow: 0 0 0 1px #c6c6c6;
   cursor: pointer;
 }
 
 input[type="range"]::-moz-range-thumb {
   -webkit-appearance: none;
```

### Comparing `d3vis_ipynb-0.1.5/js/lib/labplugin.js` & `d3vis_ipynb-0.2.0/js/lib/labplugin.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.5/js/lib/web-dev.js` & `d3vis_ipynb-0.2.0/js/lib/web-dev.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.5/js/lib/widgets.js` & `d3vis_ipynb-0.2.0/js/lib/widgets.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -14,15 +14,15 @@
 } from "./graphs/linearhistplot";
 import {
     rangeslider
 } from "./graphs/rangeslider";
 import {
     scatterplot
 } from "./graphs/scatterplot";
-const data = require("../package.json");
+const packageData = require("../package.json");
 
 const WIDGET_HEIGHT = 400;
 const WIDGET_MARGIN = {
     top: 20,
     right: 20,
     bottom: 30,
     left: 40
@@ -54,19 +54,19 @@
             histogramData: [],
             elementId: String,
             clickedValue: String,
         };
     }
 
     static model_name = "LinearHistPlotModel";
-    static model_module = data.name;
-    static model_module_version = data.version;
+    static model_module = packageData.name;
+    static model_module_version = packageData.version;
     static view_name = "LinearHistPlotView"; // Set to null if no view
-    static view_module = data.name; // Set to null if no view
-    static view_module_version = data.version;
+    static view_module = packageData.name; // Set to null if no view
+    static view_module_version = packageData.version;
 }
 
 export class LinearHistPlotView extends DOMWidgetView {
     timeout;
 
     render() {
         plotAfterInterval(this);
@@ -119,47 +119,47 @@
             _model_name: ScatterPlotModel.model_name,
             _view_name: ScatterPlotModel.view_name,
             _model_module: ScatterPlotModel.model_module,
             _view_module: ScatterPlotModel.view_module,
             _model_module_version: ScatterPlotModel.model_module_version,
             _view_module_version: ScatterPlotModel.view_module_version,
 
-            data: [],
+            dataRecords: [],
             x: String,
             y: String,
             hue: String,
             elementId: String,
             clickedValue: String,
-            selectedValues: [],
+            selectedValuesRecords: [],
         };
     }
 
     static model_name = "ScatterplotModel";
-    static model_module = data.name;
-    static model_module_version = data.version;
+    static model_module = packageData.name;
+    static model_module_version = packageData.version;
     static view_name = "ScatterplotView"; // Set to null if no view
-    static view_module = data.name; // Set to null if no view
-    static view_module_version = data.version;
+    static view_module = packageData.name; // Set to null if no view
+    static view_module_version = packageData.version;
 }
 
 export class ScatterPlotView extends DOMWidgetView {
     timeout;
 
     render() {
         plotAfterInterval(this);
 
-        this.model.on("change:data", () => plotAfterInterval(this), this);
+        this.model.on("change:dataRecords", () => plotAfterInterval(this), this);
         this.model.on("change:x", () => plotAfterInterval(this), this);
         this.model.on("change:y", () => plotAfterInterval(this), this);
         this.model.on("change:hue", () => plotAfterInterval(this), this);
         window.addEventListener("resize", () => plotAfterInterval(this));
     }
 
     plot() {
-        const data = this.model.get("data");
+        const data = this.model.get("dataRecords");
         const x = this.model.get("x");
         const y = this.model.get("y");
         const hue = this.model.get("hue");
         const elementId = this.model.get("elementId");
 
         let height = WIDGET_HEIGHT;
         let element = this.el;
@@ -189,15 +189,15 @@
             clickedValue: text
         });
         this.model.save_changes();
     }
 
     setSelectedValues(values) {
         this.model.set({
-            selectedValues: values
+            selectedValuesRecords: values
         });
         this.model.save_changes();
     }
 }
 
 export class BarPlotModel extends DOMWidgetModel {
     defaults() {
@@ -206,54 +206,50 @@
             _model_name: BarPlotModel.model_name,
             _view_name: BarPlotModel.view_name,
             _model_module: BarPlotModel.model_module,
             _view_module: BarPlotModel.view_module,
             _model_module_version: BarPlotModel.model_module_version,
             _view_module_version: BarPlotModel.view_module_version,
 
-            data: [],
+            dataRecords: [],
             x: String,
             y: String,
             hue: String,
             elementId: String,
         };
     }
 
     static model_name = "BarplotModel";
-    static model_module = data.name;
-    static model_module_version = data.version;
+    static model_module = packageData.name;
+    static model_module_version = packageData.version;
     static view_name = "BarplotView"; // Set to null if no view
-    static view_module = data.name; // Set to null if no view
-    static view_module_version = data.version;
+    static view_module = packageData.name; // Set to null if no view
+    static view_module_version = packageData.version;
 }
 
 export class BarPlotView extends DOMWidgetView {
     timeout;
 
     render() {
         plotAfterInterval(this);
 
-        this.model.on("change:data", () => plotAfterInterval(this), this);
+        this.model.on("change:dataRecords", () => plotAfterInterval(this), this);
         this.model.on("change:x", () => plotAfterInterval(this), this);
         this.model.on("change:y", () => plotAfterInterval(this), this);
         this.model.on("change:hue", () => plotAfterInterval(this), this);
         window.addEventListener("resize", () => plotAfterInterval(this));
     }
 
     plot() {
-        const data = this.model.get("data");
+        const data = this.model.get("dataRecords");
         const x = this.model.get("x");
         const y = this.model.get("y");
         const hue = this.model.get("hue");
         const elementId = this.model.get("elementId");
 
-        console.log("barplot");
-        console.log("elementId:");
-        console.log(elementId);
-
         let height = WIDGET_HEIGHT;
         let element = this.el;
         if (elementId) {
             element = document.getElementById(elementId);
             height = element.clientHeight;
         }
         let width = element.clientWidth;
@@ -270,45 +266,45 @@
             _model_name: HistogramPlotModel.model_name,
             _view_name: HistogramPlotModel.view_name,
             _model_module: HistogramPlotModel.model_module,
             _view_module: HistogramPlotModel.view_module,
             _model_module_version: HistogramPlotModel.model_module_version,
             _view_module_version: HistogramPlotModel.view_module_version,
 
-            data: [],
+            dataRecords: [],
             x: String,
             start: Number,
             end: Number,
             elementId: String,
         };
     }
 
     static model_name = "HistogramplotModel";
-    static model_module = data.name;
-    static model_module_version = data.version;
+    static model_module = packageData.name;
+    static model_module_version = packageData.version;
     static view_name = "HistogramplotView"; // Set to null if no view
-    static view_module = data.name; // Set to null if no view
-    static view_module_version = data.version;
+    static view_module = packageData.name; // Set to null if no view
+    static view_module_version = packageData.version;
 }
 
 export class HistogramPlotView extends DOMWidgetView {
     timeout;
 
     render() {
         plotAfterInterval(this);
 
-        this.model.on("change:data", () => plotAfterInterval(this), this);
+        this.model.on("change:dataRecords", () => plotAfterInterval(this), this);
         this.model.on("change:x", () => plotAfterInterval(this), this);
         this.model.on("change:start", () => plotAfterInterval(this), this);
         this.model.on("change:end", () => plotAfterInterval(this), this);
         window.addEventListener("resize", () => plotAfterInterval(this));
     }
 
     plot() {
-        const data = this.model.get("data");
+        const data = this.model.get("dataRecords");
         const x = this.model.get("x");
         const start = this.model.get("start");
         const end = this.model.get("end");
         const elementId = this.model.get("elementId");
 
         let height = WIDGET_HEIGHT;
         let element = this.el;
@@ -338,19 +334,19 @@
             grid_areas: [],
             grid_template_areas: String,
             style: String,
         };
     }
 
     static model_name = "EmbeddingModel";
-    static model_module = data.name;
-    static model_module_version = data.version;
+    static model_module = packageData.name;
+    static model_module_version = packageData.version;
     static view_name = "EmbeddingView"; // Set to null if no view
-    static view_module = data.name; // Set to null if no view
-    static view_module_version = data.version;
+    static view_module = packageData.name; // Set to null if no view
+    static view_module_version = packageData.version;
 }
 
 export class EmbeddingView extends DOMWidgetView {
     render() {
         this.value_changed();
     }
 
@@ -378,61 +374,59 @@
             grid_area.setAttribute("id", area);
             grid_area.style.gridArea = area;
             grid_area.classList.add("dashboard-div");
             node.appendChild(grid_area);
         });
 
         this.el.appendChild(node);
-        console.log("Embedding:")
-        console.log(node)
     }
 }
 
 export class RangeSliderModel extends DOMWidgetModel {
     defaults() {
         return {
             ...super.defaults(),
             _model_name: RangeSliderModel.model_name,
             _view_name: RangeSliderModel.view_name,
             _model_module: RangeSliderModel.model_module,
             _view_module: RangeSliderModel.view_module,
             _model_module_version: RangeSliderModel.model_module_version,
             _view_module_version: RangeSliderModel.view_module_version,
 
-            data: [],
+            dataRecords: [],
             variable: String,
             step: Number,
             description: String,
             minValue: Number,
             maxValue: Number,
             elementId: String,
         };
     }
 
     static model_name = "RangeSliderModel";
-    static model_module = data.name;
-    static model_module_version = data.version;
+    static model_module = packageData.name;
+    static model_module_version = packageData.version;
     static view_name = "RangeSliderView"; // Set to null if no view
-    static view_module = data.name; // Set to null if no view
-    static view_module_version = data.version;
+    static view_module = packageData.name; // Set to null if no view
+    static view_module_version = packageData.version;
 }
 
 export class RangeSliderView extends DOMWidgetView {
     render() {
         plotAfterInterval(this);
 
-        this.model.on("change:data", () => plotAfterInterval(this), this);
+        this.model.on("change:dataRecords", () => plotAfterInterval(this), this);
         this.model.on("change:variable", () => plotAfterInterval(this), this);
         this.model.on("change:step", () => plotAfterInterval(this), this);
         this.model.on("change:description", () => plotAfterInterval(this), this);
         window.addEventListener("resize", () => plotAfterInterval(this));
     }
 
     plot() {
-        const data = this.model.get("data");
+        const data = this.model.get("dataRecords");
         const variable = this.model.get("variable");
         const step = this.model.get("step");
         const description = this.model.get("description");
         const elementId = this.model.get("elementId");
         const minValue = this.model.get("minValue");
         const maxValue = this.model.get("maxValue");
```

### Comparing `d3vis_ipynb-0.1.5/js/lib/graphs/barplot.js` & `d3vis_ipynb-0.2.0/js/lib/graphs/barplot.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -9,21 +9,14 @@
     width,
     height,
     margin
 ) {
     const innerWidth = width - margin.left - margin.right;
     const innerHeight = height - margin.top - margin.bottom;
 
-    console.log("element:");
-    console.log(element);
-    console.log("width:");
-    console.log(width);
-    console.log("height:");
-    console.log(height);
-
     d3.select(element).selectAll("*").remove();
 
     const svg = d3
         .select(element)
         .append("svg")
         .attr("width", width)
         .attr("height", height)
```

### Comparing `d3vis_ipynb-0.1.5/js/lib/graphs/histogramplot.js` & `d3vis_ipynb-0.2.0/js/lib/graphs/histogramplot.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.5/js/lib/graphs/linearhistplot.js` & `d3vis_ipynb-0.2.0/js/lib/graphs/linearhistplot.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.5/js/lib/graphs/rangeslider.js` & `d3vis_ipynb-0.2.0/js/lib/graphs/rangeslider.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.5/js/lib/graphs/scatterplot.js` & `d3vis_ipynb-0.2.0/js/lib/graphs/scatterplot.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.5/js/lib/tools/lasso.js` & `d3vis_ipynb-0.2.0/js/lib/tools/lasso.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.5/js/lib/wrappers/embedding.wrapper.js` & `d3vis_ipynb-0.2.0/js/lib/wrappers/embedding.wrapper.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.5/LICENSE.txt` & `d3vis_ipynb-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.5/README.md` & `d3vis_ipynb-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.5/pyproject.toml` & `d3vis_ipynb-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "ipywidgets==7.7.1",
     "simplejson >=3.19.0",
     "anywidget >= 0.9.6"
 ]
-version = "0.1.5"
+version = "0.2.0"
 
 [project.optional-dependencies]
 docs = [
     "jupyter_sphinx",
     "nbsphinx",
     "nbsphinx-link",
     "pypandoc",
```

### Comparing `d3vis_ipynb-0.1.5/PKG-INFO` & `d3vis_ipynb-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: d3vis_ipynb
-Version: 0.1.5
+Version: 0.2.0
 Summary: A Custom Jupyter Widget Library with visualizations created with D3.js.
 Project-URL: Homepage, https://github.com/H-IAAC/d3vis_ipynb
 Author-email: Daniel Adam Miranda <daniel.miranda@eldorado.org.br>
 License: Copyright (c) 2024 Daniel Adam Miranda
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```


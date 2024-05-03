# Comparing `tmp/comfy_script-0.5.0a2.tar.gz` & `tmp/comfy_script-0.5.0a3.tar.gz`

## Comparing `comfy_script-0.5.0a2.tar` & `comfy_script-0.5.0a3.tar`

### file list

```diff
@@ -1,48 +1,50 @@
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/__init__.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/requirements.txt
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/.vscode/launch.json
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/docs/README.md
--rw-r--r--   0        0        0    18293 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/docs/Runtime.md
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/docs/Transpiler.md
--rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/docs/Image/README.md
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/docs/Latent/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/docs/Models/README.md
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/docs/Nodes/README.md
--rw-r--r--   0        0        0   839054 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/docs/images/README/auto-queue.png
--rw-r--r--   0        0        0    41490 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/docs/images/README/diff.png
--rw-r--r--   0        0        0   908632 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/docs/images/README/plot.png
--rw-r--r--   0        0        0  2677075 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/docs/images/README/select.png
--rw-r--r--   0        0        0    74672 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/docs/images/README/type-stubs.png
--rw-r--r--   0        0        0    51995 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/docs/images/README/type-stubs2.png
--rw-r--r--   0        0        0    89265 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/docs/images/README/workflow.png
--rw-r--r--   0        0        0   170300 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/docs/images/README/workflow2.png
--rw-r--r--   0        0        0   199246 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/docs/images/Runtime/load-api-format.png
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/src/comfy_script/__init__.py
--rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/src/comfy_script/astutil.py
--rw-r--r--   0        0        0     7619 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/src/comfy_script/client/__init__.py
--rw-r--r--   0        0        0     8029 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/src/comfy_script/nodes/__init__.py
--rw-r--r--   0        0        0    45421 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/src/comfy_script/runtime/__init__.py
--rw-r--r--   0        0        0    20573 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/src/comfy_script/runtime/factory.py
--rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/src/comfy_script/runtime/nodes.py
--rw-r--r--   0        0        0     4442 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/src/comfy_script/runtime/data/Images.py
--rw-r--r--   0        0        0     4973 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/src/comfy_script/runtime/data/__init__.py
--rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/src/comfy_script/runtime/real/__init__.py
--rw-r--r--   0        0        0     7291 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/src/comfy_script/runtime/real/nodes.py
--rw-r--r--   0        0        0    14763 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/src/comfy_script/transpile/__init__.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/src/comfy_script/transpile/__main__.py
--rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/src/comfy_script/transpile/prompt.py
--rw-r--r--   0        0        0     5299 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/src/comfy_script/transpile/passes/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/src/comfy_script/ui/__init__.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/src/comfy_script/ui/solara/__init__.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/src/comfy_script/ui/solara/metadata.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/tests/__init__.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/tests/test_astutil.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/tests/transpile/__init__.py
--rw-r--r--   0        0        0    23060 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/tests/transpile/bypass.json
--rw-r--r--   0        0        0     5819 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/tests/transpile/default.json
--rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/tests/transpile/test_transpiler.py
--rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/LICENSE.txt
--rw-r--r--   0        0        0    14501 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/README.md
--rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/pyproject.toml
--rw-r--r--   0        0        0    16183 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/__init__.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/requirements.txt
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/settings.example.toml
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/.vscode/launch.json
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/docs/README.md
+-rw-r--r--   0        0        0    18293 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/docs/Runtime.md
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/docs/Transpiler.md
+-rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/docs/Image/README.md
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/docs/Latent/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/docs/Models/README.md
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/docs/Nodes/README.md
+-rw-r--r--   0        0        0   839054 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/docs/images/README/auto-queue.png
+-rw-r--r--   0        0        0    41490 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/docs/images/README/diff.png
+-rw-r--r--   0        0        0   908632 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/docs/images/README/plot.png
+-rw-r--r--   0        0        0  2677075 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/docs/images/README/select.png
+-rw-r--r--   0        0        0    74672 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/docs/images/README/type-stubs.png
+-rw-r--r--   0        0        0    51995 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/docs/images/README/type-stubs2.png
+-rw-r--r--   0        0        0    89265 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/docs/images/README/workflow.png
+-rw-r--r--   0        0        0   170300 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/docs/images/README/workflow2.png
+-rw-r--r--   0        0        0   199246 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/docs/images/Runtime/load-api-format.png
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/src/comfy_script/__init__.py
+-rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/src/comfy_script/astutil.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/src/comfy_script/config.py
+-rw-r--r--   0        0        0     7619 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/src/comfy_script/client/__init__.py
+-rw-r--r--   0        0        0     8525 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/src/comfy_script/nodes/__init__.py
+-rw-r--r--   0        0        0    45421 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/src/comfy_script/runtime/__init__.py
+-rw-r--r--   0        0        0    20573 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/src/comfy_script/runtime/factory.py
+-rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/src/comfy_script/runtime/nodes.py
+-rw-r--r--   0        0        0     4442 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/src/comfy_script/runtime/data/Images.py
+-rw-r--r--   0        0        0     4973 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/src/comfy_script/runtime/data/__init__.py
+-rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/src/comfy_script/runtime/real/__init__.py
+-rw-r--r--   0        0        0     7291 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/src/comfy_script/runtime/real/nodes.py
+-rw-r--r--   0        0        0    14763 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/src/comfy_script/transpile/__init__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/src/comfy_script/transpile/__main__.py
+-rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/src/comfy_script/transpile/prompt.py
+-rw-r--r--   0        0        0     5299 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/src/comfy_script/transpile/passes/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/src/comfy_script/ui/__init__.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/src/comfy_script/ui/solara/__init__.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/src/comfy_script/ui/solara/metadata.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/tests/__init__.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/tests/test_astutil.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/tests/transpile/__init__.py
+-rw-r--r--   0        0        0    23060 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/tests/transpile/bypass.json
+-rw-r--r--   0        0        0     5819 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/tests/transpile/default.json
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/tests/transpile/test_transpiler.py
+-rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/LICENSE.txt
+-rw-r--r--   0        0        0    14584 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/README.md
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/pyproject.toml
+-rw-r--r--   0        0        0    16315 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/PKG-INFO
```

### Comparing `comfy_script-0.5.0a2/__init__.py` & `comfy_script-0.5.0a3/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a2/docs/README.md` & `comfy_script-0.5.0a3/docs/README.md`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a2/docs/Runtime.md` & `comfy_script-0.5.0a3/docs/Runtime.md`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a2/docs/Image/README.md` & `comfy_script-0.5.0a3/docs/Image/README.md`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a2/docs/Latent/README.md` & `comfy_script-0.5.0a3/docs/Latent/README.md`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a2/docs/Nodes/README.md` & `comfy_script-0.5.0a3/docs/Nodes/README.md`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a2/docs/images/README/auto-queue.png` & `comfy_script-0.5.0a3/docs/images/README/auto-queue.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a2/docs/images/README/diff.png` & `comfy_script-0.5.0a3/docs/images/README/diff.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a2/docs/images/README/plot.png` & `comfy_script-0.5.0a3/docs/images/README/plot.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a2/docs/images/README/select.png` & `comfy_script-0.5.0a3/docs/images/README/select.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a2/docs/images/README/type-stubs.png` & `comfy_script-0.5.0a3/docs/images/README/type-stubs.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a2/docs/images/README/type-stubs2.png` & `comfy_script-0.5.0a3/docs/images/README/type-stubs2.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a2/docs/images/README/workflow.png` & `comfy_script-0.5.0a3/docs/images/README/workflow.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a2/docs/images/README/workflow2.png` & `comfy_script-0.5.0a3/docs/images/README/workflow2.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a2/docs/images/Runtime/load-api-format.png` & `comfy_script-0.5.0a3/docs/images/Runtime/load-api-format.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a2/src/comfy_script/astutil.py` & `comfy_script-0.5.0a3/src/comfy_script/astutil.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a2/src/comfy_script/client/__init__.py` & `comfy_script-0.5.0a3/src/comfy_script/client/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a2/src/comfy_script/nodes/__init__.py` & `comfy_script-0.5.0a3/src/comfy_script/nodes/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -73,38 +73,43 @@
         
         @property
         def chunks(self):
             if self._texts:
                 chunks = self._chunks
                 self._chunks = []
 
-                if 'workflow' in self._texts or 'prompt' in self._texts:
-                    try:
-                        workflow, zip = self._texts['workflow' if 'workflow' in self._texts else 'prompt']
-                        
-                        end_nodes = None
-                        # TODO: UNIQUE_ID
-                        frame = inspect.currentframe()
-                        while frame := frame.f_back:
-                            if 'unique_id' in frame.f_locals:
-                                end_nodes = [frame.f_locals['unique_id']]
-                                break
-                        else:
-                            print('ComfyScript: Failed to resolve the id of current node.')
-
-                        comfy_script = transpile.WorkflowToScriptTranspiler(workflow).to_script(end_nodes)
-                        # TODO: Syntax highlight?
-                        print('ComfyScript:', comfy_script, sep='\n')
-
-                        super().add_text('ComfyScript', comfy_script, zip)
-                    except Exception:
-                        # Print stack trace, but do not block the original saving
-                        traceback.print_exc()
-                else:
-                    print("ComfyScript: Failed to save ComfyScript because neither of workflow and prompt is in extra_pnginfo")
+                print_script = settings.transpile.hook.print_script
+                save_script = settings.transpile.hook.save_script
+                if print_script is True or save_script is True:
+                    if 'workflow' in self._texts or 'prompt' in self._texts:
+                        try:
+                            workflow, zip = self._texts['workflow' if 'workflow' in self._texts else 'prompt']
+                            
+                            end_nodes = None
+                            # TODO: UNIQUE_ID
+                            frame = inspect.currentframe()
+                            while frame := frame.f_back:
+                                if 'unique_id' in frame.f_locals:
+                                    end_nodes = [frame.f_locals['unique_id']]
+                                    break
+                            else:
+                                print('ComfyScript: Failed to resolve the id of current node.')
+
+                            comfy_script = transpile.WorkflowToScriptTranspiler(workflow).to_script(end_nodes)
+                            if print_script is True:
+                                # TODO: Syntax highlight?
+                                print('ComfyScript:', comfy_script, sep='\n')
+
+                            if save_script is True:
+                                super().add_text('ComfyScript', comfy_script, zip)
+                        except Exception:
+                            # Print stack trace, but do not block the original saving
+                            traceback.print_exc()
+                    else:
+                        print("ComfyScript: Failed to save ComfyScript because neither of workflow and prompt is in extra_pnginfo")
                 
                 if 'ComfyScriptSource' in self._texts:
                     try:
                         source, zip = self._texts['ComfyScriptSource']
                         source = json.loads(source)
                         # print(source)
                         super().add_text('ComfyScriptSource', source, zip)
@@ -161,15 +166,17 @@
     #     #     except Exception:
     #     #         # Print stack trace, but do not block the original saving
     #     #         traceback.print_exc()
     #     return save_images_orginal(self, images, filename_prefix, prompt, extra_pnginfo)
     # setattr(SaveImage, SaveImage.FUNCTION, save_images_hook)
 
 try:
-    setup()
+    from ..config import settings
+    if settings.transpile.hook.enabled is True:
+        setup()
 except ImportError as e:
     success = False
     print(
 f'''\033[34mComfyScript: \033[91mFailed to setup script translation due to missing dependencies: {e}.
 If you need this feature, try to run:
 python -m pip install -r "{Path(__file__).resolve().parents[3] / 'requirements.txt'}"
 \033[0m''')
```

### Comparing `comfy_script-0.5.0a2/src/comfy_script/runtime/__init__.py` & `comfy_script-0.5.0a3/src/comfy_script/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a2/src/comfy_script/runtime/factory.py` & `comfy_script-0.5.0a3/src/comfy_script/runtime/factory.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a2/src/comfy_script/runtime/nodes.py` & `comfy_script-0.5.0a3/src/comfy_script/runtime/nodes.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a2/src/comfy_script/runtime/data/Images.py` & `comfy_script-0.5.0a3/src/comfy_script/runtime/data/Images.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a2/src/comfy_script/runtime/data/__init__.py` & `comfy_script-0.5.0a3/src/comfy_script/runtime/data/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a2/src/comfy_script/runtime/real/__init__.py` & `comfy_script-0.5.0a3/src/comfy_script/runtime/real/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a2/src/comfy_script/runtime/real/nodes.py` & `comfy_script-0.5.0a3/src/comfy_script/runtime/real/nodes.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a2/src/comfy_script/transpile/__init__.py` & `comfy_script-0.5.0a3/src/comfy_script/transpile/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a2/src/comfy_script/transpile/prompt.py` & `comfy_script-0.5.0a3/src/comfy_script/transpile/prompt.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a2/src/comfy_script/transpile/passes/__init__.py` & `comfy_script-0.5.0a3/src/comfy_script/transpile/passes/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a2/src/comfy_script/ui/solara/metadata.py` & `comfy_script-0.5.0a3/src/comfy_script/ui/solara/metadata.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a2/tests/test_astutil.py` & `comfy_script-0.5.0a3/tests/test_astutil.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a2/tests/transpile/bypass.json` & `comfy_script-0.5.0a3/tests/transpile/bypass.json`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a2/tests/transpile/default.json` & `comfy_script-0.5.0a3/tests/transpile/default.json`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a2/tests/transpile/test_transpiler.py` & `comfy_script-0.5.0a3/tests/transpile/test_transpiler.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a2/.gitignore` & `comfy_script-0.5.0a3/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 private/
 *.private
 *.private.*
 
 /examples
 
+# Ignore dynaconf files
+.secrets.*
+*.local.*
+
 # Hatch will only respect the first .gitignore file
 /src/comfy_script/runtime/**/*.pyi
 
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
```

### Comparing `comfy_script-0.5.0a2/LICENSE.txt` & `comfy_script-0.5.0a3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a2/README.md` & `comfy_script-0.5.0a3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
 ### Other ways
 ComfyScript can also be used without installed ComfyUI. See [only ComfyScript package](docs/README.md#only-comfyscript-package) for details. And see [uninstallation](docs/README.md#uninstallation) for how to uninstall.
 
 ## Transpiler
 The transpiler can translate ComfyUI's workflows to ComfyScript.
 
-When ComfyScript is installed as custom nodes, `SaveImage` and similar nodes will be hooked to automatically save the script as images' metadata. And the script will also be output to the terminal.
+When ComfyScript is installed as custom nodes, `SaveImage` and similar nodes will be hooked to automatically save the script as the image's metadata. The script will also be printed to the terminal.
 
 For example, here is a workflow in ComfyUI:
 
 ![](docs/images/README/workflow.png)
 
 ComfyScript translated from it:
 ```python
@@ -129,14 +129,16 @@
    SaveImage(image, 'ComfyUI')
    ```
 
 Comparing scripts:
 
 ![](docs/images/README/diff.png)
 
+To control these features, see [settings.example.toml](settings.example.toml).
+
 You can also use the transpiler via the [CLI](docs/Transpiler.md#cli).
 
 ## Runtime
 With the runtime, one can run ComfyScript like this:
 ```python
 from comfy_script.runtime import *
 load()
```

### Comparing `comfy_script-0.5.0a2/pyproject.toml` & `comfy_script-0.5.0a3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "comfy-script"
-version = "0.5.0a2"
+version = "0.5.0a3"
 description = "A Python front end and library for ComfyUI"
 readme = "README.md"
 # ComfyUI: >=3.8
 # comfyui: >=3.9
 # >=3.6 is required to preserve insertion order of input types
 requires-python = ">=3.9"
 authors = [
@@ -33,18 +33,21 @@
   "Pillow",
 
   "aenum ~= 3.1"
 ]
 
 # Transpiler
 transpile = [
+  # Already required by ComfyUI (torch)
   "networkx[default] ~= 3.0",
 
   # Used to get nodes info
   "comfy-script[client]",
+
+  "dynaconf ~= 3.0",
 ]
 
 # Runtime
 runtime = [
   # Already required by ComfyUI
   "Pillow",
```

### Comparing `comfy_script-0.5.0a2/PKG-INFO` & `comfy_script-0.5.0a3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comfy-script
-Version: 0.5.0a2
+Version: 0.5.0a3
 Summary: A Python front end and library for ComfyUI
 Project-URL: Homepage, https://github.com/Chaoses-Ib/ComfyScript
 Project-URL: Issues, https://github.com/Chaoses-Ib/ComfyScript/issues
 Author-email: Chaoses-Ib <Chaos-es@outlook.com>
 License-File: LICENSE.txt
 Keywords: comfyui
 Classifier: License :: OSI Approved :: MIT License
@@ -39,14 +39,15 @@
 Provides-Extra: runtime
 Requires-Dist: comfy-script[client]; extra == 'runtime'
 Requires-Dist: comfy-script[transpile]; extra == 'runtime'
 Requires-Dist: pillow; extra == 'runtime'
 Requires-Dist: wrapt~=1.0; extra == 'runtime'
 Provides-Extra: transpile
 Requires-Dist: comfy-script[client]; extra == 'transpile'
+Requires-Dist: dynaconf~=3.0; extra == 'transpile'
 Requires-Dist: networkx[default]~=3.0; extra == 'transpile'
 Description-Content-Type: text/markdown
 
 # ComfyScript
 [![PyPI - Version](https://img.shields.io/pypi/v/comfy-script)](https://pypi.org/project/comfy-script) ![Python Version from PEP 621 TOML](https://img.shields.io/python/required-version-toml?tomlFilePath=https%3A%2F%2Fraw.githubusercontent.com%2FChaoses-Ib%2FComfyScript%2Fmain%2Fpyproject.toml) [![License](https://img.shields.io/pypi/l/comfy-script)](LICENSE.txt)
 
 A Python front end and library for [ComfyUI](https://github.com/comfyanonymous/ComfyUI).
@@ -130,15 +131,15 @@
 
 ### Other ways
 ComfyScript can also be used without installed ComfyUI. See [only ComfyScript package](docs/README.md#only-comfyscript-package) for details. And see [uninstallation](docs/README.md#uninstallation) for how to uninstall.
 
 ## Transpiler
 The transpiler can translate ComfyUI's workflows to ComfyScript.
 
-When ComfyScript is installed as custom nodes, `SaveImage` and similar nodes will be hooked to automatically save the script as images' metadata. And the script will also be output to the terminal.
+When ComfyScript is installed as custom nodes, `SaveImage` and similar nodes will be hooked to automatically save the script as the image's metadata. The script will also be printed to the terminal.
 
 For example, here is a workflow in ComfyUI:
 
 ![](docs/images/README/workflow.png)
 
 ComfyScript translated from it:
 ```python
@@ -177,14 +178,16 @@
    SaveImage(image, 'ComfyUI')
    ```
 
 Comparing scripts:
 
 ![](docs/images/README/diff.png)
 
+To control these features, see [settings.example.toml](settings.example.toml).
+
 You can also use the transpiler via the [CLI](docs/Transpiler.md#cli).
 
 ## Runtime
 With the runtime, one can run ComfyScript like this:
 ```python
 from comfy_script.runtime import *
 load()
```


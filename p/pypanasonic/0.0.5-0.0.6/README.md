# Comparing `tmp/pypanasonic-0.0.5.tar.gz` & `tmp/pypanasonic-0.0.6.tar.gz`

## Comparing `pypanasonic-0.0.5.tar` & `pypanasonic-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,17 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pypanasonic-0.0.5/.idea/.gitignore
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 pypanasonic-0.0.5/.idea/misc.xml
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 pypanasonic-0.0.5/.idea/modules.xml
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 pypanasonic-0.0.5/.idea/pypanasonic.iml
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 pypanasonic-0.0.5/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pypanasonic-0.0.5/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 pypanasonic-0.0.5/src/pypanasonic/__about__.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 pypanasonic-0.0.5/src/pypanasonic/__init__.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 pypanasonic-0.0.5/src/pypanasonic/mewtocol.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 pypanasonic-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 pypanasonic-0.0.5/LICENSE.txt
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 pypanasonic-0.0.5/README.md
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 pypanasonic-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 pypanasonic-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pypanasonic-0.0.6/.gitattributes
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pypanasonic-0.0.6/.idea/.gitignore
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 pypanasonic-0.0.6/.idea/misc.xml
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 pypanasonic-0.0.6/.idea/modules.xml
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 pypanasonic-0.0.6/.idea/pypanasonic.iml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pypanasonic-0.0.6/.idea/vcs.xml
+-rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 pypanasonic-0.0.6/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pypanasonic-0.0.6/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 pypanasonic-0.0.6/src/pypanasonic/__about__.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 pypanasonic-0.0.6/src/pypanasonic/__init__.py
+-rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 pypanasonic-0.0.6/src/pypanasonic/mewtocol.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 pypanasonic-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pypanasonic-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 pypanasonic-0.0.6/LICENSE.txt
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 pypanasonic-0.0.6/README.md
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 pypanasonic-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 pypanasonic-0.0.6/PKG-INFO
```

### Comparing `pypanasonic-0.0.5/.idea/workspace.xml` & `pypanasonic-0.0.6/.idea/workspace.xml`

 * *Files 12% similar despite different names*

#### Comparing `pypanasonic-0.0.5/.idea/workspace.xml` & `pypanasonic-0.0.6/.idea/workspace.xml`

```diff
@@ -1,43 +1,52 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="2b1357ce-b248-4f73-891d-de6acd2abccf" name="Changes" comment=""/>
+    <list default="true" id="2b1357ce-b248-4f73-891d-de6acd2abccf" name="Changes" comment="">
+      <change beforePath="$PROJECT_DIR$/README.md" beforeDir="false" afterPath="$PROJECT_DIR$/README.md" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/pypanasonic/mewtocol.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/pypanasonic/mewtocol.py" afterDir="false"/>
+    </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
     <option name="RECENT_TEMPLATES">
       <list>
         <option value="Python Script"/>
       </list>
     </option>
   </component>
+  <component name="Git.Settings">
+    <option name="RECENT_GIT_ROOT_PATH" value="$PROJECT_DIR$"/>
+  </component>
   <component name="MarkdownSettingsMigration">
     <option name="stateVersion" value="1"/>
   </component>
-  <component name="ProjectColorInfo"><![CDATA[{
-  "customColor": "",
-  "associatedIndex": 2
-}]]></component>
+  <component name="ProjectColorInfo">{
+  &quot;customColor&quot;: &quot;&quot;,
+  &quot;associatedIndex&quot;: 2
+}</component>
   <component name="ProjectId" id="2fpGzzWcLkKi3uLtpPYbSzPL7IW"/>
   <component name="ProjectViewState">
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
   </component>
   <component name="PropertiesComponent"><![CDATA[{
   "keyToString": {
     "RunOnceActivity.OpenProjectViewOnStart": "true",
     "RunOnceActivity.ShowReadmeOnStart": "true",
-    "last_opened_file_path": "F:/repopy/pypanasonic"
+    "git-widget-placeholder": "main",
+    "ignore.virus.scanning.warn.message": "true",
+    "last_opened_file_path": "F:/repopy/mewtocol-ex"
   }
 }]]></component>
   <component name="SharedIndexes">
     <attachedChunks>
       <set>
         <option value="bundled-python-sdk-50da183f06c8-d3b881c8e49f-com.jetbrains.pycharm.community.sharedIndexes.bundled-PC-233.13135.95"/>
       </set>
```

### Comparing `pypanasonic-0.0.5/src/pypanasonic/mewtocol.py` & `pypanasonic-0.0.6/src/pypanasonic/mewtocol.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,9 +62,9 @@
     end1 = re.match('^[0-9]+$',End)
     if(not start1 or  not end1):
         exit()
     return "%EE#RDD"+str(Start)+str(End)+"**"+"\r"
 
 # Send message to PLC, you could use that for plc connectection test.
 def plcVer():
-    return "%EE#RT00\r"
+    return "%EE#RT00**\r"
```

### Comparing `pypanasonic-0.0.5/LICENSE.txt` & `pypanasonic-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pypanasonic-0.0.5/pyproject.toml` & `pypanasonic-0.0.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypanasonic"
-version = "0.0.5"
+version = "0.0.6"
 description = "Panasonic PLC mewtocol lib via serial port"
 readme = "README.md"
 requires-python = ">=3.8"
 license = "MIT"
 keywords = ["Panasonic", "Mewtocol", "Protocol", "Serial", "PLC"]
 authors = [
-  { name = "hy1stax", email = "130333760+hy1stax@users.noreply.github.com" },
+  { name = "hy1stax", email = "luweizhao09@gmail.com" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
@@ -24,18 +24,14 @@
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = ["regex",]
 
 [project.urls]
 Homepage = "https://github.com/hy1stax/pypanasonic"
-Documentation = "https://github.com/hy1stax/pypanasonic/README.md"
-Repository = "https://github.com/hy1stax/pypanasonic.git"
-"Bug Tracker" = "https://github.com/hy1stax/pypanasonic/issues"
-Changelog = "https://github.com/hy1stax/pypanasonic/CHANGELOG.md"
 
 [tool.hatch.version]
 path = "src/pypanasonic/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "coverage[toml]>=6.5",
```


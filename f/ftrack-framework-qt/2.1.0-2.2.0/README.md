# Comparing `tmp/ftrack_framework_qt-2.1.0.tar.gz` & `tmp/ftrack_framework_qt-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ftrack_framework_qt-2.1.0.tar", max compression
+gzip compressed data, was "ftrack_framework_qt-2.2.0.tar", max compression
```

## Comparing `ftrack_framework_qt-2.1.0.tar` & `ftrack_framework_qt-2.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    10176 2024-04-02 08:38:27.226584 ftrack_framework_qt-2.1.0/LICENSE.txt
--rw-r--r--   0        0        0      167 2024-04-02 08:38:27.226584 ftrack_framework_qt-2.1.0/README.md
--rw-r--r--   0        0        0     1164 2024-04-02 08:38:27.226584 ftrack_framework_qt-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      463 2024-04-02 08:38:27.226584 ftrack_framework_qt-2.1.0/source/ftrack_framework_qt/__init__.py
--rw-r--r--   0        0        0      199 2024-04-02 08:38:27.226584 ftrack_framework_qt-2.1.0/source/ftrack_framework_qt/dialogs/__init__.py
--rw-r--r--   0        0        0     3295 2024-04-02 08:38:27.226584 ftrack_framework_qt-2.1.0/source/ftrack_framework_qt/dialogs/base_context_dialog.py
--rw-r--r--   0        0        0     5521 2024-04-02 08:38:27.226584 ftrack_framework_qt-2.1.0/source/ftrack_framework_qt/dialogs/base_dialog.py
--rw-r--r--   0        0        0      121 2024-04-02 08:38:27.226584 ftrack_framework_qt-2.1.0/source/ftrack_framework_qt/widgets/__init__.py
--rw-r--r--   0        0        0     1095 2024-04-02 08:38:27.226584 ftrack_framework_qt-2.1.0/source/ftrack_framework_qt/widgets/base_widget.py
--rw-r--r--   0        0        0     1304 1970-01-01 00:00:00.000000 ftrack_framework_qt-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0    10176 2024-05-02 08:05:07.726353 ftrack_framework_qt-2.2.0/LICENSE.txt
+-rw-r--r--   0        0        0      167 2024-05-02 08:05:07.726353 ftrack_framework_qt-2.2.0/README.md
+-rw-r--r--   0        0        0     1282 2024-05-02 08:05:07.726353 ftrack_framework_qt-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0      463 2024-05-02 08:05:07.726353 ftrack_framework_qt-2.2.0/source/ftrack_framework_qt/__init__.py
+-rw-r--r--   0        0        0      199 2024-05-02 08:05:07.726353 ftrack_framework_qt-2.2.0/source/ftrack_framework_qt/dialogs/__init__.py
+-rw-r--r--   0        0        0     3419 2024-05-02 08:05:07.726353 ftrack_framework_qt-2.2.0/source/ftrack_framework_qt/dialogs/base_context_dialog.py
+-rw-r--r--   0        0        0     7863 2024-05-02 08:05:07.726353 ftrack_framework_qt-2.2.0/source/ftrack_framework_qt/dialogs/base_dialog.py
+-rw-r--r--   0        0        0      121 2024-05-02 08:05:07.726353 ftrack_framework_qt-2.2.0/source/ftrack_framework_qt/widgets/__init__.py
+-rw-r--r--   0        0        0     1164 2024-05-02 08:05:07.730353 ftrack_framework_qt-2.2.0/source/ftrack_framework_qt/widgets/base_widget.py
+-rw-r--r--   0        0        0     1437 1970-01-01 00:00:00.000000 ftrack_framework_qt-2.2.0/PKG-INFO
```

### Comparing `ftrack_framework_qt-2.1.0/LICENSE.txt` & `ftrack_framework_qt-2.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ftrack_framework_qt-2.1.0/pyproject.toml` & `ftrack_framework_qt-2.2.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ftrack-framework-qt"
-version = "2.1.0"
+version = "2.2.0"
 description='ftrack framework qt library'
 authors = ["ftrack Integrations Team <integrations@backlight.co>"]
 readme = "README.md"
 packages = [{include = "ftrack_framework_qt", from = "source"}]
 license = "Apache-2.0"
 homepage = "https://ftrack.com"
 repository = "https://github.com/ftrackhq/integrations/tree/main/libs/framework-qt"
@@ -20,22 +20,25 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dependencies]
 python = ">= 3.7, < 3.12"
-"Qt.py" = ">=1.0.0, < 2"
+PySide2 = { version = "^5.13.2", optional = true }
+PySide6 = { version = "^6.5", optional = true }
 #ftrack
 ftrack-constants= {  version = "^2.0.0", optional = true }
 ftrack-utils = {  version = "^2.0.0", optional = true }
 ftrack-qt = {  version = "^2.0.0", optional = true }
 #framework
 ftrack-framework-core = {  version = "^2.0.0", optional = true }
 
 [tool.poetry.extras]
+pyside2 = ["PySide2"]
+pyside6 = ["PySide6"]
 ftrack-libs = ["ftrack-constants", "ftrack-utils", "ftrack-qt"]
 framework-libs = ["ftrack-framework-core"]
 
 [tool.black]
 line-length = 79
 skip-string-normalization = true
```

### Comparing `ftrack_framework_qt-2.1.0/source/ftrack_framework_qt/dialogs/base_context_dialog.py` & `ftrack_framework_qt-2.2.0/source/ftrack_framework_qt/dialogs/base_context_dialog.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
 
-from Qt import QtWidgets, QtCore
+try:
+    from PySide6 import QtWidgets, QtCore
+except ImportError:
+    from PySide2 import QtWidgets, QtCore
 
 from ftrack_framework_qt.dialogs.base_dialog import BaseDialog
 
 from ftrack_qt.widgets.headers import SessionHeader
 from ftrack_qt.widgets.selectors import ContextSelector
 
 
@@ -73,18 +76,20 @@
 
         self._tool_widget = QtWidgets.QWidget()
         _tool_widget_layout = QtWidgets.QVBoxLayout()
         self._tool_widget.setLayout(_tool_widget_layout)
 
         self._run_button = QtWidgets.QPushButton(self.run_button_title)
 
-        self.layout().addWidget(self._header)
-        self.layout().addWidget(self._context_selector, QtCore.Qt.AlignTop)
-        self.layout().addWidget(self._tool_widget)
-        self.layout().addWidget(self._run_button)
+        self.main_layout.addWidget(self._header)
+        self.main_layout.addWidget(
+            self._context_selector, QtCore.Qt.AlignmentFlag.AlignTop
+        )
+        self.main_layout.addWidget(self._tool_widget)
+        self.main_layout.addWidget(self._run_button)
 
     def post_build(self):
         '''Override the post_build method to create context selector signals'''
         super(BaseContextDialog, self).post_build()
         # Connect context selector signals
         self._context_selector.context_changed.connect(
             self._on_context_selected_callback
```

### Comparing `ftrack_framework_qt-2.1.0/source/ftrack_framework_qt/widgets/base_widget.py` & `ftrack_framework_qt-2.2.0/source/ftrack_framework_qt/widgets/base_widget.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
 
-from Qt import QtWidgets, QtCore, QtGui
+try:
+    from PySide6 import QtWidgets, QtCore
+except ImportError:
+    from PySide2 import QtWidgets, QtCore
 
 from ftrack_framework_core.widget.widget import FrameworkWidget
 
 
 class BaseWidget(FrameworkWidget, QtWidgets.QWidget):
     '''Main class to represent base framework widget.'''
```

### Comparing `ftrack_framework_qt-2.1.0/PKG-INFO` & `ftrack_framework_qt-2.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftrack-framework-qt
-Version: 2.1.0
+Version: 2.2.0
 Summary: ftrack framework qt library
 Home-page: https://ftrack.com
 License: Apache-2.0
 Author: ftrack Integrations Team
 Author-email: integrations@backlight.co
 Requires-Python: >=3.7,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,15 +12,18 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: framework-libs
 Provides-Extra: ftrack-libs
-Requires-Dist: Qt.py (>=1.0.0,<2)
+Provides-Extra: pyside2
+Provides-Extra: pyside6
+Requires-Dist: PySide2 (>=5.13.2,<6.0.0) ; extra == "pyside2"
+Requires-Dist: PySide6 (>=6.5,<7.0) ; extra == "pyside6"
 Requires-Dist: ftrack-constants (>=2.0.0,<3.0.0) ; extra == "ftrack-libs"
 Requires-Dist: ftrack-framework-core (>=2.0.0,<3.0.0) ; extra == "framework-libs"
 Requires-Dist: ftrack-qt (>=2.0.0,<3.0.0) ; extra == "ftrack-libs"
 Requires-Dist: ftrack-utils (>=2.0.0,<3.0.0) ; extra == "ftrack-libs"
 Project-URL: Repository, https://github.com/ftrackhq/integrations/tree/main/libs/framework-qt
 Description-Content-Type: text/markdown
```


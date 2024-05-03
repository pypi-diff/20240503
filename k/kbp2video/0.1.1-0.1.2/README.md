# Comparing `tmp/kbp2video-0.1.1.tar.gz` & `tmp/kbp2video-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kbp2video-0.1.1.tar", last modified: Mon Apr 29 21:58:17 2024, max compression
+gzip compressed data, was "kbp2video-0.1.2.tar", last modified: Fri May  3 18:37:35 2024, max compression
```

## Comparing `kbp2video-0.1.1.tar` & `kbp2video-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-04-29 21:58:17.264047 kbp2video-0.1.1/
--rw-r--r--   0 matt      (1000) matt      (1000)    11346 2024-04-25 01:31:39.000000 kbp2video-0.1.1/LICENSE
--rw-r--r--   0 matt      (1000) matt      (1000)      166 2024-04-29 21:58:17.264047 kbp2video-0.1.1/PKG-INFO
--rw-r--r--   0 matt      (1000) matt      (1000)      471 2024-04-25 01:31:39.000000 kbp2video-0.1.1/README.md
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-04-29 21:58:17.260714 kbp2video-0.1.1/kbp2video/
--rw-r--r--   0 matt      (1000) matt      (1000)      290 2024-04-25 01:31:39.000000 kbp2video-0.1.1/kbp2video/__init__.py
--rw-r--r--   0 matt      (1000) matt      (1000)       28 2024-04-25 01:31:39.000000 kbp2video-0.1.1/kbp2video/__main__.py
--rw-r--r--   0 matt      (1000) matt      (1000)      923 2024-04-25 01:31:39.000000 kbp2video-0.1.1/kbp2video/_ffmpegcolor.py
--rw-r--r--   0 matt      (1000) matt      (1000)    74002 2024-04-29 21:56:59.000000 kbp2video-0.1.1/kbp2video/_gui.py
--rw-r--r--   0 matt      (1000) matt      (1000)    14259 2024-04-25 01:31:39.000000 kbp2video-0.1.1/kbp2video/advanced_editor.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1115 2024-04-25 01:31:39.000000 kbp2video-0.1.1/kbp2video/utils.py
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-04-29 21:58:17.260714 kbp2video-0.1.1/kbp2video.egg-info/
--rw-r--r--   0 matt      (1000) matt      (1000)      166 2024-04-29 21:58:17.000000 kbp2video-0.1.1/kbp2video.egg-info/PKG-INFO
--rw-r--r--   0 matt      (1000) matt      (1000)      368 2024-04-29 21:58:17.000000 kbp2video-0.1.1/kbp2video.egg-info/SOURCES.txt
--rw-r--r--   0 matt      (1000) matt      (1000)        1 2024-04-29 21:58:17.000000 kbp2video-0.1.1/kbp2video.egg-info/dependency_links.txt
--rw-r--r--   0 matt      (1000) matt      (1000)       49 2024-04-29 21:58:17.000000 kbp2video-0.1.1/kbp2video.egg-info/entry_points.txt
--rw-r--r--   0 matt      (1000) matt      (1000)       46 2024-04-29 21:58:17.000000 kbp2video-0.1.1/kbp2video.egg-info/requires.txt
--rw-r--r--   0 matt      (1000) matt      (1000)       10 2024-04-29 21:58:17.000000 kbp2video-0.1.1/kbp2video.egg-info/top_level.txt
--rw-r--r--   0 matt      (1000) matt      (1000)      322 2024-04-29 21:56:59.000000 kbp2video-0.1.1/pyproject.toml
--rw-r--r--   0 matt      (1000) matt      (1000)       38 2024-04-29 21:58:17.264047 kbp2video-0.1.1/setup.cfg
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-05-03 18:37:35.103513 kbp2video-0.1.2/
+-rw-r--r--   0 matt      (1000) matt      (1000)    11346 2024-04-25 01:31:39.000000 kbp2video-0.1.2/LICENSE
+-rw-r--r--   0 matt      (1000) matt      (1000)      173 2024-05-03 18:37:35.103513 kbp2video-0.1.2/PKG-INFO
+-rw-r--r--   0 matt      (1000) matt      (1000)      471 2024-04-25 01:31:39.000000 kbp2video-0.1.2/README.md
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-05-03 18:37:35.100180 kbp2video-0.1.2/kbp2video/
+-rw-r--r--   0 matt      (1000) matt      (1000)      312 2024-05-03 18:36:57.000000 kbp2video-0.1.2/kbp2video/__init__.py
+-rw-r--r--   0 matt      (1000) matt      (1000)       28 2024-04-25 01:31:39.000000 kbp2video-0.1.2/kbp2video/__main__.py
+-rw-r--r--   0 matt      (1000) matt      (1000)      923 2024-04-25 01:31:39.000000 kbp2video-0.1.2/kbp2video/_ffmpegcolor.py
+-rw-r--r--   0 matt      (1000) matt      (1000)    75758 2024-05-03 18:36:57.000000 kbp2video-0.1.2/kbp2video/_gui.py
+-rw-r--r--   0 matt      (1000) matt      (1000)    14259 2024-04-25 01:31:39.000000 kbp2video-0.1.2/kbp2video/advanced_editor.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1115 2024-04-25 01:31:39.000000 kbp2video-0.1.2/kbp2video/utils.py
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-05-03 18:37:35.100180 kbp2video-0.1.2/kbp2video.egg-info/
+-rw-r--r--   0 matt      (1000) matt      (1000)      173 2024-05-03 18:37:35.000000 kbp2video-0.1.2/kbp2video.egg-info/PKG-INFO
+-rw-r--r--   0 matt      (1000) matt      (1000)      368 2024-05-03 18:37:35.000000 kbp2video-0.1.2/kbp2video.egg-info/SOURCES.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)        1 2024-05-03 18:37:35.000000 kbp2video-0.1.2/kbp2video.egg-info/dependency_links.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)       49 2024-05-03 18:37:35.000000 kbp2video-0.1.2/kbp2video.egg-info/entry_points.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)       53 2024-05-03 18:37:35.000000 kbp2video-0.1.2/kbp2video.egg-info/requires.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)       10 2024-05-03 18:37:35.000000 kbp2video-0.1.2/kbp2video.egg-info/top_level.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)      414 2024-05-03 18:36:57.000000 kbp2video-0.1.2/pyproject.toml
+-rw-r--r--   0 matt      (1000) matt      (1000)       38 2024-05-03 18:37:35.103513 kbp2video-0.1.2/setup.cfg
```

### Comparing `kbp2video-0.1.1/LICENSE` & `kbp2video-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kbp2video-0.1.1/kbp2video/_ffmpegcolor.py` & `kbp2video-0.1.2/kbp2video/_ffmpegcolor.py`

 * *Files identical despite different names*

### Comparing `kbp2video-0.1.1/kbp2video/_gui.py` & `kbp2video-0.1.2/kbp2video/_gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from .advanced_editor import AdvancedEditor
 import ffmpeg
 from ._ffmpegcolor import ffmpeg_color
 import enum
 import kbputils
 import io
 import shutil
+from . import __version__
 
 class TrackTableColumn(enum.Enum):
     KBP_ASS = 0
     Audio = 1
     Background = 2
     Advanced = 3
 
@@ -507,14 +508,24 @@
         # TODO: Create menubar with contents
         # self.menubar = QMenuBar()
         # self.menubar.setObjectName("menubar")
         # self.menubar.setGeometry(QRect(0, 0, 886, 25))
         # self.menubar.addMenu("test")
         # self.setMenuBar(self.menubar)
         self.setStatusBar(self.bind("statusbar", QStatusBar(self)))
+        try:
+            q = QProcess(program="ffmpeg", arguments=["-version"])
+            q.start()
+            q.waitForFinished(1000)
+            q.setReadChannel(QProcess.StandardOutput)
+            version_line = str(q.readLine()).split()
+            ffmpeg_version = version_line[i+1] if (i := version_line.index("version")) else 'UNKNOWN'
+        except:
+            ffmpeg_version = "MISSING/UNKNOWN"
+        self.statusbar.showMessage(f"kbp2video {__version__} (kbputils {kbputils.__version__}, ffmpeg {ffmpeg_version})")
 
         QCoreApplication.setOrganizationName("ItMightBeKaraoke")
         QCoreApplication.setApplicationName("kbp2video")
         QCoreApplication.setOrganizationDomain("itmightbekaraoke.com")
 
         self.settings = QSettings()
 
@@ -680,14 +691,21 @@
 
         gridRow += 1
         #self.gridLayout.addWidget(self.bind("transparencyBox", QCheckBox(checkState=Qt.Checked if self.settings.value("subtitle/transparent_bg", type=bool, defaultValue=True) else Qt.Unchecked)), gridRow, 0, alignment=Qt.AlignRight)
         self.gridLayout.addWidget(self.bind("transparencyBox", QCheckBox()), gridRow, 0, alignment=Qt.AlignRight)
         self.gridLayout.addWidget(self.bind("transparencyLabel", ClickLabel(buddy=self.transparencyBox, buddyMethod=QCheckBox.toggle)), gridRow, 1, 1, 2)
 
         gridRow += 1
+        self.gridLayout.addWidget(
+            self.bind("overflowBox", QComboBox()), gridRow, 1, 1, 2)
+        self.gridLayout.addWidget(
+            self.bind("overflowLabel", ClickLabel(buddy=self.overflowBox)), gridRow, 0)
+        self.overflowBox.addItems(["no wrap","even split","top split","bottom split"])
+
+        gridRow += 1
         self.gridLayout.addItem(QSpacerItem(20, 20, QSizePolicy.Minimum, QSizePolicy.Expanding), gridRow, 0, 1, 3)
         self.gridLayout.setRowStretch(gridRow, 10)
 
         gridRow += 1
         self.gridLayout.addWidget(self.bind("ffmpegDivider", ClickLabel(
             alignment=Qt.AlignCenter)), gridRow, 0, 1, 3)
 
@@ -973,14 +991,15 @@
         to_save = {
             "subtitle/aspect_ratio": self.aspectRatioBox.currentText(),
             "subtitle/fade_in": self.fadeIn.value(),
             "subtitle/fade_out": self.fadeOut.value(),
             "subtitle/offset": self.offset.value(),
             "subtitle/override_offset": check2bool(self.overrideOffset),
             "subtitle/transparent_bg": check2bool(self.transparencyBox),
+            "subtitle/overflow": self.overflowBox.currentText(),
             "video/background_color": self.colorText.text(),
             "video/output_resolution": self.resolutionBox.currentText(),
             "video/override_bg_resolution": check2bool(self.overrideBGResolution),
             "video/container_format_index": self.containerBox.currentIndex(),
             "video/video_codec_index": self.vcodecBox.currentIndex(),
             "video/lossless": check2bool(self.lossless),
             "video/quality": self.quality.value(),
@@ -1011,14 +1030,15 @@
             self.aspectRatioBox.setCurrentText(aspect_text)
 
         self.fadeIn.setValue(self.settings.value("subtitle/fade_in", type=int, defaultValue=50))
         self.fadeOut.setValue(self.settings.value("subtitle/fade_out", type=int, defaultValue=50))
         self.offset.setValue(self.settings.value("subtitle/offset", type=float, defaultValue=0.0))
         self.offset_check_box(setState=bool2check(self.settings.value("subtitle/override_offset", type=bool, defaultValue=False)))
         self.transparencyBox.setCheckState(bool2check(self.settings.value("subtitle/transparent_bg", type=bool, defaultValue=True)))
+        self.overflowBox.setCurrentText(self.settings.value("subtitle/overflow", type=str, defaultValue="no wrap"))
         self.updateColor(setColor=self.settings.value("video/background_color", type=str, defaultValue="#000000"))
 
         # Restore existing or custom option
         resolution_text = self.settings.value("video/output_resolution", type=str, defaultValue="<NONEXISTENT>")
         if (index := self.resolutionBox.findText(resolution_text)) != -1:
             self.resolutionBox.setCurrentIndex(index)
         elif resolution_text != "<NONEXISTENT>":
@@ -1159,14 +1179,15 @@
         kbputils_options['fade_out'] = self.fadeOut.value()
         if self.overrideOffset.checkState() == Qt.Checked:
             assOptions += ["-o", f"{self.offset.value()}"]
             kbputils_options['offset'] = self.offset.value()
         if self.transparencyBox.checkState() != Qt.Checked:
             assOptions += ["--no-t"]
             kbputils_options['transparency'] = False
+        kbputils_options['overflow'] = kbputils.AssOverflow[self.overflowBox.currentText().replace(" ", "_").upper()]
         for row in range(self.tableWidget.rowCount()):
             kbp_table_item = self.tableWidget.item(row, TrackTableColumn.KBP_ASS.value)
             kbp_obj = kbp_table_item.data(Qt.UserRole) or kbp_table_item.text()
             kbp = str(kbp_obj)
             audio = self.tableWidget.filename(row, TrackTableColumn.Audio.value)
             background = self.tableWidget.filename(row, TrackTableColumn.Background.value)
             advanced = self.tableWidget.item(row, TrackTableColumn.Advanced.value).data(Qt.UserRole) or {}
@@ -1436,14 +1457,18 @@
             "MainWindow", "&Fade In/Out", None))
         self.aspectLabel.setText(QCoreApplication.translate(
             "MainWindow", "A&spect Ratio", None))
         self.transparencyLabel.setText(QCoreApplication.translate(
             "MainWindow", "&Draw BG color transparent", None))
         self.transparencyLabel.setToolTip(QCoreApplication.translate(
             "MainWindow", "When using palette index 0 as a font or border color in KBS, make that color\ntransparent in the resulting .ass file. This improves compatibility with\ndrawing appearing and overlapping text. ", None))
+        self.overflowLabel.setText(QCoreApplication.translate(
+            "MainWindow", "Word Wrappin&g", None))
+        self.overflowBox.setToolTip(QCoreApplication.translate(
+            "MainWindow", "When a line is too wide for the screen, use this strategy to wrap words\n  no wrap: Allow text to go off screen\n  even split: Wrap words in a way that makes the following line(s) about the same size\n  top split: Keep the first line long, only wrap at the word that causes it to go offscreen\n  bottom split: Make the bottom line long when wrapping", None))
         self.overrideOffsetLabel.setText(QCoreApplication.translate(
             "MainWindow", "Overr&ide Timestamp Offset", None))
         self.overrideOffsetLabel.setToolTip(QCoreApplication.translate(
             "MainWindow", "Set an offset to be applied to every timestamp in the KBP file when converting\nto .ass. If not overridden, the setting from within KBS is used if it can be located.", None))
         self.offsetLabel.setText(QCoreApplication.translate(
             "MainWindow", "Timesta&mp Offset", None))
         self.ffmpegDivider.setText(QCoreApplication.translate(
@@ -1459,15 +1484,15 @@
         self.abitrateLabel.setText(QCoreApplication.translate(
             "MainWindow", "Audio &Bitrate", None))
         self.abitrateLabel.setToolTip(QCoreApplication.translate(
             "MainWindow", "Enter a number in bits per second, or suffixed with a k for kilobits per second.", None))
         self.abitrateBox.setPlaceholderText(QCoreApplication.translate(
             "MainWindow", "Leave blank for default", None))
         self.overrideBGLabel.setText(QCoreApplication.translate(
-            "MainWindow", "Override back&ground", None))
+            "MainWindow", "Override background", None))
         self.overrideBGLabel.setToolTip(QCoreApplication.translate(
             "MainWindow", "If this is unchecked, the resolution setting is only used for tracks with\nthe background set as a color. If it is checked, background image/video\nis scaled (and letterboxed if the aspect ratio differs) to achieve the\ntarget resolution.\n\nFEATURE NOT SUPPORTED YET", None))
         self.losslessLabel.setText(QCoreApplication.translate(
             "MainWindow", "Lossless video", None))
         self.lossless.setToolTip(QCoreApplication.translate(
             "MainWindow", "Use lossless quality settings on video (may create very large files).\nFor lossless audio and video, use an mkv container with this checked and flac codec for audio.", None))
         self.qualityLabel.setText(QCoreApplication.translate(
```

### Comparing `kbp2video-0.1.1/kbp2video/advanced_editor.py` & `kbp2video-0.1.2/kbp2video/advanced_editor.py`

 * *Files identical despite different names*

### Comparing `kbp2video-0.1.1/kbp2video/utils.py` & `kbp2video-0.1.2/kbp2video/utils.py`

 * *Files identical despite different names*


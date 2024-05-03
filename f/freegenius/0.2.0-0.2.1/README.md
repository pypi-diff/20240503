# Comparing `tmp/freegenius-0.2.0.tar.gz` & `tmp/freegenius-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freegenius-0.2.0.tar", last modified: Thu May  2 19:11:46 2024, max compression
+gzip compressed data, was "freegenius-0.2.1.tar", last modified: Thu May  2 21:58:50 2024, max compression
```

## Comparing `freegenius-0.2.0.tar` & `freegenius-0.2.1.tar`

### file list

```diff
@@ -1,180 +1,180 @@
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 19:11:46.465759 freegenius-0.2.0/
--rw-r--r--   0 eliran    (1000) eliran    (1000)    14884 2024-05-02 19:11:46.465759 freegenius-0.2.0/PKG-INFO
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 19:11:46.437759 freegenius-0.2.0/freegenius/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    11707 2024-05-02 19:11:46.000000 freegenius-0.2.0/freegenius/README.md
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3316 2024-04-11 08:45:18.000000 freegenius-0.2.0/freegenius/__init__.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 19:11:46.437759 freegenius-0.2.0/freegenius/audio/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    15588 2024-02-18 17:53:14.000000 freegenius-0.2.0/freegenius/audio/notification1.mp3
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2925 2024-02-20 11:12:21.000000 freegenius-0.2.0/freegenius/audio/notification1_mild.mp3
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    19428 2024-02-18 17:51:50.000000 freegenius-0.2.0/freegenius/audio/notification2.mp3
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3693 2024-02-20 11:18:40.000000 freegenius-0.2.0/freegenius/audio/notification2_mild.mp3
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7006 2024-04-28 21:17:47.000000 freegenius-0.2.0/freegenius/autoassist.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     9421 2024-04-13 20:55:38.000000 freegenius-0.2.0/freegenius/autobuilder.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    11081 2024-04-28 21:19:22.000000 freegenius-0.2.0/freegenius/autoretriever.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6933 2024-04-03 20:55:06.000000 freegenius-0.2.0/freegenius/chatgpt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7037 2024-04-03 20:55:57.000000 freegenius-0.2.0/freegenius/codey.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      833 2024-03-25 21:25:36.000000 freegenius-0.2.0/freegenius/commandprompt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)        0 2024-05-02 19:11:46.000000 freegenius-0.2.0/freegenius/config.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    29583 2023-12-02 22:39:56.000000 freegenius-0.2.0/freegenius/eTextEdit.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 19:11:46.437759 freegenius-0.2.0/freegenius/files/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       31 2023-11-28 12:28:19.000000 freegenius-0.2.0/freegenius/files/Readme.md
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    11372 2024-04-16 20:22:58.000000 freegenius-0.2.0/freegenius/geminipro.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7838 2024-04-16 20:22:58.000000 freegenius-0.2.0/freegenius/geminiprovision.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6470 2024-05-02 18:09:51.000000 freegenius-0.2.0/freegenius/groqchat.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 19:11:46.437759 freegenius-0.2.0/freegenius/gui/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     9741 2024-04-09 22:46:08.000000 freegenius-0.2.0/freegenius/gui/chatgui.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2154 2024-03-12 11:57:01.000000 freegenius-0.2.0/freegenius/gui/worker.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 19:11:46.437759 freegenius-0.2.0/freegenius/history/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       29 2023-11-28 12:28:19.000000 freegenius-0.2.0/freegenius/history/Readme.md
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 19:11:46.449759 freegenius-0.2.0/freegenius/icons/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)   158655 2024-04-10 10:01:55.000000 freegenius-0.2.0/freegenius/icons/FreeGenius.ico
--rw-rw-r--   0 eliran    (1000) eliran    (1000)  2549036 2024-04-10 09:49:32.000000 freegenius-0.2.0/freegenius/icons/FreeGenius.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)  3162696 2024-04-10 09:20:11.000000 freegenius-0.2.0/freegenius/icons/FreeGenius_original.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)  3141194 2024-04-10 09:41:18.000000 freegenius-0.2.0/freegenius/icons/ai.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)  2390858 2024-04-10 09:27:35.000000 freegenius-0.2.0/freegenius/icons/ai_original.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     8119 2024-04-11 14:34:40.000000 freegenius-0.2.0/freegenius/llamacpp.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 19:11:46.433759 freegenius-0.2.0/freegenius/macOS_service/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 19:11:46.429759 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Download_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 19:11:46.453759 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      644 2024-04-06 16:47:12.000000 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 19:11:46.453759 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5680 2024-04-06 16:46:45.000000 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 19:11:46.429759 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Explanation_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 19:11:46.453759 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 19:11:46.453759 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5679 2024-04-06 16:46:45.000000 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 19:11:46.429759 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Files_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 19:11:46.453759 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/
--rw-r--r--   0 eliran    (1000) eliran    (1000)      635 2024-04-06 16:47:12.000000 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 19:11:46.453759 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/
--rw-r--r--   0 eliran    (1000) eliran    (1000)     4100 2023-12-01 10:53:39.000000 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5684 2024-04-06 16:46:45.000000 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 19:11:46.429759 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Pronounce_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 19:11:46.453759 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      649 2024-04-06 16:47:12.000000 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 19:11:46.453759 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 19:11:46.429759 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Summary_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 19:11:46.453759 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      643 2024-04-06 16:47:12.000000 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 19:11:46.453759 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 19:11:46.433759 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Text_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 19:11:46.453759 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/
--rw-r--r--   0 eliran    (1000) eliran    (1000)      640 2024-04-06 16:47:12.000000 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 19:11:46.453759 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/
--rw-r--r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-01 10:53:44.000000 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5656 2024-04-06 16:46:45.000000 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 19:11:46.433759 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Translation_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 19:11:46.453759 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 19:11:46.453759 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 19:11:46.433759 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 19:11:46.453759 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 19:11:46.453759 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5692 2024-04-06 16:46:45.000000 freegenius-0.2.0/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7320 2024-04-10 10:50:28.000000 freegenius-0.2.0/freegenius/main.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    10959 2024-04-07 18:24:27.000000 freegenius-0.2.0/freegenius/ollamachat.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       10 2024-05-02 19:11:46.000000 freegenius-0.2.0/freegenius/package_name.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7573 2024-04-03 20:57:58.000000 freegenius-0.2.0/freegenius/palm2.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 19:11:46.461759 freegenius-0.2.0/freegenius/plugins/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1326 2024-03-25 18:25:44.000000 freegenius-0.2.0/freegenius/plugins/000_check_ffmpeg.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1616 2024-04-25 10:21:23.000000 freegenius-0.2.0/freegenius/plugins/000_check_pyaudio.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1465 2024-03-25 18:26:33.000000 freegenius-0.2.0/freegenius/plugins/000_check_vlc.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      115 2023-11-28 12:28:19.000000 freegenius-0.2.0/freegenius/plugins/Readme.md
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6812 2024-04-12 22:35:03.000000 freegenius-0.2.0/freegenius/plugins/add calendar event.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3358 2024-04-02 21:37:01.000000 freegenius-0.2.0/freegenius/plugins/aliases.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7437 2024-04-27 13:00:33.000000 freegenius-0.2.0/freegenius/plugins/analyze audio.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2154 2024-04-09 10:22:46.000000 freegenius-0.2.0/freegenius/plugins/analyze files.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4677 2024-04-27 13:03:55.000000 freegenius-0.2.0/freegenius/plugins/analyze images.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2316 2024-04-09 22:27:35.000000 freegenius-0.2.0/freegenius/plugins/analyze web content.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2559 2024-04-14 22:20:21.000000 freegenius-0.2.0/freegenius/plugins/auto correct python code.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1860 2024-04-02 21:37:01.000000 freegenius-0.2.0/freegenius/plugins/awesome prompts.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5876 2024-04-02 21:37:01.000000 freegenius-0.2.0/freegenius/plugins/character analysis.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      654 2024-04-04 22:28:27.000000 freegenius-0.2.0/freegenius/plugins/chat.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      762 2024-04-04 08:36:50.000000 freegenius-0.2.0/freegenius/plugins/contexts.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7220 2024-04-02 21:37:01.000000 freegenius-0.2.0/freegenius/plugins/counselling.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1688 2024-04-04 22:11:59.000000 freegenius-0.2.0/freegenius/plugins/create ai assistants.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5160 2024-04-27 13:04:35.000000 freegenius-0.2.0/freegenius/plugins/create images.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1262 2024-04-10 07:42:48.000000 freegenius-0.2.0/freegenius/plugins/create maps.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1520 2024-04-04 22:15:17.000000 freegenius-0.2.0/freegenius/plugins/create qrcode.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1522 2024-04-10 07:42:48.000000 freegenius-0.2.0/freegenius/plugins/create statistical graphics.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1211 2024-04-13 22:43:22.000000 freegenius-0.2.0/freegenius/plugins/dates and times.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3950 2024-04-09 22:27:52.000000 freegenius-0.2.0/freegenius/plugins/download youtube or web content.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1862 2024-04-05 11:08:57.000000 freegenius-0.2.0/freegenius/plugins/edit text.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3316 2024-04-13 22:42:39.000000 freegenius-0.2.0/freegenius/plugins/execute computing tasks.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4213 2024-04-09 22:24:00.000000 freegenius-0.2.0/freegenius/plugins/execute termux command.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6940 2024-04-02 21:37:01.000000 freegenius-0.2.0/freegenius/plugins/global finance.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      975 2024-04-02 21:37:01.000000 freegenius-0.2.0/freegenius/plugins/improve British English.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2315 2024-04-25 10:21:23.000000 freegenius-0.2.0/freegenius/plugins/input suggestions.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1077 2024-04-07 19:39:31.000000 freegenius-0.2.0/freegenius/plugins/install python package.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1670 2024-04-04 22:36:17.000000 freegenius-0.2.0/freegenius/plugins/integrate google searches.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4606 2024-04-11 22:17:28.000000 freegenius-0.2.0/freegenius/plugins/memory.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     8646 2024-04-27 13:03:30.000000 freegenius-0.2.0/freegenius/plugins/modify images.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      944 2024-04-09 22:25:30.000000 freegenius-0.2.0/freegenius/plugins/open web browser.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1296 2024-04-05 11:14:34.000000 freegenius-0.2.0/freegenius/plugins/pronounce words.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2409 2024-04-10 07:42:48.000000 freegenius-0.2.0/freegenius/plugins/remove image background.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5906 2024-04-27 11:30:39.000000 freegenius-0.2.0/freegenius/plugins/search chat records.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1156 2024-04-10 07:42:48.000000 freegenius-0.2.0/freegenius/plugins/search financial data.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1966 2024-04-04 22:42:40.000000 freegenius-0.2.0/freegenius/plugins/search latest news.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3479 2024-04-11 22:13:56.000000 freegenius-0.2.0/freegenius/plugins/search sqlite.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1539 2024-04-10 07:42:48.000000 freegenius-0.2.0/freegenius/plugins/search weather info.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3987 2024-04-09 22:25:48.000000 freegenius-0.2.0/freegenius/plugins/send email.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      898 2024-04-09 22:26:03.000000 freegenius-0.2.0/freegenius/plugins/send tweet.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1280 2024-04-05 11:15:56.000000 freegenius-0.2.0/freegenius/plugins/send whatsapp messages.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      528 2024-04-02 21:37:01.000000 freegenius-0.2.0/freegenius/plugins/simplified Chinese to traditional Chinese.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      242 2024-03-25 12:56:42.000000 freegenius-0.2.0/freegenius/qt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     9711 2024-04-09 10:22:46.000000 freegenius-0.2.0/freegenius/rag.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      840 2024-04-26 22:24:44.000000 freegenius-0.2.0/freegenius/requirements.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1359 2024-04-25 20:30:31.000000 freegenius-0.2.0/freegenius/servers.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7714 2024-04-27 15:10:04.000000 freegenius-0.2.0/freegenius/systemtray.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 19:11:46.461759 freegenius-0.2.0/freegenius/temp/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       36 2023-11-28 12:28:19.000000 freegenius-0.2.0/freegenius/temp/Readme.md
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 19:11:46.465759 freegenius-0.2.0/freegenius/utils/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)   112149 2024-05-02 18:49:22.000000 freegenius-0.2.0/freegenius/utils/assistant.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    29750 2024-05-02 18:43:53.000000 freegenius-0.2.0/freegenius/utils/call_chatgpt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    17281 2024-05-02 18:43:53.000000 freegenius-0.2.0/freegenius/utils/call_gemini.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    20049 2024-05-02 19:08:49.000000 freegenius-0.2.0/freegenius/utils/call_groq.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    24628 2024-05-02 18:43:56.000000 freegenius-0.2.0/freegenius/utils/call_llamacpp.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     8528 2024-04-27 07:40:12.000000 freegenius-0.2.0/freegenius/utils/call_llm.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    18685 2024-05-02 18:43:53.000000 freegenius-0.2.0/freegenius/utils/call_ollama.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    18484 2024-05-02 18:14:18.000000 freegenius-0.2.0/freegenius/utils/config_essential.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2616 2024-04-03 21:01:16.000000 freegenius-0.2.0/freegenius/utils/config_tools.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1368 2024-03-27 21:22:10.000000 freegenius-0.2.0/freegenius/utils/download.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    14296 2024-04-03 21:01:58.000000 freegenius-0.2.0/freegenius/utils/get_path_prompt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4888 2024-04-23 21:13:11.000000 freegenius-0.2.0/freegenius/utils/ollama_models.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3872 2024-04-09 22:46:08.000000 freegenius-0.2.0/freegenius/utils/promptValidator.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6973 2024-03-25 11:20:01.000000 freegenius-0.2.0/freegenius/utils/prompt_multiline_shared_key_bindings.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7880 2024-04-09 22:40:12.000000 freegenius-0.2.0/freegenius/utils/prompt_shared_key_bindings.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    21592 2024-04-09 22:46:08.000000 freegenius-0.2.0/freegenius/utils/prompts.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1681 2024-04-12 23:13:01.000000 freegenius-0.2.0/freegenius/utils/python_utils.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    50846 2024-04-28 21:25:47.000000 freegenius-0.2.0/freegenius/utils/shared_utils.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    21476 2024-04-10 11:33:28.000000 freegenius-0.2.0/freegenius/utils/shortcuts.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     8558 2024-04-04 08:45:13.000000 freegenius-0.2.0/freegenius/utils/single_prompt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7936 2024-04-09 10:22:46.000000 freegenius-0.2.0/freegenius/utils/streaming_word_wrapper.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7580 2024-02-22 12:18:47.000000 freegenius-0.2.0/freegenius/utils/sttLanguages.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4781 2024-03-26 19:39:22.000000 freegenius-0.2.0/freegenius/utils/terminal_mode_dialogs.py
--rwxrwxr-x   0 eliran    (1000) eliran    (1000)     9891 2024-04-03 21:02:14.000000 freegenius-0.2.0/freegenius/utils/terminal_system_command_prompt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    23917 2024-03-12 11:57:01.000000 freegenius-0.2.0/freegenius/utils/text_utils.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4353 2024-05-02 17:22:30.000000 freegenius-0.2.0/freegenius/utils/tool_plugins.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7640 2024-02-22 00:47:05.000000 freegenius-0.2.0/freegenius/utils/ttsLanguages.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     8563 2024-03-28 23:38:45.000000 freegenius-0.2.0/freegenius/utils/tts_utils.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4651 2024-04-09 22:46:08.000000 freegenius-0.2.0/freegenius/utils/vlc_utils.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 19:11:46.465759 freegenius-0.2.0/freegenius.egg-info/
--rw-r--r--   0 eliran    (1000) eliran    (1000)    14884 2024-05-02 19:11:46.000000 freegenius-0.2.0/freegenius.egg-info/PKG-INFO
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5909 2024-05-02 19:11:46.000000 freegenius-0.2.0/freegenius.egg-info/SOURCES.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)        1 2024-05-02 19:11:46.000000 freegenius-0.2.0/freegenius.egg-info/dependency_links.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1262 2024-05-02 19:11:46.000000 freegenius-0.2.0/freegenius.egg-info/entry_points.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      841 2024-05-02 19:11:46.000000 freegenius-0.2.0/freegenius.egg-info/requires.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       11 2024-05-02 19:11:46.000000 freegenius-0.2.0/freegenius.egg-info/top_level.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       38 2024-05-02 19:11:46.465759 freegenius-0.2.0/setup.cfg
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    10455 2024-05-02 19:11:34.000000 freegenius-0.2.0/setup.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 21:58:50.664007 freegenius-0.2.1/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)    14884 2024-05-02 21:58:50.664007 freegenius-0.2.1/PKG-INFO
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 21:58:50.632007 freegenius-0.2.1/freegenius/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    11707 2024-05-02 21:58:50.000000 freegenius-0.2.1/freegenius/README.md
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3316 2024-04-11 08:45:18.000000 freegenius-0.2.1/freegenius/__init__.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 21:58:50.636007 freegenius-0.2.1/freegenius/audio/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    15588 2024-02-18 17:53:14.000000 freegenius-0.2.1/freegenius/audio/notification1.mp3
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2925 2024-02-20 11:12:21.000000 freegenius-0.2.1/freegenius/audio/notification1_mild.mp3
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    19428 2024-02-18 17:51:50.000000 freegenius-0.2.1/freegenius/audio/notification2.mp3
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3693 2024-02-20 11:18:40.000000 freegenius-0.2.1/freegenius/audio/notification2_mild.mp3
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7006 2024-04-28 21:17:47.000000 freegenius-0.2.1/freegenius/autoassist.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     9421 2024-04-13 20:55:38.000000 freegenius-0.2.1/freegenius/autobuilder.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    11081 2024-04-28 21:19:22.000000 freegenius-0.2.1/freegenius/autoretriever.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6933 2024-04-03 20:55:06.000000 freegenius-0.2.1/freegenius/chatgpt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7037 2024-04-03 20:55:57.000000 freegenius-0.2.1/freegenius/codey.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      833 2024-03-25 21:25:36.000000 freegenius-0.2.1/freegenius/commandprompt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)        0 2024-05-02 21:58:50.000000 freegenius-0.2.1/freegenius/config.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    29583 2023-12-02 22:39:56.000000 freegenius-0.2.1/freegenius/eTextEdit.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 21:58:50.636007 freegenius-0.2.1/freegenius/files/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       31 2023-11-28 12:28:19.000000 freegenius-0.2.1/freegenius/files/Readme.md
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    11372 2024-04-16 20:22:58.000000 freegenius-0.2.1/freegenius/geminipro.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7838 2024-04-16 20:22:58.000000 freegenius-0.2.1/freegenius/geminiprovision.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6513 2024-05-02 21:45:33.000000 freegenius-0.2.1/freegenius/groqchat.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 21:58:50.636007 freegenius-0.2.1/freegenius/gui/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     9741 2024-04-09 22:46:08.000000 freegenius-0.2.1/freegenius/gui/chatgui.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2154 2024-03-12 11:57:01.000000 freegenius-0.2.1/freegenius/gui/worker.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 21:58:50.636007 freegenius-0.2.1/freegenius/history/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       29 2023-11-28 12:28:19.000000 freegenius-0.2.1/freegenius/history/Readme.md
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 21:58:50.648007 freegenius-0.2.1/freegenius/icons/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)   158655 2024-04-10 10:01:55.000000 freegenius-0.2.1/freegenius/icons/FreeGenius.ico
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)  2549036 2024-04-10 09:49:32.000000 freegenius-0.2.1/freegenius/icons/FreeGenius.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)  3162696 2024-04-10 09:20:11.000000 freegenius-0.2.1/freegenius/icons/FreeGenius_original.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)  3141194 2024-04-10 09:41:18.000000 freegenius-0.2.1/freegenius/icons/ai.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)  2390858 2024-04-10 09:27:35.000000 freegenius-0.2.1/freegenius/icons/ai_original.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     8119 2024-04-11 14:34:40.000000 freegenius-0.2.1/freegenius/llamacpp.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 21:58:50.628007 freegenius-0.2.1/freegenius/macOS_service/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 21:58:50.628007 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Download_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 21:58:50.648007 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      644 2024-04-06 16:47:12.000000 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 21:58:50.648007 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5680 2024-04-06 16:46:45.000000 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 21:58:50.628007 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Explanation_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 21:58:50.652007 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 21:58:50.652007 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5679 2024-04-06 16:46:45.000000 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 21:58:50.628007 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Files_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 21:58:50.652007 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)      635 2024-04-06 16:47:12.000000 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 21:58:50.652007 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)     4100 2023-12-01 10:53:39.000000 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5684 2024-04-06 16:46:45.000000 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 21:58:50.628007 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Pronounce_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 21:58:50.652007 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      649 2024-04-06 16:47:12.000000 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 21:58:50.652007 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 21:58:50.628007 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Summary_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 21:58:50.652007 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      643 2024-04-06 16:47:12.000000 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 21:58:50.652007 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 21:58:50.628007 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Text_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 21:58:50.652007 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)      640 2024-04-06 16:47:12.000000 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 21:58:50.652007 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-01 10:53:44.000000 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5656 2024-04-06 16:46:45.000000 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 21:58:50.628007 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Translation_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 21:58:50.652007 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 21:58:50.652007 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 21:58:50.628007 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 21:58:50.652007 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 21:58:50.652007 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5692 2024-04-06 16:46:45.000000 freegenius-0.2.1/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7320 2024-04-10 10:50:28.000000 freegenius-0.2.1/freegenius/main.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    10959 2024-04-07 18:24:27.000000 freegenius-0.2.1/freegenius/ollamachat.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       10 2024-05-02 21:58:50.000000 freegenius-0.2.1/freegenius/package_name.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7573 2024-04-03 20:57:58.000000 freegenius-0.2.1/freegenius/palm2.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 21:58:50.660007 freegenius-0.2.1/freegenius/plugins/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1326 2024-03-25 18:25:44.000000 freegenius-0.2.1/freegenius/plugins/000_check_ffmpeg.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1616 2024-04-25 10:21:23.000000 freegenius-0.2.1/freegenius/plugins/000_check_pyaudio.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1465 2024-03-25 18:26:33.000000 freegenius-0.2.1/freegenius/plugins/000_check_vlc.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      115 2023-11-28 12:28:19.000000 freegenius-0.2.1/freegenius/plugins/Readme.md
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6812 2024-04-12 22:35:03.000000 freegenius-0.2.1/freegenius/plugins/add calendar event.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3358 2024-04-02 21:37:01.000000 freegenius-0.2.1/freegenius/plugins/aliases.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7437 2024-04-27 13:00:33.000000 freegenius-0.2.1/freegenius/plugins/analyze audio.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2154 2024-04-09 10:22:46.000000 freegenius-0.2.1/freegenius/plugins/analyze files.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4677 2024-04-27 13:03:55.000000 freegenius-0.2.1/freegenius/plugins/analyze images.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2316 2024-04-09 22:27:35.000000 freegenius-0.2.1/freegenius/plugins/analyze web content.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2563 2024-05-02 19:23:00.000000 freegenius-0.2.1/freegenius/plugins/auto correct python code.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1860 2024-04-02 21:37:01.000000 freegenius-0.2.1/freegenius/plugins/awesome prompts.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5876 2024-04-02 21:37:01.000000 freegenius-0.2.1/freegenius/plugins/character analysis.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      654 2024-04-04 22:28:27.000000 freegenius-0.2.1/freegenius/plugins/chat.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      762 2024-04-04 08:36:50.000000 freegenius-0.2.1/freegenius/plugins/contexts.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7220 2024-04-02 21:37:01.000000 freegenius-0.2.1/freegenius/plugins/counselling.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1688 2024-04-04 22:11:59.000000 freegenius-0.2.1/freegenius/plugins/create ai assistants.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5160 2024-04-27 13:04:35.000000 freegenius-0.2.1/freegenius/plugins/create images.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1262 2024-04-10 07:42:48.000000 freegenius-0.2.1/freegenius/plugins/create maps.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1520 2024-04-04 22:15:17.000000 freegenius-0.2.1/freegenius/plugins/create qrcode.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1522 2024-04-10 07:42:48.000000 freegenius-0.2.1/freegenius/plugins/create statistical graphics.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1211 2024-04-13 22:43:22.000000 freegenius-0.2.1/freegenius/plugins/dates and times.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3950 2024-04-09 22:27:52.000000 freegenius-0.2.1/freegenius/plugins/download youtube or web content.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1862 2024-04-05 11:08:57.000000 freegenius-0.2.1/freegenius/plugins/edit text.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3316 2024-04-13 22:42:39.000000 freegenius-0.2.1/freegenius/plugins/execute computing tasks.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4213 2024-04-09 22:24:00.000000 freegenius-0.2.1/freegenius/plugins/execute termux command.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6940 2024-04-02 21:37:01.000000 freegenius-0.2.1/freegenius/plugins/global finance.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      975 2024-04-02 21:37:01.000000 freegenius-0.2.1/freegenius/plugins/improve British English.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2315 2024-04-25 10:21:23.000000 freegenius-0.2.1/freegenius/plugins/input suggestions.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1077 2024-04-07 19:39:31.000000 freegenius-0.2.1/freegenius/plugins/install python package.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1670 2024-04-04 22:36:17.000000 freegenius-0.2.1/freegenius/plugins/integrate google searches.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4606 2024-04-11 22:17:28.000000 freegenius-0.2.1/freegenius/plugins/memory.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     8646 2024-04-27 13:03:30.000000 freegenius-0.2.1/freegenius/plugins/modify images.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      944 2024-04-09 22:25:30.000000 freegenius-0.2.1/freegenius/plugins/open web browser.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1296 2024-04-05 11:14:34.000000 freegenius-0.2.1/freegenius/plugins/pronounce words.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2409 2024-04-10 07:42:48.000000 freegenius-0.2.1/freegenius/plugins/remove image background.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5906 2024-04-27 11:30:39.000000 freegenius-0.2.1/freegenius/plugins/search chat records.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1165 2024-05-02 19:22:09.000000 freegenius-0.2.1/freegenius/plugins/search financial data.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1966 2024-04-04 22:42:40.000000 freegenius-0.2.1/freegenius/plugins/search latest news.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3479 2024-04-11 22:13:56.000000 freegenius-0.2.1/freegenius/plugins/search sqlite.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1539 2024-04-10 07:42:48.000000 freegenius-0.2.1/freegenius/plugins/search weather info.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3987 2024-04-09 22:25:48.000000 freegenius-0.2.1/freegenius/plugins/send email.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      898 2024-04-09 22:26:03.000000 freegenius-0.2.1/freegenius/plugins/send tweet.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1280 2024-04-05 11:15:56.000000 freegenius-0.2.1/freegenius/plugins/send whatsapp messages.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      528 2024-04-02 21:37:01.000000 freegenius-0.2.1/freegenius/plugins/simplified Chinese to traditional Chinese.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      242 2024-03-25 12:56:42.000000 freegenius-0.2.1/freegenius/qt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     9711 2024-04-09 10:22:46.000000 freegenius-0.2.1/freegenius/rag.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      840 2024-04-26 22:24:44.000000 freegenius-0.2.1/freegenius/requirements.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1359 2024-04-25 20:30:31.000000 freegenius-0.2.1/freegenius/servers.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7714 2024-04-27 15:10:04.000000 freegenius-0.2.1/freegenius/systemtray.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 21:58:50.660007 freegenius-0.2.1/freegenius/temp/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       36 2023-11-28 12:28:19.000000 freegenius-0.2.1/freegenius/temp/Readme.md
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 21:58:50.664007 freegenius-0.2.1/freegenius/utils/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)   112149 2024-05-02 18:49:22.000000 freegenius-0.2.1/freegenius/utils/assistant.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    29750 2024-05-02 18:43:53.000000 freegenius-0.2.1/freegenius/utils/call_chatgpt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    17281 2024-05-02 18:43:53.000000 freegenius-0.2.1/freegenius/utils/call_gemini.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    20964 2024-05-02 21:47:17.000000 freegenius-0.2.1/freegenius/utils/call_groq.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    24628 2024-05-02 18:43:56.000000 freegenius-0.2.1/freegenius/utils/call_llamacpp.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     8528 2024-04-27 07:40:12.000000 freegenius-0.2.1/freegenius/utils/call_llm.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    18685 2024-05-02 18:43:53.000000 freegenius-0.2.1/freegenius/utils/call_ollama.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    18484 2024-05-02 18:14:18.000000 freegenius-0.2.1/freegenius/utils/config_essential.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2616 2024-04-03 21:01:16.000000 freegenius-0.2.1/freegenius/utils/config_tools.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1368 2024-03-27 21:22:10.000000 freegenius-0.2.1/freegenius/utils/download.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    14296 2024-04-03 21:01:58.000000 freegenius-0.2.1/freegenius/utils/get_path_prompt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4888 2024-04-23 21:13:11.000000 freegenius-0.2.1/freegenius/utils/ollama_models.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3872 2024-04-09 22:46:08.000000 freegenius-0.2.1/freegenius/utils/promptValidator.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6973 2024-03-25 11:20:01.000000 freegenius-0.2.1/freegenius/utils/prompt_multiline_shared_key_bindings.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7880 2024-04-09 22:40:12.000000 freegenius-0.2.1/freegenius/utils/prompt_shared_key_bindings.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    21592 2024-04-09 22:46:08.000000 freegenius-0.2.1/freegenius/utils/prompts.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1681 2024-04-12 23:13:01.000000 freegenius-0.2.1/freegenius/utils/python_utils.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    50846 2024-04-28 21:25:47.000000 freegenius-0.2.1/freegenius/utils/shared_utils.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    21476 2024-04-10 11:33:28.000000 freegenius-0.2.1/freegenius/utils/shortcuts.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     8558 2024-04-04 08:45:13.000000 freegenius-0.2.1/freegenius/utils/single_prompt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7936 2024-04-09 10:22:46.000000 freegenius-0.2.1/freegenius/utils/streaming_word_wrapper.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7580 2024-02-22 12:18:47.000000 freegenius-0.2.1/freegenius/utils/sttLanguages.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4781 2024-03-26 19:39:22.000000 freegenius-0.2.1/freegenius/utils/terminal_mode_dialogs.py
+-rwxrwxr-x   0 eliran    (1000) eliran    (1000)     9891 2024-04-03 21:02:14.000000 freegenius-0.2.1/freegenius/utils/terminal_system_command_prompt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    23917 2024-03-12 11:57:01.000000 freegenius-0.2.1/freegenius/utils/text_utils.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4353 2024-05-02 17:22:30.000000 freegenius-0.2.1/freegenius/utils/tool_plugins.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7640 2024-02-22 00:47:05.000000 freegenius-0.2.1/freegenius/utils/ttsLanguages.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     8563 2024-03-28 23:38:45.000000 freegenius-0.2.1/freegenius/utils/tts_utils.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4651 2024-04-09 22:46:08.000000 freegenius-0.2.1/freegenius/utils/vlc_utils.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 21:58:50.664007 freegenius-0.2.1/freegenius.egg-info/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)    14884 2024-05-02 21:58:50.000000 freegenius-0.2.1/freegenius.egg-info/PKG-INFO
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5909 2024-05-02 21:58:50.000000 freegenius-0.2.1/freegenius.egg-info/SOURCES.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)        1 2024-05-02 21:58:50.000000 freegenius-0.2.1/freegenius.egg-info/dependency_links.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1262 2024-05-02 21:58:50.000000 freegenius-0.2.1/freegenius.egg-info/entry_points.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      841 2024-05-02 21:58:50.000000 freegenius-0.2.1/freegenius.egg-info/requires.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       11 2024-05-02 21:58:50.000000 freegenius-0.2.1/freegenius.egg-info/top_level.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       38 2024-05-02 21:58:50.664007 freegenius-0.2.1/setup.cfg
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    10455 2024-05-02 21:43:41.000000 freegenius-0.2.1/setup.py
```

### Comparing `freegenius-0.2.0/PKG-INFO` & `freegenius-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freegenius
-Version: 0.2.0
+Version: 0.2.1
 Summary: FreeGenius AI, an advanced AI assistant that can talk and take multi-step actions. Supports numerous open-source LLMs via Llama.cpp or Ollama or Groq Cloud API, with optional integration with AutoGen agents, OpenAI API, Google Gemini Pro and unlimited plugins.
 Home-page: https://letmedoit.ai
 Author: Eliran Wong
 Author-email: support@letmedoit.ai
 License: GNU General Public License (GPL)
 Project-URL: Source, https://github.com/eliranwong/letmedoit
 Project-URL: Tracker, https://github.com/eliranwong/letmedoit/issues
```

### Comparing `freegenius-0.2.0/freegenius/README.md` & `freegenius-0.2.1/freegenius/README.md`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/__init__.py` & `freegenius-0.2.1/freegenius/__init__.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/audio/notification1.mp3` & `freegenius-0.2.1/freegenius/audio/notification1.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/audio/notification1_mild.mp3` & `freegenius-0.2.1/freegenius/audio/notification1_mild.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/audio/notification2.mp3` & `freegenius-0.2.1/freegenius/audio/notification2.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/audio/notification2_mild.mp3` & `freegenius-0.2.1/freegenius/audio/notification2_mild.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/autoassist.py` & `freegenius-0.2.1/freegenius/autoassist.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/autobuilder.py` & `freegenius-0.2.1/freegenius/autobuilder.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/autoretriever.py` & `freegenius-0.2.1/freegenius/autoretriever.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/chatgpt.py` & `freegenius-0.2.1/freegenius/chatgpt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/codey.py` & `freegenius-0.2.1/freegenius/codey.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/commandprompt.py` & `freegenius-0.2.1/freegenius/commandprompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/eTextEdit.py` & `freegenius-0.2.1/freegenius/eTextEdit.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/geminipro.py` & `freegenius-0.2.1/freegenius/geminipro.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/geminiprovision.py` & `freegenius-0.2.1/freegenius/geminiprovision.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/groqchat.py` & `freegenius-0.2.1/freegenius/groqchat.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
     """
     A simple Groq chatbot, without function calling.
     It is created for use with 3rd-party applications.
     """
 
     def __init__(self, name="Groq Chatbot", temperature=config.llmTemperature, max_output_tokens=config.groqApi_max_tokens):
         self.name, self.temperature, self.max_output_tokens = name, temperature, max_output_tokens
-        self.client = getGroqClient()
         self.messages = self.resetMessages()
         if hasattr(config, "currentMessages") and config.currentMessages:
             self.messages += config.currentMessages[:-1]
         self.defaultPrompt = ""
 
     def resetMessages(self):
         return [{"role": "system", "content": config.systemMessage_groq},]
@@ -69,21 +68,22 @@
                 self.messages = self.resetMessages()
                 print("New chat started!")
             elif prompt := prompt.strip():
                 streamingWordWrapper = StreamingWordWrapper()
                 config.pagerContent = ""
 
                 try:
-                    completion = self.client.chat.completions.create(
+                    completion = getGroqClient().chat.completions.create(
                         model=config.groqApi_chat_model if config.useAdditionalChatModel else config.groqApi_main_model,
                         messages=self.messages,
                         temperature=self.temperature,
                         max_tokens=config.groqApi_max_tokens,
                         n=1,
                         stream=True,
+                        **config.groqApi_chat_model_additional_chat_options,
                     )
 
                     # Create a new thread for the streaming task
                     streaming_event = threading.Event()
                     self.streaming_thread = threading.Thread(target=streamingWordWrapper.streamOutputs, args=(streaming_event, completion, True))
                     # Start the streaming thread
                     self.streaming_thread.start()
```

### Comparing `freegenius-0.2.0/freegenius/gui/chatgui.py` & `freegenius-0.2.1/freegenius/gui/chatgui.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/gui/worker.py` & `freegenius-0.2.1/freegenius/gui/worker.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/icons/FreeGenius.ico` & `freegenius-0.2.1/freegenius/icons/FreeGenius.ico`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/icons/FreeGenius.png` & `freegenius-0.2.1/freegenius/icons/FreeGenius.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/icons/FreeGenius_original.png` & `freegenius-0.2.1/freegenius/icons/FreeGenius_original.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/icons/ai.png` & `freegenius-0.2.1/freegenius/icons/ai.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/icons/ai_original.png` & `freegenius-0.2.1/freegenius/icons/ai_original.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/llamacpp.py` & `freegenius-0.2.1/freegenius/llamacpp.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist` & `freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow` & `freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist` & `freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow` & `freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist` & `freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow` & `freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist` & `freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow` & `freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist` & `freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow` & `freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist` & `freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow` & `freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist` & `freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow` & `freegenius-0.2.1/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist` & `freegenius-0.2.1/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.2.1/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow` & `freegenius-0.2.1/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/main.py` & `freegenius-0.2.1/freegenius/main.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/ollamachat.py` & `freegenius-0.2.1/freegenius/ollamachat.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/palm2.py` & `freegenius-0.2.1/freegenius/palm2.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/plugins/000_check_ffmpeg.py` & `freegenius-0.2.1/freegenius/plugins/000_check_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/plugins/000_check_pyaudio.py` & `freegenius-0.2.1/freegenius/plugins/000_check_pyaudio.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/plugins/000_check_vlc.py` & `freegenius-0.2.1/freegenius/plugins/000_check_vlc.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/plugins/add calendar event.py` & `freegenius-0.2.1/freegenius/plugins/add calendar event.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/plugins/aliases.py` & `freegenius-0.2.1/freegenius/plugins/aliases.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/plugins/analyze audio.py` & `freegenius-0.2.1/freegenius/plugins/analyze audio.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/plugins/analyze files.py` & `freegenius-0.2.1/freegenius/plugins/analyze files.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/plugins/analyze images.py` & `freegenius-0.2.1/freegenius/plugins/analyze images.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/plugins/analyze web content.py` & `freegenius-0.2.1/freegenius/plugins/analyze web content.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/plugins/auto correct python code.py` & `freegenius-0.2.1/freegenius/plugins/auto correct python code.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     "name": "correct_python",
     "description": "Fix python code if both original code and traceback error are provided",
     "parameters": {
         "type": "object",
         "properties": {
             "code": {
                 "type": "string",
-                "description": "Improved version of python code that resolved the traceback error. Return the original code instead only if traceback shows an import error.",
+                "description": "Generate an improved version of python code that resolved the traceback error. Return the original code only if traceback shows an import error.",
             },
             "missing_module": {
                 "type": "string",
                 "description": """The module name identified in ModuleNotFoundError, if any. Return '' if there is no import error in the traceback.""",
             },
             "issue": {
                 "type": "string",
```

### Comparing `freegenius-0.2.0/freegenius/plugins/awesome prompts.py` & `freegenius-0.2.1/freegenius/plugins/awesome prompts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/plugins/character analysis.py` & `freegenius-0.2.1/freegenius/plugins/character analysis.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/plugins/chat.py` & `freegenius-0.2.1/freegenius/plugins/chat.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/plugins/contexts.py` & `freegenius-0.2.1/freegenius/plugins/contexts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/plugins/counselling.py` & `freegenius-0.2.1/freegenius/plugins/counselling.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/plugins/create ai assistants.py` & `freegenius-0.2.1/freegenius/plugins/create ai assistants.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/plugins/create images.py` & `freegenius-0.2.1/freegenius/plugins/create images.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/plugins/create maps.py` & `freegenius-0.2.1/freegenius/plugins/create maps.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/plugins/create qrcode.py` & `freegenius-0.2.1/freegenius/plugins/create qrcode.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/plugins/create statistical graphics.py` & `freegenius-0.2.1/freegenius/plugins/create statistical graphics.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/plugins/dates and times.py` & `freegenius-0.2.1/freegenius/plugins/dates and times.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/plugins/download youtube or web content.py` & `freegenius-0.2.1/freegenius/plugins/download youtube or web content.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/plugins/edit text.py` & `freegenius-0.2.1/freegenius/plugins/edit text.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/plugins/execute computing tasks.py` & `freegenius-0.2.1/freegenius/plugins/execute computing tasks.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/plugins/execute termux command.py` & `freegenius-0.2.1/freegenius/plugins/execute termux command.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/plugins/global finance.py` & `freegenius-0.2.1/freegenius/plugins/global finance.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/plugins/improve British English.py` & `freegenius-0.2.1/freegenius/plugins/improve British English.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/plugins/input suggestions.py` & `freegenius-0.2.1/freegenius/plugins/input suggestions.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/plugins/install python package.py` & `freegenius-0.2.1/freegenius/plugins/install python package.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/plugins/integrate google searches.py` & `freegenius-0.2.1/freegenius/plugins/integrate google searches.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/plugins/memory.py` & `freegenius-0.2.1/freegenius/plugins/memory.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/plugins/modify images.py` & `freegenius-0.2.1/freegenius/plugins/modify images.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/plugins/open web browser.py` & `freegenius-0.2.1/freegenius/plugins/open web browser.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/plugins/pronounce words.py` & `freegenius-0.2.1/freegenius/plugins/pronounce words.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/plugins/remove image background.py` & `freegenius-0.2.1/freegenius/plugins/remove image background.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/plugins/search chat records.py` & `freegenius-0.2.1/freegenius/plugins/search chat records.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/plugins/search financial data.py` & `freegenius-0.2.1/freegenius/plugins/search financial data.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "name": "search_finance",
     "description": f'''Search or analyze financial data. Use this function ONLY WHEN package yfinance is useful to resolve my request''',
     "parameters": {
         "type": "object",
         "properties": {
             "code": {
                 "type": "string",
-                "description": "Python code that integrates package yfinance to resolve my request. Integrate package matplotlib to visualize data, if applicable.",
+                "description": "Generate python code that integrates package yfinance to resolve my request. Integrate package matplotlib to visualize data, if applicable.",
             },
         },
         "required": ["code"],
     },
 }
 
 config.addFunctionCall(signature=functionSignature, method=search_finance)
```

### Comparing `freegenius-0.2.0/freegenius/plugins/search latest news.py` & `freegenius-0.2.1/freegenius/plugins/search latest news.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/plugins/search sqlite.py` & `freegenius-0.2.1/freegenius/plugins/search sqlite.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/plugins/search weather info.py` & `freegenius-0.2.1/freegenius/plugins/search weather info.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/plugins/send email.py` & `freegenius-0.2.1/freegenius/plugins/send email.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/plugins/send tweet.py` & `freegenius-0.2.1/freegenius/plugins/send tweet.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/plugins/send whatsapp messages.py` & `freegenius-0.2.1/freegenius/plugins/send whatsapp messages.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/plugins/simplified Chinese to traditional Chinese.py` & `freegenius-0.2.1/freegenius/plugins/simplified Chinese to traditional Chinese.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/rag.py` & `freegenius-0.2.1/freegenius/rag.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/requirements.txt` & `freegenius-0.2.1/freegenius/requirements.txt`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/servers.py` & `freegenius-0.2.1/freegenius/servers.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/systemtray.py` & `freegenius-0.2.1/freegenius/systemtray.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/utils/assistant.py` & `freegenius-0.2.1/freegenius/utils/assistant.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/utils/call_chatgpt.py` & `freegenius-0.2.1/freegenius/utils/call_chatgpt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/utils/call_gemini.py` & `freegenius-0.2.1/freegenius/utils/call_gemini.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/utils/call_groq.py` & `freegenius-0.2.1/freegenius/utils/call_groq.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 from freegenius import print1, print2, print3, selectTool, check_llm_errors, getGroqClient, toParameterSchema, extractPythonCode
 import re, traceback, pprint, copy, textwrap, json, pygments
 from pygments.lexers.python import PythonLexer
 from prompt_toolkit import print_formatted_text, HTML
 from prompt_toolkit.formatted_text import PygmentsTokens
 from prompt_toolkit import prompt
 from typing import Optional
+from pydantic import BaseModel
+
+class Screening(BaseModel):
+    answer: str
 
 class CallGroq:
 
     @staticmethod
     def riskAssessment(code):
         content = f"""You are a senior python engineer.
     Assess the risk level of damaging my device upon executing the python code that I will provide for you.
@@ -247,21 +251,20 @@
             stream=False,
             **config.groqApi_main_model_additional_chat_options,
         )
         responseDict = json.loads(completion.choices[0].message.tool_calls[0].function.arguments)
         return responseDict
 
     # Auto Function Call equivalence
-
     @staticmethod
     def runGeniusCall(messages: dict, noFunctionCall: bool = False):
         user_request = messages[-1]["content"]
         if config.intent_screening and config.tool_dependence > 0.0:
             # 1. Intent Screening
-            noFunctionCall = True if noFunctionCall else CallGroq.isChatOnly(messages=messages)
+            noFunctionCall = True if noFunctionCall else CallGroq.isChatOnly(user_request=user_request)
         if noFunctionCall or config.tool_dependence <= 0.0:
             return CallGroq.regularCall(messages)
         else:
             # 2. Tool Selection
             if config.selectedTool and config.selectedTool in config.toolFunctionSchemas:
                 tool_name = config.selectedTool
                 tool_schema = config.toolFunctionSchemas[tool_name]
@@ -340,41 +343,56 @@
                     # tool function executed without chat extension
                     config.currentMessages.append({"role": "assistant", "content": config.tempContent if config.tempContent else "Done!"})
                     config.tempContent = ""
                     config.conversationStarted = True
                     return None
 
     @staticmethod
-    def isChatOnly(messages: dict) -> bool:
+    def isChatOnly(user_request: str) -> bool:
         print2("```screening")
-        properties = {
-            "answer": {
-                "type": "string",
-                "description": """Evaluate my request to determine if you are able to resolve my request as a text-based AI:
+        try:
+            chat_completion = getGroqClient().chat.completions.create(
+                messages=[
+                    {
+                        "role": "system",
+                        "content": "You are a text-based language model that evaluate the nature of my request and tell me whether you can resolve it with full confidence. Output your answer in JSON. Your answer can only be either 'yes' or 'no'.\n"
+                        f" The JSON object must use the schema: {json.dumps(Screening.model_json_schema(), indent=2)}",
+                    },
+                    {
+                        "role": "user",
+                        "content": f"""Answer either 'yes' or 'no' in JSON format, in response to my request:
+<request>
+{user_request}
+</request>
+
+Question: Tell me honesly whether you are able to resolve the above request?
 - Answer 'no' if you are asked to execute a computing task or an online search.
 - Answer 'no' if you are asked for updates / news / real-time information.
 - Answer 'yes' if the request is a greeting or translation.
-- Answer 'yes' only if you have full information to give a direct response.""",
-                "enum": ['yes', 'no'],
-            },
-        }
-        schema = {
-            "name": "screen_user_request",
-            "description": f'''Estimate user request''',
-            "parameters": {
-                "type": "object",
-                "properties": properties,
-                "required": ["code"],
-            },
-        }
-        output = CallGroq.getDictionaryOutput(messages, schema=schema)
-        chatOnly = True if "yes" in str(output).lower() else False
-        print3(f"""Tool may {"not " if chatOnly else ""}be required.""")
+- Answer 'yes' only if you have full information to give a direct response.
+
+Remember, answer either 'yes' or 'no' in JSON, without extra information.""",
+                    },
+                ],
+                model=config.groqApi_main_model,
+                temperature=0,
+                max_tokens=20,
+                stream=False,
+                response_format={"type": "json_object"},
+            )
+            answer = Screening.model_validate_json(chat_completion.choices[0].message.content)
+        except:
+            # in case JSON output is failed
+            print3("Error: Unable to complete screening!")
+            answer = "no"
+        #print(answer) # check
+        answer = True if "yes" in str(answer).lower() else False
+        print3(f"""Comment: Tool may {"not " if answer else ""}be required.""")
         print2("```")
-        return chatOnly
+        return answer
 
     @staticmethod
     def extractToolParameters(schema: dict, userInput: str, ongoingMessages: list = [], temperature: Optional[float]=None, max_tokens: Optional[int]=None) -> dict:
         """
         Extract action parameters
         """
         name = schema["name"]
```

### Comparing `freegenius-0.2.0/freegenius/utils/call_llamacpp.py` & `freegenius-0.2.1/freegenius/utils/call_llamacpp.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/utils/call_llm.py` & `freegenius-0.2.1/freegenius/utils/call_llm.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/utils/call_ollama.py` & `freegenius-0.2.1/freegenius/utils/call_ollama.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/utils/config_essential.py` & `freegenius-0.2.1/freegenius/utils/config_essential.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/utils/config_tools.py` & `freegenius-0.2.1/freegenius/utils/config_tools.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/utils/download.py` & `freegenius-0.2.1/freegenius/utils/download.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/utils/get_path_prompt.py` & `freegenius-0.2.1/freegenius/utils/get_path_prompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/utils/ollama_models.py` & `freegenius-0.2.1/freegenius/utils/ollama_models.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/utils/promptValidator.py` & `freegenius-0.2.1/freegenius/utils/promptValidator.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/utils/prompt_multiline_shared_key_bindings.py` & `freegenius-0.2.1/freegenius/utils/prompt_multiline_shared_key_bindings.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/utils/prompt_shared_key_bindings.py` & `freegenius-0.2.1/freegenius/utils/prompt_shared_key_bindings.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/utils/prompts.py` & `freegenius-0.2.1/freegenius/utils/prompts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/utils/python_utils.py` & `freegenius-0.2.1/freegenius/utils/python_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/utils/shared_utils.py` & `freegenius-0.2.1/freegenius/utils/shared_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/utils/shortcuts.py` & `freegenius-0.2.1/freegenius/utils/shortcuts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/utils/single_prompt.py` & `freegenius-0.2.1/freegenius/utils/single_prompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/utils/streaming_word_wrapper.py` & `freegenius-0.2.1/freegenius/utils/streaming_word_wrapper.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/utils/sttLanguages.py` & `freegenius-0.2.1/freegenius/utils/sttLanguages.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/utils/terminal_mode_dialogs.py` & `freegenius-0.2.1/freegenius/utils/terminal_mode_dialogs.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/utils/terminal_system_command_prompt.py` & `freegenius-0.2.1/freegenius/utils/terminal_system_command_prompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/utils/text_utils.py` & `freegenius-0.2.1/freegenius/utils/text_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/utils/tool_plugins.py` & `freegenius-0.2.1/freegenius/utils/tool_plugins.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/utils/ttsLanguages.py` & `freegenius-0.2.1/freegenius/utils/ttsLanguages.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/utils/tts_utils.py` & `freegenius-0.2.1/freegenius/utils/tts_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius/utils/vlc_utils.py` & `freegenius-0.2.1/freegenius/utils/vlc_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius.egg-info/PKG-INFO` & `freegenius-0.2.1/freegenius.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freegenius
-Version: 0.2.0
+Version: 0.2.1
 Summary: FreeGenius AI, an advanced AI assistant that can talk and take multi-step actions. Supports numerous open-source LLMs via Llama.cpp or Ollama or Groq Cloud API, with optional integration with AutoGen agents, OpenAI API, Google Gemini Pro and unlimited plugins.
 Home-page: https://letmedoit.ai
 Author: Eliran Wong
 Author-email: support@letmedoit.ai
 License: GNU General Public License (GPL)
 Project-URL: Source, https://github.com/eliranwong/letmedoit
 Project-URL: Tracker, https://github.com/eliranwong/letmedoit/issues
```

### Comparing `freegenius-0.2.0/freegenius.egg-info/SOURCES.txt` & `freegenius-0.2.1/freegenius.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius.egg-info/entry_points.txt` & `freegenius-0.2.1/freegenius.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/freegenius.egg-info/requires.txt` & `freegenius-0.2.1/freegenius.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.0/setup.py` & `freegenius-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 # make sure config.py is empty
 open(os.path.join(package, "config.py"), "w").close()
 
 # https://packaging.python.org/en/latest/guides/distributing-packages-using-setuptools/
 setup(
     name=package,
-    version="0.2.00",
+    version="0.2.01",
     python_requires=">=3.8, <3.12",
     description=f"{appFullName}, an advanced AI assistant that can talk and take multi-step actions. Supports numerous open-source LLMs via Llama.cpp or Ollama or Groq Cloud API, with optional integration with AutoGen agents, OpenAI API, Google Gemini Pro and unlimited plugins.",
     long_description=long_description,
     author="Eliran Wong",
     author_email="support@letmedoit.ai",
     cmdclass={
         'install': PreInstallCommand,
```


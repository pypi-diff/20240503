# Comparing `tmp/sound_source_id-0.2.2.tar.gz` & `tmp/sound_source_id-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sound_source_id-0.2.2.tar", last modified: Thu May  2 20:34:48 2024, max compression
+gzip compressed data, was "sound_source_id-0.2.3.tar", last modified: Fri May  3 07:13:29 2024, max compression
```

## Comparing `sound_source_id-0.2.2.tar` & `sound_source_id-0.2.3.tar`

### file list

```diff
@@ -1,164 +1,164 @@
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:34:48.732953 sound_source_id-0.2.2/
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     1054 2024-02-05 09:35:07.000000 sound_source_id-0.2.2/.readthedocs.yaml
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)    35147 2010-06-04 09:15:48.000000 sound_source_id-0.2.2/COPYING.txt
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      408 2023-06-03 06:35:59.000000 sound_source_id-0.2.2/MANIFEST.in
--rw-r--r--   0 sam       (1000) extdrive  (1777)    41711 2024-05-02 20:34:48.732953 sound_source_id-0.2.2/PKG-INFO
--rw-rwsr--   0 sam       (1000) extdrive  (1777)       46 2023-02-28 10:13:11.000000 sound_source_id-0.2.2/README.md
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:34:46.812944 sound_source_id-0.2.2/icons/
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)    13103 2012-08-13 00:56:29.000000 sound_source_id-0.2.2/icons/audio-headphones.svgz
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)    16622 2011-11-01 10:05:06.000000 sound_source_id-0.2.2/icons/exit.svg
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)     7056 2012-08-13 00:59:09.000000 sound_source_id-0.2.2/icons/help-about.svgz
--rw-rwsr--   0 sam       (1000) extdrive  (1777)   679822 2015-11-04 09:40:24.000000 sound_source_id-0.2.2/icons/help-contents.svgz
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)   255671 2012-08-13 01:04:33.000000 sound_source_id-0.2.2/icons/help-contextual.svgz
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     7408 2023-06-02 05:19:07.000000 sound_source_id-0.2.2/icons/point-left.svg
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    21662 2023-06-06 21:15:49.000000 sound_source_id-0.2.2/icons/point-right.ico
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     4761 2023-06-02 05:19:10.000000 sound_source_id-0.2.2/icons/point-right.svg
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)    10662 2012-08-13 00:56:47.000000 sound_source_id-0.2.2/icons/preferences-other.svgz
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:34:46.812944 sound_source_id-0.2.2/make_noises/
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     2120 2023-05-31 05:23:34.000000 sound_source_id-0.2.2/make_noises/make_pink_noises.py
--rw-rwsr--   0 sam       (1000) extdrive  (1777)   171895 2020-04-12 10:56:23.000000 sound_source_id-0.2.2/make_noises/sndlib.py
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:34:46.912944 sound_source_id-0.2.2/prep-release/
--rw-rwxr--   0 sam       (1000) extdrive  (1777)        1 2024-05-02 20:34:16.000000 sound_source_id-0.2.2/prep-release/minor_minor_number.txt
--rwxrwsr-x   0 sam       (1000) extdrive  (1777)      178 2023-05-30 15:49:16.000000 sound_source_id-0.2.2/prep-release/mkupdate_pyqt5.sh
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)      547 2023-06-12 14:48:08.000000 sound_source_id-0.2.2/prep-release/mkupdate_pyqt6.sh
--rwxrwsr-x   0 sam       (1000) extdrive  (1777)      184 2023-06-08 21:48:18.000000 sound_source_id-0.2.2/prep-release/pypi_build.sh
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     3821 2024-05-02 15:25:43.000000 sound_source_id-0.2.2/prep-release/release.py
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)      478 2023-06-12 14:47:06.000000 sound_source_id-0.2.2/prep-release/sound_source_id.pro
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    22230 2023-06-19 21:36:07.000000 sound_source_id-0.2.2/prep-release/sound_source_id_el.ts
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    20770 2024-05-02 20:34:25.000000 sound_source_id-0.2.2/prep-release/sound_source_id_en_GB.ts
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    22230 2023-06-19 21:36:07.000000 sound_source_id-0.2.2/prep-release/sound_source_id_en_US.ts
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    20770 2024-05-02 20:34:25.000000 sound_source_id-0.2.2/prep-release/sound_source_id_es.ts
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    21950 2024-05-02 20:34:25.000000 sound_source_id-0.2.2/prep-release/sound_source_id_fr.ts
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    21015 2024-05-02 20:34:25.000000 sound_source_id-0.2.2/prep-release/sound_source_id_it.ts
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      937 2023-05-30 15:51:22.000000 sound_source_id-0.2.2/prep-release/switch_pyqt5.py
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      937 2023-05-30 15:51:35.000000 sound_source_id-0.2.2/prep-release/switch_pyqt6.py
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      217 2023-06-08 21:49:59.000000 sound_source_id-0.2.2/prep-release/win_installer_readme.md
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      146 2023-06-07 10:17:57.000000 sound_source_id-0.2.2/prep-release/win_launch_iss_compiler.bat
--rwxrwsr-x   0 sam       (1000) extdrive  (1777)      521 2023-06-07 17:49:12.000000 sound_source_id-0.2.2/prep-release/win_launch_iss_compiler.sh
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     3982 2024-05-02 20:34:16.000000 sound_source_id-0.2.2/prep-release/win_sound_source_id.iss
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      773 2023-06-12 15:13:58.000000 sound_source_id-0.2.2/prep-release/winbuild.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     1330 2024-05-02 20:34:16.000000 sound_source_id-0.2.2/pyproject.toml
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      821 2023-06-02 05:25:58.000000 sound_source_id-0.2.2/resources.qrc
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       38 2024-05-02 20:34:48.732953 sound_source_id-0.2.2/setup.cfg
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     1847 2024-05-02 20:34:16.000000 sound_source_id-0.2.2/setup_cx.py
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:34:46.920944 sound_source_id-0.2.2/sound_source_id/
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)        0 2008-10-28 02:30:54.000000 sound_source_id-0.2.2/sound_source_id/__init__.py
--rwxrwxr-x   0 sam       (1000) extdrive  (1777)    65651 2024-05-02 19:48:18.000000 sound_source_id-0.2.2/sound_source_id/__main__.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      107 2024-05-02 20:34:16.000000 sound_source_id-0.2.2/sound_source_id/_version_info.py
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    16558 2023-06-01 15:19:47.000000 sound_source_id-0.2.2/sound_source_id/audio_manager.py
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    19849 2023-06-11 08:20:40.000000 sound_source_id-0.2.2/sound_source_id/dialog_edit_preferences.py
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)    15831 2023-06-11 08:22:26.000000 sound_source_id-0.2.2/sound_source_id/dialog_edit_transducers.py
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:34:46.960944 sound_source_id-0.2.2/sound_source_id/doc/
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:34:46.996945 sound_source_id-0.2.2/sound_source_id/doc/Figures/
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    20275 2023-06-11 13:37:55.000000 sound_source_id-0.2.2/sound_source_id/doc/Figures/edit_transducers.png
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    17653 2023-02-23 14:52:34.000000 sound_source_id-0.2.2/sound_source_id/doc/Figures/sound_source_id_screenshot.png
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    10241 2023-03-14 14:49:17.000000 sound_source_id-0.2.2/sound_source_id/doc/Figures/stim_file.png
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      634 2023-02-23 15:00:48.000000 sound_source_id-0.2.2/sound_source_id/doc/Makefile
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:34:46.736943 sound_source_id-0.2.2/sound_source_id/doc/_build/
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:34:47.000944 sound_source_id-0.2.2/sound_source_id/doc/_build/html/
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      230 2024-05-02 20:34:32.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/.buildinfo
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:34:47.052945 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_images/
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    20275 2023-06-11 13:37:55.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_images/edit_transducers.png
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    17653 2023-02-23 14:52:34.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_images/sound_source_id_screenshot.png
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    10241 2023-03-14 14:49:17.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_images/stim_file.png
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:34:47.336946 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_sources/
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     2248 2023-06-11 14:05:30.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_sources/calibration.rst.txt
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     2670 2023-06-05 07:43:19.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_sources/experiment_setup.rst.txt
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      521 2023-06-11 14:02:33.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_sources/index.rst.txt
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     1499 2024-05-02 15:24:49.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_sources/installation.rst.txt
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      436 2023-06-03 06:22:36.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_sources/intro.rst.txt
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:34:47.680948 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_static/
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     4418 2023-03-29 08:31:27.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    14810 2024-05-02 20:34:32.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_static/basic.css
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     4472 2023-03-29 08:31:27.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_static/doctools.js
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      420 2024-05-02 20:34:32.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_static/documentation_options.js
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      286 2023-03-29 08:31:27.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_static/file.png
--rw-rwsr--   0 sam       (1000) extdrive  (1777)   289782 2022-08-29 08:27:59.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_static/jquery.js
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     4758 2024-05-02 20:34:32.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_static/language_data.js
--rw-rwsr--   0 sam       (1000) extdrive  (1777)       90 2023-03-29 08:31:27.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_static/minus.png
--rw-rwsr--   0 sam       (1000) extdrive  (1777)       90 2023-03-29 08:31:27.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_static/plus.png
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     4819 2024-05-02 20:34:32.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_static/pygments.css
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    18747 2023-03-29 08:31:27.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_static/searchtools.js
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     5097 2023-03-29 08:31:27.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_static/sphinx_highlight.js
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    68416 2022-06-02 12:39:04.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_static/underscore.js
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     7861 2024-05-02 20:34:31.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/calibration.html
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    11522 2024-05-02 20:34:31.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/experiment_setup.html
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     3976 2024-05-02 20:34:32.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/genindex.html
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     6000 2024-05-02 20:34:31.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/index.html
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     7384 2024-05-02 20:34:31.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/installation.html
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     6034 2024-05-02 20:34:32.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/intro.html
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      492 2024-05-02 20:34:32.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/objects.inv
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     4375 2024-05-02 20:34:32.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/search.html
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     5375 2024-05-02 20:34:32.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/searchindex.js
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:34:47.728948 sound_source_id-0.2.2/sound_source_id/doc/_build/latex/
--rw-rwxr--   0 sam       (1000) extdrive  (1777)   223206 2024-05-02 20:34:36.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/latex/sound_source_id.pdf
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     2248 2023-06-11 14:05:30.000000 sound_source_id-0.2.2/sound_source_id/doc/calibration.rst
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     2172 2024-05-02 20:34:16.000000 sound_source_id-0.2.2/sound_source_id/doc/conf.py
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     2670 2023-06-11 14:03:05.000000 sound_source_id-0.2.2/sound_source_id/doc/experiment_setup.rst
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      521 2023-06-11 14:02:33.000000 sound_source_id-0.2.2/sound_source_id/doc/index.rst
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     1499 2024-05-02 15:24:49.000000 sound_source_id-0.2.2/sound_source_id/doc/installation.rst
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      436 2023-06-03 06:22:36.000000 sound_source_id-0.2.2/sound_source_id/doc/intro.rst
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      795 2023-02-23 15:00:48.000000 sound_source_id-0.2.2/sound_source_id/doc/make.bat
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)      104 2023-02-23 14:58:04.000000 sound_source_id-0.2.2/sound_source_id/doc/mkdoc.sh
--rw-rwsr--   0 sam       (1000) extdrive  (1777)       18 2024-02-05 09:32:26.000000 sound_source_id-0.2.2/sound_source_id/doc/requirements.txt
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)     9341 2024-04-25 10:53:08.000000 sound_source_id-0.2.2/sound_source_id/global_parameters.py
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:34:48.124950 sound_source_id-0.2.2/sound_source_id/prm_files/
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:34:48.732953 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise1.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise10.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise11.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise12.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise13.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise14.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise15.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise16.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise17.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise18.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise19.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise2.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise20.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise21.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise22.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise23.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise24.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise25.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise26.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise27.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise28.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise29.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise3.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise30.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise4.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise5.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise6.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise7.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise8.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise9.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      389 2023-06-19 10:37:35.000000 sound_source_id-0.2.2/sound_source_id/prm_files/prm.txt
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      198 2023-06-19 10:37:35.000000 sound_source_id-0.2.2/sound_source_id/prm_files/prm_2_targets.txt
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      624 2023-06-19 10:37:35.000000 sound_source_id-0.2.2/sound_source_id/prm_files/prm_circle_36_targets.txt
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      421 2023-06-19 10:37:35.000000 sound_source_id-0.2.2/sound_source_id/prm_files/prm_virtual.txt
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      326 2023-06-19 10:37:35.000000 sound_source_id-0.2.2/sound_source_id/prm_files/prm_virtual_2_targets.txt
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      356 2023-06-19 10:37:35.000000 sound_source_id-0.2.2/sound_source_id/prm_files/prm_virtual_4_front_back.txt
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      427 2023-06-19 10:37:35.000000 sound_source_id-0.2.2/sound_source_id/prm_files/prm_virtual_circle_12_targets.txt
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      751 2023-06-19 10:37:35.000000 sound_source_id-0.2.2/sound_source_id/prm_files/prm_virtual_circle_36_targets.txt
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      646 2023-06-19 10:37:35.000000 sound_source_id-0.2.2/sound_source_id/prm_files/prm_virtual_circle_8_az_2_elev.txt
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     1257 2023-06-19 10:37:35.000000 sound_source_id-0.2.2/sound_source_id/prm_files/stim_list.csv
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      459 2023-06-19 10:37:35.000000 sound_source_id-0.2.2/sound_source_id/prm_files/stim_list_2_speak.csv
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      759 2023-06-19 10:37:35.000000 sound_source_id-0.2.2/sound_source_id/prm_files/stim_list_4_front_back.csv
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      710 2023-06-19 10:37:35.000000 sound_source_id-0.2.2/sound_source_id/prm_files/stim_list_8_az_2_elev.csv
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     1521 2023-06-19 10:37:35.000000 sound_source_id-0.2.2/sound_source_id/prm_files/stim_list_circle.csv
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      541 2023-06-19 10:37:35.000000 sound_source_id-0.2.2/sound_source_id/prm_files/stim_list_circle_12_tgs.csv
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      824 2024-05-02 20:34:12.000000 sound_source_id-0.2.2/sound_source_id/pyqtver.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)  2972123 2024-05-02 20:34:29.000000 sound_source_id-0.2.2/sound_source_id/qrc_resources.py
--rw-rwsr--   0 sam       (1000) extdrive  (1777)   175964 2023-05-04 21:44:23.000000 sound_source_id-0.2.2/sound_source_id/sndlib.py
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      991 2023-06-11 08:24:39.000000 sound_source_id-0.2.2/sound_source_id/utils.py
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    10419 2023-05-09 08:07:18.000000 sound_source_id-0.2.2/sound_source_id/wavpy.py
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     2953 2023-05-08 10:12:35.000000 sound_source_id-0.2.2/sound_source_id/wavpy_sndf.py
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:34:48.732953 sound_source_id-0.2.2/sound_source_id.egg-info/
--rw-r--r--   0 sam       (1000) extdrive  (1777)    41711 2024-05-02 20:34:46.000000 sound_source_id-0.2.2/sound_source_id.egg-info/PKG-INFO
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     6086 2024-05-02 20:34:46.000000 sound_source_id-0.2.2/sound_source_id.egg-info/SOURCES.txt
--rw-rwxr--   0 sam       (1000) extdrive  (1777)        1 2024-05-02 20:34:46.000000 sound_source_id-0.2.2/sound_source_id.egg-info/dependency_links.txt
--rw-rwxr--   0 sam       (1000) extdrive  (1777)       62 2024-05-02 20:34:46.000000 sound_source_id-0.2.2/sound_source_id.egg-info/entry_points.txt
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      101 2024-05-02 20:34:46.000000 sound_source_id-0.2.2/sound_source_id.egg-info/requires.txt
--rw-rwxr--   0 sam       (1000) extdrive  (1777)       16 2024-05-02 20:34:46.000000 sound_source_id-0.2.2/sound_source_id.egg-info/top_level.txt
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-03 07:13:29.515505 sound_source_id-0.2.3/
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     1054 2024-02-05 09:35:07.000000 sound_source_id-0.2.3/.readthedocs.yaml
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)    35147 2010-06-04 09:15:48.000000 sound_source_id-0.2.3/COPYING.txt
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      408 2023-06-03 06:35:59.000000 sound_source_id-0.2.3/MANIFEST.in
+-rw-r--r--   0 sam       (1000) extdrive  (1777)    41722 2024-05-03 07:13:29.515505 sound_source_id-0.2.3/PKG-INFO
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)       46 2023-02-28 10:13:11.000000 sound_source_id-0.2.3/README.md
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-03 07:13:26.595491 sound_source_id-0.2.3/icons/
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)    13103 2012-08-13 00:56:29.000000 sound_source_id-0.2.3/icons/audio-headphones.svgz
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)    16622 2011-11-01 10:05:06.000000 sound_source_id-0.2.3/icons/exit.svg
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)     7056 2012-08-13 00:59:09.000000 sound_source_id-0.2.3/icons/help-about.svgz
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)   679822 2015-11-04 09:40:24.000000 sound_source_id-0.2.3/icons/help-contents.svgz
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)   255671 2012-08-13 01:04:33.000000 sound_source_id-0.2.3/icons/help-contextual.svgz
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     7408 2023-06-02 05:19:07.000000 sound_source_id-0.2.3/icons/point-left.svg
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    21662 2023-06-06 21:15:49.000000 sound_source_id-0.2.3/icons/point-right.ico
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     4761 2023-06-02 05:19:10.000000 sound_source_id-0.2.3/icons/point-right.svg
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)    10662 2012-08-13 00:56:47.000000 sound_source_id-0.2.3/icons/preferences-other.svgz
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-03 07:13:26.595491 sound_source_id-0.2.3/make_noises/
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     2120 2023-05-31 05:23:34.000000 sound_source_id-0.2.3/make_noises/make_pink_noises.py
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)   171895 2020-04-12 10:56:23.000000 sound_source_id-0.2.3/make_noises/sndlib.py
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-03 07:13:26.775492 sound_source_id-0.2.3/prep-release/
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)        1 2024-05-03 07:12:53.000000 sound_source_id-0.2.3/prep-release/minor_minor_number.txt
+-rwxrwsr-x   0 sam       (1000) extdrive  (1777)      178 2023-05-30 15:49:16.000000 sound_source_id-0.2.3/prep-release/mkupdate_pyqt5.sh
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)      547 2023-06-12 14:48:08.000000 sound_source_id-0.2.3/prep-release/mkupdate_pyqt6.sh
+-rwxrwsr-x   0 sam       (1000) extdrive  (1777)      184 2023-06-08 21:48:18.000000 sound_source_id-0.2.3/prep-release/pypi_build.sh
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     3821 2024-05-02 15:25:43.000000 sound_source_id-0.2.3/prep-release/release.py
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)      478 2023-06-12 14:47:06.000000 sound_source_id-0.2.3/prep-release/sound_source_id.pro
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    19143 2024-05-03 07:10:38.000000 sound_source_id-0.2.3/prep-release/sound_source_id_el.ts
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    20770 2024-05-03 07:13:04.000000 sound_source_id-0.2.3/prep-release/sound_source_id_en_GB.ts
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    19143 2024-05-03 07:10:38.000000 sound_source_id-0.2.3/prep-release/sound_source_id_en_US.ts
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    20770 2024-05-03 07:13:04.000000 sound_source_id-0.2.3/prep-release/sound_source_id_es.ts
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    21950 2024-05-03 07:13:04.000000 sound_source_id-0.2.3/prep-release/sound_source_id_fr.ts
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    21015 2024-05-03 07:13:04.000000 sound_source_id-0.2.3/prep-release/sound_source_id_it.ts
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      937 2023-05-30 15:51:22.000000 sound_source_id-0.2.3/prep-release/switch_pyqt5.py
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      937 2023-05-30 15:51:35.000000 sound_source_id-0.2.3/prep-release/switch_pyqt6.py
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      217 2023-06-08 21:49:59.000000 sound_source_id-0.2.3/prep-release/win_installer_readme.md
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      146 2023-06-07 10:17:57.000000 sound_source_id-0.2.3/prep-release/win_launch_iss_compiler.bat
+-rwxrwsr-x   0 sam       (1000) extdrive  (1777)      521 2023-06-07 17:49:12.000000 sound_source_id-0.2.3/prep-release/win_launch_iss_compiler.sh
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     3982 2024-05-03 07:12:53.000000 sound_source_id-0.2.3/prep-release/win_sound_source_id.iss
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      773 2023-06-12 15:13:58.000000 sound_source_id-0.2.3/prep-release/winbuild.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     1341 2024-05-03 07:12:53.000000 sound_source_id-0.2.3/pyproject.toml
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      821 2023-06-02 05:25:58.000000 sound_source_id-0.2.3/resources.qrc
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       38 2024-05-03 07:13:29.515505 sound_source_id-0.2.3/setup.cfg
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     1847 2024-05-03 07:12:53.000000 sound_source_id-0.2.3/setup_cx.py
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-03 07:13:26.783492 sound_source_id-0.2.3/sound_source_id/
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)        0 2008-10-28 02:30:54.000000 sound_source_id-0.2.3/sound_source_id/__init__.py
+-rwxrwxr-x   0 sam       (1000) extdrive  (1777)    65651 2024-05-02 19:48:18.000000 sound_source_id-0.2.3/sound_source_id/__main__.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      107 2024-05-03 07:12:53.000000 sound_source_id-0.2.3/sound_source_id/_version_info.py
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    16558 2023-06-01 15:19:47.000000 sound_source_id-0.2.3/sound_source_id/audio_manager.py
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    19849 2023-06-11 08:20:40.000000 sound_source_id-0.2.3/sound_source_id/dialog_edit_preferences.py
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)    15831 2023-06-11 08:22:26.000000 sound_source_id-0.2.3/sound_source_id/dialog_edit_transducers.py
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-03 07:13:26.819492 sound_source_id-0.2.3/sound_source_id/doc/
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-03 07:13:26.883493 sound_source_id-0.2.3/sound_source_id/doc/Figures/
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    20275 2023-06-11 13:37:55.000000 sound_source_id-0.2.3/sound_source_id/doc/Figures/edit_transducers.png
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    17653 2023-02-23 14:52:34.000000 sound_source_id-0.2.3/sound_source_id/doc/Figures/sound_source_id_screenshot.png
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    10241 2023-03-14 14:49:17.000000 sound_source_id-0.2.3/sound_source_id/doc/Figures/stim_file.png
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      634 2023-02-23 15:00:48.000000 sound_source_id-0.2.3/sound_source_id/doc/Makefile
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-03 07:13:26.527491 sound_source_id-0.2.3/sound_source_id/doc/_build/
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-03 07:13:26.891492 sound_source_id-0.2.3/sound_source_id/doc/_build/html/
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      230 2024-05-03 07:13:08.000000 sound_source_id-0.2.3/sound_source_id/doc/_build/html/.buildinfo
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-03 07:13:26.943493 sound_source_id-0.2.3/sound_source_id/doc/_build/html/_images/
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    20275 2023-06-11 13:37:55.000000 sound_source_id-0.2.3/sound_source_id/doc/_build/html/_images/edit_transducers.png
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    17653 2023-02-23 14:52:34.000000 sound_source_id-0.2.3/sound_source_id/doc/_build/html/_images/sound_source_id_screenshot.png
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    10241 2023-03-14 14:49:17.000000 sound_source_id-0.2.3/sound_source_id/doc/_build/html/_images/stim_file.png
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-03 07:13:27.099494 sound_source_id-0.2.3/sound_source_id/doc/_build/html/_sources/
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     2248 2023-06-11 14:05:30.000000 sound_source_id-0.2.3/sound_source_id/doc/_build/html/_sources/calibration.rst.txt
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     2670 2023-06-05 07:43:19.000000 sound_source_id-0.2.3/sound_source_id/doc/_build/html/_sources/experiment_setup.rst.txt
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      521 2023-06-11 14:02:33.000000 sound_source_id-0.2.3/sound_source_id/doc/_build/html/_sources/index.rst.txt
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     1499 2024-05-02 15:24:49.000000 sound_source_id-0.2.3/sound_source_id/doc/_build/html/_sources/installation.rst.txt
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      436 2023-06-03 06:22:36.000000 sound_source_id-0.2.3/sound_source_id/doc/_build/html/_sources/intro.rst.txt
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-03 07:13:27.783497 sound_source_id-0.2.3/sound_source_id/doc/_build/html/_static/
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     4418 2023-03-29 08:31:27.000000 sound_source_id-0.2.3/sound_source_id/doc/_build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    14810 2024-05-03 07:13:08.000000 sound_source_id-0.2.3/sound_source_id/doc/_build/html/_static/basic.css
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     4472 2023-03-29 08:31:27.000000 sound_source_id-0.2.3/sound_source_id/doc/_build/html/_static/doctools.js
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      420 2024-05-03 07:13:08.000000 sound_source_id-0.2.3/sound_source_id/doc/_build/html/_static/documentation_options.js
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      286 2023-03-29 08:31:27.000000 sound_source_id-0.2.3/sound_source_id/doc/_build/html/_static/file.png
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)   289782 2022-08-29 08:27:59.000000 sound_source_id-0.2.3/sound_source_id/doc/_build/html/_static/jquery.js
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     4758 2024-05-03 07:13:08.000000 sound_source_id-0.2.3/sound_source_id/doc/_build/html/_static/language_data.js
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)       90 2023-03-29 08:31:27.000000 sound_source_id-0.2.3/sound_source_id/doc/_build/html/_static/minus.png
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)       90 2023-03-29 08:31:27.000000 sound_source_id-0.2.3/sound_source_id/doc/_build/html/_static/plus.png
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     4819 2024-05-03 07:13:08.000000 sound_source_id-0.2.3/sound_source_id/doc/_build/html/_static/pygments.css
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    18747 2023-03-29 08:31:27.000000 sound_source_id-0.2.3/sound_source_id/doc/_build/html/_static/searchtools.js
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     5097 2023-03-29 08:31:27.000000 sound_source_id-0.2.3/sound_source_id/doc/_build/html/_static/sphinx_highlight.js
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    68416 2022-06-02 12:39:04.000000 sound_source_id-0.2.3/sound_source_id/doc/_build/html/_static/underscore.js
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     7861 2024-05-03 07:13:08.000000 sound_source_id-0.2.3/sound_source_id/doc/_build/html/calibration.html
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    11522 2024-05-03 07:13:08.000000 sound_source_id-0.2.3/sound_source_id/doc/_build/html/experiment_setup.html
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     3976 2024-05-03 07:13:08.000000 sound_source_id-0.2.3/sound_source_id/doc/_build/html/genindex.html
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     6000 2024-05-03 07:13:08.000000 sound_source_id-0.2.3/sound_source_id/doc/_build/html/index.html
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     7384 2024-05-03 07:13:08.000000 sound_source_id-0.2.3/sound_source_id/doc/_build/html/installation.html
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     6034 2024-05-03 07:13:08.000000 sound_source_id-0.2.3/sound_source_id/doc/_build/html/intro.html
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      492 2024-05-03 07:13:08.000000 sound_source_id-0.2.3/sound_source_id/doc/_build/html/objects.inv
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     4375 2024-05-03 07:13:08.000000 sound_source_id-0.2.3/sound_source_id/doc/_build/html/search.html
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     5375 2024-05-03 07:13:08.000000 sound_source_id-0.2.3/sound_source_id/doc/_build/html/searchindex.js
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-03 07:13:27.823497 sound_source_id-0.2.3/sound_source_id/doc/_build/latex/
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)   223377 2024-05-03 07:13:14.000000 sound_source_id-0.2.3/sound_source_id/doc/_build/latex/sound_source_id.pdf
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     2248 2023-06-11 14:05:30.000000 sound_source_id-0.2.3/sound_source_id/doc/calibration.rst
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     2172 2024-05-03 07:12:53.000000 sound_source_id-0.2.3/sound_source_id/doc/conf.py
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     2670 2023-06-11 14:03:05.000000 sound_source_id-0.2.3/sound_source_id/doc/experiment_setup.rst
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      521 2023-06-11 14:02:33.000000 sound_source_id-0.2.3/sound_source_id/doc/index.rst
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     1499 2024-05-02 15:24:49.000000 sound_source_id-0.2.3/sound_source_id/doc/installation.rst
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      436 2023-06-03 06:22:36.000000 sound_source_id-0.2.3/sound_source_id/doc/intro.rst
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      795 2023-02-23 15:00:48.000000 sound_source_id-0.2.3/sound_source_id/doc/make.bat
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)      104 2023-02-23 14:58:04.000000 sound_source_id-0.2.3/sound_source_id/doc/mkdoc.sh
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)       18 2024-02-05 09:32:26.000000 sound_source_id-0.2.3/sound_source_id/doc/requirements.txt
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)     9341 2024-04-25 10:53:08.000000 sound_source_id-0.2.3/sound_source_id/global_parameters.py
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-03 07:13:28.111498 sound_source_id-0.2.3/sound_source_id/prm_files/
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-03 07:13:29.479505 sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise1.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise10.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise11.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise12.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise13.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise14.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise15.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise16.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise17.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise18.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise19.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise2.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise20.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise21.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise22.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise23.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise24.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise25.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise26.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise27.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise28.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise29.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise3.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise30.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise4.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise5.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise6.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise7.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise8.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise9.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      389 2023-06-19 10:37:35.000000 sound_source_id-0.2.3/sound_source_id/prm_files/prm.txt
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      198 2023-06-19 10:37:35.000000 sound_source_id-0.2.3/sound_source_id/prm_files/prm_2_targets.txt
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      624 2023-06-19 10:37:35.000000 sound_source_id-0.2.3/sound_source_id/prm_files/prm_circle_36_targets.txt
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      421 2023-06-19 10:37:35.000000 sound_source_id-0.2.3/sound_source_id/prm_files/prm_virtual.txt
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      326 2023-06-19 10:37:35.000000 sound_source_id-0.2.3/sound_source_id/prm_files/prm_virtual_2_targets.txt
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      356 2023-06-19 10:37:35.000000 sound_source_id-0.2.3/sound_source_id/prm_files/prm_virtual_4_front_back.txt
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      427 2023-06-19 10:37:35.000000 sound_source_id-0.2.3/sound_source_id/prm_files/prm_virtual_circle_12_targets.txt
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      751 2023-06-19 10:37:35.000000 sound_source_id-0.2.3/sound_source_id/prm_files/prm_virtual_circle_36_targets.txt
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      646 2023-06-19 10:37:35.000000 sound_source_id-0.2.3/sound_source_id/prm_files/prm_virtual_circle_8_az_2_elev.txt
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     1257 2023-06-19 10:37:35.000000 sound_source_id-0.2.3/sound_source_id/prm_files/stim_list.csv
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      459 2023-06-19 10:37:35.000000 sound_source_id-0.2.3/sound_source_id/prm_files/stim_list_2_speak.csv
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      759 2023-06-19 10:37:35.000000 sound_source_id-0.2.3/sound_source_id/prm_files/stim_list_4_front_back.csv
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      710 2023-06-19 10:37:35.000000 sound_source_id-0.2.3/sound_source_id/prm_files/stim_list_8_az_2_elev.csv
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     1521 2023-06-19 10:37:35.000000 sound_source_id-0.2.3/sound_source_id/prm_files/stim_list_circle.csv
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      541 2023-06-19 10:37:35.000000 sound_source_id-0.2.3/sound_source_id/prm_files/stim_list_circle_12_tgs.csv
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      824 2024-05-03 07:12:48.000000 sound_source_id-0.2.3/sound_source_id/pyqtver.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)  2972123 2024-05-03 07:13:06.000000 sound_source_id-0.2.3/sound_source_id/qrc_resources.py
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)   175964 2023-05-04 21:44:23.000000 sound_source_id-0.2.3/sound_source_id/sndlib.py
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      991 2023-06-11 08:24:39.000000 sound_source_id-0.2.3/sound_source_id/utils.py
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    10419 2023-05-09 08:07:18.000000 sound_source_id-0.2.3/sound_source_id/wavpy.py
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     2953 2023-05-08 10:12:35.000000 sound_source_id-0.2.3/sound_source_id/wavpy_sndf.py
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-03 07:13:29.515505 sound_source_id-0.2.3/sound_source_id.egg-info/
+-rw-r--r--   0 sam       (1000) extdrive  (1777)    41722 2024-05-03 07:13:26.000000 sound_source_id-0.2.3/sound_source_id.egg-info/PKG-INFO
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     6086 2024-05-03 07:13:26.000000 sound_source_id-0.2.3/sound_source_id.egg-info/SOURCES.txt
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)        1 2024-05-03 07:13:26.000000 sound_source_id-0.2.3/sound_source_id.egg-info/dependency_links.txt
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)       62 2024-05-03 07:13:26.000000 sound_source_id-0.2.3/sound_source_id.egg-info/entry_points.txt
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      112 2024-05-03 07:13:26.000000 sound_source_id-0.2.3/sound_source_id.egg-info/requires.txt
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)       16 2024-05-03 07:13:26.000000 sound_source_id-0.2.3/sound_source_id.egg-info/top_level.txt
```

### Comparing `sound_source_id-0.2.2/.readthedocs.yaml` & `sound_source_id-0.2.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/COPYING.txt` & `sound_source_id-0.2.3/COPYING.txt`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/PKG-INFO` & `sound_source_id-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sound_source_id
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python application for running sound localization experiments
 Author-email: Samuele Carcagno <sam.carcagno@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -695,10 +695,10 @@
 License-File: COPYING.txt
 Requires-Dist: matplotlib>=3.0.0
 Requires-Dist: numpy>=1.0.0
 Requires-Dist: pandas>=1.0.0
 Requires-Dist: PyAudio>=0.2.11
 Requires-Dist: PyQt6>=6.6.0
 Requires-Dist: scipy>=1.0.1
-Requires-Dist: pysofa>=0.1.1
+Requires-Dist: pysofaconventions>=0.1.1
 
 Python program for sound localization tests.
```

### Comparing `sound_source_id-0.2.2/icons/audio-headphones.svgz` & `sound_source_id-0.2.3/icons/audio-headphones.svgz`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/icons/exit.svg` & `sound_source_id-0.2.3/icons/exit.svg`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/icons/help-about.svgz` & `sound_source_id-0.2.3/icons/help-about.svgz`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/icons/help-contents.svgz` & `sound_source_id-0.2.3/icons/help-contents.svgz`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/icons/help-contextual.svgz` & `sound_source_id-0.2.3/icons/help-contextual.svgz`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/icons/point-left.svg` & `sound_source_id-0.2.3/icons/point-left.svg`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/icons/point-right.ico` & `sound_source_id-0.2.3/icons/point-right.ico`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/icons/point-right.svg` & `sound_source_id-0.2.3/icons/point-right.svg`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/icons/preferences-other.svgz` & `sound_source_id-0.2.3/icons/preferences-other.svgz`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/make_noises/make_pink_noises.py` & `sound_source_id-0.2.3/make_noises/make_pink_noises.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/make_noises/sndlib.py` & `sound_source_id-0.2.3/make_noises/sndlib.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/prep-release/mkupdate_pyqt6.sh` & `sound_source_id-0.2.3/prep-release/mkupdate_pyqt6.sh`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/prep-release/release.py` & `sound_source_id-0.2.3/prep-release/release.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/prep-release/sound_source_id_el.ts` & `sound_source_id-0.2.3/prep-release/sound_source_id_el.ts`

 * *Files 12% similar despite different names*

#### Comparing `sound_source_id-0.2.2/prep-release/sound_source_id_el.ts` & `sound_source_id-0.2.3/prep-release/sound_source_id_el.ts`

```diff
@@ -7,114 +7,29 @@
       <location filename="../sound_source_id/global_parameters.py" line="167"/>
       <source>custom</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>Preferences Window</name>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="91"/>
-      <source>System Settings</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="92"/>
-      <source>en</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="93"/>
-      <source>it</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="94"/>
-      <source>fr</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="95"/>
-      <source>es</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="96"/>
-      <source>el</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="99"/>
-      <source>US</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="100"/>
-      <source>GB</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="102"/>
-      <source>IT</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="103"/>
-      <source>CH</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="104"/>
-      <source>FR</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="105"/>
-      <source>CA</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="107"/>
-      <source>ES</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="108"/>
-      <source>BO</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="109"/>
-      <source>CL</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="111"/>
-      <source>GR</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="112"/>
-      <source>CY</source>
-      <translation type="unfinished"/>
-    </message>
   </context>
   <context>
     <name>applicationWindow</name>
     <message>
       <location filename="../sound_source_id/__main__.py" line="149"/>
       <source>sound_source_id</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/__main__.py" line="169"/>
       <source>&amp;File</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="272"/>
+      <location filename="../sound_source_id/__main__.py" line="277"/>
       <source>Load Parameters</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/__main__.py" line="173"/>
       <source>Load Parameters File</source>
       <translation type="unfinished"/>
@@ -151,80 +66,80 @@
     </message>
     <message>
       <location filename="../sound_source_id/__main__.py" line="202"/>
       <source>Manual (pdf)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="952"/>
+      <location filename="../sound_source_id/__main__.py" line="964"/>
       <source>About sound_source_id</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="411"/>
+      <location filename="../sound_source_id/__main__.py" line="423"/>
       <source>Loaded</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="411"/>
+      <location filename="../sound_source_id/__main__.py" line="423"/>
       <source>parameter file</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="424"/>
+      <location filename="../sound_source_id/__main__.py" line="436"/>
       <source>Choose parameters file to load</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="424"/>
+      <location filename="../sound_source_id/__main__.py" line="436"/>
       <source>All Files (*)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="536"/>
+      <location filename="../sound_source_id/__main__.py" line="548"/>
       <source>Choose file to write results</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="591"/>
+      <location filename="../sound_source_id/__main__.py" line="603"/>
       <source>Warning</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="569"/>
+      <location filename="../sound_source_id/__main__.py" line="581"/>
       <source>You need to select a file where to save the results to proceed</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="573"/>
+      <location filename="../sound_source_id/__main__.py" line="585"/>
       <source>Please, enter the listener's name:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="574"/>
+      <location filename="../sound_source_id/__main__.py" line="586"/>
       <source>Input Dialog:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="729"/>
+      <location filename="../sound_source_id/__main__.py" line="741"/>
       <source>Running</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="841"/>
+      <location filename="../sound_source_id/__main__.py" line="853"/>
       <source>Run Block</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="844"/>
+      <location filename="../sound_source_id/__main__.py" line="856"/>
       <source>Finished</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="952"/>
+      <location filename="../sound_source_id/__main__.py" line="964"/>
       <source>&lt;b&gt;sound_source_id - Python app for sound localization experiments&lt;/b&gt; &lt;br&gt;
                               - version: {0}; &lt;br&gt;
                               - build date: {1} &lt;br&gt;
                               &lt;p&gt; Copyright &amp;copy; 2022-2023 Samuele Carcagno. &lt;a href=&quot;mailto:sam.carcagno@gmail.com&quot;&gt;sam.carcagno@gmail.com&lt;/a&gt; 
                               All rights reserved. &lt;p&gt;
                               This program is free software: you can redistribute it and/or modify
                               it under the terms of the GNU General Public License as published by
@@ -238,93 +153,98 @@
                               &lt;p&gt;
                               You should have received a copy of the GNU General Public License
                               along with this program.  If not, see &lt;a href=&quot;http://www.gnu.org/licenses/&quot;&gt;http://www.gnu.org/licenses/&lt;/a&gt;
                               &lt;p&gt;Python {2} - {3} {4} compiled against Qt {5}, and running with Qt {6} on {7}</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="603"/>
+      <location filename="../sound_source_id/__main__.py" line="615"/>
       <source>Start</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="288"/>
+      <location filename="../sound_source_id/__main__.py" line="293"/>
       <source>Run Demo</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="248"/>
+      <location filename="../sound_source_id/__main__.py" line="253"/>
       <source>There was an issue loading your default parameter file. It is likely to contain an error. Please select a new default parameters file and restart the program.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="263"/>
+      <location filename="../sound_source_id/__main__.py" line="268"/>
       <source>The default parameters file could not be found. Please select a new default parameters file and restart the program.</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/__main__.py" line="210"/>
       <source>Show Play Buttons</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/__main__.py" line="191"/>
       <source>Transducers</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="225"/>
+      <location filename="../sound_source_id/__main__.py" line="230"/>
       <source>Listener:</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/__main__.py" line="214"/>
       <source>Show Response Buttons</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/__main__.py" line="219"/>
       <source>Show Response Lights</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="277"/>
+      <location filename="../sound_source_id/__main__.py" line="282"/>
       <source>Choose Results File</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="283"/>
+      <location filename="../sound_source_id/__main__.py" line="288"/>
       <source>Reset</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="591"/>
+      <location filename="../sound_source_id/__main__.py" line="603"/>
       <source>This will stop the current test. Are you sure you want to proceed?</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="560"/>
+      <location filename="../sound_source_id/__main__.py" line="572"/>
       <source>The results file cannot be changed while a test is running. Reset the test and then choose a new results file.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="536"/>
+      <location filename="../sound_source_id/__main__.py" line="548"/>
       <source>csv (*.csv)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="541"/>
+      <location filename="../sound_source_id/__main__.py" line="553"/>
       <source>File</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="541"/>
+      <location filename="../sound_source_id/__main__.py" line="553"/>
       <source>already exists. Do you want to overwrite it?</source>
       <translation type="unfinished"/>
     </message>
+    <message>
+      <location filename="../sound_source_id/__main__.py" line="224"/>
+      <source>Show Control Panel</source>
+      <translation type="unfinished"/>
+    </message>
   </context>
   <context>
     <name>preferencesDialog</name>
     <message>
       <location filename="../sound_source_id/dialog_edit_preferences.py" line="65"/>
       <source>Language (requires restart):</source>
       <translation type="unfinished"/>
@@ -414,45 +334,45 @@
       <source>Transducers:</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>responseLight</name>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="1134"/>
+      <location filename="../sound_source_id/__main__.py" line="1146"/>
       <source>Light &amp; Text</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="1110"/>
+      <location filename="../sound_source_id/__main__.py" line="1122"/>
       <source>Light</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="1146"/>
+      <location filename="../sound_source_id/__main__.py" line="1158"/>
       <source>Light &amp; Smiley</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="1168"/>
+      <location filename="../sound_source_id/__main__.py" line="1180"/>
       <source>Light &amp; Text &amp; Smiley</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="1116"/>
+      <location filename="../sound_source_id/__main__.py" line="1128"/>
       <source>Text</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="1153"/>
+      <location filename="../sound_source_id/__main__.py" line="1165"/>
       <source>Text &amp; Smiley</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="1127"/>
+      <location filename="../sound_source_id/__main__.py" line="1139"/>
       <source>Smiley</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>transducersDialog</name>
     <message>
```

### Comparing `sound_source_id-0.2.2/prep-release/sound_source_id_en_GB.ts` & `sound_source_id-0.2.3/prep-release/sound_source_id_en_GB.ts`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/prep-release/sound_source_id_en_US.ts` & `sound_source_id-0.2.3/prep-release/sound_source_id_en_US.ts`

 * *Files 12% similar despite different names*

#### Comparing `sound_source_id-0.2.2/prep-release/sound_source_id_en_US.ts` & `sound_source_id-0.2.3/prep-release/sound_source_id_en_US.ts`

```diff
@@ -7,114 +7,29 @@
       <location filename="../sound_source_id/global_parameters.py" line="167"/>
       <source>custom</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>Preferences Window</name>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="91"/>
-      <source>System Settings</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="92"/>
-      <source>en</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="93"/>
-      <source>it</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="94"/>
-      <source>fr</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="95"/>
-      <source>es</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="96"/>
-      <source>el</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="99"/>
-      <source>US</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="100"/>
-      <source>GB</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="102"/>
-      <source>IT</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="103"/>
-      <source>CH</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="104"/>
-      <source>FR</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="105"/>
-      <source>CA</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="107"/>
-      <source>ES</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="108"/>
-      <source>BO</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="109"/>
-      <source>CL</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="111"/>
-      <source>GR</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="112"/>
-      <source>CY</source>
-      <translation type="unfinished"/>
-    </message>
   </context>
   <context>
     <name>applicationWindow</name>
     <message>
       <location filename="../sound_source_id/__main__.py" line="149"/>
       <source>sound_source_id</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/__main__.py" line="169"/>
       <source>&amp;File</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="272"/>
+      <location filename="../sound_source_id/__main__.py" line="277"/>
       <source>Load Parameters</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/__main__.py" line="173"/>
       <source>Load Parameters File</source>
       <translation type="unfinished"/>
@@ -151,80 +66,80 @@
     </message>
     <message>
       <location filename="../sound_source_id/__main__.py" line="202"/>
       <source>Manual (pdf)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="952"/>
+      <location filename="../sound_source_id/__main__.py" line="964"/>
       <source>About sound_source_id</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="411"/>
+      <location filename="../sound_source_id/__main__.py" line="423"/>
       <source>Loaded</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="411"/>
+      <location filename="../sound_source_id/__main__.py" line="423"/>
       <source>parameter file</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="424"/>
+      <location filename="../sound_source_id/__main__.py" line="436"/>
       <source>Choose parameters file to load</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="424"/>
+      <location filename="../sound_source_id/__main__.py" line="436"/>
       <source>All Files (*)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="536"/>
+      <location filename="../sound_source_id/__main__.py" line="548"/>
       <source>Choose file to write results</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="591"/>
+      <location filename="../sound_source_id/__main__.py" line="603"/>
       <source>Warning</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="569"/>
+      <location filename="../sound_source_id/__main__.py" line="581"/>
       <source>You need to select a file where to save the results to proceed</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="573"/>
+      <location filename="../sound_source_id/__main__.py" line="585"/>
       <source>Please, enter the listener's name:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="574"/>
+      <location filename="../sound_source_id/__main__.py" line="586"/>
       <source>Input Dialog:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="729"/>
+      <location filename="../sound_source_id/__main__.py" line="741"/>
       <source>Running</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="841"/>
+      <location filename="../sound_source_id/__main__.py" line="853"/>
       <source>Run Block</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="844"/>
+      <location filename="../sound_source_id/__main__.py" line="856"/>
       <source>Finished</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="952"/>
+      <location filename="../sound_source_id/__main__.py" line="964"/>
       <source>&lt;b&gt;sound_source_id - Python app for sound localization experiments&lt;/b&gt; &lt;br&gt;
                               - version: {0}; &lt;br&gt;
                               - build date: {1} &lt;br&gt;
                               &lt;p&gt; Copyright &amp;copy; 2022-2023 Samuele Carcagno. &lt;a href=&quot;mailto:sam.carcagno@gmail.com&quot;&gt;sam.carcagno@gmail.com&lt;/a&gt; 
                               All rights reserved. &lt;p&gt;
                               This program is free software: you can redistribute it and/or modify
                               it under the terms of the GNU General Public License as published by
@@ -238,93 +153,98 @@
                               &lt;p&gt;
                               You should have received a copy of the GNU General Public License
                               along with this program.  If not, see &lt;a href=&quot;http://www.gnu.org/licenses/&quot;&gt;http://www.gnu.org/licenses/&lt;/a&gt;
                               &lt;p&gt;Python {2} - {3} {4} compiled against Qt {5}, and running with Qt {6} on {7}</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="603"/>
+      <location filename="../sound_source_id/__main__.py" line="615"/>
       <source>Start</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="288"/>
+      <location filename="../sound_source_id/__main__.py" line="293"/>
       <source>Run Demo</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="248"/>
+      <location filename="../sound_source_id/__main__.py" line="253"/>
       <source>There was an issue loading your default parameter file. It is likely to contain an error. Please select a new default parameters file and restart the program.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="263"/>
+      <location filename="../sound_source_id/__main__.py" line="268"/>
       <source>The default parameters file could not be found. Please select a new default parameters file and restart the program.</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/__main__.py" line="210"/>
       <source>Show Play Buttons</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/__main__.py" line="191"/>
       <source>Transducers</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="225"/>
+      <location filename="../sound_source_id/__main__.py" line="230"/>
       <source>Listener:</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/__main__.py" line="214"/>
       <source>Show Response Buttons</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/__main__.py" line="219"/>
       <source>Show Response Lights</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="277"/>
+      <location filename="../sound_source_id/__main__.py" line="282"/>
       <source>Choose Results File</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="283"/>
+      <location filename="../sound_source_id/__main__.py" line="288"/>
       <source>Reset</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="591"/>
+      <location filename="../sound_source_id/__main__.py" line="603"/>
       <source>This will stop the current test. Are you sure you want to proceed?</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="560"/>
+      <location filename="../sound_source_id/__main__.py" line="572"/>
       <source>The results file cannot be changed while a test is running. Reset the test and then choose a new results file.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="536"/>
+      <location filename="../sound_source_id/__main__.py" line="548"/>
       <source>csv (*.csv)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="541"/>
+      <location filename="../sound_source_id/__main__.py" line="553"/>
       <source>File</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="541"/>
+      <location filename="../sound_source_id/__main__.py" line="553"/>
       <source>already exists. Do you want to overwrite it?</source>
       <translation type="unfinished"/>
     </message>
+    <message>
+      <location filename="../sound_source_id/__main__.py" line="224"/>
+      <source>Show Control Panel</source>
+      <translation type="unfinished"/>
+    </message>
   </context>
   <context>
     <name>preferencesDialog</name>
     <message>
       <location filename="../sound_source_id/dialog_edit_preferences.py" line="65"/>
       <source>Language (requires restart):</source>
       <translation type="unfinished"/>
@@ -414,45 +334,45 @@
       <source>Transducers:</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>responseLight</name>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="1134"/>
+      <location filename="../sound_source_id/__main__.py" line="1146"/>
       <source>Light &amp; Text</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="1110"/>
+      <location filename="../sound_source_id/__main__.py" line="1122"/>
       <source>Light</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="1146"/>
+      <location filename="../sound_source_id/__main__.py" line="1158"/>
       <source>Light &amp; Smiley</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="1168"/>
+      <location filename="../sound_source_id/__main__.py" line="1180"/>
       <source>Light &amp; Text &amp; Smiley</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="1116"/>
+      <location filename="../sound_source_id/__main__.py" line="1128"/>
       <source>Text</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="1153"/>
+      <location filename="../sound_source_id/__main__.py" line="1165"/>
       <source>Text &amp; Smiley</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="1127"/>
+      <location filename="../sound_source_id/__main__.py" line="1139"/>
       <source>Smiley</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>transducersDialog</name>
     <message>
```

### Comparing `sound_source_id-0.2.2/prep-release/sound_source_id_es.ts` & `sound_source_id-0.2.3/prep-release/sound_source_id_es.ts`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/prep-release/sound_source_id_fr.ts` & `sound_source_id-0.2.3/prep-release/sound_source_id_fr.ts`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/prep-release/sound_source_id_it.ts` & `sound_source_id-0.2.3/prep-release/sound_source_id_it.ts`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/prep-release/switch_pyqt5.py` & `sound_source_id-0.2.3/prep-release/switch_pyqt5.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/prep-release/switch_pyqt6.py` & `sound_source_id-0.2.3/prep-release/switch_pyqt6.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/prep-release/win_launch_iss_compiler.sh` & `sound_source_id-0.2.3/prep-release/win_launch_iss_compiler.sh`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/prep-release/win_sound_source_id.iss` & `sound_source_id-0.2.3/prep-release/win_sound_source_id.iss`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ; Script generated by the Inno Setup Script Wizard.
 ; SEE THE DOCUMENTATION FOR DETAILS ON CREATING INNO SETUP SCRIPT FILES!
 
 #define MyAppName "sound_source_id"
-#define MyAppVersion "0.2.2"
+#define MyAppVersion "0.2.3"
 #define MyAppPublisher "Samuele Carcagno"
 #define MyAppURL "https://samcarcagno.altervista.org/sound_source_id/sound_source_id.html"
 #define MyAppExeName "sound_source_id.exe"
 
 [Setup]
 ; NOTE: The value of AppId uniquely identifies this application. Do not use the same AppId value in installers for other applications.
 ; (To generate a new GUID, click Tools | Generate GUID inside the IDE.)
```

### Comparing `sound_source_id-0.2.2/prep-release/winbuild.py` & `sound_source_id-0.2.3/prep-release/winbuild.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/pyproject.toml` & `sound_source_id-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sound_source_id"
-    version="0.2.2"
+    version="0.2.3"
 
 authors = [
   { name="Samuele Carcagno", email="sam.carcagno@gmail.com" },
 ]
 description = "Python application for running sound localization experiments"
 license = {file = "COPYING.txt"}
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = ["matplotlib (>=3.0.0)",
                 "numpy (>=1.0.0)",
 		"pandas (>=1.0.0)",
 		"PyAudio (>=0.2.11)",
 		"PyQt6 (>=6.6.0)",
 		"scipy (>=1.0.1)",
-		"pysofa (>=0.1.1)"
+		"pysofaconventions (>=0.1.1)"
 		]
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
     "Development Status :: 3 - Alpha",
```

### Comparing `sound_source_id-0.2.2/resources.qrc` & `sound_source_id-0.2.3/resources.qrc`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/setup_cx.py` & `sound_source_id-0.2.3/setup_cx.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,11 +39,11 @@
     Executable('sound_source_id\\__main__.py',
                base=base,
                target_name = 'sound_source_id',
                icon='icons/point-right.ico')
 ]
 
 setup(name='sound_source_id',
-    version="0.2.2",
+    version="0.2.3",
       description = '',
       options = {'build_exe': build_options},
       executables = executables)
```

### Comparing `sound_source_id-0.2.2/sound_source_id/__main__.py` & `sound_source_id-0.2.3/sound_source_id/__main__.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/audio_manager.py` & `sound_source_id-0.2.3/sound_source_id/audio_manager.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/dialog_edit_preferences.py` & `sound_source_id-0.2.3/sound_source_id/dialog_edit_preferences.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/dialog_edit_transducers.py` & `sound_source_id-0.2.3/sound_source_id/dialog_edit_transducers.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/doc/Figures/edit_transducers.png` & `sound_source_id-0.2.3/sound_source_id/doc/Figures/edit_transducers.png`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/doc/Figures/sound_source_id_screenshot.png` & `sound_source_id-0.2.3/sound_source_id/doc/Figures/sound_source_id_screenshot.png`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/doc/Figures/stim_file.png` & `sound_source_id-0.2.3/sound_source_id/doc/Figures/stim_file.png`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/doc/Makefile` & `sound_source_id-0.2.3/sound_source_id/doc/Makefile`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/doc/_build/html/_images/edit_transducers.png` & `sound_source_id-0.2.3/sound_source_id/doc/_build/html/_images/edit_transducers.png`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/doc/_build/html/_images/sound_source_id_screenshot.png` & `sound_source_id-0.2.3/sound_source_id/doc/_build/html/_images/sound_source_id_screenshot.png`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/doc/_build/html/_images/stim_file.png` & `sound_source_id-0.2.3/sound_source_id/doc/_build/html/_images/stim_file.png`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/doc/_build/html/_sources/calibration.rst.txt` & `sound_source_id-0.2.3/sound_source_id/doc/_build/html/_sources/calibration.rst.txt`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/doc/_build/html/_sources/experiment_setup.rst.txt` & `sound_source_id-0.2.3/sound_source_id/doc/_build/html/_sources/experiment_setup.rst.txt`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/doc/_build/html/_sources/index.rst.txt` & `sound_source_id-0.2.3/sound_source_id/doc/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/doc/_build/html/_sources/installation.rst.txt` & `sound_source_id-0.2.3/sound_source_id/doc/_build/html/_sources/installation.rst.txt`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/doc/_build/html/_static/_sphinx_javascript_frameworks_compat.js` & `sound_source_id-0.2.3/sound_source_id/doc/_build/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/doc/_build/html/_static/basic.css` & `sound_source_id-0.2.3/sound_source_id/doc/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/doc/_build/html/_static/doctools.js` & `sound_source_id-0.2.3/sound_source_id/doc/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/doc/_build/html/_static/jquery.js` & `sound_source_id-0.2.3/sound_source_id/doc/_build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/doc/_build/html/_static/language_data.js` & `sound_source_id-0.2.3/sound_source_id/doc/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/doc/_build/html/_static/pygments.css` & `sound_source_id-0.2.3/sound_source_id/doc/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/doc/_build/html/_static/searchtools.js` & `sound_source_id-0.2.3/sound_source_id/doc/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/doc/_build/html/_static/sphinx_highlight.js` & `sound_source_id-0.2.3/sound_source_id/doc/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/doc/_build/html/_static/underscore.js` & `sound_source_id-0.2.3/sound_source_id/doc/_build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/doc/_build/html/calibration.html` & `sound_source_id-0.2.3/sound_source_id/doc/_build/html/calibration.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Sound Level Calibration &mdash; sound_source_id 0.2.2 documentation</title>
+  <title>Sound Level Calibration &mdash; sound_source_id 0.2.3 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             sound_source_id
           </a>
               <div class="version">
-                0.2.2
+                0.2.3
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _s_o_u_n_d___s_o_u_r_c_e___i_d
-0.2.2
+0.2.3
 [q                   ]
 Contents:
     * _s_o_u_n_d___s_o_u_r_c_e___i_d
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _P_a_r_a_m_e_t_e_r_s_ _f_i_l_e
     * _S_t_i_m_u_l_a_t_i_o_n_ _f_i_l_e
     * _S_o_u_n_d_ _L_e_v_e_l_ _C_a_l_i_b_r_a_t_i_o_n
```

### Comparing `sound_source_id-0.2.2/sound_source_id/doc/_build/html/experiment_setup.html` & `sound_source_id-0.2.3/sound_source_id/doc/_build/html/experiment_setup.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Parameters file &mdash; sound_source_id 0.2.2 documentation</title>
+  <title>Parameters file &mdash; sound_source_id 0.2.3 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             sound_source_id
           </a>
               <div class="version">
-                0.2.2
+                0.2.3
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _s_o_u_n_d___s_o_u_r_c_e___i_d
-0.2.2
+0.2.3
 [q                   ]
 Contents:
     * _s_o_u_n_d___s_o_u_r_c_e___i_d
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _P_a_r_a_m_e_t_e_r_s_ _f_i_l_e
     * _S_t_i_m_u_l_a_t_i_o_n_ _f_i_l_e
     * _S_o_u_n_d_ _L_e_v_e_l_ _C_a_l_i_b_r_a_t_i_o_n
```

### Comparing `sound_source_id-0.2.2/sound_source_id/doc/_build/html/genindex.html` & `sound_source_id-0.2.3/sound_source_id/doc/_build/html/genindex.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Index &mdash; sound_source_id 0.2.2 documentation</title>
+  <title>Index &mdash; sound_source_id 0.2.3 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -26,15 +26,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             sound_source_id
           </a>
               <div class="version">
-                0.2.2
+                0.2.3
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _s_o_u_n_d___s_o_u_r_c_e___i_d
-0.2.2
+0.2.3
 [q                   ]
 Contents:
     * _s_o_u_n_d___s_o_u_r_c_e___i_d
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _P_a_r_a_m_e_t_e_r_s_ _f_i_l_e
     * _S_t_i_m_u_l_a_t_i_o_n_ _f_i_l_e
     * _S_o_u_n_d_ _L_e_v_e_l_ _C_a_l_i_b_r_a_t_i_o_n
```

### Comparing `sound_source_id-0.2.2/sound_source_id/doc/_build/html/index.html` & `sound_source_id-0.2.3/sound_source_id/doc/_build/html/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Welcome to sound_source_id’s documentation! &mdash; sound_source_id 0.2.2 documentation</title>
+  <title>Welcome to sound_source_id’s documentation! &mdash; sound_source_id 0.2.3 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -28,15 +28,15 @@
 
           
           
           <a href="#" class="icon icon-home">
             sound_source_id
           </a>
               <div class="version">
-                0.2.2
+                0.2.3
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _s_o_u_n_d___s_o_u_r_c_e___i_d
-0.2.2
+0.2.3
 [q                   ]
 Contents:
     * _s_o_u_n_d___s_o_u_r_c_e___i_d
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _P_a_r_a_m_e_t_e_r_s_ _f_i_l_e
     * _S_t_i_m_u_l_a_t_i_o_n_ _f_i_l_e
     * _S_o_u_n_d_ _L_e_v_e_l_ _C_a_l_i_b_r_a_t_i_o_n
```

### Comparing `sound_source_id-0.2.2/sound_source_id/doc/_build/html/installation.html` & `sound_source_id-0.2.3/sound_source_id/doc/_build/html/installation.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Installation &mdash; sound_source_id 0.2.2 documentation</title>
+  <title>Installation &mdash; sound_source_id 0.2.3 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             sound_source_id
           </a>
               <div class="version">
-                0.2.2
+                0.2.3
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _s_o_u_n_d___s_o_u_r_c_e___i_d
-0.2.2
+0.2.3
 [q                   ]
 Contents:
     * _s_o_u_n_d___s_o_u_r_c_e___i_d
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _P_a_r_a_m_e_t_e_r_s_ _f_i_l_e
     * _S_t_i_m_u_l_a_t_i_o_n_ _f_i_l_e
     * _S_o_u_n_d_ _L_e_v_e_l_ _C_a_l_i_b_r_a_t_i_o_n
```

### Comparing `sound_source_id-0.2.2/sound_source_id/doc/_build/html/intro.html` & `sound_source_id-0.2.3/sound_source_id/doc/_build/html/intro.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>sound_source_id &mdash; sound_source_id 0.2.2 documentation</title>
+  <title>sound_source_id &mdash; sound_source_id 0.2.3 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             sound_source_id
           </a>
               <div class="version">
-                0.2.2
+                0.2.3
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _s_o_u_n_d___s_o_u_r_c_e___i_d
-0.2.2
+0.2.3
 [q                   ]
 Contents:
     * _s_o_u_n_d___s_o_u_r_c_e___i_d
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _P_a_r_a_m_e_t_e_r_s_ _f_i_l_e
     * _S_t_i_m_u_l_a_t_i_o_n_ _f_i_l_e
     * _S_o_u_n_d_ _L_e_v_e_l_ _C_a_l_i_b_r_a_t_i_o_n
```

### Comparing `sound_source_id-0.2.2/sound_source_id/doc/_build/html/search.html` & `sound_source_id-0.2.3/sound_source_id/doc/_build/html/search.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Search &mdash; sound_source_id 0.2.2 documentation</title>
+  <title>Search &mdash; sound_source_id 0.2.3 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
     
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             sound_source_id
           </a>
               <div class="version">
-                0.2.2
+                0.2.3
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="#" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _s_o_u_n_d___s_o_u_r_c_e___i_d
-0.2.2
+0.2.3
 [q                   ]
 Contents:
     * _s_o_u_n_d___s_o_u_r_c_e___i_d
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _P_a_r_a_m_e_t_e_r_s_ _f_i_l_e
     * _S_t_i_m_u_l_a_t_i_o_n_ _f_i_l_e
     * _S_o_u_n_d_ _L_e_v_e_l_ _C_a_l_i_b_r_a_t_i_o_n
```

### Comparing `sound_source_id-0.2.2/sound_source_id/doc/_build/html/searchindex.js` & `sound_source_id-0.2.3/sound_source_id/doc/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/doc/_build/latex/sound_source_id.pdf` & `sound_source_id-0.2.3/sound_source_id/doc/_build/latex/sound_source_id.pdf`

 * *Files 8% similar despite different names*

#### Comparing `sound_source_id-0.2.2/sound_source_id/doc/_build/latex/sound_source_id.pdf` & `sound_source_id-0.2.3/sound_source_id/doc/_build/latex/sound_source_id.pdf`

 * *Document info*

```diff
@@ -1,10 +1,10 @@
 Author: 'Samuele Carcagno'
-CreationDate: "D:20240502223433+02'00'"
+CreationDate: "D:20240503091310+02'00'"
 Creator: 'LaTeX with hyperref'
 Keywords: ''
-ModDate: "D:20240502223433+02'00'"
+ModDate: "D:20240503091310+02'00'"
 PTEX.Fullbanner: 'This is pdfTeX, Version 3.141592653-2.6-1.40.24 (TeX Live 2022/Debian) kpathsea version 6.3.4'
 Producer: 'pdfTeX-1.40.24'
 Subject: ''
 Title: 'sound_source_id'
 Trapped: '/False'
```

#### pdftotext {} -

```diff
@@ -1,13 +1,13 @@
 sound_source_id
-Release 0.2.2
+Release 0.2.3
 
 Samuele Carcagno
 
-May 02, 2024
+May 03, 2024
 
 CONTENTS:
 
 1
 
 sound_source_id
 
@@ -56,15 +56,15 @@
 sound_source_id is program for testing static sound localization. The interface is shown in Figure Screenshot of the
 sound_source_id interface..
 
 Fig. 1: Screenshot of the sound_source_id interface.
 
 1
 
-sound_source_id, Release 0.2.2
+sound_source_id, Release 0.2.3
 
 2
 
 Chapter 1. sound_source_id
 
 CHAPTER
 
@@ -94,15 +94,15 @@
 on how you want sound to be played, you need to install:
 • pyalsaaudio https://pypi.org/project/pyalsaaudio/
 or SoX:
 • https://sox.sourceforge.net/
 
 3
 
-sound_source_id, Release 0.2.2
+sound_source_id, Release 0.2.3
 
 4
 
 Chapter 2. Installation
 
 CHAPTER
 
@@ -131,15 +131,15 @@
 • stim_list_file: the path (absolute or relative) to the file containing the stimulation list (see below)
 • randomize: if true the stim_list_file will be shuffled before each block repetition
 • demo_stim: the path to the WAV file to be used for the demo
 • demo_stim_lev: the sound level (in dB SPL) to be used for the demo
 
 5
 
-sound_source_id, Release 0.2.2
+sound_source_id, Release 0.2.3
 
 6
 
 Chapter 3. Parameters file
 
 CHAPTER
 
@@ -160,15 +160,15 @@
 has been correctly calibrated)
 • roving: a level rove, actual sound level will be euqual to the base level plus a value drawn from a random uniform
 distribution between +/- the roving level
 • feedback: if true, feedback will be given to the listener at the end of each trial
 
 7
 
-sound_source_id, Release 0.2.2
+sound_source_id, Release 0.2.3
 
 8
 
 Chapter 4. Stimulation file
 
 CHAPTER
 
@@ -194,15 +194,15 @@
 We can measure the RMS level of the WAV file with the noise used for calibration, let’s call it 𝑟𝑚𝑠𝑛𝑜𝑖𝑠𝑒. A full
 amplitude sinusoid has a root-mean-square amplitude of 1/sqrt(2) = 0.707. The difference in dB between the level of
 a sinusoid at max amplitude and our calibration noise will be equal to:
 𝑑𝑏𝑑𝑖𝑓 𝑓 = 20 * 𝑙𝑜𝑔10((1/𝑠𝑞𝑟𝑡(2))/𝑟𝑚𝑠𝑛𝑜𝑖𝑠𝑒)
 
 9
 
-sound_source_id, Release 0.2.2
+sound_source_id, Release 0.2.3
 
 Therefore, if our calibration noise had a level (measured with the SPL meter) or 𝑥 dB SPL, a sinusoid at max amplitude
 would have a level of:
 𝑚𝑎𝑥𝑙𝑒𝑣 = 𝑥 + 𝑑𝑏𝑑𝑖𝑓 𝑓
 this is the value that you need to enter in the Max Level field of the transducers calibration table for the loudspeakers
 in question.
```

### Comparing `sound_source_id-0.2.2/sound_source_id/doc/calibration.rst` & `sound_source_id-0.2.3/sound_source_id/doc/calibration.rst`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/doc/conf.py` & `sound_source_id-0.2.3/sound_source_id/doc/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 author = 'Samuele Carcagno'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = "0.2.2"
+version = "0.2.3"
 # The full version, including alpha/beta/rc tags.
-release = "0.2.2"
+release = "0.2.3"
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
```

### Comparing `sound_source_id-0.2.2/sound_source_id/doc/experiment_setup.rst` & `sound_source_id-0.2.3/sound_source_id/doc/experiment_setup.rst`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/doc/index.rst` & `sound_source_id-0.2.3/sound_source_id/doc/index.rst`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/doc/installation.rst` & `sound_source_id-0.2.3/sound_source_id/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/doc/make.bat` & `sound_source_id-0.2.3/sound_source_id/doc/make.bat`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/global_parameters.py` & `sound_source_id-0.2.3/sound_source_id/global_parameters.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise1.wav` & `sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise1.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise10.wav` & `sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise10.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise11.wav` & `sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise11.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise12.wav` & `sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise12.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise13.wav` & `sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise13.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise14.wav` & `sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise14.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise15.wav` & `sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise15.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise16.wav` & `sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise16.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise17.wav` & `sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise17.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise18.wav` & `sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise18.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise19.wav` & `sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise19.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise2.wav` & `sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise2.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise20.wav` & `sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise20.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise21.wav` & `sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise21.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise22.wav` & `sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise22.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise23.wav` & `sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise23.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise24.wav` & `sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise24.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise25.wav` & `sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise25.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise26.wav` & `sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise26.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise27.wav` & `sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise27.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise28.wav` & `sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise28.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise29.wav` & `sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise29.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise3.wav` & `sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise3.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise30.wav` & `sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise30.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise4.wav` & `sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise4.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise5.wav` & `sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise5.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise6.wav` & `sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise6.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise7.wav` & `sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise7.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise8.wav` & `sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise8.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise9.wav` & `sound_source_id-0.2.3/sound_source_id/prm_files/pink_noises/noise9.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/prm_files/prm_circle_36_targets.txt` & `sound_source_id-0.2.3/sound_source_id/prm_files/prm_circle_36_targets.txt`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/prm_files/prm_virtual_circle_36_targets.txt` & `sound_source_id-0.2.3/sound_source_id/prm_files/prm_virtual_circle_36_targets.txt`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/prm_files/prm_virtual_circle_8_az_2_elev.txt` & `sound_source_id-0.2.3/sound_source_id/prm_files/prm_virtual_circle_8_az_2_elev.txt`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/prm_files/stim_list.csv` & `sound_source_id-0.2.3/sound_source_id/prm_files/stim_list.csv`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/prm_files/stim_list_4_front_back.csv` & `sound_source_id-0.2.3/sound_source_id/prm_files/stim_list_4_front_back.csv`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/prm_files/stim_list_8_az_2_elev.csv` & `sound_source_id-0.2.3/sound_source_id/prm_files/stim_list_8_az_2_elev.csv`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/prm_files/stim_list_circle.csv` & `sound_source_id-0.2.3/sound_source_id/prm_files/stim_list_circle.csv`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/prm_files/stim_list_circle_12_tgs.csv` & `sound_source_id-0.2.3/sound_source_id/prm_files/stim_list_circle_12_tgs.csv`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/pyqtver.py` & `sound_source_id-0.2.3/sound_source_id/pyqtver.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/qrc_resources.py` & `sound_source_id-0.2.3/sound_source_id/qrc_resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -61268,25 +61268,25 @@
 \x00\x00\x00\xa8\x00\x00\x00\x00\x00\x01\x00\x0a\xa9\x04\
 \x00\x00\x019\x1d\x82\xc4\xe8\
 \x00\x00\x00\x1a\x00\x02\x00\x00\x00\x06\x00\x00\x00\x0a\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00\xe6\x00\x00\x00\x00\x00\x01\x00\x0e\xabS\
 \x00\x00\x019\x1d{\xa8\x98\
 \x00\x00\x01\xa4\x00\x00\x00\x00\x00\x01\x00\x0e\xdcW\
-\x00\x00\x01\x8f;\x04\x02|\
+\x00\x00\x01\x8f=L\xac\xfb\
 \x00\x00\x02\x0a\x00\x00\x00\x00\x00\x01\x00\x0e\xdc\x7f\
-\x00\x00\x01\x8f;\x04\x02x\
+\x00\x00\x01\x8f=L\xac\xfb\
 \x00\x00\x01t\x00\x00\x00\x00\x00\x01\x00\x0e\xdcC\
-\x00\x00\x01\x8f;\x04\x02|\
+\x00\x00\x01\x8f=L\xac\xfb\
 \x00\x00\x01\x0e\x00\x00\x00\x00\x00\x01\x00\x0e\xd4\xfd\
-\x00\x00\x01\x8f;\x04\x02x\
+\x00\x00\x01\x8f=L\xac\xf7\
 \x00\x00\x01\xd4\x00\x00\x00\x00\x00\x01\x00\x0e\xdck\
-\x00\x00\x01\x8f;\x04\x02|\
+\x00\x00\x01\x8f=L\xac\xff\
 \x00\x00\x01>\x00\x00\x00\x00\x00\x01\x00\x0e\xdc/\
-\x00\x00\x01\x8f;\x04\x02|\
+\x00\x00\x01\x8f=L\xac\xff\
 "
 
 def qInitResources():
     QtCore.qRegisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
 
 def qCleanupResources():
     QtCore.qUnregisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
```

### Comparing `sound_source_id-0.2.2/sound_source_id/sndlib.py` & `sound_source_id-0.2.3/sound_source_id/sndlib.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/utils.py` & `sound_source_id-0.2.3/sound_source_id/utils.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/wavpy.py` & `sound_source_id-0.2.3/sound_source_id/wavpy.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id/wavpy_sndf.py` & `sound_source_id-0.2.3/sound_source_id/wavpy_sndf.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.2/sound_source_id.egg-info/PKG-INFO` & `sound_source_id-0.2.3/sound_source_id.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sound_source_id
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python application for running sound localization experiments
 Author-email: Samuele Carcagno <sam.carcagno@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -695,10 +695,10 @@
 License-File: COPYING.txt
 Requires-Dist: matplotlib>=3.0.0
 Requires-Dist: numpy>=1.0.0
 Requires-Dist: pandas>=1.0.0
 Requires-Dist: PyAudio>=0.2.11
 Requires-Dist: PyQt6>=6.6.0
 Requires-Dist: scipy>=1.0.1
-Requires-Dist: pysofa>=0.1.1
+Requires-Dist: pysofaconventions>=0.1.1
 
 Python program for sound localization tests.
```

### Comparing `sound_source_id-0.2.2/sound_source_id.egg-info/SOURCES.txt` & `sound_source_id-0.2.3/sound_source_id.egg-info/SOURCES.txt`

 * *Files identical despite different names*


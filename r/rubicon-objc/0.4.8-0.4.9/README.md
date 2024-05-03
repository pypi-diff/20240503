# Comparing `tmp/rubicon-objc-0.4.8.tar.gz` & `tmp/rubicon_objc-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubicon-objc-0.4.8.tar", last modified: Wed Apr  3 05:07:38 2024, max compression
+gzip compressed data, was "rubicon_objc-0.4.9.tar", last modified: Fri May  3 01:42:48 2024, max compression
```

## Comparing `rubicon-objc-0.4.8.tar` & `rubicon_objc-0.4.9.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-03 05:07:38.894561 rubicon-objc-0.4.8/
--rw-r--r--   0 runner     (501) staff       (20)       71 2024-04-03 05:06:50.000000 rubicon-objc-0.4.8/.git-blame-ignore-revs
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-03 05:07:38.844670 rubicon-objc-0.4.8/.github/
--rw-r--r--   0 runner     (501) staff       (20)      377 2024-04-03 05:06:50.000000 rubicon-objc-0.4.8/.github/dependabot.yml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-03 05:07:38.848033 rubicon-objc-0.4.8/.github/workflows/
--rw-r--r--   0 runner     (501) staff       (20)     2386 2024-04-03 05:06:50.000000 rubicon-objc-0.4.8/.github/workflows/ci.yml
--rw-r--r--   0 runner     (501) staff       (20)      281 2024-04-03 05:06:50.000000 rubicon-objc-0.4.8/.github/workflows/config-file-deps-bump.yml
--rw-r--r--   0 runner     (501) staff       (20)      230 2024-04-03 05:06:50.000000 rubicon-objc-0.4.8/.github/workflows/dependabot-changenote.yml
--rw-r--r--   0 runner     (501) staff       (20)      257 2024-04-03 05:06:50.000000 rubicon-objc-0.4.8/.github/workflows/pre-commit-update.yml
--rw-r--r--   0 runner     (501) staff       (20)      740 2024-04-03 05:06:50.000000 rubicon-objc-0.4.8/.github/workflows/publish.yml
--rw-r--r--   0 runner     (501) staff       (20)     2117 2024-04-03 05:06:50.000000 rubicon-objc-0.4.8/.github/workflows/release.yml
--rw-r--r--   0 runner     (501) staff       (20)      158 2024-04-03 05:06:50.000000 rubicon-objc-0.4.8/.gitignore
--rw-r--r--   0 runner     (501) staff       (20)      855 2024-04-03 05:06:50.000000 rubicon-objc-0.4.8/.pre-commit-config.yaml
--rw-r--r--   0 runner     (501) staff       (20)      707 2024-04-03 05:06:50.000000 rubicon-objc-0.4.8/.readthedocs.yml
--rw-r--r--   0 runner     (501) staff       (20)      140 2024-04-03 05:06:50.000000 rubicon-objc-0.4.8/CHANGELOG.rst
--rw-r--r--   0 runner     (501) staff       (20)      182 2024-04-03 05:06:50.000000 rubicon-objc-0.4.8/CONTRIBUTING.md
--rw-r--r--   0 runner     (501) staff       (20)     3278 2024-04-03 05:06:50.000000 rubicon-objc-0.4.8/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)     5714 2024-04-03 05:07:38.893824 rubicon-objc-0.4.8/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     3411 2024-04-03 05:06:50.000000 rubicon-objc-0.4.8/README.rst
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-03 05:07:38.849081 rubicon-objc-0.4.8/changes/
--rw-r--r--   0 runner     (501) staff       (20)       12 2024-04-03 05:06:51.000000 rubicon-objc-0.4.8/changes/.gitignore
--rw-r--r--   0 runner     (501) staff       (20)      792 2024-04-03 05:06:51.000000 rubicon-objc-0.4.8/changes/template.rst
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-03 05:07:38.851839 rubicon-objc-0.4.8/docs/
--rw-r--r--   0 runner     (501) staff       (20)      728 2024-04-03 05:06:51.000000 rubicon-objc-0.4.8/docs/Makefile
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-03 05:07:38.835752 rubicon-objc-0.4.8/docs/_mocked_modules/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-03 05:07:38.852902 rubicon-objc-0.4.8/docs/_mocked_modules/ctypes/
--rw-r--r--   0 runner     (501) staff       (20)    10469 2024-04-03 05:06:51.000000 rubicon-objc-0.4.8/docs/_mocked_modules/ctypes/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      127 2024-04-03 05:06:51.000000 rubicon-objc-0.4.8/docs/_mocked_modules/ctypes/util.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-03 05:07:38.836190 rubicon-objc-0.4.8/docs/_static/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-03 05:07:38.853464 rubicon-objc-0.4.8/docs/_static/images/
--rw-r--r--   0 runner     (501) staff       (20)    22360 2024-04-03 05:06:51.000000 rubicon-objc-0.4.8/docs/_static/images/rubicon.png
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-03 05:07:38.856880 rubicon-objc-0.4.8/docs/background/
--rw-r--r--   0 runner     (501) staff       (20)     1045 2024-04-03 05:06:51.000000 rubicon-objc-0.4.8/docs/background/community.rst
--rw-r--r--   0 runner     (501) staff       (20)      826 2024-04-03 05:06:51.000000 rubicon-objc-0.4.8/docs/background/faq.rst
--rw-r--r--   0 runner     (501) staff       (20)      245 2024-04-03 05:06:51.000000 rubicon-objc-0.4.8/docs/background/index.rst
--rw-r--r--   0 runner     (501) staff       (20)    28855 2024-04-03 05:06:51.000000 rubicon-objc-0.4.8/docs/background/releases.rst
--rw-r--r--   0 runner     (501) staff       (20)       18 2024-04-03 05:06:51.000000 rubicon-objc-0.4.8/docs/background/roadmap.rst
--rw-r--r--   0 runner     (501) staff       (20)      245 2024-04-03 05:06:51.000000 rubicon-objc-0.4.8/docs/background/success.rst
--rw-r--r--   0 runner     (501) staff       (20)    10989 2024-04-03 05:06:51.000000 rubicon-objc-0.4.8/docs/conf.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-03 05:07:38.861678 rubicon-objc-0.4.8/docs/how-to/
--rw-r--r--   0 runner     (501) staff       (20)     3667 2024-04-03 05:06:51.000000 rubicon-objc-0.4.8/docs/how-to/async.rst
--rw-r--r--   0 runner     (501) staff       (20)    21047 2024-04-03 05:06:51.000000 rubicon-objc-0.4.8/docs/how-to/c-functions.rst
--rw-r--r--   0 runner     (501) staff       (20)     4934 2024-04-03 05:06:51.000000 rubicon-objc-0.4.8/docs/how-to/contribute-code.rst
--rw-r--r--   0 runner     (501) staff       (20)     4159 2024-04-03 05:06:52.000000 rubicon-objc-0.4.8/docs/how-to/contribute-docs.rst
--rw-r--r--   0 runner     (501) staff       (20)      508 2024-04-03 05:06:52.000000 rubicon-objc-0.4.8/docs/how-to/get-started.rst
--rw-r--r--   0 runner     (501) staff       (20)      490 2024-04-03 05:06:52.000000 rubicon-objc-0.4.8/docs/how-to/index.rst
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-03 05:07:38.862809 rubicon-objc-0.4.8/docs/how-to/internal/
--rw-r--r--   0 runner     (501) staff       (20)      229 2024-04-03 05:06:52.000000 rubicon-objc-0.4.8/docs/how-to/internal/index.rst
--rw-r--r--   0 runner     (501) staff       (20)     4264 2024-04-03 05:06:52.000000 rubicon-objc-0.4.8/docs/how-to/internal/release.rst
--rw-r--r--   0 runner     (501) staff       (20)     4699 2024-04-03 05:06:52.000000 rubicon-objc-0.4.8/docs/how-to/memory-management.rst
--rw-r--r--   0 runner     (501) staff       (20)     3709 2024-04-03 05:06:52.000000 rubicon-objc-0.4.8/docs/how-to/protocols.rst
--rw-r--r--   0 runner     (501) staff       (20)    14675 2024-04-03 05:06:52.000000 rubicon-objc-0.4.8/docs/how-to/type-mapping.rst
--rw-r--r--   0 runner     (501) staff       (20)     1504 2024-04-03 05:06:52.000000 rubicon-objc-0.4.8/docs/index.rst
--rw-r--r--   0 runner     (501) staff       (20)      933 2024-04-03 05:06:52.000000 rubicon-objc-0.4.8/docs/make.bat
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-03 05:07:38.866447 rubicon-objc-0.4.8/docs/reference/
--rw-r--r--   0 runner     (501) staff       (20)      448 2024-04-03 05:06:52.000000 rubicon-objc-0.4.8/docs/reference/index.rst
--rw-r--r--   0 runner     (501) staff       (20)    20276 2024-04-03 05:06:52.000000 rubicon-objc-0.4.8/docs/reference/rubicon-objc-api.rst
--rw-r--r--   0 runner     (501) staff       (20)      791 2024-04-03 05:06:52.000000 rubicon-objc-0.4.8/docs/reference/rubicon-objc-eventloop.rst
--rw-r--r--   0 runner     (501) staff       (20)     5641 2024-04-03 05:06:52.000000 rubicon-objc-0.4.8/docs/reference/rubicon-objc-runtime.rst
--rw-r--r--   0 runner     (501) staff       (20)    15405 2024-04-03 05:06:52.000000 rubicon-objc-0.4.8/docs/reference/rubicon-objc-types.rst
--rw-r--r--   0 runner     (501) staff       (20)     3418 2024-04-03 05:06:52.000000 rubicon-objc-0.4.8/docs/reference/rubicon-objc.rst
--rw-r--r--   0 runner     (501) staff       (20)      493 2024-04-03 05:06:52.000000 rubicon-objc-0.4.8/docs/spelling_wordlist
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-03 05:07:38.867983 rubicon-objc-0.4.8/docs/tutorial/
--rw-r--r--   0 runner     (501) staff       (20)      506 2024-04-03 05:06:53.000000 rubicon-objc-0.4.8/docs/tutorial/index.rst
--rw-r--r--   0 runner     (501) staff       (20)     4506 2024-04-03 05:06:53.000000 rubicon-objc-0.4.8/docs/tutorial/tutorial-1.rst
--rw-r--r--   0 runner     (501) staff       (20)     5518 2024-04-03 05:06:53.000000 rubicon-objc-0.4.8/docs/tutorial/tutorial-2.rst
--rw-r--r--   0 runner     (501) staff       (20)     3126 2024-04-03 05:06:53.000000 rubicon-objc-0.4.8/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)       38 2024-04-03 05:07:38.894728 rubicon-objc-0.4.8/setup.cfg
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-03 05:07:38.838425 rubicon-objc-0.4.8/src/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-03 05:07:38.838160 rubicon-objc-0.4.8/src/rubicon/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-03 05:07:38.872398 rubicon-objc-0.4.8/src/rubicon/objc/
--rw-r--r--   0 runner     (501) staff       (20)     3656 2024-04-03 05:06:53.000000 rubicon-objc-0.4.8/src/rubicon/objc/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)   100198 2024-04-03 05:06:53.000000 rubicon-objc-0.4.8/src/rubicon/objc/api.py
--rw-r--r--   0 runner     (501) staff       (20)    13945 2024-04-03 05:06:53.000000 rubicon-objc-0.4.8/src/rubicon/objc/collections.py
--rw-r--r--   0 runner     (501) staff       (20)    10066 2024-04-03 05:06:53.000000 rubicon-objc-0.4.8/src/rubicon/objc/ctypes_patch.py
--rw-r--r--   0 runner     (501) staff       (20)    24378 2024-04-03 05:06:53.000000 rubicon-objc-0.4.8/src/rubicon/objc/eventloop.py
--rw-r--r--   0 runner     (501) staff       (20)    42343 2024-04-03 05:06:53.000000 rubicon-objc-0.4.8/src/rubicon/objc/runtime.py
--rw-r--r--   0 runner     (501) staff       (20)    31846 2024-04-03 05:06:53.000000 rubicon-objc-0.4.8/src/rubicon/objc/types.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-03 05:07:38.889200 rubicon-objc-0.4.8/src/rubicon_objc.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     5714 2024-04-03 05:07:38.000000 rubicon-objc-0.4.8/src/rubicon_objc.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     2377 2024-04-03 05:07:38.000000 rubicon-objc-0.4.8/src/rubicon_objc.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-04-03 05:07:38.000000 rubicon-objc-0.4.8/src/rubicon_objc.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)      432 2024-04-03 05:07:38.000000 rubicon-objc-0.4.8/src/rubicon_objc.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)        8 2024-04-03 05:07:38.000000 rubicon-objc-0.4.8/src/rubicon_objc.egg-info/top_level.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-03 05:07:38.879645 rubicon-objc-0.4.8/tests/
--rw-r--r--   0 runner     (501) staff       (20)      492 2024-04-03 05:06:53.000000 rubicon-objc-0.4.8/tests/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-03 05:07:38.888573 rubicon-objc-0.4.8/tests/objc/
--rw-r--r--   0 runner     (501) staff       (20)      104 2024-04-03 05:06:53.000000 rubicon-objc-0.4.8/tests/objc/Altered_Example.h
--rw-r--r--   0 runner     (501) staff       (20)       85 2024-04-03 05:06:53.000000 rubicon-objc-0.4.8/tests/objc/Altered_Example.m
--rw-r--r--   0 runner     (501) staff       (20)      567 2024-04-03 05:06:53.000000 rubicon-objc-0.4.8/tests/objc/BaseExample.h
--rw-r--r--   0 runner     (501) staff       (20)     1331 2024-04-03 05:06:53.000000 rubicon-objc-0.4.8/tests/objc/BaseExample.m
--rw-r--r--   0 runner     (501) staff       (20)      929 2024-04-03 05:06:54.000000 rubicon-objc-0.4.8/tests/objc/Blocks.h
--rw-r--r--   0 runner     (501) staff       (20)     1239 2024-04-03 05:06:54.000000 rubicon-objc-0.4.8/tests/objc/Blocks.m
--rw-r--r--   0 runner     (501) staff       (20)      264 2024-04-03 05:06:54.000000 rubicon-objc-0.4.8/tests/objc/Callback.h
--rw-r--r--   0 runner     (501) staff       (20)      392 2024-04-03 05:06:54.000000 rubicon-objc-0.4.8/tests/objc/DescriptionTester.h
--rw-r--r--   0 runner     (501) staff       (20)      641 2024-04-03 05:06:54.000000 rubicon-objc-0.4.8/tests/objc/DescriptionTester.m
--rw-r--r--   0 runner     (501) staff       (20)     2558 2024-04-03 05:06:54.000000 rubicon-objc-0.4.8/tests/objc/Example.h
--rw-r--r--   0 runner     (501) staff       (20)     4767 2024-04-03 05:06:54.000000 rubicon-objc-0.4.8/tests/objc/Example.m
--rw-r--r--   0 runner     (501) staff       (20)      593 2024-04-03 05:06:54.000000 rubicon-objc-0.4.8/tests/objc/Makefile
--rw-r--r--   0 runner     (501) staff       (20)      197 2024-04-03 05:06:54.000000 rubicon-objc-0.4.8/tests/objc/Protocols.h
--rw-r--r--   0 runner     (501) staff       (20)      104 2024-04-03 05:06:54.000000 rubicon-objc-0.4.8/tests/objc/SpecificExample.h
--rw-r--r--   0 runner     (501) staff       (20)      394 2024-04-03 05:06:54.000000 rubicon-objc-0.4.8/tests/objc/SpecificExample.m
--rw-r--r--   0 runner     (501) staff       (20)      328 2024-04-03 05:06:54.000000 rubicon-objc-0.4.8/tests/objc/Thing.h
--rw-r--r--   0 runner     (501) staff       (20)      711 2024-04-03 05:06:54.000000 rubicon-objc-0.4.8/tests/objc/Thing.m
--rw-r--r--   0 runner     (501) staff       (20)    11932 2024-04-03 05:06:54.000000 rubicon-objc-0.4.8/tests/test_NSArray.py
--rw-r--r--   0 runner     (501) staff       (20)    13268 2024-04-03 05:06:54.000000 rubicon-objc-0.4.8/tests/test_NSDictionary.py
--rw-r--r--   0 runner     (501) staff       (20)    16420 2024-04-03 05:06:54.000000 rubicon-objc-0.4.8/tests/test_NSString.py
--rw-r--r--   0 runner     (501) staff       (20)     5843 2024-04-03 05:06:54.000000 rubicon-objc-0.4.8/tests/test_async.py
--rw-r--r--   0 runner     (501) staff       (20)     8086 2024-04-03 05:06:55.000000 rubicon-objc-0.4.8/tests/test_blocks.py
--rw-r--r--   0 runner     (501) staff       (20)    74860 2024-04-03 05:06:55.000000 rubicon-objc-0.4.8/tests/test_core.py
--rw-r--r--   0 runner     (501) staff       (20)     4369 2024-04-03 05:06:55.000000 rubicon-objc-0.4.8/tests/test_ctypes_patch.py
--rw-r--r--   0 runner     (501) staff       (20)     2508 2024-04-03 05:06:55.000000 rubicon-objc-0.4.8/tox.ini
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-03 01:42:48.896587 rubicon_objc-0.4.9/
+-rw-r--r--   0 runner     (501) staff       (20)       71 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/.git-blame-ignore-revs
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-03 01:42:48.883496 rubicon_objc-0.4.9/.github/
+-rw-r--r--   0 runner     (501) staff       (20)      377 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/.github/dependabot.yml
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-03 01:42:48.884331 rubicon_objc-0.4.9/.github/workflows/
+-rw-r--r--   0 runner     (501) staff       (20)     2386 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/.github/workflows/ci.yml
+-rw-r--r--   0 runner     (501) staff       (20)      281 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/.github/workflows/config-file-deps-bump.yml
+-rw-r--r--   0 runner     (501) staff       (20)      230 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/.github/workflows/dependabot-changenote.yml
+-rw-r--r--   0 runner     (501) staff       (20)      257 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/.github/workflows/pre-commit-update.yml
+-rw-r--r--   0 runner     (501) staff       (20)      740 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/.github/workflows/publish.yml
+-rw-r--r--   0 runner     (501) staff       (20)     2117 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/.github/workflows/release.yml
+-rw-r--r--   0 runner     (501) staff       (20)      158 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/.gitignore
+-rw-r--r--   0 runner     (501) staff       (20)      855 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner     (501) staff       (20)      707 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/.readthedocs.yml
+-rw-r--r--   0 runner     (501) staff       (20)      140 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/CHANGELOG.rst
+-rw-r--r--   0 runner     (501) staff       (20)      182 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/CONTRIBUTING.md
+-rw-r--r--   0 runner     (501) staff       (20)     3278 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)     5847 2024-05-03 01:42:48.896237 rubicon_objc-0.4.9/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     3543 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/README.rst
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-03 01:42:48.884568 rubicon_objc-0.4.9/changes/
+-rw-r--r--   0 runner     (501) staff       (20)       12 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/changes/.gitignore
+-rw-r--r--   0 runner     (501) staff       (20)      792 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/changes/template.rst
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-03 01:42:48.885207 rubicon_objc-0.4.9/docs/
+-rw-r--r--   0 runner     (501) staff       (20)      728 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/docs/Makefile
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-03 01:42:48.880989 rubicon_objc-0.4.9/docs/_mocked_modules/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-03 01:42:48.885476 rubicon_objc-0.4.9/docs/_mocked_modules/ctypes/
+-rw-r--r--   0 runner     (501) staff       (20)    10469 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/docs/_mocked_modules/ctypes/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      127 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/docs/_mocked_modules/ctypes/util.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-03 01:42:48.881098 rubicon_objc-0.4.9/docs/_static/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-03 01:42:48.885617 rubicon_objc-0.4.9/docs/_static/images/
+-rw-r--r--   0 runner     (501) staff       (20)    22360 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/docs/_static/images/rubicon.png
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-03 01:42:48.886475 rubicon_objc-0.4.9/docs/background/
+-rw-r--r--   0 runner     (501) staff       (20)     1045 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/docs/background/community.rst
+-rw-r--r--   0 runner     (501) staff       (20)      826 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/docs/background/faq.rst
+-rw-r--r--   0 runner     (501) staff       (20)      245 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/docs/background/index.rst
+-rw-r--r--   0 runner     (501) staff       (20)    29811 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/docs/background/releases.rst
+-rw-r--r--   0 runner     (501) staff       (20)       18 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/docs/background/roadmap.rst
+-rw-r--r--   0 runner     (501) staff       (20)      245 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/docs/background/success.rst
+-rw-r--r--   0 runner     (501) staff       (20)    10989 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/docs/conf.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-03 01:42:48.887833 rubicon_objc-0.4.9/docs/how-to/
+-rw-r--r--   0 runner     (501) staff       (20)     3667 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/docs/how-to/async.rst
+-rw-r--r--   0 runner     (501) staff       (20)    21039 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/docs/how-to/c-functions.rst
+-rw-r--r--   0 runner     (501) staff       (20)     4934 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/docs/how-to/contribute-code.rst
+-rw-r--r--   0 runner     (501) staff       (20)     4159 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/docs/how-to/contribute-docs.rst
+-rw-r--r--   0 runner     (501) staff       (20)      508 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/docs/how-to/get-started.rst
+-rw-r--r--   0 runner     (501) staff       (20)      490 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/docs/how-to/index.rst
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-03 01:42:48.888117 rubicon_objc-0.4.9/docs/how-to/internal/
+-rw-r--r--   0 runner     (501) staff       (20)      229 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/docs/how-to/internal/index.rst
+-rw-r--r--   0 runner     (501) staff       (20)     4264 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/docs/how-to/internal/release.rst
+-rw-r--r--   0 runner     (501) staff       (20)     4699 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/docs/how-to/memory-management.rst
+-rw-r--r--   0 runner     (501) staff       (20)     3705 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/docs/how-to/protocols.rst
+-rw-r--r--   0 runner     (501) staff       (20)    18232 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/docs/how-to/type-mapping.rst
+-rw-r--r--   0 runner     (501) staff       (20)     1504 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/docs/index.rst
+-rw-r--r--   0 runner     (501) staff       (20)      933 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/docs/make.bat
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-03 01:42:48.889038 rubicon_objc-0.4.9/docs/reference/
+-rw-r--r--   0 runner     (501) staff       (20)      448 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/docs/reference/index.rst
+-rw-r--r--   0 runner     (501) staff       (20)    20276 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/docs/reference/rubicon-objc-api.rst
+-rw-r--r--   0 runner     (501) staff       (20)      791 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/docs/reference/rubicon-objc-eventloop.rst
+-rw-r--r--   0 runner     (501) staff       (20)     5641 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/docs/reference/rubicon-objc-runtime.rst
+-rw-r--r--   0 runner     (501) staff       (20)    15405 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/docs/reference/rubicon-objc-types.rst
+-rw-r--r--   0 runner     (501) staff       (20)     3418 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/docs/reference/rubicon-objc.rst
+-rw-r--r--   0 runner     (501) staff       (20)      493 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/docs/spelling_wordlist
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-03 01:42:48.889432 rubicon_objc-0.4.9/docs/tutorial/
+-rw-r--r--   0 runner     (501) staff       (20)      506 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/docs/tutorial/index.rst
+-rw-r--r--   0 runner     (501) staff       (20)     4907 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/docs/tutorial/tutorial-1.rst
+-rw-r--r--   0 runner     (501) staff       (20)     5519 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/docs/tutorial/tutorial-2.rst
+-rw-r--r--   0 runner     (501) staff       (20)     3127 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)       38 2024-05-03 01:42:48.896639 rubicon_objc-0.4.9/setup.cfg
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-03 01:42:48.881758 rubicon_objc-0.4.9/src/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-03 01:42:48.881694 rubicon_objc-0.4.9/src/rubicon/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-03 01:42:48.890857 rubicon_objc-0.4.9/src/rubicon/objc/
+-rw-r--r--   0 runner     (501) staff       (20)     3656 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/src/rubicon/objc/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    99485 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/src/rubicon/objc/api.py
+-rw-r--r--   0 runner     (501) staff       (20)    13945 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/src/rubicon/objc/collections.py
+-rw-r--r--   0 runner     (501) staff       (20)    12828 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/src/rubicon/objc/ctypes_patch.py
+-rw-r--r--   0 runner     (501) staff       (20)    24378 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/src/rubicon/objc/eventloop.py
+-rw-r--r--   0 runner     (501) staff       (20)    42343 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/src/rubicon/objc/runtime.py
+-rw-r--r--   0 runner     (501) staff       (20)    31846 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/src/rubicon/objc/types.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-03 01:42:48.894814 rubicon_objc-0.4.9/src/rubicon_objc.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     5847 2024-05-03 01:42:48.000000 rubicon_objc-0.4.9/src/rubicon_objc.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     2377 2024-05-03 01:42:48.000000 rubicon_objc-0.4.9/src/rubicon_objc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-05-03 01:42:48.000000 rubicon_objc-0.4.9/src/rubicon_objc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)      433 2024-05-03 01:42:48.000000 rubicon_objc-0.4.9/src/rubicon_objc.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)        8 2024-05-03 01:42:48.000000 rubicon_objc-0.4.9/src/rubicon_objc.egg-info/top_level.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-03 01:42:48.892667 rubicon_objc-0.4.9/tests/
+-rw-r--r--   0 runner     (501) staff       (20)      492 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/tests/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-03 01:42:48.894623 rubicon_objc-0.4.9/tests/objc/
+-rw-r--r--   0 runner     (501) staff       (20)      104 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/tests/objc/Altered_Example.h
+-rw-r--r--   0 runner     (501) staff       (20)       85 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/tests/objc/Altered_Example.m
+-rw-r--r--   0 runner     (501) staff       (20)      567 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/tests/objc/BaseExample.h
+-rw-r--r--   0 runner     (501) staff       (20)     1331 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/tests/objc/BaseExample.m
+-rw-r--r--   0 runner     (501) staff       (20)      929 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/tests/objc/Blocks.h
+-rw-r--r--   0 runner     (501) staff       (20)     1239 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/tests/objc/Blocks.m
+-rw-r--r--   0 runner     (501) staff       (20)      264 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/tests/objc/Callback.h
+-rw-r--r--   0 runner     (501) staff       (20)      392 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/tests/objc/DescriptionTester.h
+-rw-r--r--   0 runner     (501) staff       (20)      641 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/tests/objc/DescriptionTester.m
+-rw-r--r--   0 runner     (501) staff       (20)     2956 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/tests/objc/Example.h
+-rw-r--r--   0 runner     (501) staff       (20)     5296 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/tests/objc/Example.m
+-rw-r--r--   0 runner     (501) staff       (20)      593 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/tests/objc/Makefile
+-rw-r--r--   0 runner     (501) staff       (20)      197 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/tests/objc/Protocols.h
+-rw-r--r--   0 runner     (501) staff       (20)      104 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/tests/objc/SpecificExample.h
+-rw-r--r--   0 runner     (501) staff       (20)      394 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/tests/objc/SpecificExample.m
+-rw-r--r--   0 runner     (501) staff       (20)      328 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/tests/objc/Thing.h
+-rw-r--r--   0 runner     (501) staff       (20)      711 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/tests/objc/Thing.m
+-rw-r--r--   0 runner     (501) staff       (20)    11932 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/tests/test_NSArray.py
+-rw-r--r--   0 runner     (501) staff       (20)    13268 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/tests/test_NSDictionary.py
+-rw-r--r--   0 runner     (501) staff       (20)    16420 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/tests/test_NSString.py
+-rw-r--r--   0 runner     (501) staff       (20)     5843 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/tests/test_async.py
+-rw-r--r--   0 runner     (501) staff       (20)     8086 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/tests/test_blocks.py
+-rw-r--r--   0 runner     (501) staff       (20)    76078 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/tests/test_core.py
+-rw-r--r--   0 runner     (501) staff       (20)     4369 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/tests/test_ctypes_patch.py
+-rw-r--r--   0 runner     (501) staff       (20)     2508 2024-05-03 01:42:33.000000 rubicon_objc-0.4.9/tox.ini
```

### Comparing `rubicon-objc-0.4.8/.github/workflows/ci.yml` & `rubicon_objc-0.4.9/.github/workflows/ci.yml`

 * *Files 0% similar despite different names*

```diff
@@ -60,25 +60,25 @@
             python-version : "3.8"
 
           - platform: "macos-14"
             python-version : "3.9"
 
     steps:
     - name: Checkout
-      uses: actions/checkout@v4.1.2
+      uses: actions/checkout@v4.1.4
       with:
         fetch-depth: 0
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v5.1.0
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Get packages
-      uses: actions/download-artifact@v4.1.4
+      uses: actions/download-artifact@v4.1.7
       with:
         name: ${{ needs.package.outputs.artifact-name }}
         path: dist
 
     - name: Install dev dependencies
       run: |
         # We don't actually want to install rubicon;
```

### Comparing `rubicon-objc-0.4.8/.github/workflows/publish.yml` & `rubicon_objc-0.4.9/.github/workflows/publish.yml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 jobs:
   deploy:
     runs-on: ubuntu-latest
     permissions:
       # This permission is required for trusted publishing.
       id-token: write
     steps:
-      - uses: dsaltares/fetch-gh-release-asset@1.1.1
+      - uses: dsaltares/fetch-gh-release-asset@1.1.2
         with:
           version: tags/${{ github.event.release.tag_name }}
           # This next line is *not* a bash filename expansion - it's a regex.
           # We need to match all files that start with rubicon-objc or
           # rubicon_objc, but not the "Source code" zip and tarball.
           file: rubicon.*
           regex: true
```

### Comparing `rubicon-objc-0.4.8/.github/workflows/release.yml` & `rubicon_objc-0.4.9/.github/workflows/release.yml`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
       - name: Set up Python
         uses: actions/setup-python@v5.1.0
         with:
           python-version: "3.X"
 
       - name: Get packages
-        uses: actions/download-artifact@v4.1.4
+        uses: actions/download-artifact@v4.1.7
         with:
           name: ${{ needs.ci.outputs.artifact-name }}
           path: dist
 
       - name: Install packages
         run: pip install dist/rubicon_objc-*.whl
 
@@ -64,15 +64,15 @@
     runs-on: ubuntu-latest
     permissions:
       contents: write
       # This permission is required for trusted publishing.
       id-token: write
     steps:
       - name: Get packages
-        uses: actions/download-artifact@v4.1.4
+        uses: actions/download-artifact@v4.1.7
         with:
           name: ${{ needs.ci.outputs.artifact-name }}
           path: dist
 
       - name: Publish release to Test PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
```

### Comparing `rubicon-objc-0.4.8/.pre-commit-config.yaml` & `rubicon_objc-0.4.9/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: check-toml
       - id: check-yaml
       - id: check-case-conflict
       - id: check-docstring-first
       - id: end-of-file-fixer
       - id: trailing-whitespace
@@ -15,15 +15,15 @@
         additional_dependencies: [toml]
   - repo: https://github.com/asottile/pyupgrade
     rev: v3.15.2
     hooks:
       - id: pyupgrade
         args: [--py38-plus]
   - repo: https://github.com/psf/black-pre-commit-mirror
-    rev: 24.3.0
+    rev: 24.4.2
     hooks:
     - id: black
   - repo: https://github.com/PyCQA/flake8
     rev: 7.0.0
     hooks:
       - id: flake8
   - repo: https://github.com/codespell-project/codespell
```

### Comparing `rubicon-objc-0.4.8/.readthedocs.yml` & `rubicon_objc-0.4.9/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.8/LICENSE` & `rubicon_objc-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.8/PKG-INFO` & `rubicon_objc-0.4.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubicon-objc
-Version: 0.4.8
+Version: 0.4.9
 Summary: A bridge between an Objective C runtime environment and Python.
 Author-email: Russell Keith-Magee <russell@keith-magee.com>
 Maintainer-email: BeeWare Team <team@beeware.org>
 License: New BSD
 Project-URL: Homepage, https://beeware.org/rubicon
 Project-URL: Funding, https://beeware.org/contributing/membership/
 Project-URL: Documentation, https://rubicon-objc.readthedocs.io/en/latest/
@@ -26,60 +26,64 @@
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Provides-Extra: dev
 Requires-Dist: pre-commit==3.5.0; python_version < "3.9" and extra == "dev"
 Requires-Dist: pre-commit==3.7.0; python_version >= "3.9" and extra == "dev"
-Requires-Dist: pytest==8.1.1; extra == "dev"
+Requires-Dist: pytest==8.2.0; extra == "dev"
 Requires-Dist: pytest-tldr==0.2.5; extra == "dev"
 Requires-Dist: setuptools_scm==8.0.4; extra == "dev"
-Requires-Dist: tox==4.14.2; extra == "dev"
+Requires-Dist: tox==4.15.0; extra == "dev"
 Provides-Extra: docs
-Requires-Dist: furo==2024.1.29; extra == "docs"
+Requires-Dist: furo==2024.4.27; extra == "docs"
 Requires-Dist: pyenchant==3.2.2; extra == "docs"
 Requires-Dist: sphinx==7.1.2; python_version < "3.9" and extra == "docs"
-Requires-Dist: sphinx==7.2.6; python_version >= "3.9" and extra == "docs"
+Requires-Dist: sphinx==7.3.7; python_version >= "3.9" and extra == "docs"
 Requires-Dist: sphinx_tabs==3.4.5; extra == "docs"
 Requires-Dist: sphinx-autobuild==2021.3.14; python_version < "3.9" and extra == "docs"
-Requires-Dist: sphinx-autobuild==2024.2.4; python_version >= "3.9" and extra == "docs"
+Requires-Dist: sphinx-autobuild==2024.4.16; python_version >= "3.9" and extra == "docs"
 Requires-Dist: sphinx-copybutton==0.5.2; extra == "docs"
 Requires-Dist: sphinxcontrib-spelling==8.0.0; extra == "docs"
 
-.. image:: https://beeware.org/project/projects/bridges/rubicon/rubicon.png
+.. |logo| image:: https://beeware.org/project/projects/bridges/rubicon/rubicon.png
     :width: 72px
     :target: https://beeware.org/rubicon
 
-Rubicon-ObjC
-============
-
-.. image:: https://img.shields.io/pypi/pyversions/rubicon-objc.svg
+.. |pyversions| image:: https://img.shields.io/pypi/pyversions/rubicon-objc.svg
    :target: https://pypi.python.org/pypi/rubicon-objc
    :alt: Python Versions
 
-.. image:: https://img.shields.io/pypi/v/rubicon-objc.svg
+.. |version| image:: https://img.shields.io/pypi/v/rubicon-objc.svg
    :target: https://pypi.python.org/pypi/rubicon-objc
    :alt: Project Version
 
-.. image:: https://img.shields.io/pypi/status/rubicon-objc.svg
+.. |maturity| image:: https://img.shields.io/pypi/status/rubicon-objc.svg
    :target: https://pypi.python.org/pypi/rubicon-objc
    :alt: Project status
 
-.. image:: https://img.shields.io/pypi/l/rubicon-objc.svg
+.. |license| image:: https://img.shields.io/pypi/l/rubicon-objc.svg
    :target: https://github.com/beeware/rubicon-objc/blob/main/LICENSE
    :alt: License
 
-.. image:: https://github.com/beeware/rubicon-objc/workflows/CI/badge.svg?branch=main
+.. |ci| image:: https://github.com/beeware/rubicon-objc/workflows/CI/badge.svg?branch=main
    :target: https://github.com/beeware/rubicon-objc/actions
    :alt: Build Status
 
-.. image:: https://img.shields.io/discord/836455665257021440?label=Discord%20Chat&logo=discord&style=plastic
+.. |social| image:: https://img.shields.io/discord/836455665257021440?label=Discord%20Chat&logo=discord&style=plastic
    :target: https://beeware.org/bee/chat/
    :alt: Discord server
 
+|logo|
+
+Rubicon-ObjC
+============
+
+|pyversions| |version| |maturity| |license| |ci| |social|
+
 Rubicon-ObjC is a bridge between Objective-C and Python. It enables you to:
 
 * Use Python to instantiate objects defined in Objective-C,
 * Use Python to invoke methods on objects defined in Objective-C, and
 * Subclass and extend Objective-C classes in Python.
 
 It also includes wrappers of the some key data types from the Foundation
```

### Comparing `rubicon-objc-0.4.8/README.rst` & `rubicon_objc-0.4.9/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,42 @@
-.. image:: https://beeware.org/project/projects/bridges/rubicon/rubicon.png
+.. |logo| image:: https://beeware.org/project/projects/bridges/rubicon/rubicon.png
     :width: 72px
     :target: https://beeware.org/rubicon
 
-Rubicon-ObjC
-============
-
-.. image:: https://img.shields.io/pypi/pyversions/rubicon-objc.svg
+.. |pyversions| image:: https://img.shields.io/pypi/pyversions/rubicon-objc.svg
    :target: https://pypi.python.org/pypi/rubicon-objc
    :alt: Python Versions
 
-.. image:: https://img.shields.io/pypi/v/rubicon-objc.svg
+.. |version| image:: https://img.shields.io/pypi/v/rubicon-objc.svg
    :target: https://pypi.python.org/pypi/rubicon-objc
    :alt: Project Version
 
-.. image:: https://img.shields.io/pypi/status/rubicon-objc.svg
+.. |maturity| image:: https://img.shields.io/pypi/status/rubicon-objc.svg
    :target: https://pypi.python.org/pypi/rubicon-objc
    :alt: Project status
 
-.. image:: https://img.shields.io/pypi/l/rubicon-objc.svg
+.. |license| image:: https://img.shields.io/pypi/l/rubicon-objc.svg
    :target: https://github.com/beeware/rubicon-objc/blob/main/LICENSE
    :alt: License
 
-.. image:: https://github.com/beeware/rubicon-objc/workflows/CI/badge.svg?branch=main
+.. |ci| image:: https://github.com/beeware/rubicon-objc/workflows/CI/badge.svg?branch=main
    :target: https://github.com/beeware/rubicon-objc/actions
    :alt: Build Status
 
-.. image:: https://img.shields.io/discord/836455665257021440?label=Discord%20Chat&logo=discord&style=plastic
+.. |social| image:: https://img.shields.io/discord/836455665257021440?label=Discord%20Chat&logo=discord&style=plastic
    :target: https://beeware.org/bee/chat/
    :alt: Discord server
 
+|logo|
+
+Rubicon-ObjC
+============
+
+|pyversions| |version| |maturity| |license| |ci| |social|
+
 Rubicon-ObjC is a bridge between Objective-C and Python. It enables you to:
 
 * Use Python to instantiate objects defined in Objective-C,
 * Use Python to invoke methods on objects defined in Objective-C, and
 * Subclass and extend Objective-C classes in Python.
 
 It also includes wrappers of the some key data types from the Foundation
```

### Comparing `rubicon-objc-0.4.8/changes/template.rst` & `rubicon_objc-0.4.9/changes/template.rst`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.8/docs/Makefile` & `rubicon_objc-0.4.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.8/docs/_mocked_modules/ctypes/__init__.py` & `rubicon_objc-0.4.9/docs/_mocked_modules/ctypes/__init__.py`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.8/docs/_static/images/rubicon.png` & `rubicon_objc-0.4.9/docs/_static/images/rubicon.png`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.8/docs/background/community.rst` & `rubicon_objc-0.4.9/docs/background/community.rst`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.8/docs/background/faq.rst` & `rubicon_objc-0.4.9/docs/background/faq.rst`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.8/docs/background/releases.rst` & `rubicon_objc-0.4.9/docs/background/releases.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,46 @@
 Release History
 ===============
 
 .. towncrier release notes start
 
+0.4.9 (2024-05-03)
+==================
+
+Features
+--------
+
+* Objective-C methods with repeated argument names can now be called by using a ``__`` suffix in the Python keyword argument to provide a unique name. (#148)
+* The error message has been improved when an Objective-C selector matching the provided arguments cannot be found. (#461)
+
+
+Bugfixes
+--------
+
+* The handling of structure and union return types was updated to be compatible with changes to ctypes introduced in Python 3.13.0a6. (#444)
+
+
+Backward Incompatible Changes
+-----------------------------
+
+* The order of keyword arguments used when invoking methods must now match the order they are defined in the Objective-C API. Previously arguments could be in any order. (#453)
+
+
+Documentation
+-------------
+
+* The README badges were updated to display correctly on GitHub. (#463)
+
+
+Misc
+----
+
+* #440, #441, #442, #443, #447, #448, #449, #450, #452, #454, #455, #456, #457, #458, #459, #460
+
+
 0.4.8 (2024-04-03)
 ==================
 
 Features
 --------
 
 * Name clashes caused by re-registering Objective C classes and protocols can now be automatically avoided by marking the class with ``auto_rename``. (#181)
```

### Comparing `rubicon-objc-0.4.8/docs/conf.py` & `rubicon_objc-0.4.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.8/docs/how-to/async.rst` & `rubicon_objc-0.4.9/docs/how-to/async.rst`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.8/docs/how-to/c-functions.rst` & `rubicon_objc-0.4.9/docs/how-to/c-functions.rst`

 * *Files 1% similar despite different names*

```diff
@@ -24,39 +24,39 @@
 
 Before we can call the function, we need to look it up first. To do this, we
 need to find and load the library in which the function is defined. In the case
 of standard C functions, this is the standard C library, ``libc``. Because this
 library is commonly used, Rubicon already loads it by default and exposes it in
 Python as :attr:`rubicon.objc.runtime.libc`.
 
-.. code-block:: python
+.. code-block:: pycon
 
     >>> from rubicon.objc.runtime import libc
     >>> libc
     <CDLL '/usr/lib/libc.dylib', handle 7fff60d0cb90 at 0x105850b38>
 
 .. note::
 
     For a list of all C libraries that Rubicon loads and exposes by default,
     see the :ref:`predefined-c-libraries` section of the
     :mod:`rubicon.objc.runtime` reference documentation.
 
     To access a library that is not predefined by Rubicon, you can use the
     :func:`~rubicon.objc.runtime.load_library` function:
 
-    .. code-block:: python
+    .. code-block:: pycon
 
         >>> from rubicon.objc.runtime import load_library
         >>> libm = load_library("m")
         >>> libm
         <CDLL '/usr/lib/libm.dylib', handle 7fff60d0cb90 at 0x10596be10>
 
 C functions are accessed as attributes on their library:
 
-.. code-block:: python
+.. code-block:: pycon
 
     >>> libc.puts
     <_FuncPtr object at 0x110178f20>
 
 However, unlike Objective-C methods, we cannot call C functions right away ---
 we must first declare the function's argument and return types. (Rubicon cannot
 do this automatically like with Objective-C methods, because plain C doesn't
@@ -91,30 +91,30 @@
 
     int puts(const char *);
 
 This means that ``puts`` returns an ``int`` and takes a single argument of type
 ``const char *`` (a pointer to one or more characters, i.e. a C string). This
 translates to the following Python ``ctypes`` code:
 
-.. code-block:: python
+.. code-block:: pycon
 
     >>> from ctypes import c_char_p, c_int
     >>> libc.puts.restype = c_int
     >>> libc.puts.argtypes = [c_char_p]
 
 Now that we have provided all of the necessary type information, we can call
 ``libc.puts``.
 
 For the ``c_char_p`` argument, we pass a byte string with the message we want
 to print out. ``ctypes`` automatically converts the byte string object to a
 ``c_char_p`` (``char *``) as the C function expects it. The string specifically
 needs to be a byte string (``bytes``), because C's ``char *`` strings are
 byte-based, unlike normal Python strings (``str``), which are Unicode-based.
 
-.. code-block:: python
+.. code-block:: pycon
 
     >>> res = libc.puts(b"Hello!")
     Hello!
 
 .. note::
 
     If you're running this code from an editor or IDE and don't see ``Hello!``
@@ -223,28 +223,28 @@
 
 Like functions, global variables are accessed via the library that they are
 defined by. The syntax is somewhat different for global variables though -
 instead of reading them directly as attributes of the library object, you use
 the ``in_dll`` method of the variable's *type*. (Every ``ctypes`` type has an
 ``in_dll`` method.)
 
-.. code-block:: python
+.. code-block:: pycon
 
     >>> from ctypes import c_double
     >>> from rubicon.objc.runtime import Foundation
     >>> NSFoundationVersionNumber = c_double.in_dll(Foundation, "NSFoundationVersionNumber")
     >>> NSFoundationVersionNumber
     c_double(1575.23)
 
 Note that ``in_dll`` doesn't return the variable's value directly - instead it
 returns a ``ctypes`` data object that has the variable's type, in this case
 ``c_double``. To access the variable's actual value, you can use the data
 object's ``value`` attribute:
 
-.. code-block:: python
+.. code-block:: pycon
 
     >>> NSFoundationVersionNumber.value
     1575.23
 
 Objective-C object constants
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
@@ -257,15 +257,15 @@
 .. code-block:: objc
 
     FOUNDATION_EXPORT NSString * const NSMetadataItemFSNameKey;
 
 Because they are so common, Rubicon provides the convenience function
 ``objc_const`` specifically for accessing Objective-C object constants:
 
-.. code-block:: python
+.. code-block:: pycon
 
     >>> from rubicon.objc import objc_const
     >>> from rubicon.objc.runtime import Foundation
     >>> NSMetadataItemFSNameKey = objc_const(Foundation, "NSMetadataItemFSNameKey")
     >>> NSMetadataItemFSNameKey
     <ObjCStrInstance: __NSCFConstantString at 0x10eecf350: kMDItemFSName>
```

### Comparing `rubicon-objc-0.4.8/docs/how-to/contribute-code.rst` & `rubicon_objc-0.4.9/docs/how-to/contribute-code.rst`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.8/docs/how-to/contribute-docs.rst` & `rubicon_objc-0.4.9/docs/how-to/contribute-docs.rst`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.8/docs/how-to/internal/release.rst` & `rubicon_objc-0.4.9/docs/how-to/internal/release.rst`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.8/docs/how-to/memory-management.rst` & `rubicon_objc-0.4.9/docs/how-to/memory-management.rst`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.8/docs/how-to/protocols.rst` & `rubicon_objc-0.4.9/docs/how-to/protocols.rst`

 * *Files 7% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 
 Looking up a protocol
 ---------------------
 
 Protocol objects can be looked up using the ``ObjCProtocol`` constructor,
 similar to how classes can be looked up using ``ObjCClass``:
 
-.. code-block:: python
+.. code-block:: pycon
 
     >>> NSCopying = ObjCProtocol('NSCopying')
     >>> NSCopying
     <ObjCProtocol: NSCopying>
 
 The ``isinstance`` function can be used to check whether an object conforms to
 a protocol:
 
-.. code-block:: python
+.. code-block:: pycon
 
     >>> isinstance(NSObject.new(), NSCopying)
     False
     >>> isinstance(NSArray.array(), NSCopying)
     True
 
 Implementing a protocol
@@ -59,25 +59,25 @@
         @objc_method
         def copyWithZone_(self, zone):
             return UserAccount.alloc().initWithUsername(self.username, emailAddress=self.emailAddress)
 
 We can now use our class. The ``copy`` method (which uses our implemented
 ``copyWithZone:`` method) can also be used:
 
-.. code-block:: python
+.. code-block:: pycon
 
     >>> ua = UserAccount.alloc().initWithUsername_emailAddress_(at('person'), at('person@example.com'))
     >>> ua
     <ObjCInstance: UserAccount at 0x106543210: <UserAccount: 0x106543220>>
     >>> ua.copy()
     <ObjCInstance: UserAccount at 0x106543210: <UserAccount: 0x106543220>>
 
 And we can check that the class conforms to the protocol:
 
-.. code-block:: python
+.. code-block:: pycon
 
     >>> isinstance(ua, NSCopying)
     True
 
 Writing custom protocols
 ------------------------
```

### Comparing `rubicon-objc-0.4.8/docs/how-to/type-mapping.rst` & `rubicon_objc-0.4.9/docs/how-to/type-mapping.rst`

 * *Files 18% similar despite different names*

```diff
@@ -107,14 +107,95 @@
 
 Objective-C objects are automatically returned as
 :class:`~rubicon.objc.api.ObjCInstance` objects, so you can call methods on
 them and access their properties. In some cases, Rubicon also provides
 additional Python methods on Objective-C objects -
 see :ref:`python_style_apis_for_objc` for details.
 
+Invoking Objective-C methods
+----------------------------
+
+Once an Objective-C class has been wrapped, the selectors on that class (or
+instances of that class) can be invoked as if they were methods on the Python
+class. Each Objective-C selector is converted into a Python method name by
+replacing the colons in the selector with underscores.
+
+For example, the Objective-C class ``NSURL`` has defines a instance selector of
+``-initWithString:relativeToURL:``; this will be converted into the Python
+method ``initWithString_relativeToURL_()``. Arguments to this method are all
+positional, and passed in the order they are defined in the selector. Selectors
+without arguments (such as ``+alloc`` or ``-init``) are defined as methods with
+no arguments, and no underscores in the name:
+
+.. code-block:: python
+
+    # Wrap the NSURL class
+    NSURL = ObjCClass("NSURL")
+    # Invoke the +alloc selector
+    my_url = NSURL.alloc()
+    # Invoke -initWithString:relativeToURL:
+    my_url.initWithString_relativeToURL_("something/", "https://example.com/")
+
+This can result in very long method names; so Rubicon also provides an alternate
+mapping for methods, using Python keyword arguments. In this approach, the first
+argument is handled as a positional argument, and all subsequent arguments are
+handled as keyword arguments, with the underscore suffixes being omitted. The
+last method in the previous example could also be invoked as:
+
+.. code-block:: python
+
+    # Invoke -initWithString:relativeToURL:
+    my_url.initWithString("something/", relativeToURL="https://example.com/")
+
+Keyword arguments *must* be passed in the order they are defined in the
+selector. For example, if you were invoking
+``-initFileURLWithPath:isDirectory:relativeToURL``, it *must* be invoked as:
+
+.. code-block:: python
+
+    # Invoke -initFileURLWithPath:isDirectory:relativeToURL
+    my_url.initFileURLWithPath(
+        "something/",
+        isDirectory=True,
+        relativeToURL="file:///Users/brutus/"
+    )
+
+Even though from a strict *Python* perspective, passing ``relativeToURL`` before
+``isDirectory`` would be syntactically equivalent, this *will not* match the
+corresponding Objective-C selector.
+
+This "interleaved" keyword syntax works for *most* Objective-C selectors without
+any problem. However, Objective-C allows arguments in a selector to be repeated.
+For example, ``NSLayoutConstraint`` defines a
+``+constraintWithItem:attribute:relatedBy:toItem:attribute:multiplier:constant:``
+selector, duplicating the ``attribute`` keyword. Python will not allow a keyword
+argument to be duplicated, so to reach selectors of this type, Rubicon allows
+any keyword argument to be appended with a ``__`` suffix to generate a name that
+is unique in the Python code:
+
+.. code-block:: python
+
+    # Invoke +constraintWithItem:attribute:relatedBy:toItem:attribute:multiplier:constant:
+    NSLayoutConstraint.constraintWithItem(
+        first_item,
+        attribute__1=first_attribute,
+        relatedBy=relation,
+        toItem=second_item,
+        attribute__2=second_attribute,
+        multiplier=2.0,
+        constant=1.0
+    )
+
+The name used after the ``__`` has no significance - it is only used to ensure
+that the Python keyword is unique, and is immediately stripped and ignored. By
+convention, we recommend using integers as we've done in this example; but you
+*can* use any unique text you want. For example, ``attribute__from`` and
+``attribute__to`` would also work in this situation, as would ``attribute`` and
+``atribute__to`` (as the names are unique in the Python namespace).
+
 .. _python_style_apis_for_objc:
 
 Python-style APIs and methods for Objective-C objects
 -----------------------------------------------------
 
 For some standard Foundation classes, such as lists and dictionaries,
 Rubicon provides additional Python methods to make them behave more like their
@@ -124,15 +205,15 @@
 Strings
 ^^^^^^^
 
 :class:`~rubicon.objc.api.NSString` objects behave almost exactly like Python
 :class:`str` objects - they can be sliced, concatenated, compared, etc. with
 other Objective-C and Python strings.
 
-.. code-block:: python
+.. code-block:: pycon
 
     # Call an Objective-C method that returns a string.
     # We're using NSBundle to give us a string version of a path
     >>> NSBundle.mainBundle.bundlePath
     <ObjCStrInstance: __NSCFString at 0x114a94d68: /Users/brutus/path/to/somewhere>
 
     # Slice the Objective-C string
@@ -149,26 +230,26 @@
     in your code.
 
 If you have an :class:`~rubicon.objc.api.NSString`, and you need to pass it to
 a method that does a specific type check for :class:`str`, you can use
 ``str(nsstring)`` to convert the :class:`~rubicon.objc.api.NSString` to
 :class:`str`:
 
-.. code-block:: python
+.. code-block:: pycon
 
     # Convert the Objective-C string to a Python string.
     >>> str(NSBundle.mainBundle.bundlePath)
     '/Users/rkm/projects/beeware/venv3.6/bin'
 
 Conversely, if you have a :class:`str`, and you specifically require a
 :class:`~rubicon.objc.api.NSString`, you can use the
 :func:`~rubicon.objc.api.at` function to convert the Python instance to an
 :class:`~rubicon.objc.api.NSString`.
 
-.. code-block:: python
+.. code-block:: pycon
 
     >>> from rubicon.objc import at
     # Create a Python string
     >>> py_str = 'hello world'
     # Convert to an Objective-C string
     >>> at(py_str)
     <ObjCStrInstance: __NSCFString at 0x114a94e48: hello world>
@@ -177,15 +258,15 @@
 are available on :class:`str`, such as ``replace`` and ``split``. When these
 methods return a string, the implementation may return Python :class:`str` or
 Objective-C :class:`~rubicon.objc.api.NSString` instances. If you need to use
 the return value from these methods, you should always use :class:`str` or
 :func:`~rubicon.objc.api.at` to ensure that you have the right kind of string
 for your needs.
 
-.. code-block:: python
+.. code-block:: pycon
 
     # Is the path comprised of all lowercase letters? (Hint: it isn't)
     >>> NSBundle.mainBundle.bundlePath.islower()
     False
 
     # Convert string to lower case; use str() to ensure we get a Python string.
     >>> str(NSBundle.mainBundle.bundlePath.lower())
@@ -205,15 +286,15 @@
 Lists
 ^^^^^
 
 :class:`~rubicon.objc.api.NSArray` objects behave like any other Python
 sequence - they can be indexed, sliced, etc. and standard operations like
 :func:`len` and ``in`` are supported:
 
-.. code-block:: python
+.. code-block:: pycon
 
     >>> from rubicon.objc import NSArray
     >>> array = NSArray.arrayWithArray(list(range(4)))
     >>> array[0]
     0
     >>> array[1:3]
     <ObjCListInstance: _NSArrayI at 0x10b855208: <__NSArrayI 0x7f86f8e61950>(
@@ -237,15 +318,15 @@
     objects. This is an implementation detail - you should not refer to the
     ``ObjCListInstance`` and ``ObjCMutableListInstance`` classes explicitly in
     your code.
 
 :class:`~rubicon.objc.api.NSMutableArray` objects additionally support mutating
 operations, like item and slice assignment:
 
-.. code-block:: python
+.. code-block:: pycon
 
     >>> from rubicon.objc import NSMutableArray
     >>> mutarray = NSMutableArray.arrayWithArray(list(range(4)))
     >>> mutarray[0] = 42
     >>> mutarray
     <ObjCMutableListInstance: __NSArrayM at 0x10b8558d0: <__NSArrayM 0x7f86fb04d9f0>(
     42,
@@ -263,15 +344,15 @@
     7,
     3
     )
     >
 
 Sequence methods like ``index`` and ``pop`` are also supported:
 
-.. code-block:: python
+.. code-block:: pycon
 
     >>> mutarray.index(7)
     3
     >>> mutarray.pop(3)
     7
 
 .. note::
@@ -283,15 +364,15 @@
 Dictionaries
 ^^^^^^^^^^^^
 
 :class:`~rubicon.objc.api.NSDictionary` objects behave like any other Python
 mapping - their items can be accessed and standard operations like :func:`len`
 and ``in`` are supported:
 
-.. code-block:: python
+.. code-block:: pycon
 
     >>> from rubicon.objc import NSDictionary
     >>> d = objc.NSDictionary.dictionaryWithDictionary({"one": 1, "two": 2})
     >>> d["one"]
     1
     >>> len(d)
     >>> 2
@@ -309,28 +390,28 @@
     objects. This is an implementation detail - you should not refer to the
     ``ObjCDictInstance`` and ``ObjCMutableDictInstance`` classes explicitly in
     your code.
 
 :class:`~rubicon.objc.api.NSMutableDictionary` objects additionally support
 mutating operations, like item assignment:
 
-.. code-block:: python
+.. code-block:: pycon
 
     >>> md = objc.NSMutableDictionary.dictionaryWithDictionary({"one": 1, "two": 2})
     >>> md["three"] = 3
     >>> md
     <ObjCMutableDictInstance: __NSDictionaryM at 0x10b8a7860: {
         one = 1;
         three = 3;
         two = 2;
     }>
 
 Mapping methods like ``keys`` and ``values`` are also supported:
 
-.. code-block:: python
+.. code-block:: pycon
 
     >>> d.keys()
     <ObjCListInstance: __NSArrayI at 0x10b898a90: <__NSArrayI 0x7f86f8db6b70>(
     one,
     two
     )
     >
```

### Comparing `rubicon-objc-0.4.8/docs/index.rst` & `rubicon_objc-0.4.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.8/docs/make.bat` & `rubicon_objc-0.4.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.8/docs/reference/rubicon-objc-api.rst` & `rubicon_objc-0.4.9/docs/reference/rubicon-objc-api.rst`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.8/docs/reference/rubicon-objc-eventloop.rst` & `rubicon_objc-0.4.9/docs/reference/rubicon-objc-eventloop.rst`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.8/docs/reference/rubicon-objc-runtime.rst` & `rubicon_objc-0.4.9/docs/reference/rubicon-objc-runtime.rst`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.8/docs/reference/rubicon-objc-types.rst` & `rubicon_objc-0.4.9/docs/reference/rubicon-objc-types.rst`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.8/docs/reference/rubicon-objc.rst` & `rubicon_objc-0.4.9/docs/reference/rubicon-objc.rst`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.8/docs/tutorial/tutorial-1.rst` & `rubicon_objc-0.4.9/docs/tutorial/tutorial-1.rst`

 * *Files 7% similar despite different names*

```diff
@@ -48,24 +48,34 @@
 
     >>> full = NSURL.URLWithString("contributing/", relativeToURL=base)
 
 The second argument (``relativeToURL``) is accessed as a keyword argument. This
 argument is declared as being of type ``NSURL *``; since ``base`` is an
 instance of ``NSURL``, Rubicon can pass through this instance.
 
-Sometimes, an Objective-C method definition will use the same keyword
-argument name twice. This is legal in Objective-C, but not in Python, as you
-can't repeat a keyword argument in a method call. In this case, you can use a
-"long form" of the method to explicitly invoke a descriptor by replacing
-colons with underscores:
+Sometimes, an Objective-C method definition will use the same keyword argument
+name twice (for example, ``NSLayoutConstraint`` has a
+``+constraintWithItem:attribute:relatedBy:toItem:attribute:multiplier:constant:``
+selector, using the ``attribute`` keyword twice). This is legal in Objective-C,
+but not in Python, as you can't repeat a keyword argument in a method call. In
+this case, you can use a ``__`` suffix on the ambiguous keyword argument to make
+it unique. Any content after and including the ``__`` will be stripped when
+making the Objective-C call:
 
 .. code-block:: pycon
 
-    >>> base = NSURL.URLWithString_("https://beeware.org/")
-    >>> full = NSURL.URLWithString_relativeToURL_("contributing", base)
+    >>> constraint = NSLayoutConstraint.constraintWithItem(
+    ...     first_item,
+    ...     attribute__1=first_attribute,
+    ...     relatedBy=relation,
+    ...     toItem=second_item,
+    ...     attribute__2=second_attribute,
+    ...     multiplier=2.0,
+    ...     constant=1.0
+    ... )
 
 Instance methods
 ================
 
 So far, we've been using the ``+URLWithString:`` static constructor. However,
 ``NSURL`` also provides an initializer method ``-initWithString:``. To use this
 method, you first have to instruct the Objective-C runtime to allocate memory
```

### Comparing `rubicon-objc-0.4.8/docs/tutorial/tutorial-2.rst` & `rubicon_objc-0.4.9/docs/tutorial/tutorial-2.rst`

 * *Files 0% similar despite different names*

```diff
@@ -129,14 +129,15 @@
 .. code-block:: pycon
 
     >>> class Handler(NSObject, auto_rename=True):
     ...     pass
 
 If this option is used, the Objective C class name will have a numeric suffix
 (e.g., `Handler_2`). The Python class name will be unchanged.
+
 What, no ``__init__()``?
 ========================
 
 You'll also notice that our example code *doesn't* have an ``__init__()``
 method like you'd normally expect of Python code. As we're defining an
 Objective-C class, we need to follow the Objective-C object life cycle - which
 means defining initializer methods that are visible to the Objective-C runtime,
```

### Comparing `rubicon-objc-0.4.8/pyproject.toml` & `rubicon_objc-0.4.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [build-system]
 requires = [
-    "setuptools==69.2.0",
+    "setuptools==69.5.1",
     "setuptools_scm==8.0.4",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 dynamic = ["version"]
 name = "rubicon-objc"
@@ -47,29 +47,29 @@
 Source = "https://github.com/beeware/rubicon-objc"
 
 [project.optional-dependencies]
 dev = [
     # Pre-commit 3.6.0 deprecated support for Python 3.8
     "pre-commit == 3.5.0 ; python_version < '3.9'",
     "pre-commit == 3.7.0 ; python_version >= '3.9'",
-    "pytest == 8.1.1",
+    "pytest == 8.2.0",
     "pytest-tldr == 0.2.5",
     "setuptools_scm == 8.0.4",
-    "tox == 4.14.2",
+    "tox == 4.15.0",
 ]
 docs = [
-    "furo == 2024.1.29",
+    "furo == 2024.4.27",
     "pyenchant == 3.2.2",
     # Sphinx 7.2 deprecated support for Python 3.8
     "sphinx == 7.1.2 ; python_version < '3.9'",
-    "sphinx == 7.2.6 ; python_version >= '3.9'",
+    "sphinx == 7.3.7 ; python_version >= '3.9'",
     "sphinx_tabs == 3.4.5",
     # Sphinx 2024.2.4 deprecated support for Python 3.8
     "sphinx-autobuild == 2021.3.14 ; python_version < '3.9'",
-    "sphinx-autobuild == 2024.2.4 ; python_version >= '3.9'",
+    "sphinx-autobuild == 2024.4.16 ; python_version >= '3.9'",
     "sphinx-copybutton == 0.5.2",
     "sphinxcontrib-spelling == 8.0.0",
 ]
 
 [tool.codespell]
 skip = ".git,*.pdf,*.svg"
 # the way to make case sensitive skips of words etc
```

### Comparing `rubicon-objc-0.4.8/src/rubicon/objc/__init__.py` & `rubicon_objc-0.4.9/src/rubicon/objc/__init__.py`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.8/src/rubicon/objc/api.py` & `rubicon_objc-0.4.9/src/rubicon/objc/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,36 +242,40 @@
         self.name_start = name_start
         self.methods = {}  # Initialized in ObjCClass._load_methods
 
     def __repr__(self):
         return f"{type(self).__qualname__}({self.name_start!r})"
 
     def __call__(self, receiver, first_arg=_sentinel, **kwargs):
+        # Ignore parts of argument names after "__".
+        order = tuple(argname.split("__")[0] for argname in kwargs)
+        args = [arg for arg in kwargs.values()]
+
         if first_arg is ObjCPartialMethod._sentinel:
             if kwargs:
                 raise TypeError("Missing first (positional) argument")
-
-            args = []
-            rest = frozenset()
+            rest = order
         else:
-            args = [first_arg]
-            # Add "" to rest to indicate that the method takes arguments
-            rest = frozenset(kwargs) | frozenset(("",))
+            args.insert(0, first_arg)
+            rest = ("",) + order
 
         try:
-            name, order = self.methods[rest]
+            name = self.methods[rest]
         except KeyError:
+            if first_arg is self._sentinel:
+                specified_sel = self.name_start
+            else:
+                specified_sel = f"{self.name_start}:{':'.join(kwargs.keys())}:"
             raise ValueError(
-                f"No method was found starting with {self.name_start!r} and with keywords {set(kwargs)}\n"
-                f"Known keywords are:\n"
-                + "\n".join(repr(keywords) for keywords in self.methods)
-            )
+                f"Invalid selector {specified_sel}. Available selectors are: "
+                f"{', '.join(sel for sel in self.methods.values())}"
+            ) from None
 
         meth = receiver.objc_class._cache_method(name)
-        args += [kwargs[name] for name in order]
+
         return meth(receiver, *args)
 
 
 class ObjCBoundMethod:
     """This represents an Objective-C method (an IMP) which has been bound to
     some id which will be passed as the first parameter to the method.
     """
@@ -1031,36 +1035,19 @@
           the attribute name and the keyword arguments passed to the returned
           method. For example, the Objective-C method call ``[self initWithRed:r
           green:g blue:b]`` translates to ``self.initWithRed(r, green=g,
           blue=b)``.
 
         The "interleaved" syntax is usually preferred, since it looks more
         similar to normal Objective-C syntax. However, the "flat" syntax is also
-        fully supported. Certain method names require the "flat" syntax, for
-        example if two arguments have the same label (e.g.
-        ``performSelector:withObject:withObject:``), which is not supported by
-        Python's keyword argument syntax.
-
-        .. warning::
-
-            The "interleaved" syntax currently ignores the ordering of its
-            keyword arguments. However, in the interest of readability, the
-            keyword arguments should always be passed in the same order as they
-            appear in the method name.
-
-            This also means that two methods whose names which differ only in
-            the ordering of their keywords will conflict with each other, and
-            can only be called reliably using "flat" syntax.
-
-            As of Python 3.6, the order of keyword arguments passed to functions
-            is preserved (:pep:`468`). In the future, once Rubicon requires
-            Python 3.6 or newer, "interleaved" method calls will respect keyword
-            argument order. This will fix the kind of conflict described above,
-            but will also disallow specifying the keyword arguments out of
-            order.
+        fully supported. If two arguments have the same name (e.g.
+        ``performSelector:withObject:withObject:``), you can use ``__`` in the
+        keywords to disambiguate (e.g., ``performSelector(..., withObject__1=...,
+        withObject__2=...)``. Any content after and including the ``__`` in an argument
+        will be ignored.
         """
         # Search for named instance method in the class object and if it
         # exists, return callable object with self as hidden argument.
         # Note: you should give self and not self.ptr as a parameter to
         # ObjCBoundMethod, so that it will be able to keep the ObjCInstance
         # alive for chained calls like MyClass.alloc().init() where the
         # object created by alloc() is not assigned to a variable.
@@ -1086,15 +1073,15 @@
                     method = cls.partial_methods[name]
                     break
                 except KeyError:
                     cls = cls.superclass
         else:
             method = None
 
-        if method is None or set(method.methods) == {frozenset()}:
+        if method is None or set(method.methods) == {()}:
             # Find a method whose full name matches the given name if no partial
             # method was found, or the partial method can only resolve to a
             # single method that takes no arguments. The latter case avoids
             # returning partial methods in cases where a regular method works
             # just as well.
             method = self.objc_class._cache_method(name.replace("_", ":"))
 
@@ -1650,28 +1637,31 @@
                 partial.methods.update(superpartial.methods)
 
         for i in range(methods_ptr_count.value):
             method = methods_ptr[i]
             name = libobjc.method_getName(method).name.decode("utf-8")
             self.instance_method_ptrs[name] = method
 
-            first, *rest = name.split(":")
-            # Selectors end in a colon iff the method takes arguments.
-            # Because of this, rest must either be empty (method takes no arguments)
-            # or the last element must be an empty string (method takes arguments).
-            assert not rest or rest[-1] == ""
+            # Selectors end with a colon if the method takes arguments.
+            if name.endswith(":"):
+                first, *rest, _ = name.split(":")
+                # Insert an empty string in order to indicate that the method
+                # takes a first argument as a positional argument.
+                rest.insert(0, "")
+                rest = tuple(rest)
+            else:
+                first = name
+                rest = ()
 
             try:
                 partial = self.partial_methods[first]
             except KeyError:
                 partial = self.partial_methods[first] = ObjCPartialMethod(first)
 
-            # order is rest without the dummy "" part
-            order = rest[:-1]
-            partial.methods[frozenset(rest)] = (name, order)
+            partial.methods[rest] = name
 
         # Set the list of methods for the class to the computed list.
         self.methods_ptr = methods_ptr
 
 
 class ObjCMetaClass(ObjCClass):
     """Python wrapper for an Objective-C metaclass.
```

### Comparing `rubicon-objc-0.4.8/src/rubicon/objc/collections.py` & `rubicon_objc-0.4.9/src/rubicon/objc/collections.py`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.8/src/rubicon/objc/ctypes_patch.py` & `rubicon_objc-0.4.9/src/rubicon/objc/ctypes_patch.py`

 * *Files 20% similar despite different names*

```diff
@@ -61,40 +61,14 @@
     ("tp_basicsize", ctypes.c_ssize_t),
     ("tp_itemsize", ctypes.c_ssize_t),
     # There are many more fields, but we're only interested in the size fields,
     # so we can leave out everything else.
 ]
 
 
-# The PyTypeObject structure for the dict class.
-# This is used to determine the size of the PyDictObject structure.
-PyDict_Type = PyTypeObject.from_address(id(dict))
-
-
-# The PyDictObject structure from "Include/dictobject.h". This structure is not
-# stable across Python versions, and did indeed change in recent Python
-# releases. Because we only care about the size of the structure and not its
-# actual contents, we can declare it as an opaque byte array, with the length
-# taken from PyDict_Type.
-class PyDictObject(ctypes.Structure):
-    _fields_ = [
-        ("PyDictObject_opaque", (ctypes.c_ubyte * PyDict_Type.tp_basicsize)),
-    ]
-
-
-# The mappingproxyobject struct from "Objects/descrobject.c". This structure is
-# not officially stable across Python versions, but its layout hasn't changed
-# since 2001.
-class mappingproxyobject(ctypes.Structure):
-    _fields_ = [
-        ("ob_base", PyObject),
-        ("mapping", ctypes.py_object),
-    ]
-
-
 # The ffi_type structure from libffi's "include/ffi.h". This is a forward
 # declaration, because the structure contains pointers to itself.
 class ffi_type(ctypes.Structure):
     pass
 
 
 ffi_type._fields_ = [
@@ -111,76 +85,158 @@
 # around a ctypes bug (https://github.com/python/cpython/issues/81061). See the comment
 # in make_callback_returnable's setfunc for details.
 SETFUNC = ctypes.PYFUNCTYPE(
     ctypes.c_void_p, ctypes.c_void_p, ctypes.py_object, ctypes.c_ssize_t
 )
 
 
-# The StgDictObject structure from "Modules/_ctypes/ctypes.h". This structure is
-# not officially stable across Python versions, but it basically hasn't changed
-# since ctypes was originally added to Python in 2009.
-class StgDictObject(ctypes.Structure):
-    _fields_ = [
-        ("dict", PyDictObject),
-        ("size", ctypes.c_ssize_t),
-        ("align", ctypes.c_ssize_t),
-        ("length", ctypes.c_ssize_t),
-        ("ffi_type_pointer", ffi_type),
-        ("proto", ctypes.py_object),
-        ("setfunc", SETFUNC),
-        ("getfunc", GETFUNC),
-        # There are a few more fields, but we leave them out again because we don't need them.
-    ]
-
-
-ctypes.pythonapi.Py_IncRef.restype = None
-ctypes.pythonapi.Py_IncRef.argtypes = [ctypes.POINTER(PyObject)]
-
-
-def unwrap_mappingproxy(proxy):
-    """Return the mapping contained in a mapping proxy object."""
+if sys.version_info < (3, 13):
+    # The PyTypeObject structure for the dict class.
+    # This is used to determine the size of the PyDictObject structure.
+    PyDict_Type = PyTypeObject.from_address(id(dict))
+
+    # The PyDictObject structure from "Include/dictobject.h". This structure is not
+    # stable across Python versions, and did indeed change in recent Python
+    # releases. Because we only care about the size of the structure and not its
+    # actual contents, we can declare it as an opaque byte array, with the length
+    # taken from PyDict_Type.
+    class PyDictObject(ctypes.Structure):
+        _fields_ = [
+            ("PyDictObject_opaque", (ctypes.c_ubyte * PyDict_Type.tp_basicsize)),
+        ]
+
+    # The StgDictObject structure from "Modules/_ctypes/ctypes.h". This structure is
+    # not officially stable across Python versions, but it didn't change between being
+    # introduced in 2009, and being replaced in 2024/Python 3.13.0a6.
+    class StgDictObject(ctypes.Structure):
+        _fields_ = [
+            ("dict", PyDictObject),
+            ("size", ctypes.c_ssize_t),
+            ("align", ctypes.c_ssize_t),
+            ("length", ctypes.c_ssize_t),
+            ("ffi_type_pointer", ffi_type),
+            ("proto", ctypes.py_object),
+            ("setfunc", SETFUNC),
+            ("getfunc", GETFUNC),
+            # There are a few more fields, but we leave them out again because
+            # we don't need them.
+        ]
+
+    # The mappingproxyobject struct from "Objects/descrobject.c". This structure is
+    # not officially stable across Python versions, but its layout hasn't changed
+    # since 2001.
+    class mappingproxyobject(ctypes.Structure):
+        _fields_ = [
+            ("ob_base", PyObject),
+            ("mapping", ctypes.py_object),
+        ]
+
+    def unwrap_mappingproxy(proxy):
+        """Return the mapping contained in a mapping proxy object."""
+
+        if not isinstance(proxy, types.MappingProxyType):
+            raise TypeError(
+                "Expected a mapping proxy object, not "
+                f"{type(proxy).__module__}.{type(proxy).__qualname__}"
+            )
 
-    if not isinstance(proxy, types.MappingProxyType):
-        raise TypeError(
-            f"Expected a mapping proxy object, not {type(proxy).__module__}.{type(proxy).__qualname__}"
-        )
+        return mappingproxyobject.from_address(id(proxy)).mapping
 
-    return mappingproxyobject.from_address(id(proxy)).mapping
+    def get_stgdict_of_type(tp):
+        """Return the given ctypes type's StgDict object. If the object's dict is
+        not a StgDict, an error is raised.
+
+        This function is roughly equivalent to the PyType_stgdict function in the
+        ctypes source code. We cannot use that function directly, because it is not
+        part of CPython's public C API, and thus not accessible on some systems (see
+        #113).
+        """
+
+        if not isinstance(tp, type):
+            raise TypeError(
+                "Expected a type object, not "
+                f"{type(tp).__module__}.{type(tp).__qualname__}"
+            )
 
+        stgdict = tp.__dict__
+        if isinstance(stgdict, types.MappingProxyType):
+            # If the type's __dict__ is wrapped in a mapping proxy, we need to
+            # unwrap it. (This appears to always be the case, so the isinstance
+            # check above could perhaps be left out, but it doesn't hurt to check.)
+            stgdict = unwrap_mappingproxy(stgdict)
+
+        # The StgDict type is not publicly exposed anywhere, so we can't use
+        # isinstance. Checking the name is the best we can do here.
+        if type(stgdict).__name__ != "StgDict":
+            raise TypeError(
+                "The given type's dict must be a StgDict, not "
+                f"{type(stgdict).__module__}.{type(stgdict).__qualname__}"
+            )
 
-def get_stgdict_of_type(tp):
-    """Return the given ctypes type's StgDict object. If the object's dict is
-    not a StgDict, an error is raised.
+        return StgDictObject.from_address(id(stgdict))
 
-    This function is roughly equivalent to the PyType_stgdict function in the
-    ctypes source code. We cannot use that function directly, because it is not
-    part of CPython's public C API, and thus not accessible on some systems (see
-    #113).
-    """
+else:
+    # In Python 3.13.0a6 (https://github.com/python/cpython/issues/114314),
+    # StgDict was replaced with a new StgInfo data type that requires less
+    # metaclass magic.
+
+    class StgInfo(ctypes.Structure):
+        _fields_ = [
+            ("initialized", ctypes.c_int),
+            ("size", ctypes.c_ssize_t),
+            ("align", ctypes.c_ssize_t),
+            ("length", ctypes.c_ssize_t),
+            ("ffi_type_pointer", ffi_type),
+            ("proto", ctypes.py_object),
+            ("setfunc", SETFUNC),
+            ("getfunc", GETFUNC),
+            # There are a few more fields, but we leave them out again because
+            # we don't need them.
+        ]
+
+    # void *PyObject_GetTypeData(PyObject *o, PyTypeObject *cls);
+    ctypes.pythonapi.PyObject_GetTypeData.restype = ctypes.c_void_p
+    ctypes.pythonapi.PyObject_GetTypeData.argtypes = [ctypes.c_void_p, ctypes.c_void_p]
+
+    def get_stginfo_of_type(tp):
+        """Return the given ctypes type's StgInfo object.
+
+        This function is roughly equivalent to the PyStgInfo_FromType function in the
+        ctypes source code. We cannot use that function directly, because it is not
+        part of CPython's public C API, and thus not accessible).
+        """
+        # Original code:
+        #     if (!PyObject_IsInstance((PyObject *)type, (PyObject *)state->PyCType_Type))
+        if not isinstance(tp, type(ctypes.Structure).__base__):
+            raise TypeError(
+                "Expected a ctypes structure type, "
+                f"not {type(tp).__module__}.{type(tp).__qualname__}"
+            )
 
-    if not isinstance(tp, type):
-        raise TypeError(
-            f"Expected a type object, not {type(tp).__module__}.{type(tp).__qualname__}"
+        # tp is the Python representation of the type. The StgInfo struct is the
+        # type data stored on ctypes.CType_Type (which is the base class of
+        # ctypes.Structure).
+        # Original code:
+        #     StgInfo *info = PyObject_GetTypeData((PyObject *)type, state->PyCType_Type);
+        info = ctypes.pythonapi.PyObject_GetTypeData(
+            id(tp),
+            id(type(ctypes.Structure).__base__),
         )
+        result = StgInfo.from_address(info)
+        if not result.initialized:
+            raise TypeError(
+                f"{type(tp).__module__}.{type(tp).__qualname__} has not been "
+                "initialized; it may be an abstract class"
+            )
 
-    stgdict = tp.__dict__
-    if isinstance(stgdict, types.MappingProxyType):
-        # If the type's __dict__ is wrapped in a mapping proxy, we need to
-        # unwrap it. (This appears to always be the case, so the isinstance
-        # check above could perhaps be left out, but it doesn't hurt to check.)
-        stgdict = unwrap_mappingproxy(stgdict)
-
-    # The StgDict type is not publicly exposed anywhere, so we can't use
-    # isinstance. Checking the name is the best we can do here.
-    if type(stgdict).__name__ != "StgDict":
-        raise TypeError(
-            f"The given type's dict must be a StgDict, not {type(stgdict).__module__}.{type(stgdict).__qualname__}"
-        )
+        return result
 
-    return stgdict
+
+ctypes.pythonapi.Py_IncRef.restype = None
+ctypes.pythonapi.Py_IncRef.argtypes = [ctypes.POINTER(PyObject)]
 
 
 def make_callback_returnable(ctype):
     """Modify the given ctypes type so it can be returned from a callback
     function.
 
     This function may be used as a decorator on a struct/union declaration.
@@ -189,24 +245,26 @@
     is invoked on a type.
     """
     # The presence of the _rubicon_objc_ctypes_patch_getfunc attribute is a
     # sentinel for whether the type has been modified previously.
     if hasattr(ctype, "_rubicon_objc_ctypes_patch_getfunc"):
         return ctype
 
-    # Extract the StgDict from the ctype.
-    stgdict = get_stgdict_of_type(ctype)
-    stgdict_c = StgDictObject.from_address(id(stgdict))
+    # The implementation changed in 3.13.0a6; StgDict was replaced with StgInfo
+    if sys.version_info < (3, 13):
+        stg = get_stgdict_of_type(ctype)
+    else:
+        stg = get_stginfo_of_type(ctype)
 
     # Ensure that there is no existing getfunc or setfunc on the stgdict.
-    if ctypes.cast(stgdict_c.getfunc, ctypes.c_void_p).value is not None:
+    if ctypes.cast(stg.getfunc, ctypes.c_void_p).value is not None:
         raise ValueError(
             f"The ctype {ctype.__module__}.{ctype.__name__} already has a getfunc"
         )
-    elif ctypes.cast(stgdict_c.setfunc, ctypes.c_void_p).value is not None:
+    elif ctypes.cast(stg.setfunc, ctypes.c_void_p).value is not None:
         raise ValueError(
             f"The ctype {ctype.__module__}.{ctype.__name__} already has a setfunc"
         )
 
     # Define the getfunc and setfunc.
     @GETFUNC
     def getfunc(ptr, size):
@@ -244,13 +302,14 @@
         # otherwise ctypes won't recognize it and will raise a TypeError.
         return ctypes.cast(none_ptr, ctypes.c_void_p).value
 
     # Store the getfunc and setfunc as attributes on the ctype, so they don't
     # get garbage-collected.
     ctype._rubicon_objc_ctypes_patch_getfunc = getfunc
     ctype._rubicon_objc_ctypes_patch_setfunc = setfunc
-    # Put the getfunc and setfunc into the stgdict fields.
-    stgdict_c.getfunc = getfunc
-    stgdict_c.setfunc = setfunc
+
+    # Put the getfunc and setfunc into the stg fields.
+    stg.getfunc = getfunc
+    stg.setfunc = setfunc
 
     # Return the passed in ctype, so this function can be used as a decorator.
     return ctype
```

### Comparing `rubicon-objc-0.4.8/src/rubicon/objc/eventloop.py` & `rubicon_objc-0.4.9/src/rubicon/objc/eventloop.py`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.8/src/rubicon/objc/runtime.py` & `rubicon_objc-0.4.9/src/rubicon/objc/runtime.py`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.8/src/rubicon/objc/types.py` & `rubicon_objc-0.4.9/src/rubicon/objc/types.py`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.8/src/rubicon_objc.egg-info/PKG-INFO` & `rubicon_objc-0.4.9/src/rubicon_objc.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubicon-objc
-Version: 0.4.8
+Version: 0.4.9
 Summary: A bridge between an Objective C runtime environment and Python.
 Author-email: Russell Keith-Magee <russell@keith-magee.com>
 Maintainer-email: BeeWare Team <team@beeware.org>
 License: New BSD
 Project-URL: Homepage, https://beeware.org/rubicon
 Project-URL: Funding, https://beeware.org/contributing/membership/
 Project-URL: Documentation, https://rubicon-objc.readthedocs.io/en/latest/
@@ -26,60 +26,64 @@
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Provides-Extra: dev
 Requires-Dist: pre-commit==3.5.0; python_version < "3.9" and extra == "dev"
 Requires-Dist: pre-commit==3.7.0; python_version >= "3.9" and extra == "dev"
-Requires-Dist: pytest==8.1.1; extra == "dev"
+Requires-Dist: pytest==8.2.0; extra == "dev"
 Requires-Dist: pytest-tldr==0.2.5; extra == "dev"
 Requires-Dist: setuptools_scm==8.0.4; extra == "dev"
-Requires-Dist: tox==4.14.2; extra == "dev"
+Requires-Dist: tox==4.15.0; extra == "dev"
 Provides-Extra: docs
-Requires-Dist: furo==2024.1.29; extra == "docs"
+Requires-Dist: furo==2024.4.27; extra == "docs"
 Requires-Dist: pyenchant==3.2.2; extra == "docs"
 Requires-Dist: sphinx==7.1.2; python_version < "3.9" and extra == "docs"
-Requires-Dist: sphinx==7.2.6; python_version >= "3.9" and extra == "docs"
+Requires-Dist: sphinx==7.3.7; python_version >= "3.9" and extra == "docs"
 Requires-Dist: sphinx_tabs==3.4.5; extra == "docs"
 Requires-Dist: sphinx-autobuild==2021.3.14; python_version < "3.9" and extra == "docs"
-Requires-Dist: sphinx-autobuild==2024.2.4; python_version >= "3.9" and extra == "docs"
+Requires-Dist: sphinx-autobuild==2024.4.16; python_version >= "3.9" and extra == "docs"
 Requires-Dist: sphinx-copybutton==0.5.2; extra == "docs"
 Requires-Dist: sphinxcontrib-spelling==8.0.0; extra == "docs"
 
-.. image:: https://beeware.org/project/projects/bridges/rubicon/rubicon.png
+.. |logo| image:: https://beeware.org/project/projects/bridges/rubicon/rubicon.png
     :width: 72px
     :target: https://beeware.org/rubicon
 
-Rubicon-ObjC
-============
-
-.. image:: https://img.shields.io/pypi/pyversions/rubicon-objc.svg
+.. |pyversions| image:: https://img.shields.io/pypi/pyversions/rubicon-objc.svg
    :target: https://pypi.python.org/pypi/rubicon-objc
    :alt: Python Versions
 
-.. image:: https://img.shields.io/pypi/v/rubicon-objc.svg
+.. |version| image:: https://img.shields.io/pypi/v/rubicon-objc.svg
    :target: https://pypi.python.org/pypi/rubicon-objc
    :alt: Project Version
 
-.. image:: https://img.shields.io/pypi/status/rubicon-objc.svg
+.. |maturity| image:: https://img.shields.io/pypi/status/rubicon-objc.svg
    :target: https://pypi.python.org/pypi/rubicon-objc
    :alt: Project status
 
-.. image:: https://img.shields.io/pypi/l/rubicon-objc.svg
+.. |license| image:: https://img.shields.io/pypi/l/rubicon-objc.svg
    :target: https://github.com/beeware/rubicon-objc/blob/main/LICENSE
    :alt: License
 
-.. image:: https://github.com/beeware/rubicon-objc/workflows/CI/badge.svg?branch=main
+.. |ci| image:: https://github.com/beeware/rubicon-objc/workflows/CI/badge.svg?branch=main
    :target: https://github.com/beeware/rubicon-objc/actions
    :alt: Build Status
 
-.. image:: https://img.shields.io/discord/836455665257021440?label=Discord%20Chat&logo=discord&style=plastic
+.. |social| image:: https://img.shields.io/discord/836455665257021440?label=Discord%20Chat&logo=discord&style=plastic
    :target: https://beeware.org/bee/chat/
    :alt: Discord server
 
+|logo|
+
+Rubicon-ObjC
+============
+
+|pyversions| |version| |maturity| |license| |ci| |social|
+
 Rubicon-ObjC is a bridge between Objective-C and Python. It enables you to:
 
 * Use Python to instantiate objects defined in Objective-C,
 * Use Python to invoke methods on objects defined in Objective-C, and
 * Subclass and extend Objective-C classes in Python.
 
 It also includes wrappers of the some key data types from the Foundation
```

### Comparing `rubicon-objc-0.4.8/src/rubicon_objc.egg-info/SOURCES.txt` & `rubicon_objc-0.4.9/src/rubicon_objc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.8/tests/objc/BaseExample.h` & `rubicon_objc-0.4.9/tests/objc/BaseExample.h`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.8/tests/objc/BaseExample.m` & `rubicon_objc-0.4.9/tests/objc/BaseExample.m`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.8/tests/objc/Blocks.h` & `rubicon_objc-0.4.9/tests/objc/Blocks.h`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.8/tests/objc/Blocks.m` & `rubicon_objc-0.4.9/tests/objc/Blocks.m`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.8/tests/objc/DescriptionTester.m` & `rubicon_objc-0.4.9/tests/objc/DescriptionTester.m`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.8/tests/objc/Example.h` & `rubicon_objc-0.4.9/tests/objc/Example.h`

 * *Files 20% similar despite different names*

```diff
@@ -99,14 +99,18 @@
 -(void) testPeek:(int) value;
 -(NSString *) getMessage;
 -(NSString *) reverseIt:(NSString *) input;
 
 +(NSUInteger) overloaded;
 +(NSUInteger) overloaded:(NSUInteger)arg1;
 +(NSUInteger) overloaded:(NSUInteger)arg1 extraArg:(NSUInteger)arg2;
++(NSUInteger) overloaded:(NSUInteger)arg1 extraArg1:(NSUInteger)arg2 extraArg2:(NSUInteger)arg3;
++(NSUInteger) overloaded:(NSUInteger)arg1 extraArg2:(NSUInteger)arg2 extraArg1:(NSUInteger)arg3;
++(NSUInteger) overloaded:(NSUInteger)arg1 orderedArg1:(NSUInteger)arg2 orderedArg2:(NSUInteger)arg3;
++(NSUInteger) overloaded:(NSUInteger)arg1 duplicateArg:(NSUInteger)arg2 duplicateArg:(NSUInteger)arg3;
 
 +(struct complex) doStuffWithStruct:(struct simple)simple;
 
 -(id) processDictionary:(NSDictionary *) dict;
 -(id) processArray:(NSArray *) dict;
 
 -(NSSize) testThing:(int) value;
```

### Comparing `rubicon-objc-0.4.8/tests/objc/Example.m` & `rubicon_objc-0.4.9/tests/objc/Example.m`

 * *Files 13% similar despite different names*

```diff
@@ -237,14 +237,34 @@
 }
 
 +(NSUInteger) overloaded:(NSUInteger)arg1 extraArg:(NSUInteger)arg2
 {
     return arg1 + arg2;
 }
 
++(NSUInteger) overloaded:(NSUInteger)arg1 extraArg1:(NSUInteger)arg2 extraArg2:(NSUInteger)arg3
+{
+    return arg1 + arg2 + arg3;
+}
+
++(NSUInteger) overloaded:(NSUInteger)arg1 extraArg2:(NSUInteger)arg2 extraArg1:(NSUInteger)arg3
+{
+    return arg1 * arg2 * arg3;
+}
+
++(NSUInteger) overloaded:(NSUInteger)arg1 orderedArg1:(NSUInteger)arg2 orderedArg2:(NSUInteger)arg3
+{
+    return 0;
+}
+
++(NSUInteger) overloaded:(NSUInteger)arg1 duplicateArg:(NSUInteger)arg2 duplicateArg:(NSUInteger)arg3
+{
+    return arg1 + 2 * arg2 + 3 * arg3;
+}
+
 +(struct complex) doStuffWithStruct:(struct simple)simple
 {
     return (struct complex){
         .things = {1, 2, 3, 4},
         .callback = NULL,
         .s = simple,
         .next = NULL,
```

### Comparing `rubicon-objc-0.4.8/tests/objc/Makefile` & `rubicon_objc-0.4.9/tests/objc/Makefile`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.8/tests/objc/Thing.m` & `rubicon_objc-0.4.9/tests/objc/Thing.m`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.8/tests/test_NSArray.py` & `rubicon_objc-0.4.9/tests/test_NSArray.py`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.8/tests/test_NSDictionary.py` & `rubicon_objc-0.4.9/tests/test_NSDictionary.py`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.8/tests/test_NSString.py` & `rubicon_objc-0.4.9/tests/test_NSString.py`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.8/tests/test_async.py` & `rubicon_objc-0.4.9/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.8/tests/test_blocks.py` & `rubicon_objc-0.4.9/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.8/tests/test_core.py` & `rubicon_objc-0.4.9/tests/test_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -982,14 +982,42 @@
             encoding=4,  # NSUTF8StringEncoding
             options=0,
             range=NSRange(0, 7),
             remainingRange=byref(remaining),
         )
         self.assertEqual(buf.value.decode("utf-8"), pystring)
 
+    def test_partial_method_arg_order(self):
+        Example = ObjCClass("Example")
+
+        self.assertEqual(Example.overloaded(3, extraArg1=5, extraArg2=7), 3 + 5 + 7)
+        self.assertEqual(Example.overloaded(3, extraArg2=5, extraArg1=7), 3 * 5 * 7)
+
+        # Although the arguments are a unique match, they're not in the right order.
+        with self.assertRaises(ValueError):
+            Example.overloaded(0, orderedArg2=0, orderedArg1=0)
+
+    def test_partial_method_duplicate_arg_names(self):
+        Example = ObjCClass("Example")
+        self.assertEqual(
+            Example.overloaded(24, duplicateArg__a=16, duplicateArg__b=6),
+            24 + 2 * 16 + 3 * 6,
+        )
+
+    def test_partial_method_exception(self):
+        Example = ObjCClass("Example")
+        with self.assertRaisesRegex(
+            ValueError,
+            "Invalid selector overloaded:invalidArgument:. Available selectors are: "
+            "overloaded, overloaded:, overloaded:extraArg:, "
+            "overloaded:extraArg1:extraArg2:, overloaded:extraArg2:extraArg1:, "
+            "overloaded:orderedArg1:orderedArg2:, overloaded:duplicateArg:duplicateArg:",
+        ):
+            Example.overloaded(0, invalidArgument=0)
+
     def test_objcmethod_str_repr(self):
         """Test ObjCMethod, ObjCPartialMethod, and ObjCBoundMethod str and repr"""
 
         obj = NSObject.new()
 
         # ObjCMethod
         self.assertEqual(repr(obj.init.method), "<ObjCMethod: init @16@0:8>")
```

### Comparing `rubicon-objc-0.4.8/tests/test_ctypes_patch.py` & `rubicon_objc-0.4.9/tests/test_ctypes_patch.py`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.8/tox.ini` & `rubicon_objc-0.4.9/tox.ini`

 * *Files identical despite different names*


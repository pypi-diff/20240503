# Comparing `tmp/rosdistro-0.9.0.tar.gz` & `tmp/rosdistro-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rosdistro-0.9.0.tar", last modified: Fri Jun 10 18:20:34 2022, max compression
+gzip compressed data, was "rosdistro-0.9.1.tar", last modified: Fri May  3 19:22:15 2024, max compression
```

## Comparing `rosdistro-0.9.0.tar` & `rosdistro-0.9.1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 18:20:34.000000 rosdistro-0.9.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 18:20:34.000000 rosdistro-0.9.0/scripts/
--rwxr-xr-x   0 root         (0) root         (0)     4192 2021-12-03 00:40:00.000000 rosdistro-0.9.0/scripts/rosdistro_build_cache
--rwxr-xr-x   0 root         (0) root         (0)     4186 2021-12-03 00:40:00.000000 rosdistro-0.9.0/scripts/rosdistro_freeze_source
--rwxr-xr-x   0 root         (0) root         (0)     5980 2021-12-03 00:40:00.000000 rosdistro-0.9.0/scripts/rosdistro_migrate_to_rep_141
--rwxr-xr-x   0 root         (0) root         (0)     1176 2021-12-03 00:40:00.000000 rosdistro-0.9.0/scripts/rosdistro_migrate_to_rep_143
--rwxr-xr-x   0 root         (0) root         (0)     2641 2021-12-03 00:40:00.000000 rosdistro-0.9.0/scripts/rosdistro_reformat
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 18:20:34.000000 rosdistro-0.9.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 18:20:34.000000 rosdistro-0.9.0/src/rosdistro/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 18:20:34.000000 rosdistro-0.9.0/src/rosdistro/external/
--rw-r--r--   0 root         (0) root         (0)        0 2021-12-03 00:40:00.000000 rosdistro-0.9.0/src/rosdistro/external/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21043 2021-12-03 00:40:00.000000 rosdistro-0.9.0/src/rosdistro/external/appdirs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 18:20:34.000000 rosdistro-0.9.0/src/rosdistro/manifest_provider/
--rw-r--r--   0 root         (0) root         (0)     1874 2021-12-03 00:40:00.000000 rosdistro-0.9.0/src/rosdistro/manifest_provider/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3554 2021-12-03 00:40:00.000000 rosdistro-0.9.0/src/rosdistro/manifest_provider/bitbucket.py
--rw-r--r--   0 root         (0) root         (0)     6112 2021-12-03 00:40:00.000000 rosdistro-0.9.0/src/rosdistro/manifest_provider/cache.py
--rw-r--r--   0 root         (0) root         (0)     4854 2021-12-03 00:40:00.000000 rosdistro-0.9.0/src/rosdistro/manifest_provider/git.py
--rw-r--r--   0 root         (0) root         (0)     5168 2021-12-03 00:40:00.000000 rosdistro-0.9.0/src/rosdistro/manifest_provider/github.py
--rw-r--r--   0 root         (0) root         (0)     5094 2021-12-03 00:40:00.000000 rosdistro-0.9.0/src/rosdistro/manifest_provider/tar.py
--rw-r--r--   0 root         (0) root         (0)     7510 2022-06-10 18:01:20.000000 rosdistro-0.9.0/src/rosdistro/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1927 2021-12-03 00:40:00.000000 rosdistro-0.9.0/src/rosdistro/aptdistro.py
--rw-r--r--   0 root         (0) root         (0)     1090 2021-12-03 00:40:00.000000 rosdistro-0.9.0/src/rosdistro/common.py
--rw-r--r--   0 root         (0) root         (0)     7703 2021-12-03 00:40:00.000000 rosdistro-0.9.0/src/rosdistro/dependency_walker.py
--rw-r--r--   0 root         (0) root         (0)     1268 2021-12-03 00:40:00.000000 rosdistro-0.9.0/src/rosdistro/develdistro.py
--rw-r--r--   0 root         (0) root         (0)     5025 2021-12-03 00:40:00.000000 rosdistro-0.9.0/src/rosdistro/distribution.py
--rw-r--r--   0 root         (0) root         (0)     9959 2021-12-03 00:40:00.000000 rosdistro-0.9.0/src/rosdistro/distribution_cache.py
--rw-r--r--   0 root         (0) root         (0)     9225 2021-12-03 00:40:00.000000 rosdistro-0.9.0/src/rosdistro/distribution_cache_generator.py
--rw-r--r--   0 root         (0) root         (0)     6832 2021-12-03 00:40:00.000000 rosdistro-0.9.0/src/rosdistro/distribution_file.py
--rw-r--r--   0 root         (0) root         (0)     6966 2021-12-03 00:40:00.000000 rosdistro-0.9.0/src/rosdistro/doc_build_file.py
--rw-r--r--   0 root         (0) root         (0)     3266 2021-12-03 00:40:00.000000 rosdistro-0.9.0/src/rosdistro/doc_file.py
--rw-r--r--   0 root         (0) root         (0)     2578 2021-12-03 00:40:00.000000 rosdistro-0.9.0/src/rosdistro/doc_repository_specification.py
--rw-r--r--   0 root         (0) root         (0)     5143 2021-12-03 00:40:00.000000 rosdistro-0.9.0/src/rosdistro/freeze_source.py
--rw-r--r--   0 root         (0) root         (0)     6464 2021-12-03 00:40:00.000000 rosdistro-0.9.0/src/rosdistro/index.py
--rw-r--r--   0 root         (0) root         (0)     8708 2021-12-03 00:40:00.000000 rosdistro-0.9.0/src/rosdistro/legacy.py
--rw-r--r--   0 root         (0) root         (0)     2819 2021-12-03 00:40:00.000000 rosdistro-0.9.0/src/rosdistro/loader.py
--rw-r--r--   0 root         (0) root         (0)     1921 2021-12-03 00:40:00.000000 rosdistro-0.9.0/src/rosdistro/package.py
--rw-r--r--   0 root         (0) root         (0)     3377 2021-12-03 00:40:00.000000 rosdistro-0.9.0/src/rosdistro/release.py
--rw-r--r--   0 root         (0) root         (0)     3197 2021-12-03 00:40:00.000000 rosdistro-0.9.0/src/rosdistro/release_build.py
--rw-r--r--   0 root         (0) root         (0)     7858 2021-12-03 00:40:00.000000 rosdistro-0.9.0/src/rosdistro/release_build_file.py
--rw-r--r--   0 root         (0) root         (0)     5018 2021-12-03 00:40:00.000000 rosdistro-0.9.0/src/rosdistro/release_cache.py
--rw-r--r--   0 root         (0) root         (0)     6119 2021-12-03 00:40:00.000000 rosdistro-0.9.0/src/rosdistro/release_cache_generator.py
--rw-r--r--   0 root         (0) root         (0)     4899 2021-12-03 00:40:00.000000 rosdistro-0.9.0/src/rosdistro/release_file.py
--rw-r--r--   0 root         (0) root         (0)     3378 2021-12-03 00:40:00.000000 rosdistro-0.9.0/src/rosdistro/release_repository_specification.py
--rw-r--r--   0 root         (0) root         (0)     4381 2021-12-03 00:40:00.000000 rosdistro-0.9.0/src/rosdistro/repository.py
--rw-r--r--   0 root         (0) root         (0)     3781 2021-12-03 00:40:00.000000 rosdistro-0.9.0/src/rosdistro/repository_specification.py
--rw-r--r--   0 root         (0) root         (0)    14873 2021-12-03 00:40:00.000000 rosdistro-0.9.0/src/rosdistro/rosdistro.py
--rw-r--r--   0 root         (0) root         (0)     6469 2021-12-03 00:40:00.000000 rosdistro-0.9.0/src/rosdistro/source_build_file.py
--rw-r--r--   0 root         (0) root         (0)     3365 2021-12-03 00:40:00.000000 rosdistro-0.9.0/src/rosdistro/source_file.py
--rw-r--r--   0 root         (0) root         (0)     4083 2021-12-03 00:40:00.000000 rosdistro-0.9.0/src/rosdistro/source_repository_cache.py
--rw-r--r--   0 root         (0) root         (0)     2661 2021-12-03 00:40:00.000000 rosdistro-0.9.0/src/rosdistro/source_repository_specification.py
--rw-r--r--   0 root         (0) root         (0)     1898 2021-12-03 00:40:00.000000 rosdistro-0.9.0/src/rosdistro/status.py
--rw-r--r--   0 root         (0) root         (0)     3754 2021-12-03 00:40:00.000000 rosdistro-0.9.0/src/rosdistro/vcs.py
--rw-r--r--   0 root         (0) root         (0)     6342 2021-12-03 00:40:00.000000 rosdistro-0.9.0/src/rosdistro/verify.py
--rw-r--r--   0 root         (0) root         (0)     2037 2021-12-03 00:40:00.000000 rosdistro-0.9.0/src/rosdistro/writer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 18:20:34.000000 rosdistro-0.9.0/src/rosdistro.egg-info/
--rw-r--r--   0 root         (0) root         (0)      701 2022-06-10 18:20:34.000000 rosdistro-0.9.0/src/rosdistro.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2122 2022-06-10 18:20:34.000000 rosdistro-0.9.0/src/rosdistro.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-10 18:20:34.000000 rosdistro-0.9.0/src/rosdistro.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       87 2022-06-10 18:20:34.000000 rosdistro-0.9.0/src/rosdistro.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2022-06-10 18:20:34.000000 rosdistro-0.9.0/src/rosdistro.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 18:20:34.000000 rosdistro-0.9.0/test/
--rw-r--r--   0 root         (0) root         (0)      307 2021-12-03 00:40:00.000000 rosdistro-0.9.0/test/test_cache.py
--rw-r--r--   0 root         (0) root         (0)     1343 2021-12-03 00:40:00.000000 rosdistro-0.9.0/test/test_distribution.py
--rw-r--r--   0 root         (0) root         (0)     1112 2021-12-03 00:40:00.000000 rosdistro-0.9.0/test/test_doc.py
--rw-r--r--   0 root         (0) root         (0)      693 2021-12-03 00:40:00.000000 rosdistro-0.9.0/test/test_doc_build.py
--rw-r--r--   0 root         (0) root         (0)     3030 2021-12-03 00:40:00.000000 rosdistro-0.9.0/test/test_index.py
--rw-r--r--   0 root         (0) root         (0)     6333 2022-06-10 18:01:20.000000 rosdistro-0.9.0/test/test_manifest_providers.py
--rw-r--r--   0 root         (0) root         (0)     1124 2021-12-03 00:40:00.000000 rosdistro-0.9.0/test/test_release.py
--rw-r--r--   0 root         (0) root         (0)     1849 2021-12-03 00:40:00.000000 rosdistro-0.9.0/test/test_release_build.py
--rw-r--r--   0 root         (0) root         (0)      956 2021-12-03 00:40:00.000000 rosdistro-0.9.0/test/test_repository_specification.py
--rw-r--r--   0 root         (0) root         (0)     1133 2021-12-03 00:40:00.000000 rosdistro-0.9.0/test/test_source.py
--rw-r--r--   0 root         (0) root         (0)      717 2021-12-03 00:40:00.000000 rosdistro-0.9.0/test/test_source_build.py
--rw-r--r--   0 root         (0) root         (0)      459 2021-12-03 00:40:00.000000 rosdistro-0.9.0/test/test_verify.py
--rw-r--r--   0 root         (0) root         (0)     1302 2021-12-03 00:40:00.000000 rosdistro-0.9.0/test/test_writer.py
--rw-r--r--   0 root         (0) root         (0)     1536 2021-12-03 00:40:00.000000 rosdistro-0.9.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      475 2021-12-03 00:40:00.000000 rosdistro-0.9.0/README.rst
--rw-r--r--   0 root         (0) root         (0)      232 2022-06-10 18:20:34.000000 rosdistro-0.9.0/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1834 2022-06-10 18:01:20.000000 rosdistro-0.9.0/setup.py
--rw-r--r--   0 root         (0) root         (0)      701 2022-06-10 18:20:34.000000 rosdistro-0.9.0/PKG-INFO
+drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2024-05-03 19:22:15.433243 rosdistro-0.9.1/
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1536 2024-05-03 18:52:33.000000 rosdistro-0.9.1/LICENSE.txt
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      701 2024-05-03 19:22:15.433243 rosdistro-0.9.1/PKG-INFO
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      475 2024-05-03 18:52:33.000000 rosdistro-0.9.1/README.rst
+drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2024-05-03 19:22:15.425243 rosdistro-0.9.1/scripts/
+-rwxrwxr-x   0 cottsay   (1000) cottsay   (1000)     4192 2024-05-03 18:52:33.000000 rosdistro-0.9.1/scripts/rosdistro_build_cache
+-rwxrwxr-x   0 cottsay   (1000) cottsay   (1000)     4186 2024-05-03 18:52:33.000000 rosdistro-0.9.1/scripts/rosdistro_freeze_source
+-rwxrwxr-x   0 cottsay   (1000) cottsay   (1000)     5980 2024-05-03 18:52:33.000000 rosdistro-0.9.1/scripts/rosdistro_migrate_to_rep_141
+-rwxrwxr-x   0 cottsay   (1000) cottsay   (1000)     1176 2024-05-03 18:52:33.000000 rosdistro-0.9.1/scripts/rosdistro_migrate_to_rep_143
+-rwxrwxr-x   0 cottsay   (1000) cottsay   (1000)     2641 2024-05-03 18:52:33.000000 rosdistro-0.9.1/scripts/rosdistro_reformat
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      232 2024-05-03 19:22:15.433243 rosdistro-0.9.1/setup.cfg
+-rwxrwxr-x   0 cottsay   (1000) cottsay   (1000)     1834 2024-05-03 18:52:33.000000 rosdistro-0.9.1/setup.py
+drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2024-05-03 19:22:15.425243 rosdistro-0.9.1/src/
+drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2024-05-03 19:22:15.429243 rosdistro-0.9.1/src/rosdistro/
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     7510 2024-05-03 18:52:33.000000 rosdistro-0.9.1/src/rosdistro/__init__.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1927 2024-05-03 18:52:33.000000 rosdistro-0.9.1/src/rosdistro/aptdistro.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1090 2024-05-03 18:52:33.000000 rosdistro-0.9.1/src/rosdistro/common.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     7703 2024-05-03 18:52:33.000000 rosdistro-0.9.1/src/rosdistro/dependency_walker.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1268 2024-05-03 18:52:33.000000 rosdistro-0.9.1/src/rosdistro/develdistro.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     5025 2024-05-03 18:52:33.000000 rosdistro-0.9.1/src/rosdistro/distribution.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     9959 2024-05-03 18:52:33.000000 rosdistro-0.9.1/src/rosdistro/distribution_cache.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     9226 2024-05-03 18:52:33.000000 rosdistro-0.9.1/src/rosdistro/distribution_cache_generator.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     6832 2024-05-03 18:52:33.000000 rosdistro-0.9.1/src/rosdistro/distribution_file.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     6966 2024-05-03 18:52:33.000000 rosdistro-0.9.1/src/rosdistro/doc_build_file.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     3266 2024-05-03 18:52:33.000000 rosdistro-0.9.1/src/rosdistro/doc_file.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     2578 2024-05-03 18:52:33.000000 rosdistro-0.9.1/src/rosdistro/doc_repository_specification.py
+drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2024-05-03 19:22:15.433243 rosdistro-0.9.1/src/rosdistro/external/
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)        0 2024-05-03 18:52:33.000000 rosdistro-0.9.1/src/rosdistro/external/__init__.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)    21045 2024-05-03 18:52:33.000000 rosdistro-0.9.1/src/rosdistro/external/appdirs.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     5143 2024-05-03 18:52:33.000000 rosdistro-0.9.1/src/rosdistro/freeze_source.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     6464 2024-05-03 18:52:33.000000 rosdistro-0.9.1/src/rosdistro/index.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     8708 2024-05-03 18:52:33.000000 rosdistro-0.9.1/src/rosdistro/legacy.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     2819 2024-05-03 18:52:33.000000 rosdistro-0.9.1/src/rosdistro/loader.py
+drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2024-05-03 19:22:15.433243 rosdistro-0.9.1/src/rosdistro/manifest_provider/
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1874 2024-05-03 18:52:33.000000 rosdistro-0.9.1/src/rosdistro/manifest_provider/__init__.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     3554 2024-05-03 18:52:33.000000 rosdistro-0.9.1/src/rosdistro/manifest_provider/bitbucket.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     6112 2024-05-03 18:52:33.000000 rosdistro-0.9.1/src/rosdistro/manifest_provider/cache.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     4854 2024-05-03 18:52:33.000000 rosdistro-0.9.1/src/rosdistro/manifest_provider/git.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     5168 2024-05-03 18:52:33.000000 rosdistro-0.9.1/src/rosdistro/manifest_provider/github.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     5082 2024-05-03 18:52:33.000000 rosdistro-0.9.1/src/rosdistro/manifest_provider/tar.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1921 2024-05-03 18:52:33.000000 rosdistro-0.9.1/src/rosdistro/package.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     3377 2024-05-03 18:52:33.000000 rosdistro-0.9.1/src/rosdistro/release.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     3197 2024-05-03 18:52:33.000000 rosdistro-0.9.1/src/rosdistro/release_build.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     7858 2024-05-03 18:52:33.000000 rosdistro-0.9.1/src/rosdistro/release_build_file.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     5018 2024-05-03 18:52:33.000000 rosdistro-0.9.1/src/rosdistro/release_cache.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     6120 2024-05-03 18:52:33.000000 rosdistro-0.9.1/src/rosdistro/release_cache_generator.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     4899 2024-05-03 18:52:33.000000 rosdistro-0.9.1/src/rosdistro/release_file.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     3378 2024-05-03 18:52:33.000000 rosdistro-0.9.1/src/rosdistro/release_repository_specification.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     4381 2024-05-03 18:52:33.000000 rosdistro-0.9.1/src/rosdistro/repository.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     3782 2024-05-03 18:52:33.000000 rosdistro-0.9.1/src/rosdistro/repository_specification.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)    14873 2024-05-03 18:52:33.000000 rosdistro-0.9.1/src/rosdistro/rosdistro.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     6469 2024-05-03 18:52:33.000000 rosdistro-0.9.1/src/rosdistro/source_build_file.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     3365 2024-05-03 18:52:33.000000 rosdistro-0.9.1/src/rosdistro/source_file.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     4083 2024-05-03 18:52:33.000000 rosdistro-0.9.1/src/rosdistro/source_repository_cache.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     2661 2024-05-03 18:52:33.000000 rosdistro-0.9.1/src/rosdistro/source_repository_specification.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1898 2024-05-03 18:52:33.000000 rosdistro-0.9.1/src/rosdistro/status.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     3728 2024-05-03 18:52:33.000000 rosdistro-0.9.1/src/rosdistro/vcs.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     6342 2024-05-03 18:52:33.000000 rosdistro-0.9.1/src/rosdistro/verify.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     2037 2024-05-03 18:52:33.000000 rosdistro-0.9.1/src/rosdistro/writer.py
+drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2024-05-03 19:22:15.433243 rosdistro-0.9.1/src/rosdistro.egg-info/
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      701 2024-05-03 19:22:15.000000 rosdistro-0.9.1/src/rosdistro.egg-info/PKG-INFO
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     2122 2024-05-03 19:22:15.000000 rosdistro-0.9.1/src/rosdistro.egg-info/SOURCES.txt
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)        1 2024-05-03 19:22:15.000000 rosdistro-0.9.1/src/rosdistro.egg-info/dependency_links.txt
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)       87 2024-05-03 19:22:15.000000 rosdistro-0.9.1/src/rosdistro.egg-info/requires.txt
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)       10 2024-05-03 19:22:15.000000 rosdistro-0.9.1/src/rosdistro.egg-info/top_level.txt
+drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2024-05-03 19:22:15.433243 rosdistro-0.9.1/test/
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      347 2024-05-03 18:52:33.000000 rosdistro-0.9.1/test/test_cache.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1399 2024-05-03 18:52:33.000000 rosdistro-0.9.1/test/test_distribution.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1168 2024-05-03 18:52:33.000000 rosdistro-0.9.1/test/test_doc.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      749 2024-05-03 18:52:33.000000 rosdistro-0.9.1/test/test_doc_build.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     3109 2024-05-03 18:52:33.000000 rosdistro-0.9.1/test/test_index.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     6361 2024-05-03 18:52:33.000000 rosdistro-0.9.1/test/test_manifest_providers.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1180 2024-05-03 18:52:33.000000 rosdistro-0.9.1/test/test_release.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1918 2024-05-03 18:52:33.000000 rosdistro-0.9.1/test/test_release_build.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      956 2024-05-03 18:52:33.000000 rosdistro-0.9.1/test/test_repository_specification.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1189 2024-05-03 18:52:33.000000 rosdistro-0.9.1/test/test_source.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      773 2024-05-03 18:52:33.000000 rosdistro-0.9.1/test/test_source_build.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      512 2024-05-03 18:52:33.000000 rosdistro-0.9.1/test/test_verify.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1342 2024-05-03 18:52:33.000000 rosdistro-0.9.1/test/test_writer.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `rosdistro-0.9.0/scripts/rosdistro_build_cache` & `rosdistro-0.9.1/scripts/rosdistro_build_cache`

 * *Files identical despite different names*

### Comparing `rosdistro-0.9.0/scripts/rosdistro_freeze_source` & `rosdistro-0.9.1/scripts/rosdistro_freeze_source`

 * *Files identical despite different names*

### Comparing `rosdistro-0.9.0/scripts/rosdistro_migrate_to_rep_141` & `rosdistro-0.9.1/scripts/rosdistro_migrate_to_rep_141`

 * *Files identical despite different names*

### Comparing `rosdistro-0.9.0/scripts/rosdistro_migrate_to_rep_143` & `rosdistro-0.9.1/scripts/rosdistro_migrate_to_rep_143`

 * *Files identical despite different names*

### Comparing `rosdistro-0.9.0/scripts/rosdistro_reformat` & `rosdistro-0.9.1/scripts/rosdistro_reformat`

 * *Files identical despite different names*

### Comparing `rosdistro-0.9.0/src/rosdistro/external/appdirs.py` & `rosdistro-0.9.1/src/rosdistro/external/appdirs.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
             path = os.path.join(path, appname)
     if appname and version:
         path = os.path.join(path, version)
     return path
 
 
 def site_data_dir(appname=None, appauthor=None, version=None, multipath=False):
-    """Return full path to the user-shared data dir for this application.
+    r"""Return full path to the user-shared data dir for this application.
 
         "appname" is the name of application.
             If None, just the system directory is returned.
         "appauthor" (only required and used on Windows) is the name of the
             appauthor or distributing body for this application. Typically
             it is the owning company name. This falls back to appname.
         "version" is an optional version path element to append to the
@@ -196,15 +196,15 @@
             path = os.path.join(path, appname)
     if appname and version:
         path = os.path.join(path, version)
     return path
 
 
 def site_config_dir(appname=None, appauthor=None, version=None, multipath=False):
-    """Return full path to the user-shared data dir for this application.
+    r"""Return full path to the user-shared data dir for this application.
 
         "appname" is the name of application.
             If None, just the system directory is returned.
         "appauthor" (only required and used on Windows) is the name of the
             appauthor or distributing body for this application. Typically
             it is the owning company name. This falls back to appname.
         "version" is an optional version path element to append to the
```

### Comparing `rosdistro-0.9.0/src/rosdistro/manifest_provider/__init__.py` & `rosdistro-0.9.1/src/rosdistro/manifest_provider/__init__.py`

 * *Files identical despite different names*

### Comparing `rosdistro-0.9.0/src/rosdistro/manifest_provider/bitbucket.py` & `rosdistro-0.9.1/src/rosdistro/manifest_provider/bitbucket.py`

 * *Files identical despite different names*

### Comparing `rosdistro-0.9.0/src/rosdistro/manifest_provider/cache.py` & `rosdistro-0.9.1/src/rosdistro/manifest_provider/cache.py`

 * *Files identical despite different names*

### Comparing `rosdistro-0.9.0/src/rosdistro/manifest_provider/git.py` & `rosdistro-0.9.1/src/rosdistro/manifest_provider/git.py`

 * *Files identical despite different names*

### Comparing `rosdistro-0.9.0/src/rosdistro/manifest_provider/github.py` & `rosdistro-0.9.1/src/rosdistro/manifest_provider/github.py`

 * *Files identical despite different names*

### Comparing `rosdistro-0.9.0/src/rosdistro/manifest_provider/tar.py` & `rosdistro-0.9.1/src/rosdistro/manifest_provider/tar.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         request.add_header('Authorization', authheader)
     elif _TAR_PASSWORD:
         logger.debug('- using private token auth from supplied environment variables.')
         request.add_header('Private-Token', _TAR_PASSWORD)
 
     response = urlopen(request)
     with tarfile.open(fileobj=io.BytesIO(response.read())) as tar:
-        package_xml = tar.extractfile(os.path.join(subdir, 'package.xml')).read()
+        package_xml = tar.extractfile(subdir + '/package.xml').read()
 
         # Python2 returns strings, Python3 returns bytes-- support both
         try:
             return package_xml.decode('utf-8')
         except AttributeError:
             return package_xml
```

### Comparing `rosdistro-0.9.0/src/rosdistro/__init__.py` & `rosdistro-0.9.1/src/rosdistro/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 from .loader import load_url  # noqa
 from .manifest_provider.cache import CachedManifestProvider, CachedSourceManifestProvider  # noqa
 
 
 # same version as in:
 # - setup.py
 # - stdeb.cfg
-__version__ = '0.9.0'
+__version__ = '0.9.1'
 
 # index information
 
 DEFAULT_INDEX_URL = 'https://raw.githubusercontent.com/ros/rosdistro/master/index-v4.yaml'
 
 
 def get_index_url():
```

### Comparing `rosdistro-0.9.0/src/rosdistro/aptdistro.py` & `rosdistro-0.9.1/src/rosdistro/aptdistro.py`

 * *Files identical despite different names*

### Comparing `rosdistro-0.9.0/src/rosdistro/common.py` & `rosdistro-0.9.1/src/rosdistro/common.py`

 * *Files identical despite different names*

### Comparing `rosdistro-0.9.0/src/rosdistro/dependency_walker.py` & `rosdistro-0.9.1/src/rosdistro/dependency_walker.py`

 * *Files identical despite different names*

### Comparing `rosdistro-0.9.0/src/rosdistro/develdistro.py` & `rosdistro-0.9.1/src/rosdistro/develdistro.py`

 * *Files identical despite different names*

### Comparing `rosdistro-0.9.0/src/rosdistro/distribution.py` & `rosdistro-0.9.1/src/rosdistro/distribution.py`

 * *Files identical despite different names*

### Comparing `rosdistro-0.9.0/src/rosdistro/distribution_cache.py` & `rosdistro-0.9.1/src/rosdistro/distribution_cache.py`

 * *Files identical despite different names*

### Comparing `rosdistro-0.9.0/src/rosdistro/distribution_cache_generator.py` & `rosdistro-0.9.1/src/rosdistro/distribution_cache_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         # check that package.xml is parseable
         try:
             pkg = parse_package_string(package_xml)
         except InvalidPackage as e:
             errors.append('%s: invalid package.xml file for package "%s": %s' % (dist_name, pkg_name, e))
             continue
         # check that version numbers match (at least without deb inc)
-        if not re.match('^%s(-[\dA-z~\+\.]+)?$' % re.escape(pkg.version), repo.version):
+        if not re.match(r'^%s(-[\dA-z~\+\.]+)?$' % re.escape(pkg.version), repo.version):
             errors.append('%s: different version in package.xml (%s) for package "%s" than for the repository (%s) (after removing the debian increment)' % (dist_name, pkg.version, pkg_name, repo.version))
 
         if package_xml != old_package_xml:
             print("  - updated manifest of package '%s' to version '%s'" % (pkg_name, pkg.version))
 
     if not debug:
         print('')
```

### Comparing `rosdistro-0.9.0/src/rosdistro/distribution_file.py` & `rosdistro-0.9.1/src/rosdistro/distribution_file.py`

 * *Files identical despite different names*

### Comparing `rosdistro-0.9.0/src/rosdistro/doc_build_file.py` & `rosdistro-0.9.1/src/rosdistro/doc_build_file.py`

 * *Files identical despite different names*

### Comparing `rosdistro-0.9.0/src/rosdistro/doc_file.py` & `rosdistro-0.9.1/src/rosdistro/doc_file.py`

 * *Files identical despite different names*

### Comparing `rosdistro-0.9.0/src/rosdistro/doc_repository_specification.py` & `rosdistro-0.9.1/src/rosdistro/doc_repository_specification.py`

 * *Files identical despite different names*

### Comparing `rosdistro-0.9.0/src/rosdistro/freeze_source.py` & `rosdistro-0.9.1/src/rosdistro/freeze_source.py`

 * *Files identical despite different names*

### Comparing `rosdistro-0.9.0/src/rosdistro/index.py` & `rosdistro-0.9.1/src/rosdistro/index.py`

 * *Files identical despite different names*

### Comparing `rosdistro-0.9.0/src/rosdistro/legacy.py` & `rosdistro-0.9.1/src/rosdistro/legacy.py`

 * *Files identical despite different names*

### Comparing `rosdistro-0.9.0/src/rosdistro/loader.py` & `rosdistro-0.9.1/src/rosdistro/loader.py`

 * *Files identical despite different names*

### Comparing `rosdistro-0.9.0/src/rosdistro/package.py` & `rosdistro-0.9.1/src/rosdistro/package.py`

 * *Files identical despite different names*

### Comparing `rosdistro-0.9.0/src/rosdistro/release.py` & `rosdistro-0.9.1/src/rosdistro/release.py`

 * *Files identical despite different names*

### Comparing `rosdistro-0.9.0/src/rosdistro/release_build.py` & `rosdistro-0.9.1/src/rosdistro/release_build.py`

 * *Files identical despite different names*

### Comparing `rosdistro-0.9.0/src/rosdistro/release_build_file.py` & `rosdistro-0.9.1/src/rosdistro/release_build_file.py`

 * *Files identical despite different names*

### Comparing `rosdistro-0.9.0/src/rosdistro/release_cache.py` & `rosdistro-0.9.1/src/rosdistro/release_cache.py`

 * *Files identical despite different names*

### Comparing `rosdistro-0.9.0/src/rosdistro/release_cache_generator.py` & `rosdistro-0.9.1/src/rosdistro/release_cache_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         # check that package.xml is parseable
         try:
             pkg = parse_package_string(package_xml)
         except InvalidPackage:
             errors.append('%s: invalid package.xml file for package "%s"' % (dist_name, pkg_name))
             continue
         # check that version numbers match (at least without deb inc)
-        if not re.match('^%s(-[\dA-z~\+\.]+)?$' % re.escape(pkg.version), repo.version):
+        if not re.match(r'^%s(-[\dA-z~\+\.]+)?$' % re.escape(pkg.version), repo.version):
             errors.append('%s: different version in package.xml (%s) for package "%s" than for the repository (%s) (after removing the debian increment)' % (dist_name, pkg.version, pkg_name, repo.version))
 
     if not debug:
         print('')
 
     if errors:
         raise RuntimeError('\n'.join(errors))
```

### Comparing `rosdistro-0.9.0/src/rosdistro/release_file.py` & `rosdistro-0.9.1/src/rosdistro/release_file.py`

 * *Files identical despite different names*

### Comparing `rosdistro-0.9.0/src/rosdistro/release_repository_specification.py` & `rosdistro-0.9.1/src/rosdistro/release_repository_specification.py`

 * *Files identical despite different names*

### Comparing `rosdistro-0.9.0/src/rosdistro/repository.py` & `rosdistro-0.9.1/src/rosdistro/repository.py`

 * *Files identical despite different names*

### Comparing `rosdistro-0.9.0/src/rosdistro/repository_specification.py` & `rosdistro-0.9.1/src/rosdistro/repository_specification.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 import re
 
 from .vcs import Git
 
 
 class RepositorySpecification(object):
     # Match groups are server and path on server.
-    VCS_REGEX = re.compile('(?:https?:\/\/|ssh:\/\/|git:\/\/|git@)((?:[a-fA-F0-9]{40}@)?[\w.-]+)[:/]([\w/-]*)(?:\.git)?$')
+    VCS_REGEX = re.compile(r'(?:https?:\/\/|ssh:\/\/|git:\/\/|git@)((?:[a-fA-F0-9]{40}@)?[\w.-]+)[:/]([\w/-]*)(?:\.git)?$')
 
     def __init__(self, name, data):
         self.name = name
         self.type = data.get('type', 'git')
         assert 'url' in data and data['url'], "Repository '%s' lacks required URL information" % name
         self.url = data['url']
         self.version = data.get('version', None)
```

### Comparing `rosdistro-0.9.0/src/rosdistro/rosdistro.py` & `rosdistro-0.9.1/src/rosdistro/rosdistro.py`

 * *Files identical despite different names*

### Comparing `rosdistro-0.9.0/src/rosdistro/source_build_file.py` & `rosdistro-0.9.1/src/rosdistro/source_build_file.py`

 * *Files identical despite different names*

### Comparing `rosdistro-0.9.0/src/rosdistro/source_file.py` & `rosdistro-0.9.1/src/rosdistro/source_file.py`

 * *Files identical despite different names*

### Comparing `rosdistro-0.9.0/src/rosdistro/source_repository_cache.py` & `rosdistro-0.9.1/src/rosdistro/source_repository_cache.py`

 * *Files identical despite different names*

### Comparing `rosdistro-0.9.0/src/rosdistro/source_repository_specification.py` & `rosdistro-0.9.1/src/rosdistro/source_repository_specification.py`

 * *Files identical despite different names*

### Comparing `rosdistro-0.9.0/src/rosdistro/status.py` & `rosdistro-0.9.1/src/rosdistro/status.py`

 * *Files identical despite different names*

### Comparing `rosdistro-0.9.0/src/rosdistro/vcs.py` & `rosdistro-0.9.1/src/rosdistro/vcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 def ref_is_hash(ref):
     return re.match('^[0-9a-f]{40}$', ref) is not None
 
 
 def _run_command(cmd, cwd=None, env=None):
     result = {'cmd': ' '.join(cmd), 'cwd': cwd}
     try:
-        proc = subprocess.Popen(cmd, cwd=cwd, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, env=env)
+        proc = subprocess.Popen(cmd, cwd=cwd, stdout=subprocess.PIPE, env=env)
         output, _ = proc.communicate()
         result['output'] = output.rstrip()
         result['returncode'] = proc.returncode
     except subprocess.CalledProcessError as e:
         result['output'] = e.output
         result['returncode'] = e.returncode
     if not isinstance(result['output'], str):
```

### Comparing `rosdistro-0.9.0/src/rosdistro/verify.py` & `rosdistro-0.9.1/src/rosdistro/verify.py`

 * *Files identical despite different names*

### Comparing `rosdistro-0.9.0/src/rosdistro/writer.py` & `rosdistro-0.9.1/src/rosdistro/writer.py`

 * *Files identical despite different names*

### Comparing `rosdistro-0.9.0/src/rosdistro.egg-info/PKG-INFO` & `rosdistro-0.9.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosdistro
-Version: 0.9.0
+Version: 0.9.1
 Summary: A tool to work with rosdistro files
 Home-page: http://wiki.ros.org/rosdistro
 Author: Wim Meeussen, Dirk Thomas
 Author-email: wim@hidof.com, dthomas@osrfoundation.org
 Maintainer: ROS Infrastructure Team
 License: BSD, MIT
 Project-URL: Source code, https://github.com/ros-infrastructure/rosdistro
```

### Comparing `rosdistro-0.9.0/src/rosdistro.egg-info/SOURCES.txt` & `rosdistro-0.9.1/src/rosdistro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rosdistro-0.9.0/test/test_distribution.py` & `rosdistro-0.9.1/test/test_release.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 import os
 
-from rosdistro import get_distribution_file, get_distribution_files, get_index
-from rosdistro.distribution_file import DistributionFile
+from rosdistro import get_index, get_release_file
 from rosdistro.loader import load_url
+from rosdistro.release_file import ReleaseFile
 
 import yaml
 
+from . import path_to_url
+
 FILES_DIR = os.path.normpath(os.path.join(os.path.dirname(os.path.abspath(__file__)), 'files'))
 
 
-def test_distribution_file():
-    url = 'file://' + FILES_DIR + '/foo/distribution.yaml'
+def test_release_file():
+    url = path_to_url(os.path.join(FILES_DIR, 'foo', 'distribution.yaml'))
     yaml_str = load_url(url)
     data = yaml.safe_load(yaml_str)
-    dist_file = DistributionFile('foo', data)
-    _validate_dist_file(dist_file)
+    rel_file = ReleaseFile('foo', data)
+    _validate_rel_file(rel_file)
 
 
-def test_get_distribution_file():
-    url = 'file://' + FILES_DIR + '/index_v2.yaml'
+def test_get_release_file():
+    url = path_to_url(os.path.join(FILES_DIR, 'index_v2.yaml'))
     i = get_index(url)
-    dist_file = get_distribution_file(i, 'foo')
-    _validate_dist_file(dist_file)
-
-    dist_files = get_distribution_files(i, 'foo')
-    assert len(dist_files) == 1
+    rel_file = get_release_file(i, 'foo')
+    _validate_rel_file(rel_file)
 
 
-def _validate_dist_file(dist_file):
-    assert('bar_repo' in dist_file.repositories)
-    repo = dist_file.repositories['bar_repo']
-    assert repo.release_repository.package_names == ['bar_repo']
-    assert 'bar_repo' in dist_file.release_packages
-
-    assert'baz-repo' in dist_file.repositories
-    repo = dist_file.repositories['baz-repo']
-    assert set(repo.release_repository.package_names) == set(['baz_pkg1', 'baz_pkg2'])
-    assert 'baz_pkg1' in dist_file.release_packages
-    assert 'baz_pkg2' in dist_file.release_packages
+def _validate_rel_file(rel_file):
+    assert('bar_repo' in rel_file.repositories)
+    repo = rel_file.repositories['bar_repo']
+    assert repo.package_names == ['bar_repo']
+    assert 'bar_repo' in rel_file.packages
+
+    assert'baz-repo' in rel_file.repositories
+    repo = rel_file.repositories['baz-repo']
+    assert set(repo.package_names) == set(['baz_pkg1', 'baz_pkg2'])
+    assert 'baz_pkg1' in rel_file.packages
+    assert 'baz_pkg2' in rel_file.packages
```

### Comparing `rosdistro-0.9.0/test/test_doc.py` & `rosdistro-0.9.1/test/test_doc.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,27 +2,29 @@
 
 from rosdistro import get_doc_file, get_index
 from rosdistro.doc_file import DocFile
 from rosdistro.loader import load_url
 
 import yaml
 
+from . import path_to_url
+
 FILES_DIR = os.path.normpath(os.path.join(os.path.dirname(os.path.abspath(__file__)), 'files'))
 
 
 def test_doc_file():
-    url = 'file://' + FILES_DIR + '/foo/distribution.yaml'
+    url = path_to_url(os.path.join(FILES_DIR, 'foo', 'distribution.yaml'))
     yaml_str = load_url(url)
     data = yaml.safe_load(yaml_str)
     doc_file = DocFile('foo', data)
     _validate_doc_file(doc_file)
 
 
 def test_get_doc_file():
-    url = 'file://' + FILES_DIR + '/index_v2.yaml'
+    url = path_to_url(os.path.join(FILES_DIR, 'index_v2.yaml'))
     i = get_index(url)
     doc_file = get_doc_file(i, 'foo')
     _validate_doc_file(doc_file)
 
 
 def _validate_doc_file(doc_file):
     assert(set(['bar_repo', 'baz-repo']) == set(doc_file.repositories.keys()))
```

### Comparing `rosdistro-0.9.0/test/test_doc_build.py` & `rosdistro-0.9.1/test/test_doc_build.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,24 +2,26 @@
 
 from rosdistro import get_doc_build_files, get_index
 from rosdistro.doc_build_file import DocBuildFile
 from rosdistro.loader import load_url
 
 import yaml
 
+from . import path_to_url
+
 FILES_DIR = os.path.normpath(os.path.join(os.path.dirname(os.path.abspath(__file__)), 'files'))
 
 
 def test_doc_build_file():
-    url = 'file://' + FILES_DIR + '/foo/doc-build.yaml'
+    url = path_to_url(os.path.join(FILES_DIR, 'foo', 'doc-build.yaml'))
     yaml_str = load_url(url)
     data = yaml.safe_load(yaml_str)
     DocBuildFile('foo', data)
 
 
 def test_get_doc_build_files():
-    url = 'file://' + FILES_DIR + '/index_v2.yaml'
+    url = path_to_url(os.path.join(FILES_DIR, 'index_v2.yaml'))
     i = get_index(url)
     files = get_doc_build_files(i, 'foo')
     assert len(files) == 1
     build_file = files[0]
     assert build_file.jenkins_job_timeout == 23
```

### Comparing `rosdistro-0.9.0/test/test_index.py` & `rosdistro-0.9.1/test/test_index.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,60 +1,62 @@
 import os
 
 from rosdistro import get_distribution_file
 from rosdistro import get_distribution_files
 from rosdistro import get_index
 from rosdistro import get_index_url
 
+from . import path_to_url
+
 FILES_DIR = os.path.normpath(os.path.join(os.path.dirname(os.path.abspath(__file__)), 'files'))
 
 
 def test_get_index_url():
     get_index_url()
 
 
 def test_get_index_v2():
-    url = 'file://' + FILES_DIR + '/index_v2.yaml'
+    url = path_to_url(os.path.join(FILES_DIR, 'index_v2.yaml'))
     i = get_index(url)
     assert len(i.distributions.keys()) == 1
     assert 'foo' in i.distributions.keys()
 
     assert 'distribution_status' not in i.distributions['foo']
     assert 'distribution_type' not in i.distributions['foo']
 
 
 def test_get_index_v3():
-    url = 'file://' + FILES_DIR + '/index_v3.yaml'
+    url = path_to_url(os.path.join(FILES_DIR, 'index_v3.yaml'))
     i = get_index(url)
     assert len(i.distributions.keys()) == 1
     assert 'foo' in i.distributions.keys()
 
     assert 'distribution_status' not in i.distributions['foo']
     assert 'distribution_type' not in i.distributions['foo']
 
     dist_files = get_distribution_files(i, 'foo')
     assert len(dist_files) == 2
     get_distribution_file(i, 'foo')
 
 
 def test_get_index_v3_invalid():
-    url = 'file://' + FILES_DIR + '/index_v3_invalid.yaml'
+    url = path_to_url(os.path.join(FILES_DIR, 'index_v3_invalid.yaml'))
     i = get_index(url)
 
     dist_files = get_distribution_files(i, 'foo')
     assert len(dist_files) == 2
     try:
         get_distribution_file(i, 'foo')
         assert False
     except AssertionError:
         pass
 
 
 def test_get_index_v4():
-    url = 'file://' + FILES_DIR + '/index_v4.yaml'
+    url = path_to_url(os.path.join(FILES_DIR, 'index_v4.yaml'))
     i = get_index(url)
     assert len(i.distributions.keys()) == 1
     assert 'foo' in i.distributions.keys()
 
     assert i.distributions['foo']['distribution_status'] == 'active'
     assert i.distributions['foo']['distribution_type'] == 'ros1'
```

### Comparing `rosdistro-0.9.0/test/test_manifest_providers.py` & `rosdistro-0.9.1/test/test_manifest_providers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # -*- coding: utf-8 -*-
 
+import os
+
 try:
     from unittest.mock import patch
 except ImportError:
     from mock import patch
 
 import rosdistro.manifest_provider.github
 import rosdistro.vcs
@@ -105,15 +107,15 @@
     assert '<version>0.5.11</version>' in package_xml
 
 
 def test_git_source_multi():
     repo_cache = git_source_manifest_provider(_ros_source_repo())
     assert repo_cache.ref()
     package_path, package_xml = repo_cache['roslib']
-    assert package_path == 'core/roslib'
+    assert package_path == os.path.join('core', 'roslib')
 
 
 def test_tar_source():
     repo_cache = rosdistro.manifest_provider.tar.tar_source_manifest_provider(_genmsg_source_tarball())
 
     assert repo_cache.ref() is None
```

### Comparing `rosdistro-0.9.0/test/test_release_build.py` & `rosdistro-0.9.1/test/test_release_build.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,32 +2,34 @@
 
 from rosdistro import get_index, get_release, get_release_build_files, get_release_builds
 from rosdistro.loader import load_url
 from rosdistro.release_build_file import ReleaseBuildFile
 
 import yaml
 
+from . import path_to_url
+
 FILES_DIR = os.path.normpath(os.path.join(os.path.dirname(os.path.abspath(__file__)), 'files'))
 
 
 def test_release_build_file():
-    url = 'file://' + FILES_DIR + '/foo/release-build.yaml'
+    url = path_to_url(os.path.join(FILES_DIR, 'foo', 'release-build.yaml'))
     yaml_str = load_url(url)
     data = yaml.safe_load(yaml_str)
     ReleaseBuildFile('foo', data)
 
 
 def test_get_release_build_files():
-    url = 'file://' + FILES_DIR + '/index_v2.yaml'
+    url = path_to_url(os.path.join(FILES_DIR, 'index_v2.yaml'))
     i = get_index(url)
     get_release_build_files(i, 'foo')
 
 
 def test_get_release_builds():
-    url = 'file://' + FILES_DIR + '/index_v2.yaml'
+    url = path_to_url(os.path.join(FILES_DIR, 'index_v2.yaml'))
     i = get_index(url)
     d = get_release(i, 'foo')
     builds = get_release_builds(i, d)
     assert len(builds) == 1
     build = builds[0]
     assert build.jenkins_sourcedeb_job_timeout == 5
     assert build.jenkins_binarydeb_job_timeout == 42
```

### Comparing `rosdistro-0.9.0/test/test_repository_specification.py` & `rosdistro-0.9.1/test/test_repository_specification.py`

 * *Files identical despite different names*

### Comparing `rosdistro-0.9.0/test/test_source.py` & `rosdistro-0.9.1/test/test_source.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,27 +2,29 @@
 
 from rosdistro import get_index, get_source_file
 from rosdistro.loader import load_url
 from rosdistro.source_file import SourceFile
 
 import yaml
 
+from . import path_to_url
+
 FILES_DIR = os.path.normpath(os.path.join(os.path.dirname(os.path.abspath(__file__)), 'files'))
 
 
 def test_source_file():
-    url = 'file://' + FILES_DIR + '/foo/distribution.yaml'
+    url = path_to_url(os.path.join(FILES_DIR, 'foo', 'distribution.yaml'))
     yaml_str = load_url(url)
     data = yaml.safe_load(yaml_str)
     src_file = SourceFile('foo', data)
     _validate_src_file(src_file)
 
 
 def test_get_source_file():
-    url = 'file://' + FILES_DIR + '/index_v2.yaml'
+    url = path_to_url(os.path.join(FILES_DIR, 'index_v2.yaml'))
     i = get_index(url)
     src_file = get_source_file(i, 'foo')
     _validate_src_file(src_file)
 
 
 def _validate_src_file(src_file):
     assert(set(['bar_repo', 'baz-repo']) == set(src_file.repositories.keys()))
```

### Comparing `rosdistro-0.9.0/test/test_writer.py` & `rosdistro-0.9.1/test/test_writer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import difflib
 import os
 
 from rosdistro import get_distribution_file, get_index
 
 from rosdistro.writer import yaml_from_distribution_file
 
+from . import path_to_url
+
 FILES_DIR = os.path.normpath(os.path.join(os.path.dirname(os.path.abspath(__file__)), 'files'))
 
 
 def get_diff(expected, actual):
     udiff = difflib.unified_diff(expected.splitlines(), actual.splitlines(),
                                  fromfile='expected', tofile='actual')
     udiff_raw = ''
@@ -26,14 +28,14 @@
         if line.startswith(' '):
             line += '\n'
             udiff_raw += line
     return '\n' + udiff_raw
 
 
 def test_verify_files_parsable():
-    url = 'file://' + FILES_DIR + '/index_v2.yaml'
+    url = path_to_url(os.path.join(FILES_DIR, 'index_v2.yaml'))
     index = get_index(url)
     distribution_file = get_distribution_file(index, 'foo')
     data = yaml_from_distribution_file(distribution_file)
     with open(os.path.join(FILES_DIR, 'foo', 'distribution.yaml'), 'r') as f:
         expected = f.read()
     assert data == expected, get_diff(expected, data)
```

### Comparing `rosdistro-0.9.0/LICENSE.txt` & `rosdistro-0.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rosdistro-0.9.0/setup.py` & `rosdistro-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import find_packages, setup
 
 kwargs = {
     'name': 'rosdistro',
     # same version as in:
     # - src/rosdistro/__init__.py
     # - stdeb.cfg
-    'version': '0.9.0',
+    'version': '0.9.1',
     'install_requires': ['PyYAML', 'setuptools'],
     'packages': find_packages('src'),
     'package_dir': {'': 'src'},
     'scripts': [
         # 'scripts/rosdistro',
         'scripts/rosdistro_build_cache',
         'scripts/rosdistro_freeze_source',
```

### Comparing `rosdistro-0.9.0/PKG-INFO` & `rosdistro-0.9.1/src/rosdistro.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosdistro
-Version: 0.9.0
+Version: 0.9.1
 Summary: A tool to work with rosdistro files
 Home-page: http://wiki.ros.org/rosdistro
 Author: Wim Meeussen, Dirk Thomas
 Author-email: wim@hidof.com, dthomas@osrfoundation.org
 Maintainer: ROS Infrastructure Team
 License: BSD, MIT
 Project-URL: Source code, https://github.com/ros-infrastructure/rosdistro
```


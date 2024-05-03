# Comparing `tmp/anycorn-0.17.1.tar.gz` & `tmp/anycorn-0.17.2.tar.gz`

## Comparing `anycorn-0.17.1.tar` & `anycorn-0.17.2.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 anycorn-0.17.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 anycorn-0.17.1/.readthedocs.yaml
--rw-r--r--   0        0        0    20871 2020-02-02 00:00:00.000000 anycorn-0.17.1/CHANGELOG.rst
--rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 anycorn-0.17.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 anycorn-0.17.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 anycorn-0.17.1/compliance/autobahn/fuzzingclient.json
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 anycorn-0.17.1/compliance/autobahn/summarise.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 anycorn-0.17.1/compliance/autobahn/ws_server.py
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 anycorn-0.17.1/compliance/h2spec/cert.pem
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 anycorn-0.17.1/compliance/h2spec/http_server.py
--rw-r--r--   0        0        0     3272 2020-02-02 00:00:00.000000 anycorn-0.17.1/compliance/h2spec/key.pem
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/__init__.py
--rw-r--r--   0        0        0    10592 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/__main__.py
--rw-r--r--   0        0        0     5520 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/app_wrappers.py
--rw-r--r--   0        0        0    13238 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/config.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/events.py
--rw-r--r--   0        0        0     3545 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/lifespan.py
--rw-r--r--   0        0        0     7344 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/logging.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/py.typed
--rw-r--r--   0        0        0     9348 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/run.py
--rw-r--r--   0        0        0     4408 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/statsd.py
--rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/task_group.py
--rw-r--r--   0        0        0     5747 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/tcp_server.py
--rw-r--r--   0        0        0     7128 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/typing.py
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/udp_server.py
--rw-r--r--   0        0        0     6469 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/utils.py
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/worker_context.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/middleware/__init__.py
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/middleware/dispatcher.py
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/middleware/http_to_https.py
--rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/middleware/proxy_fix.py
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/middleware/wsgi.py
--rwxr-xr-x   0        0        0     2769 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/protocol/__init__.py
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/protocol/events.py
--rwxr-xr-x   0        0        0    11624 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/protocol/h11.py
--rwxr-xr-x   0        0        0    14996 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/protocol/h2.py
--rw-r--r--   0        0        0     5334 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/protocol/h3.py
--rw-r--r--   0        0        0     7975 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/protocol/http_stream.py
--rw-r--r--   0        0        0     5068 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/protocol/quic.py
--rw-r--r--   0        0        0    14902 2020-02-02 00:00:00.000000 anycorn-0.17.1/src/anycorn/protocol/ws_stream.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/__init__.py
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/conftest.py
--rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/helpers.py
--rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/test___main__.py
--rw-r--r--   0        0        0     6025 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/test_app_wrappers.py
--rw-r--r--   0        0        0     5800 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/test_config.py
--rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/test_keep_alive.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/test_lifespan.py
--rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/test_logging.py
--rw-r--r--   0        0        0     8390 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/test_sanity.py
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/test_utils.py
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/assets/cert.pem
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/assets/config.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/assets/config.toml
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/assets/config_ssl.py
--rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/assets/key.pem
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/middleware/__init__.py
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/middleware/test_dispatcher.py
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/middleware/test_http_to_https.py
--rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/middleware/test_proxy_fix.py
--rwxr-xr-x   0        0        0    15366 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/protocol/test_h11.py
--rw-r--r--   0        0        0     3542 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/protocol/test_h2.py
--rw-r--r--   0        0        0     9873 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/protocol/test_http_stream.py
--rw-r--r--   0        0        0    17121 2020-02-02 00:00:00.000000 anycorn-0.17.1/tests/protocol/test_ws_stream.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 anycorn-0.17.1/.gitignore
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 anycorn-0.17.1/LICENSE
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 anycorn-0.17.1/README.md
--rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 anycorn-0.17.1/pyproject.toml
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 anycorn-0.17.1/PKG-INFO
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 anycorn-0.17.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 anycorn-0.17.2/.readthedocs.yaml
+-rw-r--r--   0        0        0    20871 2020-02-02 00:00:00.000000 anycorn-0.17.2/CHANGELOG.rst
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 anycorn-0.17.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 anycorn-0.17.2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 anycorn-0.17.2/compliance/autobahn/fuzzingclient.json
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 anycorn-0.17.2/compliance/autobahn/summarise.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 anycorn-0.17.2/compliance/autobahn/ws_server.py
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 anycorn-0.17.2/compliance/h2spec/cert.pem
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 anycorn-0.17.2/compliance/h2spec/http_server.py
+-rw-r--r--   0        0        0     3272 2020-02-02 00:00:00.000000 anycorn-0.17.2/compliance/h2spec/key.pem
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 anycorn-0.17.2/src/anycorn/__init__.py
+-rw-r--r--   0        0        0    10885 2020-02-02 00:00:00.000000 anycorn-0.17.2/src/anycorn/__main__.py
+-rw-r--r--   0        0        0     5520 2020-02-02 00:00:00.000000 anycorn-0.17.2/src/anycorn/app_wrappers.py
+-rw-r--r--   0        0        0    13267 2020-02-02 00:00:00.000000 anycorn-0.17.2/src/anycorn/config.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 anycorn-0.17.2/src/anycorn/events.py
+-rw-r--r--   0        0        0     3545 2020-02-02 00:00:00.000000 anycorn-0.17.2/src/anycorn/lifespan.py
+-rw-r--r--   0        0        0     7344 2020-02-02 00:00:00.000000 anycorn-0.17.2/src/anycorn/logging.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 anycorn-0.17.2/src/anycorn/py.typed
+-rw-r--r--   0        0        0     9386 2020-02-02 00:00:00.000000 anycorn-0.17.2/src/anycorn/run.py
+-rw-r--r--   0        0        0     4408 2020-02-02 00:00:00.000000 anycorn-0.17.2/src/anycorn/statsd.py
+-rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 anycorn-0.17.2/src/anycorn/task_group.py
+-rw-r--r--   0        0        0     5747 2020-02-02 00:00:00.000000 anycorn-0.17.2/src/anycorn/tcp_server.py
+-rw-r--r--   0        0        0     7128 2020-02-02 00:00:00.000000 anycorn-0.17.2/src/anycorn/typing.py
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 anycorn-0.17.2/src/anycorn/udp_server.py
+-rw-r--r--   0        0        0     6469 2020-02-02 00:00:00.000000 anycorn-0.17.2/src/anycorn/utils.py
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 anycorn-0.17.2/src/anycorn/worker_context.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 anycorn-0.17.2/src/anycorn/middleware/__init__.py
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 anycorn-0.17.2/src/anycorn/middleware/dispatcher.py
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 anycorn-0.17.2/src/anycorn/middleware/http_to_https.py
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 anycorn-0.17.2/src/anycorn/middleware/proxy_fix.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 anycorn-0.17.2/src/anycorn/middleware/wsgi.py
+-rwxr-xr-x   0        0        0     2769 2020-02-02 00:00:00.000000 anycorn-0.17.2/src/anycorn/protocol/__init__.py
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 anycorn-0.17.2/src/anycorn/protocol/events.py
+-rwxr-xr-x   0        0        0    11624 2020-02-02 00:00:00.000000 anycorn-0.17.2/src/anycorn/protocol/h11.py
+-rwxr-xr-x   0        0        0    14996 2020-02-02 00:00:00.000000 anycorn-0.17.2/src/anycorn/protocol/h2.py
+-rw-r--r--   0        0        0     5334 2020-02-02 00:00:00.000000 anycorn-0.17.2/src/anycorn/protocol/h3.py
+-rw-r--r--   0        0        0     7975 2020-02-02 00:00:00.000000 anycorn-0.17.2/src/anycorn/protocol/http_stream.py
+-rw-r--r--   0        0        0     5068 2020-02-02 00:00:00.000000 anycorn-0.17.2/src/anycorn/protocol/quic.py
+-rw-r--r--   0        0        0    14902 2020-02-02 00:00:00.000000 anycorn-0.17.2/src/anycorn/protocol/ws_stream.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anycorn-0.17.2/tests/__init__.py
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 anycorn-0.17.2/tests/conftest.py
+-rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 anycorn-0.17.2/tests/helpers.py
+-rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 anycorn-0.17.2/tests/test___main__.py
+-rw-r--r--   0        0        0     6025 2020-02-02 00:00:00.000000 anycorn-0.17.2/tests/test_app_wrappers.py
+-rw-r--r--   0        0        0     5800 2020-02-02 00:00:00.000000 anycorn-0.17.2/tests/test_config.py
+-rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 anycorn-0.17.2/tests/test_keep_alive.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 anycorn-0.17.2/tests/test_lifespan.py
+-rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 anycorn-0.17.2/tests/test_logging.py
+-rw-r--r--   0        0        0     8390 2020-02-02 00:00:00.000000 anycorn-0.17.2/tests/test_sanity.py
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 anycorn-0.17.2/tests/test_utils.py
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 anycorn-0.17.2/tests/assets/cert.pem
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 anycorn-0.17.2/tests/assets/config.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 anycorn-0.17.2/tests/assets/config.toml
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 anycorn-0.17.2/tests/assets/config_ssl.py
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 anycorn-0.17.2/tests/assets/key.pem
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anycorn-0.17.2/tests/middleware/__init__.py
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 anycorn-0.17.2/tests/middleware/test_dispatcher.py
+-rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 anycorn-0.17.2/tests/middleware/test_http_to_https.py
+-rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 anycorn-0.17.2/tests/middleware/test_proxy_fix.py
+-rwxr-xr-x   0        0        0    15366 2020-02-02 00:00:00.000000 anycorn-0.17.2/tests/protocol/test_h11.py
+-rw-r--r--   0        0        0     3542 2020-02-02 00:00:00.000000 anycorn-0.17.2/tests/protocol/test_h2.py
+-rw-r--r--   0        0        0     9873 2020-02-02 00:00:00.000000 anycorn-0.17.2/tests/protocol/test_http_stream.py
+-rw-r--r--   0        0        0    17121 2020-02-02 00:00:00.000000 anycorn-0.17.2/tests/protocol/test_ws_stream.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 anycorn-0.17.2/.gitignore
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 anycorn-0.17.2/LICENSE
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 anycorn-0.17.2/README.md
+-rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 anycorn-0.17.2/pyproject.toml
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 anycorn-0.17.2/PKG-INFO
```

### Comparing `anycorn-0.17.1/.pre-commit-config.yaml` & `anycorn-0.17.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/CHANGELOG.rst` & `anycorn-0.17.2/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/.github/workflows/ci.yml` & `anycorn-0.17.2/.github/workflows/ci.yml`

 * *Files 5% similar despite different names*

```diff
@@ -36,18 +36,18 @@
         python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
 
     steps:
       - uses: actions/checkout@v4
 
       - uses: actions/setup-python@v5
         with:
-          python-version: ${{ matrix.python }}
+          python-version: ${{ matrix.python-version }}
 
       - name: Install anycorn
-        run: pip install -e ".[test]"
+        run: python -m pip install -e ".[test]"
 
       - name: Check types
         if: ${{ (matrix.python-version == '3.12') && (matrix.os == 'ubuntu-latest') }}
         run: mypy src/anycorn/ tests/
 
       - name: Run tests
         run: pytest
@@ -63,18 +63,18 @@
 
       - uses: actions/setup-python@v5
         with:
           python-version: "3.12"
 
       - name: update pip
         run: |
-          pip install -U wheel
-          pip install -U setuptools
+          python -m pip install -U wheel
+          python -m pip install -U setuptools
           python -m pip install -U pip
-      - run: pip install trio .
+      - run: python -m pip install trio .
 
       - name: Run server
         working-directory: compliance/h2spec
         run: nohup anycorn --keyfile key.pem --certfile cert.pem http_server:app &
 
       - name: Download h2spec
         run: |
@@ -94,18 +94,18 @@
 
       - uses: actions/setup-python@v5
         with:
           python-version: "3.10"
 
       - name: update pip
         run: |
-          pip install -U wheel
-          pip install -U setuptools
+          python -m pip install -U wheel
+          python -m pip install -U setuptools
           python -m pip install -U pip
-      - run: python3 -m pip install trio .
+      - run: python -m pip install trio .
       - name: Run server
         working-directory: compliance/autobahn
         run: nohup anycorn ws_server:app &
 
       - name: Run Unit Tests
         working-directory: compliance/autobahn
         run: docker run --rm --network=host -v "${PWD}/:/config" -v "${PWD}/reports:/reports" --name fuzzingclient crossbario/autobahn-testsuite wstest -m fuzzingclient -s /config/fuzzingclient.json && python3 summarise.py
```

### Comparing `anycorn-0.17.1/.github/workflows/publish.yml` & `anycorn-0.17.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/compliance/autobahn/ws_server.py` & `anycorn-0.17.2/compliance/autobahn/ws_server.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/compliance/h2spec/cert.pem` & `anycorn-0.17.2/compliance/h2spec/cert.pem`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/compliance/h2spec/http_server.py` & `anycorn-0.17.2/compliance/h2spec/http_server.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/compliance/h2spec/key.pem` & `anycorn-0.17.2/compliance/h2spec/key.pem`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/src/anycorn/__init__.py` & `anycorn-0.17.2/src/anycorn/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from .config import Config
 from .run import worker_serve
 from .typing import Framework
 from .utils import wrap_app
 
 __all__ = ("Config", "serve")
-__version__ = "0.17.1"
+__version__ = "0.17.2"
 
 
 async def serve(
     app: Framework,
     config: Config,
     *,
     shutdown_trigger: Callable[..., Awaitable[None]] | None = None,
```

### Comparing `anycorn-0.17.1/src/anycorn/__main__.py` & `anycorn-0.17.2/src/anycorn/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,21 @@
         default=sentinel,
         type=int,
     )
     parser.add_argument(
         "-g", "--group", help="Group to own any unix sockets.", default=sentinel, type=int
     )
     parser.add_argument(
+        "-k",
+        "--worker-class",
+        dest="worker_class",
+        help="The type of worker to use. Options include asyncio and trio.",
+        default=sentinel,
+    )
+    parser.add_argument(
         "--keep-alive",
         help="Seconds to keep inactive connections alive for",
         default=sentinel,
         type=int,
     )
     parser.add_argument("--keyfile", help="Path to the SSL key file", default=sentinel)
     parser.add_argument(
@@ -270,14 +277,16 @@
         config.statsd_host = args.statsd_host
     if args.statsd_prefix is not sentinel:
         config.statsd_prefix = args.statsd_prefix
     if args.umask is not sentinel:
         config.umask = args.umask
     if args.user is not sentinel:
         config.user = args.user
+    if args.worker_class is not sentinel:
+        config.worker_class = args.worker_class
     if args.verify_mode is not sentinel:
         config.verify_mode = args.verify_mode
     if args.websocket_ping_interval is not sentinel:
         config.websocket_ping_interval = args.websocket_ping_interval
     if args.workers is not sentinel:
         config.workers = args.workers
```

### Comparing `anycorn-0.17.1/src/anycorn/app_wrappers.py` & `anycorn-0.17.2/src/anycorn/app_wrappers.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/src/anycorn/config.py` & `anycorn-0.17.2/src/anycorn/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,14 +104,15 @@
     umask: int | None = None
     use_reloader = False
     user: int | None = None
     verify_flags: VerifyFlags | None = None
     verify_mode: VerifyMode | None = None
     websocket_max_message_size = 16 * 1024 * 1024 * BYTES
     websocket_ping_interval: float | None = None
+    worker_class = "asyncio"
     workers = 1
     wsgi_max_body_size = 16 * 1024 * 1024 * BYTES
 
     def set_cert_reqs(self, value: int) -> None:
         warnings.warn("Please use verify_mode instead", Warning)
         self.verify_mode = VerifyMode(value)
```

### Comparing `anycorn-0.17.1/src/anycorn/lifespan.py` & `anycorn-0.17.2/src/anycorn/lifespan.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/src/anycorn/logging.py` & `anycorn-0.17.2/src/anycorn/logging.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/src/anycorn/run.py` & `anycorn-0.17.2/src/anycorn/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,9 +254,10 @@
     app = load_application(config.application_path, config.wsgi_max_body_size)
 
     shutdown_trigger = None
     if shutdown_event is not None:
         shutdown_trigger = partial(check_multiprocess_shutdown_event, shutdown_event, anyio.sleep)
 
     anyio.run(
-        partial(worker_serve, app, config, sockets=sockets, shutdown_trigger=shutdown_trigger)
+        partial(worker_serve, app, config, sockets=sockets, shutdown_trigger=shutdown_trigger),
+        backend=config.worker_class,
     )
```

### Comparing `anycorn-0.17.1/src/anycorn/statsd.py` & `anycorn-0.17.2/src/anycorn/statsd.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/src/anycorn/task_group.py` & `anycorn-0.17.2/src/anycorn/task_group.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/src/anycorn/tcp_server.py` & `anycorn-0.17.2/src/anycorn/tcp_server.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/src/anycorn/typing.py` & `anycorn-0.17.2/src/anycorn/typing.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/src/anycorn/udp_server.py` & `anycorn-0.17.2/src/anycorn/udp_server.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/src/anycorn/utils.py` & `anycorn-0.17.2/src/anycorn/utils.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/src/anycorn/worker_context.py` & `anycorn-0.17.2/src/anycorn/worker_context.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/src/anycorn/middleware/dispatcher.py` & `anycorn-0.17.2/src/anycorn/middleware/dispatcher.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/src/anycorn/middleware/http_to_https.py` & `anycorn-0.17.2/src/anycorn/middleware/http_to_https.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/src/anycorn/middleware/proxy_fix.py` & `anycorn-0.17.2/src/anycorn/middleware/proxy_fix.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/src/anycorn/middleware/wsgi.py` & `anycorn-0.17.2/src/anycorn/middleware/wsgi.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/src/anycorn/protocol/__init__.py` & `anycorn-0.17.2/src/anycorn/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/src/anycorn/protocol/events.py` & `anycorn-0.17.2/src/anycorn/protocol/events.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/src/anycorn/protocol/h11.py` & `anycorn-0.17.2/src/anycorn/protocol/h11.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/src/anycorn/protocol/h2.py` & `anycorn-0.17.2/src/anycorn/protocol/h2.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/src/anycorn/protocol/h3.py` & `anycorn-0.17.2/src/anycorn/protocol/h3.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/src/anycorn/protocol/http_stream.py` & `anycorn-0.17.2/src/anycorn/protocol/http_stream.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/src/anycorn/protocol/quic.py` & `anycorn-0.17.2/src/anycorn/protocol/quic.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/src/anycorn/protocol/ws_stream.py` & `anycorn-0.17.2/src/anycorn/protocol/ws_stream.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/tests/conftest.py` & `anycorn-0.17.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/tests/helpers.py` & `anycorn-0.17.2/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/tests/test___main__.py` & `anycorn-0.17.2/tests/test___main__.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/tests/test_app_wrappers.py` & `anycorn-0.17.2/tests/test_app_wrappers.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/tests/test_config.py` & `anycorn-0.17.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/tests/test_keep_alive.py` & `anycorn-0.17.2/tests/test_keep_alive.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/tests/test_lifespan.py` & `anycorn-0.17.2/tests/test_lifespan.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/tests/test_logging.py` & `anycorn-0.17.2/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/tests/test_sanity.py` & `anycorn-0.17.2/tests/test_sanity.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/tests/test_utils.py` & `anycorn-0.17.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/tests/assets/cert.pem` & `anycorn-0.17.2/tests/assets/cert.pem`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/tests/assets/key.pem` & `anycorn-0.17.2/tests/assets/key.pem`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/tests/middleware/test_dispatcher.py` & `anycorn-0.17.2/tests/middleware/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/tests/middleware/test_http_to_https.py` & `anycorn-0.17.2/tests/middleware/test_http_to_https.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/tests/middleware/test_proxy_fix.py` & `anycorn-0.17.2/tests/middleware/test_proxy_fix.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/tests/protocol/test_h11.py` & `anycorn-0.17.2/tests/protocol/test_h11.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/tests/protocol/test_h2.py` & `anycorn-0.17.2/tests/protocol/test_h2.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/tests/protocol/test_http_stream.py` & `anycorn-0.17.2/tests/protocol/test_http_stream.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/tests/protocol/test_ws_stream.py` & `anycorn-0.17.2/tests/protocol/test_ws_stream.py`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/LICENSE` & `anycorn-0.17.2/LICENSE`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/README.md` & `anycorn-0.17.2/README.md`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/pyproject.toml` & `anycorn-0.17.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `anycorn-0.17.1/PKG-INFO` & `anycorn-0.17.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: anycorn
-Version: 0.17.1
+Version: 0.17.2
 Summary: A fork of Hypercorn that uses AnyIO
 Author-email: Philip Graham Jones <philip.graham.jones@googlemail.com>, David Brochart <david.brochart@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```


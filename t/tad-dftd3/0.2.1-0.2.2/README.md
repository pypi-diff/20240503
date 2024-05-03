# Comparing `tmp/tad_dftd3-0.2.1.tar.gz` & `tmp/tad_dftd3-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tad_dftd3-0.2.1.tar", last modified: Fri Apr 26 18:44:39 2024, max compression
+gzip compressed data, was "tad_dftd3-0.2.2.tar", last modified: Fri May  3 15:45:24 2024, max compression
```

## Comparing `tad_dftd3-0.2.1.tar` & `tad_dftd3-0.2.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-26 18:44:39.796524 tad_dftd3-0.2.1/
--rw-rw-r--   0 marvin    (1000) marvin    (1000)    11358 2024-01-17 17:30:51.000000 tad_dftd3-0.2.1/LICENSE
--rw-r--r--   0 marvin    (1000) marvin    (1000)    12580 2024-04-26 18:44:39.796524 tad_dftd3-0.2.1/PKG-INFO
--rw-rw-r--   0 marvin    (1000) marvin    (1000)    11010 2024-04-26 18:44:27.000000 tad_dftd3-0.2.1/README.rst
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     1306 2024-01-17 17:30:51.000000 tad_dftd3-0.2.1/pyproject.toml
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     1312 2024-04-26 18:44:39.796524 tad_dftd3-0.2.1/setup.cfg
--rw-rw-r--   0 marvin    (1000) marvin    (1000)      679 2024-01-17 17:30:51.000000 tad_dftd3-0.2.1/setup.py
-drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-26 18:44:39.772524 tad_dftd3-0.2.1/src/
-drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-26 18:44:39.788524 tad_dftd3-0.2.1/src/tad_dftd3/
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     3485 2024-04-09 21:13:38.000000 tad_dftd3-0.2.1/src/tad_dftd3/__init__.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)      672 2024-04-26 18:44:27.000000 tad_dftd3-0.2.1/src/tad_dftd3/__version__.py
-drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-26 18:44:39.792524 tad_dftd3-0.2.1/src/tad_dftd3/damping/
--rw-rw-r--   0 marvin    (1000) marvin    (1000)      762 2024-01-17 17:30:51.000000 tad_dftd3-0.2.1/src/tad_dftd3/damping/__init__.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     4772 2024-01-17 17:30:51.000000 tad_dftd3-0.2.1/src/tad_dftd3/damping/atm.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     1990 2024-01-17 17:30:51.000000 tad_dftd3-0.2.1/src/tad_dftd3/damping/rational.py
-drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-26 18:44:39.792524 tad_dftd3-0.2.1/src/tad_dftd3/data/
--rw-rw-r--   0 marvin    (1000) marvin    (1000)      761 2024-01-17 17:30:51.000000 tad_dftd3-0.2.1/src/tad_dftd3/data/__init__.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     2464 2024-01-17 17:30:51.000000 tad_dftd3-0.2.1/src/tad_dftd3/data/r4r2.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     1761 2024-01-17 17:30:51.000000 tad_dftd3-0.2.1/src/tad_dftd3/data/radii.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)    87275 2024-01-17 17:30:51.000000 tad_dftd3-0.2.1/src/tad_dftd3/data/vdw-d3.pt
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     1671 2024-04-09 21:13:38.000000 tad_dftd3-0.2.1/src/tad_dftd3/defaults.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)    10789 2024-04-26 18:44:27.000000 tad_dftd3-0.2.1/src/tad_dftd3/disp.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)      832 2024-01-17 17:30:51.000000 tad_dftd3-0.2.1/src/tad_dftd3/exception.py
-drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-26 18:44:39.796524 tad_dftd3-0.2.1/src/tad_dftd3/model/
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     1707 2024-04-26 18:44:27.000000 tad_dftd3-0.2.1/src/tad_dftd3/model/__init__.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)    12518 2024-04-26 18:44:27.000000 tad_dftd3-0.2.1/src/tad_dftd3/model/c6.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     6070 2024-04-26 18:44:27.000000 tad_dftd3-0.2.1/src/tad_dftd3/model/weights.py
-drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-26 18:44:39.796524 tad_dftd3-0.2.1/src/tad_dftd3/ncoord/
--rw-rw-r--   0 marvin    (1000) marvin    (1000)      861 2024-04-09 21:13:38.000000 tad_dftd3-0.2.1/src/tad_dftd3/ncoord/__init__.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)        0 2024-01-17 17:30:51.000000 tad_dftd3-0.2.1/src/tad_dftd3/py.typed
--rw-rw-r--   0 marvin    (1000) marvin    (1000)  4240619 2024-01-17 17:30:51.000000 tad_dftd3-0.2.1/src/tad_dftd3/reference-c6.pt
--rw-rw-r--   0 marvin    (1000) marvin    (1000)    15344 2024-04-09 21:13:38.000000 tad_dftd3-0.2.1/src/tad_dftd3/reference.py
-drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-26 18:44:39.796524 tad_dftd3-0.2.1/src/tad_dftd3/typing/
--rw-rw-r--   0 marvin    (1000) marvin    (1000)      756 2024-01-17 17:30:51.000000 tad_dftd3-0.2.1/src/tad_dftd3/typing/__init__.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)      921 2024-04-26 18:44:27.000000 tad_dftd3-0.2.1/src/tad_dftd3/typing/builtin.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)      822 2024-01-17 17:30:51.000000 tad_dftd3-0.2.1/src/tad_dftd3/typing/d3.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     1097 2024-04-26 18:44:27.000000 tad_dftd3-0.2.1/src/tad_dftd3/typing/pytorch.py
-drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-26 18:44:39.796524 tad_dftd3-0.2.1/src/tad_dftd3.egg-info/
--rw-r--r--   0 marvin    (1000) marvin    (1000)    12580 2024-04-26 18:44:39.000000 tad_dftd3-0.2.1/src/tad_dftd3.egg-info/PKG-INFO
--rw-rw-r--   0 marvin    (1000) marvin    (1000)      904 2024-04-26 18:44:39.000000 tad_dftd3-0.2.1/src/tad_dftd3.egg-info/SOURCES.txt
--rw-rw-r--   0 marvin    (1000) marvin    (1000)        1 2024-04-26 18:44:39.000000 tad_dftd3-0.2.1/src/tad_dftd3.egg-info/dependency_links.txt
--rw-rw-r--   0 marvin    (1000) marvin    (1000)      194 2024-04-26 18:44:39.000000 tad_dftd3-0.2.1/src/tad_dftd3.egg-info/requires.txt
--rw-rw-r--   0 marvin    (1000) marvin    (1000)       10 2024-04-26 18:44:39.000000 tad_dftd3-0.2.1/src/tad_dftd3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:45:24.489815 tad_dftd3-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-03 15:45:20.000000 tad_dftd3-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12580 2024-05-03 15:45:24.489815 tad_dftd3-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11010 2024-05-03 15:45:20.000000 tad_dftd3-0.2.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-03 15:45:20.000000 tad_dftd3-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-03 15:45:24.493815 tad_dftd3-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-03 15:45:20.000000 tad_dftd3-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:45:24.473815 tad_dftd3-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:45:24.485815 tad_dftd3-0.2.2/src/tad_dftd3/
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-05-03 15:45:20.000000 tad_dftd3-0.2.2/src/tad_dftd3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-03 15:45:20.000000 tad_dftd3-0.2.2/src/tad_dftd3/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:45:24.485815 tad_dftd3-0.2.2/src/tad_dftd3/damping/
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-03 15:45:20.000000 tad_dftd3-0.2.2/src/tad_dftd3/damping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4772 2024-05-03 15:45:20.000000 tad_dftd3-0.2.2/src/tad_dftd3/damping/atm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-03 15:45:20.000000 tad_dftd3-0.2.2/src/tad_dftd3/damping/rational.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:45:24.485815 tad_dftd3-0.2.2/src/tad_dftd3/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-03 15:45:20.000000 tad_dftd3-0.2.2/src/tad_dftd3/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-03 15:45:20.000000 tad_dftd3-0.2.2/src/tad_dftd3/data/r4r2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-03 15:45:20.000000 tad_dftd3-0.2.2/src/tad_dftd3/data/radii.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87275 2024-05-03 15:45:20.000000 tad_dftd3-0.2.2/src/tad_dftd3/data/vdw-d3.pt
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-03 15:45:20.000000 tad_dftd3-0.2.2/src/tad_dftd3/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-05-03 15:45:20.000000 tad_dftd3-0.2.2/src/tad_dftd3/disp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-03 15:45:20.000000 tad_dftd3-0.2.2/src/tad_dftd3/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:45:24.485815 tad_dftd3-0.2.2/src/tad_dftd3/model/
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-03 15:45:20.000000 tad_dftd3-0.2.2/src/tad_dftd3/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13476 2024-05-03 15:45:20.000000 tad_dftd3-0.2.2/src/tad_dftd3/model/c6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6070 2024-05-03 15:45:20.000000 tad_dftd3-0.2.2/src/tad_dftd3/model/weights.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:45:24.485815 tad_dftd3-0.2.2/src/tad_dftd3/ncoord/
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-03 15:45:20.000000 tad_dftd3-0.2.2/src/tad_dftd3/ncoord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:45:20.000000 tad_dftd3-0.2.2/src/tad_dftd3/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)  4240619 2024-05-03 15:45:20.000000 tad_dftd3-0.2.2/src/tad_dftd3/reference-c6.pt
+-rw-r--r--   0 runner    (1001) docker     (127)    15344 2024-05-03 15:45:20.000000 tad_dftd3-0.2.2/src/tad_dftd3/reference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:45:24.489815 tad_dftd3-0.2.2/src/tad_dftd3/typing/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-03 15:45:20.000000 tad_dftd3-0.2.2/src/tad_dftd3/typing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-03 15:45:20.000000 tad_dftd3-0.2.2/src/tad_dftd3/typing/builtin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-03 15:45:20.000000 tad_dftd3-0.2.2/src/tad_dftd3/typing/d3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-03 15:45:20.000000 tad_dftd3-0.2.2/src/tad_dftd3/typing/pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:45:24.489815 tad_dftd3-0.2.2/src/tad_dftd3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12580 2024-05-03 15:45:24.000000 tad_dftd3-0.2.2/src/tad_dftd3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-03 15:45:24.000000 tad_dftd3-0.2.2/src/tad_dftd3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 15:45:24.000000 tad_dftd3-0.2.2/src/tad_dftd3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-03 15:45:24.000000 tad_dftd3-0.2.2/src/tad_dftd3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-03 15:45:24.000000 tad_dftd3-0.2.2/src/tad_dftd3.egg-info/top_level.txt
```

### Comparing `tad_dftd3-0.2.1/LICENSE` & `tad_dftd3-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.2.1/PKG-INFO` & `tad_dftd3-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tad_dftd3
-Version: 0.2.1
+Version: 0.2.2
 Summary: Torch autodiff DFT-D3 implementation
 License: Apache-2.0
 Project-URL: Documentation, https://tad-dftd3.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/dftd3/tad-dftd3
 Project-URL: Tracker, https://github.com/dftd3/tad-dftd3/issues
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tad_dftd3-0.2.1/README.rst` & `tad_dftd3-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.2.1/pyproject.toml` & `tad_dftd3-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.2.1/setup.cfg` & `tad_dftd3-0.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.2.1/setup.py` & `tad_dftd3-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.2.1/src/tad_dftd3/__init__.py` & `tad_dftd3-0.2.2/src/tad_dftd3/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.2.1/src/tad_dftd3/__version__.py` & `tad_dftd3-0.2.2/src/tad_dftd3/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
 Version module for *tad-dftd3*.
 """
-__version__ = "0.2.1"
+__version__ = "0.2.2"
```

### Comparing `tad_dftd3-0.2.1/src/tad_dftd3/damping/__init__.py` & `tad_dftd3-0.2.2/src/tad_dftd3/damping/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.2.1/src/tad_dftd3/damping/atm.py` & `tad_dftd3-0.2.2/src/tad_dftd3/damping/atm.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.2.1/src/tad_dftd3/damping/rational.py` & `tad_dftd3-0.2.2/src/tad_dftd3/damping/rational.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.2.1/src/tad_dftd3/data/__init__.py` & `tad_dftd3-0.2.2/src/tad_dftd3/data/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.2.1/src/tad_dftd3/data/r4r2.py` & `tad_dftd3-0.2.2/src/tad_dftd3/data/r4r2.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.2.1/src/tad_dftd3/data/radii.py` & `tad_dftd3-0.2.2/src/tad_dftd3/data/radii.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.2.1/src/tad_dftd3/data/vdw-d3.pt` & `tad_dftd3-0.2.2/src/tad_dftd3/data/vdw-d3.pt`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.2.1/src/tad_dftd3/defaults.py` & `tad_dftd3-0.2.2/src/tad_dftd3/defaults.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.2.1/src/tad_dftd3/disp.py` & `tad_dftd3-0.2.2/src/tad_dftd3/disp.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.2.1/src/tad_dftd3/exception.py` & `tad_dftd3-0.2.2/src/tad_dftd3/exception.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.2.1/src/tad_dftd3/model/__init__.py` & `tad_dftd3-0.2.2/src/tad_dftd3/model/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.2.1/src/tad_dftd3/model/c6.py` & `tad_dftd3-0.2.2/src/tad_dftd3/model/c6.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,14 +65,33 @@
     Returns
     -------
     Tensor
         Atomic dispersion coefficients of shape `(..., nat, nat)`.
     """
     _check_memory(numbers, weights, chunk_size)
 
+    # PyTorch 2.0.x has a bug with functorch and custom autograd functions as
+    # documented in: https://github.com/pytorch/pytorch/issues/99973
+    #
+    # RuntimeError: unwrapped_count > 0 INTERNAL ASSERT FAILED at "../aten/src/
+    # ATen/functorch/TensorWrapper.cpp":202, please report a bug to PyTorch.
+    # Should have at least one dead wrapper
+    #
+    # Hence, we cannot use the custom backwards for reduced memory consumption.
+    if __tversion__[0] == 2 and __tversion__[1] == 0:  # pragma: no cover
+        track_weights = torch._C._functorch.is_gradtrackingtensor(weights)
+        track_numbers = torch._C._functorch.is_gradtrackingtensor(numbers)
+        if track_weights or track_numbers:
+
+            if chunk_size is None:
+                return _atomic_c6_full(numbers, weights, reference)
+
+            return _atomic_c6_chunked(numbers, weights, reference, chunk_size)
+
+    # Use custom autograd function for reduced memory consumption
     AtomicC6 = AtomicC6_V1 if __tversion__ < (2, 0, 0) else AtomicC6_V2
     res = AtomicC6.apply(numbers, weights, reference, chunk_size)
     assert res is not None
     return res
 
 
 # helpers
```

### Comparing `tad_dftd3-0.2.1/src/tad_dftd3/model/weights.py` & `tad_dftd3-0.2.2/src/tad_dftd3/model/weights.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.2.1/src/tad_dftd3/ncoord/__init__.py` & `tad_dftd3-0.2.2/src/tad_dftd3/ncoord/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.2.1/src/tad_dftd3/reference-c6.pt` & `tad_dftd3-0.2.2/src/tad_dftd3/reference-c6.pt`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.2.1/src/tad_dftd3/reference.py` & `tad_dftd3-0.2.2/src/tad_dftd3/reference.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.2.1/src/tad_dftd3/typing/__init__.py` & `tad_dftd3-0.2.2/src/tad_dftd3/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.2.1/src/tad_dftd3/typing/builtin.py` & `tad_dftd3-0.2.2/src/tad_dftd3/typing/builtin.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.2.1/src/tad_dftd3/typing/d3.py` & `tad_dftd3-0.2.2/src/tad_dftd3/typing/d3.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.2.1/src/tad_dftd3/typing/pytorch.py` & `tad_dftd3-0.2.2/src/tad_dftd3/typing/pytorch.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.2.1/src/tad_dftd3.egg-info/PKG-INFO` & `tad_dftd3-0.2.2/src/tad_dftd3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tad_dftd3
-Version: 0.2.1
+Version: 0.2.2
 Summary: Torch autodiff DFT-D3 implementation
 License: Apache-2.0
 Project-URL: Documentation, https://tad-dftd3.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/dftd3/tad-dftd3
 Project-URL: Tracker, https://github.com/dftd3/tad-dftd3/issues
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tad_dftd3-0.2.1/src/tad_dftd3.egg-info/SOURCES.txt` & `tad_dftd3-0.2.2/src/tad_dftd3.egg-info/SOURCES.txt`

 * *Files identical despite different names*


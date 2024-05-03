# Comparing `tmp/intersphinx_registry-0.0.1.tar.gz` & `tmp/intersphinx_registry-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intersphinx_registry-0.0.1.tar", last modified: Fri May  3 09:28:50 2024, max compression
+gzip compressed data, was "intersphinx_registry-0.0.2.tar", last modified: Fri May  3 13:40:48 2024, max compression
```

## Comparing `intersphinx_registry-0.0.1.tar` & `intersphinx_registry-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0     1086 2024-05-03 07:52:01.783580 intersphinx_registry-0.0.1/LICENSE
--rw-r--r--   0        0        0      969 2024-05-03 09:27:52.385967 intersphinx_registry-0.0.1/README.md
--rw-r--r--   0        0        0      548 2024-05-03 09:19:19.810226 intersphinx_registry-0.0.1/intersphinx_registry/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 07:55:04.206909 intersphinx_registry-0.0.1/intersphinx_registry/py.typed
--rw-r--r--   0        0        0     9187 2024-05-03 09:18:44.675639 intersphinx_registry-0.0.1/intersphinx_registry/registry.json
--rw-r--r--   0        0        0      406 2024-05-03 07:52:01.783820 intersphinx_registry-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      339 1970-01-01 00:00:00.000000 intersphinx_registry-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        6 2024-05-03 12:40:56.982097 intersphinx_registry-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1086 2024-05-03 07:52:01.783580 intersphinx_registry-0.0.2/LICENSE
+-rw-r--r--   0        0        0      975 2024-05-03 09:31:21.573054 intersphinx_registry-0.0.2/README.md
+-rw-r--r--   0        0        0     1186 2024-05-03 13:31:30.245018 intersphinx_registry-0.0.2/intersphinx_registry/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 07:55:04.206909 intersphinx_registry-0.0.2/intersphinx_registry/py.typed
+-rw-r--r--   0        0        0     9197 2024-05-03 12:41:46.514755 intersphinx_registry-0.0.2/intersphinx_registry/registry.json
+-rw-r--r--   0        0        0      637 2024-05-03 13:38:36.749859 intersphinx_registry-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      747 2024-05-03 13:36:03.207243 intersphinx_registry-0.0.2/tests/test_basic.py
+-rw-r--r--   0        0        0     1514 1970-01-01 00:00:00.000000 intersphinx_registry-0.0.2/PKG-INFO
```

### Comparing `intersphinx_registry-0.0.1/LICENSE` & `intersphinx_registry-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `intersphinx_registry-0.0.1/README.md` & `intersphinx_registry-0.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Intersphinx Registry
 
 A simple utility package that provide default inter sphinx mapping for a large chunk of the python ecosystem.
 
 Usage in `conf.py`
 
-```
+```python
 from intersphinx_registry import get_intersphinx_mapping
 
 # ...
 
 intersphinx_mapping = get_intersphinx_mapping()
 intersphinx_mapping.update({
     'overwrite': ('<url>', None),
```

### Comparing `intersphinx_registry-0.0.1/intersphinx_registry/registry.json` & `intersphinx_registry-0.0.2/intersphinx_registry/registry.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9319248826291084%*

 * *Differences: {"'bokeh'": "{insert: [(0, 'https://docs.bokeh.org/en/latest/')], delete: [0]}",*

 * * "'cython'": "{insert: [(0, 'https://docs.cython.org/en/latest/')], delete: [0]}",*

 * * "'dask'": "{insert: [(0, 'https://docs.dask.org/en/latest/')], delete: [0]}",*

 * * "'devpi'": "{insert: [(0, 'https://devpi.net/docs/devpi/devpi/latest/+doc/')], delete: [0]}",*

 * * "'dlpack'": "{insert: [(0, 'https://dmlc.github.io/dlpack/latest/')], delete: [0]}",*

 * * "'imageio'": "{insert: [(0, 'https://imageio.readthedocs.io/en/stable/')], delete: [0]} […]*

```diff
@@ -32,15 +32,15 @@
         null
     ],
     "bhub": [
         "https://binderhub.readthedocs.io/en/latest/",
         null
     ],
     "bokeh": [
-        "https://docs.bokeh.org/en/latest",
+        "https://docs.bokeh.org/en/latest/",
         null
     ],
     "boltons": [
         "https://boltons.readthedocs.io/en/latest/",
         null
     ],
     "bottle": [
@@ -68,31 +68,31 @@
         null
     ],
     "cycler": [
         "https://matplotlib.org/cycler/",
         null
     ],
     "cython": [
-        "https://docs.cython.org/en/latest",
+        "https://docs.cython.org/en/latest/",
         null
     ],
     "dask": [
-        "https://docs.dask.org/en/latest",
+        "https://docs.dask.org/en/latest/",
         null
     ],
     "dateutil": [
         "https://dateutil.readthedocs.io/en/latest/",
         null
     ],
     "devguide": [
         "https://devguide.python.org/",
         null
     ],
     "devpi": [
-        "https://devpi.net/docs/devpi/devpi/latest/+doc",
+        "https://devpi.net/docs/devpi/devpi/latest/+doc/",
         null
     ],
     "dh-virtualenv": [
         "https://dh-virtualenv.readthedocs.io/en/latest/",
         null
     ],
     "distlib": [
@@ -104,15 +104,15 @@
         null
     ],
     "django": [
         "https://docs.djangoproject.com/en/2.2/",
         "https://docs.djangoproject.com/en/2.2/_objects/"
     ],
     "dlpack": [
-        "https://dmlc.github.io/dlpack/latest",
+        "https://dmlc.github.io/dlpack/latest/",
         null
     ],
     "flax": [
         "https://flax.readthedocs.io/en/latest/",
         null
     ],
     "flexx": [
@@ -128,19 +128,19 @@
         null
     ],
     "hub": [
         "https://jupyterhub.readthedocs.io/en/latest/",
         null
     ],
     "imageio": [
-        "https://imageio.readthedocs.io/en/stable",
+        "https://imageio.readthedocs.io/en/stable/",
         null
     ],
     "importlib-resources": [
-        "https://importlib-resources.readthedocs.io/en/latest",
+        "https://importlib-resources.readthedocs.io/en/latest/",
         null
     ],
     "ipykernel": [
         "https://ipykernel.readthedocs.io/en/latest/",
         null
     ],
     "ipyleaflet": [
@@ -164,19 +164,19 @@
         null
     ],
     "jedi": [
         "https://jedi.readthedocs.io/en/latest/",
         null
     ],
     "jinja": [
-        "http://jinja.pocoo.org/docs",
+        "http://jinja.pocoo.org/docs/",
         null
     ],
     "jupyter": [
-        "https://jupyter.readthedocs.io/en/latest",
+        "https://jupyter.readthedocs.io/en/latest/",
         null
     ],
     "jupyter-server": [
         "https://jupyter-server.readthedocs.io/en/stable/",
         null
     ],
     "jupyter_core": [
@@ -220,27 +220,27 @@
         null
     ],
     "magicgui": [
         "https://pyapp-kit.github.io/magicgui/",
         null
     ],
     "markdown_it": [
-        "https://markdown-it-py.readthedocs.io/en/latest",
+        "https://markdown-it-py.readthedocs.io/en/latest/",
         null
     ],
     "matplotlib": [
         "https://matplotlib.org/stable/",
         null
     ],
     "meson-python": [
         "https://meson-python.readthedocs.io/en/stable/",
         null
     ],
     "monkeytype": [
-        "https://monkeytype.readthedocs.io/en/latest",
+        "https://monkeytype.readthedocs.io/en/latest/",
         null
     ],
     "mpmath": [
         "https://mpmath.org/doc/current/",
         null
     ],
     "myst-nb": [
@@ -280,31 +280,31 @@
         null
     ],
     "networkx": [
         "https://networkx.org/documentation/stable/",
         null
     ],
     "notebook": [
-        "https://jupyter-notebook.readthedocs.org/en/stable/",
+        "https://jupyter-notebook.readthedocs.io/en/stable/",
         null
     ],
     "nox": [
         "https://nox.thea.codes/en/latest/",
         null
     ],
     "numpy": [
         "https://numpy.org/doc/stable/",
         null
     ],
     "numpy-tutorials": [
-        "https://numpy.org/numpy-tutorials",
+        "https://numpy.org/numpy-tutorials/",
         null
     ],
     "numpydoc": [
-        "https://numpydoc.readthedocs.io/en/latest",
+        "https://numpydoc.readthedocs.io/en/latest/",
         null
     ],
     "nx-guides": [
         "https://networkx.org/nx-guides/",
         null
     ],
     "openstack": [
@@ -332,19 +332,19 @@
         null
     ],
     "piwheels": [
         "https://piwheels.readthedocs.io/en/latest/",
         null
     ],
     "pluggy": [
-        "https://pluggy.readthedocs.io/en/stable",
+        "https://pluggy.readthedocs.io/en/stable/",
         null
     ],
     "poliastro": [
-        "https://docs.poliastro.space/en/v0.15.2/",
+        "https://docs.poliastro.space/en/stable/",
         null
     ],
     "prompt_toolkit": [
         "https://python-prompt-toolkit.readthedocs.io/en/stable/",
         null
     ],
     "py": [
@@ -384,47 +384,47 @@
         null
     ],
     "pypug": [
         "https://packaging.python.org/",
         null
     ],
     "pypy": [
-        "http://pypy.readthedocs.org/en/latest/",
+        "https://pypy.readthedocs.io/en/latest/",
         null
     ],
     "pyro": [
-        "http://docs.pyro.ai/en/stable/",
+        "https://docs.pyro.ai/en/stable/",
         null
     ],
     "pytest": [
         "https://pytest.org/en/stable/",
         null
     ],
     "python": [
         "https://docs.python.org/3/",
         null
     ],
     "python-guide": [
-        "https://docs.python-guide.org",
+        "https://docs.python-guide.org/",
         null
     ],
     "pytorch_lightning": [
         "https://pytorch-lightning.readthedocs.io/en/stable/",
         null
     ],
     "qiskit": [
-        "https://qiskit.org/documentation/",
+        "https://docs.quantum.ibm.com/api/qiskit/",
         null
     ],
     "qtconsole": [
         "https://jupyter.org/qtconsole/dev/",
         null
     ],
     "readthedocs": [
-        "https://docs.readthedocs.io/en/stable",
+        "https://docs.readthedocs.io/en/stable/",
         null
     ],
     "requests": [
         "https://docs.python-requests.org/en/latest/",
         null
     ],
     "rpy2": [
@@ -448,31 +448,31 @@
         null
     ],
     "scipy": [
         "https://docs.scipy.org/doc/scipy/reference/",
         null
     ],
     "scipy-lecture-notes": [
-        "https://scipy-lectures.org",
+        "https://scipy-lectures.org/",
         null
     ],
     "scriptconfig": [
         "https://scriptconfig.readthedocs.io/en/latest/",
         null
     ],
     "server": [
-        "https://jupyter-server.readthedocs.org/en/stable",
+        "https://jupyter-server.readthedocs.io/en/stable/",
         null
     ],
     "setuptools": [
-        "https://setuptools.pypa.io/en/stable",
+        "https://setuptools.pypa.io/en/stable/",
         null
     ],
     "six": [
-        "https://six.readthedocs.io",
+        "https://six.readthedocs.io/",
         null
     ],
     "skimage": [
         "https://scikit-image.org/docs/stable/",
         null
     ],
     "spack": [
@@ -496,15 +496,15 @@
         null
     ],
     "sqlalchemy": [
         "https://docs.sqlalchemy.org/en/latest/",
         null
     ],
     "statsmodels": [
-        "https://www.statsmodels.org/stable",
+        "https://www.statsmodels.org/stable/",
         null
     ],
     "sympy": [
         "https://docs.sympy.org/latest/",
         null
     ],
     "tljh": [
@@ -516,19 +516,19 @@
         null
     ],
     "tornado": [
         "https://www.tornadoweb.org/en/stable/",
         null
     ],
     "tox": [
-        "https://tox.wiki/en/stable",
+        "https://tox.wiki/en/stable/",
         null
     ],
     "traitlets": [
-        "https://traitlets.readthedocs.io/en/stable/",
+        "https://traitlets.readthedocs.io/en/latest/",
         null
     ],
     "twine": [
         "https://twine.readthedocs.io/en/stable/",
         null
     ],
     "typing": [
@@ -556,15 +556,15 @@
         null
     ],
     "xdoctest": [
         "https://xdoctest.readthedocs.io/en/latest/",
         null
     ],
     "z2jh": [
-        "https://zero-to-jupyterhub.readthedocs.io/en/latest/",
+        "https://z2jh.jupyter.org/en/latest/",
         null
     ],
     "zarr": [
         "https://zarr.readthedocs.io/en/latest/",
         null
     ]
 }
```


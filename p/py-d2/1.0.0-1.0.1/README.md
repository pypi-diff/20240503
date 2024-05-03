# Comparing `tmp/py_d2-1.0.0.tar.gz` & `tmp/py_d2-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_d2-1.0.0.tar", max compression
+gzip compressed data, was "py_d2-1.0.1.tar", max compression
```

## Comparing `py_d2-1.0.0.tar` & `py_d2-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1061 2023-05-27 10:38:08.216752 py_d2-1.0.0/LICENSE
--rw-r--r--   0        0        0     2600 2023-05-27 10:38:08.216752 py_d2-1.0.0/README.md
--rw-r--r--   0        0        0     5044 2023-05-27 10:38:08.220752 py_d2-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      296 2023-05-27 10:38:08.220752 py_d2-1.0.0/src/py_d2/__init__.py
--rw-r--r--   0        0        0      710 2023-05-27 10:38:08.220752 py_d2-1.0.0/src/py_d2/connection.py
--rw-r--r--   0        0        0      782 2023-05-27 10:38:08.220752 py_d2-1.0.0/src/py_d2/diagram.py
--rw-r--r--   0        0        0      796 2023-05-27 10:38:08.220752 py_d2-1.0.0/src/py_d2/helpers.py
--rw-r--r--   0        0        0      721 2023-05-27 10:38:08.220752 py_d2-1.0.0/src/py_d2/main.py
--rw-r--r--   0        0        0     3625 2023-05-27 10:38:08.224752 py_d2-1.0.0/src/py_d2/shape.py
--rw-r--r--   0        0        0     1642 2023-05-27 10:38:08.224752 py_d2-1.0.0/src/py_d2/style.py
--rw-r--r--   0        0        0     3511 1970-01-01 00:00:00.000000 py_d2-1.0.0/setup.py
--rw-r--r--   0        0        0     3546 1970-01-01 00:00:00.000000 py_d2-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-05-03 06:24:47.788966 py_d2-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2600 2024-05-03 06:24:47.788966 py_d2-1.0.1/README.md
+-rw-r--r--   0        0        0     5044 2024-05-03 06:24:47.796966 py_d2-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      296 2024-05-03 06:24:47.796966 py_d2-1.0.1/src/py_d2/__init__.py
+-rw-r--r--   0        0        0     1088 2024-05-03 06:24:47.796966 py_d2-1.0.1/src/py_d2/connection.py
+-rw-r--r--   0        0        0      782 2024-05-03 06:24:47.796966 py_d2-1.0.1/src/py_d2/diagram.py
+-rw-r--r--   0        0        0      796 2024-05-03 06:24:47.796966 py_d2-1.0.1/src/py_d2/helpers.py
+-rw-r--r--   0        0        0      721 2024-05-03 06:24:47.796966 py_d2-1.0.1/src/py_d2/main.py
+-rw-r--r--   0        0        0     3625 2024-05-03 06:24:47.796966 py_d2-1.0.1/src/py_d2/shape.py
+-rw-r--r--   0        0        0     1642 2024-05-03 06:24:47.796966 py_d2-1.0.1/src/py_d2/style.py
+-rw-r--r--   0        0        0     3511 1970-01-01 00:00:00.000000 py_d2-1.0.1/setup.py
+-rw-r--r--   0        0        0     3546 1970-01-01 00:00:00.000000 py_d2-1.0.1/PKG-INFO
```

### Comparing `py_d2-1.0.0/LICENSE` & `py_d2-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_d2-1.0.0/README.md` & `py_d2-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `py_d2-1.0.0/pyproject.toml` & `py_d2-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-d2"
-version = "1.0.0"
+version = "1.0.1"
 description = "An unofficial, fully typed python interface for building .d2 graph files in python."
 authors = ["David Revay <daverevay@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://mrblenny.github.io/py-d2/"
 repository = "https://github.com/mrblenny/py-d2"
 documentation = "https://github.com/MrBlenny/py-d2/blob/main/README.md"
```

### Comparing `py_d2-1.0.0/src/py_d2/connection.py` & `py_d2-1.0.1/src/py_d2/connection.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,7 +22,20 @@
         base = f"{self.shape_1} {self.direction.value} {self.shape_2}"
         if self.label:
             base += f": {self.label}"
         return [base]
 
     def __repr__(self) -> str:
         return "\n".join(self.lines())
+
+    def __hash__(self):
+        return hash((self.shape_1, self.shape_2, self.label, self.direction))
+
+    def __eq__(self, other) -> bool:
+        if (self.shape_1, self.shape_2, self.direction, self.label) == (
+            other.shape_1,
+            other.shape_2,
+            other.direction,
+            other.label,
+        ):
+            return True
+        return False
```

### Comparing `py_d2-1.0.0/src/py_d2/diagram.py` & `py_d2-1.0.1/src/py_d2/diagram.py`

 * *Files identical despite different names*

### Comparing `py_d2-1.0.0/src/py_d2/helpers.py` & `py_d2-1.0.1/src/py_d2/helpers.py`

 * *Files identical despite different names*

### Comparing `py_d2-1.0.0/src/py_d2/main.py` & `py_d2-1.0.1/src/py_d2/main.py`

 * *Files identical despite different names*

### Comparing `py_d2-1.0.0/src/py_d2/shape.py` & `py_d2-1.0.1/src/py_d2/shape.py`

 * *Files identical despite different names*

### Comparing `py_d2-1.0.0/src/py_d2/style.py` & `py_d2-1.0.1/src/py_d2/style.py`

 * *Files identical despite different names*

### Comparing `py_d2-1.0.0/setup.py` & `py_d2-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 entry_points = \
 {'console_scripts': ['example = py_d2.main:example']}
 
 setup_kwargs = {
     'name': 'py-d2',
-    'version': '1.0.0',
+    'version': '1.0.1',
     'description': 'An unofficial, fully typed python interface for building .d2 graph files in python.',
     'long_description': '# py-d2\n\n![Banner](docs/images/banner.png)\n\nAn unofficial, fully typed python interface for building [.d2](https://github.com/terrastruct/d2) diagram files in python.\n\n## Installation\n\n```bash\npip install py-d2\n```\n\n## Usage\n\n```python\nfrom py_d2 import D2Diagram, D2Shape, D2Connection, D2Style\n\nshapes = [\n    D2Shape(name="shape_name1", style=D2Style(fill="red")),\n    D2Shape(name="shape_name2", style=D2Style(fill="blue"))]\nconnections = [\n    D2Connection(shape_1="shape_name1", shape_2="shape_name2")\n]\n\ndiagram = D2Diagram(shapes=shapes, connections=connections)\n\nwith open("graph.d2", "w", encoding="utf-8") as f:\n    f.write(str(diagram))\n\n```\n\nproduces the following graph.d2 file:\n\n```d2\n\nshape_name1: {\n  style: {\n    fill: red\n  }\n}\nshape_name2: {\n  style: {\n    fill: blue\n  }\n}\nshape_name1 -> shape_name2\n\n```\n\nThis can be rendered using `d2 graph.d2 graph.svg && open graph.svg` or [https://play.d2lang.com/](https://play.d2lang.com/) to produce\n\n![example graph](/docs/images/d2.svg)\n\nSee the [tests](/tests/test_py_d2) for more detailed usage examples.\n\n\n## Supported Features\n\n- [x] Shapes (nodes)\n- [x] Connections (links)\n- [x] Styles\n- [x] Containers (nodes/links in nodes)\n- [x] Shapes in shapes\n- [x] Arrow directions\n- [x] Markdown / block strings / code in shapes\n- [ ] Icons in shapes\n- [ ] SQL table shapes\n- [ ] Class shapes\n- [ ] Comments\n\n\n## Development\n### Prerequisite\n\n- [Python 3.7+](https://www.python.org/)\n- [Poetry 1.3](https://python-poetry.org/)\n- [pre-commit](https://pre-commit.com/)\n\n### Installation\n\nfollowing the steps below to setup the project:\n\n```bash\n\n```bash\n# Clone the repository\ngit clone git@github.com:MrBlenny/py-d2.git && cd py-d2\n\n# Install all dependencies\npoetry install --sync --all-extras --with dev,test,coverage\n\n# install git hook scripts for development\npre-commit install\n\n# Install dependencies with group \'dev\'、\'test\' for development\npoetry install --with dev,test\n# Only install required dependencies for production\npoetry install\n```\n\n### Usage\n\nThere are some useful commands for development:\n\n```bash\n# Run the example\npoetry run example\n\n# Debug with ipdb3\npoetry run ipdb3 ./src/py_d2/main.py\n\n# Code test\npoetry run pytest -s\n\n# Run default coverage test\npoetry run tox\n\n# Run example project coverage test at python 3.9 and 3.10\npoetry run tox -e py{39,310}-py-d2\n\n# Lint with black\npoetry run black ./src --check\n\n# Format code with black\npoetry run black ./src\n\n# Check with mypy\npoetry run mypy ./src\n\n# Check import order with isort\npoetry run isort ./src --check\n\n# Lint with flake8\npoetry run flake8 ./src\n```\n',
     'author': 'David Revay',
     'author_email': 'daverevay@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://mrblenny.github.io/py-d2/',
```

### Comparing `py_d2-1.0.0/PKG-INFO` & `py_d2-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-d2
-Version: 1.0.0
+Version: 1.0.1
 Summary: An unofficial, fully typed python interface for building .d2 graph files in python.
 Home-page: https://mrblenny.github.io/py-d2/
 License: MIT
 Keywords: py-d2,d2-lang,d2-python,diagram-language,terrastruct
 Author: David Revay
 Author-email: daverevay@gmail.com
 Requires-Python: >=3.7,<4.0
```


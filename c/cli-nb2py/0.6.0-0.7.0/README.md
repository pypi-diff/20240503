# Comparing `tmp/cli-nb2py-0.6.0.tar.gz` & `tmp/cli-nb2py-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli-nb2py-0.6.0.tar", last modified: Thu Feb 15 22:38:36 2024, max compression
+gzip compressed data, was "cli-nb2py-0.7.0.tar", last modified: Fri May  3 14:16:09 2024, max compression
```

## Comparing `cli-nb2py-0.6.0.tar` & `cli-nb2py-0.7.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-02-15 22:38:36.223336 cli-nb2py-0.6.0/
--rw-rw-rw-   0        0        0     1093 2024-02-14 23:13:45.000000 cli-nb2py-0.6.0/LICENSE
--rw-rw-rw-   0        0        0     3276 2024-02-15 22:38:36.221321 cli-nb2py-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     2795 2024-02-15 20:39:47.000000 cli-nb2py-0.6.0/README.md
-drwxrwxrwx   0        0        0        0 2024-02-15 22:38:36.201374 cli-nb2py-0.6.0/cli_nb2py/
--rw-rw-rw-   0        0        0        0 2024-02-14 23:02:34.000000 cli-nb2py-0.6.0/cli_nb2py/__init__.py
--rw-rw-rw-   0        0        0     3629 2024-02-15 22:26:10.000000 cli-nb2py-0.6.0/cli_nb2py/main.py
-drwxrwxrwx   0        0        0        0 2024-02-15 22:38:36.220402 cli-nb2py-0.6.0/cli_nb2py.egg-info/
--rw-rw-rw-   0        0        0     3276 2024-02-15 22:38:36.000000 cli-nb2py-0.6.0/cli_nb2py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2024-02-15 22:38:36.000000 cli-nb2py-0.6.0/cli_nb2py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-15 22:38:36.000000 cli-nb2py-0.6.0/cli_nb2py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-02-15 22:38:36.000000 cli-nb2py-0.6.0/cli_nb2py.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2024-02-15 22:38:36.000000 cli-nb2py-0.6.0/cli_nb2py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-02-15 22:38:36.000000 cli-nb2py-0.6.0/cli_nb2py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-15 22:38:36.223336 cli-nb2py-0.6.0/setup.cfg
--rw-rw-rw-   0        0        0      863 2024-02-15 22:26:47.000000 cli-nb2py-0.6.0/setup.py
+drwxr-xr-x   0 bardiakhosravi   (501) staff       (20)        0 2024-05-03 14:16:09.630922 cli-nb2py-0.7.0/
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)     1072 2024-05-03 14:09:37.000000 cli-nb2py-0.7.0/LICENSE
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)     3358 2024-05-03 14:16:09.630731 cli-nb2py-0.7.0/PKG-INFO
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)     2892 2024-05-03 14:12:12.000000 cli-nb2py-0.7.0/README.md
+drwxr-xr-x   0 bardiakhosravi   (501) staff       (20)        0 2024-05-03 14:16:09.629746 cli-nb2py-0.7.0/cli_nb2py/
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)        0 2024-05-03 14:09:37.000000 cli-nb2py-0.7.0/cli_nb2py/__init__.py
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)     4560 2024-05-03 14:10:01.000000 cli-nb2py-0.7.0/cli_nb2py/main.py
+drwxr-xr-x   0 bardiakhosravi   (501) staff       (20)        0 2024-05-03 14:16:09.630490 cli-nb2py-0.7.0/cli_nb2py.egg-info/
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)     3358 2024-05-03 14:16:09.000000 cli-nb2py-0.7.0/cli_nb2py.egg-info/PKG-INFO
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)      266 2024-05-03 14:16:09.000000 cli-nb2py-0.7.0/cli_nb2py.egg-info/SOURCES.txt
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)        1 2024-05-03 14:16:09.000000 cli-nb2py-0.7.0/cli_nb2py.egg-info/dependency_links.txt
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)       46 2024-05-03 14:16:09.000000 cli-nb2py-0.7.0/cli_nb2py.egg-info/entry_points.txt
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)        9 2024-05-03 14:16:09.000000 cli-nb2py-0.7.0/cli_nb2py.egg-info/requires.txt
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)       10 2024-05-03 14:16:09.000000 cli-nb2py-0.7.0/cli_nb2py.egg-info/top_level.txt
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)       38 2024-05-03 14:16:09.630957 cli-nb2py-0.7.0/setup.cfg
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)      834 2024-05-03 14:10:13.000000 cli-nb2py-0.7.0/setup.py
```

### Comparing `cli-nb2py-0.6.0/PKG-INFO` & `cli-nb2py-0.7.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,77 +1,63 @@
-Metadata-Version: 2.1
-Name: cli-nb2py
-Version: 0.6.0
-Summary: Reliable Notebook to Python converter
-Home-page: https://github.com/BardiaKh/nb2py
-Author: Bardia Khosravi
-Author-email: bardiakhosravi95@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: argparse
-
-# nb2py
-
-`nb2py` is a comprehensive tool designed to convert Jupyter Notebooks (.ipynb files) into Python scripts (.py files). This tool simplifies the process of transforming interactive notebook cells into a structured Python script, automatically separating import statements and wrapping executable code within an `if __name__ == '__main__':` guard to maintain the script's portability and usability.
-
-This tool has two versions, a **command-line** version based on python and a **vscode extension**.
-
-## Features
-
-- **VSCode Extension**: A one-click solution for converting notebooks to python files.
-- **Command-Line Simplicity**: Offers a straightforward command-line interface for easy conversion of notebooks to Python scripts.
-- **Import Optimization**: Automatically moves all import statements to the top of the generated Python script.
-- **Executable Wrap**: Wraps all executable code within an `if __name__ == '__main__':` block, ensuring that the script can be imported without unintended execution.
-- **Markdown Conversion**: Converts markdown cells into Python comments, preserving the notebook's documentation in the script.
-
-## VSCode Extension 
-
-### Installation
-
-You can install the `nb2py` extension directly from the Visual Studio Code Marketplace:
-
-1. Open VS Code.
-2. Navigate to the Extensions view by clicking on the Extensions icon in the Activity Bar on the side of the window.
-3. Search for `nb2py`. [if not found here is the [link](https://marketplace.visualstudio.com/items?itemName=BardiaKhosravi.nb2py)]
-4. Click on the Install button.
-
-## Usage
-
-After installation, open the Jupyter Notebook you wish to convert. You'll see a new icon in the editor title bar that looks like a Python logo. Click this icon to convert the currently open notebook.
-
-The converted Python script will be saved in the same directory as the notebook with the extension of `.py`.
-
-![Convert Notebook to Python Script Button](vscode_nb2py/assets/screenshot.png)
-
-## CLI Tool 
-
-### Installation
-
-To install `nb2py`, run the following setup script. Ensure you have Python 3.6 or later installed on your system.
-
-```bash
-pip install cli-nb2py
-```
-
-### Usage
-
-To convert a Jupyter Notebook to a Python script, use the following command:
-
-```bash
-nb2py input_notebook.ipynb output_script.py
-```
-
-If the output file name is not provided, `nb2py` will generate a Python script with the same name as the input notebook (replacing the `.ipynb` extension with `.py`).
-
-## License
-
-`nb2py` is released under the MIT License. See the [LICENSE](LICENSE) file for more details.
-
-## Contact
-
-- Developer: Bardia Khosravi
-- Email: bardiakhosravi95@gmail.com
-- GitHub: [https://github.com/BardiaKh/nb2py](https://github.com/BardiaKh/nb2py)
+# nb2py
+
+`nb2py` is a comprehensive tool designed to convert Jupyter Notebooks (.ipynb files) into Python scripts (.py files). This tool simplifies the process of transforming interactive notebook cells into a structured Python script, automatically separating import statements and wrapping executable code within an `if __name__ == '__main__':` guard to maintain the script's portability and usability.
+
+This tool has two versions, a **command-line** version based on python and a **vscode extension**.
+
+## Features
+
+- **VSCode Extension**: A one-click solution for converting notebooks to python files.
+- **Command-Line Simplicity**: Offers a straightforward command-line interface for easy conversion of notebooks to Python scripts.
+- **Import Optimization**: Automatically moves all import statements to the top of the generated Python script.
+- **Executable Wrap**: Wraps all executable code within an `if __name__ == '__main__':` block, ensuring that the script can be imported without unintended execution.
+- **Markdown Conversion**: Converts markdown cells into Python comments, preserving the notebook's documentation in the script.
+- **Handling Multiline Strings**: Converts `""" """` to multiple `" "\` so there is no spacing issues. Especially useful for prompting LLMs. (added in v0.7.0)
+
+## VSCode Extension 
+
+### Installation
+
+You can install the `nb2py` extension directly from the Visual Studio Code Marketplace:
+
+1. Open VS Code.
+2. Navigate to the Extensions view by clicking on the Extensions icon in the Activity Bar on the side of the window.
+3. Search for `nb2py`. [if not found here is the [link](https://marketplace.visualstudio.com/items?itemName=BardiaKhosravi.nb2py)]
+4. Click on the Install button.
+
+## Usage
+
+After installation, open the Jupyter Notebook you wish to convert. You'll see a new icon in the editor title bar that looks like a Python logo. Click this icon to convert the currently open notebook.
+
+The converted Python script will be saved in the same directory as the notebook with the extension of `.py`.
+
+![Convert Notebook to Python Script Button](vscode_nb2py/assets/screenshot.png)
+
+## CLI Tool 
+
+### Installation
+
+To install `nb2py`, run the following setup script. Ensure you have Python 3.6 or later installed on your system.
+
+```bash
+pip install cli-nb2py
+```
+
+### Usage
+
+To convert a Jupyter Notebook to a Python script, use the following command:
+
+```bash
+nb2py input_notebook.ipynb output_script.py
+```
+
+If the output file name is not provided, `nb2py` will generate a Python script with the same name as the input notebook (replacing the `.ipynb` extension with `.py`).
+
+## License
+
+`nb2py` is released under the MIT License. See the [LICENSE](LICENSE) file for more details.
+
+## Contact
+
+- Developer: Bardia Khosravi
+- Email: bardiakhosravi95@gmail.com
+- GitHub: [https://github.com/BardiaKh/nb2py](https://github.com/BardiaKh/nb2py)
```

### Comparing `cli-nb2py-0.6.0/cli_nb2py.egg-info/PKG-INFO` & `cli-nb2py-0.7.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,77 +1,78 @@
-Metadata-Version: 2.1
-Name: cli-nb2py
-Version: 0.6.0
-Summary: Reliable Notebook to Python converter
-Home-page: https://github.com/BardiaKh/nb2py
-Author: Bardia Khosravi
-Author-email: bardiakhosravi95@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: argparse
-
-# nb2py
-
-`nb2py` is a comprehensive tool designed to convert Jupyter Notebooks (.ipynb files) into Python scripts (.py files). This tool simplifies the process of transforming interactive notebook cells into a structured Python script, automatically separating import statements and wrapping executable code within an `if __name__ == '__main__':` guard to maintain the script's portability and usability.
-
-This tool has two versions, a **command-line** version based on python and a **vscode extension**.
-
-## Features
-
-- **VSCode Extension**: A one-click solution for converting notebooks to python files.
-- **Command-Line Simplicity**: Offers a straightforward command-line interface for easy conversion of notebooks to Python scripts.
-- **Import Optimization**: Automatically moves all import statements to the top of the generated Python script.
-- **Executable Wrap**: Wraps all executable code within an `if __name__ == '__main__':` block, ensuring that the script can be imported without unintended execution.
-- **Markdown Conversion**: Converts markdown cells into Python comments, preserving the notebook's documentation in the script.
-
-## VSCode Extension 
-
-### Installation
-
-You can install the `nb2py` extension directly from the Visual Studio Code Marketplace:
-
-1. Open VS Code.
-2. Navigate to the Extensions view by clicking on the Extensions icon in the Activity Bar on the side of the window.
-3. Search for `nb2py`. [if not found here is the [link](https://marketplace.visualstudio.com/items?itemName=BardiaKhosravi.nb2py)]
-4. Click on the Install button.
-
-## Usage
-
-After installation, open the Jupyter Notebook you wish to convert. You'll see a new icon in the editor title bar that looks like a Python logo. Click this icon to convert the currently open notebook.
-
-The converted Python script will be saved in the same directory as the notebook with the extension of `.py`.
-
-![Convert Notebook to Python Script Button](vscode_nb2py/assets/screenshot.png)
-
-## CLI Tool 
-
-### Installation
-
-To install `nb2py`, run the following setup script. Ensure you have Python 3.6 or later installed on your system.
-
-```bash
-pip install cli-nb2py
-```
-
-### Usage
-
-To convert a Jupyter Notebook to a Python script, use the following command:
-
-```bash
-nb2py input_notebook.ipynb output_script.py
-```
-
-If the output file name is not provided, `nb2py` will generate a Python script with the same name as the input notebook (replacing the `.ipynb` extension with `.py`).
-
-## License
-
-`nb2py` is released under the MIT License. See the [LICENSE](LICENSE) file for more details.
-
-## Contact
-
-- Developer: Bardia Khosravi
-- Email: bardiakhosravi95@gmail.com
-- GitHub: [https://github.com/BardiaKh/nb2py](https://github.com/BardiaKh/nb2py)
+Metadata-Version: 2.1
+Name: cli-nb2py
+Version: 0.7.0
+Summary: Reliable Notebook to Python converter
+Home-page: https://github.com/BardiaKh/nb2py
+Author: Bardia Khosravi
+Author-email: bardiakhosravi95@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: argparse
+
+# nb2py
+
+`nb2py` is a comprehensive tool designed to convert Jupyter Notebooks (.ipynb files) into Python scripts (.py files). This tool simplifies the process of transforming interactive notebook cells into a structured Python script, automatically separating import statements and wrapping executable code within an `if __name__ == '__main__':` guard to maintain the script's portability and usability.
+
+This tool has two versions, a **command-line** version based on python and a **vscode extension**.
+
+## Features
+
+- **VSCode Extension**: A one-click solution for converting notebooks to python files.
+- **Command-Line Simplicity**: Offers a straightforward command-line interface for easy conversion of notebooks to Python scripts.
+- **Import Optimization**: Automatically moves all import statements to the top of the generated Python script.
+- **Executable Wrap**: Wraps all executable code within an `if __name__ == '__main__':` block, ensuring that the script can be imported without unintended execution.
+- **Markdown Conversion**: Converts markdown cells into Python comments, preserving the notebook's documentation in the script.
+- **Handling Multiline Strings**: Converts `""" """` to multiple `" "\` so there is no spacing issues. Especially useful for prompting LLMs. (added in v0.7.0)
+
+## VSCode Extension 
+
+### Installation
+
+You can install the `nb2py` extension directly from the Visual Studio Code Marketplace:
+
+1. Open VS Code.
+2. Navigate to the Extensions view by clicking on the Extensions icon in the Activity Bar on the side of the window.
+3. Search for `nb2py`. [if not found here is the [link](https://marketplace.visualstudio.com/items?itemName=BardiaKhosravi.nb2py)]
+4. Click on the Install button.
+
+## Usage
+
+After installation, open the Jupyter Notebook you wish to convert. You'll see a new icon in the editor title bar that looks like a Python logo. Click this icon to convert the currently open notebook.
+
+The converted Python script will be saved in the same directory as the notebook with the extension of `.py`.
+
+![Convert Notebook to Python Script Button](vscode_nb2py/assets/screenshot.png)
+
+## CLI Tool 
+
+### Installation
+
+To install `nb2py`, run the following setup script. Ensure you have Python 3.6 or later installed on your system.
+
+```bash
+pip install cli-nb2py
+```
+
+### Usage
+
+To convert a Jupyter Notebook to a Python script, use the following command:
+
+```bash
+nb2py input_notebook.ipynb output_script.py
+```
+
+If the output file name is not provided, `nb2py` will generate a Python script with the same name as the input notebook (replacing the `.ipynb` extension with `.py`).
+
+## License
+
+`nb2py` is released under the MIT License. See the [LICENSE](LICENSE) file for more details.
+
+## Contact
+
+- Developer: Bardia Khosravi
+- Email: bardiakhosravi95@gmail.com
+- GitHub: [https://github.com/BardiaKh/nb2py](https://github.com/BardiaKh/nb2py)
```

### Comparing `cli-nb2py-0.6.0/setup.py` & `cli-nb2py-0.7.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-import setuptools
-
-with open("README.md", "r", encoding="utf-8") as fh:
-    long_description = fh.read()
-
-setuptools.setup(
-    name="cli-nb2py",
-    version="0.6.0",
-    author="Bardia Khosravi",
-    author_email="bardiakhosravi95@gmail.com",
-    description="Reliable Notebook to Python converter",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/BardiaKh/nb2py",
-    packages = setuptools.find_packages(),
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-    install_requires=[
-        "argparse",
-    ],
-    entry_points={
-        'console_scripts': [
-            'nb2py=cli_nb2py.main:main',
-        ],
-    },
-    python_requires='>=3.6',
+import setuptools
+
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+
+setuptools.setup(
+    name="cli-nb2py",
+    version="0.7.0",
+    author="Bardia Khosravi",
+    author_email="bardiakhosravi95@gmail.com",
+    description="Reliable Notebook to Python converter",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/BardiaKh/nb2py",
+    packages = setuptools.find_packages(),
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+    install_requires=[
+        "argparse",
+    ],
+    entry_points={
+        'console_scripts': [
+            'nb2py=cli_nb2py.main:main',
+        ],
+    },
+    python_requires='>=3.6',
 )
```


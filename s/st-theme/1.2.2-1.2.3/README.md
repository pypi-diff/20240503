# Comparing `tmp/st-theme-1.2.2.tar.gz` & `tmp/st-theme-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st-theme-1.2.2.tar", last modified: Fri Mar 15 15:06:15 2024, max compression
+gzip compressed data, was "st-theme-1.2.3.tar", last modified: Fri May  3 19:25:07 2024, max compression
```

## Comparing `st-theme-1.2.2.tar` & `st-theme-1.2.3.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-03-15 15:06:15.186346 st-theme-1.2.2/
--rw-r--r--   0 gabrieltempass   (501) staff       (20)     1073 2024-03-06 21:18:39.000000 st-theme-1.2.2/LICENSE
--rw-r--r--   0 gabrieltempass   (501) staff       (20)       50 2024-03-08 19:56:12.000000 st-theme-1.2.2/MANIFEST.in
--rw-r--r--   0 gabrieltempass   (501) staff       (20)     7006 2024-03-15 15:06:15.186212 st-theme-1.2.2/PKG-INFO
--rw-r--r--   0 gabrieltempass   (501) staff       (20)     5250 2024-03-14 21:36:10.000000 st-theme-1.2.2/README.md
--rw-r--r--   0 gabrieltempass   (501) staff       (20)       38 2024-03-15 15:06:15.186397 st-theme-1.2.2/setup.cfg
--rw-r--r--   0 gabrieltempass   (501) staff       (20)      793 2024-03-15 15:00:33.000000 st-theme-1.2.2/setup.py
-drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-03-15 15:06:15.182279 st-theme-1.2.2/st_theme.egg-info/
--rw-r--r--   0 gabrieltempass   (501) staff       (20)     7006 2024-03-15 15:06:15.000000 st-theme-1.2.2/st_theme.egg-info/PKG-INFO
--rw-r--r--   0 gabrieltempass   (501) staff       (20)      404 2024-03-15 15:06:15.000000 st-theme-1.2.2/st_theme.egg-info/SOURCES.txt
--rw-r--r--   0 gabrieltempass   (501) staff       (20)        1 2024-03-15 15:06:15.000000 st-theme-1.2.2/st_theme.egg-info/dependency_links.txt
--rw-r--r--   0 gabrieltempass   (501) staff       (20)       16 2024-03-15 15:06:15.000000 st-theme-1.2.2/st_theme.egg-info/requires.txt
--rw-r--r--   0 gabrieltempass   (501) staff       (20)       16 2024-03-15 15:06:15.000000 st-theme-1.2.2/st_theme.egg-info/top_level.txt
-drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-03-15 15:06:15.182524 st-theme-1.2.2/streamlit_theme/
--rw-r--r--   0 gabrieltempass   (501) staff       (20)     6060 2024-03-15 15:06:04.000000 st-theme-1.2.2/streamlit_theme/__init__.py
--rw-r--r--   0 gabrieltempass   (501) staff       (20)      429 2024-03-14 21:29:50.000000 st-theme-1.2.2/streamlit_theme/example.py
-drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-03-15 15:06:15.181059 st-theme-1.2.2/streamlit_theme/frontend/
-drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-03-15 15:06:15.182818 st-theme-1.2.2/streamlit_theme/frontend/dist/
-drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-03-15 15:06:15.185817 st-theme-1.2.2/streamlit_theme/frontend/dist/assets/
--rw-r--r--   0 gabrieltempass   (501) staff       (20)   238048 2024-03-14 20:30:32.000000 st-theme-1.2.2/streamlit_theme/frontend/dist/assets/index--ZWO88yE.js
--rw-r--r--   0 gabrieltempass   (501) staff       (20)       71 2024-03-14 20:30:32.000000 st-theme-1.2.2/streamlit_theme/frontend/dist/assets/index-3Jrapfwd.css
--rw-r--r--   0 gabrieltempass   (501) staff       (20)      682 2024-03-14 20:30:32.000000 st-theme-1.2.2/streamlit_theme/frontend/dist/index.html
+drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-05-03 19:25:07.239322 st-theme-1.2.3/
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)     1073 2024-03-06 21:18:39.000000 st-theme-1.2.3/LICENSE
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)       50 2024-03-08 19:56:12.000000 st-theme-1.2.3/MANIFEST.in
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)     6894 2024-05-03 19:25:07.239204 st-theme-1.2.3/PKG-INFO
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)     5153 2024-05-03 14:02:43.000000 st-theme-1.2.3/README.md
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)       38 2024-05-03 19:25:07.239368 st-theme-1.2.3/setup.cfg
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)     2235 2024-05-03 19:20:27.000000 st-theme-1.2.3/setup.py
+drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-05-03 19:25:07.236915 st-theme-1.2.3/st_theme.egg-info/
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)     6894 2024-05-03 19:25:07.000000 st-theme-1.2.3/st_theme.egg-info/PKG-INFO
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)      467 2024-05-03 19:25:07.000000 st-theme-1.2.3/st_theme.egg-info/SOURCES.txt
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)        1 2024-05-03 19:25:07.000000 st-theme-1.2.3/st_theme.egg-info/dependency_links.txt
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)       60 2024-05-03 19:25:07.000000 st-theme-1.2.3/st_theme.egg-info/entry_points.txt
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)       16 2024-05-03 19:25:07.000000 st-theme-1.2.3/st_theme.egg-info/requires.txt
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)       16 2024-05-03 19:25:07.000000 st-theme-1.2.3/st_theme.egg-info/top_level.txt
+drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-05-03 19:25:07.237563 st-theme-1.2.3/streamlit_theme/
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)     5608 2024-05-03 19:23:23.000000 st-theme-1.2.3/streamlit_theme/__init__.py
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)       77 2024-05-03 16:40:58.000000 st-theme-1.2.3/streamlit_theme/__main__.py
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)      429 2024-03-14 21:29:50.000000 st-theme-1.2.3/streamlit_theme/example.py
+drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-05-03 19:25:07.235602 st-theme-1.2.3/streamlit_theme/frontend/
+drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-05-03 19:25:07.237792 st-theme-1.2.3/streamlit_theme/frontend/dist/
+drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-05-03 19:25:07.238932 st-theme-1.2.3/streamlit_theme/frontend/dist/assets/
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)   238048 2024-03-14 20:30:32.000000 st-theme-1.2.3/streamlit_theme/frontend/dist/assets/index--ZWO88yE.js
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)       71 2024-03-14 20:30:32.000000 st-theme-1.2.3/streamlit_theme/frontend/dist/assets/index-3Jrapfwd.css
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)      682 2024-03-14 20:30:32.000000 st-theme-1.2.3/streamlit_theme/frontend/dist/index.html
```

### Comparing `st-theme-1.2.2/LICENSE` & `st-theme-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `st-theme-1.2.2/PKG-INFO` & `st-theme-1.2.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,175 +1,197 @@
 Metadata-Version: 2.1
 Name: st-theme
-Version: 1.2.2
+Version: 1.2.3
 Summary: A component that returns the active theme of the Streamlit app.
 Home-page: https://github.com/gabrieltempass/streamlit-theme
 Author: Gabriel Tem Pass
 Author-email: redo_hint_0x@icloud.com
-License: UNKNOWN
-Description: # Streamlit Theme
-        
-        A component that returns the active theme of the Streamlit app.
-        
-        [![Overview](https://github.com/gabrieltempass/streamlit-theme/raw/main/images/st_theme_1.gif)](https://st-theme-1.streamlit.app/)
-        
-        ## Installation
-        
-        ``` bash
-        pip install st-theme
-        ```
-        
-        ## Usage
-        
-        The function immediately returns the active theme, when it is called. If the
-        user manually changes the theme, after the web app is already running, it
-        updates the returned value.
-        
-        ## Parameters
-        
-        **adjust** : `bool`, `default=True`</br>
-        If set to ``True``, which is the default, it makes a CSS adjustment and removes
-        a space that would otherwise be added to the page by calling the ``st_theme``
-        function.
-        
-        Streamlit components are meant to render something in the web app, and
-        Streamlit adds a space for them even when there is nothing to render. Since
-        ``st_theme`` does not render anything, and only communicates with the frontend
-        to fetch the active theme, it makes a CSS adjustment to remove this space.
-        
-        In most cases, the CSS adjustment does not interfere with the rest of the web
-        app, however there could be some situations where this occurs. If this happens,
-        or it is desired to disable it, pass ``False`` to `adjust` and, when necessary,
-        make your own CSS adjustment with ``st.markdown``.
-        
-        **key** : `str` or `int`, optional</br>
-        A string or integer to use as a unique key for the component. Multiple
-        ``st_themes`` may not share the same key. Defaults to ``None``.
-        
-        ## Returns
-        
-        **theme** : `dict of str: str` or `None`</br>
-        A dictionary with the style settings being used by the active theme of the
-        Streamlit app, or ``None``, if for some reason it could not be fetched.
-        
-        ## Notes
-        
-        There is a known bug, that depends on the browser, where the theme is not
-        returned immediately when the function is called. But it is returned normally
-        when the user changes it.
-        
-        This can be a problem in determining the initial theme of the web app. Because,
-        by default, Streamlit uses the user's operating system setting (which might be
-        unknown) to automatically apply the light or dark mode to the app, when it is
-        first rendered.
-        
-        To solve the issue, it is recommended to set a
-        [default theme configuration](https://docs.streamlit.io/library/advanced-features/theming)
-        for the app, and use its value in case of ``st_theme`` returning ``None``.
-        
-        ## Examples
-        
-        A basic example:
-        
-        ``` python
-        import streamlit as st
-        from streamlit_theme import st_theme
-        theme = st_theme()
-        st.write(theme)
-        ```
-        [![Example 1](https://github.com/gabrieltempass/streamlit-theme/raw/main/images/st_theme_1.gif)](https://st-theme-1.streamlit.app/)
-        [**[App]**](https://st-theme-1.streamlit.app/) 
-        [**[Source]**](https://github.com/gabrieltempass/streamlit-theme/blob/main/examples/st_theme_1.py)
-        
-        An example showing the CSS adjustment made, when set to ``True``:
-        
-        ``` python
-        import streamlit as st
-        from streamlit_theme import st_theme
-        
-        adjust = st.toggle("Make the CSS adjustment")
-        
-        st.write("Input:")
-        st.code(
-            f"""
-            st.write("Lorem ipsum")
-            st_theme(adjust={adjust})
-            st.write("Lorem ipsum")
-            """
-        )
-        
-        st.write("Output:")
-        st.write("Lorem ipsum")
-        st_theme(adjust=adjust)
-        st.write("Lorem ipsum")
-        ```
-        [![Example 2](https://github.com/gabrieltempass/streamlit-theme/raw/main/images/st_theme_2.gif)](https://st-theme-2.streamlit.app/)
-        [**[App]**](https://st-theme-2.streamlit.app/) 
-        [**[Source]**](https://github.com/gabrieltempass/streamlit-theme/blob/main/examples/st_theme_2.py)
-        
-        ## Requirements
-        
-        To use this Streamlit component in your app, you will need:
-        * **Python 3.8+**
-        * **Streamlit 1.20+**
-        * The CSS adjustment depends on the
-          [browser compatibility for the :has pseudo-class](https://developer.mozilla.org/en-US/docs/Web/CSS/:has#browser_compatibility).
-        
-        ## Development
-        
-        Ensure you have [Python 3.8+](https://www.python.org/downloads/),
-        [Node.js](https://nodejs.org) and
-        [npm](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)
-        installed.
-        
-        1. Clone this repository:
-        ``` bash
-        git clone git@github.com:gabrieltempass/streamlit-theme.git
-        ```
-        
-        2. Go to the `frontend` directory and initialize and run the component template
-        frontend:
-        ``` bash
-        cd streamlit-theme/streamlit_theme/frontend
-        ```
-        ``` bash
-        npm install
-        npm run dev
-        ```
-        
-        3. From a separate terminal, go to the repository root directory, create a new
-        Python virtual environment, activate it and install Streamlit and the template
-        as an editable package:
-        ``` bash
-        cd streamlit-theme
-        ```
-        ``` bash
-        python3 -m venv venv
-        . venv/bin/activate
-        pip install streamlit
-        pip install -e .
-        ```
-        
-        Still from the same separate terminal, run the example Streamlit app:
-        ``` bash
-        streamlit run streamlit_theme/example.py
-        ```
-        
-        If all goes well, you should see something like this:
-        
-        ![Quickstart success](https://github.com/gabrieltempass/streamlit-theme/raw/main/images/development.png)
-        
-        Modify the frontend code at
-        `streamlit_theme/frontend/src/StTheme.vue`.
-        Modify the Python code at `streamlit_theme/__init__.py`.
-        
-        ## References
-        
-        This Streamlit component is based on the [streamlit-component-vue-vite-template](https://github.com/gabrieltempass/streamlit-component-vue-vite-template)
-        repository, that uses Vue 3 to code the frontend and Vite to serve the files
-        locally during development, as well as bundle and compile them for production.
-        
+License: MIT License
+Project-URL: Source Code, https://github.com/gabrieltempass/streamlit-theme
+Project-URL: Bug Tracker, https://github.com/gabrieltempass/streamlit-theme/issues
+Project-URL: Release notes, https://github.com/gabrieltempass/streamlit-theme/releases
+Project-URL: Documentation, https://github.com/gabrieltempass/streamlit-theme
+Project-URL: Community, https://discuss.streamlit.io/t/new-component-st-theme-it-returns-the-active-theme-of-the-streamlit-app/64424
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Database :: Front-Ends
+Classifier: Topic :: Office/Business :: Financial :: Spreadsheet
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Scientific/Engineering :: Visualization
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Topic :: Software Development :: Widget Sets
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Streamlit Theme
+
+A component that returns the active theme of the Streamlit app.
+
+[![Overview](https://github.com/gabrieltempass/streamlit-theme/raw/main/images/st_theme_1.gif)](https://st-theme-1.streamlit.app/)
+
+## Installation
+
+``` bash
+pip install st-theme
+```
+
+## Usage
+
+The function immediately returns the active theme, when it is called. If the
+user manually changes the theme, after the web app is already running, it
+updates the returned value.
+
+## Parameters
+
+**adjust** : `bool`, `default=True`</br>
+If set to ``True``, which is the default, it makes a CSS adjustment and removes
+a space that would otherwise be added to the page by calling the ``st_theme``
+function.
+
+Streamlit components are meant to render something in the web app, and
+Streamlit adds a space for them even when there is nothing to render. Since
+``st_theme`` does not render anything, and only communicates with the frontend
+to fetch the active theme, it makes a CSS adjustment to remove this space.
+
+In most cases, the CSS adjustment does not interfere with the rest of the web
+app, however there could be some situations where this occurs. If this happens,
+or it is desired to disable it, pass ``False`` to `adjust` and, when necessary,
+make your own CSS adjustment with ``st.html``.
+
+**key** : `str` or `int`, optional</br>
+A string or integer to use as a unique key for the component. Multiple
+``st_themes`` may not share the same key. Defaults to ``None``.
+
+## Returns
+
+**theme** : `dict of {str : str}` or `None`</br>
+A dictionary with the style settings being used by the active theme of the
+Streamlit app, or ``None``, if for some reason it could not be fetched.
+
+## Notes
+
+There is a known bug, that depends on the browser, where the theme is not
+returned immediately when the function is called. But it is returned normally
+when the user changes it.
+
+This can be a problem in determining the initial theme of the web app. Because,
+by default, Streamlit uses the user's operating system setting (which might be
+unknown) to automatically apply the light or dark mode to the app, when it is
+first rendered.
+
+To solve the issue, it is recommended to set a
+[default theme configuration](https://docs.streamlit.io/library/advanced-features/theming)
+for the app, and use its value in case of ``st_theme`` returning ``None``.
+
+## Examples
+
+A basic example:
+
+``` python
+import streamlit as st
+from streamlit_theme import st_theme
+theme = st_theme()
+st.write(theme)
+```
+[![Example 1](https://github.com/gabrieltempass/streamlit-theme/raw/main/images/st_theme_1.gif)](https://st-theme-1.streamlit.app/)
+[**[App]**](https://st-theme-1.streamlit.app/) 
+[**[Source]**](https://github.com/gabrieltempass/streamlit-theme/blob/main/examples/st_theme_1.py)
+
+An example showing the CSS adjustment made, when set to ``True``:
+
+``` python
+import streamlit as st
+from streamlit_theme import st_theme
+
+adjust = st.toggle("Make the CSS adjustment")
+
+st.write("Input:")
+st.code(
+    f"""
+    st.write("Lorem ipsum")
+    st_theme(adjust={adjust})
+    st.write("Lorem ipsum")
+    """
+)
+
+st.write("Output:")
+st.write("Lorem ipsum")
+st_theme(adjust=adjust)
+st.write("Lorem ipsum")
+```
+[![Example 2](https://github.com/gabrieltempass/streamlit-theme/raw/main/images/st_theme_2.gif)](https://st-theme-2.streamlit.app/)
+[**[App]**](https://st-theme-2.streamlit.app/) 
+[**[Source]**](https://github.com/gabrieltempass/streamlit-theme/blob/main/examples/st_theme_2.py)
+
+## Requirements
+
+To use this Streamlit component in your app, you will need:
+* **Python 3.8+**
+* **Streamlit 1.20+**
+* The CSS adjustment depends on the
+  [browser compatibility with the :has pseudo-class](https://developer.mozilla.org/en-US/docs/Web/CSS/:has#browser_compatibility)
+
+## Development
+
+Ensure you have [Python 3.8+](https://www.python.org/downloads/),
+[Node.js](https://nodejs.org) and
+[npm](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)
+installed.
+
+1. Clone this repository:
+``` bash
+git clone git@github.com:gabrieltempass/streamlit-theme.git
+```
+
+2. Go to the `frontend` directory and initialize and run the component template
+frontend:
+``` bash
+cd streamlit-theme/streamlit_theme/frontend
+```
+``` bash
+npm install
+npm run dev
+```
+
+3. From a separate terminal, go to the repository root directory, create a new
+Python virtual environment, activate it and install Streamlit and the template
+as an editable package:
+``` bash
+cd streamlit-theme
+```
+``` bash
+python3 -m venv venv
+. venv/bin/activate
+pip install streamlit
+pip install -e .
+```
+
+Still from the same separate terminal, run the example Streamlit app:
+``` bash
+streamlit run streamlit_theme/example.py
+```
+
+If all goes well, you should see something like this:
+
+![Quickstart success](https://github.com/gabrieltempass/streamlit-theme/raw/main/images/development.png)
+
+Modify the frontend code at
+`streamlit_theme/frontend/src/StTheme.vue`.
+Modify the Python code at `streamlit_theme/__init__.py`.
+
+## References
+
+This Streamlit component was made with the [streamlit-component-vue-vite-template](https://github.com/gabrieltempass/streamlit-component-vue-vite-template), by
+[@gabrieltempass](https://github.com/gabrieltempass).
+
+
```

### Comparing `st-theme-1.2.2/README.md` & `st-theme-1.2.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -27,23 +27,23 @@
 Streamlit adds a space for them even when there is nothing to render. Since
 ``st_theme`` does not render anything, and only communicates with the frontend
 to fetch the active theme, it makes a CSS adjustment to remove this space.
 
 In most cases, the CSS adjustment does not interfere with the rest of the web
 app, however there could be some situations where this occurs. If this happens,
 or it is desired to disable it, pass ``False`` to `adjust` and, when necessary,
-make your own CSS adjustment with ``st.markdown``.
+make your own CSS adjustment with ``st.html``.
 
 **key** : `str` or `int`, optional</br>
 A string or integer to use as a unique key for the component. Multiple
 ``st_themes`` may not share the same key. Defaults to ``None``.
 
 ## Returns
 
-**theme** : `dict of str: str` or `None`</br>
+**theme** : `dict of {str : str}` or `None`</br>
 A dictionary with the style settings being used by the active theme of the
 Streamlit app, or ``None``, if for some reason it could not be fetched.
 
 ## Notes
 
 There is a known bug, that depends on the browser, where the theme is not
 returned immediately when the function is called. But it is returned normally
@@ -100,15 +100,15 @@
 
 ## Requirements
 
 To use this Streamlit component in your app, you will need:
 * **Python 3.8+**
 * **Streamlit 1.20+**
 * The CSS adjustment depends on the
-  [browser compatibility for the :has pseudo-class](https://developer.mozilla.org/en-US/docs/Web/CSS/:has#browser_compatibility).
+  [browser compatibility with the :has pseudo-class](https://developer.mozilla.org/en-US/docs/Web/CSS/:has#browser_compatibility)
 
 ## Development
 
 Ensure you have [Python 3.8+](https://www.python.org/downloads/),
 [Node.js](https://nodejs.org) and
 [npm](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)
 installed.
@@ -152,10 +152,9 @@
 
 Modify the frontend code at
 `streamlit_theme/frontend/src/StTheme.vue`.
 Modify the Python code at `streamlit_theme/__init__.py`.
 
 ## References
 
-This Streamlit component is based on the [streamlit-component-vue-vite-template](https://github.com/gabrieltempass/streamlit-component-vue-vite-template)
-repository, that uses Vue 3 to code the frontend and Vite to serve the files
-locally during development, as well as bundle and compile them for production.
+This Streamlit component was made with the [streamlit-component-vue-vite-template](https://github.com/gabrieltempass/streamlit-component-vue-vite-template), by
+[@gabrieltempass](https://github.com/gabrieltempass).
```

### Comparing `st-theme-1.2.2/st_theme.egg-info/PKG-INFO` & `st-theme-1.2.3/st_theme.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,175 +1,197 @@
 Metadata-Version: 2.1
 Name: st-theme
-Version: 1.2.2
+Version: 1.2.3
 Summary: A component that returns the active theme of the Streamlit app.
 Home-page: https://github.com/gabrieltempass/streamlit-theme
 Author: Gabriel Tem Pass
 Author-email: redo_hint_0x@icloud.com
-License: UNKNOWN
-Description: # Streamlit Theme
-        
-        A component that returns the active theme of the Streamlit app.
-        
-        [![Overview](https://github.com/gabrieltempass/streamlit-theme/raw/main/images/st_theme_1.gif)](https://st-theme-1.streamlit.app/)
-        
-        ## Installation
-        
-        ``` bash
-        pip install st-theme
-        ```
-        
-        ## Usage
-        
-        The function immediately returns the active theme, when it is called. If the
-        user manually changes the theme, after the web app is already running, it
-        updates the returned value.
-        
-        ## Parameters
-        
-        **adjust** : `bool`, `default=True`</br>
-        If set to ``True``, which is the default, it makes a CSS adjustment and removes
-        a space that would otherwise be added to the page by calling the ``st_theme``
-        function.
-        
-        Streamlit components are meant to render something in the web app, and
-        Streamlit adds a space for them even when there is nothing to render. Since
-        ``st_theme`` does not render anything, and only communicates with the frontend
-        to fetch the active theme, it makes a CSS adjustment to remove this space.
-        
-        In most cases, the CSS adjustment does not interfere with the rest of the web
-        app, however there could be some situations where this occurs. If this happens,
-        or it is desired to disable it, pass ``False`` to `adjust` and, when necessary,
-        make your own CSS adjustment with ``st.markdown``.
-        
-        **key** : `str` or `int`, optional</br>
-        A string or integer to use as a unique key for the component. Multiple
-        ``st_themes`` may not share the same key. Defaults to ``None``.
-        
-        ## Returns
-        
-        **theme** : `dict of str: str` or `None`</br>
-        A dictionary with the style settings being used by the active theme of the
-        Streamlit app, or ``None``, if for some reason it could not be fetched.
-        
-        ## Notes
-        
-        There is a known bug, that depends on the browser, where the theme is not
-        returned immediately when the function is called. But it is returned normally
-        when the user changes it.
-        
-        This can be a problem in determining the initial theme of the web app. Because,
-        by default, Streamlit uses the user's operating system setting (which might be
-        unknown) to automatically apply the light or dark mode to the app, when it is
-        first rendered.
-        
-        To solve the issue, it is recommended to set a
-        [default theme configuration](https://docs.streamlit.io/library/advanced-features/theming)
-        for the app, and use its value in case of ``st_theme`` returning ``None``.
-        
-        ## Examples
-        
-        A basic example:
-        
-        ``` python
-        import streamlit as st
-        from streamlit_theme import st_theme
-        theme = st_theme()
-        st.write(theme)
-        ```
-        [![Example 1](https://github.com/gabrieltempass/streamlit-theme/raw/main/images/st_theme_1.gif)](https://st-theme-1.streamlit.app/)
-        [**[App]**](https://st-theme-1.streamlit.app/) 
-        [**[Source]**](https://github.com/gabrieltempass/streamlit-theme/blob/main/examples/st_theme_1.py)
-        
-        An example showing the CSS adjustment made, when set to ``True``:
-        
-        ``` python
-        import streamlit as st
-        from streamlit_theme import st_theme
-        
-        adjust = st.toggle("Make the CSS adjustment")
-        
-        st.write("Input:")
-        st.code(
-            f"""
-            st.write("Lorem ipsum")
-            st_theme(adjust={adjust})
-            st.write("Lorem ipsum")
-            """
-        )
-        
-        st.write("Output:")
-        st.write("Lorem ipsum")
-        st_theme(adjust=adjust)
-        st.write("Lorem ipsum")
-        ```
-        [![Example 2](https://github.com/gabrieltempass/streamlit-theme/raw/main/images/st_theme_2.gif)](https://st-theme-2.streamlit.app/)
-        [**[App]**](https://st-theme-2.streamlit.app/) 
-        [**[Source]**](https://github.com/gabrieltempass/streamlit-theme/blob/main/examples/st_theme_2.py)
-        
-        ## Requirements
-        
-        To use this Streamlit component in your app, you will need:
-        * **Python 3.8+**
-        * **Streamlit 1.20+**
-        * The CSS adjustment depends on the
-          [browser compatibility for the :has pseudo-class](https://developer.mozilla.org/en-US/docs/Web/CSS/:has#browser_compatibility).
-        
-        ## Development
-        
-        Ensure you have [Python 3.8+](https://www.python.org/downloads/),
-        [Node.js](https://nodejs.org) and
-        [npm](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)
-        installed.
-        
-        1. Clone this repository:
-        ``` bash
-        git clone git@github.com:gabrieltempass/streamlit-theme.git
-        ```
-        
-        2. Go to the `frontend` directory and initialize and run the component template
-        frontend:
-        ``` bash
-        cd streamlit-theme/streamlit_theme/frontend
-        ```
-        ``` bash
-        npm install
-        npm run dev
-        ```
-        
-        3. From a separate terminal, go to the repository root directory, create a new
-        Python virtual environment, activate it and install Streamlit and the template
-        as an editable package:
-        ``` bash
-        cd streamlit-theme
-        ```
-        ``` bash
-        python3 -m venv venv
-        . venv/bin/activate
-        pip install streamlit
-        pip install -e .
-        ```
-        
-        Still from the same separate terminal, run the example Streamlit app:
-        ``` bash
-        streamlit run streamlit_theme/example.py
-        ```
-        
-        If all goes well, you should see something like this:
-        
-        ![Quickstart success](https://github.com/gabrieltempass/streamlit-theme/raw/main/images/development.png)
-        
-        Modify the frontend code at
-        `streamlit_theme/frontend/src/StTheme.vue`.
-        Modify the Python code at `streamlit_theme/__init__.py`.
-        
-        ## References
-        
-        This Streamlit component is based on the [streamlit-component-vue-vite-template](https://github.com/gabrieltempass/streamlit-component-vue-vite-template)
-        repository, that uses Vue 3 to code the frontend and Vite to serve the files
-        locally during development, as well as bundle and compile them for production.
-        
+License: MIT License
+Project-URL: Source Code, https://github.com/gabrieltempass/streamlit-theme
+Project-URL: Bug Tracker, https://github.com/gabrieltempass/streamlit-theme/issues
+Project-URL: Release notes, https://github.com/gabrieltempass/streamlit-theme/releases
+Project-URL: Documentation, https://github.com/gabrieltempass/streamlit-theme
+Project-URL: Community, https://discuss.streamlit.io/t/new-component-st-theme-it-returns-the-active-theme-of-the-streamlit-app/64424
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Database :: Front-Ends
+Classifier: Topic :: Office/Business :: Financial :: Spreadsheet
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Scientific/Engineering :: Visualization
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Topic :: Software Development :: Widget Sets
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Streamlit Theme
+
+A component that returns the active theme of the Streamlit app.
+
+[![Overview](https://github.com/gabrieltempass/streamlit-theme/raw/main/images/st_theme_1.gif)](https://st-theme-1.streamlit.app/)
+
+## Installation
+
+``` bash
+pip install st-theme
+```
+
+## Usage
+
+The function immediately returns the active theme, when it is called. If the
+user manually changes the theme, after the web app is already running, it
+updates the returned value.
+
+## Parameters
+
+**adjust** : `bool`, `default=True`</br>
+If set to ``True``, which is the default, it makes a CSS adjustment and removes
+a space that would otherwise be added to the page by calling the ``st_theme``
+function.
+
+Streamlit components are meant to render something in the web app, and
+Streamlit adds a space for them even when there is nothing to render. Since
+``st_theme`` does not render anything, and only communicates with the frontend
+to fetch the active theme, it makes a CSS adjustment to remove this space.
+
+In most cases, the CSS adjustment does not interfere with the rest of the web
+app, however there could be some situations where this occurs. If this happens,
+or it is desired to disable it, pass ``False`` to `adjust` and, when necessary,
+make your own CSS adjustment with ``st.html``.
+
+**key** : `str` or `int`, optional</br>
+A string or integer to use as a unique key for the component. Multiple
+``st_themes`` may not share the same key. Defaults to ``None``.
+
+## Returns
+
+**theme** : `dict of {str : str}` or `None`</br>
+A dictionary with the style settings being used by the active theme of the
+Streamlit app, or ``None``, if for some reason it could not be fetched.
+
+## Notes
+
+There is a known bug, that depends on the browser, where the theme is not
+returned immediately when the function is called. But it is returned normally
+when the user changes it.
+
+This can be a problem in determining the initial theme of the web app. Because,
+by default, Streamlit uses the user's operating system setting (which might be
+unknown) to automatically apply the light or dark mode to the app, when it is
+first rendered.
+
+To solve the issue, it is recommended to set a
+[default theme configuration](https://docs.streamlit.io/library/advanced-features/theming)
+for the app, and use its value in case of ``st_theme`` returning ``None``.
+
+## Examples
+
+A basic example:
+
+``` python
+import streamlit as st
+from streamlit_theme import st_theme
+theme = st_theme()
+st.write(theme)
+```
+[![Example 1](https://github.com/gabrieltempass/streamlit-theme/raw/main/images/st_theme_1.gif)](https://st-theme-1.streamlit.app/)
+[**[App]**](https://st-theme-1.streamlit.app/) 
+[**[Source]**](https://github.com/gabrieltempass/streamlit-theme/blob/main/examples/st_theme_1.py)
+
+An example showing the CSS adjustment made, when set to ``True``:
+
+``` python
+import streamlit as st
+from streamlit_theme import st_theme
+
+adjust = st.toggle("Make the CSS adjustment")
+
+st.write("Input:")
+st.code(
+    f"""
+    st.write("Lorem ipsum")
+    st_theme(adjust={adjust})
+    st.write("Lorem ipsum")
+    """
+)
+
+st.write("Output:")
+st.write("Lorem ipsum")
+st_theme(adjust=adjust)
+st.write("Lorem ipsum")
+```
+[![Example 2](https://github.com/gabrieltempass/streamlit-theme/raw/main/images/st_theme_2.gif)](https://st-theme-2.streamlit.app/)
+[**[App]**](https://st-theme-2.streamlit.app/) 
+[**[Source]**](https://github.com/gabrieltempass/streamlit-theme/blob/main/examples/st_theme_2.py)
+
+## Requirements
+
+To use this Streamlit component in your app, you will need:
+* **Python 3.8+**
+* **Streamlit 1.20+**
+* The CSS adjustment depends on the
+  [browser compatibility with the :has pseudo-class](https://developer.mozilla.org/en-US/docs/Web/CSS/:has#browser_compatibility)
+
+## Development
+
+Ensure you have [Python 3.8+](https://www.python.org/downloads/),
+[Node.js](https://nodejs.org) and
+[npm](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)
+installed.
+
+1. Clone this repository:
+``` bash
+git clone git@github.com:gabrieltempass/streamlit-theme.git
+```
+
+2. Go to the `frontend` directory and initialize and run the component template
+frontend:
+``` bash
+cd streamlit-theme/streamlit_theme/frontend
+```
+``` bash
+npm install
+npm run dev
+```
+
+3. From a separate terminal, go to the repository root directory, create a new
+Python virtual environment, activate it and install Streamlit and the template
+as an editable package:
+``` bash
+cd streamlit-theme
+```
+``` bash
+python3 -m venv venv
+. venv/bin/activate
+pip install streamlit
+pip install -e .
+```
+
+Still from the same separate terminal, run the example Streamlit app:
+``` bash
+streamlit run streamlit_theme/example.py
+```
+
+If all goes well, you should see something like this:
+
+![Quickstart success](https://github.com/gabrieltempass/streamlit-theme/raw/main/images/development.png)
+
+Modify the frontend code at
+`streamlit_theme/frontend/src/StTheme.vue`.
+Modify the Python code at `streamlit_theme/__init__.py`.
+
+## References
+
+This Streamlit component was made with the [streamlit-component-vue-vite-template](https://github.com/gabrieltempass/streamlit-component-vue-vite-template), by
+[@gabrieltempass](https://github.com/gabrieltempass).
+
+
```

### Comparing `st-theme-1.2.2/streamlit_theme/__init__.py` & `st-theme-1.2.3/streamlit_theme/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import json
 from contextlib import nullcontext
+from importlib.metadata import version as _version
 
 import streamlit as st
 import streamlit.components.v1 as components
 from streamlit.errors import StreamlitAPIException
 
 
 _RELEASE = True
@@ -19,57 +20,60 @@
     build_dir = os.path.join(parent_dir, "frontend/dist")
     _st_theme = components.declare_component(
         "st_theme",
         path=build_dir
     )
 
 
+def print_version():
+    """Show the installed version of the Streamlit Theme package."""
+    version = _version("st-theme")
+    print(f"Streamlit Theme, version {version}")
+
+
 def stylized_container(key):
     """
+    Add a spaceless container to the app.
+    
     Insert a container into the app, which receives an iframe that does not
-    render anything. Style this container using CSS and a unique key to remove
-    the space added by Streamlit.
+    render anything. Style this container using CSS and a unique key. The style
+    targeting `"stVerticalBlockBorderWrapper"` removes 1rem of space added by
+    the iframe. While the style targeting the div that contains the iframe
+    changes its height from 1.5625rem to 0.
 
     Parameters
     ----------
-    key : str or int or None
-        The key associated with this container. This needs to be unique since
-        all styles will be applied to the container with this key.
+    key : str, int or None
+        A key associated with this container. This needs to be unique since all
+        styles will be applied to the container with this key.
 
     Returns
     -------
     container : DeltaGenerator
         A container object. Elements can be added to this container using
         either the "with" notation or by calling methods directly on the
         returned object.
     """
-    key = f"streamlit_theme_{key}"
-    selector = (
-        "div.element-container > div.stMarkdown > "
-        f"div[data-testid='stMarkdownContainer'] > p > span.{key}"
-    )
-
-    # The style targeting "stVerticalBlockBorderWrapper" removes 1 rem of space
-    # added by the iframe and another 1 rem added by st.markdown.
+    key = f"st_theme_{key}"
+    selector = f"div.element-container > div.stHtml > span.{key}"
     css = (
         f"""
         <style>
             div[data-testid="stVerticalBlockBorderWrapper"]:has({selector}) {{
-                margin-bottom: -2rem;
+                margin-bottom: -1rem;
             }}
             div[data-testid="stVerticalBlock"]:has(> {selector}) div:has(iframe) {{
                 height: 0;
             }}
         </style>
         """
         f"<span class='{key}'></span>"
     )
-
     container = st.container()
-    container.markdown(css, unsafe_allow_html=True)
+    container.html(css)
     return container
 
 
 def st_theme(adjust=True, key=None):
     """
     Get the active theme of the Streamlit app.
 
@@ -90,22 +94,22 @@
         the frontend to fetch the active theme, it makes a CSS adjustment to
         remove this space.
 
         In most cases, the CSS adjustment does not interfere with the rest of
         the web app, however there could be some situations where this occurs.
         If this happens, or it is desired to disable it, pass ``False`` to
         `adjust` and, when necessary, make your own CSS adjustment with
-        ``st.markdown``.
+        ``st.html``.
     key : str or int, optional
         A string or integer to use as a unique key for the component. Multiple
         ``st_themes`` may not share the same key. Defaults to ``None``.
 
     Returns
     -------
-    theme : dict of str: str or None
+    theme : dict of {str : str} or None
         A dictionary with the style settings being used by the active theme of
         the Streamlit app, or ``None``, if for some reason it could not be
         fetched.
 
     Notes
     -----
     There is a known bug, that depends on the browser, where the theme is not
@@ -114,41 +118,27 @@
 
     This can be a problem in determining the initial theme of the web app.
     Because, by default, Streamlit uses the user's operating system setting
     (which might be unknown) to automatically apply the light or dark mode to
     the app, when it is first rendered.
 
     To solve the issue, it is recommended to set a default theme configuration
-    (https://docs.streamlit.io/library/advanced-features/theming) for the app,
+    for the app (https://docs.streamlit.io/library/advanced-features/theming),
     and use its value in case of ``st_theme`` returning ``None``.
 
     Examples
     --------
+    >>> import streamlit as st
     >>> from streamlit_theme import st_theme
     >>> theme = st_theme()
-    >>> theme
-    {
-        "primaryColor": "#ff4b4b"
-        "backgroundColor": "#ffffff"
-        "secondaryBackgroundColor": "#f0f2f6"
-        "textColor": "#31333F"
-        "base": "light"
-        "font": ""Source Sans Pro", sans-serif"
-        "linkText": "#0068c9"
-        "fadedText05": "rgba(49, 51, 63, 0.1)"
-        "fadedText10": "rgba(49, 51, 63, 0.2)"
-        "fadedText20": "rgba(49, 51, 63, 0.3)"
-        "fadedText40": "rgba(49, 51, 63, 0.4)"
-        "fadedText60": "rgba(49, 51, 63, 0.6)"
-        "bgMix": "rgba(248, 249, 251, 1)"
-        "darkenedBgMix100": "hsla(220, 27%, 68%, 1)"
-        "darkenedBgMix25": "rgba(151, 166, 195, 0.25)"
-        "darkenedBgMix15": "rgba(151, 166, 195, 0.15)"
-        "lightenedBg05": "hsla(0, 0%, 100%, 1)"
-    }
+    >>> st.write(theme)
+    
+    .. output::
+       https://st-theme-1.streamlit.app/
+       height: 300px
     """
     
     if not isinstance(adjust, bool):
         raise StreamlitAPIException(
             "The adjust parameter from st_theme() received an invalid type.\n"
             "\nExpected: *bool*  "
             f"\nGot: *{type(adjust).__name__}*"
```

### Comparing `st-theme-1.2.2/streamlit_theme/frontend/dist/assets/index--ZWO88yE.js` & `st-theme-1.2.3/streamlit_theme/frontend/dist/assets/index--ZWO88yE.js`

 * *Files identical despite different names*

### Comparing `st-theme-1.2.2/streamlit_theme/frontend/dist/index.html` & `st-theme-1.2.3/streamlit_theme/frontend/dist/index.html`

 * *Files identical despite different names*


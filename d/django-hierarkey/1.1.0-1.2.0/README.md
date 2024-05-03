# Comparing `tmp/django-hierarkey-1.1.0.tar.gz` & `tmp/django_hierarkey-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-hierarkey-1.1.0.tar", last modified: Mon Mar  7 09:26:37 2022, max compression
+gzip compressed data, was "django_hierarkey-1.2.0.tar", last modified: Fri May  3 10:22:11 2024, max compression
```

## Comparing `django-hierarkey-1.1.0.tar` & `django_hierarkey-1.2.0.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2022-03-07 09:26:37.658133 django-hierarkey-1.1.0/
--rw-r--r--   0 raphael   (1000) raphael   (1000)      304 2022-02-19 18:45:31.000000 django-hierarkey-1.1.0/AUTHORS
--rw-r--r--   0 raphael   (1000) raphael   (1000)    11358 2022-02-19 18:45:31.000000 django-hierarkey-1.1.0/LICENSE
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1964 2022-03-07 09:26:37.658133 django-hierarkey-1.1.0/PKG-INFO
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1220 2022-03-07 09:07:08.000000 django-hierarkey-1.1.0/README.rst
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2022-03-07 09:26:37.658133 django-hierarkey-1.1.0/django_hierarkey.egg-info/
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1964 2022-03-07 09:26:37.000000 django-hierarkey-1.1.0/django_hierarkey.egg-info/PKG-INFO
--rw-r--r--   0 raphael   (1000) raphael   (1000)      324 2022-03-07 09:26:37.000000 django-hierarkey-1.1.0/django_hierarkey.egg-info/SOURCES.txt
--rw-r--r--   0 raphael   (1000) raphael   (1000)        1 2022-03-07 09:26:37.000000 django-hierarkey-1.1.0/django_hierarkey.egg-info/dependency_links.txt
--rw-r--r--   0 raphael   (1000) raphael   (1000)       16 2022-03-07 09:26:37.000000 django-hierarkey-1.1.0/django_hierarkey.egg-info/requires.txt
--rw-r--r--   0 raphael   (1000) raphael   (1000)       10 2022-03-07 09:26:37.000000 django-hierarkey-1.1.0/django_hierarkey.egg-info/top_level.txt
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2022-03-07 09:26:37.658133 django-hierarkey-1.1.0/hierarkey/
--rw-r--r--   0 raphael   (1000) raphael   (1000)       18 2022-03-07 09:26:15.000000 django-hierarkey-1.1.0/hierarkey/__init__.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     3872 2022-03-07 09:18:31.000000 django-hierarkey-1.1.0/hierarkey/forms.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     8264 2022-03-07 09:24:16.000000 django-hierarkey-1.1.0/hierarkey/models.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     8681 2022-02-19 18:45:31.000000 django-hierarkey-1.1.0/hierarkey/proxy.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)      380 2022-03-07 09:26:37.658133 django-hierarkey-1.1.0/setup.cfg
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1355 2022-03-07 09:25:56.000000 django-hierarkey-1.1.0/setup.py
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2024-05-03 10:22:11.968499 django_hierarkey-1.2.0/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      304 2022-02-19 18:45:31.000000 django_hierarkey-1.2.0/AUTHORS
+-rw-r--r--   0 raphael   (1000) raphael   (1000)    11358 2022-02-19 18:45:31.000000 django_hierarkey-1.2.0/LICENSE
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     1975 2024-05-03 10:22:11.968499 django_hierarkey-1.2.0/PKG-INFO
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     1220 2022-03-07 09:07:08.000000 django_hierarkey-1.2.0/README.rst
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2024-05-03 10:22:11.968499 django_hierarkey-1.2.0/django_hierarkey.egg-info/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     1975 2024-05-03 10:22:11.000000 django_hierarkey-1.2.0/django_hierarkey.egg-info/PKG-INFO
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      401 2024-05-03 10:22:11.000000 django_hierarkey-1.2.0/django_hierarkey.egg-info/SOURCES.txt
+-rw-r--r--   0 raphael   (1000) raphael   (1000)        1 2024-05-03 10:22:11.000000 django_hierarkey-1.2.0/django_hierarkey.egg-info/dependency_links.txt
+-rw-r--r--   0 raphael   (1000) raphael   (1000)       16 2024-05-03 10:22:11.000000 django_hierarkey-1.2.0/django_hierarkey.egg-info/requires.txt
+-rw-r--r--   0 raphael   (1000) raphael   (1000)       10 2024-05-03 10:22:11.000000 django_hierarkey-1.2.0/django_hierarkey.egg-info/top_level.txt
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2024-05-03 10:22:11.968499 django_hierarkey-1.2.0/hierarkey/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)       18 2024-05-03 10:20:57.000000 django_hierarkey-1.2.0/hierarkey/__init__.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     3872 2022-03-07 09:18:31.000000 django_hierarkey-1.2.0/hierarkey/forms.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     8509 2024-05-03 10:20:43.000000 django_hierarkey-1.2.0/hierarkey/models.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     8657 2024-05-03 10:20:43.000000 django_hierarkey-1.2.0/hierarkey/proxy.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      380 2024-05-03 10:22:11.968499 django_hierarkey-1.2.0/setup.cfg
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     1355 2022-03-07 09:25:56.000000 django_hierarkey-1.2.0/setup.py
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2024-05-03 10:22:11.968499 django_hierarkey-1.2.0/tests/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     5756 2022-03-07 09:25:03.000000 django_hierarkey-1.2.0/tests/test_form.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      707 2022-02-19 18:45:31.000000 django_hierarkey-1.2.0/tests/test_improperly_configured.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)    11145 2022-02-19 18:45:31.000000 django_hierarkey-1.2.0/tests/test_storage.py
```

### Comparing `django-hierarkey-1.1.0/LICENSE` & `django_hierarkey-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-hierarkey-1.1.0/PKG-INFO` & `django_hierarkey-1.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: django-hierarkey
-Version: 1.1.0
+Version: 1.2.0
 Summary: Hierarchical key-value store for django
 Home-page: https://github.com/raphaelm/django-hierarkey
 Author: Raphael Michel
 Author-email: mail@raphaelmichel.de
 License: Apache License 2.0
 Keywords: strings database models keyvalue
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 License-File: LICENSE
 License-File: AUTHORS
+Requires-Dist: python-dateutil
 
 django-hierarkey -- Hierarchical key-value store
 ================================================
 
 .. image:: https://img.shields.io/pypi/v/django-hierarkey.svg
    :target: https://pypi.python.org/pypi/django-hierarkey
 
@@ -43,9 +43,7 @@
 The code in this repository is published under the terms of the Apache License. 
 See the LICENSE file for the complete license text.
 
 This project is maintained by Raphael Michel <mail@raphaelmichel.de>. See the
 AUTHORS file for a list of all the awesome folks who contributed to this project.
 
 .. _pretix: https://github.com/pretix/pretix
-
-
```

### Comparing `django-hierarkey-1.1.0/README.rst` & `django_hierarkey-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-hierarkey-1.1.0/django_hierarkey.egg-info/PKG-INFO` & `django_hierarkey-1.2.0/django_hierarkey.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: django-hierarkey
-Version: 1.1.0
+Version: 1.2.0
 Summary: Hierarchical key-value store for django
 Home-page: https://github.com/raphaelm/django-hierarkey
 Author: Raphael Michel
 Author-email: mail@raphaelmichel.de
 License: Apache License 2.0
 Keywords: strings database models keyvalue
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 License-File: LICENSE
 License-File: AUTHORS
+Requires-Dist: python-dateutil
 
 django-hierarkey -- Hierarchical key-value store
 ================================================
 
 .. image:: https://img.shields.io/pypi/v/django-hierarkey.svg
    :target: https://pypi.python.org/pypi/django-hierarkey
 
@@ -43,9 +43,7 @@
 The code in this repository is published under the terms of the Apache License. 
 See the LICENSE file for the complete license text.
 
 This project is maintained by Raphael Michel <mail@raphaelmichel.de>. See the
 AUTHORS file for a list of all the awesome folks who contributed to this project.
 
 .. _pretix: https://github.com/pretix/pretix
-
-
```

### Comparing `django-hierarkey-1.1.0/hierarkey/forms.py` & `django_hierarkey-1.2.0/hierarkey/forms.py`

 * *Files identical despite different names*

### Comparing `django-hierarkey-1.1.0/hierarkey/models.py` & `django_hierarkey-1.2.0/hierarkey/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,22 @@
 
         :param key: Key
         :param value: *Serialized* default value, i.e. a string or ``None``.
         :param default_type: The type to deserialize values for this key to, defaults to ``str``.
         """
         self.defaults[key] = HierarkeyDefault(value, default_type)
 
+    def get_declared_type(self, key: str) -> type:
+        """
+        Returns the type that is declared for a key using add_default.
+
+        :param key: Key
+        """
+        return self.defaults[key].type if key in self.defaults else None
+
     def add_type(self, type: type, serialize: Callable[[Any], str], unserialize: Callable[[str], Any]) -> None:
         """
         Adds serialization support for a new type.
 
         :param type: The type to add support for.
         :param serialize: A callable that takes an object of type ``type`` and returns a string.
         :param unserialize: A callable that takes a string and returns an object of type ``type``.
```

### Comparing `django-hierarkey-1.1.0/hierarkey/proxy.py` & `django_hierarkey-1.2.0/hierarkey/proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,16 +152,16 @@
         up to the global settings layer (if configured) will be queried. If still no value is
         found, a default value set in ths source code will be returned if one exists.
         If not, the value of the ``default`` argument of this method will be returned instead.
 
         If you receive a ``File`` object, it will already be opened. You can specify the ``binary_file``
         flag to indicate that it should be opened in binary mode.
         """
-        if as_type is None and key in self._h.defaults:
-            as_type = self._h.defaults[key].type
+        if as_type is None:
+            as_type = self._h.get_declared_type(key)
 
         if key in self._cache():
             value = self._cache()[key]
         else:
             value = None
             if self._parent:
                 value = getattr(self._parent, self._h.attribute_name).get(key, as_type=str)
```

### Comparing `django-hierarkey-1.1.0/setup.py` & `django_hierarkey-1.2.0/setup.py`

 * *Files identical despite different names*


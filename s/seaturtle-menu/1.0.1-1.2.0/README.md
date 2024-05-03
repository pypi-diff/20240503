# Comparing `tmp/seaturtle_menu-1.0.1.tar.gz` & `tmp/seaturtle_menu-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seaturtle_menu-1.0.1.tar", last modified: Thu May  2 19:40:18 2024, max compression
+gzip compressed data, was "seaturtle_menu-1.2.0.tar", last modified: Fri May  3 21:43:58 2024, max compression
```

## Comparing `seaturtle_menu-1.0.1.tar` & `seaturtle_menu-1.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 tathya    (1000) tathya    (1000)        0 2024-05-02 19:40:18.406342 seaturtle_menu-1.0.1/
--rw-rw-r--   0 tathya    (1000) tathya    (1000)     1058 2024-05-02 16:30:48.000000 seaturtle_menu-1.0.1/LICENSE
--rw-r--r--   0 tathya    (1000) tathya    (1000)     2143 2024-05-02 19:40:18.406342 seaturtle_menu-1.0.1/PKG-INFO
--rw-rw-r--   0 tathya    (1000) tathya    (1000)      377 2024-05-02 17:28:04.000000 seaturtle_menu-1.0.1/README.md
--rw-rw-r--   0 tathya    (1000) tathya    (1000)      756 2024-05-02 19:39:27.000000 seaturtle_menu-1.0.1/pyproject.toml
-drwxrwxr-x   0 tathya    (1000) tathya    (1000)        0 2024-05-02 19:40:18.406342 seaturtle_menu-1.0.1/seaturtle_menu/
--rw-rw-r--   0 tathya    (1000) tathya    (1000)      331 2024-05-02 19:39:32.000000 seaturtle_menu-1.0.1/seaturtle_menu/__init__.py
--rw-rw-r--   0 tathya    (1000) tathya    (1000)     2575 2024-05-02 18:51:21.000000 seaturtle_menu-1.0.1/seaturtle_menu/bullets.py
--rw-rw-r--   0 tathya    (1000) tathya    (1000)       81 2024-05-02 16:19:13.000000 seaturtle_menu-1.0.1/seaturtle_menu/consts.py
--rw-rw-r--   0 tathya    (1000) tathya    (1000)     3101 2024-05-02 19:38:23.000000 seaturtle_menu-1.0.1/seaturtle_menu/menu.py
--rw-rw-r--   0 tathya    (1000) tathya    (1000)      229 2024-05-02 13:25:08.000000 seaturtle_menu-1.0.1/seaturtle_menu/utils.py
-drwxrwxr-x   0 tathya    (1000) tathya    (1000)        0 2024-05-02 19:40:18.406342 seaturtle_menu-1.0.1/seaturtle_menu.egg-info/
--rw-r--r--   0 tathya    (1000) tathya    (1000)     2143 2024-05-02 19:40:18.000000 seaturtle_menu-1.0.1/seaturtle_menu.egg-info/PKG-INFO
--rw-rw-r--   0 tathya    (1000) tathya    (1000)      318 2024-05-02 19:40:18.000000 seaturtle_menu-1.0.1/seaturtle_menu.egg-info/SOURCES.txt
--rw-rw-r--   0 tathya    (1000) tathya    (1000)        1 2024-05-02 19:40:18.000000 seaturtle_menu-1.0.1/seaturtle_menu.egg-info/dependency_links.txt
--rw-rw-r--   0 tathya    (1000) tathya    (1000)       15 2024-05-02 19:40:18.000000 seaturtle_menu-1.0.1/seaturtle_menu.egg-info/top_level.txt
--rw-rw-r--   0 tathya    (1000) tathya    (1000)       38 2024-05-02 19:40:18.406342 seaturtle_menu-1.0.1/setup.cfg
--rw-rw-r--   0 tathya    (1000) tathya    (1000)      666 2024-05-02 19:39:22.000000 seaturtle_menu-1.0.1/setup.py
+drwxrwxr-x   0 tathya    (1000) tathya    (1000)        0 2024-05-03 21:43:58.250208 seaturtle_menu-1.2.0/
+-rw-rw-r--   0 tathya    (1000) tathya    (1000)     1058 2024-05-02 16:30:48.000000 seaturtle_menu-1.2.0/LICENSE
+-rw-r--r--   0 tathya    (1000) tathya    (1000)     2143 2024-05-03 21:43:58.246209 seaturtle_menu-1.2.0/PKG-INFO
+-rw-rw-r--   0 tathya    (1000) tathya    (1000)      377 2024-05-02 17:28:04.000000 seaturtle_menu-1.2.0/README.md
+-rw-rw-r--   0 tathya    (1000) tathya    (1000)      756 2024-05-03 21:43:25.000000 seaturtle_menu-1.2.0/pyproject.toml
+drwxrwxr-x   0 tathya    (1000) tathya    (1000)        0 2024-05-03 21:43:58.246209 seaturtle_menu-1.2.0/seaturtle_menu/
+-rw-rw-r--   0 tathya    (1000) tathya    (1000)      331 2024-05-03 21:43:32.000000 seaturtle_menu-1.2.0/seaturtle_menu/__init__.py
+-rw-rw-r--   0 tathya    (1000) tathya    (1000)     2483 2024-05-02 21:23:30.000000 seaturtle_menu-1.2.0/seaturtle_menu/bullets.py
+-rw-rw-r--   0 tathya    (1000) tathya    (1000)       81 2024-05-02 16:19:13.000000 seaturtle_menu-1.2.0/seaturtle_menu/consts.py
+-rw-rw-r--   0 tathya    (1000) tathya    (1000)     3433 2024-05-03 21:42:56.000000 seaturtle_menu-1.2.0/seaturtle_menu/menu.py
+-rw-rw-r--   0 tathya    (1000) tathya    (1000)      229 2024-05-02 13:25:08.000000 seaturtle_menu-1.2.0/seaturtle_menu/utils.py
+drwxrwxr-x   0 tathya    (1000) tathya    (1000)        0 2024-05-03 21:43:58.246209 seaturtle_menu-1.2.0/seaturtle_menu.egg-info/
+-rw-r--r--   0 tathya    (1000) tathya    (1000)     2143 2024-05-03 21:43:58.000000 seaturtle_menu-1.2.0/seaturtle_menu.egg-info/PKG-INFO
+-rw-rw-r--   0 tathya    (1000) tathya    (1000)      318 2024-05-03 21:43:58.000000 seaturtle_menu-1.2.0/seaturtle_menu.egg-info/SOURCES.txt
+-rw-rw-r--   0 tathya    (1000) tathya    (1000)        1 2024-05-03 21:43:58.000000 seaturtle_menu-1.2.0/seaturtle_menu.egg-info/dependency_links.txt
+-rw-rw-r--   0 tathya    (1000) tathya    (1000)       15 2024-05-03 21:43:58.000000 seaturtle_menu-1.2.0/seaturtle_menu.egg-info/top_level.txt
+-rw-rw-r--   0 tathya    (1000) tathya    (1000)       38 2024-05-03 21:43:58.250208 seaturtle_menu-1.2.0/setup.cfg
+-rw-rw-r--   0 tathya    (1000) tathya    (1000)      666 2024-05-03 21:43:20.000000 seaturtle_menu-1.2.0/setup.py
```

### Comparing `seaturtle_menu-1.0.1/LICENSE` & `seaturtle_menu-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `seaturtle_menu-1.0.1/PKG-INFO` & `seaturtle_menu-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seaturtle_menu
-Version: 1.0.1
+Version: 1.2.0
 Summary: Make effective terminal menus quickly and concisely.
 Author: Tathya Garg
 Author-email: Tathya Garg <tathya.garg@gmail.com>
 Maintainer-email: Tathya Garg <tathya.garg@gmail.com>
 License: Copyright 2024 Tathya Garg
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `seaturtle_menu-1.0.1/pyproject.toml` & `seaturtle_menu-1.2.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "seaturtle_menu"
-version = "1.0.1"
+version = "1.2.0"
 dependencies = []
 requires-python = ">=3.12"
 authors = [
   {name = "Tathya Garg", email = "tathya.garg@gmail.com"},
 ]
 maintainers = [
   {name = "Tathya Garg", email = "tathya.garg@gmail.com"},
```

### Comparing `seaturtle_menu-1.0.1/seaturtle_menu/bullets.py` & `seaturtle_menu-1.2.0/seaturtle_menu/bullets.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,26 +12,21 @@
 
         self.charset = list(charset)
         self.allow_increase_width = allow_increase_width
         self.width = width
         self.start = start
 
     def make_iter(self, width: int = 1) -> list[str]:
-        """
-        Make a list of bullets with the desired width.
-
-        Args:
-            width: The width of each bullet to return, in terms of bullet count.
+        """Make a list of bullets with the desired width.
 
-        Returns:
-            A list of bullets with the desired width
+        :param width: The width of each bullet to return, in terms of bullet count (default is 1)
+        :type width: int
 
-        Example usage:
-            >>> Bullets('abc', width=2).make_iter(2)
-            ['aa', 'ab', 'ac', 'ba', 'bb', 'bc', 'ca', 'cb', 'cc']
+        :returns: A list of bullets with the desired width
+        :rtype: list[str]
         """
         if width == 1: return self.charset
 
         items: list[str] = self.make_iter(width - 1)
         result: list[str] = []
 
         for i, item in enumerate(items * len(self.charset)):
@@ -54,22 +49,21 @@
     This class is used as an intermediate which is created before you know the desired width.
     """
     def __init__(self, maker: Callable[[int], Bullets], charset_len: int) -> None:
         self.maker = maker
         self.charset_len = charset_len
 
     def from_width(self, width: int) -> Bullets:
-        """
-        Make a Bullets object after you know the desired width.
+        """Make a Bullets object after you know the desired width.
 
-        Args:
-            width: The desired width of the Bullets object
+        :param width: The desired width of the Bullets object
+        :type width: int
 
-        Returns:
-            A Bullets object from the maker function with the given width.
+        :returns: A Bullets object from the maker function with the given width.
+        :rtype: Bullets
         """
         return self.maker(width)
 
 
 LOWERCASE_ALPHABET: Bulletable = Bulletable(maker=lambda width: Bullets(string.ascii_lowercase, width=width), charset_len=len(string.ascii_lowercase))
 UPPERCASE_ALPHABET: Bulletable = Bulletable(maker=lambda width: Bullets(string.ascii_uppercase, width=width), charset_len=len(string.ascii_uppercase))
 DIGITS: Bulletable = Bulletable(maker=lambda width: Bullets(string.digits, width=width, start=1), charset_len=len(string.digits))
```

### Comparing `seaturtle_menu-1.0.1/seaturtle_menu/menu.py` & `seaturtle_menu-1.2.0/seaturtle_menu/menu.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,36 +6,40 @@
 
 class Menu:
     def __init__(
             self,
             _bullets: Bullets | Bulletable,
             action_prompt_map: dict[str, Callable | None],
             *,
+            restart_after_action: bool = False,
             bracketing: str = '.',
             use_default_function: bool = False,
             input_converter: Callable[[str], str] = None,
             greeting: str = ''
     ) -> None:
         input_converter = input_converter or (lambda text: text)
 
-        verify_type(use_default_function, bool)
+        verify_type(_bullets, (Bullets, Bulletable))
         verify_type(action_prompt_map, dict)
         for k, v in action_prompt_map.items():
             verify_type(k, str)
             if v:
                 verify_type(v, Callable)
             elif use_default_function:
                 action_prompt_map[k] = DEFAULT_ACTION
             else:
                 raise ValueError(
                     f"Expected Callable value as value for key = {k}, found {type(v)}. Use `use_default_function=True` to use a default function instead."
                 )
 
-        verify_type(_bullets, (Bullets, Bulletable))
+        verify_type(restart_after_action, bool)
+        verify_type(bracketing, str)
+        verify_type(use_default_function, bool)
         verify_type(input_converter, Callable)
+        verify_type(greeting, str)
 
         self.action_prompt_map = action_prompt_map
         self.prompts: list[str] = list(action_prompt_map.keys())
         self.actions: list[Callable] = list(action_prompt_map.values())
         if isinstance(_bullets, Bulletable):
             size: int = len(self.prompts)
             width = 0
@@ -50,39 +54,40 @@
             self.width = _bullets.width
             self.bullets = _bullets
 
         self.bullets_as_list = list(self.bullets)[:len(self.prompts)]
         self.bracketing: str = bracketing
         self.converter: Callable[[str], str] = input_converter
         self.greeting = greeting
+        self.restart_after_action = restart_after_action
 
     def get_verified_input(self) -> str:
-        """
-        Gets user input that is guaranteed to be one of the bullets.
+        """Gets user input that is guaranteed to be one of the bullets.
 
-        Returns:
-            A user choice that is in the bullets.
+        :returns: A user choice that is in the bullets.
+        :rtype: str
         """
-        choice = input('>>> ')
+        choice = input('Choice: ')
         while choice not in self.bullets_as_list and \
                 self.converter(choice) not in self.bullets_as_list:
             print('Invalid!')
-            choice = input('>>> ')
+            choice = input('Choice: ')
 
         return self.converter(choice)
 
     def run(self) -> Any:
-        """
-        Runs the menu.
-        Prints out the greeting, options, gets a verified user input, and performs the associated action.
+        """Runs the menu. Prints out the greeting, options, gets a verified user input, and performs the associated action.
 
-        Returns:
-            The value returned by the function associated to the user's choice.
+        :returns: The value returned by the function associated to the user's choice (provided restart_after_action is False).
+        :rtype: Any
         """
         if self.greeting:
             print(self.greeting)
 
         for bullet, prompt in zip(self.bullets, self.prompts):
             print(f'{bullet}{self.bracketing} {prompt}')
 
         choice: str = self.get_verified_input()
-        return self.action_prompt_map[self.prompts[self.bullets_as_list.index(choice)]]()
+
+        if not self.restart_after_action:
+            return self.action_prompt_map[self.prompts[self.bullets_as_list.index(choice)]]()
+        self.run()
```

### Comparing `seaturtle_menu-1.0.1/seaturtle_menu.egg-info/PKG-INFO` & `seaturtle_menu-1.2.0/seaturtle_menu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seaturtle_menu
-Version: 1.0.1
+Version: 1.2.0
 Summary: Make effective terminal menus quickly and concisely.
 Author: Tathya Garg
 Author-email: Tathya Garg <tathya.garg@gmail.com>
 Maintainer-email: Tathya Garg <tathya.garg@gmail.com>
 License: Copyright 2024 Tathya Garg
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `seaturtle_menu-1.0.1/setup.py` & `seaturtle_menu-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.1'
+VERSION = '1.2.0'
 DESCRIPTION = 'Make effective terminal menus quickly and concisely.'
 
 setup(
     name='seaturtle_menu',
     version=VERSION,
     author='Tathya Garg',
     author_email='tathya.garg@gmail.com',
```


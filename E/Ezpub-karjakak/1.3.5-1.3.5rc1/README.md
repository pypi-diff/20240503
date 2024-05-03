# Comparing `tmp/ezpub_karjakak-1.3.5.tar.gz` & `tmp/Ezpub-karjakak-1.3.5rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezpub_karjakak-1.3.5.tar", last modified: Fri May  3 07:04:18 2024, max compression
+gzip compressed data, was "Ezpub-karjakak-1.3.5rc1.tar", last modified: Wed Mar 27 06:08:51 2024, max compression
```

## Comparing `ezpub_karjakak-1.3.5.tar` & `Ezpub-karjakak-1.3.5rc1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 07:04:18.781411 ezpub_karjakak-1.3.5/
-drwxrwxrwx   0        0        0        0 2024-05-03 07:04:18.758669 ezpub_karjakak-1.3.5/Ezpub/
--rw-rw-rw-   0        0        0       23 2024-02-26 00:12:04.000000 ezpub_karjakak-1.3.5/Ezpub/__init__.py
--rw-rw-rw-   0        0        0     8713 2024-05-03 06:45:47.000000 ezpub_karjakak-1.3.5/Ezpub/ezpub.py
-drwxrwxrwx   0        0        0        0 2024-05-03 07:04:18.777035 ezpub_karjakak-1.3.5/Ezpub_karjakak.egg-info/
--rw-rw-rw-   0        0        0     2604 2024-05-03 07:04:18.000000 ezpub_karjakak-1.3.5/Ezpub_karjakak.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-05-03 07:04:18.000000 ezpub_karjakak-1.3.5/Ezpub_karjakak.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 07:04:18.000000 ezpub_karjakak-1.3.5/Ezpub_karjakak.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-05-03 07:04:18.000000 ezpub_karjakak-1.3.5/Ezpub_karjakak.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      129 2024-05-03 07:04:18.000000 ezpub_karjakak-1.3.5/Ezpub_karjakak.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-03 07:04:18.000000 ezpub_karjakak-1.3.5/Ezpub_karjakak.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1086 2024-02-26 00:12:04.000000 ezpub_karjakak-1.3.5/LICENSE
--rw-rw-rw-   0        0        0     2604 2024-05-03 07:04:18.780453 ezpub_karjakak-1.3.5/PKG-INFO
--rw-rw-rw-   0        0        0     1766 2024-05-03 07:02:37.000000 ezpub_karjakak-1.3.5/README.md
--rw-rw-rw-   0        0        0      124 2024-02-26 00:12:04.000000 ezpub_karjakak-1.3.5/pyproject.toml
--rw-rw-rw-   0        0        0      908 2024-05-03 07:04:18.781411 ezpub_karjakak-1.3.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-03-27 06:08:51.345276 Ezpub-karjakak-1.3.5rc1/
+drwxrwxrwx   0        0        0        0 2024-03-27 06:08:51.323169 Ezpub-karjakak-1.3.5rc1/Ezpub/
+-rw-rw-rw-   0        0        0       23 2024-02-26 00:12:04.000000 Ezpub-karjakak-1.3.5rc1/Ezpub/__init__.py
+-rw-rw-rw-   0        0        0     8709 2024-03-27 04:40:02.000000 Ezpub-karjakak-1.3.5rc1/Ezpub/ezpub.py
+drwxrwxrwx   0        0        0        0 2024-03-27 06:08:51.342589 Ezpub-karjakak-1.3.5rc1/Ezpub_karjakak.egg-info/
+-rw-rw-rw-   0        0        0     2614 2024-03-27 06:08:51.000000 Ezpub-karjakak-1.3.5rc1/Ezpub_karjakak.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2024-03-27 06:08:51.000000 Ezpub-karjakak-1.3.5rc1/Ezpub_karjakak.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-27 06:08:51.000000 Ezpub-karjakak-1.3.5rc1/Ezpub_karjakak.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-03-27 06:08:51.000000 Ezpub-karjakak-1.3.5rc1/Ezpub_karjakak.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      129 2024-03-27 06:08:51.000000 Ezpub-karjakak-1.3.5rc1/Ezpub_karjakak.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-03-27 06:08:51.000000 Ezpub-karjakak-1.3.5rc1/Ezpub_karjakak.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1086 2024-02-26 00:12:04.000000 Ezpub-karjakak-1.3.5rc1/LICENSE
+-rw-rw-rw-   0        0        0     2614 2024-03-27 06:08:51.345276 Ezpub-karjakak-1.3.5rc1/PKG-INFO
+-rw-rw-rw-   0        0        0     1773 2024-03-27 04:32:01.000000 Ezpub-karjakak-1.3.5rc1/README.md
+-rw-rw-rw-   0        0        0      124 2024-02-26 00:12:04.000000 Ezpub-karjakak-1.3.5rc1/pyproject.toml
+-rw-rw-rw-   0        0        0      911 2024-03-27 06:08:51.345276 Ezpub-karjakak-1.3.5rc1/setup.cfg
```

### Comparing `ezpub_karjakak-1.3.5/Ezpub/ezpub.py` & `Ezpub-karjakak-1.3.5rc1/Ezpub/ezpub.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,20 +200,20 @@
         ppth = self.pathpypi()
         ckplt = (
             (Path(ppth), True) if platform.startswith("win") else (Path(ppth), False)
         )
         match (altr := os.path.exists(ckplt[0]), ckplt[1]):
             case (True, True):
                 os.chdir(ckplt[0].parent)
-                pnam = f'python3 -m twine upload \"{pth}\"'
+                pnam = f'python3 -m twine upload "{pth}"'
                 self.popenp(pnam)
             case (True, False):
                 os.chdir(ckplt[0].parent)
                 self.prre(ppth)
-                pnam = ["python3", "-m", "twine", "upload", f'\"{pth}\"']
+                pnam = ["python3", "-m", "twine", "upload", f'"{pth}"']
                 self.popenp(pnam)
                 self.prre(ppth, False)
             case (False, _):
                 print("Please create token first!")
         del pth, ppth, ckplt, altr
```

### Comparing `ezpub_karjakak-1.3.5/Ezpub_karjakak.egg-info/PKG-INFO` & `Ezpub-karjakak-1.3.5rc1/Ezpub_karjakak.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Ezpub-karjakak
-Version: 1.3.5
+Version: 1.3.5rc1
 Summary: Ezpub is a tool for developer to upload package to PyPI
 Home-page: https://github.com/kakkarja/Ezpub
 Author: karjakak
 Author-email: kakkarja.github@gmail.com
 License: MIT License
 Classifier: Environment :: Console
 Classifier: Environment :: Win32 (MS Windows)
@@ -28,15 +28,15 @@
 
 ## Installation
 
 ```Terminal
 pip3 install Ezpub-karjakak
 ```
 
->**Ezpub require setuptools as back-end engine and pyproject.toml file (setup.cfg is optional).**
+>**Publish package require setuptools as back-end engine and pyproject.toml file (setup.cfg is optional).**
 
 ## Usage
 
 **Create token for variable environment and save it for publish with twine [token key-in in tkinter simpledialog for showing in hidden].**
 
 ```Terminal
 ezpub -t None
@@ -58,33 +58,33 @@
 ezpub -t $VARTOKEN
 ```
 
 **Building the package and create [build, dist, and package.egg-info] for uploading to PyPI.**
 
 ```Terminal
 # Window
-ezpub -b .\package-path\
+ezpub -b "\package-path"
 
 # MacOS X
-ezpub -b ./package_path/
+ezpub -b /package_path
 ```
 
 **TAKE NOTE:**
 
 * **Ezpub will try to move existing [build, dist, and package.egg-info] to created archive folder and create new one.**
   * **If Exception occured, user need to remove them manually.**
 
 **Pubish to PyPI.**
 
 ```Terminal
 # For Windows only
-ezpub -p .\package-path\dist\*
+ezpub -p \package-path\dist\*
 
 # For MacOS X
-ezpub -p ./package_path/dist/*
+ezpub -p "package_path/dist/*"
 ```
 
 **TAKE NOTE:**
 
 * **If token is not created yet, ~~it will start process "-t" automatically~~ user will be prompt to create first.**
 * **Some firewall not allowed moving files to archive, you may exclude Ezpub from it.**
 * **You can move the files manually and using `py -m build`  instead. [Please see the source code for assurance]**
```

### Comparing `ezpub_karjakak-1.3.5/LICENSE` & `Ezpub-karjakak-1.3.5rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `ezpub_karjakak-1.3.5/PKG-INFO` & `Ezpub-karjakak-1.3.5rc1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Ezpub-karjakak
-Version: 1.3.5
+Version: 1.3.5rc1
 Summary: Ezpub is a tool for developer to upload package to PyPI
 Home-page: https://github.com/kakkarja/Ezpub
 Author: karjakak
 Author-email: kakkarja.github@gmail.com
 License: MIT License
 Classifier: Environment :: Console
 Classifier: Environment :: Win32 (MS Windows)
@@ -28,15 +28,15 @@
 
 ## Installation
 
 ```Terminal
 pip3 install Ezpub-karjakak
 ```
 
->**Ezpub require setuptools as back-end engine and pyproject.toml file (setup.cfg is optional).**
+>**Publish package require setuptools as back-end engine and pyproject.toml file (setup.cfg is optional).**
 
 ## Usage
 
 **Create token for variable environment and save it for publish with twine [token key-in in tkinter simpledialog for showing in hidden].**
 
 ```Terminal
 ezpub -t None
@@ -58,33 +58,33 @@
 ezpub -t $VARTOKEN
 ```
 
 **Building the package and create [build, dist, and package.egg-info] for uploading to PyPI.**
 
 ```Terminal
 # Window
-ezpub -b .\package-path\
+ezpub -b "\package-path"
 
 # MacOS X
-ezpub -b ./package_path/
+ezpub -b /package_path
 ```
 
 **TAKE NOTE:**
 
 * **Ezpub will try to move existing [build, dist, and package.egg-info] to created archive folder and create new one.**
   * **If Exception occured, user need to remove them manually.**
 
 **Pubish to PyPI.**
 
 ```Terminal
 # For Windows only
-ezpub -p .\package-path\dist\*
+ezpub -p \package-path\dist\*
 
 # For MacOS X
-ezpub -p ./package_path/dist/*
+ezpub -p "package_path/dist/*"
 ```
 
 **TAKE NOTE:**
 
 * **If token is not created yet, ~~it will start process "-t" automatically~~ user will be prompt to create first.**
 * **Some firewall not allowed moving files to archive, you may exclude Ezpub from it.**
 * **You can move the files manually and using `py -m build`  instead. [Please see the source code for assurance]**
```

### Comparing `ezpub_karjakak-1.3.5/README.md` & `Ezpub-karjakak-1.3.5rc1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 ## Installation
 
 ```Terminal
 pip3 install Ezpub-karjakak
 ```
 
->**Ezpub require setuptools as back-end engine and pyproject.toml file (setup.cfg is optional).**
+>**Publish package require setuptools as back-end engine and pyproject.toml file (setup.cfg is optional).**
 
 ## Usage
 
 **Create token for variable environment and save it for publish with twine [token key-in in tkinter simpledialog for showing in hidden].**
 
 ```Terminal
 ezpub -t None
@@ -34,33 +34,33 @@
 ezpub -t $VARTOKEN
 ```
 
 **Building the package and create [build, dist, and package.egg-info] for uploading to PyPI.**
 
 ```Terminal
 # Window
-ezpub -b .\package-path\
+ezpub -b "\package-path"
 
 # MacOS X
-ezpub -b ./package_path/
+ezpub -b /package_path
 ```
 
 **TAKE NOTE:**
 
 * **Ezpub will try to move existing [build, dist, and package.egg-info] to created archive folder and create new one.**
   * **If Exception occured, user need to remove them manually.**
 
 **Pubish to PyPI.**
 
 ```Terminal
 # For Windows only
-ezpub -p .\package-path\dist\*
+ezpub -p \package-path\dist\*
 
 # For MacOS X
-ezpub -p ./package_path/dist/*
+ezpub -p "package_path/dist/*"
 ```
 
 **TAKE NOTE:**
 
 * **If token is not created yet, ~~it will start process "-t" automatically~~ user will be prompt to create first.**
 * **Some firewall not allowed moving files to archive, you may exclude Ezpub from it.**
 * **You can move the files manually and using `py -m build`  instead. [Please see the source code for assurance]**
```

### Comparing `ezpub_karjakak-1.3.5/setup.cfg` & `Ezpub-karjakak-1.3.5rc1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2045 7a70 7562 2d6b 6172 6a61 6b61   = Ezpub-karjaka
 00000020: 6b0d 0a76 6572 7369 6f6e 203d 2031 2e33  k..version = 1.3
-00000030: 2e35 0d0a 6175 7468 6f72 203d 206b 6172  .5..author = kar
-00000040: 6a61 6b61 6b0d 0a61 7574 686f 725f 656d  jakak..author_em
-00000050: 6169 6c20 3d20 6b61 6b6b 6172 6a61 2e67  ail = kakkarja.g
-00000060: 6974 6875 6240 676d 6169 6c2e 636f 6d0d  ithub@gmail.com.
-00000070: 0a64 6573 6372 6970 7469 6f6e 203d 2045  .description = E
-00000080: 7a70 7562 2069 7320 6120 746f 6f6c 2066  zpub is a tool f
-00000090: 6f72 2064 6576 656c 6f70 6572 2074 6f20  or developer to 
-000000a0: 7570 6c6f 6164 2070 6163 6b61 6765 2074  upload package t
-000000b0: 6f20 5079 5049 0d0a 6c6f 6e67 5f64 6573  o PyPI..long_des
-000000c0: 6372 6970 7469 6f6e 203d 2066 696c 653a  cription = file:
-000000d0: 2052 4541 444d 452e 6d64 0d0a 6c6f 6e67   README.md..long
-000000e0: 5f64 6573 6372 6970 7469 6f6e 5f63 6f6e  _description_con
-000000f0: 7465 6e74 5f74 7970 6520 3d20 7465 7874  tent_type = text
-00000100: 2f6d 6172 6b64 6f77 6e0d 0a75 726c 203d  /markdown..url =
-00000110: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00000120: 636f 6d2f 6b61 6b6b 6172 6a61 2f45 7a70  com/kakkarja/Ezp
-00000130: 7562 0d0a 6c69 6365 6e73 6520 3d20 4d49  ub..license = MI
-00000140: 5420 4c69 6365 6e73 650d 0a63 6c61 7373  T License..class
-00000150: 6966 6965 7273 203d 200d 0a09 456e 7669  ifiers = ...Envi
-00000160: 726f 6e6d 656e 7420 3a3a 2043 6f6e 736f  ronment :: Conso
-00000170: 6c65 0d0a 0945 6e76 6972 6f6e 6d65 6e74  le...Environment
-00000180: 203a 3a20 5769 6e33 3220 284d 5320 5769   :: Win32 (MS Wi
-00000190: 6e64 6f77 7329 0d0a 0945 6e76 6972 6f6e  ndows)...Environ
-000001a0: 6d65 6e74 203a 3a20 4d61 634f 5320 580d  ment :: MacOS X.
-000001b0: 0a09 496e 7465 6e64 6564 2041 7564 6965  ..Intended Audie
-000001c0: 6e63 6520 3a3a 2044 6576 656c 6f70 6572  nce :: Developer
-000001d0: 730d 0a09 5072 6f67 7261 6d6d 696e 6720  s...Programming 
-000001e0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-000001f0: 6f6e 203a 3a20 332e 3130 0d0a 094c 6963  on :: 3.10...Lic
-00000200: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
-00000210: 6f76 6564 203a 3a20 4d49 5420 4c69 6365  oved :: MIT Lice
-00000220: 6e73 650d 0a0d 0a5b 6f70 7469 6f6e 735d  nse....[options]
-00000230: 0d0a 7061 636b 6167 6573 203d 2066 696e  ..packages = fin
-00000240: 643a 0d0a 696e 636c 7564 655f 656e 7472  d:..include_entr
-00000250: 795f 706f 696e 7473 203d 2054 7275 650d  y_points = True.
-00000260: 0a70 7974 686f 6e5f 7265 7175 6972 6573  .python_requires
-00000270: 203d 203e 3d33 2e31 300d 0a69 6e73 7461   = >=3.10..insta
-00000280: 6c6c 5f72 6571 7569 7265 7320 3d20 0d0a  ll_requires = ..
-00000290: 0954 7769 6e65 3e3d 332e 342e 310d 0a09  .Twine>=3.4.1...
-000002a0: 436c 6965 6e2d 6b61 726a 616b 616b 3e3d  Clien-karjakak>=
-000002b0: 302e 302e 380d 0a09 6669 6c65 706d 6f6e  0.0.8...filepmon
-000002c0: 2d6b 6172 6a61 6b61 6b3e 3d30 2e31 2e30  -karjakak>=0.1.0
-000002d0: 0d0a 0966 696c 666c 612d 6b61 726a 616b  ...filfla-karjak
-000002e0: 616b 3e3d 302e 312e 300d 0a09 6669 6c61  ak>=0.1.0...fila
-000002f0: 7474 2d6b 6172 6a61 6b61 6b3e 3d30 2e31  tt-karjakak>=0.1
-00000300: 2e30 0d0a 0965 7863 7074 722d 6b61 726a  .0...excptr-karj
-00000310: 616b 616b 3e3d 302e 312e 300d 0a0d 0a5b  akak>=0.1.0....[
-00000320: 6f70 7469 6f6e 732e 656e 7472 795f 706f  options.entry_po
-00000330: 696e 7473 5d0d 0a63 6f6e 736f 6c65 5f73  ints]..console_s
-00000340: 6372 6970 7473 203d 200d 0a09 657a 7075  cripts = ...ezpu
-00000350: 6220 3d20 457a 7075 623a 6d61 696e 0d0a  b = Ezpub:main..
-00000360: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
-00000370: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
-00000380: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
+00000030: 2e35 7263 310d 0a61 7574 686f 7220 3d20  .5rc1..author = 
+00000040: 6b61 726a 616b 616b 0d0a 6175 7468 6f72  karjakak..author
+00000050: 5f65 6d61 696c 203d 206b 616b 6b61 726a  _email = kakkarj
+00000060: 612e 6769 7468 7562 4067 6d61 696c 2e63  a.github@gmail.c
+00000070: 6f6d 0d0a 6465 7363 7269 7074 696f 6e20  om..description 
+00000080: 3d20 457a 7075 6220 6973 2061 2074 6f6f  = Ezpub is a too
+00000090: 6c20 666f 7220 6465 7665 6c6f 7065 7220  l for developer 
+000000a0: 746f 2075 706c 6f61 6420 7061 636b 6167  to upload packag
+000000b0: 6520 746f 2050 7950 490d 0a6c 6f6e 675f  e to PyPI..long_
+000000c0: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
+000000d0: 6c65 3a20 5245 4144 4d45 2e6d 640d 0a6c  le: README.md..l
+000000e0: 6f6e 675f 6465 7363 7269 7074 696f 6e5f  ong_description_
+000000f0: 636f 6e74 656e 745f 7479 7065 203d 2074  content_type = t
+00000100: 6578 742f 6d61 726b 646f 776e 0d0a 7572  ext/markdown..ur
+00000110: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
+00000120: 7562 2e63 6f6d 2f6b 616b 6b61 726a 612f  ub.com/kakkarja/
+00000130: 457a 7075 620d 0a6c 6963 656e 7365 203d  Ezpub..license =
+00000140: 204d 4954 204c 6963 656e 7365 0d0a 636c   MIT License..cl
+00000150: 6173 7369 6669 6572 7320 3d20 0d0a 0945  assifiers = ...E
+00000160: 6e76 6972 6f6e 6d65 6e74 203a 3a20 436f  nvironment :: Co
+00000170: 6e73 6f6c 650d 0a09 456e 7669 726f 6e6d  nsole...Environm
+00000180: 656e 7420 3a3a 2057 696e 3332 2028 4d53  ent :: Win32 (MS
+00000190: 2057 696e 646f 7773 290d 0a09 456e 7669   Windows)...Envi
+000001a0: 726f 6e6d 656e 7420 3a3a 204d 6163 4f53  ronment :: MacOS
+000001b0: 2058 0d0a 0949 6e74 656e 6465 6420 4175   X...Intended Au
+000001c0: 6469 656e 6365 203a 3a20 4465 7665 6c6f  dience :: Develo
+000001d0: 7065 7273 0d0a 0950 726f 6772 616d 6d69  pers...Programmi
+000001e0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+000001f0: 7974 686f 6e20 3a3a 2033 2e31 300d 0a09  ython :: 3.10...
+00000200: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
+00000210: 7070 726f 7665 6420 3a3a 204d 4954 204c  pproved :: MIT L
+00000220: 6963 656e 7365 0d0a 0d0a 5b6f 7074 696f  icense....[optio
+00000230: 6e73 5d0d 0a70 6163 6b61 6765 7320 3d20  ns]..packages = 
+00000240: 6669 6e64 3a0d 0a69 6e63 6c75 6465 5f65  find:..include_e
+00000250: 6e74 7279 5f70 6f69 6e74 7320 3d20 5472  ntry_points = Tr
+00000260: 7565 0d0a 7079 7468 6f6e 5f72 6571 7569  ue..python_requi
+00000270: 7265 7320 3d20 3e3d 332e 3130 0d0a 696e  res = >=3.10..in
+00000280: 7374 616c 6c5f 7265 7175 6972 6573 203d  stall_requires =
+00000290: 200d 0a09 5477 696e 653e 3d33 2e34 2e31   ...Twine>=3.4.1
+000002a0: 0d0a 0943 6c69 656e 2d6b 6172 6a61 6b61  ...Clien-karjaka
+000002b0: 6b3e 3d30 2e30 2e38 0d0a 0966 696c 6570  k>=0.0.8...filep
+000002c0: 6d6f 6e2d 6b61 726a 616b 616b 3e3d 302e  mon-karjakak>=0.
+000002d0: 312e 300d 0a09 6669 6c66 6c61 2d6b 6172  1.0...filfla-kar
+000002e0: 6a61 6b61 6b3e 3d30 2e31 2e30 0d0a 0966  jakak>=0.1.0...f
+000002f0: 696c 6174 742d 6b61 726a 616b 616b 3e3d  ilatt-karjakak>=
+00000300: 302e 312e 300d 0a09 6578 6370 7472 2d6b  0.1.0...excptr-k
+00000310: 6172 6a61 6b61 6b3e 3d30 2e31 2e30 0d0a  arjakak>=0.1.0..
+00000320: 0d0a 5b6f 7074 696f 6e73 2e65 6e74 7279  ..[options.entry
+00000330: 5f70 6f69 6e74 735d 0d0a 636f 6e73 6f6c  _points]..consol
+00000340: 655f 7363 7269 7074 7320 3d20 0d0a 0965  e_scripts = ...e
+00000350: 7a70 7562 203d 2045 7a70 7562 3a6d 6169  zpub = Ezpub:mai
+00000360: 6e0d 0a0d 0a5b 6567 675f 696e 666f 5d0d  n....[egg_info].
+00000370: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
+00000380: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
```


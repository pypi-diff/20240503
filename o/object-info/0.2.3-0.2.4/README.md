# Comparing `tmp/object_info-0.2.3.tar.gz` & `tmp/object_info-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "object_info-0.2.3.tar", last modified: Mon Mar 18 08:58:31 2024, max compression
+gzip compressed data, was "object_info-0.2.4.tar", last modified: Fri May  3 12:14:50 2024, max compression
```

## Comparing `object_info-0.2.3.tar` & `object_info-0.2.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-03-18 08:58:31.859700 object_info-0.2.3/
--rw-rw-rw-   0        0        0     1082 2023-11-27 14:37:20.000000 object_info-0.2.3/LICENSE
--rw-rw-rw-   0        0        0    13757 2024-03-18 08:58:31.858375 object_info-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0    12802 2024-03-18 08:58:07.000000 object_info-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2024-03-18 08:58:31.847084 object_info-0.2.3/object_info/
--rw-rw-rw-   0        0        0       21 2023-11-27 14:37:20.000000 object_info-0.2.3/object_info/__init__.py
--rw-rw-rw-   0        0        0    17459 2024-03-18 08:55:00.000000 object_info-0.2.3/object_info/main.py
-drwxrwxrwx   0        0        0        0 2024-03-18 08:58:31.857572 object_info-0.2.3/object_info.egg-info/
--rw-rw-rw-   0        0        0    13757 2024-03-18 08:58:31.000000 object_info-0.2.3/object_info.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2024-03-18 08:58:31.000000 object_info-0.2.3/object_info.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-18 08:58:31.000000 object_info-0.2.3/object_info.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-03-18 08:58:31.000000 object_info-0.2.3/object_info.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-18 08:58:31.860908 object_info-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 object_info-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 12:14:50.608662 object_info-0.2.4/
+-rw-rw-rw-   0        0        0     1082 2023-11-27 14:37:20.000000 object_info-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0    13531 2024-05-03 12:14:50.608409 object_info-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0    12576 2024-05-03 12:10:10.000000 object_info-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 12:14:50.599773 object_info-0.2.4/object_info/
+-rw-rw-rw-   0        0        0       21 2023-11-27 14:37:20.000000 object_info-0.2.4/object_info/__init__.py
+-rw-rw-rw-   0        0        0    17571 2024-05-03 12:08:45.000000 object_info-0.2.4/object_info/main.py
+drwxrwxrwx   0        0        0        0 2024-05-03 12:14:50.606792 object_info-0.2.4/object_info.egg-info/
+-rw-rw-rw-   0        0        0    13531 2024-05-03 12:14:50.000000 object_info-0.2.4/object_info.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2024-05-03 12:14:50.000000 object_info-0.2.4/object_info.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 12:14:50.000000 object_info-0.2.4/object_info.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-03 12:14:50.000000 object_info-0.2.4/object_info.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 12:14:50.610176 object_info-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 object_info-0.2.4/setup.py
```

### Comparing `object_info-0.2.3/LICENSE` & `object_info-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `object_info-0.2.3/PKG-INFO` & `object_info-0.2.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: object_info
-Version: 0.2.3
+Version: 0.2.4
 Summary: print info about object (attributes+properties+methods results)
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/object_info
 Keywords: object info,object attributes,object properties,object methods,print attributes,print properties,print methods
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# object_info (v0.2.3)
+# object_info (v0.2.4)
 
 ## DESCRIPTION_SHORT
 print info about object (attributes+properties+methods results)
 
 ## DESCRIPTION_LONG
 Designed to print info about object (properties+methods results)  
 
@@ -115,202 +115,200 @@
     log_iter=True,
     names__use_only_parts=[],
     names__skip_full=["attrSkipFullName", ],
     names__skip_parts=["SkipPartName", ],
     hide_build_in=None,
 ).print()
 """
-====================================================================================================
+==========================================================================================
 ----------OBJECTINFO.PRINT--------------------------------------------------------------------------
-str(SOURCE)=<__main__.Cls1 object at 0x0000011EFDE34A90>
-repr(SOURCE)=<__main__.Cls1 object at 0x0000011EFDE34A90>
+str(SOURCE)=<__main__.Cls1 object at 0x000001A014B97950>
+repr(SOURCE)=<__main__.Cls1 object at 0x000001A014B97950>
 ----------SETTINGS----------------------------------------------------------------------------------
 self.NAMES__USE_ONLY_PARTS=[]
-self.NAMES__SKIP_FULL=['checkout', 'detach', 'run', 'start', 'wait', 'join', 'terminate', 'quit', 'disconnect', 'exec', 'exec_', 'pyqtConfigure', 'pop', 'popleft', 'append', 'appendleft', 'extend', 'extendleft', 'add', 'insert', 'reverse', 'rotate', 'sort', 'attrSkipFullName', 'attrSkipFullName']
-self.NAMES__SKIP_PARTS=['init', 'new', 'create', 'enter', 'install', 'set', 'clone', 'copy', 'move', 'next', 'clear', 'reduce', 'close', 'del', 'exit', 'kill', 'SkipPartName', 'SkipPartName']
+self.NAMES__SKIP_FULL=['attrSkipFullName']
+self.NAMES__SKIP_PARTS=['init', 'new', 'create', 'enter', 'install', 'set', 'clone', 'copy', 'move', 'next', 'clear', 'reduce', 'close', 'del', 'exit', 'kill', 'exec', 'exec_', 'pyqtConfigure', 'checkout', 'detach', 'run', 'start', 'wait', 'join', 'terminate', 'quit', 'disconnect', 'pop', 'popleft', 'append', 'appendleft', 'extend', 'extendleft', 'add', 'insert', 'reverse', 'rotate', 'sort', 'SkipPartName']
 self.HIDE_BUILD_IN=None
 self.LOG_ITER=True
 self.MAX_LINE_LEN=100
 self.MAX_ITER_ITEMS=5
 ----------log_iter(wait last touched)---------------------------------------------------------------
-1:		ATTR_UPPERCASE
-2:		__class__
-3:		__delattr__
-4:		__dict__
-5:		__dir__
-6:		__doc__
-7:		__eq__
-8:		__format__
-9:		__ge__
-10:		__getattribute__
-11:		__getstate__
-12:		__gt__
-13:		__hash__
-14:		__init__
-15:		__init_subclass__
-16:		__le__
-17:		__lt__
-18:		__module__
-19:		__ne__
-20:		__new__
-21:		__reduce__
-22:		__reduce_ex__
-23:		__repr__
-24:		__setattr__
-25:		__sizeof__
-26:		__slotnames__
-27:		__str__
-28:		__subclasshook__
-29:		__weakref__
-30:		attrClass
-31:		attrDict
-32:		attrFloat
-33:		attrInt
-34:		attrList
-35:		attrListObj
-36:		attrNone
-37:		attrObj
-38:		attrSet
-39:		attrSkipFullName
-40:		attrSkipPartName
-41:		attrTuple
-42:		methExx
-43:		methInt
-44:		propertyExx
-45:		propertyInt
+1:	ATTR_UPPERCASE
+2:	__class__
+3:	__delattr__
+4:	__dict__
+5:	__dir__
+6:	__doc__
+7:	__eq__
+8:	__format__
+9:	__ge__
+10:	__getattribute__
+11:	__getstate__
+12:	__gt__
+13:	__hash__
+14:	__init__
+15:	__init_subclass__
+16:	__le__
+17:	__lt__
+18:	__module__
+19:	__ne__
+20:	__new__
+21:	__reduce__
+22:	__reduce_ex__
+23:	__repr__
+24:	__setattr__
+25:	__sizeof__
+26:	__str__
+27:	__subclasshook__
+28:	__weakref__
+29:	attrClass
+30:	attrDict
+31:	attrFloat
+32:	attrInt
+33:	attrList
+34:	attrListObj
+35:	attrNone
+36:	attrObj
+37:	attrSet
+38:	attrSkipFullName
+39:	attrSkipPartName
+40:	attrTuple
+41:	methExx
+42:	methInt
+43:	propertyExx
+44:	propertyInt
 ----------SKIPPED_FULLNAMES-------------------------------------------------------------------------
-1:		attrSkipFullName
+1:	attrSkipFullName
 ----------SKIPPED_PARTNAMES-------------------------------------------------------------------------
-1:		__delattr__
-2:		__init__
-3:		__init_subclass__
-4:		__new__
-5:		__reduce__
-6:		__reduce_ex__
-7:		__setattr__
-8:		attrSkipPartName
+1:	__delattr__
+2:	__init__
+3:	__init_subclass__
+4:	__new__
+5:	__reduce__
+6:	__reduce_ex__
+7:	__setattr__
+8:	attrSkipPartName
 ----------PROPERTIES__ELEMENTARY_SINGLE-------------------------------------------------------------
 ATTR_UPPERCASE      	str         :UPPERCASE
 __doc__             	NoneType    :None
 __module__          	str         :__main__
 __weakref__         	NoneType    :None
 attrFloat           	float       :2.2
 attrInt             	int         :1
 attrNone            	NoneType    :None
 propertyInt         	int         :1
 ----------PROPERTIES__ELEMENTARY_COLLECTION---------------------------------------------------------
 __dict__            	dict        :{}
-__slotnames__       	list        :[]
 attrDict            	dict        :{1: 1}
 attrList            	list        :[1, 2, 3]
-attrListObj         	list        :[<__main__.Cls0 object at 0x0000011EFDFB70D0>, <__main__.Cls0 o...
-                    	Cls0        :	<__main__.Cls0 object at 0x0000011EFDFB70D0>
-                    	Cls0        :	<__main__.Cls0 object at 0x0000011EFDFB70D0>
-                    	Cls0        :	<__main__.Cls0 object at 0x0000011EFDFB70D0>
-                    	Cls0        :	<__main__.Cls0 object at 0x0000011EFDFB70D0>
-                    	Cls0        :	<__main__.Cls0 object at 0x0000011EFDFB70D0>
+attrListObj         	list        :[<__main__.Cls0 object at 0x000001A014B96E10>, <__main__.Cls0 o...
+                    	Cls0        :	<__main__.Cls0 object at 0x000001A014B96E10>
+                    	Cls0        :	<__main__.Cls0 object at 0x000001A014B96E10>
+                    	Cls0        :	<__main__.Cls0 object at 0x000001A014B96E10>
+                    	Cls0        :	<__main__.Cls0 object at 0x000001A014B96E10>
+                    	Cls0        :	<__main__.Cls0 object at 0x000001A014B96E10>
                     	            :	...
 attrSet             	set         :{1, 2, 3}
 attrTuple           	tuple       :(1, 2, 3)
 ----------PROPERTIES__OBJECTS-----------------------------------------------------------------------
-attrObj             	Cls0        :<__main__.Cls0 object at 0x0000011EFDFB7050>
-                    	__repr()    :<__main__.Cls0 object at 0x0000011EFDFB7050>
+attrObj             	Cls0        :<__main__.Cls0 object at 0x000001A014B978D0>
+                    	__repr()    :<__main__.Cls0 object at 0x000001A014B978D0>
 ----------PROPERTIES__EXX---------------------------------------------------------------------------
 propertyExx         	Exception   :Exception('exxMsg')
 ----------METHODS__ELEMENTARY_SINGLE----------------------------------------------------------------
 __getstate__        	NoneType    :None
-__hash__            	int         :77038761129
-__repr__            	str         :<__main__.Cls1 object at 0x0000011EFDE34A90>
+__hash__            	int         :111690880917
+__repr__            	str         :<__main__.Cls1 object at 0x000001A014B97950>
 __sizeof__          	int         :24
-__str__             	str         :<__main__.Cls1 object at 0x0000011EFDE34A90>
+__str__             	str         :<__main__.Cls1 object at 0x000001A014B97950>
 methInt             	int         :1
 ----------METHODS__ELEMENTARY_COLLECTION------------------------------------------------------------
 __dir__             	list        :['__module__', 'ATTR_UPPERCASE', 'attrSkipFullName', 'attrSkipP...
                     	str         :	__module__
                     	str         :	ATTR_UPPERCASE
                     	str         :	attrSkipFullName
                     	str         :	attrSkipPartName
                     	str         :	attrNone
                     	            :	...
 ----------METHODS__OBJECTS--------------------------------------------------------------------------
-__class__           	Cls1        :<__main__.Cls1 object at 0x0000011EFE5CD490>
-                    	__repr()    :<__main__.Cls1 object at 0x0000011EFE5CD490>
+__class__           	Cls1        :<__main__.Cls1 object at 0x000001A014B97C10>
+                    	__repr()    :<__main__.Cls1 object at 0x000001A014B97C10>
 __subclasshook__    	NotImplementedType:NotImplemented
                     	__repr()    :NotImplemented
-attrClass           	Cls0        :<__main__.Cls0 object at 0x0000011EFE5CD790>
-                    	__repr()    :<__main__.Cls0 object at 0x0000011EFE5CD790>
+attrClass           	Cls0        :<__main__.Cls0 object at 0x000001A0151A9150>
+                    	__repr()    :<__main__.Cls0 object at 0x000001A0151A9150>
 ----------METHODS__EXX------------------------------------------------------------------------------
 __eq__              	TypeError   :TypeError('expected 1 argument, got 0')
 __format__          	TypeError   :TypeError('Cls1.__format__() takes exactly one argument (0 give...
 __ge__              	TypeError   :TypeError('expected 1 argument, got 0')
 __getattribute__    	TypeError   :TypeError('expected 1 argument, got 0')
 __gt__              	TypeError   :TypeError('expected 1 argument, got 0')
 __le__              	TypeError   :TypeError('expected 1 argument, got 0')
 __lt__              	TypeError   :TypeError('expected 1 argument, got 0')
 __ne__              	TypeError   :TypeError('expected 1 argument, got 0')
 methExx             	Exception   :Exception('exxMsg')
-====================================================================================================
+==========================================================================================
 """
 
 ObjectInfo(
     Cls1(),
     log_iter=False,
     names__use_only_parts="attr",
     # names__skip_full=["attrSkipFullName", ],
     # names__skip_parts=["SkipPartName", ],
     # hide_build_in=None,
     # max_line_len=0,
     # max_iter_items=0,
 ).print()
 """
-====================================================================================================
+==========================================================================================
 ----------OBJECTINFO.PRINT--------------------------------------------------------------------------
-str(SOURCE)=<__main__.Cls1 object at 0x0000011EFE5CD910>
-repr(SOURCE)=<__main__.Cls1 object at 0x0000011EFE5CD910>
+str(SOURCE)=<__main__.Cls1 object at 0x000001A014BE28D0>
+repr(SOURCE)=<__main__.Cls1 object at 0x000001A014BE28D0>
 ----------SETTINGS----------------------------------------------------------------------------------
 self.NAMES__USE_ONLY_PARTS=['attr']
-self.NAMES__SKIP_FULL=['checkout', 'detach', 'run', 'start', 'wait', 'join', 'terminate', 'quit', 'disconnect', 'exec', 'exec_', 'pyqtConfigure', 'pop', 'popleft', 'append', 'appendleft', 'extend', 'extendleft', 'add', 'insert', 'reverse', 'rotate', 'sort', 'attrSkipFullName', 'attrSkipFullName']
-self.NAMES__SKIP_PARTS=['init', 'new', 'create', 'enter', 'install', 'set', 'clone', 'copy', 'move', 'next', 'clear', 'reduce', 'close', 'del', 'exit', 'kill', 'SkipPartName', 'SkipPartName']
+self.NAMES__SKIP_FULL=['attrSkipFullName']
+self.NAMES__SKIP_PARTS=['init', 'new', 'create', 'enter', 'install', 'set', 'clone', 'copy', 'move', 'next', 'clear', 'reduce', 'close', 'del', 'exit', 'kill', 'exec', 'exec_', 'pyqtConfigure', 'checkout', 'detach', 'run', 'start', 'wait', 'join', 'terminate', 'quit', 'disconnect', 'pop', 'popleft', 'append', 'appendleft', 'extend', 'extendleft', 'add', 'insert', 'reverse', 'rotate', 'sort', 'SkipPartName']
 self.HIDE_BUILD_IN=None
 self.LOG_ITER=False
 self.MAX_LINE_LEN=100
 self.MAX_ITER_ITEMS=5
 ----------log_iter(wait last touched)---------------------------------------------------------------
 ----------SKIPPED_FULLNAMES-------------------------------------------------------------------------
-1:		attrSkipFullName
+1:	attrSkipFullName
 ----------SKIPPED_PARTNAMES-------------------------------------------------------------------------
-1:		__delattr__
-2:		__setattr__
-3:		attrSkipPartName
+1:	__delattr__
+2:	__setattr__
+3:	attrSkipPartName
 ----------PROPERTIES__ELEMENTARY_SINGLE-------------------------------------------------------------
 ATTR_UPPERCASE      	str         :UPPERCASE
 attrFloat           	float       :2.2
 attrInt             	int         :1
 attrNone            	NoneType    :None
 ----------PROPERTIES__ELEMENTARY_COLLECTION---------------------------------------------------------
 attrDict            	dict        :{1: 1}
 attrList            	list        :[1, 2, 3]
-attrListObj         	list        :[<__main__.Cls0 object at 0x0000011EFDFB70D0>, <__main__.Cls0 o...
-                    	Cls0        :	<__main__.Cls0 object at 0x0000011EFDFB70D0>
-                    	Cls0        :	<__main__.Cls0 object at 0x0000011EFDFB70D0>
-                    	Cls0        :	<__main__.Cls0 object at 0x0000011EFDFB70D0>
-                    	Cls0        :	<__main__.Cls0 object at 0x0000011EFDFB70D0>
-                    	Cls0        :	<__main__.Cls0 object at 0x0000011EFDFB70D0>
+attrListObj         	list        :[<__main__.Cls0 object at 0x000001A014B96E10>, <__main__.Cls0 o...
+                    	Cls0        :	<__main__.Cls0 object at 0x000001A014B96E10>
+                    	Cls0        :	<__main__.Cls0 object at 0x000001A014B96E10>
+                    	Cls0        :	<__main__.Cls0 object at 0x000001A014B96E10>
+                    	Cls0        :	<__main__.Cls0 object at 0x000001A014B96E10>
+                    	Cls0        :	<__main__.Cls0 object at 0x000001A014B96E10>
                     	            :	...
 attrSet             	set         :{1, 2, 3}
 attrTuple           	tuple       :(1, 2, 3)
 ----------PROPERTIES__OBJECTS-----------------------------------------------------------------------
-attrObj             	Cls0        :<__main__.Cls0 object at 0x0000011EFDFB7050>
-                    	__repr()    :<__main__.Cls0 object at 0x0000011EFDFB7050>
+attrObj             	Cls0        :<__main__.Cls0 object at 0x000001A014B978D0>
+                    	__repr()    :<__main__.Cls0 object at 0x000001A014B978D0>
 ----------PROPERTIES__EXX---------------------------------------------------------------------------
 ----------METHODS__ELEMENTARY_SINGLE----------------------------------------------------------------
 ----------METHODS__ELEMENTARY_COLLECTION------------------------------------------------------------
 ----------METHODS__OBJECTS--------------------------------------------------------------------------
-attrClass           	Cls0        :<__main__.Cls0 object at 0x0000011EFE5CDE50>
-                    	__repr()    :<__main__.Cls0 object at 0x0000011EFE5CDE50>
+attrClass           	Cls0        :<__main__.Cls0 object at 0x000001A0151A9C90>
+                    	__repr()    :<__main__.Cls0 object at 0x000001A0151A9C90>
 ----------METHODS__EXX------------------------------------------------------------------------------
 __getattribute__    	TypeError   :TypeError('expected 1 argument, got 0')
-====================================================================================================
+==========================================================================================
 """
 ```
 
 ********************************************************************************
```

### Comparing `object_info-0.2.3/README.md` & `object_info-0.2.4/object_info.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,30 @@
-# object_info (v0.2.3)
+Metadata-Version: 2.1
+Name: object_info
+Version: 0.2.4
+Summary: print info about object (attributes+properties+methods results)
+Home-page: https://github.com/centroid457/
+Author: Andrei Starichenko
+Author-email: centroid@mail.ru
+Project-URL: Source, https://github.com/centroid457/object_info
+Keywords: object info,object attributes,object properties,object methods,print attributes,print properties,print methods
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Typing :: Typed
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# object_info (v0.2.4)
 
 ## DESCRIPTION_SHORT
 print info about object (attributes+properties+methods results)
 
 ## DESCRIPTION_LONG
 Designed to print info about object (properties+methods results)  
 
@@ -93,202 +115,200 @@
     log_iter=True,
     names__use_only_parts=[],
     names__skip_full=["attrSkipFullName", ],
     names__skip_parts=["SkipPartName", ],
     hide_build_in=None,
 ).print()
 """
-====================================================================================================
+==========================================================================================
 ----------OBJECTINFO.PRINT--------------------------------------------------------------------------
-str(SOURCE)=<__main__.Cls1 object at 0x0000011EFDE34A90>
-repr(SOURCE)=<__main__.Cls1 object at 0x0000011EFDE34A90>
+str(SOURCE)=<__main__.Cls1 object at 0x000001A014B97950>
+repr(SOURCE)=<__main__.Cls1 object at 0x000001A014B97950>
 ----------SETTINGS----------------------------------------------------------------------------------
 self.NAMES__USE_ONLY_PARTS=[]
-self.NAMES__SKIP_FULL=['checkout', 'detach', 'run', 'start', 'wait', 'join', 'terminate', 'quit', 'disconnect', 'exec', 'exec_', 'pyqtConfigure', 'pop', 'popleft', 'append', 'appendleft', 'extend', 'extendleft', 'add', 'insert', 'reverse', 'rotate', 'sort', 'attrSkipFullName', 'attrSkipFullName']
-self.NAMES__SKIP_PARTS=['init', 'new', 'create', 'enter', 'install', 'set', 'clone', 'copy', 'move', 'next', 'clear', 'reduce', 'close', 'del', 'exit', 'kill', 'SkipPartName', 'SkipPartName']
+self.NAMES__SKIP_FULL=['attrSkipFullName']
+self.NAMES__SKIP_PARTS=['init', 'new', 'create', 'enter', 'install', 'set', 'clone', 'copy', 'move', 'next', 'clear', 'reduce', 'close', 'del', 'exit', 'kill', 'exec', 'exec_', 'pyqtConfigure', 'checkout', 'detach', 'run', 'start', 'wait', 'join', 'terminate', 'quit', 'disconnect', 'pop', 'popleft', 'append', 'appendleft', 'extend', 'extendleft', 'add', 'insert', 'reverse', 'rotate', 'sort', 'SkipPartName']
 self.HIDE_BUILD_IN=None
 self.LOG_ITER=True
 self.MAX_LINE_LEN=100
 self.MAX_ITER_ITEMS=5
 ----------log_iter(wait last touched)---------------------------------------------------------------
-1:		ATTR_UPPERCASE
-2:		__class__
-3:		__delattr__
-4:		__dict__
-5:		__dir__
-6:		__doc__
-7:		__eq__
-8:		__format__
-9:		__ge__
-10:		__getattribute__
-11:		__getstate__
-12:		__gt__
-13:		__hash__
-14:		__init__
-15:		__init_subclass__
-16:		__le__
-17:		__lt__
-18:		__module__
-19:		__ne__
-20:		__new__
-21:		__reduce__
-22:		__reduce_ex__
-23:		__repr__
-24:		__setattr__
-25:		__sizeof__
-26:		__slotnames__
-27:		__str__
-28:		__subclasshook__
-29:		__weakref__
-30:		attrClass
-31:		attrDict
-32:		attrFloat
-33:		attrInt
-34:		attrList
-35:		attrListObj
-36:		attrNone
-37:		attrObj
-38:		attrSet
-39:		attrSkipFullName
-40:		attrSkipPartName
-41:		attrTuple
-42:		methExx
-43:		methInt
-44:		propertyExx
-45:		propertyInt
+1:	ATTR_UPPERCASE
+2:	__class__
+3:	__delattr__
+4:	__dict__
+5:	__dir__
+6:	__doc__
+7:	__eq__
+8:	__format__
+9:	__ge__
+10:	__getattribute__
+11:	__getstate__
+12:	__gt__
+13:	__hash__
+14:	__init__
+15:	__init_subclass__
+16:	__le__
+17:	__lt__
+18:	__module__
+19:	__ne__
+20:	__new__
+21:	__reduce__
+22:	__reduce_ex__
+23:	__repr__
+24:	__setattr__
+25:	__sizeof__
+26:	__str__
+27:	__subclasshook__
+28:	__weakref__
+29:	attrClass
+30:	attrDict
+31:	attrFloat
+32:	attrInt
+33:	attrList
+34:	attrListObj
+35:	attrNone
+36:	attrObj
+37:	attrSet
+38:	attrSkipFullName
+39:	attrSkipPartName
+40:	attrTuple
+41:	methExx
+42:	methInt
+43:	propertyExx
+44:	propertyInt
 ----------SKIPPED_FULLNAMES-------------------------------------------------------------------------
-1:		attrSkipFullName
+1:	attrSkipFullName
 ----------SKIPPED_PARTNAMES-------------------------------------------------------------------------
-1:		__delattr__
-2:		__init__
-3:		__init_subclass__
-4:		__new__
-5:		__reduce__
-6:		__reduce_ex__
-7:		__setattr__
-8:		attrSkipPartName
+1:	__delattr__
+2:	__init__
+3:	__init_subclass__
+4:	__new__
+5:	__reduce__
+6:	__reduce_ex__
+7:	__setattr__
+8:	attrSkipPartName
 ----------PROPERTIES__ELEMENTARY_SINGLE-------------------------------------------------------------
 ATTR_UPPERCASE      	str         :UPPERCASE
 __doc__             	NoneType    :None
 __module__          	str         :__main__
 __weakref__         	NoneType    :None
 attrFloat           	float       :2.2
 attrInt             	int         :1
 attrNone            	NoneType    :None
 propertyInt         	int         :1
 ----------PROPERTIES__ELEMENTARY_COLLECTION---------------------------------------------------------
 __dict__            	dict        :{}
-__slotnames__       	list        :[]
 attrDict            	dict        :{1: 1}
 attrList            	list        :[1, 2, 3]
-attrListObj         	list        :[<__main__.Cls0 object at 0x0000011EFDFB70D0>, <__main__.Cls0 o...
-                    	Cls0        :	<__main__.Cls0 object at 0x0000011EFDFB70D0>
-                    	Cls0        :	<__main__.Cls0 object at 0x0000011EFDFB70D0>
-                    	Cls0        :	<__main__.Cls0 object at 0x0000011EFDFB70D0>
-                    	Cls0        :	<__main__.Cls0 object at 0x0000011EFDFB70D0>
-                    	Cls0        :	<__main__.Cls0 object at 0x0000011EFDFB70D0>
+attrListObj         	list        :[<__main__.Cls0 object at 0x000001A014B96E10>, <__main__.Cls0 o...
+                    	Cls0        :	<__main__.Cls0 object at 0x000001A014B96E10>
+                    	Cls0        :	<__main__.Cls0 object at 0x000001A014B96E10>
+                    	Cls0        :	<__main__.Cls0 object at 0x000001A014B96E10>
+                    	Cls0        :	<__main__.Cls0 object at 0x000001A014B96E10>
+                    	Cls0        :	<__main__.Cls0 object at 0x000001A014B96E10>
                     	            :	...
 attrSet             	set         :{1, 2, 3}
 attrTuple           	tuple       :(1, 2, 3)
 ----------PROPERTIES__OBJECTS-----------------------------------------------------------------------
-attrObj             	Cls0        :<__main__.Cls0 object at 0x0000011EFDFB7050>
-                    	__repr()    :<__main__.Cls0 object at 0x0000011EFDFB7050>
+attrObj             	Cls0        :<__main__.Cls0 object at 0x000001A014B978D0>
+                    	__repr()    :<__main__.Cls0 object at 0x000001A014B978D0>
 ----------PROPERTIES__EXX---------------------------------------------------------------------------
 propertyExx         	Exception   :Exception('exxMsg')
 ----------METHODS__ELEMENTARY_SINGLE----------------------------------------------------------------
 __getstate__        	NoneType    :None
-__hash__            	int         :77038761129
-__repr__            	str         :<__main__.Cls1 object at 0x0000011EFDE34A90>
+__hash__            	int         :111690880917
+__repr__            	str         :<__main__.Cls1 object at 0x000001A014B97950>
 __sizeof__          	int         :24
-__str__             	str         :<__main__.Cls1 object at 0x0000011EFDE34A90>
+__str__             	str         :<__main__.Cls1 object at 0x000001A014B97950>
 methInt             	int         :1
 ----------METHODS__ELEMENTARY_COLLECTION------------------------------------------------------------
 __dir__             	list        :['__module__', 'ATTR_UPPERCASE', 'attrSkipFullName', 'attrSkipP...
                     	str         :	__module__
                     	str         :	ATTR_UPPERCASE
                     	str         :	attrSkipFullName
                     	str         :	attrSkipPartName
                     	str         :	attrNone
                     	            :	...
 ----------METHODS__OBJECTS--------------------------------------------------------------------------
-__class__           	Cls1        :<__main__.Cls1 object at 0x0000011EFE5CD490>
-                    	__repr()    :<__main__.Cls1 object at 0x0000011EFE5CD490>
+__class__           	Cls1        :<__main__.Cls1 object at 0x000001A014B97C10>
+                    	__repr()    :<__main__.Cls1 object at 0x000001A014B97C10>
 __subclasshook__    	NotImplementedType:NotImplemented
                     	__repr()    :NotImplemented
-attrClass           	Cls0        :<__main__.Cls0 object at 0x0000011EFE5CD790>
-                    	__repr()    :<__main__.Cls0 object at 0x0000011EFE5CD790>
+attrClass           	Cls0        :<__main__.Cls0 object at 0x000001A0151A9150>
+                    	__repr()    :<__main__.Cls0 object at 0x000001A0151A9150>
 ----------METHODS__EXX------------------------------------------------------------------------------
 __eq__              	TypeError   :TypeError('expected 1 argument, got 0')
 __format__          	TypeError   :TypeError('Cls1.__format__() takes exactly one argument (0 give...
 __ge__              	TypeError   :TypeError('expected 1 argument, got 0')
 __getattribute__    	TypeError   :TypeError('expected 1 argument, got 0')
 __gt__              	TypeError   :TypeError('expected 1 argument, got 0')
 __le__              	TypeError   :TypeError('expected 1 argument, got 0')
 __lt__              	TypeError   :TypeError('expected 1 argument, got 0')
 __ne__              	TypeError   :TypeError('expected 1 argument, got 0')
 methExx             	Exception   :Exception('exxMsg')
-====================================================================================================
+==========================================================================================
 """
 
 ObjectInfo(
     Cls1(),
     log_iter=False,
     names__use_only_parts="attr",
     # names__skip_full=["attrSkipFullName", ],
     # names__skip_parts=["SkipPartName", ],
     # hide_build_in=None,
     # max_line_len=0,
     # max_iter_items=0,
 ).print()
 """
-====================================================================================================
+==========================================================================================
 ----------OBJECTINFO.PRINT--------------------------------------------------------------------------
-str(SOURCE)=<__main__.Cls1 object at 0x0000011EFE5CD910>
-repr(SOURCE)=<__main__.Cls1 object at 0x0000011EFE5CD910>
+str(SOURCE)=<__main__.Cls1 object at 0x000001A014BE28D0>
+repr(SOURCE)=<__main__.Cls1 object at 0x000001A014BE28D0>
 ----------SETTINGS----------------------------------------------------------------------------------
 self.NAMES__USE_ONLY_PARTS=['attr']
-self.NAMES__SKIP_FULL=['checkout', 'detach', 'run', 'start', 'wait', 'join', 'terminate', 'quit', 'disconnect', 'exec', 'exec_', 'pyqtConfigure', 'pop', 'popleft', 'append', 'appendleft', 'extend', 'extendleft', 'add', 'insert', 'reverse', 'rotate', 'sort', 'attrSkipFullName', 'attrSkipFullName']
-self.NAMES__SKIP_PARTS=['init', 'new', 'create', 'enter', 'install', 'set', 'clone', 'copy', 'move', 'next', 'clear', 'reduce', 'close', 'del', 'exit', 'kill', 'SkipPartName', 'SkipPartName']
+self.NAMES__SKIP_FULL=['attrSkipFullName']
+self.NAMES__SKIP_PARTS=['init', 'new', 'create', 'enter', 'install', 'set', 'clone', 'copy', 'move', 'next', 'clear', 'reduce', 'close', 'del', 'exit', 'kill', 'exec', 'exec_', 'pyqtConfigure', 'checkout', 'detach', 'run', 'start', 'wait', 'join', 'terminate', 'quit', 'disconnect', 'pop', 'popleft', 'append', 'appendleft', 'extend', 'extendleft', 'add', 'insert', 'reverse', 'rotate', 'sort', 'SkipPartName']
 self.HIDE_BUILD_IN=None
 self.LOG_ITER=False
 self.MAX_LINE_LEN=100
 self.MAX_ITER_ITEMS=5
 ----------log_iter(wait last touched)---------------------------------------------------------------
 ----------SKIPPED_FULLNAMES-------------------------------------------------------------------------
-1:		attrSkipFullName
+1:	attrSkipFullName
 ----------SKIPPED_PARTNAMES-------------------------------------------------------------------------
-1:		__delattr__
-2:		__setattr__
-3:		attrSkipPartName
+1:	__delattr__
+2:	__setattr__
+3:	attrSkipPartName
 ----------PROPERTIES__ELEMENTARY_SINGLE-------------------------------------------------------------
 ATTR_UPPERCASE      	str         :UPPERCASE
 attrFloat           	float       :2.2
 attrInt             	int         :1
 attrNone            	NoneType    :None
 ----------PROPERTIES__ELEMENTARY_COLLECTION---------------------------------------------------------
 attrDict            	dict        :{1: 1}
 attrList            	list        :[1, 2, 3]
-attrListObj         	list        :[<__main__.Cls0 object at 0x0000011EFDFB70D0>, <__main__.Cls0 o...
-                    	Cls0        :	<__main__.Cls0 object at 0x0000011EFDFB70D0>
-                    	Cls0        :	<__main__.Cls0 object at 0x0000011EFDFB70D0>
-                    	Cls0        :	<__main__.Cls0 object at 0x0000011EFDFB70D0>
-                    	Cls0        :	<__main__.Cls0 object at 0x0000011EFDFB70D0>
-                    	Cls0        :	<__main__.Cls0 object at 0x0000011EFDFB70D0>
+attrListObj         	list        :[<__main__.Cls0 object at 0x000001A014B96E10>, <__main__.Cls0 o...
+                    	Cls0        :	<__main__.Cls0 object at 0x000001A014B96E10>
+                    	Cls0        :	<__main__.Cls0 object at 0x000001A014B96E10>
+                    	Cls0        :	<__main__.Cls0 object at 0x000001A014B96E10>
+                    	Cls0        :	<__main__.Cls0 object at 0x000001A014B96E10>
+                    	Cls0        :	<__main__.Cls0 object at 0x000001A014B96E10>
                     	            :	...
 attrSet             	set         :{1, 2, 3}
 attrTuple           	tuple       :(1, 2, 3)
 ----------PROPERTIES__OBJECTS-----------------------------------------------------------------------
-attrObj             	Cls0        :<__main__.Cls0 object at 0x0000011EFDFB7050>
-                    	__repr()    :<__main__.Cls0 object at 0x0000011EFDFB7050>
+attrObj             	Cls0        :<__main__.Cls0 object at 0x000001A014B978D0>
+                    	__repr()    :<__main__.Cls0 object at 0x000001A014B978D0>
 ----------PROPERTIES__EXX---------------------------------------------------------------------------
 ----------METHODS__ELEMENTARY_SINGLE----------------------------------------------------------------
 ----------METHODS__ELEMENTARY_COLLECTION------------------------------------------------------------
 ----------METHODS__OBJECTS--------------------------------------------------------------------------
-attrClass           	Cls0        :<__main__.Cls0 object at 0x0000011EFE5CDE50>
-                    	__repr()    :<__main__.Cls0 object at 0x0000011EFE5CDE50>
+attrClass           	Cls0        :<__main__.Cls0 object at 0x000001A0151A9C90>
+                    	__repr()    :<__main__.Cls0 object at 0x000001A0151A9C90>
 ----------METHODS__EXX------------------------------------------------------------------------------
 __getattribute__    	TypeError   :TypeError('expected 1 argument, got 0')
-====================================================================================================
+==========================================================================================
 """
 ```
 
 ********************************************************************************
```

### Comparing `object_info-0.2.3/object_info/main.py` & `object_info-0.2.4/object_info/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -338,15 +338,15 @@
         elif TypeChecker.check__Exception(value):
             block_value = f"{value!r}"
 
         # -------------------------------
         result = f"{block_name:20}\t{block_type:12}:{_block_intend}{block_value}"
 
         if self.MAX_LINE_LEN and len(result) > self.MAX_LINE_LEN:
-            result = result[:self.MAX_LINE_LEN - 3] + "..."
+            result = result[:self.MAX_LINE_LEN - 3*2] + "..."
 
         # --------------------------------------------------------------------------------------
         print(result)
 
         # -------------------------------
         if name and TypeChecker.check__Object(value):
             # additional print for object
@@ -413,29 +413,30 @@
                     self._print_line__name_type_value(name=None, value=ItemInternal(item_key, item_value))
 
     # =================================================================================================================
     def print(self) -> None:
         """print all params from object
         if method - try to start it!
         """
-        print("="*100)
+        WRAPPER_MAIN_LINE = "="*min(90, self.MAX_LINE_LEN)  # here we need use less then
+
+        print(WRAPPER_MAIN_LINE)
         self._print_block__head()
         self._item_reload()
 
         for group_name, group_values in self.ITEM.__getstate__().items():
             self._print_line__group_separator(group_name)
 
             if TypeChecker.check__elementary_collection_not_dict(group_values):
                 for pos, name in enumerate(group_values, start=1):
                     print(f"{pos}:\t{name}")
             else:
                 for name, value in group_values.items():
                     self._print_block__name_value(name, value)
-
-        print("="*100)
+        print(WRAPPER_MAIN_LINE)
 
     # =================================================================================================================
     def print_diffs(self) -> None:
         pass
         # TODO: FINISH!
```

### Comparing `object_info-0.2.3/object_info.egg-info/PKG-INFO` & `object_info-0.2.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,8 @@
-Metadata-Version: 2.1
-Name: object_info
-Version: 0.2.3
-Summary: print info about object (attributes+properties+methods results)
-Home-page: https://github.com/centroid457/
-Author: Andrei Starichenko
-Author-email: centroid@mail.ru
-Project-URL: Source, https://github.com/centroid457/object_info
-Keywords: object info,object attributes,object properties,object methods,print attributes,print properties,print methods
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Typing :: Typed
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# object_info (v0.2.3)
+# object_info (v0.2.4)
 
 ## DESCRIPTION_SHORT
 print info about object (attributes+properties+methods results)
 
 ## DESCRIPTION_LONG
 Designed to print info about object (properties+methods results)  
 
@@ -115,202 +93,200 @@
     log_iter=True,
     names__use_only_parts=[],
     names__skip_full=["attrSkipFullName", ],
     names__skip_parts=["SkipPartName", ],
     hide_build_in=None,
 ).print()
 """
-====================================================================================================
+==========================================================================================
 ----------OBJECTINFO.PRINT--------------------------------------------------------------------------
-str(SOURCE)=<__main__.Cls1 object at 0x0000011EFDE34A90>
-repr(SOURCE)=<__main__.Cls1 object at 0x0000011EFDE34A90>
+str(SOURCE)=<__main__.Cls1 object at 0x000001A014B97950>
+repr(SOURCE)=<__main__.Cls1 object at 0x000001A014B97950>
 ----------SETTINGS----------------------------------------------------------------------------------
 self.NAMES__USE_ONLY_PARTS=[]
-self.NAMES__SKIP_FULL=['checkout', 'detach', 'run', 'start', 'wait', 'join', 'terminate', 'quit', 'disconnect', 'exec', 'exec_', 'pyqtConfigure', 'pop', 'popleft', 'append', 'appendleft', 'extend', 'extendleft', 'add', 'insert', 'reverse', 'rotate', 'sort', 'attrSkipFullName', 'attrSkipFullName']
-self.NAMES__SKIP_PARTS=['init', 'new', 'create', 'enter', 'install', 'set', 'clone', 'copy', 'move', 'next', 'clear', 'reduce', 'close', 'del', 'exit', 'kill', 'SkipPartName', 'SkipPartName']
+self.NAMES__SKIP_FULL=['attrSkipFullName']
+self.NAMES__SKIP_PARTS=['init', 'new', 'create', 'enter', 'install', 'set', 'clone', 'copy', 'move', 'next', 'clear', 'reduce', 'close', 'del', 'exit', 'kill', 'exec', 'exec_', 'pyqtConfigure', 'checkout', 'detach', 'run', 'start', 'wait', 'join', 'terminate', 'quit', 'disconnect', 'pop', 'popleft', 'append', 'appendleft', 'extend', 'extendleft', 'add', 'insert', 'reverse', 'rotate', 'sort', 'SkipPartName']
 self.HIDE_BUILD_IN=None
 self.LOG_ITER=True
 self.MAX_LINE_LEN=100
 self.MAX_ITER_ITEMS=5
 ----------log_iter(wait last touched)---------------------------------------------------------------
-1:		ATTR_UPPERCASE
-2:		__class__
-3:		__delattr__
-4:		__dict__
-5:		__dir__
-6:		__doc__
-7:		__eq__
-8:		__format__
-9:		__ge__
-10:		__getattribute__
-11:		__getstate__
-12:		__gt__
-13:		__hash__
-14:		__init__
-15:		__init_subclass__
-16:		__le__
-17:		__lt__
-18:		__module__
-19:		__ne__
-20:		__new__
-21:		__reduce__
-22:		__reduce_ex__
-23:		__repr__
-24:		__setattr__
-25:		__sizeof__
-26:		__slotnames__
-27:		__str__
-28:		__subclasshook__
-29:		__weakref__
-30:		attrClass
-31:		attrDict
-32:		attrFloat
-33:		attrInt
-34:		attrList
-35:		attrListObj
-36:		attrNone
-37:		attrObj
-38:		attrSet
-39:		attrSkipFullName
-40:		attrSkipPartName
-41:		attrTuple
-42:		methExx
-43:		methInt
-44:		propertyExx
-45:		propertyInt
+1:	ATTR_UPPERCASE
+2:	__class__
+3:	__delattr__
+4:	__dict__
+5:	__dir__
+6:	__doc__
+7:	__eq__
+8:	__format__
+9:	__ge__
+10:	__getattribute__
+11:	__getstate__
+12:	__gt__
+13:	__hash__
+14:	__init__
+15:	__init_subclass__
+16:	__le__
+17:	__lt__
+18:	__module__
+19:	__ne__
+20:	__new__
+21:	__reduce__
+22:	__reduce_ex__
+23:	__repr__
+24:	__setattr__
+25:	__sizeof__
+26:	__str__
+27:	__subclasshook__
+28:	__weakref__
+29:	attrClass
+30:	attrDict
+31:	attrFloat
+32:	attrInt
+33:	attrList
+34:	attrListObj
+35:	attrNone
+36:	attrObj
+37:	attrSet
+38:	attrSkipFullName
+39:	attrSkipPartName
+40:	attrTuple
+41:	methExx
+42:	methInt
+43:	propertyExx
+44:	propertyInt
 ----------SKIPPED_FULLNAMES-------------------------------------------------------------------------
-1:		attrSkipFullName
+1:	attrSkipFullName
 ----------SKIPPED_PARTNAMES-------------------------------------------------------------------------
-1:		__delattr__
-2:		__init__
-3:		__init_subclass__
-4:		__new__
-5:		__reduce__
-6:		__reduce_ex__
-7:		__setattr__
-8:		attrSkipPartName
+1:	__delattr__
+2:	__init__
+3:	__init_subclass__
+4:	__new__
+5:	__reduce__
+6:	__reduce_ex__
+7:	__setattr__
+8:	attrSkipPartName
 ----------PROPERTIES__ELEMENTARY_SINGLE-------------------------------------------------------------
 ATTR_UPPERCASE      	str         :UPPERCASE
 __doc__             	NoneType    :None
 __module__          	str         :__main__
 __weakref__         	NoneType    :None
 attrFloat           	float       :2.2
 attrInt             	int         :1
 attrNone            	NoneType    :None
 propertyInt         	int         :1
 ----------PROPERTIES__ELEMENTARY_COLLECTION---------------------------------------------------------
 __dict__            	dict        :{}
-__slotnames__       	list        :[]
 attrDict            	dict        :{1: 1}
 attrList            	list        :[1, 2, 3]
-attrListObj         	list        :[<__main__.Cls0 object at 0x0000011EFDFB70D0>, <__main__.Cls0 o...
-                    	Cls0        :	<__main__.Cls0 object at 0x0000011EFDFB70D0>
-                    	Cls0        :	<__main__.Cls0 object at 0x0000011EFDFB70D0>
-                    	Cls0        :	<__main__.Cls0 object at 0x0000011EFDFB70D0>
-                    	Cls0        :	<__main__.Cls0 object at 0x0000011EFDFB70D0>
-                    	Cls0        :	<__main__.Cls0 object at 0x0000011EFDFB70D0>
+attrListObj         	list        :[<__main__.Cls0 object at 0x000001A014B96E10>, <__main__.Cls0 o...
+                    	Cls0        :	<__main__.Cls0 object at 0x000001A014B96E10>
+                    	Cls0        :	<__main__.Cls0 object at 0x000001A014B96E10>
+                    	Cls0        :	<__main__.Cls0 object at 0x000001A014B96E10>
+                    	Cls0        :	<__main__.Cls0 object at 0x000001A014B96E10>
+                    	Cls0        :	<__main__.Cls0 object at 0x000001A014B96E10>
                     	            :	...
 attrSet             	set         :{1, 2, 3}
 attrTuple           	tuple       :(1, 2, 3)
 ----------PROPERTIES__OBJECTS-----------------------------------------------------------------------
-attrObj             	Cls0        :<__main__.Cls0 object at 0x0000011EFDFB7050>
-                    	__repr()    :<__main__.Cls0 object at 0x0000011EFDFB7050>
+attrObj             	Cls0        :<__main__.Cls0 object at 0x000001A014B978D0>
+                    	__repr()    :<__main__.Cls0 object at 0x000001A014B978D0>
 ----------PROPERTIES__EXX---------------------------------------------------------------------------
 propertyExx         	Exception   :Exception('exxMsg')
 ----------METHODS__ELEMENTARY_SINGLE----------------------------------------------------------------
 __getstate__        	NoneType    :None
-__hash__            	int         :77038761129
-__repr__            	str         :<__main__.Cls1 object at 0x0000011EFDE34A90>
+__hash__            	int         :111690880917
+__repr__            	str         :<__main__.Cls1 object at 0x000001A014B97950>
 __sizeof__          	int         :24
-__str__             	str         :<__main__.Cls1 object at 0x0000011EFDE34A90>
+__str__             	str         :<__main__.Cls1 object at 0x000001A014B97950>
 methInt             	int         :1
 ----------METHODS__ELEMENTARY_COLLECTION------------------------------------------------------------
 __dir__             	list        :['__module__', 'ATTR_UPPERCASE', 'attrSkipFullName', 'attrSkipP...
                     	str         :	__module__
                     	str         :	ATTR_UPPERCASE
                     	str         :	attrSkipFullName
                     	str         :	attrSkipPartName
                     	str         :	attrNone
                     	            :	...
 ----------METHODS__OBJECTS--------------------------------------------------------------------------
-__class__           	Cls1        :<__main__.Cls1 object at 0x0000011EFE5CD490>
-                    	__repr()    :<__main__.Cls1 object at 0x0000011EFE5CD490>
+__class__           	Cls1        :<__main__.Cls1 object at 0x000001A014B97C10>
+                    	__repr()    :<__main__.Cls1 object at 0x000001A014B97C10>
 __subclasshook__    	NotImplementedType:NotImplemented
                     	__repr()    :NotImplemented
-attrClass           	Cls0        :<__main__.Cls0 object at 0x0000011EFE5CD790>
-                    	__repr()    :<__main__.Cls0 object at 0x0000011EFE5CD790>
+attrClass           	Cls0        :<__main__.Cls0 object at 0x000001A0151A9150>
+                    	__repr()    :<__main__.Cls0 object at 0x000001A0151A9150>
 ----------METHODS__EXX------------------------------------------------------------------------------
 __eq__              	TypeError   :TypeError('expected 1 argument, got 0')
 __format__          	TypeError   :TypeError('Cls1.__format__() takes exactly one argument (0 give...
 __ge__              	TypeError   :TypeError('expected 1 argument, got 0')
 __getattribute__    	TypeError   :TypeError('expected 1 argument, got 0')
 __gt__              	TypeError   :TypeError('expected 1 argument, got 0')
 __le__              	TypeError   :TypeError('expected 1 argument, got 0')
 __lt__              	TypeError   :TypeError('expected 1 argument, got 0')
 __ne__              	TypeError   :TypeError('expected 1 argument, got 0')
 methExx             	Exception   :Exception('exxMsg')
-====================================================================================================
+==========================================================================================
 """
 
 ObjectInfo(
     Cls1(),
     log_iter=False,
     names__use_only_parts="attr",
     # names__skip_full=["attrSkipFullName", ],
     # names__skip_parts=["SkipPartName", ],
     # hide_build_in=None,
     # max_line_len=0,
     # max_iter_items=0,
 ).print()
 """
-====================================================================================================
+==========================================================================================
 ----------OBJECTINFO.PRINT--------------------------------------------------------------------------
-str(SOURCE)=<__main__.Cls1 object at 0x0000011EFE5CD910>
-repr(SOURCE)=<__main__.Cls1 object at 0x0000011EFE5CD910>
+str(SOURCE)=<__main__.Cls1 object at 0x000001A014BE28D0>
+repr(SOURCE)=<__main__.Cls1 object at 0x000001A014BE28D0>
 ----------SETTINGS----------------------------------------------------------------------------------
 self.NAMES__USE_ONLY_PARTS=['attr']
-self.NAMES__SKIP_FULL=['checkout', 'detach', 'run', 'start', 'wait', 'join', 'terminate', 'quit', 'disconnect', 'exec', 'exec_', 'pyqtConfigure', 'pop', 'popleft', 'append', 'appendleft', 'extend', 'extendleft', 'add', 'insert', 'reverse', 'rotate', 'sort', 'attrSkipFullName', 'attrSkipFullName']
-self.NAMES__SKIP_PARTS=['init', 'new', 'create', 'enter', 'install', 'set', 'clone', 'copy', 'move', 'next', 'clear', 'reduce', 'close', 'del', 'exit', 'kill', 'SkipPartName', 'SkipPartName']
+self.NAMES__SKIP_FULL=['attrSkipFullName']
+self.NAMES__SKIP_PARTS=['init', 'new', 'create', 'enter', 'install', 'set', 'clone', 'copy', 'move', 'next', 'clear', 'reduce', 'close', 'del', 'exit', 'kill', 'exec', 'exec_', 'pyqtConfigure', 'checkout', 'detach', 'run', 'start', 'wait', 'join', 'terminate', 'quit', 'disconnect', 'pop', 'popleft', 'append', 'appendleft', 'extend', 'extendleft', 'add', 'insert', 'reverse', 'rotate', 'sort', 'SkipPartName']
 self.HIDE_BUILD_IN=None
 self.LOG_ITER=False
 self.MAX_LINE_LEN=100
 self.MAX_ITER_ITEMS=5
 ----------log_iter(wait last touched)---------------------------------------------------------------
 ----------SKIPPED_FULLNAMES-------------------------------------------------------------------------
-1:		attrSkipFullName
+1:	attrSkipFullName
 ----------SKIPPED_PARTNAMES-------------------------------------------------------------------------
-1:		__delattr__
-2:		__setattr__
-3:		attrSkipPartName
+1:	__delattr__
+2:	__setattr__
+3:	attrSkipPartName
 ----------PROPERTIES__ELEMENTARY_SINGLE-------------------------------------------------------------
 ATTR_UPPERCASE      	str         :UPPERCASE
 attrFloat           	float       :2.2
 attrInt             	int         :1
 attrNone            	NoneType    :None
 ----------PROPERTIES__ELEMENTARY_COLLECTION---------------------------------------------------------
 attrDict            	dict        :{1: 1}
 attrList            	list        :[1, 2, 3]
-attrListObj         	list        :[<__main__.Cls0 object at 0x0000011EFDFB70D0>, <__main__.Cls0 o...
-                    	Cls0        :	<__main__.Cls0 object at 0x0000011EFDFB70D0>
-                    	Cls0        :	<__main__.Cls0 object at 0x0000011EFDFB70D0>
-                    	Cls0        :	<__main__.Cls0 object at 0x0000011EFDFB70D0>
-                    	Cls0        :	<__main__.Cls0 object at 0x0000011EFDFB70D0>
-                    	Cls0        :	<__main__.Cls0 object at 0x0000011EFDFB70D0>
+attrListObj         	list        :[<__main__.Cls0 object at 0x000001A014B96E10>, <__main__.Cls0 o...
+                    	Cls0        :	<__main__.Cls0 object at 0x000001A014B96E10>
+                    	Cls0        :	<__main__.Cls0 object at 0x000001A014B96E10>
+                    	Cls0        :	<__main__.Cls0 object at 0x000001A014B96E10>
+                    	Cls0        :	<__main__.Cls0 object at 0x000001A014B96E10>
+                    	Cls0        :	<__main__.Cls0 object at 0x000001A014B96E10>
                     	            :	...
 attrSet             	set         :{1, 2, 3}
 attrTuple           	tuple       :(1, 2, 3)
 ----------PROPERTIES__OBJECTS-----------------------------------------------------------------------
-attrObj             	Cls0        :<__main__.Cls0 object at 0x0000011EFDFB7050>
-                    	__repr()    :<__main__.Cls0 object at 0x0000011EFDFB7050>
+attrObj             	Cls0        :<__main__.Cls0 object at 0x000001A014B978D0>
+                    	__repr()    :<__main__.Cls0 object at 0x000001A014B978D0>
 ----------PROPERTIES__EXX---------------------------------------------------------------------------
 ----------METHODS__ELEMENTARY_SINGLE----------------------------------------------------------------
 ----------METHODS__ELEMENTARY_COLLECTION------------------------------------------------------------
 ----------METHODS__OBJECTS--------------------------------------------------------------------------
-attrClass           	Cls0        :<__main__.Cls0 object at 0x0000011EFE5CDE50>
-                    	__repr()    :<__main__.Cls0 object at 0x0000011EFE5CDE50>
+attrClass           	Cls0        :<__main__.Cls0 object at 0x000001A0151A9C90>
+                    	__repr()    :<__main__.Cls0 object at 0x000001A0151A9C90>
 ----------METHODS__EXX------------------------------------------------------------------------------
 __getattribute__    	TypeError   :TypeError('expected 1 argument, got 0')
-====================================================================================================
+==========================================================================================
 """
 ```
 
 ********************************************************************************
```

### Comparing `object_info-0.2.3/setup.py` & `object_info-0.2.4/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/py-enum-1.1.0.tar.gz` & `tmp/py-enum-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-enum-1.1.0.tar", last modified: Wed Apr 24 16:52:53 2024, max compression
+gzip compressed data, was "dist/py-enum-1.1.1.tar", last modified: Fri May  3 16:31:03 2024, max compression
```

## Comparing `py-enum-1.1.0.tar` & `py-enum-1.1.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 skyler     (501) staff       (20)        0 2024-04-24 16:52:53.004480 py-enum-1.1.0/
--rw-r--r--   0 skyler     (501) staff       (20)     1066 2024-03-12 15:29:53.000000 py-enum-1.1.0/LICENSE
--rw-r--r--   0 skyler     (501) staff       (20)      249 2024-03-12 15:29:53.000000 py-enum-1.1.0/MANIFEST.in
--rw-r--r--   0 skyler     (501) staff       (20)     6483 2024-04-24 16:52:53.004281 py-enum-1.1.0/PKG-INFO
--rw-r--r--   0 skyler     (501) staff       (20)     4796 2024-04-24 16:29:18.000000 py-enum-1.1.0/README.md
-drwxr-xr-x   0 skyler     (501) staff       (20)        0 2024-04-24 16:52:53.001325 py-enum-1.1.0/py_enum/
--rw-r--r--   0 skyler     (501) staff       (20)      183 2024-04-24 16:18:06.000000 py-enum-1.1.0/py_enum/__init__.py
--rw-r--r--   0 skyler     (501) staff       (20)     3055 2024-04-24 16:18:06.000000 py-enum-1.1.0/py_enum/choice.py
--rw-r--r--   0 skyler     (501) staff       (20)    24116 2024-03-12 15:29:53.000000 py-enum-1.1.0/py_enum/enum.py
--rw-r--r--   0 skyler     (501) staff       (20)     2339 2024-03-12 15:29:53.000000 py-enum-1.1.0/py_enum/utils.py
-drwxr-xr-x   0 skyler     (501) staff       (20)        0 2024-04-24 16:52:53.002177 py-enum-1.1.0/py_enum.egg-info/
--rw-r--r--   0 skyler     (501) staff       (20)     6483 2024-04-24 16:52:52.000000 py-enum-1.1.0/py_enum.egg-info/PKG-INFO
--rw-r--r--   0 skyler     (501) staff       (20)      555 2024-04-24 16:52:52.000000 py-enum-1.1.0/py_enum.egg-info/SOURCES.txt
--rw-r--r--   0 skyler     (501) staff       (20)        1 2024-04-24 16:52:52.000000 py-enum-1.1.0/py_enum.egg-info/dependency_links.txt
--rw-r--r--   0 skyler     (501) staff       (20)        1 2024-04-24 16:30:32.000000 py-enum-1.1.0/py_enum.egg-info/not-zip-safe
--rw-r--r--   0 skyler     (501) staff       (20)       12 2024-04-24 16:52:52.000000 py-enum-1.1.0/py_enum.egg-info/requires.txt
--rw-r--r--   0 skyler     (501) staff       (20)        8 2024-04-24 16:52:52.000000 py-enum-1.1.0/py_enum.egg-info/top_level.txt
--rw-r--r--   0 skyler     (501) staff       (20)       38 2024-04-24 16:52:53.004541 py-enum-1.1.0/setup.cfg
--rw-r--r--   0 skyler     (501) staff       (20)     1391 2024-04-24 16:52:48.000000 py-enum-1.1.0/setup.py
-drwxr-xr-x   0 skyler     (501) staff       (20)        0 2024-04-24 16:52:53.003372 py-enum-1.1.0/tests/
--rw-r--r--   0 skyler     (501) staff       (20)       37 2024-03-12 15:29:53.000000 py-enum-1.1.0/tests/__init__.py
-drwxr-xr-x   0 skyler     (501) staff       (20)        0 2024-04-24 16:52:53.004019 py-enum-1.1.0/tests/app/
--rw-r--r--   0 skyler     (501) staff       (20)       37 2024-03-12 15:29:53.000000 py-enum-1.1.0/tests/app/__init__.py
--rw-r--r--   0 skyler     (501) staff       (20)      362 2024-03-12 15:29:53.000000 py-enum-1.1.0/tests/app/enums.py
--rw-r--r--   0 skyler     (501) staff       (20)      689 2024-04-24 14:48:49.000000 py-enum-1.1.0/tests/app/models.py
--rw-r--r--   0 skyler     (501) staff       (20)      408 2024-03-12 15:29:53.000000 py-enum-1.1.0/tests/app/serializers.py
--rw-r--r--   0 skyler     (501) staff       (20)      227 2024-03-12 15:29:53.000000 py-enum-1.1.0/tests/conftest.py
--rw-r--r--   0 skyler     (501) staff       (20)      462 2024-04-24 16:18:06.000000 py-enum-1.1.0/tests/settings.py
--rw-r--r--   0 skyler     (501) staff       (20)    61952 2024-03-12 15:29:53.000000 py-enum-1.1.0/tests/test_base.py
--rw-r--r--   0 skyler     (501) staff       (20)     6090 2024-04-24 16:18:06.000000 py-enum-1.1.0/tests/test_choice.py
--rw-r--r--   0 skyler     (501) staff       (20)     1026 2024-03-12 15:29:53.000000 py-enum-1.1.0/tests/test_django_field.py
--rw-r--r--   0 skyler     (501) staff       (20)      642 2024-03-12 15:29:53.000000 py-enum-1.1.0/tests/test_drf_serializer.py
--rw-r--r--   0 skyler     (501) staff       (20)     9892 2024-03-12 15:29:53.000000 py-enum-1.1.0/tests/test_dynamic_cls.py
+drwxr-xr-x   0 skyler     (501) staff       (20)        0 2024-05-03 16:31:03.000000 py-enum-1.1.1/
+-rw-r--r--   0 skyler     (501) staff       (20)     6586 2024-05-03 16:31:03.000000 py-enum-1.1.1/PKG-INFO
+-rw-r--r--   0 skyler     (501) staff       (20)     1066 2024-03-12 15:29:53.000000 py-enum-1.1.1/LICENSE
+drwxr-xr-x   0 skyler     (501) staff       (20)        0 2024-05-03 16:31:03.000000 py-enum-1.1.1/tests/
+-rw-r--r--   0 skyler     (501) staff       (20)      330 2024-05-03 13:45:51.000000 py-enum-1.1.1/tests/conftest.py
+-rw-r--r--   0 skyler     (501) staff       (20)      642 2024-03-12 15:29:53.000000 py-enum-1.1.1/tests/test_drf_serializer.py
+drwxr-xr-x   0 skyler     (501) staff       (20)        0 2024-05-03 16:31:03.000000 py-enum-1.1.1/tests/app/
+-rw-r--r--   0 skyler     (501) staff       (20)      564 2024-05-03 13:46:51.000000 py-enum-1.1.1/tests/app/enums.py
+-rw-r--r--   0 skyler     (501) staff       (20)      689 2024-04-24 14:48:49.000000 py-enum-1.1.1/tests/app/models.py
+-rw-r--r--   0 skyler     (501) staff       (20)      408 2024-03-12 15:29:53.000000 py-enum-1.1.1/tests/app/serializers.py
+-rw-r--r--   0 skyler     (501) staff       (20)       37 2024-03-12 15:29:53.000000 py-enum-1.1.1/tests/app/__init__.py
+-rw-r--r--   0 skyler     (501) staff       (20)     9892 2024-03-12 15:29:53.000000 py-enum-1.1.1/tests/test_dynamic_cls.py
+-rw-r--r--   0 skyler     (501) staff       (20)       37 2024-03-12 15:29:53.000000 py-enum-1.1.1/tests/__init__.py
+-rw-r--r--   0 skyler     (501) staff       (20)     1026 2024-04-30 11:17:46.000000 py-enum-1.1.1/tests/test_django_field.py
+-rw-r--r--   0 skyler     (501) staff       (20)      462 2024-04-24 17:28:59.000000 py-enum-1.1.1/tests/settings.py
+-rw-r--r--   0 skyler     (501) staff       (20)     6097 2024-05-03 13:52:46.000000 py-enum-1.1.1/tests/test_choice.py
+-rw-r--r--   0 skyler     (501) staff       (20)    61952 2024-03-12 15:29:53.000000 py-enum-1.1.1/tests/test_base.py
+-rw-r--r--   0 skyler     (501) staff       (20)      249 2024-03-12 15:29:53.000000 py-enum-1.1.1/MANIFEST.in
+-rw-r--r--   0 skyler     (501) staff       (20)     4899 2024-05-03 13:25:11.000000 py-enum-1.1.1/README.md
+-rw-r--r--   0 skyler     (501) staff       (20)     1156 2024-04-24 17:15:21.000000 py-enum-1.1.1/setup.py
+-rw-r--r--   0 skyler     (501) staff       (20)       38 2024-05-03 16:31:03.000000 py-enum-1.1.1/setup.cfg
+drwxr-xr-x   0 skyler     (501) staff       (20)        0 2024-05-03 16:31:03.000000 py-enum-1.1.1/py_enum.egg-info/
+-rw-r--r--   0 skyler     (501) staff       (20)     6586 2024-05-03 16:31:03.000000 py-enum-1.1.1/py_enum.egg-info/PKG-INFO
+-rw-r--r--   0 skyler     (501) staff       (20)        1 2024-04-24 16:30:32.000000 py-enum-1.1.1/py_enum.egg-info/not-zip-safe
+-rw-r--r--   0 skyler     (501) staff       (20)      555 2024-05-03 16:31:03.000000 py-enum-1.1.1/py_enum.egg-info/SOURCES.txt
+-rw-r--r--   0 skyler     (501) staff       (20)       12 2024-05-03 16:31:03.000000 py-enum-1.1.1/py_enum.egg-info/requires.txt
+-rw-r--r--   0 skyler     (501) staff       (20)        8 2024-05-03 16:31:03.000000 py-enum-1.1.1/py_enum.egg-info/top_level.txt
+-rw-r--r--   0 skyler     (501) staff       (20)        1 2024-05-03 16:31:03.000000 py-enum-1.1.1/py_enum.egg-info/dependency_links.txt
+drwxr-xr-x   0 skyler     (501) staff       (20)        0 2024-05-03 16:31:03.000000 py-enum-1.1.1/py_enum/
+-rw-r--r--   0 skyler     (501) staff       (20)     3443 2024-05-03 13:48:45.000000 py-enum-1.1.1/py_enum/choice.py
+-rw-r--r--   0 skyler     (501) staff       (20)      183 2024-05-03 13:25:23.000000 py-enum-1.1.1/py_enum/__init__.py
+-rw-r--r--   0 skyler     (501) staff       (20)     2339 2024-05-03 13:12:51.000000 py-enum-1.1.1/py_enum/utils.py
+-rw-r--r--   0 skyler     (501) staff       (20)    24116 2024-03-12 15:29:53.000000 py-enum-1.1.1/py_enum/enum.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `py-enum-1.1.0/LICENSE` & `py-enum-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py-enum-1.1.0/PKG-INFO` & `py-enum-1.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: py-enum
-Version: 1.1.0
+Version: 1.1.1
 Summary: enums for choices fields
 Home-page: https://github.com/SkylerHu/py-enum.git
 Author: SkylerHu
 Author-email: skylerhu@qq.com
 License: MIT Licence
 Description: # py-enum
         A python enum module for python2.7 and django choices fields.
         
-        ## 前言
-        通过改造python3中的enum.py而来，主要变更有：
-        - 在支持python3的同时，增加了对python2的支持
-        - Django中`choices`选项直接使用枚举对象
+        通过改造python3中的enum.py而来，增加对python2的支持，并新增类`ChoiceEnum`用于以下场景：
+        - argparse使用 `add_argument` 的参数 `choices`
+        - Django中 `models.CharField` 的参数 `choices`
+        - Django REST framework `ChoiceField` 的参数 `choices`
         
-        ## 安装
+        
+        ## 1. 安装
         
         	pip install py-enum
         
         可查看版本变更记录[ChangeLog](https://github.com/SkylerHu/py-enum/blob/master/docs/CHANGELOG-1.x.md)
         
-        # 类ChoiceEnum
-        集成自改造后的Enum对象，用于创建枚举型的基类。
+        ## 2. 使用(Usage)
         
-        ## 使用
+        ### 2.1 用ChoiceEnum定义枚举
         
         ```python
         # 导入
         from py_enum import ChoiceEnum, unique
         
         # 定义
         class Color(ChoiceEnum):
@@ -40,21 +40,21 @@
             PROCESSING = ('processing', '处理中')
             APPROVED = ('approved', '已审批')
             CANCELED = ('canceled', '已取消')
             CLOSED = ('closed', '已关闭')
         ```
         定义如上，按照`Key = (value, label, extra)`的形式进行定义，value定义的值；label是对值的描述；第三个参数是extra，额外信息，可以任意类型。
         
-        ## 基础用法
+        ### 2.2 基础用法
         - `直接根据Key访问value值`，而并不是一个tuple，正是和原生Enum的区别
         - get_label方法
         - get_extra方法
         - `直接遍历枚举类`，这是能够作为Choices Enum的关键
         
-        ```
+        ```python
         print(Color.RED)  # 1
         type(Color.RED)  # <enum 'Color'>
         len(colors) == 3  # true
         Color.RED in Color  # true
         1 in Color  # true
         0 not in Color  # true
         
@@ -74,93 +74,93 @@
             {"key": "RED", "value": 1, "label": "红色"},
             {"key": "GREEN", "value": 2, "label": "绿色"},
             {"key": "BLUE", "value": 3, "label": "蓝色", "extra": {"value": "blue"}}
         ]
         """
         ```
         
-        ## 枚举对象实例化
-        ```
+        ### 2.3 枚举对象实例化
+        ```python
         member = Color(Color.RED)  # 或者 Color(1)
         member.value == 1  # true
         member.name == 'RED'  # true
         member.label == '红色'  # true
         member.option == (1, '红色')  # true
         member.extra == None  # true，因为没有定义
         # 以上几个属性无法修改，直接赋值会抛出AttributeError异常
         member.value in Color  # true
         ```
         
-        ## 在Python argparse中使用
-        ```
+        ### 2.4 在Python argparse中使用
+        ```python
         import argparse
         
         parser = argparse.ArgumentParser(description='test ChoiceEnum use in argparse.')
         parser.add_argument('--color', type=int, choices=Color, required=True)
         args = parser.parse_args(['--color', str(Color.RED)])
         # args.color == Color.RED
         ```
         
-        ## 在Django中使用
-        ```
+        ### 2.5 在Django中使用
+        ```python
         from django.db import models
         
         class ColorModel(models.Model):
             color = models.IntegerField(verbose_name='颜色', choices=Color, default=Color.RED)
         
         instance = ColorModel.objects.create()
         assert instance.color == colors.RED
         instance.color = colors.BLUE
         instance.save()
         ```
         
-        ## 在DRF中使用
-        ```
+        ### 2.6 在DRF中使用
+        ```python
         from rest_framework import serializers
         
         class ColorSerializer(serializers.Serializer):
             color = serializers.ChoiceField(help_text='选择颜色', choices=Color, default=Color.RED)
         
         s = ColorSerializer()
         s = ColorSerializer(data={'status': status.CLOSED})
         assert s.is_valid() is True
         s = ColorSerializer(data={'status': 1})
         assert s.is_valid() is True
         s = ColorSerializer(data={'status': 0})
         assert s.is_valid() is False  # 值不在枚举定义范围内，校验不通过
         ```
         
-        # 类Enum和unique
+        ### 2.7 类Enum和unique
         和python3中原生的Enum并无太大区别，具体可以参考[官方原生开发文档](https://docs.python.org/3.6/library/enum.html)
         
-        ## 导入
-        
-            from py_enum import Enum unique
+        ```python
+        from py_enum import Enum, unique
         
-            @unique
-            class Season(Enum):
-                SPRING = 1
-                SUMMER = 2
-                AUTUMN = 3
-                WINTER = 4
+        @unique
+        class Season(Enum):
+            SPRING = 1
+            SUMMER = 2
+            AUTUMN = 3
+            WINTER = 4
+        ```
         
-        # 对比
+        ## 3. 对比
         - `Enum`可以在`Python2`中使用，但需要注意的是：
           - members无序，属性定义时申明的顺序和直接遍历枚举对象时并不一定一致；需通过`_order_`来定义member的顺序
           - python2没有定义__bool__，所以不能直接用class类或者member来做逻辑判断
           - 执行 Season.SPRING > Season.SUMMER 不会报错，但结果也不符合预期
             - py3执行会raise TypeError, 不允许比较
             - 但是ChoiceEnum是直接取值，可以用来做比较运算
           - 枚举类定义时，无法识别多个相同的Key
           - 在多继承方面会受限
         - `Enum`和Python3原生enum.py对比，保留了`Enum`类和`unique`方法
         - `ChoiceEnum`和Django的 models.Choices 的优势在于低版本Django也能使用，且普通Python项目脚本也能使用
         - 新增了额外的特性
           - 额外多出了`ChoiceEnum.extra`的用法，对不同枚举成员做映射配置相关场景可以使用
-          - 增加方法`ChoiceEnum.to_js_enum`返回数组数据，可以用于前端枚举库[js-enumerate](https://github.com/SkylerHu/js-enum)初始化使用
+          - 增加方法`ChoiceEnum.to_js_enum`返回数组数据，可以用于前端枚举库 [js-enumerate](https://github.com/SkylerHu/js-enum) 初始化使用
         
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
```

### Comparing `py-enum-1.1.0/README.md` & `py-enum-1.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # py-enum
 A python enum module for python2.7 and django choices fields.
 
-## 前言
-通过改造python3中的enum.py而来，主要变更有：
-- 在支持python3的同时，增加了对python2的支持
-- Django中`choices`选项直接使用枚举对象
+通过改造python3中的enum.py而来，增加对python2的支持，并新增类`ChoiceEnum`用于以下场景：
+- argparse使用 `add_argument` 的参数 `choices`
+- Django中 `models.CharField` 的参数 `choices`
+- Django REST framework `ChoiceField` 的参数 `choices`
 
-## 安装
+
+## 1. 安装
 
 	pip install py-enum
 
 可查看版本变更记录[ChangeLog](./docs/CHANGELOG-1.x.md)
 
-# 类ChoiceEnum
-集成自改造后的Enum对象，用于创建枚举型的基类。
+## 2. 使用(Usage)
 
-## 使用
+### 2.1 用ChoiceEnum定义枚举
 
 ```python
 # 导入
 from py_enum import ChoiceEnum, unique
 
 # 定义
 class Color(ChoiceEnum):
@@ -32,21 +32,21 @@
     PROCESSING = ('processing', '处理中')
     APPROVED = ('approved', '已审批')
     CANCELED = ('canceled', '已取消')
     CLOSED = ('closed', '已关闭')
 ```
 定义如上，按照`Key = (value, label, extra)`的形式进行定义，value定义的值；label是对值的描述；第三个参数是extra，额外信息，可以任意类型。
 
-## 基础用法
+### 2.2 基础用法
 - `直接根据Key访问value值`，而并不是一个tuple，正是和原生Enum的区别
 - get_label方法
 - get_extra方法
 - `直接遍历枚举类`，这是能够作为Choices Enum的关键
 
-```
+```python
 print(Color.RED)  # 1
 type(Color.RED)  # <enum 'Color'>
 len(colors) == 3  # true
 Color.RED in Color  # true
 1 in Color  # true
 0 not in Color  # true
 
@@ -66,86 +66,86 @@
     {"key": "RED", "value": 1, "label": "红色"},
     {"key": "GREEN", "value": 2, "label": "绿色"},
     {"key": "BLUE", "value": 3, "label": "蓝色", "extra": {"value": "blue"}}
 ]
 """
 ```
 
-## 枚举对象实例化
-```
+### 2.3 枚举对象实例化
+```python
 member = Color(Color.RED)  # 或者 Color(1)
 member.value == 1  # true
 member.name == 'RED'  # true
 member.label == '红色'  # true
 member.option == (1, '红色')  # true
 member.extra == None  # true，因为没有定义
 # 以上几个属性无法修改，直接赋值会抛出AttributeError异常
 member.value in Color  # true
 ```
 
-## 在Python argparse中使用
-```
+### 2.4 在Python argparse中使用
+```python
 import argparse
 
 parser = argparse.ArgumentParser(description='test ChoiceEnum use in argparse.')
 parser.add_argument('--color', type=int, choices=Color, required=True)
 args = parser.parse_args(['--color', str(Color.RED)])
 # args.color == Color.RED
 ```
 
-## 在Django中使用
-```
+### 2.5 在Django中使用
+```python
 from django.db import models
 
 class ColorModel(models.Model):
     color = models.IntegerField(verbose_name='颜色', choices=Color, default=Color.RED)
 
 instance = ColorModel.objects.create()
 assert instance.color == colors.RED
 instance.color = colors.BLUE
 instance.save()
 ```
 
-## 在DRF中使用
-```
+### 2.6 在DRF中使用
+```python
 from rest_framework import serializers
 
 class ColorSerializer(serializers.Serializer):
     color = serializers.ChoiceField(help_text='选择颜色', choices=Color, default=Color.RED)
 
 s = ColorSerializer()
 s = ColorSerializer(data={'status': status.CLOSED})
 assert s.is_valid() is True
 s = ColorSerializer(data={'status': 1})
 assert s.is_valid() is True
 s = ColorSerializer(data={'status': 0})
 assert s.is_valid() is False  # 值不在枚举定义范围内，校验不通过
 ```
 
-# 类Enum和unique
+### 2.7 类Enum和unique
 和python3中原生的Enum并无太大区别，具体可以参考[官方原生开发文档](https://docs.python.org/3.6/library/enum.html)
 
-## 导入
-
-    from py_enum import Enum unique
+```python
+from py_enum import Enum, unique
 
-    @unique
-    class Season(Enum):
-        SPRING = 1
-        SUMMER = 2
-        AUTUMN = 3
-        WINTER = 4
+@unique
+class Season(Enum):
+    SPRING = 1
+    SUMMER = 2
+    AUTUMN = 3
+    WINTER = 4
+```
 
-# 对比
+## 3. 对比
 - `Enum`可以在`Python2`中使用，但需要注意的是：
   - members无序，属性定义时申明的顺序和直接遍历枚举对象时并不一定一致；需通过`_order_`来定义member的顺序
   - python2没有定义__bool__，所以不能直接用class类或者member来做逻辑判断
   - 执行 Season.SPRING > Season.SUMMER 不会报错，但结果也不符合预期
     - py3执行会raise TypeError, 不允许比较
     - 但是ChoiceEnum是直接取值，可以用来做比较运算
   - 枚举类定义时，无法识别多个相同的Key
   - 在多继承方面会受限
 - `Enum`和Python3原生enum.py对比，保留了`Enum`类和`unique`方法
 - `ChoiceEnum`和Django的 models.Choices 的优势在于低版本Django也能使用，且普通Python项目脚本也能使用
 - 新增了额外的特性
   - 额外多出了`ChoiceEnum.extra`的用法，对不同枚举成员做映射配置相关场景可以使用
-  - 增加方法`ChoiceEnum.to_js_enum`返回数组数据，可以用于前端枚举库[js-enumerate](https://github.com/SkylerHu/js-enum)初始化使用
+  - 增加方法`ChoiceEnum.to_js_enum`返回数组数据，可以用于前端枚举库 [js-enumerate](https://github.com/SkylerHu/js-enum) 初始化使用
```

### Comparing `py-enum-1.1.0/py_enum/choice.py` & `py-enum-1.1.1/py_enum/choice.py`

 * *Files 12% similar despite different names*

```diff
@@ -41,15 +41,18 @@
         if not isinstance(value[1], six.string_types):
             raise TypeError('value[1] %r use for label, should be a string' % (value[1], ))
 
 
 class EnumChoiceMeta(EnumMeta):
 
     def __contains__(cls, value):
-        return value in cls._value2member_map_
+        if not isinstance(value, Enum):
+            # Allow non-enums to match against member values.
+            return value in cls._value2member_map_
+        return super(EnumChoiceMeta, cls).__contains__(value)
 
     def __getattribute__(cls, name):
         attr = super(EnumChoiceMeta, cls).__getattribute__(name)
         if name == '_member_names_':
             pass
         elif name in cls._member_names_:
             attr = attr.value
@@ -57,14 +60,26 @@
 
     def __getattr__(cls, name):
         return super(EnumChoiceMeta, cls).__getattr__(name).value
 
     def __iter__(cls):
         return (cls._member_map_[name].option for name in cls._member_names_)
 
+    @property
+    def choices(cls):
+        return list(cls)
+
+    @property
+    def values(cls):
+        return [value for value, _ in cls]
+
+    @property
+    def labels(cls):
+        return [label for _, label in cls]
+
 
 class ChoiceEnum(six.with_metaclass(EnumChoiceMeta, _ChoiceType, Enum)):
 
     @DynamicClassAttribute
     def label(self):
         """枚举值对应的显示文案"""
         return self._label_
```

### Comparing `py-enum-1.1.0/py_enum/enum.py` & `py-enum-1.1.1/py_enum/enum.py`

 * *Files identical despite different names*

### Comparing `py-enum-1.1.0/py_enum/utils.py` & `py-enum-1.1.1/py_enum/utils.py`

 * *Files identical despite different names*

### Comparing `py-enum-1.1.0/py_enum.egg-info/PKG-INFO` & `py-enum-1.1.1/py_enum.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: py-enum
-Version: 1.1.0
+Version: 1.1.1
 Summary: enums for choices fields
 Home-page: https://github.com/SkylerHu/py-enum.git
 Author: SkylerHu
 Author-email: skylerhu@qq.com
 License: MIT Licence
 Description: # py-enum
         A python enum module for python2.7 and django choices fields.
         
-        ## 前言
-        通过改造python3中的enum.py而来，主要变更有：
-        - 在支持python3的同时，增加了对python2的支持
-        - Django中`choices`选项直接使用枚举对象
+        通过改造python3中的enum.py而来，增加对python2的支持，并新增类`ChoiceEnum`用于以下场景：
+        - argparse使用 `add_argument` 的参数 `choices`
+        - Django中 `models.CharField` 的参数 `choices`
+        - Django REST framework `ChoiceField` 的参数 `choices`
         
-        ## 安装
+        
+        ## 1. 安装
         
         	pip install py-enum
         
         可查看版本变更记录[ChangeLog](https://github.com/SkylerHu/py-enum/blob/master/docs/CHANGELOG-1.x.md)
         
-        # 类ChoiceEnum
-        集成自改造后的Enum对象，用于创建枚举型的基类。
+        ## 2. 使用(Usage)
         
-        ## 使用
+        ### 2.1 用ChoiceEnum定义枚举
         
         ```python
         # 导入
         from py_enum import ChoiceEnum, unique
         
         # 定义
         class Color(ChoiceEnum):
@@ -40,21 +40,21 @@
             PROCESSING = ('processing', '处理中')
             APPROVED = ('approved', '已审批')
             CANCELED = ('canceled', '已取消')
             CLOSED = ('closed', '已关闭')
         ```
         定义如上，按照`Key = (value, label, extra)`的形式进行定义，value定义的值；label是对值的描述；第三个参数是extra，额外信息，可以任意类型。
         
-        ## 基础用法
+        ### 2.2 基础用法
         - `直接根据Key访问value值`，而并不是一个tuple，正是和原生Enum的区别
         - get_label方法
         - get_extra方法
         - `直接遍历枚举类`，这是能够作为Choices Enum的关键
         
-        ```
+        ```python
         print(Color.RED)  # 1
         type(Color.RED)  # <enum 'Color'>
         len(colors) == 3  # true
         Color.RED in Color  # true
         1 in Color  # true
         0 not in Color  # true
         
@@ -74,93 +74,93 @@
             {"key": "RED", "value": 1, "label": "红色"},
             {"key": "GREEN", "value": 2, "label": "绿色"},
             {"key": "BLUE", "value": 3, "label": "蓝色", "extra": {"value": "blue"}}
         ]
         """
         ```
         
-        ## 枚举对象实例化
-        ```
+        ### 2.3 枚举对象实例化
+        ```python
         member = Color(Color.RED)  # 或者 Color(1)
         member.value == 1  # true
         member.name == 'RED'  # true
         member.label == '红色'  # true
         member.option == (1, '红色')  # true
         member.extra == None  # true，因为没有定义
         # 以上几个属性无法修改，直接赋值会抛出AttributeError异常
         member.value in Color  # true
         ```
         
-        ## 在Python argparse中使用
-        ```
+        ### 2.4 在Python argparse中使用
+        ```python
         import argparse
         
         parser = argparse.ArgumentParser(description='test ChoiceEnum use in argparse.')
         parser.add_argument('--color', type=int, choices=Color, required=True)
         args = parser.parse_args(['--color', str(Color.RED)])
         # args.color == Color.RED
         ```
         
-        ## 在Django中使用
-        ```
+        ### 2.5 在Django中使用
+        ```python
         from django.db import models
         
         class ColorModel(models.Model):
             color = models.IntegerField(verbose_name='颜色', choices=Color, default=Color.RED)
         
         instance = ColorModel.objects.create()
         assert instance.color == colors.RED
         instance.color = colors.BLUE
         instance.save()
         ```
         
-        ## 在DRF中使用
-        ```
+        ### 2.6 在DRF中使用
+        ```python
         from rest_framework import serializers
         
         class ColorSerializer(serializers.Serializer):
             color = serializers.ChoiceField(help_text='选择颜色', choices=Color, default=Color.RED)
         
         s = ColorSerializer()
         s = ColorSerializer(data={'status': status.CLOSED})
         assert s.is_valid() is True
         s = ColorSerializer(data={'status': 1})
         assert s.is_valid() is True
         s = ColorSerializer(data={'status': 0})
         assert s.is_valid() is False  # 值不在枚举定义范围内，校验不通过
         ```
         
-        # 类Enum和unique
+        ### 2.7 类Enum和unique
         和python3中原生的Enum并无太大区别，具体可以参考[官方原生开发文档](https://docs.python.org/3.6/library/enum.html)
         
-        ## 导入
-        
-            from py_enum import Enum unique
+        ```python
+        from py_enum import Enum, unique
         
-            @unique
-            class Season(Enum):
-                SPRING = 1
-                SUMMER = 2
-                AUTUMN = 3
-                WINTER = 4
+        @unique
+        class Season(Enum):
+            SPRING = 1
+            SUMMER = 2
+            AUTUMN = 3
+            WINTER = 4
+        ```
         
-        # 对比
+        ## 3. 对比
         - `Enum`可以在`Python2`中使用，但需要注意的是：
           - members无序，属性定义时申明的顺序和直接遍历枚举对象时并不一定一致；需通过`_order_`来定义member的顺序
           - python2没有定义__bool__，所以不能直接用class类或者member来做逻辑判断
           - 执行 Season.SPRING > Season.SUMMER 不会报错，但结果也不符合预期
             - py3执行会raise TypeError, 不允许比较
             - 但是ChoiceEnum是直接取值，可以用来做比较运算
           - 枚举类定义时，无法识别多个相同的Key
           - 在多继承方面会受限
         - `Enum`和Python3原生enum.py对比，保留了`Enum`类和`unique`方法
         - `ChoiceEnum`和Django的 models.Choices 的优势在于低版本Django也能使用，且普通Python项目脚本也能使用
         - 新增了额外的特性
           - 额外多出了`ChoiceEnum.extra`的用法，对不同枚举成员做映射配置相关场景可以使用
-          - 增加方法`ChoiceEnum.to_js_enum`返回数组数据，可以用于前端枚举库[js-enumerate](https://github.com/SkylerHu/js-enum)初始化使用
+          - 增加方法`ChoiceEnum.to_js_enum`返回数组数据，可以用于前端枚举库 [js-enumerate](https://github.com/SkylerHu/js-enum) 初始化使用
         
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
```

### Comparing `py-enum-1.1.0/py_enum.egg-info/SOURCES.txt` & `py-enum-1.1.1/py_enum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-enum-1.1.0/tests/app/models.py` & `py-enum-1.1.1/tests/app/models.py`

 * *Files identical despite different names*

### Comparing `py-enum-1.1.0/tests/test_base.py` & `py-enum-1.1.1/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `py-enum-1.1.0/tests/test_choice.py` & `py-enum-1.1.1/tests/test_choice.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,14 +55,15 @@
             test = 1
 
 
 def test_contains(colors, status):
     assert colors.RED in colors
     assert 0 not in colors
     assert status.CLOSED in status
+    assert colors(colors.RED) in colors
 
 
 def test_enum_with_value_name_label():
     class Huh(ChoiceEnum):
         name = (1, 'label-name')
         value = (2, 'label-value')
         label = (3, 'label-label')
@@ -91,36 +92,30 @@
         assert loads(dumps(status.CLOSED, protocol=protocol)) == status.CLOSED
         member = status(status.CLOSED)
         assert loads(dumps(member, protocol=protocol)) is member
 
 
 def test_enum_member(colors):
     assert colors['RED'].value == 1
-    assert colors(1).value == 1
-    assert colors(1) is colors['RED']
+    member = colors(1)
+    assert member.value == 1
+    assert member is colors['RED']
 
 
 def test_no_such_enum_member(colors):
     with pytest.raises(ValueError):
         colors(0)
     with pytest.raises(KeyError):
         colors['GREY']
 
 
-def test_order_members(colors):
+def test_order_members(colors, order_colors):
     _colors = colors
     if six.PY2:
-        # python2需要定义排序 _order_
-        class Color(ChoiceEnum):
-            _order_ = 'RED GREEN BLUE'
-            RED = (1, '红色')
-            GREEN = (2, '绿色')
-            BLUE = (3, '蓝色')
-
-        _colors = Color
+        _colors = order_colors
     else:
         with pytest.raises(TypeError):
             # python3定义了排序，属性顺序必须一致
             class Color(ChoiceEnum):
                 _order_ = 'RED BLUE GREEN'
                 RED = (1, '红色')
                 GREEN = (2, '绿色')
@@ -177,23 +172,17 @@
     assert Color.get_extra(Color.BLUE) == 3
     assert Color.get_extra(Color.GREY) == 'grey'
     assert Color.get_extra(Color.BLACK)['value'] == 'grey'
     assert Color.get_extra(Color.WHITE) == (1, 2)
     assert Color.get_extra(Color.YELLOW) == ('first', 'second')
 
 
-def test_to_js_enum():
-    class Color(ChoiceEnum):
-        _order_ = 'RED GREEN BLUE'
-        RED = (1, '红色')
-        GREEN = (2, '绿色')
-        BLUE = (3, '蓝色', {'value': 'blue'})
-
-    items = Color.to_js_enum()
-    assert len(items) == len(Color)
+def test_to_js_enum(order_colors):
+    items = order_colors.to_js_enum()
+    assert len(items) == len(order_colors)
     expect_output = [
         {"key": "RED", "value": 1, "label": "红色"},
         {"key": "GREEN", "value": 2, "label": "绿色"},
         {"key": "BLUE", "value": 3, "label": "蓝色", "extra": {"value": "blue"}}
     ]
     assert items == expect_output
     assert json.dumps(items) == json.dumps(expect_output)
@@ -212,7 +201,16 @@
         parser.parse_args(['--color', str(test_c)])
 
     test_c = 1
     assert test_c == colors.RED
     args = parser.parse_args(['--color', str(test_c)])
     assert args.color is colors.RED
     assert args.color == test_c
+
+
+def test_cls_property(colors, order_colors):
+    _colors = colors
+    if six.PY2:
+        _colors = order_colors
+    assert _colors.values == [1, 2, 3]
+    assert _colors.labels == ['红色', '绿色', '蓝色']
+    assert _colors.choices == [(1, '红色'), (2, '绿色'), (3, '蓝色')]
```

### Comparing `py-enum-1.1.0/tests/test_django_field.py` & `py-enum-1.1.1/tests/test_django_field.py`

 * *Files identical despite different names*

### Comparing `py-enum-1.1.0/tests/test_drf_serializer.py` & `py-enum-1.1.1/tests/test_drf_serializer.py`

 * *Files identical despite different names*

### Comparing `py-enum-1.1.0/tests/test_dynamic_cls.py` & `py-enum-1.1.1/tests/test_dynamic_cls.py`

 * *Files identical despite different names*


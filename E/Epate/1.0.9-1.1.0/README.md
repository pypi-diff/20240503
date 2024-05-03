# Comparing `tmp/epate-1.0.9.tar.gz` & `tmp/epate-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epate-1.0.9.tar", last modified: Fri Apr 26 18:24:57 2024, max compression
+gzip compressed data, was "epate-1.1.0.tar", last modified: Fri May  3 03:20:56 2024, max compression
```

## Comparing `epate-1.0.9.tar` & `epate-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 18:24:57.983624 epate-1.0.9/
-drwxrwxrwx   0        0        0        0 2024-04-26 18:24:57.949802 epate-1.0.9/Epate/
--rw-rw-rw-   0        0        0     5458 2024-04-26 18:24:26.000000 epate-1.0.9/Epate/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 17:50:18.000000 epate-1.0.9/Epate/epate.py
-drwxrwxrwx   0        0        0        0 2024-04-26 18:24:57.978312 epate-1.0.9/Epate.egg-info/
--rw-rw-rw-   0        0        0      562 2024-04-26 18:24:57.000000 epate-1.0.9/Epate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2024-04-26 18:24:57.000000 epate-1.0.9/Epate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 18:24:57.000000 epate-1.0.9/Epate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-04-26 18:24:57.000000 epate-1.0.9/Epate.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-04-26 18:24:57.000000 epate-1.0.9/Epate.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-26 18:24:57.000000 epate-1.0.9/Epate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11558 2024-04-26 15:22:07.000000 epate-1.0.9/LICENSE
--rw-rw-rw-   0        0        0      562 2024-04-26 18:24:57.979314 epate-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0       66 2024-04-26 15:22:07.000000 epate-1.0.9/README.md
--rw-rw-rw-   0        0        0       42 2024-04-26 18:24:57.983624 epate-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0      901 2024-04-26 18:24:48.000000 epate-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 03:20:56.984619 epate-1.1.0/
+drwxrwxrwx   0        0        0        0 2024-05-03 03:20:56.968721 epate-1.1.0/Epate/
+-rw-rw-rw-   0        0        0     5365 2024-05-03 03:13:09.000000 epate-1.1.0/Epate/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 17:50:18.000000 epate-1.1.0/Epate/epate.py
+drwxrwxrwx   0        0        0        0 2024-05-03 03:20:56.982621 epate-1.1.0/Epate.egg-info/
+-rw-rw-rw-   0        0        0      562 2024-05-03 03:20:56.000000 epate-1.1.0/Epate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2024-05-03 03:20:56.000000 epate-1.1.0/Epate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 03:20:56.000000 epate-1.1.0/Epate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-05-03 03:20:56.000000 epate-1.1.0/Epate.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-05-03 03:20:56.000000 epate-1.1.0/Epate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-03 03:20:56.000000 epate-1.1.0/Epate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11558 2024-04-26 15:22:07.000000 epate-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0      562 2024-05-03 03:20:56.983620 epate-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2242 2024-04-30 14:40:20.000000 epate-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-03 03:20:56.985620 epate-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      878 2024-05-03 03:13:26.000000 epate-1.1.0/setup.py
```

### Comparing `epate-1.0.9/Epate/__init__.py` & `epate-1.1.0/Epate/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,157 +1,205 @@
 import requests
 
-def login(username,password,print='no'):
-        session = requests.Session()
-        login_data = {'pid': '65edCTyg',
-                'identity': username,
-                'password': password}
-        result = session.post('https://api.codemao.cn/tiger/v3/web/accounts/login', json=login_data)
-        code = str(result.status_code)
-        def get():
-            return(result.text)
-
-        if code == '201':
-            if print == 'yes':
-                print("Login Successful[201]")
-            else:
-                return('201')
-        else:
-            if print == 'yes':
-                print("Login Failed["+ code+"]")
-            else:
-                return(code)
-               
+session = requests.Session
+
+def login(username, password, print='no'):
+
+    login_data = {
+        'pid': '65edCTyg',
+        'identity': username,
+        'password': password
+    }
+    result = session.post('https://api.codemao.cn/tiger/v3/web/accounts/login',
+                          json=login_data)
+    code = str(result.status_code)
+    global get
+
+    def get():
+        return (result.text)
+
+    if code == '201':
+        if print == 'yes':
+            print("Login Successful[201]")
+        else:
+            return ('201')
+    else:
+        if print == 'yes':
+            print("Login Failed[" + code + "]")
+        else:
+            return (code)
+
+
 def logout(print='no'):
-        session = requests.Session()
-        result = session.post('https://api.codemao.cn/tiger/v3/web/accounts/loginout')
 
-        def get():
-            return(result.text)
+    result = session.post(
+        'https://api.codemao.cn/tiger/v3/web/accounts/loginout')
+    global get
+
+    def get():
+        return (result.text)
+
+    if result.status_code == 200:
+        if print == 'yes':
+            print("Logout Successful[204]")
+        else:
+            return ('204')
+    else:
+        if print == 'yes':
+            print("Logout Failed[" + str(result.status_code) + "]")
+        else:
+            return (str(result.status_code))
+
+
+def usrinfo(kind, inputstr, inputint: int, print='no'):
+    if kind == 'nick':
+
+        change = {'nickname': inputstr}
+        result = session.patch("/tiger/v3/web/accounts/info", data=change)
+
+    if kind == 'full':
+
+        change = {'fullname': inputstr}
+        result = session.patch("/tiger/v3/web/accounts/info", data=change)
+
+    if kind == 'desc':
+
+        change = {'description': inputstr}
+        result = session.patch("/tiger/v3/web/accounts/info", data=change)
+
+    if kind == 'sex':
+
+        change = {'sex': inputint}
+        result = session.patch("/tiger/v3/web/accounts/info", data=change)
+
+    if kind == 'birth':
+
+        change = {'birthday	': inputint}
+        result = session.patch("/tiger/v3/web/accounts/info", data=change)
+
+    if kind == 'avat':
+
+        change = {'avatar_url': inputstr}
+        result = session.patch("/tiger/v3/web/accounts/info", data=change)
+    global get
+
+    def get():
+        return (result.text)
+
+    if result.status_code == 204:
+        if print == 'yes':
+            print("Change Info Successful[204]")
+        else:
+            return ('204')
+    else:
+        if print == 'yes':
+            print("Change Info Failed[" + str(result.status_code) + "]")
+        else:
+            return (str(result.status_code))
+
+
+def psc(old_password, new_password, print='no'):
+
+    change = {
+        'old_password': old_password,
+        'password': new_password,
+        'confirm_password': new_password
+    }
+    result = session.patch("/tiger/v3/web/accounts/info", data=change)
+
+    global get
+    def get():
+        return (result.text)
 
-        if result.status_code == 200:
-            if print == 'yes':
-                print("Logout Successful[204]")
-            else:
-                return('204')
-        else:
-            if print == 'yes':
-                print("Logout Failed["+str(result.status_code)+"]")
-            else:
-                return(str(result.status_code))
-            
-def usrinfo(kind,inputstr,inputint:int,print='no'):
-        if kind == 'nick':
-            session = requests.Session()
-            change = {'nickname':inputstr}
-            result = session.patch("/tiger/v3/web/accounts/info",data=change)
-        
-        if kind == 'full':
-            session = requests.Session()
-            change = {'fullname':inputstr}
-            result = session.patch("/tiger/v3/web/accounts/info",data=change)
-
-        if kind == 'desc':
-            session = requests.Session()
-            change = {'description':inputstr}
-            result = session.patch("/tiger/v3/web/accounts/info",data=change)
-
-        if kind == 'sex':
-            session = requests.Session()
-            change = {'sex':inputint}
-            result = session.patch("/tiger/v3/web/accounts/info",data=change)
-
-        if kind == 'birth':
-            session = requests.Session()
-            change = {'birthday	':inputint}
-            result = session.patch("/tiger/v3/web/accounts/info",data=change)
-
-        if kind == 'avat':
-            session = requests.Session()
-            change = {'avatar_url':inputstr}
-            result = session.patch("/tiger/v3/web/accounts/info",data=change)
-
-        def get():
-                return(result.text)    
-            
-        if result.status_code == 204:
-            if print == 'yes':
-                print("Change Info Successful[204]")
-            else:
-                return('204')
-        else:
-            if print == 'yes':
-                print("Change Info Failed["+str(result.status_code)+"]")
-            else:
-                return(str(result.status_code))
-                
-def psc(old_password,new_password,print='no'):
-        session = requests.Session()
-        change = {'old_password':old_password,'password':new_password,'confirm_password':new_password}
-        result = session.patch("/tiger/v3/web/accounts/info",data=change)
-        def get():
-                return(result.text)    
-            
-        if result.status_code == 204:
-            if print == 'yes':
-                print("Change Password Successful[204]")
-            else:
-                return('204')
-        else:
-            if print == 'yes':
-                print("Change Password Failed["+str(result.status_code)+"]")
-            else:
-                return(str(result.status_code))
-
-def like(workid,print='no'):
-        session = requests.Session()
-        result = session.post("https://api.codemao.cn/nemo/v2/works/" + workid +"/like")
-
-        def get():
-            return(result.text)
-
-        if result.status_code == 201:
-            if print == 'yes':
-                print("Like Successful[201]")
-            else:
-                return('201')
-        else:
-            if print == 'yes':
-                print("Like Failed["+str(result.status_code)+"]")
-            else:
-                return(str(result.status_code))
-
-def coll(workid,print='no'):
-        session = requests.Session()
-        result = session.post("https://api.codemao.cn/nemo/v2/works/" + workid +"/collection")
-        
-        def get():
-            return(result.text)
-        
-        if result.status_code == 201:
-            if print == 'yes':
-                print("Collection Successful[201]")
-            else:
-                return('201')
-        else:
-            if print == 'yes':
-                print("Collection Failed["+str(result.status_code)+"]")
-            else:
-                return(str(result.status_code))
-            
-def fork(workid,print='no'):
-        session = requests.Session()
-        result = session.post("https://api.codemao.cn/nemo/v2/works/" + workid +"/fork")
-
-        def get():
-            return(result.text)
-
-        if result.status_code == 201:
-            if print == 'yes':
-                print("Fork Successful[201]")
-            else:
-                return('201')
-        else:
-            if print == 'yes':
-                print("Fork Failed["+str(result.status_code)+"]")
-            else:
-                return(str(result.status_code))
+    if result.status_code == 204:
+        if print == 'yes':
+            print("Change Password Successful[204]")
+        else:
+            return ('204')
+    else:
+        if print == 'yes':
+            print("Change Password Failed[" + str(result.status_code) + "]")
+        else:
+            return (str(result.status_code))
+
+
+def like(workid, print='no'):
+
+    result = session.post("https://api.codemao.cn/nemo/v2/works/" + workid +
+                          "/like")
+    global get
+
+    def get():
+        return (result.text)
+
+    if result.status_code == 201:
+        if print == 'yes':
+            print("Like Successful[201]")
+        else:
+            return ('201')
+    else:
+        if print == 'yes':
+            print("Like Failed[" + str(result.status_code) + "]")
+        else:
+            return (str(result.status_code))
+
+
+def coll(workid, print='no'):
+
+    result = session.post("https://api.codemao.cn/nemo/v2/works/" + workid +
+                          "/collection")
+    global get
+
+    def get():
+        return (result.text)
+
+    if result.status_code == 201:
+        if print == 'yes':
+            print("Collection Successful[201]")
+        else:
+            return ('201')
+    else:
+        if print == 'yes':
+            print("Collection Failed[" + str(result.status_code) + "]")
+        else:
+            return (str(result.status_code))
+
+
+def fork(workid, print='no'):
+
+    result = session.post("https://api.codemao.cn/nemo/v2/works/" + workid +
+                          "/fork")
+    global get
+
+    def get():
+        return (result.text)
+
+    if result.status_code == 201:
+        if print == 'yes':
+            print("Fork Successful[201]")
+        else:
+            return ('201')
+    else:
+        if print == 'yes':
+            print("Fork Failed[" + str(result.status_code) + "]")
+        else:
+            return (str(result.status_code))
+
+
+def follow(userid, print='no'):
+
+    result = session.post("https://api.codemao.cn/nemo/v2/user/" + userid +
+                          "/follow")
+    global get
+    def get():
+        return (result.text)
+
+    if result.status_code == 204:
+        if print == 'yes':
+            print("Fork Successful[204]")
+        else:
+            return ('204')
+    else:
+        if print == 'yes':
+            print("Fork Failed[" + str(result.status_code) + "]")
+        else:
+            return (str(result.status_code))
```

### Comparing `epate-1.0.9/Epate.egg-info/PKG-INFO` & `epate-1.1.0/Epate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Epate
-Version: 1.0.9
+Version: 1.1.0
 Summary: A python library for many API of the codemao's website.
 Home-page: https://xiao.asia
 Author: xiaoxlh
 Author-email: xiaoxiaogzs@outlook.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `epate-1.0.9/LICENSE` & `epate-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `epate-1.0.9/PKG-INFO` & `epate-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Epate
-Version: 1.0.9
+Version: 1.1.0
 Summary: A python library for many API of the codemao's website.
 Home-page: https://xiao.asia
 Author: xiaoxlh
 Author-email: xiaoxiaogzs@outlook.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `epate-1.0.9/setup.py` & `epate-1.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,24 @@
 from setuptools import setup, find_packages
- 
+
 from pkg_resources import parse_requirements
 
 install_requires = ['requests==2.31.0']
- 
-setup(
-    name="Epate",
-    version="1.0.9",
-    author="xiaoxlh",
-    author_email="xiaoxiaogzs@outlook.com",
-    description="A python library for many API of the codemao's website.",
-    long_description="eds sdk for python",
-    license="Apache License, Version 2.0",
-    url="https://xiao.asia",
- 
-    classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Intended Audience :: Developers',
-        "Programming Language :: Python :: 3.12",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-    
-    packages=find_packages(),
-    install_requires=install_requires,
-    entry_points={
-        'console_scripts': [
-            'test = test.help:main'
-        ]
-    }
-)
+
+setup(name="Epate",
+      version="1.1.0",
+      author="xiaoxlh",
+      author_email="xiaoxiaogzs@outlook.com",
+      description="A python library for many API of the codemao's website.",
+      long_description="eds sdk for python",
+      license="Apache License, Version 2.0",
+      url="https://xiao.asia",
+      classifiers=[
+          'Development Status :: 3 - Alpha',
+          'Intended Audience :: Developers',
+          "Programming Language :: Python :: 3.12",
+          "License :: OSI Approved :: MIT License",
+          "Operating System :: OS Independent",
+      ],
+      packages=find_packages(),
+      install_requires=install_requires,
+      entry_points={'console_scripts': ['test = test.help:main']})
```


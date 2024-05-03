# Comparing `tmp/schubmult-1.3.5.tar.gz` & `tmp/schubmult-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schubmult-1.3.5.tar", last modified: Wed Apr 24 11:35:51 2024, max compression
+gzip compressed data, was "schubmult-1.3.6.tar", last modified: Fri May  3 18:01:59 2024, max compression
```

## Comparing `schubmult-1.3.5.tar` & `schubmult-1.3.6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-24 11:35:51.663000 schubmult-1.3.5/
--rwxrwxrwx   0 root         (0) root         (0)    35149 2023-09-24 17:08:26.000000 schubmult-1.3.5/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     5235 2024-04-24 11:35:51.611000 schubmult-1.3.5/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     4853 2024-04-15 14:05:16.000000 schubmult-1.3.5/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-24 11:35:48.869000 schubmult-1.3.5/schubmult/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-09-24 17:08:26.000000 schubmult-1.3.5/schubmult/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    16003 2024-04-12 18:48:00.000000 schubmult-1.3.5/schubmult/perm_lib.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-24 11:35:49.723000 schubmult-1.3.5/schubmult/schubmult_double/
--rwxrwxrwx   0 root         (0) root         (0)       41 2023-09-25 01:39:08.000000 schubmult-1.3.5/schubmult/schubmult_double/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       97 2023-09-26 17:55:50.000000 schubmult-1.3.5/schubmult/schubmult_double/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     4773 2024-04-10 12:45:13.000000 schubmult-1.3.5/schubmult/schubmult_double/schubmult_double.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-24 11:35:50.094000 schubmult-1.3.5/schubmult/schubmult_py/
--rwxrwxrwx   0 root         (0) root         (0)       36 2023-09-25 01:39:03.000000 schubmult-1.3.5/schubmult/schubmult_py/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       94 2023-09-26 17:55:38.000000 schubmult-1.3.5/schubmult/schubmult_py/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     4373 2024-04-10 12:45:06.000000 schubmult-1.3.5/schubmult/schubmult_py/schubmult_py.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-24 11:35:50.444000 schubmult-1.3.5/schubmult/schubmult_q/
--rwxrwxrwx   0 root         (0) root         (0)       36 2024-04-03 15:35:41.000000 schubmult-1.3.5/schubmult/schubmult_q/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       92 2024-04-03 15:28:43.000000 schubmult-1.3.5/schubmult/schubmult_q/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     9067 2024-04-21 14:28:57.000000 schubmult-1.3.5/schubmult/schubmult_q/schubmult_q.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-24 11:35:50.790000 schubmult-1.3.5/schubmult/schubmult_q_double/
--rwxrwxrwx   0 root         (0) root         (0)       33 2024-04-12 18:50:20.000000 schubmult-1.3.5/schubmult/schubmult_q_double/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       99 2024-04-12 18:49:31.000000 schubmult-1.3.5/schubmult/schubmult_q_double/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     3215 2024-04-15 14:01:00.000000 schubmult-1.3.5/schubmult/schubmult_q_double/schubmult_q_double.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-24 11:35:51.160000 schubmult-1.3.5/schubmult/schubmult_q_yz/
--rwxrwxrwx   0 root         (0) root         (0)       29 2024-04-12 18:49:56.000000 schubmult-1.3.5/schubmult/schubmult_q_yz/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       95 2024-04-12 18:49:43.000000 schubmult-1.3.5/schubmult/schubmult_q_yz/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     5863 2024-04-21 14:35:53.000000 schubmult-1.3.5/schubmult/schubmult_q_yz/schubmult_q_yz.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-24 11:35:51.536000 schubmult-1.3.5/schubmult/schubmult_yz/
--rwxrwxrwx   0 root         (0) root         (0)       27 2023-09-25 01:38:28.000000 schubmult-1.3.5/schubmult/schubmult_yz/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       93 2023-09-26 17:55:32.000000 schubmult-1.3.5/schubmult/schubmult_yz/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)    42460 2024-04-12 14:57:13.000000 schubmult-1.3.5/schubmult/schubmult_yz/schubmult_yz.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-24 11:35:49.362000 schubmult-1.3.5/schubmult.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     5235 2024-04-24 11:35:47.000000 schubmult-1.3.5/schubmult.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      978 2024-04-24 11:35:48.000000 schubmult-1.3.5/schubmult.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-24 11:35:47.000000 schubmult-1.3.5/schubmult.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)      353 2024-04-24 11:35:47.000000 schubmult-1.3.5/schubmult.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)       83 2024-04-24 11:35:47.000000 schubmult-1.3.5/schubmult.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       10 2024-04-24 11:35:47.000000 schubmult-1.3.5/schubmult.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       79 2024-04-24 11:35:51.645000 schubmult-1.3.5/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1243 2024-04-24 11:35:16.000000 schubmult-1.3.5/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 18:01:59.894000 schubmult-1.3.6/
+-rwxrwxrwx   0 root         (0) root         (0)    35149 2023-09-24 17:08:26.000000 schubmult-1.3.6/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     5235 2024-05-03 18:01:59.846000 schubmult-1.3.6/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     4853 2024-04-15 14:05:16.000000 schubmult-1.3.6/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 18:01:57.642000 schubmult-1.3.6/schubmult/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-09-24 17:08:26.000000 schubmult-1.3.6/schubmult/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    16320 2024-05-01 14:26:35.000000 schubmult-1.3.6/schubmult/perm_lib.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 18:01:58.350000 schubmult-1.3.6/schubmult/schubmult_double/
+-rwxrwxrwx   0 root         (0) root         (0)       41 2023-09-25 01:39:08.000000 schubmult-1.3.6/schubmult/schubmult_double/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       97 2023-09-26 17:55:50.000000 schubmult-1.3.6/schubmult/schubmult_double/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4773 2024-04-10 12:45:13.000000 schubmult-1.3.6/schubmult/schubmult_double/schubmult_double.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 18:01:58.627000 schubmult-1.3.6/schubmult/schubmult_py/
+-rwxrwxrwx   0 root         (0) root         (0)       36 2023-09-25 01:39:03.000000 schubmult-1.3.6/schubmult/schubmult_py/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       94 2023-09-26 17:55:38.000000 schubmult-1.3.6/schubmult/schubmult_py/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4373 2024-04-10 12:45:06.000000 schubmult-1.3.6/schubmult/schubmult_py/schubmult_py.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 18:01:58.941000 schubmult-1.3.6/schubmult/schubmult_q/
+-rwxrwxrwx   0 root         (0) root         (0)       36 2024-04-03 15:35:41.000000 schubmult-1.3.6/schubmult/schubmult_q/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       92 2024-04-03 15:28:43.000000 schubmult-1.3.6/schubmult/schubmult_q/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     9034 2024-05-01 11:44:33.000000 schubmult-1.3.6/schubmult/schubmult_q/schubmult_q.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 18:01:59.203000 schubmult-1.3.6/schubmult/schubmult_q_double/
+-rwxrwxrwx   0 root         (0) root         (0)       33 2024-04-12 18:50:20.000000 schubmult-1.3.6/schubmult/schubmult_q_double/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       99 2024-04-12 18:49:31.000000 schubmult-1.3.6/schubmult/schubmult_q_double/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3215 2024-04-15 14:01:00.000000 schubmult-1.3.6/schubmult/schubmult_q_double/schubmult_q_double.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 18:01:59.477000 schubmult-1.3.6/schubmult/schubmult_q_yz/
+-rwxrwxrwx   0 root         (0) root         (0)       29 2024-04-12 18:49:56.000000 schubmult-1.3.6/schubmult/schubmult_q_yz/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       95 2024-04-12 18:49:43.000000 schubmult-1.3.6/schubmult/schubmult_q_yz/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     8098 2024-05-03 15:03:11.000000 schubmult-1.3.6/schubmult/schubmult_q_yz/schubmult_q_yz.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 18:01:59.781000 schubmult-1.3.6/schubmult/schubmult_yz/
+-rwxrwxrwx   0 root         (0) root         (0)       27 2023-09-25 01:38:28.000000 schubmult-1.3.6/schubmult/schubmult_yz/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       93 2023-09-26 17:55:32.000000 schubmult-1.3.6/schubmult/schubmult_yz/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)    42460 2024-04-12 14:57:13.000000 schubmult-1.3.6/schubmult/schubmult_yz/schubmult_yz.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 18:01:58.069000 schubmult-1.3.6/schubmult.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     5235 2024-05-03 18:01:55.000000 schubmult-1.3.6/schubmult.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      978 2024-05-03 18:01:56.000000 schubmult-1.3.6/schubmult.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-03 18:01:55.000000 schubmult-1.3.6/schubmult.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)      353 2024-05-03 18:01:56.000000 schubmult-1.3.6/schubmult.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)       83 2024-05-03 18:01:56.000000 schubmult-1.3.6/schubmult.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       10 2024-05-03 18:01:56.000000 schubmult-1.3.6/schubmult.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       79 2024-05-03 18:01:59.878000 schubmult-1.3.6/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1243 2024-05-03 18:01:06.000000 schubmult-1.3.6/setup.py
```

### Comparing `schubmult-1.3.5/LICENSE` & `schubmult-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.5/PKG-INFO` & `schubmult-1.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schubmult
-Version: 1.3.5
+Version: 1.3.6
 Summary: Computing Littlewood-Richardson coefficients of Schubert polynomials
 Home-page: https://github.com/matthematics/schubmult
 Author: Matt Samuel
 Author-email: schubmult@gmail.com
 License: GNU
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `schubmult-1.3.5/README.md` & `schubmult-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.5/schubmult/perm_lib.py` & `schubmult-1.3.6/schubmult/perm_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,14 +135,27 @@
 						else:
 							new_perm_add = tuple(new_perm)
 						perm_list += [(new_perm_add,up_perm2[j])]
 						total_list+=[(new_perm_add,pp+1)]
 		up_perm_list = perm_list
 	return total_list
 
+def strict_theta(u):
+	ret = [*trimcode(u)]
+	did_one = True
+	while did_one:
+		did_one = False
+		for i in range(len(ret)-2,-1,-1):
+			if ret[i+1]!=0 and ret[i] <= ret[i+1]:
+				ret[i], ret[i+1] = ret[i+1] + 1, ret[i]
+				did_one = True
+				break
+	while len(ret)>0 and ret[-1] == 0:
+		ret.pop()
+	return ret
 
 def elem_sym_perms_q(orig_perm,p,k):	
 	total_list = [(orig_perm,0,1)]
 	up_perm_list = [(orig_perm,1,1000)]
 	for pp in range(p):
 		perm_list = []
 		for up_perm, val, last_j in up_perm_list:
```

### Comparing `schubmult-1.3.5/schubmult/schubmult_double/schubmult_double.py` & `schubmult-1.3.6/schubmult/schubmult_double/schubmult_double.py`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.5/schubmult/schubmult_py/schubmult_py.py` & `schubmult-1.3.6/schubmult/schubmult_py/schubmult_py.py`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.5/schubmult/schubmult_q/schubmult_q.py` & `schubmult-1.3.6/schubmult/schubmult_q/schubmult_q.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,15 @@
 for i in range(1,n):
 	sm = var_r[0]
 	for j in range(1,i):
 		sm += var_r[j]
 	subs_dict[var2[i]] = sm
 
 def schubmult(perm_dict,v):
-	vn1 = inverse(v)
-	th = [len(v)-i for i in range(1,len(v)+1)]	
+	th = strict_theta(inverse(v))
 	mu = permtrim(uncode(th))
 	vmu = permtrim(mulperm([*v],mu))
 	#print(f"{th=} {mu=} {vmu=}")
 	inv_vmu = inv(vmu)
 	inv_mu = inv(mu)
 	ret_dict = {}
 	vpaths = [([(vmu,0)],1)]
```

### Comparing `schubmult-1.3.5/schubmult/schubmult_q_double/schubmult_q_double.py` & `schubmult-1.3.6/schubmult/schubmult_q_double/schubmult_q_double.py`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.5/schubmult/schubmult_q_yz/schubmult_q_yz.py` & `schubmult-1.3.6/schubmult/schubmult_q_yz/schubmult_q_yz.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from schubmult.perm_lib import *
-from schubmult.schubmult_yz import compute_positive_rep
+from schubmult.schubmult_yz import compute_positive_rep, posify
 from symengine import *
 import sys
 
 
 #q_var = symarray("q",100)
 
 var2 = symarray("y",100)
@@ -11,15 +11,15 @@
 
 	
 
 	
 
 	
 def schubmult(perm_dict,v,var2=var2,var3=var3):
-	th = [len(v)-i for i in range(1,len(v))]
+	th = strict_theta(inverse(v))
 	mu = permtrim(uncode(th))
 	vmu = permtrim(mulperm([*v],mu))
 	inv_vmu = inv(vmu)
 	inv_mu = inv(mu)
 	ret_dict = {}
 	vpaths = [([(vmu,0)],1)]
 	while th[-1] == 0:
@@ -50,18 +50,72 @@
 							#print(f"{code(up2)=} {elem_sym_func_q(th[index],index+1,up,up2,v,v2,udiff,vdiff,var2,var3)=} {mul_val=} {sumval=}")							
 							newpathsums[up2][v2] = newpathsums[up2].get(v2,zero)+s*sumval*elem_sym_func_q(th[index],index+1,up,up2,v,v2,udiff,vdiff,var2,var3)
 			vpathsums = newpathsums
 		toget = tuple(vmu)
 		ret_dict = add_perm_dict({ep: vpathsums[ep].get(toget,0) for ep in vpathsums},ret_dict)
 	return ret_dict
 
+q_var2 = q_var.tolist()
+
+def sum_q_dict(q_dict1,q_dict2):
+	ret = {**q_dict1}
+	for key in q_dict2:
+		ret[key] = ret.get(key,0) + q_dict2[key]
+	return ret
+
+def mul_q_dict(q_dict1,q_dict2):
+	ret = {}
+	for key1 in q_dict1:
+		for key2 in q_dict2:
+			key3 = key1*key2
+			ret[key3] = ret.get(key3,0) + q_dict1[key1]*q_dict2[key2]
+	return ret
+
+def factor_out_q_keep_factored(poly):
+	ret = {}
+	if str(poly).find("q") == -1:
+		ret[1] = poly
+		return ret
+	elif poly in q_var2:
+		ret[poly] = 1
+		return ret
+	elif isinstance(poly,Add):
+		ag = poly.args
+		ret = factor_out_q_keep_factored(ag[0])
+		for i in range(1,len(ag)):
+			ret = sum_q_dict(ret,factor_out_q_keep_factored(ag[i]))
+		return ret
+	elif isinstance(poly,Mul):
+		ag = poly.args
+		ret = factor_out_q_keep_factored(ag[0])
+		for i in range(1,len(ag)):
+			ret = mul_q_dict(ret,factor_out_q_keep_factored(ag[i]))
+		return ret
+	elif isinstance(poly,Pow):
+		base = poly.args[0]
+		exponent = int(poly.args[1])
+		#print(f"exponent {exponent}")
+		work_val = factor_out_q_keep_factored(base)
+		ret = {1: 1}
+		while exponent > 0:
+			if exponent % 2 == 1:
+				if ret == {1: 1}:
+					ret = {**work_val}
+				else:
+					ret = mul_q_dict(ret,work_val)
+				exponent -= 1
+			else:
+				work_val = mul_q_dict(work_val,work_val)
+				exponent //= 2
+		return ret
+	return ret
+
 def factor_out_q(poly):
 	coeff_dict = expand(poly).as_coefficients_dict()
-	ret = {}
-	q_var2 = q_var.tolist()
+	ret = {}	
 	for key in coeff_dict:
 		coeff = coeff_dict[key]
 		if coeff == 0:
 			continue
 		q_part = 1
 		yz_part = coeff
 		if isinstance(key,Mul):
@@ -88,15 +142,18 @@
 			if key in q_var2:
 				q_part *= key
 			else:
 				yz_part*=key
 			
 		ret[q_part] = ret.get(q_part,0) + yz_part
 	return ret
-	
+
+var2_t = tuple(var2.tolist())
+var3_t = tuple(var3.tolist())	
+
 def main():
 	global var2
 	try:
 		sys.setrecursionlimit(1000000)
 	
 		perms=[]
 		curperm = []
@@ -175,27 +232,43 @@
 					notint = False
 					try:
 						int(val)
 					except Exception:
 						notint = True
 						val2 = 0
 						if display_positive:
-							q_dict = factor_out_q(val)
+							q_dict = factor_out_q_keep_factored(val)
 							for q_part in q_dict:
 								#print(f"{q_part=} {q_dict[q_part]=}")
 								try:
 									val2 += q_part*int(q_dict[q_part])
 								except Exception:
 									try:
-										val2 += q_part*compute_positive_rep(q_dict[q_part],var2,var3,msg,False)
-									except TypeError:
-										print(f"error; write to schubmult@gmail.com with the case {perms=} {perm=} {val=} {check_coeff_dict.get(perm,0)=}")
+										if len(perms) == 2 and q_part == 1:
+											u = permtrim([*perms[0]])
+											v = permtrim([*perms[1]])
+											val2 += posify(q_dict[q_part],tuple(u),tuple(v),perm,var2_t,var3_t,msg,False)
+										elif len(perms) == 2 and q_part in q_var2:
+											i = q_var2.index(q_part)
+											u = permtrim([*perms[0]])
+											v = permtrim([*perms[1]])											
+											#print(f"{u=} {v=} {q_part=} {q_dict[q_part]=}")
+											if i<len(u) and i<len(v) and u[i-1]>u[i] and v[i-1]>v[i]:
+												u[i], u[i-1] = u[i-1], u[i]
+												v[i], v[i-1] = v[i-1], v[i]
+												#print(f"new {u=} {v=}")
+												val2 += q_part*posify(q_dict[q_part],tuple(permtrim(u)),tuple(permtrim(v)),perm,var2_t,var3_t,msg,False)
+										else:
+											val2 += q_part*compute_positive_rep(q_dict[q_part],var2_t,var3_t,msg,False)
+									except Exception as e:
+										print(f"error; write to schubmult@gmail.com with the case {perms=} {perm=} {val=} {coeff_dict.get(perm,0)=}")
+										print(f"Exception: {e}")
 										exit(1)
 							if check and expand(val - val2)!=0:
-								print(f"error; write to schubmult@gmail.com with the case {perms=} {perm=} {val=} {check_coeff_dict.get(perm,0)=}")
+								print(f"error: value not equal; write to schubmult@gmail.com with the case {perms=} {perm=} {val=} {coeff_dict.get(perm,0)=}")
 								exit(1)
 							val = val2
 					if val!=0:
 						if ascode:
 							print(f"{str(trimcode(perm)):>{width}}  {str(val).replace('**','^').replace('*',' ')}")	
 						else:
 							print(f"{str(perm):>{width}}  {str(val).replace('**','^').replace('*',' ')}")
```

### Comparing `schubmult-1.3.5/schubmult/schubmult_yz/schubmult_yz.py` & `schubmult-1.3.6/schubmult/schubmult_yz/schubmult_yz.py`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.5/schubmult.egg-info/PKG-INFO` & `schubmult-1.3.6/schubmult.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schubmult
-Version: 1.3.5
+Version: 1.3.6
 Summary: Computing Littlewood-Richardson coefficients of Schubert polynomials
 Home-page: https://github.com/matthematics/schubmult
 Author: Matt Samuel
 Author-email: schubmult@gmail.com
 License: GNU
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `schubmult-1.3.5/schubmult.egg-info/SOURCES.txt` & `schubmult-1.3.6/schubmult.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.5/setup.py` & `schubmult-1.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="schubmult",
-    version="1.3.5",
+    version="1.3.6",
     description="Computing Littlewood-Richardson coefficients of Schubert polynomials",
 	long_description=long_description,
 	long_description_content_type='text/markdown',
     url="https://github.com/matthematics/schubmult",
     author="Matt Samuel",
     author_email="schubmult@gmail.com",
     license="GNU",
```


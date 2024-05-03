# Comparing `tmp/caluxpy_fi-0.1.45.tar.gz` & `tmp/caluxpy_fi-0.1.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caluxpy_fi-0.1.45.tar", last modified: Thu Apr 25 14:36:19 2024, max compression
+gzip compressed data, was "caluxpy_fi-0.1.46.tar", last modified: Fri May  3 21:09:27 2024, max compression
```

## Comparing `caluxpy_fi-0.1.45.tar` & `caluxpy_fi-0.1.46.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 14:36:19.204762 caluxpy_fi-0.1.45/
--rw-rw-rw-   0        0        0     1106 2024-03-18 20:26:44.000000 caluxpy_fi-0.1.45/LICENSE.txt
--rw-rw-rw-   0        0        0     4738 2024-04-25 14:36:19.204762 caluxpy_fi-0.1.45/PKG-INFO
--rw-rw-rw-   0        0        0     2724 2024-01-12 17:32:24.000000 caluxpy_fi-0.1.45/README.md
--rw-rw-rw-   0        0        0      824 2024-04-25 14:35:28.000000 caluxpy_fi-0.1.45/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-25 14:36:19.204762 caluxpy_fi-0.1.45/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-25 14:36:19.059256 caluxpy_fi-0.1.45/src/
-drwxrwxrwx   0        0        0        0 2024-04-25 14:36:19.186465 caluxpy_fi-0.1.45/src/caluxPy_fi/
--rw-rw-rw-   0        0        0    15447 2024-03-15 20:06:16.000000 caluxpy_fi-0.1.45/src/caluxPy_fi/Convexity.py
--rw-rw-rw-   0        0        0     1189 2024-01-19 17:22:58.000000 caluxpy_fi-0.1.45/src/caluxPy_fi/DataBase.py
--rw-rw-rw-   0        0        0     4225 2024-03-18 22:03:06.000000 caluxpy_fi-0.1.45/src/caluxPy_fi/ExternalImport.py
--rw-rw-rw-   0        0        0    10561 2024-03-19 16:45:38.000000 caluxpy_fi-0.1.45/src/caluxPy_fi/ExternalImport2.py
--rw-rw-rw-   0        0        0    56622 2024-04-25 14:35:17.000000 caluxpy_fi-0.1.45/src/caluxPy_fi/FixedIncome.py
--rw-rw-rw-   0        0        0     5926 2024-03-21 21:15:39.000000 caluxpy_fi-0.1.45/src/caluxPy_fi/Multiple.py
--rw-rw-rw-   0        0        0    13098 2024-03-14 14:13:38.000000 caluxpy_fi-0.1.45/src/caluxPy_fi/Portfolio.py
--rw-rw-rw-   0        0        0    12223 2024-03-21 21:17:02.000000 caluxpy_fi-0.1.45/src/caluxPy_fi/Support.py
--rw-rw-rw-   0        0        0     5887 2024-03-14 13:56:00.000000 caluxpy_fi-0.1.45/src/caluxPy_fi/UserInputs.py
--rw-rw-rw-   0        0        0       28 2024-01-11 15:43:14.000000 caluxpy_fi-0.1.45/src/caluxPy_fi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 14:36:19.204762 caluxpy_fi-0.1.45/src/caluxPy_fi.egg-info/
--rw-rw-rw-   0        0        0     4738 2024-04-25 14:36:19.000000 caluxpy_fi-0.1.45/src/caluxPy_fi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      514 2024-04-25 14:36:19.000000 caluxpy_fi-0.1.45/src/caluxPy_fi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 14:36:19.000000 caluxpy_fi-0.1.45/src/caluxPy_fi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      119 2024-04-25 14:36:19.000000 caluxpy_fi-0.1.45/src/caluxPy_fi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-25 14:36:19.000000 caluxpy_fi-0.1.45/src/caluxPy_fi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-03 21:09:27.518279 caluxpy_fi-0.1.46/
+-rw-rw-rw-   0        0        0     1106 2024-03-18 20:26:44.000000 caluxpy_fi-0.1.46/LICENSE.txt
+-rw-rw-rw-   0        0        0     4738 2024-05-03 21:09:27.518279 caluxpy_fi-0.1.46/PKG-INFO
+-rw-rw-rw-   0        0        0     2724 2024-01-12 17:32:24.000000 caluxpy_fi-0.1.46/README.md
+-rw-rw-rw-   0        0        0      824 2024-05-03 21:05:47.000000 caluxpy_fi-0.1.46/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-03 21:09:27.518279 caluxpy_fi-0.1.46/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-03 21:09:27.345389 caluxpy_fi-0.1.46/src/
+drwxrwxrwx   0        0        0        0 2024-05-03 21:09:27.487545 caluxpy_fi-0.1.46/src/caluxPy_fi/
+-rw-rw-rw-   0        0        0    16591 2024-05-03 21:05:13.000000 caluxpy_fi-0.1.46/src/caluxPy_fi/Convexity.py
+-rw-rw-rw-   0        0        0     1189 2024-04-30 15:52:50.000000 caluxpy_fi-0.1.46/src/caluxPy_fi/DataBase.py
+-rw-rw-rw-   0        0        0     4225 2024-03-18 22:03:06.000000 caluxpy_fi-0.1.46/src/caluxPy_fi/ExternalImport.py
+-rw-rw-rw-   0        0        0    10561 2024-03-19 16:45:38.000000 caluxpy_fi-0.1.46/src/caluxPy_fi/ExternalImport2.py
+-rw-rw-rw-   0        0        0    56544 2024-05-02 13:32:57.000000 caluxpy_fi-0.1.46/src/caluxPy_fi/FixedIncome.py
+-rw-rw-rw-   0        0        0     5926 2024-03-21 21:15:39.000000 caluxpy_fi-0.1.46/src/caluxPy_fi/Multiple.py
+-rw-rw-rw-   0        0        0    13098 2024-03-14 14:13:38.000000 caluxpy_fi-0.1.46/src/caluxPy_fi/Portfolio.py
+-rw-rw-rw-   0        0        0    12223 2024-03-21 21:17:02.000000 caluxpy_fi-0.1.46/src/caluxPy_fi/Support.py
+-rw-rw-rw-   0        0        0     5887 2024-03-14 13:56:00.000000 caluxpy_fi-0.1.46/src/caluxPy_fi/UserInputs.py
+-rw-rw-rw-   0        0        0       28 2024-01-11 15:43:14.000000 caluxpy_fi-0.1.46/src/caluxPy_fi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 21:09:27.509772 caluxpy_fi-0.1.46/src/caluxPy_fi.egg-info/
+-rw-rw-rw-   0        0        0     4738 2024-05-03 21:09:27.000000 caluxpy_fi-0.1.46/src/caluxPy_fi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      514 2024-05-03 21:09:27.000000 caluxpy_fi-0.1.46/src/caluxPy_fi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 21:09:27.000000 caluxpy_fi-0.1.46/src/caluxPy_fi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2024-05-03 21:09:27.000000 caluxpy_fi-0.1.46/src/caluxPy_fi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-03 21:09:27.000000 caluxpy_fi-0.1.46/src/caluxPy_fi.egg-info/top_level.txt
```

### Comparing `caluxpy_fi-0.1.45/LICENSE.txt` & `caluxpy_fi-0.1.46/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.45/PKG-INFO` & `caluxpy_fi-0.1.46/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caluxPy_fi
-Version: 0.1.45
+Version: 0.1.46
 Summary: Fixed Income Valuation and Analysis
 Author-email: Luis Manuel Tavarez Valenzuela <luima2494@gmail.com>
 Maintainer-email: Luis Manuel Tavarez Valenzuela <luima2494@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Luis Manuel Tavarez Valenzuela
```

### Comparing `caluxpy_fi-0.1.45/README.md` & `caluxpy_fi-0.1.46/README.md`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.45/pyproject.toml` & `caluxpy_fi-0.1.46/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69.2.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "caluxPy_fi"
-version = "0.1.45"
+version = "0.1.46"
 authors = [
   { name = "Luis Manuel Tavarez Valenzuela", email = "luima2494@gmail.com" }
 ]
 maintainers = [
   { name = "Luis Manuel Tavarez Valenzuela", email = "luima2494@gmail.com" }
 ]
 description = "Fixed Income Valuation and Analysis"
```

### Comparing `caluxpy_fi-0.1.45/src/caluxPy_fi/Convexity.py` & `caluxpy_fi-0.1.46/src/caluxPy_fi/Convexity.py`

 * *Files 10% similar despite different names*

```diff
@@ -124,32 +124,56 @@
             resValuation = self.presentValue(current_coupon, nper, w_coupon, discrepancy, coupon_type, maturity_date, expected_maturity, coupon_days, ytm2, periodicity, coupon_flow, payment_type, issuer, notional_value, gained_coupon)
             listPBS.append(y)
             listytms.append(ytm2)
             listCleanPrice.append(resValuation[4] * 100)
             listDirtyPrice.append(resValuation[1] * 100)
             listDuracion.append(resValuation[3])
             listModDuration.append(resValuation[5])
-            dv01 = (resValuation[5] / 100) * (resValuation[1]) * (notional_value / 100)
-            listDV01.append(dv01)
-            dicDV01[y] = dv01
+            #dv01 = (resValuation[5] / 100) * (resValuation[1]) * (notional_value / 100)
+            #listDV01.append(dv01)
+            #dicDV01[y] = dv01
             y += 1
         listPBS = np.array(listPBS)
         listytms = np.array(listytms)
         listCleanPrice = np.array(listCleanPrice)
         listDirtyPrice = np.array(listDirtyPrice)
         listDuracion = np.array(listDuracion)
         listModDuration = np.array(listModDuration)
-        listDV01 = np.array(listDV01)
-        self.df_convex = pd.DataFrame({'pbs': listPBS, 'dv01': listDV01})
-        self.df_convex['Negative'] = self.df_convex['pbs'] < 0
-        max_values_by_category = self.df_convex.groupby('Negative')['dv01'].max()
-        avg_values_by_category = self.df_convex.groupby('Negative')['dv01'].mean()
-        std_values_by_category = self.df_convex.groupby('Negative')['dv01'].std()
+        #listDV01 = np.array(listDV01)
+        self.df_convex = pd.DataFrame({'pbs': listPBS, 'Price': listDirtyPrice})
+        
+        # Treatment of the negatives in the df
+        negatives = self.df_convex[self.df_convex['pbs'] <= 0].copy()
+        negatives.sort_values(by = 'pbs', ascending = False, inplace = True)
+        negatives['dv01'] = negatives['Precio Sucio'].diff().fillna(0) * 10000
+        negatives['accum'] = negatives['dv01'].cumsum()
+        negatives.sort_values(by = 'pbs', ascending = True, inplace = True)
+        first_neg = negatives.iloc[-2]['dv01']
+        
+        # Treatment of the positives in the df
+        positives = self.df_convex[self.df_convex['pbs'] >= 0].copy()
+        positives.sort_values(by = 'pbs', ascending = True, inplace = True)
+        positives['dv01'] = positives['Precio Sucio'].diff().fillna(0) * -10000
+        positives['accum'] = positives['dv01'].cumsum()
+        first_pos = positives.iloc[1]['dv01']   
+        
+        # Getting the average
+        avg = (first_neg + first_pos) / 2
+        
+        #Concatenating the dfs to form the complete one
+        final = pd.concat([negatives, positives])
+        final.reset_index(drop = True, inplace = True)
+        self.df_convex['dv01'] = final['dv01']
+        
+        final['Negative'] = final['Stress Pbs'] < 0
+        max_values_by_category = final.groupby('Negative')['dv01'].max()
+        avg_values_by_category = final.groupby('Negative')['dv01'].mean()
+        std_values_by_category = final.groupby('Negative')['dv01'].std()
 
-        self.neg_vals = self.df_convex.groupby('Negative')
+        #self.neg_vals = final.groupby('Negative')
 
         self._logger.info(f'{self.df_convex}\n\n--------------------------------------------------------------------------------------------------------------------------------------\n')
         if self._lang == 'eng':
             self._logger.info(f'Max Values by Category -> {max_values_by_category}')
             self._logger.info(f'Average Values by Category -> {max_values_by_category}')
             self._logger.info(f'Standard Deviations by Category -> {max_values_by_category}\n\n--------------------------------------------------------------------------------------------------------------------------------------\n')
         elif self._lang == 'esp':
@@ -180,28 +204,28 @@
             self._logger.info(f'Desviación Estándar en Perdidas -> {self.std_loss}\n\n--------------------------------------------------------------------------------------------------------------------------------------\n')
     
         i = 0
         while i <= int(bps):
             if i == 0:
                 listConvexity.append(0)
             else:
-                listConvexity.append(listConvexity[i - 1] - dicDV01[i])
+                listConvexity.append(listConvexity[i - 1] - final['dv01'][i])
             i += 1
         i = -1
         while i >= -int(bps):
             if i == -1:
-                listConvexity.append(dicDV01[i])
+                listConvexity.append(final['dv01'][i])
             else:
-                listConvexity.append(listConvexity[-1] + dicDV01[i])
+                listConvexity.append(listConvexity[-1] + final['dv01'][i])
             i -= 1
         listConvexity = np.array(listConvexity)
         listConvexity[::-1].sort()
         i = -int(bps)
         while i <= int(bps):
-            listDuration2.append(dicDV01[0] * (0 - i))
+            listDuration2.append(final['dv01'][0] * (0 - i))
             i += 1
         listDuration2 = np.array(listDuration2)
 
         self.chart_data['x'] = listPBS
         self.chart_data['y1'] = listDuration2
         self.chart_data['y2'] = listConvexity
```

### Comparing `caluxpy_fi-0.1.45/src/caluxPy_fi/DataBase.py` & `caluxpy_fi-0.1.46/src/caluxPy_fi/DataBase.py`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.45/src/caluxPy_fi/ExternalImport.py` & `caluxpy_fi-0.1.46/src/caluxPy_fi/ExternalImport.py`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.45/src/caluxPy_fi/ExternalImport2.py` & `caluxpy_fi-0.1.46/src/caluxPy_fi/ExternalImport2.py`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.45/src/caluxPy_fi/FixedIncome.py` & `caluxpy_fi-0.1.46/src/caluxPy_fi/FixedIncome.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,72 +102,66 @@
                     self.expected_maturity = self.expectedMaturity(maturity_date = self.maturity_date, 
                                                                    issuance_date = self.issuance_date, 
                                                                    years_to_maturity = self._years_to_maturity,
                                                                    nper = self._per)
                 except Exception as e: self._logger.error(f'Error calculating expected maturity => {e}')
 
                 #This is the determination of the existence of a discrepancy between the maturity date and the expected maturity date
-                if (self.maturity_date.day - self.issuance_date.day) != 0 or self.maturity_date != self.expected_maturity:
-                    self._discrepancy = "Yes"
-                else:
-                    self._discrepancy = "No"
+                self._discrepancy = "Yes" if (self.maturity_date.day - self.issuance_date.day) != 0 or self.maturity_date != self.expected_maturity else 'No'
                     
                 if self.coupon_type == 'normal':
                     self.forward_date = None
                 elif coupon_type in ['fw1', 'fw2']:
                     #self.forward_date = datetime(self.maturity_date.year - math.trunc(self._years_to_maturity),self.maturity_date.month,self.maturity_date.day,0,0).date()
                     try:
                         self.forward_date = Support.get_date_years_ago(self.maturity_date, self._years_to_maturity)
                     except Exception as e:
                         self._logger.error(f'Error calculating a forward date => {e}')
                 else:
                     self.forward_date = forward_date
-                    if self.forward_date != '': 
+                    if not self.forward_date in ['', None]: 
                         try:
                             if type(forward_date) == str: self.forward_date = datetime.strptime(forward_date, self.date_format).date()
                         except ValueError as e:
                             self._logger.error(e)    
                     else:
                         self._logger.error('Forward date not specified!') 
                         raise Exception('Forward date not specified!')
                         
                 #If the security if of bullet type then any attribute of amortizable is deleted to avoid incongruencies
                 if self.payment_type == 'bullet':
-                    self.amortization_start_date = None
-                    self.amortization_periods = None
-                    self.amortization_periodicity = None
-                    self.amortizable_percentage = None
+                    self.amortization_start_date, self.amortization_periods, self.amortization_periodicity, self.amortizable_percentage = None, None, None, None
                 else:
                     #If not bullet then all the attributes are kept and verified
                     self.amortization_start_date = amortization_start_date
                     self._logger.info(f'Amortization Date -> {self.amortization_start_date} Type => {type(self.amortization_start_date)}')
-                    if self.amortization_start_date != '':
+                    if not self.amortization_start_date in ['', None]:
                         try:
                             if type(self.amortization_start_date) == str: self.amortization_start_date = datetime.strptime(self.amortization_start_date, self.date_format).date()
                             self._logger.info(f'Amortization Date -> {self.amortization_start_date} Type => {type(self.amortization_start_date)}')
                         except ValueError as e: self._logger.error(e)
                     else: 
                         self._logger.error('Amortization date not specified!') 
                         raise Exception('Amortization date not specified!')
                         
-                    if amortization_periods != '':
+                    if not amortization_periods in ['', None]:
                         self.amortization_periods = int(amortization_periods)
                     else:
                         self._logger.error('Amortization periods not specified!') 
                         raise Exception('Amortization periods not specified!')
                     
-                    if amortization_periodicity != '':
+                    if not amortization_periodicity in ['', None]:
                         try:
                             self.amortization_periodicity = Support.periodicityConversion(per = amortization_periodicity, mode = 'amortization')
                         except Exception as e: self._logger.error(f'Error converting amortization periodicity => {e}')
                     else:
                         self._logger.error('Amortization periodicity not specified!') 
                         raise Exception('Amortization periodicity not specified!')
                     
-                    if amortizable_percentage != '':
+                    if not amortizable_percentage in ['', None]:
                         try:
                             self.amortizable_percentage = Support.rateConversion(rate = amortizable_percentage)
                         except Exception as e: self._logger.error(f'Error converting amortization rate => {e}')
                     else:
                         self._logger.error('Amortization percentage not specified!') 
                         raise Exception('Amortization percentage not specified!')
```

### Comparing `caluxpy_fi-0.1.45/src/caluxPy_fi/Multiple.py` & `caluxpy_fi-0.1.46/src/caluxPy_fi/Multiple.py`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.45/src/caluxPy_fi/Portfolio.py` & `caluxpy_fi-0.1.46/src/caluxPy_fi/Portfolio.py`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.45/src/caluxPy_fi/Support.py` & `caluxpy_fi-0.1.46/src/caluxPy_fi/Support.py`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.45/src/caluxPy_fi/UserInputs.py` & `caluxpy_fi-0.1.46/src/caluxPy_fi/UserInputs.py`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.45/src/caluxPy_fi.egg-info/PKG-INFO` & `caluxpy_fi-0.1.46/src/caluxPy_fi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caluxPy_fi
-Version: 0.1.45
+Version: 0.1.46
 Summary: Fixed Income Valuation and Analysis
 Author-email: Luis Manuel Tavarez Valenzuela <luima2494@gmail.com>
 Maintainer-email: Luis Manuel Tavarez Valenzuela <luima2494@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Luis Manuel Tavarez Valenzuela
```

### Comparing `caluxpy_fi-0.1.45/src/caluxPy_fi.egg-info/SOURCES.txt` & `caluxpy_fi-0.1.46/src/caluxPy_fi.egg-info/SOURCES.txt`

 * *Files identical despite different names*


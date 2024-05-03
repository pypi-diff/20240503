# Comparing `tmp/mastsel-1.2.7.tar.gz` & `tmp/mastsel-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mastsel-1.2.7.tar", last modified: Tue Apr 16 14:29:54 2024, max compression
+gzip compressed data, was "mastsel-1.2.8.tar", last modified: Fri May  3 14:03:27 2024, max compression
```

## Comparing `mastsel-1.2.7.tar` & `mastsel-1.2.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:29:54.659911 mastsel-1.2.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:29:54.651910 mastsel-1.2.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:29:54.655911 mastsel-1.2.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-16 14:29:45.000000 mastsel-1.2.7/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-16 14:29:45.000000 mastsel-1.2.7/.github/workflows/run_tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-16 14:29:45.000000 mastsel-1.2.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-16 14:29:45.000000 mastsel-1.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-16 14:29:45.000000 mastsel-1.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-16 14:29:54.659911 mastsel-1.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-16 14:29:45.000000 mastsel-1.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:29:54.655911 mastsel-1.2.7/mastsel/
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-16 14:29:45.000000 mastsel-1.2.7/mastsel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-16 14:29:54.000000 mastsel-1.2.7/mastsel/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-16 14:29:45.000000 mastsel-1.2.7/mastsel/ini_to_yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)    26605 2024-04-16 14:29:45.000000 mastsel-1.2.7/mastsel/mavisFormulas.py
--rw-r--r--   0 runner    (1001) docker     (127)    64522 2024-04-16 14:29:45.000000 mastsel-1.2.7/mastsel/mavisLO.py
--rw-r--r--   0 runner    (1001) docker     (127)     6165 2024-04-16 14:29:45.000000 mastsel-1.2.7/mastsel/mavisParams.py
--rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-04-16 14:29:45.000000 mastsel-1.2.7/mastsel/mavisParamsOld.py
--rw-r--r--   0 runner    (1001) docker     (127)    13555 2024-04-16 14:29:45.000000 mastsel-1.2.7/mastsel/mavisPsf.py
--rw-r--r--   0 runner    (1001) docker     (127)     9155 2024-04-16 14:29:45.000000 mastsel-1.2.7/mastsel/mavisUtilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:29:54.659911 mastsel-1.2.7/mastsel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-16 14:29:54.000000 mastsel-1.2.7/mastsel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-16 14:29:54.000000 mastsel-1.2.7/mastsel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 14:29:54.000000 mastsel-1.2.7/mastsel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-16 14:29:54.000000 mastsel-1.2.7/mastsel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-16 14:29:54.000000 mastsel-1.2.7/mastsel.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:29:54.659911 mastsel-1.2.7/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-16 14:29:45.000000 mastsel-1.2.7/notebooks/MAVIS-CONVOLUTION-TEST.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-04-16 14:29:45.000000 mastsel-1.2.7/notebooks/MAVIS-CONVOLUTION.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10266 2024-04-16 14:29:45.000000 mastsel-1.2.7/notebooks/MAVIS.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10100 2024-04-16 14:29:45.000000 mastsel-1.2.7/notebooks/MAVIS2.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-04-16 14:29:45.000000 mastsel-1.2.7/notebooks/MAVIS3.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7064 2024-04-16 14:29:45.000000 mastsel-1.2.7/notebooks/MAVIS_INT_REC.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-04-16 14:29:45.000000 mastsel-1.2.7/notebooks/MAVIS_MAIN.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-16 14:29:45.000000 mastsel-1.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 14:29:54.659911 mastsel-1.2.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:29:54.659911 mastsel-1.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7556 2024-04-16 14:29:45.000000 mastsel-1.2.7/tests/allTests.py
--rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-04-16 14:29:45.000000 mastsel-1.2.7/tests/testTfOpt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:03:27.100653 mastsel-1.2.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:03:27.092653 mastsel-1.2.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:03:27.096653 mastsel-1.2.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-03 14:03:16.000000 mastsel-1.2.8/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-03 14:03:16.000000 mastsel-1.2.8/.github/workflows/run_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-03 14:03:16.000000 mastsel-1.2.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-03 14:03:16.000000 mastsel-1.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-03 14:03:16.000000 mastsel-1.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-03 14:03:27.100653 mastsel-1.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-03 14:03:16.000000 mastsel-1.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:03:27.096653 mastsel-1.2.8/mastsel/
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-03 14:03:16.000000 mastsel-1.2.8/mastsel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-03 14:03:26.000000 mastsel-1.2.8/mastsel/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-03 14:03:16.000000 mastsel-1.2.8/mastsel/ini_to_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26605 2024-05-03 14:03:16.000000 mastsel-1.2.8/mastsel/mavisFormulas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65625 2024-05-03 14:03:16.000000 mastsel-1.2.8/mastsel/mavisLO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6165 2024-05-03 14:03:16.000000 mastsel-1.2.8/mastsel/mavisParams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-05-03 14:03:16.000000 mastsel-1.2.8/mastsel/mavisParamsOld.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13555 2024-05-03 14:03:16.000000 mastsel-1.2.8/mastsel/mavisPsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9155 2024-05-03 14:03:16.000000 mastsel-1.2.8/mastsel/mavisUtilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:03:27.100653 mastsel-1.2.8/mastsel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-03 14:03:26.000000 mastsel-1.2.8/mastsel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-03 14:03:27.000000 mastsel-1.2.8/mastsel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 14:03:26.000000 mastsel-1.2.8/mastsel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-03 14:03:26.000000 mastsel-1.2.8/mastsel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-03 14:03:26.000000 mastsel-1.2.8/mastsel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:03:27.100653 mastsel-1.2.8/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-05-03 14:03:16.000000 mastsel-1.2.8/notebooks/MAVIS-CONVOLUTION-TEST.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-05-03 14:03:16.000000 mastsel-1.2.8/notebooks/MAVIS-CONVOLUTION.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10266 2024-05-03 14:03:16.000000 mastsel-1.2.8/notebooks/MAVIS.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10100 2024-05-03 14:03:16.000000 mastsel-1.2.8/notebooks/MAVIS2.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-05-03 14:03:16.000000 mastsel-1.2.8/notebooks/MAVIS3.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7064 2024-05-03 14:03:16.000000 mastsel-1.2.8/notebooks/MAVIS_INT_REC.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-05-03 14:03:16.000000 mastsel-1.2.8/notebooks/MAVIS_MAIN.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-03 14:03:16.000000 mastsel-1.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 14:03:27.100653 mastsel-1.2.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:03:27.100653 mastsel-1.2.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7556 2024-05-03 14:03:16.000000 mastsel-1.2.8/tests/allTests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-05-03 14:03:16.000000 mastsel-1.2.8/tests/testTfOpt.py
```

### Comparing `mastsel-1.2.7/.github/workflows/publish.yml` & `mastsel-1.2.8/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `mastsel-1.2.7/.github/workflows/run_tests.yml` & `mastsel-1.2.8/.github/workflows/run_tests.yml`

 * *Files identical despite different names*

### Comparing `mastsel-1.2.7/.gitignore` & `mastsel-1.2.8/.gitignore`

 * *Files identical despite different names*

### Comparing `mastsel-1.2.7/LICENSE` & `mastsel-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mastsel-1.2.7/PKG-INFO` & `mastsel-1.2.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mastsel
-Version: 1.2.7
+Version: 1.2.8
 Summary: Asterism Selection for MAVIS instrument
 Author-email: Fabio Rossi <fabio.rossi@inaf.it>
 License: MIT License
 Project-URL: repository, https://github.com/astro-tiptop/MASTSEL
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mastsel-1.2.7/README.md` & `mastsel-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `mastsel-1.2.7/mastsel/__init__.py` & `mastsel-1.2.8/mastsel/__init__.py`

 * *Files identical despite different names*

### Comparing `mastsel-1.2.7/mastsel/ini_to_yaml.py` & `mastsel-1.2.8/mastsel/ini_to_yaml.py`

 * *Files identical despite different names*

### Comparing `mastsel-1.2.7/mastsel/mavisFormulas.py` & `mastsel-1.2.8/mastsel/mavisFormulas.py`

 * *Files identical despite different names*

### Comparing `mastsel-1.2.7/mastsel/mavisLO.py` & `mastsel-1.2.8/mastsel/mavisLO.py`

 * *Files 1% similar despite different names*

```diff
@@ -239,15 +239,15 @@
         self.SensorFrameRate_LO = frequency
         self.maxLOtFreq = 0.5*self.SensorFrameRate_LO
         if self.check_config_key('telescope','windPsdFile'):
             windPsdFile = self.get_config_value('telescope','windPsdFile')
             self.psd_freq, self.psd_tip_wind, self.psd_tilt_wind = self.loadWindPsd(windPsdFile)
         else:
             if self.verbose:
-                print('No windPsdFile file is set.')
+                print('    WARNING: no windPsdFile file is set.')
             self.psd_freq = np.asarray(np.linspace(0.5, self.maxLOtFreq, int(2*self.maxLOtFreq)))
             self.psd_tip_wind = np.zeros((int(2*self.maxLOtFreq)))
             self.psd_tilt_wind = np.zeros((int(2*self.maxLOtFreq)))
 
         self.fTipS_LO, self.fTiltS_LO = self.specializedNoiseFuncs()
         self.fTipS, self.fTiltS = self.specializedWindFuncs()
         self.aFunctionM, self.expr0M = self.specializedMeanVarFormulas('truncatedMeanComponents')
@@ -736,15 +736,15 @@
             ax2.set_ylabel('Power')
         
         resultTip = xp.absolute((xp.sum(self.fTipS_lambda1( g0g_ext, psd_freq_ext, psd_tip_turb_ext), axis=(1)) ) )
         resultTilt = xp.absolute((xp.sum(self.fTiltS_lambda1( g0g_ext, psd_freq_ext, psd_tilt_turb_ext), axis=(1)) ) )
         minTipIdx = xp.where(resultTip == xp.nanmin(resultTip))
         minTiltIdx = xp.where(resultTilt == xp.nanmin(resultTilt))
         if self.verbose:
-            print('         best tip & tilt gain (noise):',g0g[minTipIdx[0][0]],g0g[minTiltIdx[0][0]])
+            print('    best tip & tilt gain (noise):', "%.3f" % g0g[minTipIdx[0][0]], "%.3f" % g0g[minTiltIdx[0][0]])
         if alib==gpulib and gpuEnabled:
             return cp.asnumpy(resultTip[minTipIdx[0][0]]), cp.asnumpy(resultTilt[minTiltIdx[0][0]])
         else:
             return (resultTip[minTipIdx[0][0]], resultTilt[minTiltIdx[0][0]])
 
     def computeFocusNoiseResidual(self, fmin, fmax, freq_samples, varX, bias, alib):
         npoints = 99
@@ -786,15 +786,15 @@
             # when the noise level is high.
             g0 = (0.00000001,0.0000001,0.000001,0.00001,0.0001,0.001)
             g0g = xp.concatenate((xp.asarray( g0),xp.linspace(0.01, 0.99, npoints)))
         elif self.LoopGain_LO == 'test':
             g0g = xp.asarray( xp.linspace(0.01, 0.99, npoints) )
         else:
             # if gain is set no optimization is done and bias is not compensated
-            g0 = (bias*self.LoopGain_LO)
+            g0 = (bias*self.LoopGain_LO,bias*self.LoopGain_LO)
             g0g = xp.asarray(g0)
 
         e1 = psd_freq.reshape((1,psd_freq.shape[0]))
         e2 = psd_focus_turb.reshape((1,psd_focus_turb.shape[0]))
         e3 = g0g.reshape((g0g.shape[0], 1))
         psd_freq_ext, psd_focus_turb_ext, g0g_ext = xp.broadcast_arrays(e1, e2, e3)
 
@@ -808,15 +808,15 @@
             ax2.set_xlabel('frequency [Hz]')
             ax2.set_ylabel('Power')
 
         resultFocus = xp.absolute((xp.sum(self.fFocusS_lambda1( g0g_ext, psd_freq_ext, psd_focus_turb_ext), axis=(1)) ) )
 
         minFocusIdx = xp.where(resultFocus == xp.nanmin(resultFocus))
         if self.verbose:
-            print('         best focus gain (noise):',g0g[minFocusIdx[0][0]])
+            print('    best focus gain (noise):',"%.3f" % cpuArray(g0g[minFocusIdx[0][0]]))
         if alib==gpulib and gpuEnabled:
             return cp.asnumpy(resultFocus[minFocusIdx[0][0]])
         else:
             return (resultFocus[minFocusIdx[0][0]])
         
     def computeWindResidual(self, psd_freq, psd_tip_wind0, psd_tilt_wind0, var1x, bias, alib):
         npoints = 99
@@ -925,18 +925,18 @@
                 ax2.set_ylabel('Power')
                 
         minTipIdx = xp.where(resultTip == xp.nanmin(resultTip))
         minTiltIdx = xp.where(resultTilt == xp.nanmin(resultTilt))
         
         if self.verbose:
             if self.LoopGain_LO == 'optimize' or self.LoopGain_LO == 'test':
-                print('         best tip & tilt gain (wind)',g0g[minTipIdx[0][0],minTipIdx[1][0]]*g1g[minTipIdx[0][0],minTipIdx[1][0]],\
-                                                             g0g[minTiltIdx[0][0],minTiltIdx[1][0]]*g1g[minTipIdx[0][0],minTipIdx[1][0]])
+                print('    best tip & tilt gain (wind)',"%.3f" % cpuArray(g0g[minTipIdx[0][0],minTipIdx[1][0]]*g1g[minTipIdx[0][0],minTipIdx[1][0]]),\
+                                                        "%.3f" % cpuArray(g0g[minTiltIdx[0][0],minTiltIdx[1][0]]*g1g[minTipIdx[0][0],minTipIdx[1][0]]))
             else:
-                print('         best tip & tilt gain (wind)',g0g[minTipIdx[0][0]],g0g[minTiltIdx[0][0]])
+                print('    best tip & tilt gain (wind)',"%.3f" % cpuArray(g0g[minTipIdx[0][0]]), "%.3f" % cpuArray(g0g[minTiltIdx[0][0]]))
                     
         if self.LoopGain_LO == 'optimize' or self.LoopGain_LO == 'test':
             if alib==gpulib and gpuEnabled:
                 return cp.asnumpy(resultTip[minTipIdx[0][0], minTipIdx[1][0]]), cp.asnumpy(resultTilt[minTiltIdx[0][0], minTiltIdx[1][0]])
             else:
                 return (resultTip[minTipIdx[0][0], minTipIdx[1][0]], resultTilt[minTiltIdx[0][0], minTiltIdx[1][0]])
         else:
@@ -1060,65 +1060,72 @@
         Caa, Cas, Css = self.computeCovMatrices(xp.asarray(aCartPointingCoordsV), xp.asarray(aaCartNGSCoords), xp=np)
         for i in range(points):
             Ri = R[2*i:2*(i+1),:]
             RTi = RT[:, 2*i:2*(i+1)]
             Casi = Cas[2*i:2*(i+1),:]
             C2b = xp.dot(Ri, xp.dot(Css, RTi)) - xp.dot(Casi, RTi) - xp.dot(Ri, Casi.transpose())
             C3 = xp.dot(Ri, xp.dot(xp.asarray(aCnn), RTi))
-            # sum tomography (Caa + C2b), noise (C3), wind (aC1) errors
+            # tomography (C2), noise (C3), wind (aC1) errors
             if self.noNoise:
                 ss = xp.asarray(aC1) + Caa + C2b 
-                print('WARNING: LO noise is not active!')
+                print('    WARNING: LO noise is not active!')
             else:
                 ss = xp.asarray(aC1) + Caa + C2b + C3
             Ctot[2*i:2*(i+1),:] = ss
+            if self.verbose:
+                print('    Star coordinates [arcsec]: ', ("{:.1f}, "*len(aCartPointingCoordsV[i])).format(*aCartPointingCoordsV[i]))
+                print('    Total Cov. (tomo., tur.+noi., wind) [nm]:',"%.2f" % np.sqrt(np.trace(ss)),
+                      '(', "%.2f" % np.sqrt(np.trace(Caa + C2b)), ',', "%.2f" % np.sqrt(np.trace(C3)), ',', "%.2f" % np.sqrt(np.trace(aC1)),')')
         return Ctot
 
         
     def CMatAssemble(self, aCartPointingCoordsV, aaCartNGSCoords, aCnn, aC1):
         R, RT = self.buildReconstuctor2(np.asarray(aCartPointingCoordsV), aaCartNGSCoords)
         Caa, Cas, Css = self.computeCovMatrices(np.asarray(aCartPointingCoordsV), aaCartNGSCoords)        
         C2 = Caa + np.dot(R, np.dot(Css, RT)) - np.dot(Cas, RT) - np.dot(R, Cas.transpose())
         C3 = np.dot(R, np.dot(aCnn, RT))
         # sum tomography (C2), noise (C3), wind (aC1) errors
         if self.noNoise:
             ss = aC1 + C2
-            print('WARNING: LO noise is not active!')
+            print('    WARNING: LO noise is not active!')
         else:
             Ctot = aC1 + C2 + C3
+        if self.verbose:
+            print('    Star coordinates [arcsec]: ', ("{:.1f}, "*len(aCartPointingCoordsV)).format(*aCartPointingCoordsV))
+            print('    Total Cov. (tomo., tur.+noi., wind) [nm]:', "%.2f" % np.sqrt(np.trace(Ctot)),
+                  '(', "%.2f" % np.sqrt(np.trace(C2)), ',', "%.2f" % np.sqrt(np.trace(C3)), ',', "%.2f" % np.sqrt(np.trace(aC1)),')')
         return Ctot
 
     
     def computeTotalResidualMatrixI(self, indices, aCartPointingCoords, aCartNGSCoords, aNGS_flux, aNGS_freq, aNGS_SR_LO, aNGS_EE_LO, aNGS_FWHM_mas):
         nPointings = aCartPointingCoords.shape[0]
         maxFluxIndex = np.where(aNGS_flux==np.amax(aNGS_flux))
         nNaturalGS = len(indices)
         C1 = np.zeros((2,2))
         Cnn = np.zeros((2*nNaturalGS,2*nNaturalGS))
         if self.verbose:
             print('mavisLO.computeTotalResidualMatrix')
-            print('         aNGS_flux',aNGS_flux)
         for starIndex in range(nNaturalGS):
             bias, amu, avar = self.bias[indices[starIndex]], self.amu[indices[starIndex]], self.avar[indices[starIndex]]            
             nr = self.nr[indices[starIndex]] 
             wr = self.wr[indices[starIndex]] 
             if self.verbose:
-                print('         turb. + noise residual [nm\u00b2]:',np.array(nr))
+                print('    NGS flux [ph/SA/s]       :', aNGS_flux[starIndex])
+                print('    NGS coordinates [arcsec] : ', ("{:.1f}, "*len(aCartNGSCoords[starIndex])).format(*aCartNGSCoords[starIndex]))
+                print('    turb. + noise residual (per NGS) [nm\u00b2]:',np.array(nr))
             Cnn[2*starIndex,2*starIndex] = nr[0]
             Cnn[2*starIndex+1,2*starIndex+1] = nr[1]
             if starIndex == maxFluxIndex[0][0]:
                 C1[0,0] = wr[0]
                 C1[1,1] = wr[1]
                 if self.verbose:
-                    print('         wind-shake residual    [nm\u00b2]:',np.array(wr))
+                    print('    wind-shake residual (brightest NGS)    [nm\u00b2]:',np.array(wr))
 
         # C1 and Cnn do not depend on aCartPointingCoords[i]
         Ctot = self.multiCMatAssemble(aCartPointingCoords, aCartNGSCoords, Cnn, C1)
-        if self.verbose:
-            print('         Ctot [nm\u00b2]:',Ctot)
         return Ctot.reshape((nPointings,2,2))
 
 
     def computeTotalResidualMatrix(self, aCartPointingCoords, aCartNGSCoords, aNGS_flux, aNGS_freq, aNGS_SR_LO, aNGS_EE_LO, aNGS_FWHM_mas, doAll=True):
         self.bias = []
         self.amu = []
         self.avar = []
@@ -1128,15 +1135,14 @@
         maxFluxIndex = np.where(aNGS_flux==np.amax(aNGS_flux))
         nNaturalGS = aCartNGSCoords.shape[0]
         C1 = np.zeros((2,2))
         Cnn = np.zeros((2*nNaturalGS,2*nNaturalGS))
 
         if self.verbose:
             print('mavisLO.computeTotalResidualMatrix')
-            print('         aNGS_flux:',aNGS_flux)
             
         for starIndex in range(nNaturalGS):
             self.configLOFreq( aNGS_freq[starIndex] )
             if self.simpleVarianceComputation:
                 bias, amu, avar = self.simplifiedComputeBiasAndVariance(aNGS_flux[starIndex], aNGS_freq[starIndex], aNGS_EE_LO[starIndex], aNGS_FWHM_mas[starIndex]) # one scalar, two
             else:
                 bias, amu, avar = self.computeBiasAndVariance(aNGS_flux[starIndex], aNGS_freq[starIndex], aNGS_EE_LO[starIndex], aNGS_FWHM_mas[starIndex]) # one scalar, two tuples of 2
@@ -1156,27 +1162,27 @@
             else:
                 wr = (0,0)
 
             self.nr.append(nr)
             self.wr.append(wr)
 
             if self.verbose:
-                print('         turb. + noise residual [nm\u00b2]:',np.array(nr))
-                print('         wind-shake residual    [nm\u00b2]:',np.array(wr))
+                print('    NGS flux [ph/SA/s]       :', aNGS_flux[starIndex])
+                print('    NGS coordinates [arcsec] : ', ("{:.1f}, "*len(aCartNGSCoords[starIndex])).format(*aCartNGSCoords[starIndex]))
+                print('    turb. + noise residual (per NGS) [nm\u00b2]:',np.array(nr))
+                print('    wind-shake residual (per NGS)    [nm\u00b2]:',np.array(wr))
             Cnn[2*starIndex,2*starIndex] = nr[0]
             Cnn[2*starIndex+1,2*starIndex+1] = nr[1]
             if starIndex == maxFluxIndex[0][0]:
                 C1[0,0] = wr[0]
                 C1[1,1] = wr[1]
 
         if doAll:
             # C1 and Cnn do not depend on aCartPointingCoords[i]
             Ctot = self.multiCMatAssemble(aCartPointingCoords, aCartNGSCoords, Cnn, C1)
-            if self.verbose:
-                print('         Ctot [nm\u00b2]:',Ctot)
             return Ctot.reshape((nPointings,2,2))
         else:
             return None
 
     def computeFocusTotalResidualMatrix(self, aCartNGSCoords, aNGS_flux, aNGS_freq, aNGS_SR_LO, aNGS_EE_LO, aNGS_FWHM_mas):
         maxFluxIndex = np.where(aNGS_flux==np.amax(aNGS_flux))
         nNaturalGS = aCartNGSCoords.shape[0]
@@ -1215,15 +1221,15 @@
         CaaL, CasL, CssL = self.computeFocusCovMatrices(np.asarray((0,0)), np.asarray(aCartLGSCoords), xp=np)
         # tomography error for a on-axis star for LGS WFSs
         CtotL = CaaL + np.dot(RL, np.dot(CssL, RLT)) - np.dot(CasL, RLT) - np.dot(RL, CasL.transpose())
         # difference
         CtotDiff = Ctot - CtotL
         
         if self.verbose:
-            print('         focus residual [nm]:',np.sqrt(CtotDiff))
+            print('    focus residual [nm]:',np.sqrt(CtotDiff))
         
         return CtotDiff    
         
     def ellipsesFromCovMats(self, Ctot):
         theta = sp.symbols('theta')
         sigma_1 = sp.symbols('sigma^2_1')
         sigma_2 = sp.symbols('sigma^2_2')
```

### Comparing `mastsel-1.2.7/mastsel/mavisParams.py` & `mastsel-1.2.8/mastsel/mavisParams.py`

 * *Files identical despite different names*

### Comparing `mastsel-1.2.7/mastsel/mavisParamsOld.py` & `mastsel-1.2.8/mastsel/mavisParamsOld.py`

 * *Files identical despite different names*

### Comparing `mastsel-1.2.7/mastsel/mavisPsf.py` & `mastsel-1.2.8/mastsel/mavisPsf.py`

 * *Files identical despite different names*

### Comparing `mastsel-1.2.7/mastsel/mavisUtilities.py` & `mastsel-1.2.8/mastsel/mavisUtilities.py`

 * *Files identical despite different names*

### Comparing `mastsel-1.2.7/mastsel.egg-info/PKG-INFO` & `mastsel-1.2.8/mastsel.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mastsel
-Version: 1.2.7
+Version: 1.2.8
 Summary: Asterism Selection for MAVIS instrument
 Author-email: Fabio Rossi <fabio.rossi@inaf.it>
 License: MIT License
 Project-URL: repository, https://github.com/astro-tiptop/MASTSEL
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mastsel-1.2.7/mastsel.egg-info/SOURCES.txt` & `mastsel-1.2.8/mastsel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mastsel-1.2.7/notebooks/MAVIS-CONVOLUTION-TEST.ipynb` & `mastsel-1.2.8/notebooks/MAVIS-CONVOLUTION-TEST.ipynb`

 * *Files identical despite different names*

### Comparing `mastsel-1.2.7/notebooks/MAVIS-CONVOLUTION.ipynb` & `mastsel-1.2.8/notebooks/MAVIS-CONVOLUTION.ipynb`

 * *Files identical despite different names*

### Comparing `mastsel-1.2.7/notebooks/MAVIS.ipynb` & `mastsel-1.2.8/notebooks/MAVIS.ipynb`

 * *Files identical despite different names*

### Comparing `mastsel-1.2.7/notebooks/MAVIS2.ipynb` & `mastsel-1.2.8/notebooks/MAVIS2.ipynb`

 * *Files identical despite different names*

### Comparing `mastsel-1.2.7/notebooks/MAVIS3.ipynb` & `mastsel-1.2.8/notebooks/MAVIS3.ipynb`

 * *Files identical despite different names*

### Comparing `mastsel-1.2.7/notebooks/MAVIS_INT_REC.ipynb` & `mastsel-1.2.8/notebooks/MAVIS_INT_REC.ipynb`

 * *Files identical despite different names*

### Comparing `mastsel-1.2.7/notebooks/MAVIS_MAIN.ipynb` & `mastsel-1.2.8/notebooks/MAVIS_MAIN.ipynb`

 * *Files identical despite different names*

### Comparing `mastsel-1.2.7/pyproject.toml` & `mastsel-1.2.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mastsel-1.2.7/tests/allTests.py` & `mastsel-1.2.8/tests/allTests.py`

 * *Files identical despite different names*

### Comparing `mastsel-1.2.7/tests/testTfOpt.py` & `mastsel-1.2.8/tests/testTfOpt.py`

 * *Files identical despite different names*


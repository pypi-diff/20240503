# Comparing `tmp/MVComp-0.9.4.tar.gz` & `tmp/MVComp-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MVComp-0.9.4.tar", last modified: Wed Apr 24 00:23:25 2024, max compression
+gzip compressed data, was "MVComp-0.9.5.tar", last modified: Fri May  3 17:04:34 2024, max compression
```

## Comparing `MVComp-0.9.4.tar` & `MVComp-0.9.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zklsmr    (1000) zklsmr    (1000)        0 2024-04-24 00:23:25.042512 MVComp-0.9.4/
--rw-r--r--   0 zklsmr    (1000) zklsmr    (1000)    11351 2024-04-11 15:03:25.000000 MVComp-0.9.4/LICENSE
-drwxr-xr-x   0 zklsmr    (1000) zklsmr    (1000)        0 2024-04-24 00:23:25.042512 MVComp-0.9.4/MVComp.egg-info/
--rw-r--r--   0 zklsmr    (1000) zklsmr    (1000)      251 2024-04-24 00:23:25.000000 MVComp-0.9.4/MVComp.egg-info/PKG-INFO
--rw-r--r--   0 zklsmr    (1000) zklsmr    (1000)      206 2024-04-24 00:23:25.000000 MVComp-0.9.4/MVComp.egg-info/SOURCES.txt
--rw-r--r--   0 zklsmr    (1000) zklsmr    (1000)        1 2024-04-24 00:23:25.000000 MVComp-0.9.4/MVComp.egg-info/dependency_links.txt
--rw-r--r--   0 zklsmr    (1000) zklsmr    (1000)       67 2024-04-24 00:23:25.000000 MVComp-0.9.4/MVComp.egg-info/requires.txt
--rw-r--r--   0 zklsmr    (1000) zklsmr    (1000)       22 2024-04-24 00:23:25.000000 MVComp-0.9.4/MVComp.egg-info/top_level.txt
--rw-r--r--   0 zklsmr    (1000) zklsmr    (1000)      251 2024-04-24 00:23:25.042512 MVComp-0.9.4/PKG-INFO
--rw-r--r--   0 zklsmr    (1000) zklsmr    (1000)     8235 2024-04-11 15:03:25.000000 MVComp-0.9.4/README.md
--rw-r--r--   0 zklsmr    (1000) zklsmr    (1000)    44524 2024-04-23 23:26:46.000000 MVComp-0.9.4/mvcomp.py
--rw-r--r--   0 zklsmr    (1000) zklsmr    (1000)     2404 2024-04-23 23:26:39.000000 MVComp-0.9.4/plotting.py
--rw-r--r--   0 zklsmr    (1000) zklsmr    (1000)       38 2024-04-24 00:23:25.042512 MVComp-0.9.4/setup.cfg
--rw-r--r--   0 zklsmr    (1000) zklsmr    (1000)      527 2024-04-24 00:23:06.000000 MVComp-0.9.4/setup.py
--rw-r--r--   0 zklsmr    (1000) zklsmr    (1000)    14481 2024-04-23 23:26:39.000000 MVComp-0.9.4/utils.py
+drwxrwxr-x   0 stechr    (1001) stechr    (1001)        0 2024-05-03 17:04:34.548681 MVComp-0.9.5/
+-rw-rw-r--   0 stechr    (1001) stechr    (1001)    11351 2024-02-27 14:51:25.000000 MVComp-0.9.5/LICENSE
+drwxrwxr-x   0 stechr    (1001) stechr    (1001)        0 2024-05-03 17:04:34.548681 MVComp-0.9.5/MVComp.egg-info/
+-rw-r--r--   0 stechr    (1001) stechr    (1001)      430 2024-05-03 17:04:34.000000 MVComp-0.9.5/MVComp.egg-info/PKG-INFO
+-rw-rw-r--   0 stechr    (1001) stechr    (1001)      206 2024-05-03 17:04:34.000000 MVComp-0.9.5/MVComp.egg-info/SOURCES.txt
+-rw-rw-r--   0 stechr    (1001) stechr    (1001)        1 2024-05-03 17:04:34.000000 MVComp-0.9.5/MVComp.egg-info/dependency_links.txt
+-rw-rw-r--   0 stechr    (1001) stechr    (1001)       67 2024-05-03 17:04:34.000000 MVComp-0.9.5/MVComp.egg-info/requires.txt
+-rw-rw-r--   0 stechr    (1001) stechr    (1001)       22 2024-05-03 17:04:34.000000 MVComp-0.9.5/MVComp.egg-info/top_level.txt
+-rw-r--r--   0 stechr    (1001) stechr    (1001)      430 2024-05-03 17:04:34.548681 MVComp-0.9.5/PKG-INFO
+-rw-rw-r--   0 stechr    (1001) stechr    (1001)     8738 2024-05-03 16:31:42.000000 MVComp-0.9.5/README.md
+-rw-rw-r--   0 stechr    (1001) stechr    (1001)    44622 2024-05-03 16:31:42.000000 MVComp-0.9.5/mvcomp.py
+-rw-rw-r--   0 stechr    (1001) stechr    (1001)     2404 2024-05-03 16:31:42.000000 MVComp-0.9.5/plotting.py
+-rw-rw-r--   0 stechr    (1001) stechr    (1001)       38 2024-05-03 17:04:34.548681 MVComp-0.9.5/setup.cfg
+-rw-rw-r--   0 stechr    (1001) stechr    (1001)      503 2024-05-03 17:03:48.000000 MVComp-0.9.5/setup.py
+-rw-rw-r--   0 stechr    (1001) stechr    (1001)    14481 2024-05-03 16:31:42.000000 MVComp-0.9.5/utils.py
```

### Comparing `MVComp-0.9.4/LICENSE` & `MVComp-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `MVComp-0.9.4/README.md` & `MVComp-0.9.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 # Multivariate Comparisons (MVComp)
 
 **Authors:** Stefanie Tremblay @stremblay18, Zaki Alasmar @zklsmr, Amir Pirhadi @amirpirhadi, Felix Carbonell, Yasser Iturria-Medina, Claudine Gauthier, Christopher Steele @steelec
 
-A set of functions to compute Mahalanobis D (D**2) on multimodal MRI images in a group of individuals in comparison to a reference group or within a single individual.
+A set of functions to compute Mahalanobis D (D<sup>2</sup> / D2) on multimodal MRI images in a group of individuals in comparison to a reference group or within a single individual.
 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10713027.svg)](https://doi.org/10.5281/zenodo.10713027)
 
+[![Documentation Status](https://readthedocs.org/projects/mvcomp/badge/?version=latest)](https://mvcomp.readthedocs.io/en/latest/?badge=latest)
+
 [Biorxiv link](https://www.biorxiv.org/content/10.1101/2024.02.27.582381v1)
 
 Reference:
 ```
-Tremblay, SA, Alasmar, Z, Pirhadi, A, Carbonell, F, Iturria-Medina, Y, Gauthier, C, Steele, CJ, (under review) MVComp toolbox: MultiVariate Comparisons of brain MRI features accounting for common information across metrics (submitted)
+Tremblay, SA, Alasmar, Z, Pirhadi, A, Carbonell, F, Iturria-Medina, Y, Gauthier, C, Steele, CJ, (under revision) MVComp toolbox: MultiVariate Comparisons of brain MRI features accounting for common information across metrics (submitted)
 ```
 
+Please refer to [mvcomp.readthedocs.io](https://mvcomp.readthedocs.io/en/latest/) for installation and usage details.
+
+After installation, please run the three examples in the `./examples/` subdirectory to confirm that your installation is functioning correctly. As necessary, please open a github issue to report any issues that may arise.
+
 # Mahalanobis d
 
 The Mahalanobis distance, or D2, is defined as the multivariate distance between a point and a distribution in which covariance between features (e.g., imaging metrics) is accounted for (Mahalanobis, 1936). D2 is thus similar to a z-score, but applicable to multivariate data because when computing D2, the shape of the distribution is taken into account such that the values that are more probable have lower distance values (Taylor et al., 2020). In other words, D2 tells us how improbable a certain combination of features is. For example, because height and weight are highly correlated, very tall individuals that have a very low weight would appear outside of the distribution and would have a high D2 value. Relationships between variables are thus accounted for in the D2 framework by dividing the Euclidean distance by the covariance matrix, which also scales the variables to have unit variance.
 
 The Mahalanobis distance approach has been used extensively in outlier detection, cluster analysis, and classification applications (e.g., Kritzman & Li, 2010; Xiang et al., 2008; Ghorbani, 2019). D2 has also been used in neuroimaging, mainly in the study of neurological disorders, to detect lesions (Gyebnár et al., 2019; Lindemer et al., 2015), or to evaluate the degree of abnormality in the brains of patients relative to controls (Dean et al., 2017; Owen et al., 2021; Taylor et al., 2020), but also to study healthy WM development (Kulikova et al., 2015). Despite promising implementations and its high versatility, D2 has not yet been widely adopted. To facilitate its use, we present here an open-source python-based tool for computing D2 relative to a reference group or within a single individual: the MultiVariate Comparison (MVComp) toolbox.
 
 ## Usage
```

### Comparing `MVComp-0.9.4/mvcomp.py` & `MVComp-0.9.5/mvcomp.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,14 +164,17 @@
 
     Returns:
         1. feature_image_fname_list (List of strings): 
             A list of the full pathnames of the features.
         2. f_list (List of strings): A list of features names.
 
     """
+    if remove_list is None:
+        remove_list = [] #recast to simplify checks prior to removal
+
     feature_image_fname_list = mysort(
         glob.glob(os.path.join(feature_in_dir, "*" + suffix_name)))
     f_list = [os.path.basename(mod).replace(suffix_name, "")
               for mod in feature_image_fname_list]
 
     if len(remove_list)>0:
         for i, rem in enumerate(remove_list):
```

### Comparing `MVComp-0.9.4/plotting.py` & `MVComp-0.9.5/plotting.py`

 * *Files identical despite different names*

### Comparing `MVComp-0.9.4/utils.py` & `MVComp-0.9.5/utils.py`

 * *Files identical despite different names*


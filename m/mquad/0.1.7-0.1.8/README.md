# Comparing `tmp/mquad-0.1.7-py3-none-any.whl.zip` & `tmp/mquad-0.1.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 20015 bytes, number of entries: 12
+Zip file size: 20021 bytes, number of entries: 12
 -rw-rwS---  2.0 unx       24 b- defN 23-Feb-24 02:02 mquad/__init__.py
--rw-rwS---  2.0 unx    13165 b- defN 23-Feb-24 02:02 mquad/mquad.py
+-rw-r--r--  2.0 unx    13166 b- defN 24-Feb-19 02:51 mquad/mquad.py
 -rw-r--r--  2.0 unx     6651 b- defN 23-Jul-24 04:14 mquad/mquad_CLI.py
--rw-rwS---  2.0 unx    14628 b- defN 23-Feb-24 03:19 mquad/mquad_batch_mixbin.py
+-rw-r--r--  2.0 unx    14633 b- defN 24-May-03 08:43 mquad/mquad_batch_mixbin.py
 -rw-rwS---  2.0 unx     2656 b- defN 23-Feb-24 02:02 mquad/mquad_utils.py
--rw-r--r--  2.0 unx       22 b- defN 23-Jul-24 04:42 mquad/version.py
--rw-rwS---  2.0 unx    11357 b- defN 23-Jul-24 04:42 mquad-0.1.7.dist-info/LICENSE
--rw-r--r--  2.0 unx     5622 b- defN 23-Jul-24 04:42 mquad-0.1.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-24 04:42 mquad-0.1.7.dist-info/WHEEL
--rw-rwS---  2.0 unx       47 b- defN 23-Jul-24 04:42 mquad-0.1.7.dist-info/entry_points.txt
--rw-rwS---  2.0 unx        6 b- defN 23-Jul-24 04:42 mquad-0.1.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      921 b- defN 23-Jul-24 04:42 mquad-0.1.7.dist-info/RECORD
-12 files, 55191 bytes uncompressed, 18483 bytes compressed:  66.5%
+-rw-r--r--  2.0 unx       22 b- defN 24-May-03 08:46 mquad/version.py
+-rw-rwS---  2.0 unx    11357 b- defN 24-May-03 09:11 mquad-0.1.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5621 b- defN 24-May-03 09:11 mquad-0.1.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-03 09:11 mquad-0.1.8.dist-info/WHEEL
+-rw-rwS---  2.0 unx       47 b- defN 24-May-03 09:11 mquad-0.1.8.dist-info/entry_points.txt
+-rw-rwS---  2.0 unx        6 b- defN 24-May-03 09:11 mquad-0.1.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      921 b- defN 24-May-03 09:11 mquad-0.1.8.dist-info/RECORD
+12 files, 55196 bytes uncompressed, 18489 bytes compressed:  66.5%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: mquad/mquad_utils.py
 Comment: 
 
 Filename: mquad/version.py
 Comment: 
 
-Filename: mquad-0.1.7.dist-info/LICENSE
+Filename: mquad-0.1.8.dist-info/LICENSE
 Comment: 
 
-Filename: mquad-0.1.7.dist-info/METADATA
+Filename: mquad-0.1.8.dist-info/METADATA
 Comment: 
 
-Filename: mquad-0.1.7.dist-info/WHEEL
+Filename: mquad-0.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: mquad-0.1.7.dist-info/entry_points.txt
+Filename: mquad-0.1.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: mquad-0.1.7.dist-info/top_level.txt
+Filename: mquad-0.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: mquad-0.1.7.dist-info/RECORD
+Filename: mquad-0.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mquad/mquad.py

```diff
@@ -276,15 +276,15 @@
                 var_file.write('\n'.join(str(var) for var in renamed_vars))
                 
         if export_heatmap:
             af = best_ad/best_dp
             #af = af.fillna(0)
             fig, ax = plt.subplots(figsize=(8,6))
             plt.title("Allele frequency of top variants")
-            plt.style.use('seaborn-dark')
+            #plt.style.use('seaborn-dark')
             pal = "YlGnBu"
             if self.variants is not None:
                 sns.heatmap(af, cmap=pal, yticklabels=renamed_vars)
                 plt.yticks(rotation=0)
             else:
                 sns.heatmap(af, cmap=pal)
                 plt.yticks(rotation=0)
```

## mquad/mquad_batch_mixbin.py

```diff
@@ -235,15 +235,15 @@
                 
         if export_heatmap is True:
             af = best_ad/best_dp
             #print(af.shape)
             #af = af.fillna(0)
             fig, ax = plt.subplots(figsize=(15,10))
             plt.title("Allele frequency of top variants")
-            plt.style.use('seaborn-dark')
+            plt.style.use('seaborn-v0_8-dark')
             if self.variants is not None:
                 sns.heatmap(af, cmap='Greens', yticklabels=renamed_vars)
             else:
                 sns.heatmap(af, cmap='Greens')
             plt.savefig(out_dir + '/top variants heatmap.pdf')
 
         #export ad dp mtx out for vireo
```

## mquad/version.py

```diff
@@ -1 +1 @@
-__version__ = '0.1.7'
+__version__ = '0.1.8'
```

## Comparing `mquad-0.1.7.dist-info/LICENSE` & `mquad-0.1.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mquad-0.1.7.dist-info/METADATA` & `mquad-0.1.8.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: mquad
-Version: 0.1.7
+Version: 0.1.8
 Summary: MQuad - Mixture Modelling for Mitochondrial Mutation detection
 Home-page: https://github.com/aaronkwc/MQuad
 Author: Aaron Kwok
 Author-email: aaronkwc@connect.hku.hk
 License: Apache-2.0
 Keywords: mitochondrial mutation,single-cell omics data,binomial mixture model,model selection
 License-File: LICENSE
-Requires-Dist: numpy (>=1.9.0)
-Requires-Dist: scipy (>=1.4.0)
+Requires-Dist: numpy >=1.9.0
+Requires-Dist: scipy >=1.4.0
 Requires-Dist: matplotlib
-Requires-Dist: BBMix (>=0.2.1)
+Requires-Dist: BBMix >=0.2.1
 Requires-Dist: vireoSNP
 Requires-Dist: kneed
 Requires-Dist: pandas
 Requires-Dist: seaborn
-Requires-Dist: sklearn
+Requires-Dist: scikit-learn
 Provides-Extra: docs
 Requires-Dist: sphinx-bootstrap-theme ; extra == 'docs'
 
 =====
 MQuad
 =====
```

## Comparing `mquad-0.1.7.dist-info/RECORD` & `mquad-0.1.8.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 mquad/__init__.py,sha256=BPMoWHuBXI1iHImJmzc7ckA3JY4TFqIRkap6qnlxmKE,24
-mquad/mquad.py,sha256=1iQGjfUoSw4TELdL83kOnaONAP90mBb6yIi-SYytgps,13165
+mquad/mquad.py,sha256=ZpnZhtQlrJPC0U833hI3-_w7u1pxxZWU3bMolw0cruM,13166
 mquad/mquad_CLI.py,sha256=8LAQgG-265Z2XlBJiVo8QvL2myRd1Yc2IaZmg-0YacA,6651
-mquad/mquad_batch_mixbin.py,sha256=KJlAak0uG3K76gqdGqpn66mGIosnDtZN_mxrVKVPyug,14628
+mquad/mquad_batch_mixbin.py,sha256=7PtyYUxY0noPQ3ZxegV7QqV8tt3q4WlRTRfQLtjyeG4,14633
 mquad/mquad_utils.py,sha256=SgTOhIDq1x_HquqWaoABVLyZHZayILsIcxRI7U84sHA,2656
-mquad/version.py,sha256=mFY0GwwuN-a3M8w93_mskS6GZIvv9SNdjLfJaWNsm-I,22
-mquad-0.1.7.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-mquad-0.1.7.dist-info/METADATA,sha256=BkKFYpo8hctZX1z29WXoRbDqXDj_VWiioW6nKCbRESo,5622
-mquad-0.1.7.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-mquad-0.1.7.dist-info/entry_points.txt,sha256=of0Qn7PzVLFVaH5xVZIdRNRKfrHtq3itydbIyeAHe-8,47
-mquad-0.1.7.dist-info/top_level.txt,sha256=2fkr83zKNY0ZlvWCCnXe1TVeVAAUeZbVfysYFt1FXNM,6
-mquad-0.1.7.dist-info/RECORD,,
+mquad/version.py,sha256=rq5OMW-khxQo_5FAvSrPaAS1lRfG9aG2hSuo-KK2Yfk,22
+mquad-0.1.8.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+mquad-0.1.8.dist-info/METADATA,sha256=JmhW3012D97L1AH9cdttiRKXHSzieR-iQCwk20O2oTs,5621
+mquad-0.1.8.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+mquad-0.1.8.dist-info/entry_points.txt,sha256=of0Qn7PzVLFVaH5xVZIdRNRKfrHtq3itydbIyeAHe-8,47
+mquad-0.1.8.dist-info/top_level.txt,sha256=2fkr83zKNY0ZlvWCCnXe1TVeVAAUeZbVfysYFt1FXNM,6
+mquad-0.1.8.dist-info/RECORD,,
```


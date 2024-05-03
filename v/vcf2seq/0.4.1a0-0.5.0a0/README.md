# Comparing `tmp/vcf2seq-0.4.1a0.tar.gz` & `tmp/vcf2seq-0.5.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcf2seq-0.4.1a0.tar", last modified: Wed Apr 17 15:30:01 2024, max compression
+gzip compressed data, was "vcf2seq-0.5.0a0.tar", last modified: Fri May  3 14:57:48 2024, max compression
```

## Comparing `vcf2seq-0.4.1a0.tar` & `vcf2seq-0.5.0a0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-04-17 15:30:01.871774 vcf2seq-0.4.1a0/
--rw-r--r--   0 benoit    (1001) bio2m     (1010)    34916 2023-03-07 08:59:59.000000 vcf2seq-0.4.1a0/LICENCE.md
--rw-r--r--   0 benoit    (1001) bio2m     (1010)       98 2024-04-09 10:58:25.000000 vcf2seq-0.4.1a0/MANIFEST.in
--rw-r--r--   0 benoit    (1001) bio2m     (1010)     2198 2024-04-17 15:30:01.871774 vcf2seq-0.4.1a0/PKG-INFO
--rw-r--r--   0 benoit    (1001) bio2m     (1010)     1606 2024-04-17 15:23:42.000000 vcf2seq-0.4.1a0/README.md
--rw-r--r--   0 benoit    (1001) bio2m     (1010)       38 2024-04-17 15:30:01.871774 vcf2seq-0.4.1a0/setup.cfg
--rw-r--r--   0 benoit    (1001) bio2m     (1010)      990 2024-04-10 14:28:47.000000 vcf2seq-0.4.1a0/setup.py
-drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-04-17 15:30:01.871774 vcf2seq-0.4.1a0/vcf2seq/
--rw-r--r--   0 benoit    (1001) bio2m     (1010)      163 2024-04-09 15:41:02.000000 vcf2seq-0.4.1a0/vcf2seq/__init__.py
--rwxr-xr-x   0 benoit    (1001) bio2m     (1010)     2393 2023-07-13 15:02:22.000000 vcf2seq-0.4.1a0/vcf2seq/ascii.py
--rw-r--r--   0 benoit    (1001) bio2m     (1010)      215 2024-04-17 15:29:52.000000 vcf2seq-0.4.1a0/vcf2seq/info.py
--rwxr-xr-x   0 benoit    (1001) bio2m     (1010)    11029 2024-04-17 15:23:37.000000 vcf2seq-0.4.1a0/vcf2seq/vcf2seq.py
-drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-04-17 15:30:01.871774 vcf2seq-0.4.1a0/vcf2seq.egg-info/
--rw-r--r--   0 benoit    (1001) bio2m     (1010)     2198 2024-04-17 15:30:01.000000 vcf2seq-0.4.1a0/vcf2seq.egg-info/PKG-INFO
--rw-r--r--   0 benoit    (1001) bio2m     (1010)      301 2024-04-17 15:30:01.000000 vcf2seq-0.4.1a0/vcf2seq.egg-info/SOURCES.txt
--rw-r--r--   0 benoit    (1001) bio2m     (1010)        1 2024-04-17 15:30:01.000000 vcf2seq-0.4.1a0/vcf2seq.egg-info/dependency_links.txt
--rw-r--r--   0 benoit    (1001) bio2m     (1010)       49 2024-04-17 15:30:01.000000 vcf2seq-0.4.1a0/vcf2seq.egg-info/entry_points.txt
--rw-r--r--   0 benoit    (1001) bio2m     (1010)        8 2024-04-17 15:30:01.000000 vcf2seq-0.4.1a0/vcf2seq.egg-info/requires.txt
--rw-r--r--   0 benoit    (1001) bio2m     (1010)        8 2024-04-17 15:30:01.000000 vcf2seq-0.4.1a0/vcf2seq.egg-info/top_level.txt
+drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-05-03 14:57:48.386566 vcf2seq-0.5.0a0/
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)    34916 2023-03-07 08:59:59.000000 vcf2seq-0.5.0a0/LICENCE.md
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)       98 2024-04-09 10:58:25.000000 vcf2seq-0.5.0a0/MANIFEST.in
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)     2231 2024-05-03 14:57:48.386566 vcf2seq-0.5.0a0/PKG-INFO
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)     1606 2024-04-17 15:23:42.000000 vcf2seq-0.5.0a0/README.md
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)       38 2024-05-03 14:57:48.386566 vcf2seq-0.5.0a0/setup.cfg
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)      990 2024-04-10 14:28:47.000000 vcf2seq-0.5.0a0/setup.py
+drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-05-03 14:57:48.386566 vcf2seq-0.5.0a0/vcf2seq/
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)      163 2024-04-09 15:41:02.000000 vcf2seq-0.5.0a0/vcf2seq/__init__.py
+-rwxr-xr-x   0 benoit    (1001) bio2m     (1010)     2393 2023-07-13 15:02:22.000000 vcf2seq-0.5.0a0/vcf2seq/ascii.py
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)      248 2024-05-03 13:44:44.000000 vcf2seq-0.5.0a0/vcf2seq/info.py
+-rwxr-xr-x   0 benoit    (1001) bio2m     (1010)    11561 2024-05-03 14:01:59.000000 vcf2seq-0.5.0a0/vcf2seq/vcf2seq.py
+drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-05-03 14:57:48.386566 vcf2seq-0.5.0a0/vcf2seq.egg-info/
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)     2231 2024-05-03 14:57:48.000000 vcf2seq-0.5.0a0/vcf2seq.egg-info/PKG-INFO
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)      301 2024-05-03 14:57:48.000000 vcf2seq-0.5.0a0/vcf2seq.egg-info/SOURCES.txt
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)        1 2024-05-03 14:57:48.000000 vcf2seq-0.5.0a0/vcf2seq.egg-info/dependency_links.txt
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)       49 2024-05-03 14:57:48.000000 vcf2seq-0.5.0a0/vcf2seq.egg-info/entry_points.txt
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)        8 2024-05-03 14:57:48.000000 vcf2seq-0.5.0a0/vcf2seq.egg-info/requires.txt
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)        8 2024-05-03 14:57:48.000000 vcf2seq-0.5.0a0/vcf2seq.egg-info/top_level.txt
```

### Comparing `vcf2seq-0.4.1a0/LICENCE.md` & `vcf2seq-0.5.0a0/LICENCE.md`

 * *Files identical despite different names*

### Comparing `vcf2seq-0.4.1a0/PKG-INFO` & `vcf2seq-0.5.0a0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: vcf2seq
-Version: 0.4.1a0
-Summary: like seqTailor, give a VCF file, it return genomic sequence.
+Version: 0.5.0a0
+Summary: Inputing a VCF file, it returns the genomic sequence at the specified length (31 by default).
 Home-page: https://github.com/bio2m/vcf2seq
 Author: Benoit Guibert
 Author-email: benoit.guibert@inserm.fr
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `vcf2seq-0.4.1a0/README.md` & `vcf2seq-0.5.0a0/README.md`

 * *Files identical despite different names*

### Comparing `vcf2seq-0.4.1a0/setup.py` & `vcf2seq-0.5.0a0/setup.py`

 * *Files identical despite different names*

### Comparing `vcf2seq-0.4.1a0/vcf2seq/ascii.py` & `vcf2seq-0.5.0a0/vcf2seq/ascii.py`

 * *Files identical despite different names*

### Comparing `vcf2seq-0.4.1a0/vcf2seq/vcf2seq.py` & `vcf2seq-0.5.0a0/vcf2seq/vcf2seq.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,16 +30,16 @@
     except pyfaidx.FastaNotFoundError as err:
         sys.exit(f"FastaNotFoundError: {err}")
     except OSError as err:
         sys.exit(f"\n{COL.RED}WriteError: directory {os.path.dirname(args.genome)!r} may not be "
                   "writable.\nIf you can't change the rights, you can create a symlink and target "
                   f"it. For example:\n  ln -s {args.genome} $HOME\n{COL.END}")
     vcf_ctrl(args, chr_dict)
-    res_ref, res_alt = compute(args, chr_dict)
-    write(args, res_ref, res_alt)
+    results, warnings = compute(args, chr_dict)
+    write(args, results, warnings)
 
 
 def vcf_ctrl(args, chr_dict):
     with open(args.vcf.name) as fh:
         for row in fh:
             if row.startswith('#'):
                 continue
@@ -58,14 +58,15 @@
                          f"Please, correct your request (or modify the file '{args.genome}.fai').")
             break
 
 
 def compute(args, chr_dict):
     res_ref = []
     res_alt = []
+    warnings = []
     num_row = 0
     cols_id = ascii.get_index(args.add_columns)    # columns chars are converted as index, ex: AA -> 27
     for variant in args.vcf:
         num_row += 1
         if not variant.rstrip('\n') or variant.startswith('#'):
             continue
         fields = variant.rstrip('\n').split('\t')
@@ -79,15 +80,16 @@
         alts = alts.split(',')
         for alt in alts:
 
             header = f">{chr}_{position}_{ref}_{alt}"
 
             ### WARNING: event bigger than kmer size
             if max(len(ref), len(alt)) > args.size :
-                print(f"{COL.PURPLE}Warning: large alteration ({chr}_{position}_{ref}_{alt}), truncated in output.")
+                warnings.append(f"Warning: large alteration ({chr}_{position}_{ref}_{alt}), truncated in output.")
+
 
             ### ERROR: REF base is not valid
             NUC = ["A", "T", "C", "G", args.blank]
             for nuc in (ref[0], alt[0]):
                 if nuc not in NUC:
                     sys.exit(f"{COL.RED}Error: REF base {nuc!r} is not valid "
                             f"(line {num_row}).\n       You might add the '--blank {nuc}' "
@@ -107,27 +109,29 @@
             #        l_alt1     l_alt2       l_alt3                                             #
             #   |------------|-------------|------------|                                       #
             #  ps_alt1                                 pe_alt3                                  #
             #                                                                                   #
             #####################################################################################
 
             ### define some corrections
-            corr_ref = 0 if len(ref)&1 else 1      # if REF length is pair, coor_ref = 1
-            corr_alt = 0 if len(alt)&1 else 1      # if ALT length is pair, coor_alt = 1
-
-            ### missing value for REF or ALT
-            if ref == args.blank:
-                corr_ref += 1
-            if alt == args.blank:
-                corr_alt += 1
+            corr_ref = 0
+            corr_alt = 0
+            if not args.size&1:                                 # k is pair
+                if len(ref)&1 and ref != args.blank: corr_ref += 1  # corr_ref + 1 if REF length is unpair
+                if len(alt)&1 and alt != args.blank: corr_alt += 1  # corr_alt + 1 if ALT length is unpair
+            else:                                               # k is unpair
+                if not len(ref)&1: corr_ref += 1                    # corr_ref + 1 if REF length is pair
+                if not len(alt)&1: corr_alt += 1                    # corr_alt + 1 if ALT length is pair
+                if ref == args.blank: corr_ref += 1                 # missing value for REF
+                if alt == args.blank: corr_alt += 1                 # missing value for ALT
 
             ## define REF kmer
-            l_ref2 = 0 if ref == args.blank else len(ref)
-            l_ref1 = (args.size - l_ref2) // 2
-            l_ref3 = (args.size - l_ref2) // 2 + corr_ref
+            l_ref2  = 0 if ref == args.blank else len(ref)
+            l_ref1  = (args.size - l_ref2) // 2
+            l_ref3  = l_ref1 + corr_ref
             ps_ref2 = int(position)-1                               # -1 for pyfaidx
             ps_ref1 = ps_ref2 - l_ref1
             pe_ref3 = ps_ref2 + l_ref2 + l_ref3
             ref_seq = chr_dict[chr][ps_ref1:pe_ref3]
 
             ## define ALT kmer
             l_alt2 = 0 if alt == args.blank else len(alt)
@@ -141,50 +145,59 @@
             alt = alt if alt != args.blank else ""
             seq_alt3 = chr_dict[chr][ps_alt3:pe_alt3]
             alt_seq = f"{seq_alt1}{alt}{seq_alt3}"
 
             ### WARNING: REF bases must be the same as the calculated position
             seq_ref2 = chr_dict[chr][ps_ref2:ps_ref2+l_ref2]
             if l_ref2 and not ref == seq_ref2:
-                print(f"{COL.PURPLE}Warning: mismatch between REF and genome "
-                         f"at line {num_row} ({chr}:{ps_ref2+1}).\n"
-                         f"          - REF on the vcf file: {ref!r}\n"
-                         f"          - found on the genome: '{seq_ref2}'\n"
-                         f"Please check if the given genome is appropriate.\n{COL.END}")
+                warnings.append("Warning: mismatch between REF and genome "
+                                f"at line {num_row} ({chr}:{ps_ref2+1}).\n"
+                                f"    - REF on the vcf file: {ref!r}\n"
+                                f"    - Found on the genome: '{seq_ref2}'\n"
+                                "    Please check if the given genome is appropriate.\n")
 
             col_txt =  ' '.join([fields[num-1] for num in cols_id])
             if len(ref_seq) == args.size == len(alt_seq):
                 res_ref.append(f"{header}_ref {col_txt}\n{ref_seq}")
                 res_alt.append(f"{header}_alt {col_txt}\n{alt_seq}")
             elif len(alt_seq) > args.size:
-                print(f"{COL.PURPLE}Warning: ALT length ({len(alt_seq)} bp) larger than sequence ({args.size} bp) at line {num_row}, ignored.{COL.END}")
+                warnings.append(f"Warning: ALT length ({len(alt_seq)} bp) larger than sequence ({args.size} bp) at line {num_row}, ignored.")
             else:
-                print(f"{COL.PURPLE}Warning: sequence size not correct at line {num_row}, ignored.{COL.END}")
+                warnings.append(f"Warning: sequence size not correct at line {num_row}, ignored ({len(alt_seq)} != {args.size}).")
 
-    return res_ref, res_alt
+    if args.type == 'alt':
+        res = res_alt
+    elif args.type == 'ref':
+        res = res_ref
+    else:
+        res = list()
+        for i,_ in enumerate(res_alt):
+            res.append(res_ref[i])
+            res.append(res_alt[i])
+    return res, warnings
 
 
-def write(args, res_ref, res_alt):
-    """ Function doc """
-    ### define output file
+
+def write(args, results, warnings):
+    ### RESULTS
+    ## define output file
     if not args.output:
         name, ext = os.path.splitext(os.path.basename(args.vcf.name))
         args.output = f"{name}-vcf2seq.fa"
-    ### write results in file
+    ## write results in file
     with open(args.output, 'w') as fh:
-        if not res_ref:
+        if not results:
             return
-        if args.type == 'alt':
-            fh.write('\n'.join([a for a in res_alt]) + "\n")
-        elif args.type == 'ref':
-            fh.write('\n'.join([a for a in res_ref]) + "\n")
-        elif args.type == 'both':
-            for i, _ in enumerate(res_alt):
-                fh.write(res_ref[i] + '\n')
-                fh.write(res_alt[i] + '\n')
+        fh.write('\n'.join([a for a in results]) + "\n")
+
+    ### WARNINGS
+    if warnings:
+        print(COL.PURPLE)
+        print(*warnings, sep='\n')
+        print(COL.END)
 
 
 class COL:
     PURPLE = '\033[95m'
     CYAN = '\033[96m'
     DARKCYAN = '\033[36m'
     BLUE = '\033[94m'
```

### Comparing `vcf2seq-0.4.1a0/vcf2seq.egg-info/PKG-INFO` & `vcf2seq-0.5.0a0/vcf2seq.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: vcf2seq
-Version: 0.4.1a0
-Summary: like seqTailor, give a VCF file, it return genomic sequence.
+Version: 0.5.0a0
+Summary: Inputing a VCF file, it returns the genomic sequence at the specified length (31 by default).
 Home-page: https://github.com/bio2m/vcf2seq
 Author: Benoit Guibert
 Author-email: benoit.guibert@inserm.fr
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
```


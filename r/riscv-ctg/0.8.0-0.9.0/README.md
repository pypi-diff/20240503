# Comparing `tmp/riscv_ctg-0.8.0.tar.gz` & `tmp/riscv_ctg-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/riscv_ctg-0.8.0.tar", last modified: Sat Aug 13 12:09:02 2022, max compression
+gzip compressed data, was "dist/riscv_ctg-0.9.0.tar", last modified: Mon Aug 29 05:34:39 2022, max compression
```

## Comparing `riscv_ctg-0.8.0.tar` & `riscv_ctg-0.9.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 12:09:02.000000 riscv_ctg-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1532 2022-08-13 12:08:40.000000 riscv_ctg-0.8.0/LICENSE.incore
--rw-r--r--   0 runner    (1001) docker     (121)      237 2022-08-13 12:08:40.000000 riscv_ctg-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      759 2022-08-13 12:09:02.000000 riscv_ctg-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      249 2022-08-13 12:08:40.000000 riscv_ctg-0.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 12:09:02.000000 riscv_ctg-0.8.0/riscv_ctg/
--rw-r--r--   0 runner    (1001) docker     (121)      203 2022-08-13 12:08:40.000000 riscv_ctg-0.8.0/riscv_ctg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8787 2022-08-13 12:08:40.000000 riscv_ctg-0.8.0/riscv_ctg/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     4764 2022-08-13 12:08:40.000000 riscv_ctg-0.8.0/riscv_ctg/ctg.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 12:09:02.000000 riscv_ctg-0.8.0/riscv_ctg/data/
--rw-r--r--   0 runner    (1001) docker     (121)    48637 2022-08-13 12:08:40.000000 riscv_ctg-0.8.0/riscv_ctg/data/fd.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    50978 2022-08-13 12:08:40.000000 riscv_ctg-0.8.0/riscv_ctg/data/imc.yaml
--rw-r--r--   0 runner    (1001) docker     (121)   276828 2022-08-13 12:08:40.000000 riscv_ctg-0.8.0/riscv_ctg/data/template.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     8723 2022-08-13 12:08:40.000000 riscv_ctg-0.8.0/riscv_ctg/dsp_function.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 12:09:02.000000 riscv_ctg-0.8.0/riscv_ctg/env/
--rw-r--r--   0 runner    (1001) docker     (121)    65947 2022-08-13 12:08:40.000000 riscv_ctg-0.8.0/riscv_ctg/env/arch_test.h
--rw-r--r--   0 runner    (1001) docker     (121)    53135 2022-08-13 12:08:40.000000 riscv_ctg-0.8.0/riscv_ctg/env/encoding.h
--rw-r--r--   0 runner    (1001) docker     (121)     8105 2022-08-13 12:08:40.000000 riscv_ctg-0.8.0/riscv_ctg/function_generators.py
--rw-r--r--   0 runner    (1001) docker     (121)    56360 2022-08-13 12:08:40.000000 riscv_ctg-0.8.0/riscv_ctg/generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2390 2022-08-13 12:08:40.000000 riscv_ctg-0.8.0/riscv_ctg/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     3080 2022-08-13 12:08:40.000000 riscv_ctg-0.8.0/riscv_ctg/log.py
--rw-r--r--   0 runner    (1001) docker     (121)     1642 2022-08-13 12:08:40.000000 riscv_ctg-0.8.0/riscv_ctg/main.py
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-08-13 12:08:40.000000 riscv_ctg-0.8.0/riscv_ctg/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)    10384 2022-08-13 12:08:40.000000 riscv_ctg-0.8.0/riscv_ctg/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 12:09:02.000000 riscv_ctg-0.8.0/riscv_ctg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      759 2022-08-13 12:09:02.000000 riscv_ctg-0.8.0/riscv_ctg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      661 2022-08-13 12:09:02.000000 riscv_ctg-0.8.0/riscv_ctg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-13 12:09:02.000000 riscv_ctg-0.8.0/riscv_ctg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-08-13 12:09:02.000000 riscv_ctg-0.8.0/riscv_ctg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-13 12:09:02.000000 riscv_ctg-0.8.0/riscv_ctg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-08-13 12:09:02.000000 riscv_ctg-0.8.0/riscv_ctg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-08-13 12:09:02.000000 riscv_ctg-0.8.0/riscv_ctg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      392 2022-08-13 12:09:02.000000 riscv_ctg-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1562 2022-08-13 12:08:40.000000 riscv_ctg-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-29 05:34:39.000000 riscv_ctg-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1532 2022-08-29 05:34:21.000000 riscv_ctg-0.9.0/LICENSE.incore
+-rw-r--r--   0 runner    (1001) docker     (121)      237 2022-08-29 05:34:21.000000 riscv_ctg-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      759 2022-08-29 05:34:39.000000 riscv_ctg-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      249 2022-08-29 05:34:21.000000 riscv_ctg-0.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-29 05:34:39.000000 riscv_ctg-0.9.0/riscv_ctg/
+-rw-r--r--   0 runner    (1001) docker     (121)      203 2022-08-29 05:34:21.000000 riscv_ctg-0.9.0/riscv_ctg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9295 2022-08-29 05:34:21.000000 riscv_ctg-0.9.0/riscv_ctg/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21417 2022-08-29 05:34:21.000000 riscv_ctg-0.9.0/riscv_ctg/cross_comb.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4949 2022-08-29 05:34:21.000000 riscv_ctg-0.9.0/riscv_ctg/ctg.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-29 05:34:39.000000 riscv_ctg-0.9.0/riscv_ctg/data/
+-rw-r--r--   0 runner    (1001) docker     (121)    48637 2022-08-29 05:34:21.000000 riscv_ctg-0.9.0/riscv_ctg/data/fd.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    50978 2022-08-29 05:34:21.000000 riscv_ctg-0.9.0/riscv_ctg/data/imc.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)   276828 2022-08-29 05:34:21.000000 riscv_ctg-0.9.0/riscv_ctg/data/template.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     8723 2022-08-29 05:34:21.000000 riscv_ctg-0.9.0/riscv_ctg/dsp_function.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-29 05:34:39.000000 riscv_ctg-0.9.0/riscv_ctg/env/
+-rw-r--r--   0 runner    (1001) docker     (121)    65947 2022-08-29 05:34:21.000000 riscv_ctg-0.9.0/riscv_ctg/env/arch_test.h
+-rw-r--r--   0 runner    (1001) docker     (121)    53135 2022-08-29 05:34:21.000000 riscv_ctg-0.9.0/riscv_ctg/env/encoding.h
+-rw-r--r--   0 runner    (1001) docker     (121)     8105 2022-08-29 05:34:21.000000 riscv_ctg-0.9.0/riscv_ctg/function_generators.py
+-rw-r--r--   0 runner    (1001) docker     (121)    56361 2022-08-29 05:34:21.000000 riscv_ctg-0.9.0/riscv_ctg/generator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2390 2022-08-29 05:34:21.000000 riscv_ctg-0.9.0/riscv_ctg/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3080 2022-08-29 05:34:21.000000 riscv_ctg-0.9.0/riscv_ctg/log.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1642 2022-08-29 05:34:21.000000 riscv_ctg-0.9.0/riscv_ctg/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)       72 2022-08-29 05:34:21.000000 riscv_ctg-0.9.0/riscv_ctg/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    11327 2022-08-29 05:34:21.000000 riscv_ctg-0.9.0/riscv_ctg/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-29 05:34:39.000000 riscv_ctg-0.9.0/riscv_ctg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      759 2022-08-29 05:34:39.000000 riscv_ctg-0.9.0/riscv_ctg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      685 2022-08-29 05:34:39.000000 riscv_ctg-0.9.0/riscv_ctg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-29 05:34:39.000000 riscv_ctg-0.9.0/riscv_ctg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       50 2022-08-29 05:34:39.000000 riscv_ctg-0.9.0/riscv_ctg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-29 05:34:39.000000 riscv_ctg-0.9.0/riscv_ctg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       72 2022-08-29 05:34:39.000000 riscv_ctg-0.9.0/riscv_ctg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-08-29 05:34:39.000000 riscv_ctg-0.9.0/riscv_ctg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      392 2022-08-29 05:34:39.000000 riscv_ctg-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1562 2022-08-29 05:34:21.000000 riscv_ctg-0.9.0/setup.py
```

### Comparing `riscv_ctg-0.8.0/LICENSE.incore` & `riscv_ctg-0.9.0/LICENSE.incore`

 * *Files identical despite different names*

### Comparing `riscv_ctg-0.8.0/PKG-INFO` & `riscv_ctg-0.9.0/riscv_ctg.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
-Name: riscv_ctg
-Version: 0.8.0
+Name: riscv-ctg
+Version: 0.9.0
 Summary: RISC-V CTG
 Home-page: https://github.com/riscv/riscv-ctg
 Author: InCore Semiconductors Pvt. Ltd.
 Author-email: info@incoresemi.com
 License: BSD-3-Clause
 Description: #################################################
         **RISC-V Compliance Test Generator** : RISC-V CTG
```

### Comparing `riscv_ctg-0.8.0/riscv_ctg/constants.py` & `riscv_ctg-0.9.0/riscv_ctg/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -213,14 +213,18 @@
 // -----------
 //'''
 
 comment_template = '''
 // This assembly file tests the $opcode instruction of the RISC-V $extension extension for the $label covergroup.
 // '''
 
+cross_comment_template = '''
+// This assembly file is used for the test of cross-combination coverpoint described in $label covergroup.
+'''
+
 test_template = Template(copyright_string + comment_template+'''
 #include "model_test.h"
 #include "arch_test.h"
 RVTEST_ISA("$isa")
 
 .section .text.init
 .globl rvtest_entry_point
@@ -236,14 +240,39 @@
 $data
 RVTEST_DATA_END
 
 RVMODEL_DATA_BEGIN
 $sig
 RVMODEL_DATA_END
 ''')
+
+cross_test_template = Template(copyright_string + cross_comment_template+'''
+#include "model_test.h"
+#include "arch_test.h"
+RVTEST_ISA("$isa")
+
+.section .text.init
+.globl rvtest_entry_point
+rvtest_entry_point:
+RVMODEL_BOOT
+RVTEST_CODE_BEGIN
+$test
+
+RVTEST_CODE_END
+RVMODEL_HALT
+
+RVTEST_DATA_BEGIN
+$data
+RVTEST_DATA_END
+
+RVMODEL_DATA_BEGIN
+$sig
+RVMODEL_DATA_END
+''')
+
 case_template = Template('''
 RVTEST_CASE($num,"//$cond;def TEST_CASE_1=True;",$cov_label)
 ''')
 
 part_template = Template('''
 #ifdef TEST_CASE_1
 $case_str
```

### Comparing `riscv_ctg-0.8.0/riscv_ctg/ctg.py` & `riscv_ctg-0.9.0/riscv_ctg/ctg.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import time
 import shutil
 from riscv_ctg.log import logger
 import riscv_ctg.utils as utils
 import riscv_ctg.constants as const
 from riscv_isac.cgf_normalize import expand_cgf
 from riscv_ctg.generator import Generator
+from riscv_ctg.cross_comb import cross
 from math import *
 from riscv_ctg.__init__ import __version__
 
 def create_test(usage_str, node,label,base_isa,max_inst, op_template, randomize, out_dir, xlen, flen):
     iflen = 0
     if 'mnemonics' not in node:
         logger.warning("mnemonics node not found in covergroup: " + str(label))
@@ -57,14 +58,15 @@
     if 'base_op' in node:
         # Extract pseudo and base instructions
         base_op = node['base_op']
         pseudop = list(node['mnemonics'].keys())[0]
         if base_op in op_template and pseudop in op_template:
             op_node = copy.deepcopy(op_template[base_op])
             pseudo_template = op_template[pseudop]
+
             # Ovewrite/add nodes from pseudoinstruction template in base instruction template
             for key, val in pseudo_template.items():
                 op_node[key] = val
 
             # Generate tests
             gen_test(op_node, pseudop)
     else:
@@ -73,15 +75,23 @@
                 op_node = op_template[opcode]
                 # Generate tests
                 gen_test(op_node, opcode)
             else:
                 logger.warning(str(opcode) + " not found in template file. Skipping")
                 return
 
+    if 'cross_comb' in node:
+        fprefix = os.path.join(out_dir,str(label))
+        cross_obj = cross(base_isa, xlen, randomize, label)
+        cross_instr_dict = cross_obj.cross_comb(node)
+        logger.info('Writing cross-comb test')
+        cross_obj.write_test(fprefix, node, usage_str, label, cross_instr_dict)
+
     # Return if there is no corresponding template
+
     if op_node is None:
         logger.warning("Skipping :" + str(opcode))
         return
 
 def ctg(verbose, out, random ,xlen_arg,flen_arg, cgf_file,num_procs,base_isa, max_inst):
     logger.level(verbose)
     logger.info('****** RISC-V Compliance Test Generator {0} *******'.format(__version__ ))
@@ -104,15 +114,10 @@
         randomize_argument = ' \\\n//                  --randomize'
     usage_str = const.usage.safe_substitute(base_isa=base_isa, \
             cgf=cgf_argument, version = __version__, time=mytime, \
             randomize=randomize_argument,xlen=str(xlen_arg))
     op_template = utils.load_yamls(const.template_files)
     cgf = expand_cgf(cgf_file,xlen,flen)
     pool = mp.Pool(num_procs)
-# <<<<<<< HEAD
-    # results = pool.starmap(create_test, [(usage_str, node,label,base_isa,max_inst) for label,node in cgf.items()])
-    # pool.close()
-# =======
     results = pool.starmap(create_test, [(usage_str, node,label,base_isa,max_inst, op_template,
         randomize, out_dir, xlen, flen) for label,node in cgf.items()])
     pool.close()
-# >>>>>>> master
```

### Comparing `riscv_ctg-0.8.0/riscv_ctg/data/fd.yaml` & `riscv_ctg-0.9.0/riscv_ctg/data/fd.yaml`

 * *Files identical despite different names*

### Comparing `riscv_ctg-0.8.0/riscv_ctg/data/imc.yaml` & `riscv_ctg-0.9.0/riscv_ctg/data/imc.yaml`

 * *Files identical despite different names*

### Comparing `riscv_ctg-0.8.0/riscv_ctg/data/template.yaml` & `riscv_ctg-0.9.0/riscv_ctg/data/template.yaml`

 * *Files identical despite different names*

### Comparing `riscv_ctg-0.8.0/riscv_ctg/dsp_function.py` & `riscv_ctg-0.9.0/riscv_ctg/dsp_function.py`

 * *Files identical despite different names*

### Comparing `riscv_ctg-0.8.0/riscv_ctg/env/arch_test.h` & `riscv_ctg-0.9.0/riscv_ctg/env/arch_test.h`

 * *Files identical despite different names*

### Comparing `riscv_ctg-0.8.0/riscv_ctg/env/encoding.h` & `riscv_ctg-0.9.0/riscv_ctg/env/encoding.h`

 * *Files identical despite different names*

### Comparing `riscv_ctg-0.8.0/riscv_ctg/function_generators.py` & `riscv_ctg-0.9.0/riscv_ctg/function_generators.py`

 * *Files identical despite different names*

### Comparing `riscv_ctg-0.8.0/riscv_ctg/generator.py` & `riscv_ctg-0.9.0/riscv_ctg/generator.py`

 * *Files identical despite different names*

```diff
@@ -811,14 +811,15 @@
                 if var_dict['rs3'] in coverpoints['rs3']:
                     cover_hits['rs3'] = set([var_dict['rs3']])
             if 'rd' in coverpoints:
                 if var_dict['rd'] in coverpoints['rd']:
                     cover_hits['rd'] = set([var_dict['rd']])
             return cover_hits
         i = 0
+
         if not self.is_fext:
             for instr in instr_dict:
                 unique = False
                 skip_val = False
                 if instr['inst'] in cgf['mnemonics']:
                     if 'rs1' in instr and 'rs2' in instr:
                         if instr['rs1'] == instr['rs2']:
```

### Comparing `riscv_ctg-0.8.0/riscv_ctg/helpers.py` & `riscv_ctg-0.9.0/riscv_ctg/helpers.py`

 * *Files identical despite different names*

### Comparing `riscv_ctg-0.8.0/riscv_ctg/log.py` & `riscv_ctg-0.9.0/riscv_ctg/log.py`

 * *Files identical despite different names*

### Comparing `riscv_ctg-0.8.0/riscv_ctg/main.py` & `riscv_ctg-0.9.0/riscv_ctg/main.py`

 * *Files identical despite different names*

### Comparing `riscv_ctg-0.8.0/riscv_ctg/utils.py` & `riscv_ctg-0.9.0/riscv_ctg/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import sys
 import os
 import subprocess
 import shlex
 from riscv_ctg.log import logger
 import ruamel
 from ruamel.yaml import YAML
+from collections import defaultdict
+import riscv_ctg.constants as const
 from riscv_isac.utils import combineReader
 
 yaml = YAML(typ="rt")
 yaml.default_flow_style = False
 yaml.allow_unicode = True
 
 def load_yaml(foo):
@@ -20,14 +22,48 @@
             return dict(yaml.load(file))
     except ruamel.yaml.constructor.DuplicateKeyError as msg:
         logger = logging.getLogger(__name__)
         error = "\n".join(str(msg).split("\n")[2:-7])
         logger.error(error)
         raise SystemExit
 
+def gen_format_data():
+    '''
+    Generate dictionary from template.yaml file with the structure:
+    Format:
+        - ISA
+            - Mnemonics
+    '''    
+    op_template = load_yaml(const.template_file)
+
+    # Initialize nested dictionary
+    nested_dict = lambda: defaultdict(nested_dict)
+    format_dict = nested_dict()
+    
+    for mnemonic, data in op_template.items():
+        if mnemonic not in ['metadata']:
+            format_type = data['formattype']
+            isa = data['isa']
+
+            for each in isa:
+                format_dict[format_type][each][mnemonic] = None
+            
+    return format_dict
+
+def get_instr_list():
+    '''
+    Get list of all instructions defined in template file
+    '''
+    op_template = load_yaml(const.template_file)
+
+    instr_lst = list(op_template.keys())
+    instr_lst.remove('metadata')
+
+    return instr_lst
+
 def load_yamls(foo):
     with combineReader(foo) as fp:
         return dict(yaml.load(fp))
 
 class makeUtil():
     """
     Utility for ease of use of make commands like `make` and `pmake`.
```

### Comparing `riscv_ctg-0.8.0/riscv_ctg.egg-info/PKG-INFO` & `riscv_ctg-0.9.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
-Name: riscv-ctg
-Version: 0.8.0
+Name: riscv_ctg
+Version: 0.9.0
 Summary: RISC-V CTG
 Home-page: https://github.com/riscv/riscv-ctg
 Author: InCore Semiconductors Pvt. Ltd.
 Author-email: info@incoresemi.com
 License: BSD-3-Clause
 Description: #################################################
         **RISC-V Compliance Test Generator** : RISC-V CTG
```

### Comparing `riscv_ctg-0.8.0/riscv_ctg.egg-info/SOURCES.txt` & `riscv_ctg-0.9.0/riscv_ctg.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE.incore
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 riscv_ctg/__init__.py
 riscv_ctg/constants.py
+riscv_ctg/cross_comb.py
 riscv_ctg/ctg.py
 riscv_ctg/dsp_function.py
 riscv_ctg/function_generators.py
 riscv_ctg/generator.py
 riscv_ctg/helpers.py
 riscv_ctg/log.py
 riscv_ctg/main.py
```

### Comparing `riscv_ctg-0.8.0/setup.py` & `riscv_ctg-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 setup_requirements = [ ]
 
 test_requirements = [ ]
 
 setup(
     name='riscv_ctg',
-    version='0.8.0',
+    version='0.9.0',
     description="RISC-V CTG",
     long_description=readme + '\n\n',
     classifiers=[
           "Programming Language :: Python :: 3.6",
           "License :: OSI Approved :: BSD License",
           "Development Status :: 4 - Beta"
     ],
```


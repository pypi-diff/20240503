# Comparing `tmp/slurmgen-3.2.0.tar.gz` & `tmp/slurmgen-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slurmgen-3.2.0.tar", last modified: Sat Mar 30 02:47:51 2024, max compression
+gzip compressed data, was "slurmgen-3.3.3.tar", last modified: Fri May  3 05:55:35 2024, max compression
```

## Comparing `slurmgen-3.2.0.tar` & `slurmgen-3.3.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-03-30 02:47:51.215095 slurmgen-3.2.0/
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      278 2023-11-27 16:21:41.000000 slurmgen-3.2.0/.gitignore
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)     1303 2023-11-27 14:39:14.000000 slurmgen-3.2.0/LICENSE.txt
--rw-r--r--   0 tguillod  (1000) tguillod  (1000)     3106 2024-03-30 02:47:51.215095 slurmgen-3.2.0/PKG-INFO
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)     2093 2024-03-30 02:44:17.000000 slurmgen-3.2.0/README.md
-drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-03-30 02:47:51.215095 slurmgen-3.2.0/example/
-drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-03-30 02:47:51.215095 slurmgen-3.2.0/example/data_output/
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)       57 2024-03-30 02:45:48.000000 slurmgen-3.2.0/example/data_output/goodbye.txt
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)       55 2024-03-30 02:45:48.000000 slurmgen-3.2.0/example/data_output/hello.txt
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      943 2024-03-30 01:45:14.000000 slurmgen-3.2.0/example/job_def.json
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)       57 2024-03-21 18:33:57.000000 slurmgen-3.2.0/example/job_tmpl.json
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)     1027 2023-11-27 20:00:16.000000 slurmgen-3.2.0/example/run_slurm.py
-drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-03-30 02:47:51.215095 slurmgen-3.2.0/example/slurm_output/
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      756 2024-03-30 02:45:48.000000 slurmgen-3.2.0/example/slurm_output/test.log
--rwxrw-r--   0 tguillod  (1000) tguillod  (1000)     1277 2024-03-30 02:45:48.000000 slurmgen-3.2.0/example/slurm_output/test.sh
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)     1573 2024-01-31 21:49:48.000000 slurmgen-3.2.0/pyproject.toml
--rwxrwxr-x   0 tguillod  (1000) tguillod  (1000)     1719 2023-11-27 16:21:41.000000 slurmgen-3.2.0/run_release.sh
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)       38 2024-03-30 02:47:51.215095 slurmgen-3.2.0/setup.cfg
-drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-03-30 02:47:51.215095 slurmgen-3.2.0/slurmgen/
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)        0 2023-11-27 15:07:42.000000 slurmgen-3.2.0/slurmgen/__init__.py
--rwxrwxr-x   0 tguillod  (1000) tguillod  (1000)     8345 2024-03-29 21:28:31.000000 slurmgen-3.2.0/slurmgen/gen.py
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)     3027 2023-12-06 17:36:44.000000 slurmgen-3.2.0/slurmgen/run.py
--rwxrwxr-x   0 tguillod  (1000) tguillod  (1000)     7432 2024-03-30 02:47:05.000000 slurmgen-3.2.0/slurmgen/script.py
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)        5 2024-03-30 02:47:51.000000 slurmgen-3.2.0/slurmgen/version.txt
-drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-03-30 02:47:51.215095 slurmgen-3.2.0/slurmgen.egg-info/
--rw-r--r--   0 tguillod  (1000) tguillod  (1000)     3106 2024-03-30 02:47:51.000000 slurmgen-3.2.0/slurmgen.egg-info/PKG-INFO
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      503 2024-03-30 02:47:51.000000 slurmgen-3.2.0/slurmgen.egg-info/SOURCES.txt
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)        1 2024-03-30 02:47:51.000000 slurmgen-3.2.0/slurmgen.egg-info/dependency_links.txt
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)       52 2024-03-30 02:47:51.000000 slurmgen-3.2.0/slurmgen.egg-info/entry_points.txt
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)        9 2024-03-30 02:47:51.000000 slurmgen-3.2.0/slurmgen.egg-info/top_level.txt
+drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-05-03 05:55:35.321225 slurmgen-3.3.3/
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      278 2023-11-27 16:21:41.000000 slurmgen-3.3.3/.gitignore
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)     1303 2023-11-27 14:39:14.000000 slurmgen-3.3.3/LICENSE.txt
+-rw-r--r--   0 tguillod  (1000) tguillod  (1000)     3106 2024-05-03 05:55:35.321225 slurmgen-3.3.3/PKG-INFO
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)     2093 2024-03-30 02:44:17.000000 slurmgen-3.3.3/README.md
+drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-05-03 05:55:35.321225 slurmgen-3.3.3/example/
+drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-05-03 05:55:35.321225 slurmgen-3.3.3/example/data_output/
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)       57 2024-05-03 05:48:48.000000 slurmgen-3.3.3/example/data_output/goodbye.txt
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)       55 2024-05-03 05:48:48.000000 slurmgen-3.3.3/example/data_output/hello.txt
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      866 2024-05-03 05:48:33.000000 slurmgen-3.3.3/example/job_def.json
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)       57 2024-03-21 18:33:57.000000 slurmgen-3.3.3/example/job_tmpl.json
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)     1027 2023-11-27 20:00:16.000000 slurmgen-3.3.3/example/run_slurm.py
+drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-05-03 05:55:35.321225 slurmgen-3.3.3/example/slurm_output/
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      756 2024-05-03 05:48:48.000000 slurmgen-3.3.3/example/slurm_output/test.log
+-rwxrw-r--   0 tguillod  (1000) tguillod  (1000)     1277 2024-05-03 05:48:48.000000 slurmgen-3.3.3/example/slurm_output/test.sh
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)     1566 2024-05-03 05:50:27.000000 slurmgen-3.3.3/pyproject.toml
+-rwxrwxr-x   0 tguillod  (1000) tguillod  (1000)     1719 2023-11-27 16:21:41.000000 slurmgen-3.3.3/run_release.sh
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)       38 2024-05-03 05:55:35.321225 slurmgen-3.3.3/setup.cfg
+drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-05-03 05:55:35.321225 slurmgen-3.3.3/slurmgen/
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      176 2024-05-03 05:52:06.000000 slurmgen-3.3.3/slurmgen/__init__.py
+-rwxrwxr-x   0 tguillod  (1000) tguillod  (1000)     8457 2024-05-03 05:48:32.000000 slurmgen-3.3.3/slurmgen/gen.py
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)     2970 2024-05-03 05:36:54.000000 slurmgen-3.3.3/slurmgen/run.py
+-rwxrwxr-x   0 tguillod  (1000) tguillod  (1000)     6753 2024-05-03 05:52:06.000000 slurmgen-3.3.3/slurmgen/script.py
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)        5 2024-05-03 05:55:35.000000 slurmgen-3.3.3/slurmgen/version.txt
+drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-05-03 05:55:35.321225 slurmgen-3.3.3/slurmgen.egg-info/
+-rw-r--r--   0 tguillod  (1000) tguillod  (1000)     3106 2024-05-03 05:55:35.000000 slurmgen-3.3.3/slurmgen.egg-info/PKG-INFO
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      503 2024-05-03 05:55:35.000000 slurmgen-3.3.3/slurmgen.egg-info/SOURCES.txt
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)        1 2024-05-03 05:55:35.000000 slurmgen-3.3.3/slurmgen.egg-info/dependency_links.txt
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)       45 2024-05-03 05:55:35.000000 slurmgen-3.3.3/slurmgen.egg-info/entry_points.txt
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)        9 2024-05-03 05:55:35.000000 slurmgen-3.3.3/slurmgen.egg-info/top_level.txt
```

### Comparing `slurmgen-3.2.0/LICENSE.txt` & `slurmgen-3.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `slurmgen-3.2.0/PKG-INFO` & `slurmgen-3.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurmgen
-Version: 3.2.0
+Version: 3.3.3
 Summary: SlurmGen - Simple Slurm Manager
 Author-email: Thomas Guillod <guillod@otvam.ch>
 Maintainer-email: Thomas Guillod <guillod@otvam.ch>
 License: BSD-2-Clause
 Project-URL: Homepage, https://github.com/otvam/slurmgen
 Project-URL: Repository, https://github.com/otvam/slurmgen
 Project-URL: Releases, https://github.com/otvam/slurmgen/releases
```

### Comparing `slurmgen-3.2.0/README.md` & `slurmgen-3.3.3/README.md`

 * *Files identical despite different names*

### Comparing `slurmgen-3.2.0/example/job_def.json` & `slurmgen-3.3.3/example/job_def.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7142857142857143%*

 * *Differences: {"'overwrite'": 'True', 'delete': "['control']"}*

```diff
@@ -22,28 +22,24 @@
                 "goodbye",
                 "goodbye world!"
             ],
             "executable": "python3",
             "tag": "goodbye"
         }
     ],
-    "control": {
-        "cluster": false,
-        "local": false,
-        "overwrite": true
-    },
     "folder": {
         "folder_create": [
             "data_output"
         ],
         "folder_delete": [
             "data_output"
         ],
         "folder_output": "slurm_output"
     },
+    "overwrite": true,
     "pragmas": {
         "mem": "8G",
         "nodes": "1",
         "ntasks-per-node": "2",
         "time": "4:00:00"
     },
     "tag": "$title",
```

### Comparing `slurmgen-3.2.0/example/run_slurm.py` & `slurmgen-3.3.3/example/run_slurm.py`

 * *Files identical despite different names*

### Comparing `slurmgen-3.2.0/example/slurm_output/test.log` & `slurmgen-3.3.3/example/slurm_output/test.log`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-================================== test - 03/30/24 02:45:48
+================================== test - 05/03/24 05:48:48
 ==================== PARAM
 JOB TAG      : test
 LOG FILE     : slurm_output/test.log
 SCRIPT FILE  : slurm_output/test.sh
 ==================== TIME
-DATE GEN     : 03/30/24 02:45:48
-DATE RUN     : 03/30/24 02:45:48
+DATE GEN     : 05/03/24 05:48:48
+DATE RUN     : 05/03/24 05:48:48
 ==================== SLURM
 JOB ID       : NOT SLURM
 JOB NAME     : NOT SLURM
 JOB NODE     : NOT SLURM
 ==================== ENV VAR
 ==================== RUN: version
 Python 3.10.12
@@ -19,8 +19,8 @@
     VARWORLD = Welcome to everyone
 exit script
 ==================== RUN: goodbye
 enter script
     ARGUMENT = goodbye world!
     VARWORLD = Welcome to everyone
 exit script
-================================== test - 03/30/24 02:45:48
+================================== test - 05/03/24 05:48:48
```

### Comparing `slurmgen-3.2.0/example/slurm_output/test.sh` & `slurmgen-3.3.3/example/slurm_output/test.sh`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 echo "==================== PARAM"
 echo "JOB TAG      : test"
 echo "LOG FILE     : slurm_output/test.log"
 echo "SCRIPT FILE  : slurm_output/test.sh"
 
 echo "==================== TIME"
-echo "DATE GEN     : 03/30/24 02:45:48"
+echo "DATE GEN     : 05/03/24 05:48:48"
 echo "DATE RUN     : `date -u +"%D %H:%M:%S"`"
 
 echo "==================== SLURM"
 echo "JOB ID       : $SLURM_JOB_ID"
 echo "JOB NAME     : $SLURM_JOB_NAME"
 echo "JOB NODE     : $SLURM_JOB_NODELIST"
```

### Comparing `slurmgen-3.2.0/pyproject.toml` & `slurmgen-3.3.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 Tags = "https://github.com/otvam/slurmgen/tags"
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
 
 [project.scripts]
-sgen = "slurmgen.script:run_script"
+sgen = "slurmgen:run_script"
 
 [tool.setuptools]
 packages = ["slurmgen"]
 license-files = ["LICENSE.txt"]
 include-package-data = true
 
 [tool.setuptools.package-data]
```

### Comparing `slurmgen-3.2.0/run_release.sh` & `slurmgen-3.3.3/run_release.sh`

 * *Files identical despite different names*

### Comparing `slurmgen-3.2.0/slurmgen/gen.py` & `slurmgen-3.3.3/slurmgen/gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,16 @@
 
     fid.write('#!/bin/bash\n')
     fid.write('\n')
     fid.write('# ############### define Slurm commands\n')
     fid.write('#SBATCH --job-name="%s"\n' % tag)
     fid.write('#SBATCH --output="%s"\n' % filename_log)
     for tag, val in pragmas.items():
-        fid.write('#SBATCH --%s="%s"\n' % (tag, val))
+        if (tag is not None) and (val is not None):
+            fid.write('#SBATCH --%s="%s"\n' % (tag, val))
     fid.write('\n')
     fid.write('# ############### init exit code\n')
     fid.write('ret=0\n')
     fid.write('\n')
 
 
 def _write_summary(fid, tag, filename_script, filename_log):
@@ -123,16 +124,17 @@
         File descriptor for the script.
     vars : dict
         Dictionary of environment variable to be set and exported.
     """
 
     if var:
         fid.write('echo "==================== ENV VAR"\n')
-        for var, value in var.items():
-            fid.write('export %s="%s"\n' % (var, value))
+        for var, val in var.items():
+            if (var is not None) and (val is not None):
+                fid.write('export %s="%s"\n' % (var, val))
         fid.write('\n')
 
 
 def _write_commands(fid, commands):
     """
     Add a command to the Slurm script.
```

### Comparing `slurmgen-3.2.0/slurmgen/run.py` & `slurmgen-3.3.3/slurmgen/run.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,104 +8,113 @@
 
 import sys
 import stat
 import os.path
 import subprocess
 
 
-def _run_cmd(command, filename_log, env, write_log):
+def _run_cmd_raw(command, env):
     """
     Run a Slurm script.
 
     Parameters
     ----------
     command : list
         Command to be executed.
-    filename_log : string
-        Path of the log file created by during the Slurm job.
     env : dict
         Dictionary with the environment variables.
     write_log : bool
         Write (or not) the output in a log file.
     """
 
     # run the command
     try:
-        if write_log:
-            with open(filename_log, "w") as fid:
-                process = subprocess.run(
-                    command,
-                    env=env,
-                    stderr=fid,
-                    stdout=fid,
-                )
-        else:
+        process = subprocess.run(
+            command,
+            env=env,
+        )
+    except OSError:
+        print("error: command not found", file=sys.stderr)
+        sys.exit(1)
+
+    # check return code
+    if process.returncode == 0:
+        print("info: valid return code")
+    else:
+        print("error: invalid return code", file=sys.stderr)
+        sys.exit(process.returncode)
+
+
+def _run_cmd_log(command, filename_log, env):
+    """
+    Run a Slurm script.
+
+    Parameters
+    ----------
+    command : list
+        Command to be executed.
+    filename_log : string
+        Path of the log file created by during the Slurm job.
+    env : dict
+        Dictionary with the environment variables.
+    """
+
+    # run the command
+    try:
+        with open(filename_log, "w") as fid:
             process = subprocess.run(
                 command,
                 env=env,
+                stderr=fid,
+                stdout=fid,
             )
     except OSError:
         print("error: command not found", file=sys.stderr)
         sys.exit(1)
 
     # check return code
     if process.returncode == 0:
         print("info: valid return code")
     else:
         print("error: invalid return code", file=sys.stderr)
         sys.exit(process.returncode)
 
 
-def run_data(filename_script, filename_log, local, cluster, afterok, afterany):
+def run_data(filename_script, filename_log, local, cluster):
     """
     Run a Slurm script.
 
     Parameters
     ----------
     filename_script : string
         Path of the script controlling the simulation.
     filename_log : string
         Path of the log file created by during the Slurm job.
     local : bool
         Run (or not) the job locally.
     cluster : bool
         Run (or not) the job on the cluster.
-    afterok : string
-        Job ids in the successful dependency list.
-    afterany : string
-        Job ids in the terminated dependency list.
     """
 
     # make the script executable
     st = os.stat(filename_script)
     os.chmod(filename_script, st.st_mode | stat.S_IEXEC)
 
     # submit Slurm job
     if cluster:
         print("info: run Slurm job")
 
         # find env
         env = os.environ.copy()
 
-        # find dependencies
-        dep = []
-        if afterok is not None:
-            dep.append("afterok:%s" % afterok)
-        if afterany is not None:
-            dep.append("afterany:%s" % afterany)
-
         # find command
-        if dep:
-            dep = ",".join(dep)
-            command = ["sbatch", "--dependency=" + dep, filename_script]
-        else:
-            command = ["sbatch", filename_script]
+        command = ["sbatch", filename_script]
 
         # run
-        _run_cmd(command, filename_log, env, False)
+        _run_cmd_raw(command, env)
 
     # run locally
     if local:
         print("info: run Shell job")
 
         # find env
         env = os.environ.copy()
@@ -113,8 +122,8 @@
         env["SLURM_JOB_NAME"] = "NOT SLURM"
         env["SLURM_JOB_NODELIST"] = "NOT SLURM"
 
         # find command
         command = [filename_script]
 
         # run
-        _run_cmd(command, filename_log, env, True)
+        _run_cmd_log(command, filename_log, env)
```

### Comparing `slurmgen-3.2.0/slurmgen/script.py` & `slurmgen-3.3.3/slurmgen/script.py`

 * *Files 9% similar despite different names*

```diff
@@ -67,57 +67,28 @@
     )
     parser.add_argument(
         "-c", "--cluster",
         help="Run the job on the Slurm cluster",
         action="store_true",
         dest="cluster",
     )
-    parser.add_argument(
-        "-o", "--overwrite",
-        help="Overwrite existing files",
-        action="store_true",
-        dest="cluster",
-    )
-    parser.add_argument(
-        "-t", "--tag",
-        help="Overwrite the job name",
-        action="store",
-        dest="tag",
-        default=None,
-    )
-
-    # add dependency options
-    parser.add_argument(
-        "-ok", "--afterok",
-        help="Run after successful dependency",
-        action="store",
-        dest="afterok",
-        default=None,
-    )
-    parser.add_argument(
-        "-any", "--afterany",
-        help="Run after terminated dependency",
-        action="store",
-        dest="afterany",
-        default=None,
-    )
 
     return parser
 
 
 def _get_template(tmpl_file, tmpl_str):
     """
     Load the template data (from file and from string).
 
     Parameters
     ----------
     tmpl_file : string
         String with a JSON file containing template data.
-    tmpl_str : string
-        String with a Python dictionary containing template data.
+    tmpl_str : list
+        List with keys/values containing template data.
 
     Returns
     -------
     tmpl_data : dict
         Dictionary with the parsed template data.
     """
 
@@ -195,17 +166,17 @@
         print("error: definition file not found", file=sys.stderr)
         sys.exit(1)
 
     # show template content
     if tmpl_data:
         print("info: template content")
         for tag, val in tmpl_data.items():
-            print("info: var: \"%s\" : \"%s\"" % (tag, val))
+            print("info: var: \"%s\" => \"%s\"" % (tag, val))
 
-    # appy the template
+    # apply the template
     try:
         obj = string.Template(data_raw)
         def_data = obj.substitute(tmpl_data)
     except (ValueError, KeyError) as ex:
         print("error: template parsing error: %s" % str(ex), file=sys.stderr)
         sys.exit(1)
 
@@ -215,72 +186,78 @@
     except json.JSONDecodeError as ex:
         print("error: definition file is invalid: %s" % str(ex), file=sys.stderr)
         sys.exit(1)
 
     return def_data
 
 
+def run_args(def_file, tmpl_file=None, tmpl_str=None, local=False, cluster=False):
+    """
+    Run the script with arguments.
+
+    Parameters
+    ----------
+    def_file : string
+        String with a JSON file containing the job definition data.
+    tmpl_file : string
+        String with a JSON file containing template data.
+    tmpl_str : list
+        List with keys/values containing template data.
+    local : bool
+        Run (or not) the job locally.
+    cluster : bool
+        Run (or not) the job on the cluster.
+    """
+
+    # get template data
+    tmpl_data = _get_template(tmpl_file, tmpl_str)
+
+    # get the job definition file and apply the template
+    def_data = _get_def(def_file, tmpl_data)
+
+    # extract data
+    tag = def_data["tag"]
+    overwrite = def_data["overwrite"]
+    folder = def_data["folder"]
+    pragmas = def_data["pragmas"]
+    vars = def_data["vars"]
+    commands = def_data["commands"]
+
+    # create the Slurm script
+    (filename_script, filename_log) = gen.run_data(tag, overwrite, folder, pragmas, vars, commands)
+
+    # run the Slurm script
+    run.run_data(filename_script, filename_log, local, cluster)
+
+
 def run_script():
     """
     Entry point for the command line script.
 
     Require one argument with the JSON file with the job definition.:
 
     Accept several options:
         - Template
             - "-tf" or "--tmpl_file" JSON file with template data.
             - "-td" or "--tmpl_str" Dictionary with template data.
         - Run options
             - "-l" or "--local" Run the job locally for debugging.
             - "-c" or "--cluster" Run the job on the Slurm cluster.
-            - "-o" or "--overwrite" Overwrite existing files.
-            - "-t" or "--tag" Overwrite the job name.
-        - Dependency options
-            - "-ok" or "--afterok" Run after successful dependency.
-            - "-any" or "--afterany" Run after terminated dependency.
     """
 
     # get argument parser
     parser = _get_parser()
 
     # parse the arguments
     args = parser.parse_args()
 
-    # get template data
-    tmpl_data = _get_template(args.tmpl_file, args.tmpl_str)
-
-    # get the job definition file and apply the template
-    def_data = _get_def(args.def_file, tmpl_data)
-
-    # extract data
-    tag = def_data["tag"]
-    control = def_data["control"]
-    folder = def_data["folder"]
-    pragmas = def_data["pragmas"]
-    vars = def_data["vars"]
-    commands = def_data["commands"]
-
-    # replace tag
-    if args.tag is not None:
-        tag = args.tag
-
-    # find control
-    cluster = control["cluster"] or args.cluster
-    local = control["local"] or args.local
-    overwrite = control["overwrite"] or args.overwrite
-
-    # dependency options
-    afterok = args.afterok
-    afterany = args.afterany
-
-    # create the Slurm script
-    (filename_script, filename_log) = gen.run_data(tag, overwrite, folder, pragmas, vars, commands)
-
-    # run the Slurm script
-    run.run_data(filename_script, filename_log, local, cluster, afterok, afterany)
+    # run
+    run_args(
+        args.def_file,
+        tmpl_file=args.tmpl_file,
+        tmpl_str=args.tmpl_str,
+        local=args.local,
+        cluster=args.cluster,
+    )
 
     # return
     sys.exit(0)
-
-
-if __name__ == "__main__":
-    run_script()
```

### Comparing `slurmgen-3.2.0/slurmgen.egg-info/PKG-INFO` & `slurmgen-3.3.3/slurmgen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurmgen
-Version: 3.2.0
+Version: 3.3.3
 Summary: SlurmGen - Simple Slurm Manager
 Author-email: Thomas Guillod <guillod@otvam.ch>
 Maintainer-email: Thomas Guillod <guillod@otvam.ch>
 License: BSD-2-Clause
 Project-URL: Homepage, https://github.com/otvam/slurmgen
 Project-URL: Repository, https://github.com/otvam/slurmgen
 Project-URL: Releases, https://github.com/otvam/slurmgen/releases
```


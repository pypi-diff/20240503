# Comparing `tmp/falcon_challenge-0.3.2.tar.gz` & `tmp/falcon_challenge-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "falcon_challenge-0.3.2.tar", last modified: Tue Apr 30 14:05:57 2024, max compression
+gzip compressed data, was "falcon_challenge-0.3.3.tar", last modified: Thu May  2 23:45:22 2024, max compression
```

## Comparing `falcon_challenge-0.3.2.tar` & `falcon_challenge-0.3.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:05:57.688868 falcon_challenge-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-30 14:05:51.000000 falcon_challenge-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-04-30 14:05:57.688868 falcon_challenge-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-30 14:05:51.000000 falcon_challenge-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:05:57.680868 falcon_challenge-0.3.2/decoder_demos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:05:51.000000 falcon_challenge-0.3.2/decoder_demos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-30 14:05:51.000000 falcon_challenge-0.3.2/decoder_demos/decoding_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8568 2024-04-30 14:05:51.000000 falcon_challenge-0.3.2/decoder_demos/filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-30 14:05:51.000000 falcon_challenge-0.3.2/decoder_demos/ndt2_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-30 14:05:51.000000 falcon_challenge-0.3.2/decoder_demos/random_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-30 14:05:51.000000 falcon_challenge-0.3.2/decoder_demos/rnn_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    13694 2024-04-30 14:05:51.000000 falcon_challenge-0.3.2/decoder_demos/sklearn_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-30 14:05:51.000000 falcon_challenge-0.3.2/decoder_demos/sklearn_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:05:57.684868 falcon_challenge-0.3.2/falcon_challenge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:05:51.000000 falcon_challenge-0.3.2/falcon_challenge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-30 14:05:51.000000 falcon_challenge-0.3.2/falcon_challenge/challenge_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-04-30 14:05:51.000000 falcon_challenge-0.3.2/falcon_challenge/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8212 2024-04-30 14:05:51.000000 falcon_challenge-0.3.2/falcon_challenge/dataloaders.py
--rw-r--r--   0 runner    (1001) docker     (127)    26489 2024-04-30 14:05:51.000000 falcon_challenge-0.3.2/falcon_challenge/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-04-30 14:05:51.000000 falcon_challenge-0.3.2/falcon_challenge/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:05:57.688868 falcon_challenge-0.3.2/falcon_challenge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-04-30 14:05:57.000000 falcon_challenge-0.3.2/falcon_challenge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-30 14:05:57.000000 falcon_challenge-0.3.2/falcon_challenge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 14:05:57.000000 falcon_challenge-0.3.2/falcon_challenge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-30 14:05:57.000000 falcon_challenge-0.3.2/falcon_challenge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-30 14:05:57.000000 falcon_challenge-0.3.2/falcon_challenge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:05:57.684868 falcon_challenge-0.3.2/preproc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:05:51.000000 falcon_challenge-0.3.2/preproc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-30 14:05:51.000000 falcon_challenge-0.3.2/preproc/assemble_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8389 2024-04-30 14:05:51.000000 falcon_challenge-0.3.2/preproc/filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-04-30 14:05:51.000000 falcon_challenge-0.3.2/preproc/h2_preproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-04-30 14:05:51.000000 falcon_challenge-0.3.2/preproc/m1_fewshot_trial_counts.py
--rw-r--r--   0 runner    (1001) docker     (127)    23601 2024-04-30 14:05:51.000000 falcon_challenge-0.3.2/preproc/m1_reachgrasp_preprocv2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-30 14:05:51.000000 falcon_challenge-0.3.2/preproc/m2_fewshot_trial_counts.py
--rw-r--r--   0 runner    (1001) docker     (127)    16660 2024-04-30 14:05:51.000000 falcon_challenge-0.3.2/preproc/m2_preproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-30 14:05:51.000000 falcon_challenge-0.3.2/preproc/merge_answers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-30 14:05:51.000000 falcon_challenge-0.3.2/preproc/nwb_create_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-30 14:05:51.000000 falcon_challenge-0.3.2/preproc/wrapper_convert_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-30 14:05:51.000000 falcon_challenge-0.3.2/preproc/zip_data.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-30 14:05:51.000000 falcon_challenge-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 14:05:57.688868 falcon_challenge-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-30 14:05:51.000000 falcon_challenge-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:45:22.188435 falcon_challenge-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-05-02 23:45:22.188435 falcon_challenge-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:45:22.184435 falcon_challenge-0.3.3/decoder_demos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/decoder_demos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/decoder_demos/decoding_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8568 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/decoder_demos/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/decoder_demos/ndt2_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/decoder_demos/random_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/decoder_demos/rnn_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13694 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/decoder_demos/sklearn_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/decoder_demos/sklearn_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:45:22.184435 falcon_challenge-0.3.3/falcon_challenge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/falcon_challenge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/falcon_challenge/challenge_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/falcon_challenge/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8212 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/falcon_challenge/dataloaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26489 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/falcon_challenge/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/falcon_challenge/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:45:22.188435 falcon_challenge-0.3.3/falcon_challenge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-05-02 23:45:22.000000 falcon_challenge-0.3.3/falcon_challenge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-02 23:45:22.000000 falcon_challenge-0.3.3/falcon_challenge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 23:45:22.000000 falcon_challenge-0.3.3/falcon_challenge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-02 23:45:22.000000 falcon_challenge-0.3.3/falcon_challenge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 23:45:22.000000 falcon_challenge-0.3.3/falcon_challenge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:45:22.188435 falcon_challenge-0.3.3/preproc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/preproc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/preproc/assemble_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8389 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/preproc/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/preproc/h2_preproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/preproc/m1_fewshot_trial_counts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24166 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/preproc/m1_reachgrasp_preprocv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/preproc/m2_fewshot_trial_counts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16660 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/preproc/m2_preproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/preproc/merge_answers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/preproc/nwb_create_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/preproc/wrapper_convert_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/preproc/zip_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 23:45:22.188435 falcon_challenge-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-02 23:45:13.000000 falcon_challenge-0.3.3/setup.py
```

### Comparing `falcon_challenge-0.3.2/LICENSE` & `falcon_challenge-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.2/PKG-INFO` & `falcon_challenge-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: falcon_challenge
-Version: 0.3.2
+Version: 0.3.3
 Home-page: https://github.com/snel-repo/stability-benchmark
 Author: Joel Ye
 Author-email: joelye9@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: hydra-core
```

### Comparing `falcon_challenge-0.3.2/README.md` & `falcon_challenge-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.2/decoder_demos/decoding_utils.py` & `falcon_challenge-0.3.3/decoder_demos/decoding_utils.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.2/decoder_demos/filtering.py` & `falcon_challenge-0.3.3/decoder_demos/filtering.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.2/decoder_demos/ndt2_sample.py` & `falcon_challenge-0.3.3/decoder_demos/ndt2_sample.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.2/decoder_demos/random_decoder.py` & `falcon_challenge-0.3.3/decoder_demos/random_decoder.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.2/decoder_demos/rnn_decoder.py` & `falcon_challenge-0.3.3/decoder_demos/rnn_decoder.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.2/decoder_demos/sklearn_decoder.py` & `falcon_challenge-0.3.3/decoder_demos/sklearn_decoder.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.2/decoder_demos/sklearn_sample.py` & `falcon_challenge-0.3.3/decoder_demos/sklearn_sample.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.2/falcon_challenge/config.py` & `falcon_challenge-0.3.3/falcon_challenge/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     @property
     def n_channels(self):
         if self.task == FalconTask.h1:
             return 176
         elif self.task == FalconTask.h2:
             return 192
         elif self.task == FalconTask.m1:
-            return 96
+            return 64
         elif self.task == FalconTask.m2:
             return 96
         raise NotImplementedError(f"Task {self.task} not implemented.")
 
     @property
     def out_dim(self):
         if self.task == FalconTask.h1:
```

### Comparing `falcon_challenge-0.3.2/falcon_challenge/dataloaders.py` & `falcon_challenge-0.3.3/falcon_challenge/dataloaders.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.2/falcon_challenge/evaluator.py` & `falcon_challenge-0.3.3/falcon_challenge/evaluator.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.2/falcon_challenge/interface.py` & `falcon_challenge-0.3.3/falcon_challenge/interface.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.2/falcon_challenge.egg-info/PKG-INFO` & `falcon_challenge-0.3.3/falcon_challenge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: falcon_challenge
-Version: 0.3.2
+Version: 0.3.3
 Home-page: https://github.com/snel-repo/stability-benchmark
 Author: Joel Ye
 Author-email: joelye9@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: hydra-core
```

### Comparing `falcon_challenge-0.3.2/falcon_challenge.egg-info/SOURCES.txt` & `falcon_challenge-0.3.3/falcon_challenge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.2/preproc/assemble_data.py` & `falcon_challenge-0.3.3/preproc/assemble_data.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.2/preproc/filtering.py` & `falcon_challenge-0.3.3/preproc/filtering.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.2/preproc/h2_preproc.py` & `falcon_challenge-0.3.3/preproc/h2_preproc.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.2/preproc/m1_fewshot_trial_counts.py` & `falcon_challenge-0.3.3/preproc/m1_fewshot_trial_counts.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.2/preproc/m1_reachgrasp_preprocv2.py` & `falcon_challenge-0.3.3/preproc/m1_reachgrasp_preprocv2.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,18 +39,18 @@
 
 handler = logging.StreamHandler(sys.stdout)
 handler.setLevel(logging.INFO)
 formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
 handler.setFormatter(formatter)
 logger.addHandler(handler)
 
-SAVE_PATH = "/snel/share/share/derived/rouse/RTG/NWB_FALCON_v5/"
+SAVE_PATH = "/snel/share/share/derived/rouse/RTG/NWB_FALCON_v7_unsorted/"
 rouse_base_dir = "/snel/share/share/data/rouse/RTG/"
 MONKEY = "L"
-EXP_DATE = "20120924"
+EXP_DATE = "20120926"
 
 if len(sys.argv) > 2:
     EXP_DATE = sys.argv[1]
     MONKEY = sys.argv[2]
 
 train_dates = ['20120924', '20120926', '20120927', '20120928']
 test_dates = ['20121004', '20121017', '20121022', '20121024']
@@ -59,15 +59,15 @@
     IS_TEST_DS = False
 if EXP_DATE in test_dates:
     IS_TEST_DS = True
 
 # emg file
 emg_mat_path = path.join(rouse_base_dir, f"{MONKEY}{EXP_DATE}_AD_Unrect_EMG.mat")
 # spikes file
-spk_mat_path = glob.glob(path.join(rouse_base_dir, f"{MONKEY}_*_{EXP_DATE}-data.mat"))[0]
+spk_mat_path = glob.glob(path.join(rouse_base_dir, 'unsorted_unit', f"{MONKEY}_*_{EXP_DATE}-data.mat"))[0]
 # get file string
 # file_id = f"{monkey}_{exp_date}"
 # load mat data
 f_emg = loadmat(emg_mat_path)
 f_spk = h5py.File(spk_mat_path, "r")
 
 def convert_datestr_to_datetime(collect_date):
@@ -110,17 +110,18 @@
     return names
 
 emg_names = convert_names_to_list(f_emg['EMGSettings'], 'ChanNames')
 fs_cont = float(f_emg['EMGSettings']['samp_rate'][0][0][0][0])
 t_offset = f_emg['EMGSettings']['analog_start_time'][0][0][0][0]
 
 #%%
-channels = np.squeeze(f_spk['SpikeSettings']['channels'][()])
+channels = np.squeeze(f_spk['SpikeSettings']['unique_channel_num'][()])
 all_spike_times = []
-for i in range(1, 97):
+possible_channel_numbers = np.concatenate([x + np.arange(1, 17) for x in [800, 900, 1000, 1100]])
+for i in possible_channel_numbers:
     ch_spk_times = []
     where_chan = np.where(channels == i)[0]
     for j in where_chan:
         spike_times = f_spk[f_spk['AllSpikeTimes'][j][0]]
         if spike_times.shape[0] == 1:
             spike_times = spike_times[0]
         else:
@@ -133,21 +134,31 @@
     all_spike_times.append(ch_spk_times)
 
 #%%
 # n_units = np.unique(f_spk['SpikeSettings']['channels'][()]).shape[0]
 array_group_by_chan = f_spk['SpikeSettings']['array_by_channel'][0]
 array_group_by_chan = [chr(array_id) for array_id in array_group_by_chan.tolist()] # this is for each channels that has spikes
 array_group_by_elec = []
-for i in range(1, 97):
-    if i in channels:
-        array_group_by_elec.append(
-            array_group_by_chan[np.where(channels == i)[0][0]]
-        )
-    else:
+for i in possible_channel_numbers:
+    if i > 1100: 
+        array_group_by_elec.append('K')
+    elif i > 1000: 
+        array_group_by_elec.append('J')
+    elif i > 900:
+        array_group_by_elec.append('I')
+    elif i > 800:
+        array_group_by_elec.append('H')
+    else: 
         array_group_by_elec.append(None)
+    # if i in channels:
+    #     array_group_by_elec.append(
+    #         array_group_by_chan[np.where(channels == i)[0][0]]
+    #     )
+    # else:
+    #     array_group_by_elec.append(None)
 
 # elec_id_by_chan = f_spk['SpikeSettings']['unique_channel_num'][0]
 
 #%%
 
 def convert_to_NWB(
     fs_cont,
@@ -350,32 +361,32 @@
     logger.info("Adding spiking data")
 
     device = nwbfile.create_device(
         name="floating microelectrode_array",
         description="16-electrode array",
         manufacturer="MicroProbes for Life Sciences",
     )
-    E_elec_group = nwbfile.create_electrode_group(
-        name="E_electrode_group",
-        description="Electrodes in an implanted FMA array labeled E",
-        location="Motor Cortex",
-        device=device,
-    )
-    F_elec_group = nwbfile.create_electrode_group(
-        name="F_electrode_group",
-        description="Electrodes in an implanted FMA array labeled F",
-        location="Motor Cortex",
-        device=device,
-    )
-    G_elec_group = nwbfile.create_electrode_group(
-        name="G_electrode_group",
-        description="Electrodes in an implanted FMA array labeled G",
-        location="Motor Cortex",
-        device=device,
-    )
+    # E_elec_group = nwbfile.create_electrode_group(
+    #     name="E_electrode_group",
+    #     description="Electrodes in an implanted FMA array labeled E",
+    #     location="Motor Cortex",
+    #     device=device,
+    # )
+    # F_elec_group = nwbfile.create_electrode_group(
+    #     name="F_electrode_group",
+    #     description="Electrodes in an implanted FMA array labeled F",
+    #     location="Motor Cortex",
+    #     device=device,
+    # )
+    # G_elec_group = nwbfile.create_electrode_group(
+    #     name="G_electrode_group",
+    #     description="Electrodes in an implanted FMA array labeled G",
+    #     location="Motor Cortex",
+    #     device=device,
+    # )
     H_elec_group = nwbfile.create_electrode_group(
         name="H_electrode_group",
         description="Electrodes in an implanted FMA array labeled H",
         location="Motor Cortex",
         device=device,
     )
     I_elec_group = nwbfile.create_electrode_group(
@@ -392,36 +403,36 @@
     )
     K_elec_group = nwbfile.create_electrode_group(
         name="K_electrode_group",
         description="Electrodes in an implanted FMA array labeled K",
         location="Motor Cortex",
         device=device,
     )
-    L_elec_group = nwbfile.create_electrode_group(
-        name="L_electrode_group",
-        description="Electrodes in an implanted FMA array labeled L",
-        location="Motor Cortex",
-        device=device,
-    )
+    # L_elec_group = nwbfile.create_electrode_group(
+    #     name="L_electrode_group",
+    #     description="Electrodes in an implanted FMA array labeled L",
+    #     location="Motor Cortex",
+    #     device=device,
+    # )
     Z_elec_group = nwbfile.create_electrode_group(
         name='Z_electrode_group',
         description="Electrodes not labelled as belonging to any other group",
         location='Motor Cortex',
         device=device,
     )
 
     elec_group_map = {
-        'E': E_elec_group,
-        'F': F_elec_group,
-        'G': G_elec_group,
+        # 'E': E_elec_group,
+        # 'F': F_elec_group,
+        # 'G': G_elec_group,
         'H': H_elec_group,
         'I': I_elec_group,
         'J': J_elec_group,
         'K': K_elec_group,
-        'L': L_elec_group,
+        # 'L': L_elec_group,
         'Z': Z_elec_group,
     }
 
     nwbfile.units = Units(
         name="units", description="Sampled at 30 kHz with anti-alias", resolution=1/fs_cont
     )
     # orig_elec_ids = np.unique(elec_id_by_chan)
@@ -431,15 +442,15 @@
     array_elec_groups = []
     for arr_id in array_group_by_chan:
         if arr_id is not None:
             array_elec_groups.append(elec_group_map[arr_id])
         else:
             array_elec_groups.append(elec_group_map['Z'])
 
-    for elec_id in range(1, 97):
+    for elec_id in range(1, 65):
         # elec_id = orig_elec_ids[i]
         try:
             nwbfile.add_electrode(
                 id=elec_id-1, #int(elec_id_map[elec_id]),
                 x=np.nan,
                 y=np.nan,
                 z=np.nan,
@@ -474,15 +485,15 @@
             stop_cutoff = t_new[-1]
         # ensure spike times are within bound of continuous data
         keep_mask = (all_spike_times > start_cutoff) & (all_spike_times < stop_cutoff)
         valid_spike_times = all_spike_times[keep_mask] if len(all_spike_times) >= 1 else all_spike_times
         # if valid_spike_times is not None:
         nwbfile.add_unit(
             id=elec_id-1,
-            spike_times=np.squeeze(valid_spike_times),
+            spike_times=np.squeeze(valid_spike_times) if len(valid_spike_times) > 1 else valid_spike_times,
             electrodes=[elec_id-1],
             obs_intervals=[[start_cutoff, stop_cutoff]],
         )
         # else:
         #     nwbfile.add_unit(
         #         id=i,
         #         electrodes=[elec_id],
```

### Comparing `falcon_challenge-0.3.2/preproc/m2_fewshot_trial_counts.py` & `falcon_challenge-0.3.3/preproc/m2_fewshot_trial_counts.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.2/preproc/m2_preproc.py` & `falcon_challenge-0.3.3/preproc/m2_preproc.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.2/preproc/merge_answers.py` & `falcon_challenge-0.3.3/preproc/merge_answers.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.2/preproc/nwb_create_utils.py` & `falcon_challenge-0.3.3/preproc/nwb_create_utils.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.2/preproc/zip_data.py` & `falcon_challenge-0.3.3/preproc/zip_data.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.2/setup.py` & `falcon_challenge-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='falcon_challenge',
-    version='0.3.2',
+    version='0.3.3',
 
     url='https://github.com/snel-repo/stability-benchmark',
     author='Joel Ye',
     author_email='joelye9@gmail.com',
 
     packages=find_packages(exclude=['data_demos', 'data']),
     install_requires=[
```


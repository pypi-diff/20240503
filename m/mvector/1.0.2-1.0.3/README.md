# Comparing `tmp/mvector-1.0.2-py3-none-any.whl.zip` & `tmp/mvector-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 60157 bytes, number of entries: 32
--rw-rw-rw-  2.0 fat      134 b- defN 24-Apr-27 06:43 mvector/__init__.py
--rw-rw-rw-  2.0 fat    17707 b- defN 24-Jan-10 12:54 mvector/predict.py
--rw-rw-rw-  2.0 fat    35940 b- defN 24-Apr-27 06:40 mvector/trainer.py
+Zip file size: 61126 bytes, number of entries: 32
+-rw-rw-rw-  2.0 fat      134 b- defN 24-May-03 03:44 mvector/__init__.py
+-rw-rw-rw-  2.0 fat    17513 b- defN 24-May-02 06:53 mvector/predict.py
+-rw-rw-rw-  2.0 fat    38106 b- defN 24-May-02 07:13 mvector/trainer.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Jan-06 05:59 mvector/data_utils/__init__.py
 -rw-rw-rw-  2.0 fat    22220 b- defN 24-Apr-27 05:32 mvector/data_utils/audio.py
--rw-rw-rw-  2.0 fat      965 b- defN 24-Jan-06 05:59 mvector/data_utils/collate_fn.py
--rw-rw-rw-  2.0 fat     3587 b- defN 24-Jan-06 05:59 mvector/data_utils/featurizer.py
--rw-rw-rw-  2.0 fat     5885 b- defN 24-Jan-06 05:59 mvector/data_utils/reader.py
+-rw-rw-rw-  2.0 fat      930 b- defN 24-May-02 05:56 mvector/data_utils/collate_fn.py
+-rw-rw-rw-  2.0 fat     3696 b- defN 24-May-02 06:00 mvector/data_utils/featurizer.py
+-rw-rw-rw-  2.0 fat     7407 b- defN 24-May-02 07:33 mvector/data_utils/reader.py
 -rw-rw-rw-  2.0 fat     1572 b- defN 24-Jan-06 05:59 mvector/data_utils/spec_aug.py
 -rw-rw-rw-  2.0 fat     4712 b- defN 24-Jan-06 05:59 mvector/data_utils/utils.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Jan-06 05:59 mvector/metric/__init__.py
 -rw-rw-rw-  2.0 fat     1517 b- defN 24-Jan-06 05:59 mvector/metric/metrics.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Jan-06 05:59 mvector/models/__init__.py
 -rw-rw-rw-  2.0 fat    13511 b- defN 24-Jan-06 05:59 mvector/models/campplus.py
 -rw-rw-rw-  2.0 fat     5293 b- defN 24-Jan-06 05:59 mvector/models/ecapa_tdnn.py
@@ -22,13 +22,13 @@
 -rw-rw-rw-  2.0 fat     5522 b- defN 24-Jan-06 05:59 mvector/models/resnet_se.py
 -rw-rw-rw-  2.0 fat     2963 b- defN 24-Jan-06 05:59 mvector/models/tdnn.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Jan-06 05:59 mvector/utils/__init__.py
 -rw-rw-rw-  2.0 fat     2839 b- defN 24-Jan-06 05:59 mvector/utils/logger.py
 -rw-rw-rw-  2.0 fat     1385 b- defN 24-Jan-15 12:44 mvector/utils/record.py
 -rw-rw-rw-  2.0 fat     3538 b- defN 24-Jan-06 05:59 mvector/utils/scheduler.py
 -rw-rw-rw-  2.0 fat     2789 b- defN 24-Jan-06 05:59 mvector/utils/utils.py
--rw-rw-rw-  2.0 fat    11558 b- defN 24-Apr-27 06:43 mvector-1.0.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    32558 b- defN 24-Apr-27 06:43 mvector-1.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-27 06:43 mvector-1.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 24-Apr-27 06:43 mvector-1.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     2595 b- defN 24-Apr-27 06:43 mvector-1.0.2.dist-info/RECORD
-32 files, 212801 bytes uncompressed, 56029 bytes compressed:  73.7%
+-rw-rw-rw-  2.0 fat    11558 b- defN 24-May-03 03:44 mvector-1.0.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    33611 b- defN 24-May-03 03:44 mvector-1.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-03 03:44 mvector-1.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 24-May-03 03:44 mvector-1.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     2595 b- defN 24-May-03 03:44 mvector-1.0.3.dist-info/RECORD
+32 files, 217422 bytes uncompressed, 56998 bytes compressed:  73.8%
```

## zipnote {}

```diff
@@ -75,23 +75,23 @@
 
 Filename: mvector/utils/scheduler.py
 Comment: 
 
 Filename: mvector/utils/utils.py
 Comment: 
 
-Filename: mvector-1.0.2.dist-info/LICENSE
+Filename: mvector-1.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: mvector-1.0.2.dist-info/METADATA
+Filename: mvector-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: mvector-1.0.2.dist-info/WHEEL
+Filename: mvector-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: mvector-1.0.2.dist-info/top_level.txt
+Filename: mvector-1.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: mvector-1.0.2.dist-info/RECORD
+Filename: mvector-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mvector/__init__.py

```diff
@@ -1,3 +1,3 @@
-__version__ = "1.0.2"
+__version__ = "1.0.3"
 # 项目支持的模型
 SUPPORT_MODEL = ['ERes2Net', 'CAMPPlus', 'EcapaTdnn', 'Res2Net', 'ResNetSE', 'TDNN']
```

## mvector/predict.py

```diff
@@ -54,15 +54,14 @@
             with open(configs, 'r', encoding='utf-8') as f:
                 configs = yaml.load(f.read(), Loader=yaml.FullLoader)
             print_arguments(configs=configs)
         self.configs = dict_to_object(configs)
         assert self.configs.use_model in SUPPORT_MODEL, f'没有该模型：{self.configs.use_model}'
         self._audio_featurizer = AudioFeaturizer(feature_method=self.configs.preprocess_conf.feature_method,
                                                  method_args=self.configs.preprocess_conf.get('method_args', {}))
-        self._audio_featurizer.to(self.device)
         # 获取模型
         if self.configs.use_model == 'ERes2Net':
             backbone = ERes2Net(input_size=self._audio_featurizer.feature_dim, **self.configs.model_conf.backbone)
         elif self.configs.use_model == 'CAMPPlus':
             backbone = CAMPPlus(input_size=self._audio_featurizer.feature_dim, **self.configs.model_conf.backbone)
         elif self.configs.use_model == 'EcapaTdnn':
             backbone = EcapaTdnn(input_size=self._audio_featurizer.feature_dim, **self.configs.model_conf.backbone)
@@ -224,17 +223,16 @@
 
         :param audio_data: 需要识别的数据，支持文件路径，文件对象，字节，numpy。如果是字节的话，必须是完整并带格式的字节文件
         :param sample_rate: 如果传入的事numpy数据，需要指定采样率
         :return: 声纹特征向量
         """
         # 加载音频文件，并进行预处理
         input_data = self._load_audio(audio_data=audio_data, sample_rate=sample_rate)
-        input_data = torch.tensor(input_data.samples, dtype=torch.float32, device=self.device).unsqueeze(0)
-        input_len_ratio = torch.tensor([1], dtype=torch.float32, device=self.device)
-        audio_feature, _ = self._audio_featurizer(input_data, input_len_ratio)
+        input_data = torch.tensor(input_data.samples, dtype=torch.float32).unsqueeze(0)
+        audio_feature = self._audio_featurizer(input_data).to(self.device)
         # 执行预测
         feature = self.predictor(audio_feature).data.cpu().numpy()[0]
         return feature
 
     def predict_batch(self, audios_data, sample_rate=16000):
         """预测一批音频的特征
 
@@ -248,25 +246,25 @@
             input_data = self._load_audio(audio_data=audio_data, sample_rate=sample_rate)
             audios_data1.append(input_data.samples)
         # 找出音频长度最长的
         batch = sorted(audios_data1, key=lambda a: a.shape[0], reverse=True)
         max_audio_length = batch[0].shape[0]
         batch_size = len(batch)
         # 以最大的长度创建0张量
-        inputs = np.zeros((batch_size, max_audio_length), dtype='float32')
+        inputs = np.zeros((batch_size, max_audio_length), dtype=np.float32)
         input_lens_ratio = []
         for x in range(batch_size):
             tensor = audios_data1[x]
             seq_length = tensor.shape[0]
             # 将数据插入都0张量中，实现了padding
             inputs[x, :seq_length] = tensor[:]
             input_lens_ratio.append(seq_length / max_audio_length)
-        audios_data = torch.tensor(inputs, dtype=torch.float32, device=self.device)
-        input_lens_ratio = torch.tensor(input_lens_ratio, dtype=torch.float32, device=self.device)
-        audio_feature, _ = self._audio_featurizer(audios_data, input_lens_ratio)
+        inputs = torch.tensor(inputs, dtype=torch.float32)
+        input_lens_ratio = torch.tensor(input_lens_ratio, dtype=torch.float32)
+        audio_feature = self._audio_featurizer(inputs, input_lens_ratio).to(self.device)
         # 执行预测
         features = self.predictor(audio_feature).data.cpu().numpy()
         return features
 
     def contrast(self, audio_data1, audio_data2):
         """声纹对比
```

## mvector/trainer.py

```diff
@@ -17,15 +17,15 @@
 from torchinfo import summary
 from tqdm import tqdm
 from visualdl import LogWriter
 
 from mvector import SUPPORT_MODEL, __version__
 from mvector.data_utils.collate_fn import collate_fn
 from mvector.data_utils.featurizer import AudioFeaturizer
-from mvector.data_utils.reader import CustomDataset
+from mvector.data_utils.reader import MVectorDataset
 from mvector.data_utils.spec_aug import SpecAug
 from mvector.metric.metrics import compute_fnr_fpr, compute_eer, compute_dcf, accuracy
 from mvector.models.campplus import CAMPPlus
 from mvector.models.ecapa_tdnn import EcapaTdnn
 from mvector.models.eres2net import ERes2Net
 from mvector.models.fc import SpeakerIdentification
 from mvector.models.loss import AAMLoss, CELoss, AMLoss, ARMLoss, SubCenterLoss, SphereFace2
@@ -59,15 +59,20 @@
                 configs = yaml.load(f.read(), Loader=yaml.FullLoader)
             print_arguments(configs=configs)
         self.configs = dict_to_object(configs)
         assert self.configs.use_model in SUPPORT_MODEL, f'没有该模型：{self.configs.use_model}'
         self.model = None
         self.backbone = None
         self.model_output_name = '1.weight'
+        self.audio_featurizer = None
+        self.train_dataset = None
+        self.train_loader = None
+        self.enroll_dataset = None
         self.enroll_loader = None
+        self.trials_dataset = None
         self.trials_loader = None
         self.margin_scheduler = None
         self.amp_scaler = None
         # 获取特征器
         self.audio_featurizer = AudioFeaturizer(feature_method=self.configs.preprocess_conf.feature_method,
                                                 method_args=self.configs.preprocess_conf.get('method_args', {}))
         self.audio_featurizer.to(self.device)
@@ -81,60 +86,93 @@
         self.train_loss, self.train_acc = None, None
         self.train_eta_sec = None
         self.eval_eer, self.eval_min_dcf, self.eval_threshold = None, None, None
         self.test_log_step, self.train_log_step = 0, 0
         self.stop_train, self.stop_eval = False, False
 
     def __setup_dataloader(self, is_train=False):
+        # 获取特征器
+        self.audio_featurizer = AudioFeaturizer(feature_method=self.configs.preprocess_conf.feature_method,
+                                                method_args=self.configs.preprocess_conf.get('method_args', {}))
         if is_train:
-            self.train_dataset = CustomDataset(data_list_path=self.configs.dataset_conf.train_list,
-                                               do_vad=self.configs.dataset_conf.do_vad,
-                                               max_duration=self.configs.dataset_conf.max_duration,
-                                               min_duration=self.configs.dataset_conf.min_duration,
-                                               sample_rate=self.configs.dataset_conf.sample_rate,
-                                               aug_conf=self.configs.dataset_conf.aug_conf,
-                                               num_speakers=self.configs.model_conf.classifier.num_speakers,
-                                               use_dB_normalization=self.configs.dataset_conf.use_dB_normalization,
-                                               target_dB=self.configs.dataset_conf.target_dB,
-                                               mode='train')
+            self.train_dataset = MVectorDataset(data_list_path=self.configs.dataset_conf.train_list,
+                                                audio_featurizer=self.audio_featurizer,
+                                                do_vad=self.configs.dataset_conf.do_vad,
+                                                max_duration=self.configs.dataset_conf.max_duration,
+                                                min_duration=self.configs.dataset_conf.min_duration,
+                                                sample_rate=self.configs.dataset_conf.sample_rate,
+                                                aug_conf=self.configs.dataset_conf.aug_conf,
+                                                num_speakers=self.configs.model_conf.classifier.num_speakers,
+                                                use_dB_normalization=self.configs.dataset_conf.use_dB_normalization,
+                                                target_dB=self.configs.dataset_conf.target_dB,
+                                                mode='train')
             train_sampler = None
             if torch.cuda.device_count() > 1:
                 # 设置支持多卡训练
                 train_sampler = DistributedSampler(dataset=self.train_dataset)
             self.train_loader = DataLoader(dataset=self.train_dataset,
                                            collate_fn=collate_fn,
                                            shuffle=(train_sampler is None),
                                            sampler=train_sampler,
                                            **self.configs.dataset_conf.dataLoader)
         # 获取评估的注册数据和检验数据
-        self.enroll_dataset = CustomDataset(data_list_path=self.configs.dataset_conf.enroll_list,
-                                            do_vad=self.configs.dataset_conf.do_vad,
-                                            max_duration=self.configs.dataset_conf.eval_conf.max_duration,
-                                            min_duration=self.configs.dataset_conf.min_duration,
-                                            sample_rate=self.configs.dataset_conf.sample_rate,
-                                            use_dB_normalization=self.configs.dataset_conf.use_dB_normalization,
-                                            target_dB=self.configs.dataset_conf.target_dB,
-                                            mode='eval')
+        self.enroll_dataset = MVectorDataset(data_list_path=self.configs.dataset_conf.enroll_list,
+                                             audio_featurizer=self.audio_featurizer,
+                                             do_vad=self.configs.dataset_conf.do_vad,
+                                             max_duration=self.configs.dataset_conf.eval_conf.max_duration,
+                                             min_duration=self.configs.dataset_conf.min_duration,
+                                             sample_rate=self.configs.dataset_conf.sample_rate,
+                                             use_dB_normalization=self.configs.dataset_conf.use_dB_normalization,
+                                             target_dB=self.configs.dataset_conf.target_dB,
+                                             mode='eval')
         self.enroll_loader = DataLoader(dataset=self.enroll_dataset,
                                         collate_fn=collate_fn,
                                         batch_size=self.configs.dataset_conf.eval_conf.batch_size,
                                         num_workers=self.configs.dataset_conf.dataLoader.num_workers)
-        self.trials_dataset = CustomDataset(data_list_path=self.configs.dataset_conf.trials_list,
-                                            do_vad=self.configs.dataset_conf.do_vad,
-                                            max_duration=self.configs.dataset_conf.eval_conf.max_duration,
-                                            min_duration=self.configs.dataset_conf.min_duration,
-                                            sample_rate=self.configs.dataset_conf.sample_rate,
-                                            use_dB_normalization=self.configs.dataset_conf.use_dB_normalization,
-                                            target_dB=self.configs.dataset_conf.target_dB,
-                                            mode='eval')
+        self.trials_dataset = MVectorDataset(data_list_path=self.configs.dataset_conf.trials_list,
+                                             audio_featurizer=self.audio_featurizer,
+                                             do_vad=self.configs.dataset_conf.do_vad,
+                                             max_duration=self.configs.dataset_conf.eval_conf.max_duration,
+                                             min_duration=self.configs.dataset_conf.min_duration,
+                                             sample_rate=self.configs.dataset_conf.sample_rate,
+                                             use_dB_normalization=self.configs.dataset_conf.use_dB_normalization,
+                                             target_dB=self.configs.dataset_conf.target_dB,
+                                             mode='eval')
         self.trials_loader = DataLoader(dataset=self.trials_dataset,
                                         collate_fn=collate_fn,
                                         batch_size=self.configs.dataset_conf.eval_conf.batch_size,
                                         num_workers=self.configs.dataset_conf.dataLoader.num_workers)
 
+    # 提取特征保存文件
+    def extract_features(self, save_dir='dataset/features'):
+        self.audio_featurizer = AudioFeaturizer(feature_method=self.configs.preprocess_conf.feature_method,
+                                                method_args=self.configs.preprocess_conf.get('method_args', {}))
+        for i, data_list in enumerate([self.configs.dataset_conf.train_list,
+                                       self.configs.dataset_conf.enroll_list,
+                                       self.configs.dataset_conf.trials_list]):
+            # 获取测试数据
+            test_dataset = MVectorDataset(data_list_path=data_list,
+                                          audio_featurizer=self.audio_featurizer,
+                                          do_vad=self.configs.dataset_conf.do_vad,
+                                          sample_rate=self.configs.dataset_conf.sample_rate,
+                                          use_dB_normalization=self.configs.dataset_conf.use_dB_normalization,
+                                          target_dB=self.configs.dataset_conf.target_dB,
+                                          mode='extract_feature')
+            save_data_list = data_list.replace('.txt', '_features.txt')
+            with open(save_data_list, 'w', encoding='utf-8') as f:
+                for i in tqdm(range(len(test_dataset))):
+                    feature, label = test_dataset[i]
+                    feature = feature.numpy()
+                    label = int(label)
+                    save_path = os.path.join(save_dir, str(label), f'{int(time.time() * 1000)}.npy').replace('\\', '/')
+                    os.makedirs(os.path.dirname(save_path), exist_ok=True)
+                    np.save(save_path, feature)
+                    f.write(f'{save_path}\t{label}\n')
+            logger.info(f'{data_list}列表中的数据已提取特征完成，新列表为：{save_data_list}')
+
     def __setup_model(self, input_size, is_train=False):
         # 获取模型
         if self.configs.use_model == 'ERes2Net':
             self.backbone = ERes2Net(input_size=input_size, **self.configs.model_conf.backbone)
         elif self.configs.use_model == 'CAMPPlus':
             self.backbone = CAMPPlus(input_size=input_size, **self.configs.model_conf.backbone)
         elif self.configs.use_model == 'EcapaTdnn':
@@ -227,15 +265,15 @@
             else:
                 raise Exception(f'不支持学习率衰减函数：{self.configs.optimizer_conf.scheduler}')
         else:
             # 不训练模型不包含分类器
             self.model = nn.Sequential(self.backbone)
             self.model.to(self.device)
         self.model.to(self.device)
-        summary(self.model, (1, 98, self.audio_featurizer.feature_dim))
+        summary(self.model, (1, 98, input_size))
         # 使用Pytorch2.0的编译器
         if self.configs.train_conf.use_compile and torch.__version__ >= "2" and platform.system().lower() != 'windows':
             self.model = torch.compile(self.model, mode="reduce-overhead")
 
     def __load_pretrained(self, pretrained_model):
         # 加载预训练模型
         if pretrained_model is None: return
@@ -334,25 +372,22 @@
                 shutil.rmtree(old_model_path)
         logger.info('已保存模型：{}'.format(model_path))
 
     def __train_epoch(self, epoch_id, save_model_path, local_rank, writer, nranks=0):
         train_times, accuracies, loss_sum = [], [], []
         start = time.time()
         use_loss = self.configs.loss_conf.get('use_loss', 'AAMLoss')
-        for batch_id, (audio, label, input_lens_ratio) in enumerate(self.train_loader):
+        for batch_id, (features, label, input_len) in enumerate(self.train_loader):
             if self.stop_train: break
             if nranks > 1:
-                audio = audio.to(local_rank)
-                input_lens_ratio = input_lens_ratio.to(local_rank)
+                features = features.to(local_rank)
                 label = label.to(local_rank).long()
             else:
-                audio = audio.to(self.device)
-                input_lens_ratio = input_lens_ratio.to(self.device)
+                features = features.to(self.device)
                 label = label.to(self.device).long()
-            features, _ = self.audio_featurizer(audio, input_lens_ratio)
             # 特征增强
             if self.configs.dataset_conf.use_spec_aug:
                 features = self.spec_aug(features)
             # 执行模型计算，是否开启自动混合精度
             with torch.cuda.amp.autocast(enabled=self.configs.train_conf.enable_amp):
                 output = self.model(features)
             # 计算损失值
@@ -450,15 +485,14 @@
         if last_epoch > 0:
             self.optimizer.step()
             [self.scheduler.step() for _ in range(last_epoch)]
 
         # 支持多卡训练
         if nranks > 1 and self.use_gpu:
             self.model.to(local_rank)
-            self.audio_featurizer.to(local_rank)
             self.model = torch.nn.parallel.DistributedDataParallel(self.model, device_ids=[local_rank])
         logger.info('训练数据：{}'.format(len(self.train_dataset)))
 
         self.train_loss, self.train_acc = None, None
         self.test_log_step, self.train_log_step = 0, 0
         self.eval_eer, self.eval_min_dcf, self.eval_threshold = None, None, None
         last_epoch += 1
@@ -528,34 +562,32 @@
             eval_model = self.model.module if len(self.model.module) == 1 else self.model.module[0]
         else:
             eval_model = self.model if len(self.model) == 1 else self.model[0]
 
         # 获取注册的声纹特征和标签
         enroll_features, enroll_labels = None, None
         with torch.no_grad():
-            for batch_id, (audio, label, input_lens_ratio) in enumerate(tqdm(self.enroll_loader, desc="注册音频声纹特征")):
+            for batch_id, (audio_features, label, input_len) in enumerate(
+                    tqdm(self.enroll_loader, desc="注册音频声纹特征")):
                 if self.stop_eval: break
-                audio = audio.to(self.device)
-                input_lens_ratio = input_lens_ratio.to(self.device)
+                audio_features = audio_features.to(self.device)
                 label = label.to(self.device).long()
-                audio_features, _ = self.audio_featurizer(audio, input_lens_ratio)
                 feature = eval_model(audio_features).data.cpu().numpy()
                 label = label.data.cpu().numpy()
                 # 存放特征
                 enroll_features = np.concatenate((enroll_features, feature)) if enroll_features is not None else feature
                 enroll_labels = np.concatenate((enroll_labels, label)) if enroll_labels is not None else label
         # 获取检验的声纹特征和标签
         trials_features, trials_labels = None, None
         with torch.no_grad():
-            for batch_id, (audio, label, input_lens_ratio) in enumerate(tqdm(self.trials_loader, desc="验证音频声纹特征")):
+            for batch_id, (audio_features, label, input_lens) in enumerate(
+                    tqdm(self.trials_loader, desc="验证音频声纹特征")):
                 if self.stop_eval: break
-                audio = audio.to(self.device)
-                input_lens_ratio = input_lens_ratio.to(self.device)
+                audio_features = audio_features.to(self.device)
                 label = label.to(self.device).long()
-                audio_features, _ = self.audio_featurizer(audio, input_lens_ratio)
                 feature = eval_model(audio_features).data.cpu().numpy()
                 label = label.data.cpu().numpy()
                 # 存放特征
                 trials_features = np.concatenate((trials_features, feature)) if trials_features is not None else feature
                 trials_labels = np.concatenate((trials_labels, label)) if trials_labels is not None else label
         self.model.train()
         enroll_labels = enroll_labels.astype(np.int32)
```

## mvector/data_utils/collate_fn.py

```diff
@@ -1,25 +1,23 @@
-import numpy as np
 import torch
 
 
 # 对一个batch的数据处理
 def collate_fn(batch):
     # 找出音频长度最长的
-    batch = sorted(batch, key=lambda sample: sample[0].shape[0], reverse=True)
-    max_audio_length = batch[0][0].shape[0]
-    batch_size = len(batch)
+    batch_sorted = sorted(batch, key=lambda sample: sample[0].size(0), reverse=True)
+    freq_size = batch_sorted[0][0].size(1)
+    max_freq_length = batch_sorted[0][0].size(0)
+    batch_size = len(batch_sorted)
     # 以最大的长度创建0张量
-    inputs = np.zeros((batch_size, max_audio_length), dtype='float32')
-    input_lens_ratio = []
-    labels = []
+    features = torch.zeros((batch_size, max_freq_length, freq_size), dtype=torch.float32)
+    input_lens, labels = [], []
     for x in range(batch_size):
-        sample = batch[x]
-        tensor = sample[0]
-        labels.append(sample[1])
-        seq_length = tensor.shape[0]
+        tensor, label = batch[x]
+        seq_length = tensor.size(0)
         # 将数据插入都0张量中，实现了padding
-        inputs[x, :seq_length] = tensor[:]
-        input_lens_ratio.append(seq_length/max_audio_length)
-    input_lens_ratio = np.array(input_lens_ratio, dtype='float32')
-    labels = np.array(labels, dtype='int64')
-    return torch.tensor(inputs), torch.tensor(labels), torch.tensor(input_lens_ratio)
+        features[x, :seq_length, :] = tensor[:, :]
+        labels.append(label)
+        input_lens.append(seq_length)
+    labels = torch.tensor(labels, dtype=torch.int64)
+    input_lens = torch.tensor(input_lens, dtype=torch.int64)
+    return features, labels, input_lens
```

## mvector/data_utils/featurizer.py

```diff
@@ -1,10 +1,10 @@
 import torch
-from torch import nn
 import torchaudio.compliance.kaldi as Kaldi
+from torch import nn
 from torchaudio.transforms import MelSpectrogram, Spectrogram, MFCC
 
 
 class AudioFeaturizer(nn.Module):
     """音频特征器
 
     :param feature_method: 所使用的预处理方法
@@ -24,40 +24,42 @@
         elif feature_method == 'MFCC':
             self.feat_fun = MFCC(**method_args)
         elif feature_method == 'Fbank':
             self.feat_fun = KaldiFbank(**method_args)
         else:
             raise Exception(f'预处理方法 {self._feature_method} 不存在!')
 
-    def forward(self, waveforms, input_lens_ratio):
+    def forward(self, waveforms, input_lens_ratio=None):
         """从AudioSegment中提取音频特征
 
         :param waveforms: Audio segment to extract features from.
         :type waveforms: AudioSegment
         :param input_lens_ratio: input length ratio
         :type input_lens_ratio: tensor
         :return: Spectrogram audio feature in 2darray.
         :rtype: ndarray
         """
+        if len(waveforms.shape) == 1:
+            waveforms = waveforms.unsqueeze(0)
         feature = self.feat_fun(waveforms)
         feature = feature.transpose(2, 1)
         # 归一化
         feature = feature - feature.mean(1, keepdim=True)
-        # 对掩码比例进行扩展
-        input_lens = (input_lens_ratio * feature.shape[1])
-        mask_lens = torch.round(input_lens).long()
-        mask_lens = mask_lens.unsqueeze(1)
-        input_lens = input_lens.int()
-        # 生成掩码张量
-        idxs = torch.arange(feature.shape[1], device=feature.device).repeat(feature.shape[0], 1)
-        mask = idxs < mask_lens
-        mask = mask.unsqueeze(-1)
-        # 对特征进行掩码操作
-        feature_masked = torch.where(mask, feature, torch.zeros_like(feature))
-        return feature_masked, input_lens
+        if input_lens_ratio is not None:
+            # 对掩码比例进行扩展
+            input_lens = (input_lens_ratio * feature.shape[1])
+            mask_lens = torch.round(input_lens).long()
+            mask_lens = mask_lens.unsqueeze(1)
+            # 生成掩码张量
+            idxs = torch.arange(feature.shape[1], device=feature.device).repeat(feature.shape[0], 1)
+            mask = idxs < mask_lens
+            mask = mask.unsqueeze(-1)
+            # 对特征进行掩码操作
+            feature = torch.where(mask, feature, torch.zeros_like(feature))
+        return feature
 
     @property
     def feature_dim(self):
         """返回特征大小
 
         :return: 特征大小
         :rtype: int
```

## mvector/data_utils/reader.py

```diff
@@ -1,89 +1,117 @@
 import os
 import random
 
 import numpy as np
+import torch
 from torch.utils.data import Dataset
 
 from mvector.data_utils.audio import AudioSegment
+from mvector.data_utils.featurizer import AudioFeaturizer
 from mvector.utils.logger import setup_logger
 
 logger = setup_logger(__name__)
 
 
-class CustomDataset(Dataset):
+class MVectorDataset(Dataset):
     def __init__(self,
                  data_list_path,
+                 audio_featurizer: AudioFeaturizer,
                  do_vad=True,
                  max_duration=3,
                  min_duration=0.5,
                  mode='train',
                  sample_rate=16000,
                  aug_conf={},
                  num_speakers=1000,
                  use_dB_normalization=True,
                  target_dB=-20):
         """音频数据加载器
 
         Args:
             data_list_path: 包含音频路径和标签的数据列表文件的路径
+            audio_featurizer: 声纹特征提取器
             do_vad: 是否对音频进行语音活动检测（VAD）来裁剪静音部分
             max_duration: 最长的音频长度，大于这个长度会裁剪掉
             min_duration: 过滤最短的音频长度
             aug_conf: 用于指定音频增强的配置
             mode: 数据集模式。在训练模式下，数据集可能会进行一些数据增强的预处理
             sample_rate: 采样率
             num_speakers: 总说话人数量
             use_dB_normalization: 是否对音频进行音量归一化
             target_dB: 音量归一化的大小
         """
-        super(CustomDataset, self).__init__()
+        super(MVectorDataset, self).__init__()
+        assert mode in ['train', 'eval', 'create_data', 'extract_feature']
         self.do_vad = do_vad
         self.max_duration = max_duration
         self.min_duration = min_duration
         self.mode = mode
         self._target_sample_rate = sample_rate
         self._use_dB_normalization = use_dB_normalization
         self._target_dB = target_dB
         self.aug_conf = aug_conf
         self.num_speakers = num_speakers
         self.noises_path = None
+        # 获取特征器
+        self.audio_featurizer = audio_featurizer
+        # 获取特征裁剪的大小
+        self.max_feature_len = self.get_crop_feature_len()
         # 获取数据列表
         with open(data_list_path, 'r', encoding='utf-8') as f:
             self.lines = f.readlines()
 
     def __getitem__(self, idx):
-        # 分割音频路径和标签
-        audio_path, spk_id = self.lines[idx].strip().split('\t')
+        # 分割数据文件路径和标签
+        data_path, spk_id = self.lines[idx].replace('\n', '').split('\t')
         spk_id = int(spk_id)
-        # 读取音频
-        audio_segment = AudioSegment.from_file(audio_path)
-        # 裁剪静音
-        if self.do_vad:
-            audio_segment.vad()
-        # 数据太短不利于训练
-        if self.mode == 'train':
-            if audio_segment.duration < self.min_duration:
-                return self.__getitem__(idx + 1 if idx < len(self.lines) - 1 else 0)
-        # 重采样
-        if audio_segment.sample_rate != self._target_sample_rate:
-            audio_segment.resample(self._target_sample_rate)
-        # 音频增强
-        if self.mode == 'train':
-            audio_segment, spk_id = self.augment_audio(audio_segment, spk_id, **self.aug_conf)
-        # decibel normalization
-        if self._use_dB_normalization:
-            audio_segment.normalize(target_db=self._target_dB)
-        # 裁剪需要的数据
-        audio_segment.crop(duration=self.max_duration, mode=self.mode)
-        return np.array(audio_segment.samples, dtype=np.float32), np.array(spk_id, dtype=np.int64)
+        # 如果后缀名为.npy的文件，那么直接读取
+        if data_path.endswith('.npy'):
+            feature = np.load(data_path)
+            if feature.shape[0] > self.max_feature_len:
+                crop_start = random.randint(0, feature.shape[0] - self.max_feature_len) if self.mode == 'eval' else 0
+                feature = feature[crop_start:crop_start + self.max_feature_len, :]
+            feature = torch.tensor(feature, dtype=torch.float32)
+        else:
+            # 读取音频
+            audio_segment = AudioSegment.from_file(data_path)
+            # 裁剪静音
+            if self.do_vad:
+                audio_segment.vad()
+            # 数据太短不利于训练
+            if self.mode == 'train':
+                if audio_segment.duration < self.min_duration:
+                    return self.__getitem__(idx + 1 if idx < len(self.lines) - 1 else 0)
+            # 重采样
+            if audio_segment.sample_rate != self._target_sample_rate:
+                audio_segment.resample(self._target_sample_rate)
+            # 音频增强
+            if self.mode == 'train':
+                audio_segment, spk_id = self.augment_audio(audio_segment, spk_id, **self.aug_conf)
+            # decibel normalization
+            if self._use_dB_normalization:
+                audio_segment.normalize(target_db=self._target_dB)
+            # 裁剪需要的数据
+            if self.mode != 'extract_feature' and audio_segment.duration > self.max_duration:
+                audio_segment.crop(duration=self.max_duration, mode=self.mode)
+            samples = torch.tensor(audio_segment.samples, dtype=torch.float32)
+            feature = self.audio_featurizer(samples)
+            feature = feature.squeeze(0)
+        spk_id = torch.tensor(spk_id, dtype=torch.int64)
+        return feature, spk_id
 
     def __len__(self):
         return len(self.lines)
 
+    def get_crop_feature_len(self):
+        samples = torch.randn((1, self.max_duration * self._target_sample_rate))
+        feature = self.audio_featurizer(samples).squeeze(0)
+        freq_len = feature.size(0)
+        return freq_len
+
     # 音频增强
     def augment_audio(self,
                       audio_segment,
                       spk_id,
                       speed_perturb=False,
                       speed_perturb_3_class=False,
                       volume_perturb=False,
```

## Comparing `mvector-1.0.2.dist-info/LICENSE` & `mvector-1.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mvector-1.0.2.dist-info/METADATA` & `mvector-1.0.3.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mvector
-Version: 1.0.2
+Version: 1.0.3
 Summary: Voice Print Recognition toolkit on Pytorch
 Home-page: https://github.com/yeyupiaoling/VoiceprintRecognition_Pytorch
 Download-URL: https://github.com/yeyupiaoling/VoiceprintRecognition_Pytorch.git
 Author: yeyupiaoling
 License: Apache License 2.0
 Keywords: Voice,Pytorch
 Classifier: Intended Audience :: Developers
@@ -167,28 +167,42 @@
 dataset/CN-Celeb2_flac/data/id11999/recitation-05-003.flac      2795
 dataset/CN-Celeb2_flac/data/id11999/recitation-04-017.flac      2795
 dataset/CN-Celeb2_flac/data/id11999/recitation-10-016.flac      2795
 dataset/CN-Celeb2_flac/data/id11999/recitation-09-001.flac      2795
 dataset/CN-Celeb2_flac/data/id11999/recitation-05-010.flac      2795
 ```
 
-# 修改预处理方法
+# 修改预处理方法（可选）
+
 配置文件中默认使用的是Fbank预处理方法，如果要使用其他预处理方法，可以修改配置文件中的安装下面方式修改，具体的值可以根据自己情况修改。如果不清楚如何设置参数，可以直接删除该部分，直接使用默认值。
 
 ```yaml
 # 数据预处理参数
 preprocess_conf:
   # 音频预处理方法，支持：MelSpectrogram、Spectrogram、MFCC、Fbank
   feature_method: 'Fbank'
   # 设置API参数，更参数查看对应API，不清楚的可以直接删除该部分，直接使用默认值
   method_args:
     sample_frequency: 16000
     num_mel_bins: 80
 ```
 
+# 提取特征（可选）
+
+在训练过程中，首先是要读取音频数据，然后提取特征，最后再进行训练。其中读取音频数据、提取特征也是比较消耗时间的，所以我们可以选择提前提取好取特征，训练模型的是就可以直接加载提取好的特征，这样训练速度会更快。这个提取特征是可选择，如果没有提取好的特征，训练模型的时候就会从读取音频数据，然后提取特征开始。提取特征步骤如下：
+
+1. 执行`extract_features.py`，提取特征，特征会保存在`dataset/features`目录下，并生成新的数据列表`train_list_features.txt`、`enroll_list_features.txt`和`trials_list_features.txt`。
+
+```shell
+python extract_features.py --configs=configs/cam++.yml --save_dir=dataset/features
+```
+
+2. 修改配置文件，将`dataset_conf.train_list`、`dataset_conf.enroll_list`和`dataset_conf.trials_list`修改为`train_list_features.txt`、`enroll_list_features.txt`和`trials_list_features.txt`。
+
+
 # 训练模型
 使用`train.py`训练模型，本项目支持多个音频预处理方式，通过`configs/ecapa_tdnn.yml`配置文件的参数`preprocess_conf.feature_method`可以指定，`MelSpectrogram`为梅尔频谱，`Spectrogram`为语谱图，`MFCC`梅尔频谱倒谱系数等等。通过参数`augment_conf_path`可以指定数据增强方式。训练过程中，会使用VisualDL保存训练日志，通过启动VisualDL可以随时查看训练结果，启动命令`visualdl --logdir=log --host 0.0.0.0`
 ```shell
 # 单卡训练
 CUDA_VISIBLE_DEVICES=0 python train.py
 # 多卡训练
 CUDA_VISIBLE_DEVICES=0,1 torchrun --standalone --nnodes=1 --nproc_per_node=2 train.py
```

## Comparing `mvector-1.0.2.dist-info/RECORD` & `mvector-1.0.3.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-mvector/__init__.py,sha256=nuwAt02ANJKWpNLCcQvX8UfLYxrRTI3OhFIZ_x5pb5g,134
-mvector/predict.py,sha256=RSiao4UGrZhrLUqkI07zA_u6__3cr8yD3IM860AVy2Y,17707
-mvector/trainer.py,sha256=aKX6ZAeDbrh2_9tak0HJPLqjgqXSagGZpeGiHo9yKeo,35940
+mvector/__init__.py,sha256=1Nqnj-dBG8NZOTjUbPp9NWTy0ddKc5o7d-vkgz53aw0,134
+mvector/predict.py,sha256=Io_wxBYRfalhOmSezKf6iJ84Xbf6p67JFFbqzROabT4,17513
+mvector/trainer.py,sha256=CJCp4SOyctHk-5lMunrG1tozw--L7LYV-oz2mOL3LO8,38106
 mvector/data_utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mvector/data_utils/audio.py,sha256=NQ4wf0SiUR20n76cg20LFPPwFCvESqbUmZrBhEWyyAM,22220
-mvector/data_utils/collate_fn.py,sha256=GxqMcZ5Q2ScQxj6crIUWeVygzWxIk9KAbC6GWW6awrQ,965
-mvector/data_utils/featurizer.py,sha256=-MAiHLattWuHK7fa4Wr1-7Jqw_AqKuY7hr-73nEqPBk,3587
-mvector/data_utils/reader.py,sha256=_QSfT5yonjNXrWQDkIm4KjSA6puxSTN7Dv2WHHuvzHs,5885
+mvector/data_utils/collate_fn.py,sha256=khDNN1B0xZpoXz1dLHJE4JBbXnOLPqcQvVlruVnRBv0,930
+mvector/data_utils/featurizer.py,sha256=dgiKRMuvAApNZBt36mdd3RDZJp3z0JTMwYBiHd6nRUg,3696
+mvector/data_utils/reader.py,sha256=pZz8HV3LVsuCXuRfOze3oVwUPF3lbiTWoj2hwFKCkSg,7407
 mvector/data_utils/spec_aug.py,sha256=Sr9-Ss6I7LA3TGMqzML_X-nb_nnMfUxt5KbsA6HJpzM,1572
 mvector/data_utils/utils.py,sha256=EmcQ5kvot_gIpmAyKALnxGWyqN0COYERp6nOKMoVK30,4712
 mvector/metric/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mvector/metric/metrics.py,sha256=59HlEhkSuV3_MKV41EkE9sLGQIfbHxtlWcUQezhJano,1517
 mvector/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mvector/models/campplus.py,sha256=1m5Y1F8ExpUeH-FTZd9WoKQ2Twd9EiuE3zn79ZRyvoc,13511
 mvector/models/ecapa_tdnn.py,sha256=U9EI5QlrMSQNgtIJ47eEmh2-p8QlttoE4-c_sSFqbCQ,5293
@@ -21,12 +21,12 @@
 mvector/models/resnet_se.py,sha256=aPElXGIlPjGNXJT5p8Z-942EsQ_n2eGEoGdlCkDdbSs,5522
 mvector/models/tdnn.py,sha256=O_YO-wUknUJPV991Ol3fOvq6T5okGjazaYCVSnEL2Ck,2963
 mvector/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mvector/utils/logger.py,sha256=-ssorx8FlHA_wrd2Eq6f4HkOqaOG2YseBGvYAo8NXN8,2839
 mvector/utils/record.py,sha256=S2sGoLPJrdRsrG7_ojNt4kwL05VNrOxnmnMOwNOZ9-0,1385
 mvector/utils/scheduler.py,sha256=3qgF4hNkOn-vE7kgN4vvj8Ou_6Y8gsPJjQoiWI1okOk,3538
 mvector/utils/utils.py,sha256=TprSWPMLDodFmxVJtGLRb0MmQ9xI16En7ZZvMJ9yuj0,2789
-mvector-1.0.2.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-mvector-1.0.2.dist-info/METADATA,sha256=bdMsIRRnPElIHf4gv4FjOkkJBMjav5-N300DUpa0FPc,32558
-mvector-1.0.2.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-mvector-1.0.2.dist-info/top_level.txt,sha256=biohDrNo0DJzZdjePn_XJZLCyGMA9w0u2mzmVVXM3cE,8
-mvector-1.0.2.dist-info/RECORD,,
+mvector-1.0.3.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+mvector-1.0.3.dist-info/METADATA,sha256=rIvhD-5mccMmqxyDD6ZgsOT2dZabVjeuQgLGfQ2CZvc,33611
+mvector-1.0.3.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+mvector-1.0.3.dist-info/top_level.txt,sha256=biohDrNo0DJzZdjePn_XJZLCyGMA9w0u2mzmVVXM3cE,8
+mvector-1.0.3.dist-info/RECORD,,
```


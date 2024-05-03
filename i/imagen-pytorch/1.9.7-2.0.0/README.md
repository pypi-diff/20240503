# Comparing `tmp/imagen-pytorch-1.9.7.tar.gz` & `tmp/imagen_pytorch-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imagen-pytorch-1.9.7.tar", last modified: Mon Aug 22 17:29:39 2022, max compression
+gzip compressed data, was "imagen_pytorch-2.0.0.tar", last modified: Fri May  3 16:55:30 2024, max compression
```

## Comparing `imagen-pytorch-1.9.7.tar` & `imagen_pytorch-2.0.0.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 17:29:39.349363 imagen-pytorch-1.9.7/
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-08-22 17:29:29.000000 imagen-pytorch-1.9.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      681 2022-08-22 17:29:39.349363 imagen-pytorch-1.9.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    31342 2022-08-22 17:29:29.000000 imagen-pytorch-1.9.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 17:29:39.349363 imagen-pytorch-1.9.7/imagen_pytorch/
--rw-r--r--   0 runner    (1001) docker     (121)      685 2022-08-22 17:29:29.000000 imagen-pytorch-1.9.7/imagen_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1595 2022-08-22 17:29:29.000000 imagen-pytorch-1.9.7/imagen_pytorch/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     6154 2022-08-22 17:29:29.000000 imagen-pytorch-1.9.7/imagen_pytorch/configs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1733 2022-08-22 17:29:29.000000 imagen-pytorch-1.9.7/imagen_pytorch/data.py
--rw-r--r--   0 runner    (1001) docker     (121)    30653 2022-08-22 17:29:29.000000 imagen-pytorch-1.9.7/imagen_pytorch/elucidated_imagen.py
--rw-r--r--   0 runner    (1001) docker     (121)    87117 2022-08-22 17:29:29.000000 imagen-pytorch-1.9.7/imagen_pytorch/imagen_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 17:29:39.349363 imagen-pytorch-1.9.7/imagen_pytorch/imagen_video/
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-08-22 17:29:29.000000 imagen-pytorch-1.9.7/imagen_pytorch/imagen_video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    53995 2022-08-22 17:29:29.000000 imagen-pytorch-1.9.7/imagen_pytorch/imagen_video/imagen_video.py
--rw-r--r--   0 runner    (1001) docker     (121)     3053 2022-08-22 17:29:29.000000 imagen-pytorch-1.9.7/imagen_pytorch/t5.py
--rw-r--r--   0 runner    (1001) docker     (121)    32674 2022-08-22 17:29:29.000000 imagen-pytorch-1.9.7/imagen_pytorch/trainer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1854 2022-08-22 17:29:29.000000 imagen-pytorch-1.9.7/imagen_pytorch/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-08-22 17:29:29.000000 imagen-pytorch-1.9.7/imagen_pytorch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 17:29:39.349363 imagen-pytorch-1.9.7/imagen_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      681 2022-08-22 17:29:39.000000 imagen-pytorch-1.9.7/imagen_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      604 2022-08-22 17:29:39.000000 imagen-pytorch-1.9.7/imagen_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-22 17:29:39.000000 imagen-pytorch-1.9.7/imagen_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-22 17:29:39.000000 imagen-pytorch-1.9.7/imagen_pytorch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      194 2022-08-22 17:29:39.000000 imagen-pytorch-1.9.7/imagen_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-08-22 17:29:39.000000 imagen-pytorch-1.9.7/imagen_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-22 17:29:39.349363 imagen-pytorch-1.9.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1394 2022-08-22 17:29:29.000000 imagen-pytorch-1.9.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:55:30.507604 imagen_pytorch-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-03 16:55:22.000000 imagen_pytorch-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-03 16:55:22.000000 imagen_pytorch-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-03 16:55:30.507604 imagen_pytorch-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    39326 2024-05-03 16:55:22.000000 imagen_pytorch-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:55:30.507604 imagen_pytorch-2.0.0/imagen_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-03 16:55:22.000000 imagen_pytorch-2.0.0/imagen_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7467 2024-05-03 16:55:22.000000 imagen_pytorch-2.0.0/imagen_pytorch/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-05-03 16:55:22.000000 imagen_pytorch-2.0.0/imagen_pytorch/configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-05-03 16:55:22.000000 imagen_pytorch-2.0.0/imagen_pytorch/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-03 16:55:22.000000 imagen_pytorch-2.0.0/imagen_pytorch/default_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)    36761 2024-05-03 16:55:22.000000 imagen_pytorch-2.0.0/imagen_pytorch/elucidated_imagen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    96490 2024-05-03 16:55:22.000000 imagen_pytorch-2.0.0/imagen_pytorch/imagen_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62497 2024-05-03 16:55:22.000000 imagen_pytorch-2.0.0/imagen_pytorch/imagen_video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-03 16:55:22.000000 imagen_pytorch-2.0.0/imagen_pytorch/t5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:55:30.507604 imagen_pytorch-2.0.0/imagen_pytorch/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-03 16:55:22.000000 imagen_pytorch-2.0.0/imagen_pytorch/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-03 16:55:22.000000 imagen_pytorch-2.0.0/imagen_pytorch/test/test_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33716 2024-05-03 16:55:22.000000 imagen_pytorch-2.0.0/imagen_pytorch/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-03 16:55:22.000000 imagen_pytorch-2.0.0/imagen_pytorch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-03 16:55:22.000000 imagen_pytorch-2.0.0/imagen_pytorch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:55:30.507604 imagen_pytorch-2.0.0/imagen_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-03 16:55:30.000000 imagen_pytorch-2.0.0/imagen_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-03 16:55:30.000000 imagen_pytorch-2.0.0/imagen_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 16:55:30.000000 imagen_pytorch-2.0.0/imagen_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-03 16:55:30.000000 imagen_pytorch-2.0.0/imagen_pytorch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-03 16:55:30.000000 imagen_pytorch-2.0.0/imagen_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-03 16:55:30.000000 imagen_pytorch-2.0.0/imagen_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 16:55:30.507604 imagen_pytorch-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-03 16:55:22.000000 imagen_pytorch-2.0.0/setup.py
```

### Comparing `imagen-pytorch-1.9.7/LICENSE` & `imagen_pytorch-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `imagen-pytorch-1.9.7/README.md` & `imagen_pytorch-2.0.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 
 ## Shoutouts
 
 - <a href="https://stability.ai/">StabilityAI</a> for the generous sponsorship, as well as my other sponsors out there
 
 - <a href="https://huggingface.co/">🤗 Huggingface</a> for their amazing transformers library. The text encoder portion is pretty much taken care of because of them
 
+- <a href="http://www.jonathanho.me/">Jonathan Ho</a> for bringing about a revolution in generative artificial intelligence through <a href="https://arxiv.org/abs/2006.11239">his seminal paper</a>
+
 - <a href="https://github.com/sgugger">Sylvain</a> and <a href="https://github.com/muellerzr">Zachary</a> for the <a href="https://github.com/huggingface/accelerate">Accelerate</a> library, which this repository uses for distributed training
 
 - <a href="https://github.com/arogozhnikov">Alex</a> for <a href="https://github.com/arogozhnikov/einops">einops</a>, indispensable tool for tensor manipulation
 
 - <a href="https://github.com/jorgemcgomes">Jorge Gomes</a> for helping out with the T5 loading code and advice on the correct T5 version
 
 - <a href="https://github.com/crowsonkb">Katherine Crowson</a>, for her <a href="https://github.com/crowsonkb/v-diffusion-jax/blob/master/diffusion/utils.py">beautiful code</a>, which helped me understand the continuous time version of gaussian diffusion
@@ -36,14 +38,18 @@
 
 - <a href="https://github.com/KhrulkovV">Valentin</a> for pointing out insufficient skip connections in the unet, as well as the specific method of attention conditioning in the base-unet in the appendix
 
 - <a href="https://github.com/BIGJUN777">BIGJUN</a> for catching a big bug with continuous time gaussian diffusion noise level conditioning at inference time
 
 - <a href="https://github.com/animebing">Bingbing</a> for identifying a bug with sampling and order of normalizing and noising with low resolution conditioning image
 
+- <a href="https://github.com/TheFusion21">Kay</a> for contributing one line command training of Imagen!
+
+- <a href="https://github.com/HReynaud">Hadrien Reynaud</a> for testing out text-to-video on a medical dataset, sharing his results, and identifying issues!
+
 ## Install
 
 ```bash
 $ pip install imagen-pytorch
 ```
 
 ## Usage
@@ -385,24 +391,75 @@
 $ accelerate launch train.py
 ```
 
 That's it!
 
 ## Command-line
 
-To further democratize the use of this machine imagination, I have built in the ability to generate an image with any text prompt using one command line as so
+Imagen can also be used via CLI directly.
+
+### Configuration
+
+ex.
+
+```bash
+$ imagen config
+```
+or
+```bash
+$ imagen config --path ./configs/config.json
+```
+
+In the config you are able to change settings for the trainer, dataset and the imagen config.
+
+The Imagen config parameters can be found <a href="https://github.com/lucidrains/imagen-pytorch/blob/f8cc75f4d9020998c577b3770d3f260ce2ee2dcf/imagen_pytorch/configs.py#L68">here</a>
+
+The Elucidated Imagen config parameters can be found <a href="https://github.com/lucidrains/imagen-pytorch/blob/f8cc75f4d9020998c577b3770d3f260ce2ee2dcf/imagen_pytorch/configs.py#L108">here</a>
+
+The Imagen Trainer config parameters can be found <a href="https://github.com/lucidrains/imagen-pytorch/blob/f8cc75f4d9020998c577b3770d3f260ce2ee2dcf/imagen_pytorch/trainer.py#L226">here</a>
+
+For the dataset parameters all dataloader parameters can be used.
+
+### Training
+
+This command allows you to train or resume training your model
+
+ex.
+```bash
+$ imagen train
+```
+or
+```bash
+$ imagen train --unet 2 --epoches 10
+```
+
+You can pass following arguments to the training command.
+
+- `--config` specify the config file to use for training [default: ./imagen_config.json]
+- `--unet` the index of the unet to train [default: 1]
+- `--epoches` how many epoches to train for [default: 50]
+
+### Sampling
+
+Be aware when sampling your checkpoint should have trained all unets to get a usable result.
 
 ex.
 
 ```bash
-$ imagen --model ./path/to/model/checkpoint.pt "a squirrel raiding the birdfeeder"
+$ imagen sample --model ./path/to/model/checkpoint.pt "a squirrel raiding the birdfeeder"
 # image is saved to ./a_squirrel_raiding_the_birdfeeder.png
 ```
 
-In order to save checkpoints that can make use of this feature, you must instantiate your Imagen instance using the config classes, `ImagenConfig` and `ElucidatedImagenConfig`
+You can pass following arguments to the sample command.
+
+- `--model` specify the model file to use for sampling
+- `--cond_scale` conditioning scale (classifier free guidance) in decoder
+- `--load_ema` load EMA version of unets if available
+
+In order to use a saved checkpoint with this feature, you either must instantiate your Imagen instance using the config classes, `ImagenConfig` and `ElucidatedImagenConfig` or create a checkpoint via the CLI directly
 
 For proper training, you'll likely want to setup config-driven training anyways.
 
 ex.
 
 ```python
 import torch
@@ -460,14 +517,31 @@
     'fireworks with blue and green sparkles',
     'dust motes swirling in the morning sunshine on the windowsill'
 ], inpaint_images = inpaint_images, inpaint_masks = inpaint_masks, cond_scale = 5.)
 
 inpainted_images # (4, 3, 512, 512)
 ```
 
+For video, similarly pass in your videos to `inpaint_videos` keyword on `.sample`. Inpainting mask can either be the same across all frames `(batch, height, width)` or different `(batch, frames, height, width)`
+
+```python
+
+inpaint_videos = torch.randn(4, 3, 8, 512, 512).cuda()   # (batch, channels, frames, height, width)
+inpaint_masks = torch.ones((4, 8, 512, 512)).bool().cuda()  # (batch, frames, height, width)
+
+inpainted_videos = trainer.sample(texts = [
+    'a whale breaching from afar',
+    'young girl blowing out candles on her birthday cake',
+    'fireworks with blue and green sparkles',
+    'dust motes swirling in the morning sunshine on the windowsill'
+], inpaint_videos = inpaint_videos, inpaint_masks = inpaint_masks, cond_scale = 5.)
+
+inpainted_videos # (4, 3, 8, 512, 512)
+```
+
 ## Experimental
 
 <a href="https://research.nvidia.com/person/tero-karras">Tero Karras</a> of StyleGAN fame has written a <a href="https://arxiv.org/abs/2206.00364">new paper</a> with results that have been corroborated by a number of independent researchers as well as on my own machine. I have decided to create a version of `Imagen`, the `ElucidatedImagen`, so that one can use the new elucidated DDPM for text-guided cascading generation.
 
 Simply import `ElucidatedImagen`, and then instantiate the instance as you did before. The hyperparameters are different than the usual ones for discrete and continuous time gaussian diffusion, and can be individualized for each unet in the cascade.
 
 Ex.
@@ -494,18 +568,20 @@
     S_noise = 1.003,
 ).cuda()
 
 # rest is the same as above
 
 ```
 
-## Text to Video (ongoing research)
+## Text to Video
 
 This repository will also start accumulating new research around text guided video synthesis. For starters it will adopt the 3d unet architecture described by Jonathan Ho in <a href="https://arxiv.org/abs/2204.03458">Video Diffusion Models</a>
 
+Update: verified <a href="https://github.com/lucidrains/imagen-pytorch/issues/305#issuecomment-1407015141">working</a> by <a href="https://github.com/HReynaud">Hadrien Reynaud</a>!
+
 Ex.
 
 ```python
 import torch
 from imagen_pytorch import Unet3D, ElucidatedImagen, ImagenTrainer
 
 unet1 = Unet3D(dim = 64, dim_mults = (1, 2, 4, 8)).cuda()
@@ -514,14 +590,15 @@
 
 # elucidated imagen, which contains the unets above (base unet and super resoluting ones)
 
 imagen = ElucidatedImagen(
     unets = (unet1, unet2),
     image_sizes = (16, 32),
     random_crop_sizes = (None, 16),
+    temporal_downsample_factor = (2, 1),        # in this example, the first unet would receive the video temporally downsampled by 2x
     num_sample_steps = 10,
     cond_drop_prob = 0.1,
     sigma_min = 0.002,                          # min noise level
     sigma_max = (80, 160),                      # max noise level, double the max noise level for upsampler
     sigma_data = 0.5,                           # standard deviation of data distribution
     rho = 7,                                    # controls the sampling schedule
     P_mean = -1.2,                              # mean of log-normal distribution from which noise is drawn for training
@@ -543,23 +620,30 @@
 
 videos = torch.randn(4, 3, 10, 32, 32).cuda() # (batch, channels, time / video frames, height, width)
 
 # feed images into imagen, training each unet in the cascade
 # for this example, only training unet 1
 
 trainer = ImagenTrainer(imagen)
-trainer(videos, texts = texts, unet_number = 1)
+
+# you can also ignore time when training on video initially, shown to improve results in video-ddpm paper. eventually will make the 3d unet trainable with either images or video. research shows it is essential (with current data regimes) to train first on text-to-image. probably won't be true in another decade. all big data becomes small data
+
+trainer(videos, texts = texts, unet_number = 1, ignore_time = False)
 trainer.update(unet_number = 1)
 
 videos = trainer.sample(texts = texts, video_frames = 20) # extrapolating to 20 frames from training on 10 frames
 
 videos.shape # (4, 3, 20, 32, 32)
 
 ```
 
+You can also train on text - image pairs first. The `Unet3D` will automatically convert it to single framed videos and learn without the temporal components (by automatically setting `ignore_time = True`), whether it be 1d convolutions or causal attention across time.
+
+This is the current approach taken by all the big artificial intelligence labs (Brain, MetaAI, Bytedance)
+
 ## FAQ
 
 - Why are my generated images not aligning well with the text?
 
 Imagen uses an algorithm called <a href="https://openreview.net/forum?id=qw8AKxfYbI">Classifier Free Guidance</a>. When sampling, you apply a scale to the conditioning (text in this case) of greater than `1.0`.
 
 Researcher <a href="https://github.com/Netruk44 ">Netruk44</a> have reported `5-10` to be optimal, but anything greater than `10` to break.
@@ -578,14 +662,28 @@
 
 More the reason why you should start training your own model, starting today! The last thing we need is this technology being in the hands of an elite few. Hopefully this repository reduces the work to just finding the necessary compute, and augmenting with your own curated dataset.
 
 - What am I allowed to do with this repository?
 
 Anything! It is MIT licensed. In other words, you can freely copy / paste for your own research, remixed for whatever modality you can think of. Go train amazing models for profit, for science, or simply to satiate your own personal pleasure at witnessing something divine unravel in front of you.
 
+## Cool Applications!
+
+- <a href="https://arxiv.org/abs/2303.12644">Echocardiogram synthesis</a> <a href="https://github.com/HReynaud/EchoDiffusion">[Code]</a>
+
+- <a href="https://www.biorxiv.org/content/10.1101/2023.10.25.564065v1">SOTA Hi-C contact matrix synthesis</a> <a href="https://github.com/CHNFTQ/Capricorn">[Code]</a>
+
+- <a href="https://arxiv.org/abs/2311.15941">Floor plan generation</a>
+
+- <a href="https://arxiv.org/abs/2312.01152">Ultra High Resolution Histopathology Slides</a>
+
+- <a href="https://arxiv.org/abs/2312.03043">Synthetic Laparoscopic Images</a>
+
+- <a href="https://www.nature.com/articles/s42256-023-00762-x">Designing MetaMaterials</a>
+
 ## Related Works
 
 - <a href="https://github.com/archinetai/audio-diffusion-pytorch">Audio diffusion</a> from <a href="https://github.com/flavioschneider">Flavio Schneider</a>
 
 - <a href="https://github.com/AssemblyAI-Examples/MinImagen">Mini Imagen</a> from <a href="https://github.com/oconnoob">Ryan O.</a> | <a href="https://www.assemblyai.com/blog/build-your-own-imagen-text-to-image-model/">AssemblyAI writeup</a>
 
 ## Todo
@@ -624,31 +722,48 @@
 - [x] extend to video generation, using axial time attention as in Ho's video ddpm paper
 - [x] allow elucidated imagen to generalize to any shape
 - [x] allow for imagen to generalize to any shape
 - [x] add <a href="https://github.com/lucidrains/x-transformers#dynamic-positional-bias">dynamic positional bias</a> for the best type of length extrapolation across video time
 - [x] move video frames to sample function, as we will be attempting time extrapolation
 - [x] attention bias to null key / values should be a learned scalar of head dimension
 - [x] add self-conditioning from <a href="https://arxiv.org/abs/2208.04202">bit diffusion</a> paper, already coded up at <a href="https://github.com/lucidrains/denoising-diffusion-pytorch/commit/beb2f2d8dd9b4f2bd5be4719f37082fe061ee450">ddpm-pytorch</a>
+- [x] add v-parameterization (https://arxiv.org/abs/2202.00512) from <a href="https://imagen.research.google/video/paper.pdf">imagen video</a> paper, the only thing new
+- [x] incorporate all learnings from make-a-video (https://makeavideo.studio/)
+- [x] build out CLI tool for training, resuming training off config file
+- [x] allow for temporal interpolation at specific stages
+- [x] make sure temporal interpolation works with inpainting
+- [x] make sure one can customize all interpolation modes (some researchers are finding better results with trilinear)
+- [x] imagen-video : allow for conditioning on preceding (and possibly future) frames of videos. ignore time should not be allowed in that scenario
+- [x] make sure to automatically take care of temporal down/upsampling for conditioning video frames, but allow for an option to turn it off
+- [x] make sure inpainting works with video
+- [x] make sure inpainting mask for video can accept be customized per frame
+
+- [ ] add flash attention
 - [ ] reread <a href="https://arxiv.org/abs/2205.15868">cogvideo</a> and figure out how frame rate conditioning could be used
 - [ ] bring in attention expertise for self attention layers in unet3d
 - [ ] consider bringing in NUWA's 3d convolutional attention
 - [ ] consider transformer-xl memories in the temporal attention blocks
 - [ ] consider <a href="github.com/lucidrains/perceiver-ar-pytorch">perceiver-ar approach</a> to attending to past time
 - [ ] frame dropouts during attention for achieving both regularizing effect as well as shortened training time
 - [ ] investigate frank wood's claims https://github.com/lucidrains/flexible-diffusion-modeling-videos-pytorch and either add the hierarchical sampling technique, or let people know about its deficiencies
-- [ ] make sure inpainting works with video
 - [ ] offer challenging moving mnist (with distractor objects) as a one-line trainable baseline for researchers to branch off of for text to video
-- [ ] build out CLI tool for training, resuming training off config file
 - [ ] preencoding of text to memmapped embeddings
 - [ ] be able to create dataloader iterators based on the old epoch style, also configure shuffling etc
 - [ ] be able to also pass in arguments (instead of requiring forward to be all keyword args on model)
 - [ ] bring in reversible blocks from revnets for 3d unet, to lessen memory burden
 - [ ] add ability to only train super-resolution network
 - [ ] read <a href="https://arxiv.org/abs/2206.00927v1">dpm-solver</a> see if it is applicable to continuous time gaussian diffusion
 - [ ] allow for conditioning video frames with arbitrary absolute times (calculate RPE during temporal attention)
+- [ ] accommodate <a href="https://dreambooth.github.io/">dream booth</a> fine tuning
+- [ ] add textual inversion
+- [ ] cleanup self conditioning to be extracted at imagen instantiation
+- [ ] make sure eventual dreambooth works with imagen-video
+- [ ] add framerate conditioning for video diffusion
+- [ ] make sure one can simulataneously condition on video frames as a prompt, as well as some conditioning image across all frames
+- [ ] test and add distillation technique from <a href="https://arxiv.org/abs/2303.01469">consistency models</a>
 
 ## Citations
 
 ```bibtex
 @inproceedings{Saharia2022PhotorealisticTD,
     title   = {Photorealistic Text-to-Image Diffusion Models with Deep Language Understanding},
     author  = {Chitwan Saharia and William Chan and Saurabh Saxena and Lala Li and Jay Whang and Emily L. Denton and Seyed Kamyar Seyed Ghasemipour and Burcu Karagol Ayan and Seyedeh Sara Mahdavi and Raphael Gontijo Lopes and Tim Salimans and Jonathan Ho and David Fleet and Mohammad Norouzi},
@@ -661,24 +776,14 @@
     title   = {Flamingo: a Visual Language Model for Few-Shot Learning},
     author  = {Jean-Baptiste Alayrac et al},
     year    = {2022}
 }
 ```
 
 ```bibtex
-@article{Choi2022PerceptionPT,
-    title   = {Perception Prioritized Training of Diffusion Models},
-    author  = {Jooyoung Choi and Jungbeom Lee and Chaehun Shin and Sungwon Kim and Hyunwoo J. Kim and Sung-Hoon Yoon},
-    journal = {ArXiv},
-    year    = {2022},
-    volume  = {abs/2204.00227}
-}
-```
-
-```bibtex
 @inproceedings{Sankararaman2022BayesFormerTW,
     title   = {BayesFormer: Transformer with Uncertainty Estimation},
     author  = {Karthik Abinav Sankararaman and Sinong Wang and Han Fang},
     year    = {2022}
 }
 ```
 
@@ -764,7 +869,81 @@
     author  = {Ting Chen and Ruixiang Zhang and Geoffrey Hinton},
     year    = {2022},
     eprint  = {2208.04202},
     archivePrefix = {arXiv},
     primaryClass = {cs.CV}
 }
 ```
+
+```bibtex
+@misc{Singer2022,
+    author  = {Uriel Singer},
+    url     = {https://makeavideo.studio/Make-A-Video.pdf}
+}
+```
+
+```bibtex
+@article{Sunkara2022NoMS,
+    title   = {No More Strided Convolutions or Pooling: A New CNN Building Block for Low-Resolution Images and Small Objects},
+    author  = {Raja Sunkara and Tie Luo},
+    journal = {ArXiv},
+    year    = {2022},
+    volume  = {abs/2208.03641}
+}
+```
+
+```bibtex
+@article{Salimans2022ProgressiveDF,
+    title   = {Progressive Distillation for Fast Sampling of Diffusion Models},
+    author  = {Tim Salimans and Jonathan Ho},
+    journal = {ArXiv},
+    year    = {2022},
+    volume  = {abs/2202.00512}
+}
+```
+
+```bibtex
+@article{Ho2022ImagenVH,
+    title   = {Imagen Video: High Definition Video Generation with Diffusion Models},
+    author  = {Jonathan Ho and William Chan and Chitwan Saharia and Jay Whang and Ruiqi Gao and Alexey A. Gritsenko and Diederik P. Kingma and Ben Poole and Mohammad Norouzi and David J. Fleet and Tim Salimans},
+    journal = {ArXiv},
+    year    = {2022},
+    volume  = {abs/2210.02303}
+}
+```
+
+```bibtex
+@misc{gilmer2023intriguing
+    title  = {Intriguing Properties of Transformer Training Instabilities},
+    author = {Justin Gilmer, Andrea Schioppa, and Jeremy Cohen},
+    year   = {2023},
+    status = {to be published - one attention stabilization technique is circulating within Google Brain, being used by multiple teams}
+}
+```
+
+```bibtex
+@inproceedings{Hang2023EfficientDT,
+    title   = {Efficient Diffusion Training via Min-SNR Weighting Strategy},
+    author  = {Tiankai Hang and Shuyang Gu and Chen Li and Jianmin Bao and Dong Chen and Han Hu and Xin Geng and Baining Guo},
+    year    = {2023}
+}
+```
+
+```bibtex
+@article{Zhang2021TokenST,
+    title   = {Token Shift Transformer for Video Classification},
+    author  = {Hao Zhang and Y. Hao and Chong-Wah Ngo},
+    journal = {Proceedings of the 29th ACM International Conference on Multimedia},
+    year    = {2021}
+}
+```
+
+```bibtex
+@inproceedings{anonymous2022normformer,
+    title   = {NormFormer: Improved Transformer Pretraining with Extra Normalization},
+    author  = {Anonymous},
+    booktitle = {Submitted to The Tenth International Conference on Learning Representations },
+    year    = {2022},
+    url     = {https://openreview.net/forum?id=GMYWzWztDx5},
+    note    = {under review}
+}
+```
```

#### html2text {}

```diff
@@ -6,135 +6,138 @@
 clipping for improved classifier free guidance, noise level conditioning, and a
 memory efficient unet design. It appears neither CLIP nor prior network is
 needed after all. And so research continues. _A_I_ _C_o_f_f_e_e_ _B_r_e_a_k_ _w_i_t_h_ _L_e_t_i_t_i_a |
 _A_s_s_e_m_b_l_y_ _A_I | _Y_a_n_n_i_c_ _K_i_l_c_h_e_r Please join _[_J_o_i_n_ _u_s_ _o_n_ _D_i_s_c_o_r_d_]if you are
 interested in helping out with the replication with the _L_A_I_O_N community ##
 Shoutouts - _S_t_a_b_i_l_i_t_y_A_I for the generous sponsorship, as well as my other
 sponsors out there - _ð__¤__ _H_u_g_g_i_n_g_f_a_c_e for their amazing transformers library.
-The text encoder portion is pretty much taken care of because of them - _S_y_l_v_a_i_n
-and _Z_a_c_h_a_r_y for the _A_c_c_e_l_e_r_a_t_e library, which this repository uses for
-distributed training - _A_l_e_x for _e_i_n_o_p_s, indispensable tool for tensor
-manipulation - _J_o_r_g_e_ _G_o_m_e_s for helping out with the T5 loading code and advice
-on the correct T5 version - _K_a_t_h_e_r_i_n_e_ _C_r_o_w_s_o_n, for her _b_e_a_u_t_i_f_u_l_ _c_o_d_e, which
-helped me understand the continuous time version of gaussian diffusion -
-_M_a_r_u_n_i_n_e and _N_e_t_r_u_k_4_4, for reviewing code, sharing experimental results, and
-help with debugging - _M_a_r_u_n_i_n_e for providing a _p_o_t_e_n_t_i_a_l_ _s_o_l_u_t_i_o_n for a color
-shifting issue in the memory efficient u-nets. Thanks to _J_a_c_o_b for sharing
-experimental comparisons between the base and memory-efficient unets - _M_a_r_u_n_i_n_e
-for finding numerous bugs, resolving an issue with resize right, and for
-sharing his experimental configurations and results - _M_a_l_u_m_a_D_e_v for proposing
-the use of pixel shuffle upsampler to fix checkboard artifacts - _V_a_l_e_n_t_i_n for
-pointing out insufficient skip connections in the unet, as well as the specific
-method of attention conditioning in the base-unet in the appendix - _B_I_G_J_U_N for
-catching a big bug with continuous time gaussian diffusion noise level
-conditioning at inference time - _B_i_n_g_b_i_n_g for identifying a bug with sampling
-and order of normalizing and noising with low resolution conditioning image ##
-Install ```bash $ pip install imagen-pytorch ``` ## Usage ```python import
-torch from imagen_pytorch import Unet, Imagen # unet for imagen unet1 = Unet
-( dim = 32, cond_dim = 512, dim_mults = (1, 2, 4, 8), num_resnet_blocks = 3,
-layer_attns = (False, True, True, True), layer_cross_attns = (False, True,
-True, True) ) unet2 = Unet( dim = 32, cond_dim = 512, dim_mults = (1, 2, 4, 8),
-num_resnet_blocks = (2, 4, 8, 8), layer_attns = (False, False, False, True),
-layer_cross_attns = (False, False, False, True) ) # imagen, which contains the
-unets above (base unet and super resoluting ones) imagen = Imagen( unets =
-(unet1, unet2), image_sizes = (64, 256), timesteps = 1000, cond_drop_prob = 0.1
-).cuda() # mock images (get a lot of this) and text encodings from large T5
-text_embeds = torch.randn(4, 256, 768).cuda() images = torch.randn(4, 3, 256,
-256).cuda() # feed images into imagen, training each unet in the cascade for i
-in (1, 2): loss = imagen(images, text_embeds = text_embeds, unet_number = i)
-loss.backward() # do the above for many many many many steps # now you can
-sample an image based on the text embeddings from the cascading ddpm images =
-imagen.sample(texts = [ 'a whale breaching from afar', 'young girl blowing out
-candles on her birthday cake', 'fireworks with blue and green sparkles' ],
-cond_scale = 3.) images.shape # (3, 3, 256, 256) ``` For simpler training, you
-can directly supply text strings instead of precomputing text encodings.
-(Although for scaling purposes, you will definitely want to precompute the
-textual embeddings + mask) The number of textual captions must match the batch
-size of the images if you go this route. ```python # mock images and text (get
-a lot of this) texts = [ 'a child screaming at finding a worm within a half-
-eaten apple', 'lizard running across the desert on two feet', 'waking up to a
-psychedelic landscape', 'seashells sparkling in the shallow waters' ] images =
-torch.randn(4, 3, 256, 256).cuda() # feed images into imagen, training each
-unet in the cascade for i in (1, 2): loss = imagen(images, texts = texts,
-unet_number = i) loss.backward() ``` With the `ImagenTrainer` wrapper class,
-the exponential moving averages for all of the U-nets in the cascading DDPM
-will be automatically taken care of when calling `update` ```python import
-torch from imagen_pytorch import Unet, Imagen, ImagenTrainer # unet for imagen
-unet1 = Unet( dim = 32, cond_dim = 512, dim_mults = (1, 2, 4, 8),
-num_resnet_blocks = 3, layer_attns = (False, True, True, True), ) unet2 = Unet
-( dim = 32, cond_dim = 512, dim_mults = (1, 2, 4, 8), num_resnet_blocks = (2,
-4, 8, 8), layer_attns = (False, False, False, True), layer_cross_attns =
-(False, False, False, True) ) # imagen, which contains the unets above (base
-unet and super resoluting ones) imagen = Imagen( unets = (unet1, unet2),
-text_encoder_name = 't5-large', image_sizes = (64, 256), timesteps = 1000,
-cond_drop_prob = 0.1 ).cuda() # wrap imagen with the trainer class trainer =
-ImagenTrainer(imagen) # mock images (get a lot of this) and text encodings from
-large T5 text_embeds = torch.randn(64, 256, 1024).cuda() images = torch.randn
-(64, 3, 256, 256).cuda() # feed images into imagen, training each unet in the
-cascade loss = trainer( images, text_embeds = text_embeds, unet_number = 1, #
-training on unet number 1 in this example, but you will have to also save
-checkpoints and then reload and continue training on unet number 2
-max_batch_size = 4 # auto divide the batch of 64 up into batch size of 4 and
-accumulate gradients, so it all fits in memory ) trainer.update(unet_number =
-1) # do the above for many many many many steps # now you can sample an image
-based on the text embeddings from the cascading ddpm images = trainer.sample
-(texts = [ 'a puppy looking anxiously at a giant donut on the table', 'the
-milky way galaxy in the style of monet' ], cond_scale = 3.) images.shape # (2,
-3, 256, 256) ``` You can also train Imagen without text (unconditional image
-generation) as follows ```python import torch from imagen_pytorch import Unet,
-Imagen, SRUnet256, ImagenTrainer # unets for unconditional imagen unet1 = Unet
-( dim = 32, dim_mults = (1, 2, 4), num_resnet_blocks = 3, layer_attns = (False,
-True, True), layer_cross_attns = False, use_linear_attn = True ) unet2 =
-SRUnet256( dim = 32, dim_mults = (1, 2, 4), num_resnet_blocks = (2, 4, 8),
-layer_attns = (False, False, True), layer_cross_attns = False ) # imagen, which
-contains the unets above (base unet and super resoluting ones) imagen = Imagen
-( condition_on_text = False, # this must be set to False for unconditional
-Imagen unets = (unet1, unet2), image_sizes = (64, 128), timesteps = 1000 )
-trainer = ImagenTrainer(imagen).cuda() # now get a ton of images and feed it
-through the Imagen trainer training_images = torch.randn(4, 3, 256, 256).cuda()
-# train each unet separately # in this example, only training on unet number 1
-loss = trainer(training_images, unet_number = 1) trainer.update(unet_number =
-1) # do the above for many many many many steps # now you can sample images
-unconditionally from the cascading unet(s) images = trainer.sample(batch_size =
-16) # (16, 3, 128, 128) ``` Or train only super-resoluting unets ```python
-import torch from imagen_pytorch import Unet, NullUnet, Imagen # unet for
-imagen unet1 = NullUnet() # add a placeholder "null" unet for the base unet
-unet2 = Unet( dim = 32, cond_dim = 512, dim_mults = (1, 2, 4, 8),
-num_resnet_blocks = (2, 4, 8, 8), layer_attns = (False, False, False, True),
-layer_cross_attns = (False, False, False, True) ) # imagen, which contains the
-unets above (base unet and super resoluting ones) imagen = Imagen( unets =
-(unet1, unet2), image_sizes = (64, 256), timesteps = 250, cond_drop_prob = 0.1
-).cuda() # mock images (get a lot of this) and text encodings from large T5
-text_embeds = torch.randn(4, 256, 768).cuda() images = torch.randn(4, 3, 256,
-256).cuda() # feed images into imagen, training each unet in the cascade loss =
-imagen(images, text_embeds = text_embeds, unet_number = 2) loss.backward() # do
-the above for many many many many steps # now you can sample an image based on
-the text embeddings as well as low resolution images lowres_images =
-torch.randn(3, 3, 64, 64).cuda() # starting un-resoluted images images =
-imagen.sample( texts = [ 'a whale breaching from afar', 'young girl blowing out
-candles on her birthday cake', 'fireworks with blue and green sparkles' ],
-start_at_unet_number = 2, # start at unet number 2 start_image_or_video =
-lowres_images, # pass in low resolution images to be resoluted cond_scale = 3.)
-images.shape # (3, 3, 256, 256) ``` At any time you can save and load the
-trainer and all associated states with the `save` and `load` methods. It is
-recommended you use these methods instead of manually saving with a
-`state_dict` call, as there are some device memory management being done
-underneath the hood within the trainer. ex. ```python trainer.save('./path/to/
-checkpoint.pt') trainer.load('./path/to/checkpoint.pt') trainer.steps # (2,)
-step number for each of the unets, in this case 2 ``` ## Dataloader You can
-also rely on the `ImagenTrainer` to automatically train off `DataLoader`
-instances. You simply have to craft your `DataLoader` to return either `images`
-(for unconditional case), or of `('images', 'text_embeds')` for text-guided
-generation. ex. unconditional training ```python from imagen_pytorch import
-Unet, Imagen, ImagenTrainer from imagen_pytorch.data import Dataset # unets for
-unconditional imagen unet = Unet( dim = 32, dim_mults = (1, 2, 4, 8),
-num_resnet_blocks = 1, layer_attns = (False, False, False, True),
-layer_cross_attns = False ) # imagen, which contains the unet above imagen =
-Imagen( condition_on_text = False, # this must be set to False for
-unconditional Imagen unets = unet, image_sizes = 128, timesteps = 1000 )
+The text encoder portion is pretty much taken care of because of them -
+_J_o_n_a_t_h_a_n_ _H_o for bringing about a revolution in generative artificial
+intelligence through _h_i_s_ _s_e_m_i_n_a_l_ _p_a_p_e_r - _S_y_l_v_a_i_n and _Z_a_c_h_a_r_y for the _A_c_c_e_l_e_r_a_t_e
+library, which this repository uses for distributed training - _A_l_e_x for _e_i_n_o_p_s,
+indispensable tool for tensor manipulation - _J_o_r_g_e_ _G_o_m_e_s for helping out with
+the T5 loading code and advice on the correct T5 version - _K_a_t_h_e_r_i_n_e_ _C_r_o_w_s_o_n,
+for her _b_e_a_u_t_i_f_u_l_ _c_o_d_e, which helped me understand the continuous time version
+of gaussian diffusion - _M_a_r_u_n_i_n_e and _N_e_t_r_u_k_4_4, for reviewing code, sharing
+experimental results, and help with debugging - _M_a_r_u_n_i_n_e for providing a
+_p_o_t_e_n_t_i_a_l_ _s_o_l_u_t_i_o_n for a color shifting issue in the memory efficient u-nets.
+Thanks to _J_a_c_o_b for sharing experimental comparisons between the base and
+memory-efficient unets - _M_a_r_u_n_i_n_e for finding numerous bugs, resolving an issue
+with resize right, and for sharing his experimental configurations and results
+- _M_a_l_u_m_a_D_e_v for proposing the use of pixel shuffle upsampler to fix checkboard
+artifacts - _V_a_l_e_n_t_i_n for pointing out insufficient skip connections in the
+unet, as well as the specific method of attention conditioning in the base-unet
+in the appendix - _B_I_G_J_U_N for catching a big bug with continuous time gaussian
+diffusion noise level conditioning at inference time - _B_i_n_g_b_i_n_g for identifying
+a bug with sampling and order of normalizing and noising with low resolution
+conditioning image - _K_a_y for contributing one line command training of Imagen!
+- _H_a_d_r_i_e_n_ _R_e_y_n_a_u_d for testing out text-to-video on a medical dataset, sharing
+his results, and identifying issues! ## Install ```bash $ pip install imagen-
+pytorch ``` ## Usage ```python import torch from imagen_pytorch import Unet,
+Imagen # unet for imagen unet1 = Unet( dim = 32, cond_dim = 512, dim_mults =
+(1, 2, 4, 8), num_resnet_blocks = 3, layer_attns = (False, True, True, True),
+layer_cross_attns = (False, True, True, True) ) unet2 = Unet( dim = 32,
+cond_dim = 512, dim_mults = (1, 2, 4, 8), num_resnet_blocks = (2, 4, 8, 8),
+layer_attns = (False, False, False, True), layer_cross_attns = (False, False,
+False, True) ) # imagen, which contains the unets above (base unet and super
+resoluting ones) imagen = Imagen( unets = (unet1, unet2), image_sizes = (64,
+256), timesteps = 1000, cond_drop_prob = 0.1 ).cuda() # mock images (get a lot
+of this) and text encodings from large T5 text_embeds = torch.randn(4, 256,
+768).cuda() images = torch.randn(4, 3, 256, 256).cuda() # feed images into
+imagen, training each unet in the cascade for i in (1, 2): loss = imagen
+(images, text_embeds = text_embeds, unet_number = i) loss.backward() # do the
+above for many many many many steps # now you can sample an image based on the
+text embeddings from the cascading ddpm images = imagen.sample(texts = [ 'a
+whale breaching from afar', 'young girl blowing out candles on her birthday
+cake', 'fireworks with blue and green sparkles' ], cond_scale = 3.)
+images.shape # (3, 3, 256, 256) ``` For simpler training, you can directly
+supply text strings instead of precomputing text encodings. (Although for
+scaling purposes, you will definitely want to precompute the textual embeddings
++ mask) The number of textual captions must match the batch size of the images
+if you go this route. ```python # mock images and text (get a lot of this)
+texts = [ 'a child screaming at finding a worm within a half-eaten apple',
+'lizard running across the desert on two feet', 'waking up to a psychedelic
+landscape', 'seashells sparkling in the shallow waters' ] images = torch.randn
+(4, 3, 256, 256).cuda() # feed images into imagen, training each unet in the
+cascade for i in (1, 2): loss = imagen(images, texts = texts, unet_number = i)
+loss.backward() ``` With the `ImagenTrainer` wrapper class, the exponential
+moving averages for all of the U-nets in the cascading DDPM will be
+automatically taken care of when calling `update` ```python import torch from
+imagen_pytorch import Unet, Imagen, ImagenTrainer # unet for imagen unet1 =
+Unet( dim = 32, cond_dim = 512, dim_mults = (1, 2, 4, 8), num_resnet_blocks =
+3, layer_attns = (False, True, True, True), ) unet2 = Unet( dim = 32, cond_dim
+= 512, dim_mults = (1, 2, 4, 8), num_resnet_blocks = (2, 4, 8, 8), layer_attns
+= (False, False, False, True), layer_cross_attns = (False, False, False, True)
+) # imagen, which contains the unets above (base unet and super resoluting
+ones) imagen = Imagen( unets = (unet1, unet2), text_encoder_name = 't5-large',
+image_sizes = (64, 256), timesteps = 1000, cond_drop_prob = 0.1 ).cuda() # wrap
+imagen with the trainer class trainer = ImagenTrainer(imagen) # mock images
+(get a lot of this) and text encodings from large T5 text_embeds = torch.randn
+(64, 256, 1024).cuda() images = torch.randn(64, 3, 256, 256).cuda() # feed
+images into imagen, training each unet in the cascade loss = trainer( images,
+text_embeds = text_embeds, unet_number = 1, # training on unet number 1 in this
+example, but you will have to also save checkpoints and then reload and
+continue training on unet number 2 max_batch_size = 4 # auto divide the batch
+of 64 up into batch size of 4 and accumulate gradients, so it all fits in
+memory ) trainer.update(unet_number = 1) # do the above for many many many many
+steps # now you can sample an image based on the text embeddings from the
+cascading ddpm images = trainer.sample(texts = [ 'a puppy looking anxiously at
+a giant donut on the table', 'the milky way galaxy in the style of monet' ],
+cond_scale = 3.) images.shape # (2, 3, 256, 256) ``` You can also train Imagen
+without text (unconditional image generation) as follows ```python import torch
+from imagen_pytorch import Unet, Imagen, SRUnet256, ImagenTrainer # unets for
+unconditional imagen unet1 = Unet( dim = 32, dim_mults = (1, 2, 4),
+num_resnet_blocks = 3, layer_attns = (False, True, True), layer_cross_attns =
+False, use_linear_attn = True ) unet2 = SRUnet256( dim = 32, dim_mults = (1, 2,
+4), num_resnet_blocks = (2, 4, 8), layer_attns = (False, False, True),
+layer_cross_attns = False ) # imagen, which contains the unets above (base unet
+and super resoluting ones) imagen = Imagen( condition_on_text = False, # this
+must be set to False for unconditional Imagen unets = (unet1, unet2),
+image_sizes = (64, 128), timesteps = 1000 ) trainer = ImagenTrainer
+(imagen).cuda() # now get a ton of images and feed it through the Imagen
+trainer training_images = torch.randn(4, 3, 256, 256).cuda() # train each unet
+separately # in this example, only training on unet number 1 loss = trainer
+(training_images, unet_number = 1) trainer.update(unet_number = 1) # do the
+above for many many many many steps # now you can sample images unconditionally
+from the cascading unet(s) images = trainer.sample(batch_size = 16) # (16, 3,
+128, 128) ``` Or train only super-resoluting unets ```python import torch from
+imagen_pytorch import Unet, NullUnet, Imagen # unet for imagen unet1 = NullUnet
+() # add a placeholder "null" unet for the base unet unet2 = Unet( dim = 32,
+cond_dim = 512, dim_mults = (1, 2, 4, 8), num_resnet_blocks = (2, 4, 8, 8),
+layer_attns = (False, False, False, True), layer_cross_attns = (False, False,
+False, True) ) # imagen, which contains the unets above (base unet and super
+resoluting ones) imagen = Imagen( unets = (unet1, unet2), image_sizes = (64,
+256), timesteps = 250, cond_drop_prob = 0.1 ).cuda() # mock images (get a lot
+of this) and text encodings from large T5 text_embeds = torch.randn(4, 256,
+768).cuda() images = torch.randn(4, 3, 256, 256).cuda() # feed images into
+imagen, training each unet in the cascade loss = imagen(images, text_embeds =
+text_embeds, unet_number = 2) loss.backward() # do the above for many many many
+many steps # now you can sample an image based on the text embeddings as well
+as low resolution images lowres_images = torch.randn(3, 3, 64, 64).cuda() #
+starting un-resoluted images images = imagen.sample( texts = [ 'a whale
+breaching from afar', 'young girl blowing out candles on her birthday cake',
+'fireworks with blue and green sparkles' ], start_at_unet_number = 2, # start
+at unet number 2 start_image_or_video = lowres_images, # pass in low resolution
+images to be resoluted cond_scale = 3.) images.shape # (3, 3, 256, 256) ``` At
+any time you can save and load the trainer and all associated states with the
+`save` and `load` methods. It is recommended you use these methods instead of
+manually saving with a `state_dict` call, as there are some device memory
+management being done underneath the hood within the trainer. ex. ```python
+trainer.save('./path/to/checkpoint.pt') trainer.load('./path/to/checkpoint.pt')
+trainer.steps # (2,) step number for each of the unets, in this case 2 ``` ##
+Dataloader You can also rely on the `ImagenTrainer` to automatically train off
+`DataLoader` instances. You simply have to craft your `DataLoader` to return
+either `images` (for unconditional case), or of `('images', 'text_embeds')` for
+text-guided generation. ex. unconditional training ```python from
+imagen_pytorch import Unet, Imagen, ImagenTrainer from imagen_pytorch.data
+import Dataset # unets for unconditional imagen unet = Unet( dim = 32,
+dim_mults = (1, 2, 4, 8), num_resnet_blocks = 1, layer_attns = (False, False,
+False, True), layer_cross_attns = False ) # imagen, which contains the unet
+above imagen = Imagen( condition_on_text = False, # this must be set to False
+for unconditional Imagen unets = unet, image_sizes = 128, timesteps = 1000 )
 trainer = ImagenTrainer( imagen = imagen, split_valid_from_train = True #
 whether to split the validation dataset from the training ).cuda() #
 instantiate your dataloader, which returns the necessary inputs to the DDPM as
 tuple in the order of images, text embeddings, then text masks. in this case,
 only images is returned as it is unconditional training dataset = Dataset('/
 path/to/training/images', image_size = 128) trainer.add_train_dataset(dataset,
 batch_size = 16) # working training loop for i in range(200000): loss =
@@ -145,44 +148,68 @@
 trainer.sample(batch_size = 1, return_pil_images = True) # returns List[Image]
 images[0].save(f'./sample-{i // 100}.png') ``` ## Multi GPU Thanks to _ð__¤_
 _A_c_c_e_l_e_r_a_t_e, you can do multi GPU training easily with two steps. First you need
 to invoke `accelerate config` in the same directory as your training script
 (say it is named `train.py`) ```bash $ accelerate config ``` Next, instead of
 calling `python train.py` as you would for single GPU, you would use the
 accelerate CLI as so ```bash $ accelerate launch train.py ``` That's it! ##
-Command-line To further democratize the use of this machine imagination, I have
-built in the ability to generate an image with any text prompt using one
-command line as so ex. ```bash $ imagen --model ./path/to/model/checkpoint.pt
-"a squirrel raiding the birdfeeder" # image is saved to ./
-a_squirrel_raiding_the_birdfeeder.png ``` In order to save checkpoints that can
-make use of this feature, you must instantiate your Imagen instance using the
-config classes, `ImagenConfig` and `ElucidatedImagenConfig` For proper
-training, you'll likely want to setup config-driven training anyways. ex.
-```python import torch from imagen_pytorch import ImagenConfig,
-ElucidatedImagenConfig, ImagenTrainer # in this example, using elucidated
-imagen imagen = ElucidatedImagenConfig( unets = [ dict(dim = 32, dim_mults =
-(1, 2, 4, 8)), dict(dim = 32, dim_mults = (1, 2, 4, 8)) ], image_sizes = (64,
-128), cond_drop_prob = 0.5, num_sample_steps = 32 ).create() trainer =
-ImagenTrainer(imagen) # do your training ... # then save it trainer.save('./
-checkpoint.pt') # you should see a message informing you that ./checkpoint.pt
-is commandable from the terminal ``` It really should be as simple as that You
-can also pass this checkpoint file around, and anyone can continue finetune on
-their own data ```python from imagen_pytorch import
+Command-line Imagen can also be used via CLI directly. ### Configuration ex.
+```bash $ imagen config ``` or ```bash $ imagen config --path ./configs/
+config.json ``` In the config you are able to change settings for the trainer,
+dataset and the imagen config. The Imagen config parameters can be found _h_e_r_e
+The Elucidated Imagen config parameters can be found _h_e_r_e The Imagen Trainer
+config parameters can be found _h_e_r_e For the dataset parameters all dataloader
+parameters can be used. ### Training This command allows you to train or resume
+training your model ex. ```bash $ imagen train ``` or ```bash $ imagen train --
+unet 2 --epoches 10 ``` You can pass following arguments to the training
+command. - `--config` specify the config file to use for training [default: ./
+imagen_config.json] - `--unet` the index of the unet to train [default: 1] - `-
+-epoches` how many epoches to train for [default: 50] ### Sampling Be aware
+when sampling your checkpoint should have trained all unets to get a usable
+result. ex. ```bash $ imagen sample --model ./path/to/model/checkpoint.pt "a
+squirrel raiding the birdfeeder" # image is saved to ./
+a_squirrel_raiding_the_birdfeeder.png ``` You can pass following arguments to
+the sample command. - `--model` specify the model file to use for sampling - `-
+-cond_scale` conditioning scale (classifier free guidance) in decoder - `--
+load_ema` load EMA version of unets if available In order to use a saved
+checkpoint with this feature, you either must instantiate your Imagen instance
+using the config classes, `ImagenConfig` and `ElucidatedImagenConfig` or create
+a checkpoint via the CLI directly For proper training, you'll likely want to
+setup config-driven training anyways. ex. ```python import torch from
+imagen_pytorch import ImagenConfig, ElucidatedImagenConfig, ImagenTrainer # in
+this example, using elucidated imagen imagen = ElucidatedImagenConfig( unets =
+[ dict(dim = 32, dim_mults = (1, 2, 4, 8)), dict(dim = 32, dim_mults = (1, 2,
+4, 8)) ], image_sizes = (64, 128), cond_drop_prob = 0.5, num_sample_steps = 32
+).create() trainer = ImagenTrainer(imagen) # do your training ... # then save
+it trainer.save('./checkpoint.pt') # you should see a message informing you
+that ./checkpoint.pt is commandable from the terminal ``` It really should be
+as simple as that You can also pass this checkpoint file around, and anyone can
+continue finetune on their own data ```python from imagen_pytorch import
 load_imagen_from_checkpoint, ImagenTrainer imagen = load_imagen_from_checkpoint
 ('./checkpoint.pt') trainer = ImagenTrainer(imagen) # continue training / fine-
 tuning ``` ## Inpainting Inpainting follows the formulation laid out by the
 recent _R_e_p_a_i_n_t_ _p_a_p_e_r. Simply pass in `inpaint_images` and `inpaint_masks` to
 the `sample` function on either `Imagen` or `ElucidatedImagen` ```python
 inpaint_images = torch.randn(4, 3, 512, 512).cuda() # (batch, channels, height,
 width) inpaint_masks = torch.ones((4, 512, 512)).bool().cuda() # (batch,
 height, width) inpainted_images = trainer.sample(texts = [ 'a whale breaching
 from afar', 'young girl blowing out candles on her birthday cake', 'fireworks
 with blue and green sparkles', 'dust motes swirling in the morning sunshine on
 the windowsill' ], inpaint_images = inpaint_images, inpaint_masks =
-inpaint_masks, cond_scale = 5.) inpainted_images # (4, 3, 512, 512) ``` ##
+inpaint_masks, cond_scale = 5.) inpainted_images # (4, 3, 512, 512) ``` For
+video, similarly pass in your videos to `inpaint_videos` keyword on `.sample`.
+Inpainting mask can either be the same across all frames `(batch, height,
+width)` or different `(batch, frames, height, width)` ```python inpaint_videos
+= torch.randn(4, 3, 8, 512, 512).cuda() # (batch, channels, frames, height,
+width) inpaint_masks = torch.ones((4, 8, 512, 512)).bool().cuda() # (batch,
+frames, height, width) inpainted_videos = trainer.sample(texts = [ 'a whale
+breaching from afar', 'young girl blowing out candles on her birthday cake',
+'fireworks with blue and green sparkles', 'dust motes swirling in the morning
+sunshine on the windowsill' ], inpaint_videos = inpaint_videos, inpaint_masks =
+inpaint_masks, cond_scale = 5.) inpainted_videos # (4, 3, 8, 512, 512) ``` ##
 Experimental _T_e_r_o_ _K_a_r_r_a_s of StyleGAN fame has written a _n_e_w_ _p_a_p_e_r with results
 that have been corroborated by a number of independent researchers as well as
 on my own machine. I have decided to create a version of `Imagen`, the
 `ElucidatedImagen`, so that one can use the new elucidated DDPM for text-guided
 cascading generation. Simply import `ElucidatedImagen`, and then instantiate
 the instance as you did before. The hyperparameters are different than the
 usual ones for discrete and continuous time gaussian diffusion, and can be
@@ -195,155 +222,182 @@
 @crowsonkb recommends double the max noise level for upsampler sigma_data =
 0.5, # standard deviation of data distribution rho = 7, # controls the sampling
 schedule P_mean = -1.2, # mean of log-normal distribution from which noise is
 drawn for training P_std = 1.2, # standard deviation of log-normal distribution
 from which noise is drawn for training S_churn = 80, # parameters for
 stochastic sampling - depends on dataset, Table 5 in apper S_tmin = 0.05,
 S_tmax = 50, S_noise = 1.003, ).cuda() # rest is the same as above ``` ## Text
-to Video (ongoing research) This repository will also start accumulating new
-research around text guided video synthesis. For starters it will adopt the 3d
-unet architecture described by Jonathan Ho in _V_i_d_e_o_ _D_i_f_f_u_s_i_o_n_ _M_o_d_e_l_s Ex.
-```python import torch from imagen_pytorch import Unet3D, ElucidatedImagen,
-ImagenTrainer unet1 = Unet3D(dim = 64, dim_mults = (1, 2, 4, 8)).cuda() unet2 =
-Unet3D(dim = 64, dim_mults = (1, 2, 4, 8)).cuda() # elucidated imagen, which
-contains the unets above (base unet and super resoluting ones) imagen =
-ElucidatedImagen( unets = (unet1, unet2), image_sizes = (16, 32),
-random_crop_sizes = (None, 16), num_sample_steps = 10, cond_drop_prob = 0.1,
-sigma_min = 0.002, # min noise level sigma_max = (80, 160), # max noise level,
-double the max noise level for upsampler sigma_data = 0.5, # standard deviation
-of data distribution rho = 7, # controls the sampling schedule P_mean = -1.2, #
-mean of log-normal distribution from which noise is drawn for training P_std =
-1.2, # standard deviation of log-normal distribution from which noise is drawn
-for training S_churn = 80, # parameters for stochastic sampling - depends on
+to Video This repository will also start accumulating new research around text
+guided video synthesis. For starters it will adopt the 3d unet architecture
+described by Jonathan Ho in _V_i_d_e_o_ _D_i_f_f_u_s_i_o_n_ _M_o_d_e_l_s Update: verified _w_o_r_k_i_n_g by
+_H_a_d_r_i_e_n_ _R_e_y_n_a_u_d! Ex. ```python import torch from imagen_pytorch import Unet3D,
+ElucidatedImagen, ImagenTrainer unet1 = Unet3D(dim = 64, dim_mults = (1, 2, 4,
+8)).cuda() unet2 = Unet3D(dim = 64, dim_mults = (1, 2, 4, 8)).cuda() #
+elucidated imagen, which contains the unets above (base unet and super
+resoluting ones) imagen = ElucidatedImagen( unets = (unet1, unet2), image_sizes
+= (16, 32), random_crop_sizes = (None, 16), temporal_downsample_factor = (2,
+1), # in this example, the first unet would receive the video temporally
+downsampled by 2x num_sample_steps = 10, cond_drop_prob = 0.1, sigma_min =
+0.002, # min noise level sigma_max = (80, 160), # max noise level, double the
+max noise level for upsampler sigma_data = 0.5, # standard deviation of data
+distribution rho = 7, # controls the sampling schedule P_mean = -1.2, # mean of
+log-normal distribution from which noise is drawn for training P_std = 1.2, #
+standard deviation of log-normal distribution from which noise is drawn for
+training S_churn = 80, # parameters for stochastic sampling - depends on
 dataset, Table 5 in apper S_tmin = 0.05, S_tmax = 50, S_noise = 1.003, ).cuda()
 # mock videos (get a lot of this) and text encodings from large T5 texts = [ 'a
 whale breaching from afar', 'young girl blowing out candles on her birthday
 cake', 'fireworks with blue and green sparkles', 'dust motes swirling in the
 morning sunshine on the windowsill' ] videos = torch.randn(4, 3, 10, 32,
 32).cuda() # (batch, channels, time / video frames, height, width) # feed
 images into imagen, training each unet in the cascade # for this example, only
-training unet 1 trainer = ImagenTrainer(imagen) trainer(videos, texts = texts,
-unet_number = 1) trainer.update(unet_number = 1) videos = trainer.sample(texts
-= texts, video_frames = 20) # extrapolating to 20 frames from training on 10
-frames videos.shape # (4, 3, 20, 32, 32) ``` ## FAQ - Why are my generated
-images not aligning well with the text? Imagen uses an algorithm called
-_C_l_a_s_s_i_f_i_e_r_ _F_r_e_e_ _G_u_i_d_a_n_c_e. When sampling, you apply a scale to the conditioning
-(text in this case) of greater than `1.0`. Researcher _N_e_t_r_u_k_4_4 have reported
-`5-10` to be optimal, but anything greater than `10` to break. ```python
-trainer.sample(texts = [ 'a cloud in the shape of a roman gladiator' ],
-cond_scale = 5.) # <-- cond_scale is the conditioning scale, needs to be
-greater than 1.0 to be better than average ``` - Are there any pretrained
-models yet? Not at the moment but one will likely be trained and open sourced
-within the year, if not sooner. If you would like to participate, you can join
-the community of artificial neural network trainers at Laion (discord link is
-in the Readme above) and start collaborating. - Will this technology take my
-job? More the reason why you should start training your own model, starting
-today! The last thing we need is this technology being in the hands of an elite
-few. Hopefully this repository reduces the work to just finding the necessary
-compute, and augmenting with your own curated dataset. - What am I allowed to
-do with this repository? Anything! It is MIT licensed. In other words, you can
-freely copy / paste for your own research, remixed for whatever modality you
-can think of. Go train amazing models for profit, for science, or simply to
-satiate your own personal pleasure at witnessing something divine unravel in
-front of you. ## Related Works - _A_u_d_i_o_ _d_i_f_f_u_s_i_o_n from _F_l_a_v_i_o_ _S_c_h_n_e_i_d_e_r - _M_i_n_i
-_I_m_a_g_e_n from _R_y_a_n_ _O_. | _A_s_s_e_m_b_l_y_A_I_ _w_r_i_t_e_u_p ## Todo - [x] use huggingface
-transformers for T5-small text embeddings - [x] add dynamic thresholding - [x]
-add dynamic thresholding DALLE2 and video-diffusion repository as well - [x]
-allow for one to set T5-large (and perhaps small factory method to take in any
-huggingface transformer) - [x] add the lowres noise level with the pseudocode
-in appendix, and figure out what is this sweep they do at inference time - [x]
-port over some training code from DALLE2 - [x] need to be able to use a
-different noise schedule per unet (cosine was used for base, but linear for SR)
-- [x] just make one master-configurable unet - [x] complete resnet block
-(biggan inspired? but with groupnorm) - complete self attention - [x] complete
-conditioning embedding block (and make it completely configurable, whether it
-be attention, film etc) - [x] consider using perceiver-resampler from https://
-github.com/lucidrains/flamingo-pytorch in place of attention pooling - [x] add
-attention pooling option, in addition to cross attention and film - [x] add
-optional cosine decay schedule with warmup, for each unet, to trainer - [x]
-switch to continuous timesteps instead of discretized, as it seems that is what
-they used for all stages - first figure out the linear noise schedule case from
-the variational ddpm paper https://openreview.net/forum?id=2LdBqxc1Yv - [x]
-figure out log(snr) for alpha cosine noise schedule. - [x] suppress the
-transformers warning because only T5encoder is used - [x] allow setting for
-using linear attention on layers where full attention cannot be used - [x]
-force unets in continuous time case to use non-fouriered conditions (just pass
-the log(snr) through an MLP with optional layernorms), as that is what i have
-working locally - [x] removed learned variance - [x] add p2 loss weighting for
-continuous time - [x] make sure cascading ddpm can be trained without text
-condition, and make sure both continuous and discrete time gaussian diffusion
-works - [x] use primer's depthwise convs on the qkv projections in linear
-attention (or use token shifting before projections) - also use new dropout
-proposed by bayesformer, as it seems to work well with linear attention - [x]
-explore skip layer excitation in unet decoder - [x] accelerate integration -
-[x] build out CLI tool and one-line generation of image - [x] knock out any
-issues that arised from accelerate - [x] add inpainting ability using resampler
-from repaint paper https://arxiv.org/abs/2201.09865 - [x] build a simple
-checkpointing system, backed by a folder - [x] add skip connection from outputs
-of all upsample blocks, used in unet squared paper and some previous unet works
-- [x] add fsspec, recommended by Romain @rom1504, for cloud / local file system
-agnostic persistence of checkpoints - [x] test out persistence in gcs with
-https://github.com/fsspec/gcsfs - [x] extend to video generation, using axial
-time attention as in Ho's video ddpm paper - [x] allow elucidated imagen to
-generalize to any shape - [x] allow for imagen to generalize to any shape - [x]
-add _d_y_n_a_m_i_c_ _p_o_s_i_t_i_o_n_a_l_ _b_i_a_s for the best type of length extrapolation across
-video time - [x] move video frames to sample function, as we will be attempting
-time extrapolation - [x] attention bias to null key / values should be a
-learned scalar of head dimension - [x] add self-conditioning from _b_i_t_ _d_i_f_f_u_s_i_o_n
-paper, already coded up at _d_d_p_m_-_p_y_t_o_r_c_h - [ ] reread _c_o_g_v_i_d_e_o and figure out
-how frame rate conditioning could be used - [ ] bring in attention expertise
-for self attention layers in unet3d - [ ] consider bringing in NUWA's 3d
+training unet 1 trainer = ImagenTrainer(imagen) # you can also ignore time when
+training on video initially, shown to improve results in video-ddpm paper.
+eventually will make the 3d unet trainable with either images or video.
+research shows it is essential (with current data regimes) to train first on
+text-to-image. probably won't be true in another decade. all big data becomes
+small data trainer(videos, texts = texts, unet_number = 1, ignore_time = False)
+trainer.update(unet_number = 1) videos = trainer.sample(texts = texts,
+video_frames = 20) # extrapolating to 20 frames from training on 10 frames
+videos.shape # (4, 3, 20, 32, 32) ``` You can also train on text - image pairs
+first. The `Unet3D` will automatically convert it to single framed videos and
+learn without the temporal components (by automatically setting `ignore_time =
+True`), whether it be 1d convolutions or causal attention across time. This is
+the current approach taken by all the big artificial intelligence labs (Brain,
+MetaAI, Bytedance) ## FAQ - Why are my generated images not aligning well with
+the text? Imagen uses an algorithm called _C_l_a_s_s_i_f_i_e_r_ _F_r_e_e_ _G_u_i_d_a_n_c_e. When
+sampling, you apply a scale to the conditioning (text in this case) of greater
+than `1.0`. Researcher _N_e_t_r_u_k_4_4 have reported `5-10` to be optimal, but
+anything greater than `10` to break. ```python trainer.sample(texts = [ 'a
+cloud in the shape of a roman gladiator' ], cond_scale = 5.) # <-- cond_scale
+is the conditioning scale, needs to be greater than 1.0 to be better than
+average ``` - Are there any pretrained models yet? Not at the moment but one
+will likely be trained and open sourced within the year, if not sooner. If you
+would like to participate, you can join the community of artificial neural
+network trainers at Laion (discord link is in the Readme above) and start
+collaborating. - Will this technology take my job? More the reason why you
+should start training your own model, starting today! The last thing we need is
+this technology being in the hands of an elite few. Hopefully this repository
+reduces the work to just finding the necessary compute, and augmenting with
+your own curated dataset. - What am I allowed to do with this repository?
+Anything! It is MIT licensed. In other words, you can freely copy / paste for
+your own research, remixed for whatever modality you can think of. Go train
+amazing models for profit, for science, or simply to satiate your own personal
+pleasure at witnessing something divine unravel in front of you. ## Cool
+Applications! - _E_c_h_o_c_a_r_d_i_o_g_r_a_m_ _s_y_n_t_h_e_s_i_s _[_C_o_d_e_] - _S_O_T_A_ _H_i_-_C_ _c_o_n_t_a_c_t_ _m_a_t_r_i_x
+_s_y_n_t_h_e_s_i_s _[_C_o_d_e_] - _F_l_o_o_r_ _p_l_a_n_ _g_e_n_e_r_a_t_i_o_n - _U_l_t_r_a_ _H_i_g_h_ _R_e_s_o_l_u_t_i_o_n_ _H_i_s_t_o_p_a_t_h_o_l_o_g_y
+_S_l_i_d_e_s - _S_y_n_t_h_e_t_i_c_ _L_a_p_a_r_o_s_c_o_p_i_c_ _I_m_a_g_e_s - _D_e_s_i_g_n_i_n_g_ _M_e_t_a_M_a_t_e_r_i_a_l_s ## Related
+Works - _A_u_d_i_o_ _d_i_f_f_u_s_i_o_n from _F_l_a_v_i_o_ _S_c_h_n_e_i_d_e_r - _M_i_n_i_ _I_m_a_g_e_n from _R_y_a_n_ _O_. |
+_A_s_s_e_m_b_l_y_A_I_ _w_r_i_t_e_u_p ## Todo - [x] use huggingface transformers for T5-small text
+embeddings - [x] add dynamic thresholding - [x] add dynamic thresholding DALLE2
+and video-diffusion repository as well - [x] allow for one to set T5-large (and
+perhaps small factory method to take in any huggingface transformer) - [x] add
+the lowres noise level with the pseudocode in appendix, and figure out what is
+this sweep they do at inference time - [x] port over some training code from
+DALLE2 - [x] need to be able to use a different noise schedule per unet (cosine
+was used for base, but linear for SR) - [x] just make one master-configurable
+unet - [x] complete resnet block (biggan inspired? but with groupnorm) -
+complete self attention - [x] complete conditioning embedding block (and make
+it completely configurable, whether it be attention, film etc) - [x] consider
+using perceiver-resampler from https://github.com/lucidrains/flamingo-pytorch
+in place of attention pooling - [x] add attention pooling option, in addition
+to cross attention and film - [x] add optional cosine decay schedule with
+warmup, for each unet, to trainer - [x] switch to continuous timesteps instead
+of discretized, as it seems that is what they used for all stages - first
+figure out the linear noise schedule case from the variational ddpm paper
+https://openreview.net/forum?id=2LdBqxc1Yv - [x] figure out log(snr) for alpha
+cosine noise schedule. - [x] suppress the transformers warning because only
+T5encoder is used - [x] allow setting for using linear attention on layers
+where full attention cannot be used - [x] force unets in continuous time case
+to use non-fouriered conditions (just pass the log(snr) through an MLP with
+optional layernorms), as that is what i have working locally - [x] removed
+learned variance - [x] add p2 loss weighting for continuous time - [x] make
+sure cascading ddpm can be trained without text condition, and make sure both
+continuous and discrete time gaussian diffusion works - [x] use primer's
+depthwise convs on the qkv projections in linear attention (or use token
+shifting before projections) - also use new dropout proposed by bayesformer, as
+it seems to work well with linear attention - [x] explore skip layer excitation
+in unet decoder - [x] accelerate integration - [x] build out CLI tool and one-
+line generation of image - [x] knock out any issues that arised from accelerate
+- [x] add inpainting ability using resampler from repaint paper https://
+arxiv.org/abs/2201.09865 - [x] build a simple checkpointing system, backed by a
+folder - [x] add skip connection from outputs of all upsample blocks, used in
+unet squared paper and some previous unet works - [x] add fsspec, recommended
+by Romain @rom1504, for cloud / local file system agnostic persistence of
+checkpoints - [x] test out persistence in gcs with https://github.com/fsspec/
+gcsfs - [x] extend to video generation, using axial time attention as in Ho's
+video ddpm paper - [x] allow elucidated imagen to generalize to any shape - [x]
+allow for imagen to generalize to any shape - [x] add _d_y_n_a_m_i_c_ _p_o_s_i_t_i_o_n_a_l_ _b_i_a_s
+for the best type of length extrapolation across video time - [x] move video
+frames to sample function, as we will be attempting time extrapolation - [x]
+attention bias to null key / values should be a learned scalar of head
+dimension - [x] add self-conditioning from _b_i_t_ _d_i_f_f_u_s_i_o_n paper, already coded
+up at _d_d_p_m_-_p_y_t_o_r_c_h - [x] add v-parameterization (https://arxiv.org/abs/
+2202.00512) from _i_m_a_g_e_n_ _v_i_d_e_o paper, the only thing new - [x] incorporate all
+learnings from make-a-video (https://makeavideo.studio/) - [x] build out CLI
+tool for training, resuming training off config file - [x] allow for temporal
+interpolation at specific stages - [x] make sure temporal interpolation works
+with inpainting - [x] make sure one can customize all interpolation modes (some
+researchers are finding better results with trilinear) - [x] imagen-video :
+allow for conditioning on preceding (and possibly future) frames of videos.
+ignore time should not be allowed in that scenario - [x] make sure to
+automatically take care of temporal down/upsampling for conditioning video
+frames, but allow for an option to turn it off - [x] make sure inpainting works
+with video - [x] make sure inpainting mask for video can accept be customized
+per frame - [ ] add flash attention - [ ] reread _c_o_g_v_i_d_e_o and figure out how
+frame rate conditioning could be used - [ ] bring in attention expertise for
+self attention layers in unet3d - [ ] consider bringing in NUWA's 3d
 convolutional attention - [ ] consider transformer-xl memories in the temporal
 attention blocks - [ ] consider _p_e_r_c_e_i_v_e_r_-_a_r_ _a_p_p_r_o_a_c_h to attending to past time
 - [ ] frame dropouts during attention for achieving both regularizing effect as
 well as shortened training time - [ ] investigate frank wood's claims https://
 github.com/lucidrains/flexible-diffusion-modeling-videos-pytorch and either add
 the hierarchical sampling technique, or let people know about its deficiencies
-- [ ] make sure inpainting works with video - [ ] offer challenging moving
-mnist (with distractor objects) as a one-line trainable baseline for
-researchers to branch off of for text to video - [ ] build out CLI tool for
-training, resuming training off config file - [ ] preencoding of text to
-memmapped embeddings - [ ] be able to create dataloader iterators based on the
-old epoch style, also configure shuffling etc - [ ] be able to also pass in
-arguments (instead of requiring forward to be all keyword args on model) - [ ]
-bring in reversible blocks from revnets for 3d unet, to lessen memory burden -
-[ ] add ability to only train super-resolution network - [ ] read _d_p_m_-_s_o_l_v_e_r
-see if it is applicable to continuous time gaussian diffusion - [ ] allow for
-conditioning video frames with arbitrary absolute times (calculate RPE during
-temporal attention) ## Citations ```bibtex @inproceedings
-{Saharia2022PhotorealisticTD, title = {Photorealistic Text-to-Image Diffusion
-Models with Deep Language Understanding}, author = {Chitwan Saharia and William
-Chan and Saurabh Saxena and Lala Li and Jay Whang and Emily L. Denton and Seyed
-Kamyar Seyed Ghasemipour and Burcu Karagol Ayan and Seyedeh Sara Mahdavi and
-Raphael Gontijo Lopes and Tim Salimans and Jonathan Ho and David Fleet and
-Mohammad Norouzi}, year = {2022} } ``` ```bibtex @article{Alayrac2022Flamingo,
-title = {Flamingo: a Visual Language Model for Few-Shot Learning}, author =
-{Jean-Baptiste Alayrac et al}, year = {2022} } ``` ```bibtex @article
-{Choi2022PerceptionPT, title = {Perception Prioritized Training of Diffusion
-Models}, author = {Jooyoung Choi and Jungbeom Lee and Chaehun Shin and Sungwon
-Kim and Hyunwoo J. Kim and Sung-Hoon Yoon}, journal = {ArXiv}, year = {2022},
-volume = {abs/2204.00227} } ``` ```bibtex @inproceedings
-{Sankararaman2022BayesFormerTW, title = {BayesFormer: Transformer with
-Uncertainty Estimation}, author = {Karthik Abinav Sankararaman and Sinong Wang
-and Han Fang}, year = {2022} } ``` ```bibtex @article{So2021PrimerSF, title =
-{Primer: Searching for Efficient Transformers for Language Modeling}, author =
-{David R. So and Wojciech Ma'nke and Hanxiao Liu and Zihang Dai and Noam M.
-Shazeer and Quoc V. Le}, journal = {ArXiv}, year = {2021}, volume = {abs/
-2109.08668} } ``` ```bibtex @misc{cao2020global, title = {Global Context
-Networks}, author = {Yue Cao and Jiarui Xu and Stephen Lin and Fangyun Wei and
-Han Hu}, year = {2020}, eprint = {2012.13375}, archivePrefix = {arXiv},
-primaryClass = {cs.CV} } ``` ```bibtex @article{Karras2022ElucidatingTD, title
-= {Elucidating the Design Space of Diffusion-Based Generative Models}, author =
-{Tero Karras and Miika Aittala and Timo Aila and Samuli Laine}, journal =
-{ArXiv}, year = {2022}, volume = {abs/2206.00364} } ``` ```bibtex
-@inproceedings{NEURIPS2020_4c5bcfec, author = {Ho, Jonathan and Jain, Ajay and
-Abbeel, Pieter}, booktitle = {Advances in Neural Information Processing
-Systems}, editor = {H. Larochelle and M. Ranzato and R. Hadsell and M.F. Balcan
-and H. Lin}, pages = {6840--6851}, publisher = {Curran Associates, Inc.}, title
-= {Denoising Diffusion Probabilistic Models}, url = {https://
+- [ ] offer challenging moving mnist (with distractor objects) as a one-line
+trainable baseline for researchers to branch off of for text to video - [ ]
+preencoding of text to memmapped embeddings - [ ] be able to create dataloader
+iterators based on the old epoch style, also configure shuffling etc - [ ] be
+able to also pass in arguments (instead of requiring forward to be all keyword
+args on model) - [ ] bring in reversible blocks from revnets for 3d unet, to
+lessen memory burden - [ ] add ability to only train super-resolution network -
+[ ] read _d_p_m_-_s_o_l_v_e_r see if it is applicable to continuous time gaussian
+diffusion - [ ] allow for conditioning video frames with arbitrary absolute
+times (calculate RPE during temporal attention) - [ ] accommodate _d_r_e_a_m_ _b_o_o_t_h
+fine tuning - [ ] add textual inversion - [ ] cleanup self conditioning to be
+extracted at imagen instantiation - [ ] make sure eventual dreambooth works
+with imagen-video - [ ] add framerate conditioning for video diffusion - [ ]
+make sure one can simulataneously condition on video frames as a prompt, as
+well as some conditioning image across all frames - [ ] test and add
+distillation technique from _c_o_n_s_i_s_t_e_n_c_y_ _m_o_d_e_l_s ## Citations ```bibtex
+@inproceedings{Saharia2022PhotorealisticTD, title = {Photorealistic Text-to-
+Image Diffusion Models with Deep Language Understanding}, author = {Chitwan
+Saharia and William Chan and Saurabh Saxena and Lala Li and Jay Whang and Emily
+L. Denton and Seyed Kamyar Seyed Ghasemipour and Burcu Karagol Ayan and Seyedeh
+Sara Mahdavi and Raphael Gontijo Lopes and Tim Salimans and Jonathan Ho and
+David Fleet and Mohammad Norouzi}, year = {2022} } ``` ```bibtex @article
+{Alayrac2022Flamingo, title = {Flamingo: a Visual Language Model for Few-Shot
+Learning}, author = {Jean-Baptiste Alayrac et al}, year = {2022} } ```
+```bibtex @inproceedings{Sankararaman2022BayesFormerTW, title = {BayesFormer:
+Transformer with Uncertainty Estimation}, author = {Karthik Abinav Sankararaman
+and Sinong Wang and Han Fang}, year = {2022} } ``` ```bibtex @article
+{So2021PrimerSF, title = {Primer: Searching for Efficient Transformers for
+Language Modeling}, author = {David R. So and Wojciech Ma'nke and Hanxiao Liu
+and Zihang Dai and Noam M. Shazeer and Quoc V. Le}, journal = {ArXiv}, year =
+{2021}, volume = {abs/2109.08668} } ``` ```bibtex @misc{cao2020global, title =
+{Global Context Networks}, author = {Yue Cao and Jiarui Xu and Stephen Lin and
+Fangyun Wei and Han Hu}, year = {2020}, eprint = {2012.13375}, archivePrefix =
+{arXiv}, primaryClass = {cs.CV} } ``` ```bibtex @article
+{Karras2022ElucidatingTD, title = {Elucidating the Design Space of Diffusion-
+Based Generative Models}, author = {Tero Karras and Miika Aittala and Timo Aila
+and Samuli Laine}, journal = {ArXiv}, year = {2022}, volume = {abs/2206.00364}
+} ``` ```bibtex @inproceedings{NEURIPS2020_4c5bcfec, author = {Ho, Jonathan and
+Jain, Ajay and Abbeel, Pieter}, booktitle = {Advances in Neural Information
+Processing Systems}, editor = {H. Larochelle and M. Ranzato and R. Hadsell and
+M.F. Balcan and H. Lin}, pages = {6840--6851}, publisher = {Curran Associates,
+Inc.}, title = {Denoising Diffusion Probabilistic Models}, url = {https://
 proceedings.neurips.cc/paper/2020/file/4c5bcfec8584af0d967f1ab10179ca4b-
 Paper.pdf}, volume = {33}, year = {2020} } ``` ```bibtex @article
 {Lugmayr2022RePaintIU, title = {RePaint: Inpainting using Denoising Diffusion
 Probabilistic Models}, author = {Andreas Lugmayr and Martin Danelljan and Andr
 {\'e}s Romero and Fisher Yu and Radu Timofte and Luc Van Gool}, journal =
 {ArXiv}, year = {2022}, volume = {abs/2201.09865} } ``` ```bibtex @misc
 {ho2022video, title = {Video Diffusion Models}, author = {Jonathan Ho and Tim
@@ -353,7 +407,36 @@
 title = {Einops: Clear and Reliable Tensor Manipulations with Einstein-like
 Notation}, author = {Alex Rogozhnikov}, booktitle = {International Conference
 on Learning Representations}, year = {2022}, url = {https://openreview.net/
 forum?id=oapKSVM2bcj} } ``` ```bibtex @misc{chen2022analog, title = {Analog
 Bits: Generating Discrete Data using Diffusion Models with Self-Conditioning},
 author = {Ting Chen and Ruixiang Zhang and Geoffrey Hinton}, year = {2022},
 eprint = {2208.04202}, archivePrefix = {arXiv}, primaryClass = {cs.CV} } ```
+```bibtex @misc{Singer2022, author = {Uriel Singer}, url = {https://
+makeavideo.studio/Make-A-Video.pdf} } ``` ```bibtex @article{Sunkara2022NoMS,
+title = {No More Strided Convolutions or Pooling: A New CNN Building Block for
+Low-Resolution Images and Small Objects}, author = {Raja Sunkara and Tie Luo},
+journal = {ArXiv}, year = {2022}, volume = {abs/2208.03641} } ``` ```bibtex
+@article{Salimans2022ProgressiveDF, title = {Progressive Distillation for Fast
+Sampling of Diffusion Models}, author = {Tim Salimans and Jonathan Ho}, journal
+= {ArXiv}, year = {2022}, volume = {abs/2202.00512} } ``` ```bibtex @article
+{Ho2022ImagenVH, title = {Imagen Video: High Definition Video Generation with
+Diffusion Models}, author = {Jonathan Ho and William Chan and Chitwan Saharia
+and Jay Whang and Ruiqi Gao and Alexey A. Gritsenko and Diederik P. Kingma and
+Ben Poole and Mohammad Norouzi and David J. Fleet and Tim Salimans}, journal =
+{ArXiv}, year = {2022}, volume = {abs/2210.02303} } ``` ```bibtex @misc
+{gilmer2023intriguing title = {Intriguing Properties of Transformer Training
+Instabilities}, author = {Justin Gilmer, Andrea Schioppa, and Jeremy Cohen},
+year = {2023}, status = {to be published - one attention stabilization
+technique is circulating within Google Brain, being used by multiple teams} }
+``` ```bibtex @inproceedings{Hang2023EfficientDT, title = {Efficient Diffusion
+Training via Min-SNR Weighting Strategy}, author = {Tiankai Hang and Shuyang Gu
+and Chen Li and Jianmin Bao and Dong Chen and Han Hu and Xin Geng and Baining
+Guo}, year = {2023} } ``` ```bibtex @article{Zhang2021TokenST, title = {Token
+Shift Transformer for Video Classification}, author = {Hao Zhang and Y. Hao and
+Chong-Wah Ngo}, journal = {Proceedings of the 29th ACM International Conference
+on Multimedia}, year = {2021} } ``` ```bibtex @inproceedings
+{anonymous2022normformer, title = {NormFormer: Improved Transformer Pretraining
+with Extra Normalization}, author = {Anonymous}, booktitle = {Submitted to The
+Tenth International Conference on Learning Representations }, year = {2022},
+url = {https://openreview.net/forum?id=GMYWzWztDx5}, note = {under review} }
+```
```

### Comparing `imagen-pytorch-1.9.7/imagen_pytorch/__init__.py` & `imagen_pytorch-2.0.0/imagen_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `imagen-pytorch-1.9.7/imagen_pytorch/configs.py` & `imagen_pytorch-2.0.0/imagen_pytorch/configs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-import json
-from pydantic import BaseModel, validator, root_validator
-from typing import List, Iterable, Optional, Union, Tuple, Dict, Any
+from pydantic import BaseModel, model_validator
+from typing import List, Optional, Union, Tuple
 from enum import Enum
 
 from imagen_pytorch.imagen_pytorch import Imagen, Unet, Unet3D, NullUnet
 from imagen_pytorch.trainer import ImagenTrainer
 from imagen_pytorch.elucidated_imagen import ElucidatedImagen
 from imagen_pytorch.t5 import DEFAULT_T5_NAME, get_encoded_dim
 
@@ -41,27 +40,27 @@
     def create(self):
         return NullUnet()
 
 class UnetConfig(AllowExtraBaseModel):
     dim:                int
     dim_mults:          ListOrTuple(int)
     text_embed_dim:     int = get_encoded_dim(DEFAULT_T5_NAME)
-    cond_dim:           int = None
+    cond_dim:           Optional[int] = None
     channels:           int = 3
     attn_dim_head:      int = 32
     attn_heads:         int = 16
 
     def create(self):
         return Unet(**self.dict())
 
 class Unet3DConfig(AllowExtraBaseModel):
     dim:                int
     dim_mults:          ListOrTuple(int)
     text_embed_dim:     int = get_encoded_dim(DEFAULT_T5_NAME)
-    cond_dim:           int = None
+    cond_dim:           Optional[int] = None
     channels:           int = 3
     attn_dim_head:      int = 32
     attn_heads:         int = 16
 
     def create(self):
         return Unet3D(**self.dict())
 
@@ -72,20 +71,19 @@
     timesteps:              SingleOrList(int) = 1000
     noise_schedules:        SingleOrList(NoiseSchedule) = 'cosine'
     text_encoder_name:      str = DEFAULT_T5_NAME
     channels:               int = 3
     loss_type:              str = 'l2'
     cond_drop_prob:         float = 0.5
 
-    @validator('image_sizes')
-    def check_image_sizes(cls, image_sizes, values):
-        unets = values.get('unets')
-        if len(image_sizes) != len(unets):
-            raise ValueError(f'image sizes length {len(image_sizes)} must be equivalent to the number of unets {len(unets)}')
-        return image_sizes
+    @model_validator(mode="after")
+    def check_image_sizes(self):
+        if len(self.image_sizes) != len(self.unets):
+            raise ValueError(f'image sizes length {len(self.image_sizes)} must be equivalent to the number of unets {len(self.unets)}')
+        return self
 
     def create(self):
         decoder_kwargs = self.dict()
         unets_kwargs = decoder_kwargs.pop('unets')
         is_video = decoder_kwargs.pop('video', False)
 
         unets = []
@@ -120,20 +118,19 @@
     P_mean:                 SingleOrList(float) = -1.2
     P_std:                  SingleOrList(float) = 1.2
     S_churn:                SingleOrList(int) = 80
     S_tmin:                 SingleOrList(float) = 0.05
     S_tmax:                 SingleOrList(int) = 50
     S_noise:                SingleOrList(float) = 1.003
 
-    @validator('image_sizes')
-    def check_image_sizes(cls, image_sizes, values):
-        unets = values.get('unets')
-        if len(image_sizes) != len(unets):
-            raise ValueError(f'image sizes length {len(image_sizes)} must be equivalent to the number of unets {len(unets)}')
-        return image_sizes
+    @model_validator(mode="after")
+    def check_image_sizes(self):
+        if len(self.image_sizes) != len(self.unets):
+            raise ValueError(f'image sizes length {len(self.image_sizes)} must be equivalent to the number of unets {len(self.unets)}')
+        return self
 
     def create(self):
         decoder_kwargs = self.dict()
         unets_kwargs = decoder_kwargs.pop('unets')
         is_video = decoder_kwargs.pop('video', False)
 
         unet_klass = Unet3D if is_video else Unet
```

### Comparing `imagen-pytorch-1.9.7/imagen_pytorch/elucidated_imagen.py` & `imagen_pytorch-2.0.0/imagen_pytorch/elucidated_imagen.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,50 +1,54 @@
 from math import sqrt
 from random import random
 from functools import partial
 from contextlib import contextmanager, nullcontext
 from typing import List, Union
 from collections import namedtuple
-from tqdm import tqdm
+from tqdm.auto import tqdm
 
 import torch
 import torch.nn.functional as F
-from torch import nn, einsum
+from torch import nn
 from torch.cuda.amp import autocast
+from torch.nn.parallel import DistributedDataParallel
 import torchvision.transforms as T
 
 import kornia.augmentation as K
 
 from einops import rearrange, repeat, reduce
-from einops_exts import rearrange_many
 
 from imagen_pytorch.imagen_pytorch import (
     GaussianDiffusionContinuousTimes,
     Unet,
     NullUnet,
     first,
     exists,
     identity,
     maybe,
     default,
     cast_tuple,
     cast_uint8_images_to_float,
     eval_decorator,
-    check_shape,
     pad_tuple_to_length,
     resize_image_to,
+    calc_all_frame_dims,
+    safe_get_tuple_index,
     right_pad_dims_to,
     module_device,
     normalize_neg_one_to_one,
     unnormalize_zero_to_one,
+    compact,
+    maybe_transform_dict_key
 )
 
-from imagen_pytorch.imagen_video.imagen_video import (
+from imagen_pytorch.imagen_video import (
     Unet3D,
-    resize_video_to
+    resize_video_to,
+    scale_video_time
 )
 
 from imagen_pytorch.t5 import t5_encode_text, get_encoded_dim, DEFAULT_T5_NAME
 
 # constants
 
 Hparams_fields = [
@@ -77,14 +81,17 @@
         *,
         image_sizes,                                # for cascading ddpm, image size at each stage
         text_encoder_name = DEFAULT_T5_NAME,
         text_embed_dim = None,
         channels = 3,
         cond_drop_prob = 0.1,
         random_crop_sizes = None,
+        resize_mode = 'nearest',
+        temporal_downsample_factor = 1,
+        resize_cond_video_frames = True,
         lowres_sample_noise_level = 0.2,            # in the paper, they present a new trick where they noise the lowres conditioning image, and at sample time, fix it to a certain level (0.1 or 0.3) - the unets are also made to be conditioned on this noise level
         per_sample_random_aug_noise_level = False,  # unclear when conditioning on augmentation noise level, whether each batch element receives a random aug noise value - turning off due to @marunine's find
         condition_on_text = True,
         auto_normalize_img = True,                  # whether to take care of normalizing the image from [0, 1] to [-1, 1] and back automatically - you can turn this off if you want to pass in the [-1, 1] ranged image yourself from the dataloader
         dynamic_thresholding = True,
         dynamic_thresholding_percentile = 0.95,     # unsure what this was based on perusal of paper
         only_train_unet_number = None,
@@ -157,20 +164,22 @@
 
         # determine whether we are training on images or video
 
         is_video = any([isinstance(unet, Unet3D) for unet in self.unets])
         self.is_video = is_video
 
         self.right_pad_dims_to_datatype = partial(rearrange, pattern = ('b -> b 1 1 1' if not is_video else 'b -> b 1 1 1 1'))
+
         self.resize_to = resize_video_to if is_video else resize_image_to
+        self.resize_to = partial(self.resize_to, mode = resize_mode)
 
         # unet image sizes
 
         self.image_sizes = cast_tuple(image_sizes)
-        assert num_unets == len(image_sizes), f'you did not supply the correct number of u-nets ({len(self.unets)}) for resolutions {image_sizes}'
+        assert num_unets == len(self.image_sizes), f'you did not supply the correct number of u-nets ({len(self.unets)}) for resolutions {self.image_sizes}'
 
         self.sample_channels = cast_tuple(self.channels, num_unets)
 
         # cascading ddpm related stuff
 
         lowres_conditions = tuple(map(lambda t: t.lowres_cond, self.unets))
         assert lowres_conditions == (False, *((True,) * (num_unets - 1))), 'the first unet must be unconditioned (by low resolution image), and the rest of the unets must have `lowres_cond` set to True'
@@ -190,14 +199,25 @@
         self.input_image_range = (0. if auto_normalize_img else -1., 1.)
 
         # dynamic thresholding
 
         self.dynamic_thresholding = cast_tuple(dynamic_thresholding, num_unets)
         self.dynamic_thresholding_percentile = dynamic_thresholding_percentile
 
+        # temporal interpolations
+
+        temporal_downsample_factor = cast_tuple(temporal_downsample_factor, num_unets)
+        self.temporal_downsample_factor = temporal_downsample_factor
+
+        self.resize_cond_video_frames = resize_cond_video_frames
+        self.temporal_downsample_divisor = temporal_downsample_factor[0]
+
+        assert temporal_downsample_factor[-1] == 1, 'downsample factor of last stage must be 1'
+        assert tuple(sorted(temporal_downsample_factor, reverse = True)) == temporal_downsample_factor, 'temporal downsample factor must be in order of descending'
+
         # elucidating parameters
 
         hparams = [
             num_sample_steps,
             sigma_min,
             sigma_max,
             sigma_data,
@@ -217,14 +237,21 @@
 
         self.register_buffer('_temp', torch.tensor([0.]), persistent = False)
 
         # default to device of unets passed in
 
         self.to(next(self.unets.parameters()).device)
 
+    def force_unconditional_(self):
+        self.condition_on_text = False
+        self.unconditional = True
+
+        for unet in self.unets:
+            unet.cond_on_text = False
+
     @property
     def device(self):
         return self._temp.device
 
     def get_unet(self, unet_number):
         assert 0 < unet_number <= len(self.unets)
         index = unet_number - 1
@@ -251,16 +278,19 @@
     @contextmanager
     def one_unet_in_gpu(self, unet_number = None, unet = None):
         assert exists(unet_number) ^ exists(unet)
 
         if exists(unet_number):
             unet = self.unets[unet_number - 1]
 
+        cpu = torch.device('cpu')
+
         devices = [module_device(unet) for unet in self.unets]
-        self.unets.cpu()
+
+        self.unets.to(cpu)
         unet.to(self.device)
 
         yield
 
         for unet, device in zip(self.unets, devices):
             unet.to(device)
 
@@ -366,23 +396,30 @@
         shape,
         *,
         unet_number,
         clamp = True,
         dynamic_threshold = True,
         cond_scale = 1.,
         use_tqdm = True,
+        inpaint_videos = None,
         inpaint_images = None,
         inpaint_masks = None,
         inpaint_resample_times = 5,
         init_images = None,
         skip_steps = None,
         sigma_min = None,
         sigma_max = None,
         **kwargs
     ):
+        # video
+
+        is_video = len(shape) == 5
+        frames = shape[-3] if is_video else None
+        resize_kwargs = dict(target_frames = frames) if exists(frames) else dict()
+
         # get specific sampling hyperparameters for unet
 
         hp = self.hparams[unet_number - 1]
 
         sigma_min = default(sigma_min, hp.sigma_min)
         sigma_max = default(sigma_max, hp.sigma_max)
 
@@ -411,21 +448,22 @@
 
         # keeping track of x0, for self conditioning if needed
 
         x_start = None
 
         # prepare inpainting images and mask
 
+        inpaint_images = default(inpaint_videos, inpaint_images)
         has_inpainting = exists(inpaint_images) and exists(inpaint_masks)
         resample_times = inpaint_resample_times if has_inpainting else 1
 
         if has_inpainting:
             inpaint_images = self.normalize_img(inpaint_images)
-            inpaint_images = self.resize_to(inpaint_images, shape[-1])
-            inpaint_masks = self.resize_to(rearrange(inpaint_masks, 'b ... -> b 1 ...').float(), shape[-1]).bool()
+            inpaint_images = self.resize_to(inpaint_images, shape[-1], **resize_kwargs)
+            inpaint_masks = self.resize_to(rearrange(inpaint_masks, 'b ... -> b 1 ...').float(), shape[-1], **resize_kwargs).bool()
 
         # unet kwargs
 
         unet_kwargs = dict(
             sigma_data = hp.sigma_data,
             clamp = clamp,
             dynamic_threshold = dynamic_threshold,
@@ -470,15 +508,17 @@
 
                 denoised_over_sigma = (images_hat - model_output) / sigma_hat
 
                 images_next = images_hat + (sigma_next - sigma_hat) * denoised_over_sigma
 
                 # second order correction, if not the last timestep
 
-                if sigma_next != 0:
+                has_second_order_correction = sigma_next != 0
+
+                if has_second_order_correction:
                     self_cond = model_output if unet.self_cond else None
 
                     model_output_next = self.preconditioned_network_forward(
                         unet.forward_with_cond_scale,
                         images_next,
                         sigma_next,
                         self_cond = self_cond,
@@ -491,15 +531,15 @@
                 images = images_next
 
                 if has_inpainting and not (is_last_resample_step or is_last_timestep):
                     # renoise in repaint and then resample
                     repaint_noise = torch.randn(shape, device = self.device)
                     images = images + (sigma - sigma_next) * repaint_noise
 
-                x_start = model_output  # save model output for self conditioning
+                x_start = model_output if not has_second_order_correction else model_output_next # save model output for self conditioning
 
         images = images.clamp(-1., 1.)
 
         if has_inpainting:
             images = images * ~inpaint_masks + inpaint_images * inpaint_masks
 
         return self.unnormalize_img(images)
@@ -508,14 +548,17 @@
     @eval_decorator
     def sample(
         self,
         texts: List[str] = None,
         text_masks = None,
         text_embeds = None,
         cond_images = None,
+        cond_video_frames = None,
+        post_cond_video_frames = None,
+        inpaint_videos = None,
         inpaint_images = None,
         inpaint_masks = None,
         inpaint_resample_times = 5,
         init_images = None,
         skip_steps = None,
         sigma_min = None,
         sigma_max = None,
@@ -525,33 +568,48 @@
         lowres_sample_noise_level = None,
         start_at_unet_number = 1,
         start_image_or_video = None,
         stop_at_unet_number = None,
         return_all_unet_outputs = False,
         return_pil_images = False,
         use_tqdm = True,
+        use_one_unet_in_gpu = True,
         device = None,
     ):
         device = default(device, self.device)
         self.reset_unets_all_one_device(device = device)
 
         cond_images = maybe(cast_uint8_images_to_float)(cond_images)
 
         if exists(texts) and not exists(text_embeds) and not self.unconditional:
+            assert all([*map(len, texts)]), 'text cannot be empty'
+
             with autocast(enabled = False):
                 text_embeds, text_masks = self.encode_text(texts, return_attn_mask = True)
 
             text_embeds, text_masks = map(lambda t: t.to(device), (text_embeds, text_masks))
 
         if not self.unconditional:
-            text_masks = default(text_masks, lambda: torch.any(text_embeds != 0., dim = -1))
+            assert exists(text_embeds), 'text must be passed in if the network was not trained without text `condition_on_text` must be set to `False` when training'
 
-        if not self.unconditional:
+            text_masks = default(text_masks, lambda: torch.any(text_embeds != 0., dim = -1))
             batch_size = text_embeds.shape[0]
 
+        # inpainting
+
+        inpaint_images = default(inpaint_videos, inpaint_images)
+
+        if exists(inpaint_images):
+            if self.unconditional:
+                if batch_size == 1: # assume researcher wants to broadcast along inpainted images
+                    batch_size = inpaint_images.shape[0]
+
+            assert inpaint_images.shape[0] == batch_size, 'number of inpainting images must be equal to the specified batch size on sample `sample(batch_size=<int>)``'
+            assert not (self.condition_on_text and inpaint_images.shape[0] != text_embeds.shape[0]), 'number of inpainting images must be equal to the number of text to be conditioned on'
+
         assert not (self.condition_on_text and not exists(text_embeds)), 'text or text encodings must be passed into imagen if specified'
         assert not (not self.condition_on_text and exists(text_embeds)), 'imagen specified not to be conditioned on text, yet it is presented'
         assert not (exists(text_embeds) and text_embeds.shape[-1] != self.text_embed_dim), f'invalid text embedding dimension being passed in (should be {self.text_embed_dim})'
 
         assert not (exists(inpaint_images) ^ exists(inpaint_masks)),  'inpaint images and masks must be both passed in to do inpainting'
 
         outputs = []
@@ -562,17 +620,27 @@
         lowres_sample_noise_level = default(lowres_sample_noise_level, self.lowres_sample_noise_level)
 
         num_unets = len(self.unets)
         cond_scale = cast_tuple(cond_scale, num_unets)
 
         # handle video and frame dimension
 
+        if self.is_video and exists(inpaint_images):
+            video_frames = inpaint_images.shape[2]
+
+            if inpaint_masks.ndim == 3:
+                inpaint_masks = repeat(inpaint_masks, 'b h w -> b f h w', f = video_frames)
+
+            assert inpaint_masks.shape[1] == video_frames
+
         assert not (self.is_video and not exists(video_frames)), 'video_frames must be passed in on sample time if training on video'
 
-        frame_dims = (video_frames,) if self.is_video else tuple()
+        # determine the frame dimensions, if needed
+
+        all_frame_dims = calc_all_frame_dims(self.temporal_downsample_factor, video_frames)
 
         # initializing with an image or video
 
         init_images = cast_tuple(init_images, num_unets)
         init_images = [maybe(self.normalize_img)(init_image) for init_image in init_images]
 
         skip_steps = cast_tuple(skip_steps, num_unets)
@@ -588,37 +656,60 @@
             assert exists(start_image_or_video), 'starting image or video must be supplied if only doing upscaling'
 
             prev_image_size = self.image_sizes[start_at_unet_number - 2]
             img = self.resize_to(start_image_or_video, prev_image_size)
 
         # go through each unet in cascade
 
-        for unet_number, unet, channel, image_size, unet_hparam, dynamic_threshold, unet_cond_scale, unet_init_images, unet_skip_steps, unet_sigma_min, unet_sigma_max in tqdm(zip(range(1, num_unets + 1), self.unets, self.sample_channels, self.image_sizes, self.hparams, self.dynamic_thresholding, cond_scale, init_images, skip_steps, sigma_min, sigma_max), disable = not use_tqdm):
+        for unet_number, unet, channel, image_size, frame_dims, unet_hparam, dynamic_threshold, unet_cond_scale, unet_init_images, unet_skip_steps, unet_sigma_min, unet_sigma_max in tqdm(zip(range(1, num_unets + 1), self.unets, self.sample_channels, self.image_sizes, all_frame_dims, self.hparams, self.dynamic_thresholding, cond_scale, init_images, skip_steps, sigma_min, sigma_max), disable = not use_tqdm):
             if unet_number < start_at_unet_number:
                 continue
 
             assert not isinstance(unet, NullUnet), 'cannot sample from null unet'
 
-            context = self.one_unet_in_gpu(unet = unet) if is_cuda else nullcontext()
+            context = self.one_unet_in_gpu(unet = unet) if is_cuda and use_one_unet_in_gpu else nullcontext()
 
             with context:
                 lowres_cond_img = lowres_noise_times = None
 
                 shape = (batch_size, channel, *frame_dims, image_size, image_size)
 
+                resize_kwargs = dict()
+                video_kwargs = dict()
+
+                if self.is_video:
+                    resize_kwargs = dict(target_frames = frame_dims[0])
+
+                    video_kwargs = dict(
+                        cond_video_frames = cond_video_frames,
+                        post_cond_video_frames = post_cond_video_frames
+                    )
+
+                    video_kwargs = compact(video_kwargs)
+
+                # handle video conditioning frames
+
+                if self.is_video and self.resize_cond_video_frames:
+                    downsample_scale = self.temporal_downsample_factor[unet_number - 1]
+                    temporal_downsample_fn = partial(scale_video_time, downsample_scale = downsample_scale)
+                    video_kwargs = maybe_transform_dict_key(video_kwargs, 'cond_video_frames', temporal_downsample_fn)
+                    video_kwargs = maybe_transform_dict_key(video_kwargs, 'post_cond_video_frames', temporal_downsample_fn)
+
+                # low resolution conditioning
+
                 if unet.lowres_cond:
                     lowres_noise_times = self.lowres_noise_schedule.get_times(batch_size, lowres_sample_noise_level, device = device)
 
-                    lowres_cond_img = self.resize_to(img, image_size)
+                    lowres_cond_img = self.resize_to(img, image_size, **resize_kwargs)
                     lowres_cond_img = self.normalize_img(lowres_cond_img)
 
-                    lowres_cond_img, _ = self.lowres_noise_schedule.q_sample(x_start = lowres_cond_img, t = lowres_noise_times, noise = torch.randn_like(lowres_cond_img))
+                    lowres_cond_img, *_ = self.lowres_noise_schedule.q_sample(x_start = lowres_cond_img, t = lowres_noise_times, noise = torch.randn_like(lowres_cond_img))
 
                 if exists(unet_init_images):
-                    unet_init_images = self.resize_to(unet_init_images, image_size)
+                    unet_init_images = self.resize_to(unet_init_images, image_size, **resize_kwargs)
 
                 shape = (batch_size, self.channels, *frame_dims, image_size, image_size)
 
                 img = self.one_unet_sample(
                     unet,
                     shape,
                     unet_number = unet_number,
@@ -632,15 +723,16 @@
                     skip_steps = unet_skip_steps,
                     sigma_min = unet_sigma_min,
                     sigma_max = unet_sigma_max,
                     cond_scale = unet_cond_scale,
                     lowres_cond_img = lowres_cond_img,
                     lowres_noise_times = lowres_noise_times,
                     dynamic_threshold = dynamic_threshold,
-                    use_tqdm = use_tqdm
+                    use_tqdm = use_tqdm,
+                    **video_kwargs
                 )
 
                 outputs.append(img)
 
             if exists(stop_at_unet_number) and stop_at_unet_number == unet_number:
                 break
 
@@ -664,50 +756,63 @@
         return (sigma ** 2 + sigma_data ** 2) * (sigma * sigma_data) ** -2
 
     def noise_distribution(self, P_mean, P_std, batch_size):
         return (P_mean + P_std * torch.randn((batch_size,), device = self.device)).exp()
 
     def forward(
         self,
-        images,
-        unet: Union[Unet, Unet3D, NullUnet] = None,
+        images, # rename to images or video
+        unet: Union[Unet, Unet3D, NullUnet, DistributedDataParallel] = None,
         texts: List[str] = None,
         text_embeds = None,
         text_masks = None,
         unet_number = None,
-        cond_images = None
+        cond_images = None,
+        **kwargs
     ):
+        if self.is_video and images.ndim == 4:
+            images = rearrange(images, 'b c h w -> b c 1 h w')
+            kwargs.update(ignore_time = True)
+
         assert images.shape[-1] == images.shape[-2], f'the images you pass in must be a square, but received dimensions of {images.shape[2]}, {images.shape[-1]}'
         assert not (len(self.unets) > 1 and not exists(unet_number)), f'you must specify which unet you want trained, from a range of 1 to {len(self.unets)}, if you are training cascading DDPM (multiple unets)'
         unet_number = default(unet_number, 1)
         assert not exists(self.only_train_unet_number) or self.only_train_unet_number == unet_number, 'you can only train on unet #{self.only_train_unet_number}'
 
         images = cast_uint8_images_to_float(images)
         cond_images = maybe(cast_uint8_images_to_float)(cond_images)
 
+        assert images.dtype == torch.float, f'images tensor needs to be floats but {images.dtype} dtype found instead'
+
         unet_index = unet_number - 1
         
         unet = default(unet, lambda: self.get_unet(unet_number))
 
         assert not isinstance(unet, NullUnet), 'null unet cannot and should not be trained'
 
         target_image_size    = self.image_sizes[unet_index]
         random_crop_size     = self.random_crop_sizes[unet_index]
         prev_image_size      = self.image_sizes[unet_index - 1] if unet_index > 0 else None
         hp                   = self.hparams[unet_index]
 
         batch_size, c, *_, h, w, device, is_video = *images.shape, images.device, (images.ndim == 5)
 
-        frames = images.shape[2] if is_video else None
-
-        check_shape(images, 'b c ...', c = self.channels)
+        frames              = images.shape[2] if is_video else None
+        all_frame_dims      = tuple(safe_get_tuple_index(el, 0) for el in calc_all_frame_dims(self.temporal_downsample_factor, frames))
+        ignore_time         = kwargs.get('ignore_time', False)
+
+        target_frame_size   = all_frame_dims[unet_index] if is_video and not ignore_time else None
+        prev_frame_size     = all_frame_dims[unet_index - 1] if is_video and not ignore_time and unet_index > 0 else None
+        frames_to_resize_kwargs = lambda frames: dict(target_frames = frames) if exists(frames) else dict()
 
+        assert images.shape[1] == self.channels
         assert h >= target_image_size and w >= target_image_size
 
         if exists(texts) and not exists(text_embeds) and not self.unconditional:
+            assert all([*map(len, texts)]), 'text cannot be empty'
             assert len(texts) == len(images), 'number of text captions does not match up with the number of images given'
 
             with autocast(enabled = False):
                 text_embeds, text_masks = self.encode_text(texts, return_attn_mask = True)
 
             text_embeds, text_masks = map(lambda t: t.to(images.device), (text_embeds, text_masks))
 
@@ -715,55 +820,65 @@
             text_masks = default(text_masks, lambda: torch.any(text_embeds != 0., dim = -1))
 
         assert not (self.condition_on_text and not exists(text_embeds)), 'text or text encodings must be passed into decoder if specified'
         assert not (not self.condition_on_text and exists(text_embeds)), 'decoder specified not to be conditioned on text, yet it is presented'
 
         assert not (exists(text_embeds) and text_embeds.shape[-1] != self.text_embed_dim), f'invalid text embedding dimension being passed in (should be {self.text_embed_dim})'
 
+        # handle video conditioning frames
+
+        if self.is_video and self.resize_cond_video_frames:
+            downsample_scale = self.temporal_downsample_factor[unet_index]
+            temporal_downsample_fn = partial(scale_video_time, downsample_scale = downsample_scale)
+            kwargs = maybe_transform_dict_key(kwargs, 'cond_video_frames', temporal_downsample_fn)
+            kwargs = maybe_transform_dict_key(kwargs, 'post_cond_video_frames', temporal_downsample_fn)
+
+        # low resolution conditioning
+
         lowres_cond_img = lowres_aug_times = None
         if exists(prev_image_size):
-            lowres_cond_img = self.resize_to(images, prev_image_size, clamp_range = self.input_image_range)
-            lowres_cond_img = self.resize_to(lowres_cond_img, target_image_size, clamp_range = self.input_image_range)
+            lowres_cond_img = self.resize_to(images, prev_image_size, **frames_to_resize_kwargs(prev_frame_size), clamp_range = self.input_image_range)
+            lowres_cond_img = self.resize_to(lowres_cond_img, target_image_size, **frames_to_resize_kwargs(target_frame_size), clamp_range = self.input_image_range)
 
             if self.per_sample_random_aug_noise_level:
                 lowres_aug_times = self.lowres_noise_schedule.sample_random_times(batch_size, device = device)
             else:
                 lowres_aug_time = self.lowres_noise_schedule.sample_random_times(1, device = device)
                 lowres_aug_times = repeat(lowres_aug_time, '1 -> b', b = batch_size)
 
-        images = self.resize_to(images, target_image_size)
+        images = self.resize_to(images, target_image_size, **frames_to_resize_kwargs(target_frame_size))
 
         # normalize to [-1, 1]
 
         images = self.normalize_img(images)
         lowres_cond_img = maybe(self.normalize_img)(lowres_cond_img)
 
         # random cropping during training
         # for upsamplers
 
         if exists(random_crop_size):
             aug = K.RandomCrop((random_crop_size, random_crop_size), p = 1.)
 
             if is_video:
-                images, lowres_cond_img = rearrange_many((images, lowres_cond_img), 'b c f h w -> (b f) c h w')
+                images, lowres_cond_img = map(lambda t: rearrange(t, 'b c f h w -> (b f) c h w'), (images, lowres_cond_img))
 
             # make sure low res conditioner and image both get augmented the same way
             # detailed https://kornia.readthedocs.io/en/latest/augmentation.module.html?highlight=randomcrop#kornia.augmentation.RandomCrop
             images = aug(images)
             lowres_cond_img = aug(lowres_cond_img, params = aug._params)
 
             if is_video:
-                images, lowres_cond_img = rearrange_many((images, lowres_cond_img), '(b f) c h w -> b c f h w', f = frames)
+                images, lowres_cond_img = map(lambda t: rearrange(t, '(b f) c h w -> b c f h w', f = frames), (images, lowres_cond_img))
 
         # noise the lowres conditioning image
         # at sample time, they then fix the noise level of 0.1 - 0.3
 
         lowres_cond_img_noisy = None
         if exists(lowres_cond_img):
-            lowres_cond_img_noisy, _ = self.lowres_noise_schedule.q_sample(x_start = lowres_cond_img, t = lowres_aug_times, noise = torch.randn_like(lowres_cond_img))
+            lowres_cond_img_noisy, *_ = self.lowres_noise_schedule.q_sample(x_start = lowres_cond_img, t = lowres_aug_times, noise = torch.randn_like(lowres_cond_img))
 
         # get the sigmas
 
         sigmas = self.noise_distribution(hp.P_mean, hp.P_std, batch_size)
         padded_sigmas = self.right_pad_dims_to_datatype(sigmas)
 
         # noise
@@ -777,19 +892,25 @@
             sigma_data = hp.sigma_data,
             text_embeds = text_embeds,
             text_mask = text_masks,
             cond_images = cond_images,
             lowres_noise_times = self.lowres_noise_schedule.get_condition(lowres_aug_times),
             lowres_cond_img = lowres_cond_img_noisy,
             cond_drop_prob = self.cond_drop_prob,
+            **kwargs
         )
 
         # self conditioning - https://arxiv.org/abs/2208.04202 - training will be 25% slower
 
-        if unet.self_cond and random() < 0.5:
+        # Because 'unet' can be an instance of DistributedDataParallel coming from the
+        # ImagenTrainer.unet_being_trained when invoking ImagenTrainer.forward(), we need to
+        # access the member 'module' of the wrapped unet instance.
+        self_cond = unet.module.self_cond if isinstance(unet, DistributedDataParallel) else unet.self_cond
+
+        if self_cond and random() < 0.5:
             with torch.no_grad():
                 pred_x0 = self.preconditioned_network_forward(
                     unet.forward,
                     noised_images,
                     sigmas,
                     **unet_kwargs
                 ).detach()
```

### Comparing `imagen-pytorch-1.9.7/imagen_pytorch/imagen_pytorch.py` & `imagen_pytorch-2.0.0/imagen_pytorch/imagen_pytorch.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 import math
-import copy
 from random import random
-from typing import List, Union
-from tqdm import tqdm
+from beartype.typing import List, Union, Optional
+from beartype import beartype
+from tqdm.auto import tqdm
 from functools import partial, wraps
 from contextlib import contextmanager, nullcontext
-from collections import namedtuple
 from pathlib import Path
 
 import torch
 import torch.nn.functional as F
+from torch.nn.parallel import DistributedDataParallel
 from torch import nn, einsum
 from torch.cuda.amp import autocast
 from torch.special import expm1
 import torchvision.transforms as T
 
 import kornia.augmentation as K
 
-from einops import rearrange, repeat, reduce
-from einops.layers.torch import Rearrange, Reduce
-from einops_exts import rearrange_many, repeat_many, check_shape
-from einops_exts.torch import EinopsToAndFrom
+from einops import rearrange, repeat, reduce, pack, unpack
+from einops.layers.torch import Rearrange
 
 from imagen_pytorch.t5 import t5_encode_text, get_encoded_dim, DEFAULT_T5_NAME
 
-from imagen_pytorch.imagen_video.imagen_video import Unet3D, resize_video_to
+from imagen_pytorch.imagen_video import Unet3D, resize_video_to, scale_video_time
 
 # helper functions
 
 def exists(val):
     return val is not None
 
 def identity(t, *args, **kwargs):
     return t
 
+def divisible_by(numer, denom):
+    return (numer % denom) == 0
+
 def first(arr, d = None):
     if len(arr) == 0:
         return d
     return arr[0]
 
 def maybe(fn):
     @wraps(fn)
@@ -72,14 +73,25 @@
     output = val if isinstance(val, tuple) else ((val,) * default(length, 1))
 
     if exists(length):
         assert len(output) == length
 
     return output
 
+def compact(input_dict):
+    return {key: value for key, value in input_dict.items() if exists(value)}
+
+def maybe_transform_dict_key(input_dict, key, fn):
+    if key not in input_dict:
+        return input_dict
+
+    copied_dict = input_dict.copy()
+    copied_dict[key] = fn(copied_dict[key])
+    return copied_dict
+
 def cast_uint8_images_to_float(images):
     if not images.dtype == torch.uint8:
         return images
     return images / 255
 
 def module_device(module):
     return next(module.parameters()).device
@@ -136,28 +148,49 @@
     masked_t = t.masked_fill(~mask, 0.)
 
     return masked_t.sum(dim = dim) / denom.clamp(min = 1e-5)
 
 def resize_image_to(
     image,
     target_image_size,
-    clamp_range = None
+    clamp_range = None,
+    mode = 'nearest'
 ):
     orig_image_size = image.shape[-1]
 
     if orig_image_size == target_image_size:
         return image
 
-    out = F.interpolate(image, target_image_size, mode = 'nearest')
+    out = F.interpolate(image, target_image_size, mode = mode)
 
     if exists(clamp_range):
         out = out.clamp(*clamp_range)
 
     return out
 
+def calc_all_frame_dims(
+    downsample_factors: List[int],
+    frames
+):
+    if not exists(frames):
+        return (tuple(),) * len(downsample_factors)
+
+    all_frame_dims = []
+
+    for divisor in downsample_factors:
+        assert divisible_by(frames, divisor)
+        all_frame_dims.append((frames // divisor,))
+
+    return all_frame_dims
+
+def safe_get_tuple_index(tup, index, default = None):
+    if len(tup) <= index:
+        return default
+    return tup[index]
+
 # image normalization functions
 # ddpms expect images to be in the range of -1 to 1
 
 def normalize_neg_one_to_one(img):
     return img * 2 - 1
 
 def unnormalize_zero_to_one(normed_img):
@@ -199,16 +232,16 @@
             raise ValueError(f'invalid noise schedule {noise_schedule}')
 
         self.num_timesteps = timesteps
 
     def get_times(self, batch_size, noise_level, *, device):
         return torch.full((batch_size,), noise_level, device = device, dtype = torch.float32)
 
-    def sample_random_times(self, batch_size, max_thres = 0.999, *, device):
-        return torch.zeros((batch_size,), device = device).float().uniform_(0, max_thres)
+    def sample_random_times(self, batch_size, *, device):
+        return torch.zeros((batch_size,), device = device).float().uniform_(0, 1)
 
     def get_condition(self, times):
         return maybe(self.log_snr)(times)
 
     def get_sampling_timesteps(self, batch, *, device):
         times = torch.linspace(1., 0., self.num_timesteps + 1, device = device)
         times = repeat(times, 't -> b t', b = batch)
@@ -244,15 +277,15 @@
             t = torch.full((batch,), t, device = x_start.device, dtype = dtype)
 
         noise = default(noise, lambda: torch.randn_like(x_start))
         log_snr = self.log_snr(t).type(dtype)
         log_snr_padded_dim = right_pad_dims_to(x_start, log_snr)
         alpha, sigma =  log_snr_to_alpha_sigma(log_snr_padded_dim)
 
-        return alpha * x_start + sigma * noise, log_snr
+        return alpha * x_start + sigma * noise, log_snr, alpha, sigma
 
     def q_sample_from_to(self, x_from, from_t, to_t, noise = None):
         shape, device, dtype = x_from.shape, x_from.device, x_from.dtype
         batch = shape[0]
 
         if isinstance(from_t, float):
             from_t = torch.full((batch,), from_t, device = device, dtype = dtype)
@@ -262,65 +295,65 @@
 
         noise = default(noise, lambda: torch.randn_like(x_from))
 
         log_snr = self.log_snr(from_t)
         log_snr_padded_dim = right_pad_dims_to(x_from, log_snr)
         alpha, sigma =  log_snr_to_alpha_sigma(log_snr_padded_dim)
 
-        log_snr_to = self.log_snr(from_t)
+        log_snr_to = self.log_snr(to_t)
         log_snr_padded_dim_to = right_pad_dims_to(x_from, log_snr_to)
         alpha_to, sigma_to =  log_snr_to_alpha_sigma(log_snr_padded_dim_to)
 
         return x_from * (alpha_to / alpha) + noise * (sigma_to * alpha - sigma * alpha_to) / alpha
 
+    def predict_start_from_v(self, x_t, t, v):
+        log_snr = self.log_snr(t)
+        log_snr = right_pad_dims_to(x_t, log_snr)
+        alpha, sigma = log_snr_to_alpha_sigma(log_snr)
+        return alpha * x_t - sigma * v
+
     def predict_start_from_noise(self, x_t, t, noise):
         log_snr = self.log_snr(t)
         log_snr = right_pad_dims_to(x_t, log_snr)
         alpha, sigma = log_snr_to_alpha_sigma(log_snr)
         return (x_t - sigma * noise) / alpha.clamp(min = 1e-8)
 
 # norms and residuals
 
-class LayerNorm(nn.Module):
-    def __init__(self, dim, stable = False):
+class ChanRMSNorm(nn.Module):
+    def __init__(self, dim):
         super().__init__()
-        self.stable = stable
-        self.g = nn.Parameter(torch.ones(dim))
+        self.scale = dim ** 0.5
+        self.gamma = nn.Parameter(torch.ones(dim, 1, 1))
 
     def forward(self, x):
-        dtype = x.dtype
+        return F.normalize(x, dim = 1) * self.scale * self.gamma
 
-        if self.stable:
-            x = x / x.amax(dim = -1, keepdim = True).detach()
-
-        eps = 1e-5 if x.dtype == torch.float32 else 1e-3
-        var = torch.var(x, dim = -1, unbiased = False, keepdim = True)
-        mean = torch.mean(x, dim = -1, keepdim = True)
-
-        return (x - mean) * (var + eps).rsqrt().type(dtype) * self.g.type(dtype)
-
-
-class ChanLayerNorm(nn.Module):
-    def __init__(self, dim, stable = False):
+class LayerNorm(nn.Module):
+    def __init__(self, feats, stable = False, dim = -1):
         super().__init__()
         self.stable = stable
-        self.g = nn.Parameter(torch.ones(1, dim, 1, 1))
+        self.dim = dim
+
+        self.g = nn.Parameter(torch.ones(feats, *((1,) * (-dim - 1))))
 
     def forward(self, x):
-        dtype = x.dtype
+        dtype, dim = x.dtype, self.dim
 
         if self.stable:
-            x = x / x.amax(dim = 1, keepdim = True).detach()
+            x = x / x.amax(dim = dim, keepdim = True).detach()
 
         eps = 1e-5 if x.dtype == torch.float32 else 1e-3
-        var = torch.var(x, dim = 1, unbiased = False, keepdim = True)
-        mean = torch.mean(x, dim = 1, keepdim = True)
+        var = torch.var(x, dim = dim, unbiased = False, keepdim = True)
+        mean = torch.mean(x, dim = dim, keepdim = True)
 
         return (x - mean) * (var + eps).rsqrt().type(dtype) * self.g.type(dtype)
 
+ChanLayerNorm = partial(LayerNorm, dim = -3)
+
 class Always():
     def __init__(self, val):
         self.val = val
 
     def __call__(self, *args, **kwargs):
         return self.val
 
@@ -346,30 +379,31 @@
 class PerceiverAttention(nn.Module):
     def __init__(
         self,
         *,
         dim,
         dim_head = 64,
         heads = 8,
-        cosine_sim_attn = False
+        scale = 8
     ):
         super().__init__()
-        self.scale = dim_head ** -0.5 if not cosine_sim_attn else 1
-        self.cosine_sim_attn = cosine_sim_attn
-        self.cosine_sim_scale = 16 if cosine_sim_attn else 1
+        self.scale = scale
 
         self.heads = heads
         inner_dim = dim_head * heads
 
         self.norm = nn.LayerNorm(dim)
         self.norm_latents = nn.LayerNorm(dim)
 
         self.to_q = nn.Linear(dim, inner_dim, bias = False)
         self.to_kv = nn.Linear(dim, inner_dim * 2, bias = False)
 
+        self.q_scale = nn.Parameter(torch.ones(dim_head))
+        self.k_scale = nn.Parameter(torch.ones(dim_head))
+
         self.to_out = nn.Sequential(
             nn.Linear(inner_dim, dim, bias = False),
             nn.LayerNorm(dim)
         )
 
     def forward(self, x, latents, mask = None):
         x = self.norm(x)
@@ -379,26 +413,25 @@
 
         q = self.to_q(latents)
 
         # the paper differs from Perceiver in which they also concat the key / values derived from the latents to be attended to
         kv_input = torch.cat((x, latents), dim = -2)
         k, v = self.to_kv(kv_input).chunk(2, dim = -1)
 
-        q, k, v = rearrange_many((q, k, v), 'b n (h d) -> b h n d', h = h)
+        q, k, v = map(lambda t: rearrange(t, 'b n (h d) -> b h n d', h = h), (q, k, v))
 
-        q = q * self.scale
-
-        # cosine sim attention
+        # qk rmsnorm
 
-        if self.cosine_sim_attn:
-            q, k = map(l2norm, (q, k))
+        q, k = map(l2norm, (q, k))
+        q = q * self.q_scale
+        k = k * self.k_scale
 
         # similarities and masking
 
-        sim = einsum('... i d, ... j d  -> ... i j', q, k) * self.cosine_sim_scale
+        sim = einsum('... i d, ... j d  -> ... i j', q, k) * self.scale
 
         if exists(mask):
             max_neg_value = -torch.finfo(sim.dtype).max
             mask = F.pad(mask, (0, latents.shape[-2]), value = True)
             mask = rearrange(mask, 'b j -> b 1 1 j')
             sim = sim.masked_fill(~mask, max_neg_value)
 
@@ -418,16 +451,15 @@
         dim,
         depth,
         dim_head = 64,
         heads = 8,
         num_latents = 64,
         num_latents_mean_pooled = 4, # number of latents derived from mean pooled representation of the sequence
         max_seq_len = 512,
-        ff_mult = 4,
-        cosine_sim_attn = False
+        ff_mult = 4
     ):
         super().__init__()
         self.pos_emb = nn.Embedding(max_seq_len, dim)
 
         self.latents = nn.Parameter(torch.randn(num_latents, dim))
 
         self.to_latents_from_mean_pooled_seq = None
@@ -438,15 +470,15 @@
                 nn.Linear(dim, dim * num_latents_mean_pooled),
                 Rearrange('b (n d) -> b n d', n = num_latents_mean_pooled)
             )
 
         self.layers = nn.ModuleList([])
         for _ in range(depth):
             self.layers.append(nn.ModuleList([
-                PerceiverAttention(dim = dim, dim_head = dim_head, heads = heads, cosine_sim_attn = cosine_sim_attn),
+                PerceiverAttention(dim = dim, dim_head = dim_head, heads = heads),
                 FeedForward(dim = dim, mult = ff_mult)
             ]))
 
     def forward(self, x, mask = None):
         n, device = x.shape[1], x.device
         pos_emb = self.pos_emb(torch.arange(n, device = device))
 
@@ -471,30 +503,31 @@
     def __init__(
         self,
         dim,
         *,
         dim_head = 64,
         heads = 8,
         context_dim = None,
-        cosine_sim_attn = False
+        scale = 8
     ):
         super().__init__()
-        self.scale = dim_head ** -0.5 if not cosine_sim_attn else 1.
-        self.cosine_sim_attn = cosine_sim_attn
-        self.cosine_sim_scale = 16 if cosine_sim_attn else 1
+        self.scale = scale
 
         self.heads = heads
         inner_dim = dim_head * heads
 
         self.norm = LayerNorm(dim)
 
         self.null_kv = nn.Parameter(torch.randn(2, dim_head))
         self.to_q = nn.Linear(dim, inner_dim, bias = False)
         self.to_kv = nn.Linear(dim, dim_head * 2, bias = False)
 
+        self.q_scale = nn.Parameter(torch.ones(dim_head))
+        self.k_scale = nn.Parameter(torch.ones(dim_head))
+
         self.to_context = nn.Sequential(nn.LayerNorm(context_dim), nn.Linear(context_dim, dim_head * 2)) if exists(context_dim) else None
 
         self.to_out = nn.Sequential(
             nn.Linear(inner_dim, dim, bias = False),
             LayerNorm(dim)
         )
 
@@ -502,38 +535,38 @@
         b, n, device = *x.shape[:2], x.device
 
         x = self.norm(x)
 
         q, k, v = (self.to_q(x), *self.to_kv(x).chunk(2, dim = -1))
 
         q = rearrange(q, 'b n (h d) -> b h n d', h = self.heads)
-        q = q * self.scale
 
         # add null key / value for classifier free guidance in prior net
 
-        nk, nv = repeat_many(self.null_kv.unbind(dim = -2), 'd -> b 1 d', b = b)
+        nk, nv = map(lambda t: repeat(t, 'd -> b 1 d', b = b), self.null_kv.unbind(dim = -2))
         k = torch.cat((nk, k), dim = -2)
         v = torch.cat((nv, v), dim = -2)
 
         # add text conditioning, if present
 
         if exists(context):
             assert exists(self.to_context)
             ck, cv = self.to_context(context).chunk(2, dim = -1)
             k = torch.cat((ck, k), dim = -2)
             v = torch.cat((cv, v), dim = -2)
 
-        # cosine sim attention
+        # qk rmsnorm
 
-        if self.cosine_sim_attn:
-            q, k = map(l2norm, (q, k))
+        q, k = map(l2norm, (q, k))
+        q = q * self.q_scale
+        k = k * self.k_scale
 
         # calculate query / key similarities
 
-        sim = einsum('b h i d, b j d -> b h i j', q, k) * self.cosine_sim_scale
+        sim = einsum('b h i d, b j d -> b h i j', q, k) * self.scale
 
         # relative positional encoding (T5 style)
 
         if exists(attn_bias):
             sim = sim + attn_bias
 
         # masking
@@ -594,16 +627,21 @@
         conv.weight.data.copy_(conv_weight)
         nn.init.zeros_(conv.bias.data)
 
     def forward(self, x):
         return self.net(x)
 
 def Downsample(dim, dim_out = None):
+    # https://arxiv.org/abs/2208.03641 shows this is the most optimal way to downsample
+    # named SP-conv in the paper, but basically a pixel unshuffle
     dim_out = default(dim_out, dim)
-    return nn.Conv2d(dim, dim_out, 4, 2, 1)
+    return nn.Sequential(
+        Rearrange('b c (h s1) (w s2) -> b (c s1 s2) h w', s1 = 2, s2 = 2),
+        nn.Conv2d(dim * 4, dim_out, 1)
+    )
 
 class SinusoidalPosEmb(nn.Module):
     def __init__(self, dim):
         super().__init__()
         self.dim = dim
 
     def forward(self, x):
@@ -631,24 +669,23 @@
         return fouriered
 
 class Block(nn.Module):
     def __init__(
         self,
         dim,
         dim_out,
-        groups = 8,
         norm = True
     ):
         super().__init__()
-        self.groupnorm = nn.GroupNorm(groups, dim) if norm else Identity()
+        self.norm = ChanRMSNorm(dim) if norm else Identity()
         self.activation = nn.SiLU()
         self.project = nn.Conv2d(dim, dim_out, 3, padding = 1)
 
     def forward(self, x, scale_shift = None):
-        x = self.groupnorm(x)
+        x = self.norm(x)
 
         if exists(scale_shift):
             scale, shift = scale_shift
             x = x * (scale + 1) + shift
 
         x = self.activation(x)
         return self.project(x)
@@ -657,15 +694,14 @@
     def __init__(
         self,
         dim,
         dim_out,
         *,
         cond_dim = None,
         time_cond_dim = None,
-        groups = 8,
         linear_attn = False,
         use_gca = False,
         squeeze_excite = False,
         **attn_kwargs
     ):
         super().__init__()
 
@@ -678,26 +714,22 @@
             )
 
         self.cross_attn = None
 
         if exists(cond_dim):
             attn_klass = CrossAttention if not linear_attn else LinearCrossAttention
 
-            self.cross_attn = EinopsToAndFrom(
-                'b c h w',
-                'b (h w) c',
-                attn_klass(
-                    dim = dim_out,
-                    context_dim = cond_dim,
-                    **attn_kwargs
-                )
+            self.cross_attn = attn_klass(
+                dim = dim_out,
+                context_dim = cond_dim,
+                **attn_kwargs
             )
 
-        self.block1 = Block(dim, dim_out, groups = groups)
-        self.block2 = Block(dim_out, dim_out, groups = groups)
+        self.block1 = Block(dim, dim_out)
+        self.block2 = Block(dim_out, dim_out)
 
         self.gca = GlobalContext(dim_in = dim_out, dim_out = dim_out) if use_gca else Always(1)
 
         self.res_conv = nn.Conv2d(dim, dim_out, 1) if dim != dim_out else Identity()
 
 
     def forward(self, x, time_emb = None, cond = None):
@@ -708,15 +740,19 @@
             time_emb = rearrange(time_emb, 'b c -> b c 1 1')
             scale_shift = time_emb.chunk(2, dim = 1)
 
         h = self.block1(x)
 
         if exists(self.cross_attn):
             assert exists(cond)
+            h = rearrange(h, 'b c h w -> b h w c')
+            h, ps = pack([h], 'b * c')
             h = self.cross_attn(h, context = cond) + h
+            h, = unpack(h, ps, 'b * c')
+            h = rearrange(h, 'b h w c -> b c h w')
 
         h = self.block2(h, scale_shift = scale_shift)
 
         h = h * self.gca(h)
 
         return h + self.res_conv(x)
 
@@ -725,65 +761,65 @@
         self,
         dim,
         *,
         context_dim = None,
         dim_head = 64,
         heads = 8,
         norm_context = False,
-        cosine_sim_attn = False
+        scale = 8
     ):
         super().__init__()
-        self.scale = dim_head ** -0.5 if not cosine_sim_attn else 1.
-        self.cosine_sim_attn = cosine_sim_attn
-        self.cosine_sim_scale = 16 if cosine_sim_attn else 1
+        self.scale = scale
 
         self.heads = heads
         inner_dim = dim_head * heads
 
         context_dim = default(context_dim, dim)
 
         self.norm = LayerNorm(dim)
         self.norm_context = LayerNorm(context_dim) if norm_context else Identity()
 
         self.null_kv = nn.Parameter(torch.randn(2, dim_head))
         self.to_q = nn.Linear(dim, inner_dim, bias = False)
         self.to_kv = nn.Linear(context_dim, inner_dim * 2, bias = False)
 
+        self.q_scale = nn.Parameter(torch.ones(dim_head))
+        self.k_scale = nn.Parameter(torch.ones(dim_head))
+
         self.to_out = nn.Sequential(
             nn.Linear(inner_dim, dim, bias = False),
             LayerNorm(dim)
         )
 
     def forward(self, x, context, mask = None):
         b, n, device = *x.shape[:2], x.device
 
         x = self.norm(x)
         context = self.norm_context(context)
 
         q, k, v = (self.to_q(x), *self.to_kv(context).chunk(2, dim = -1))
 
-        q, k, v = rearrange_many((q, k, v), 'b n (h d) -> b h n d', h = self.heads)
+        q, k, v = map(lambda t: rearrange(t, 'b n (h d) -> b h n d', h = self.heads), (q, k, v))
 
         # add null key / value for classifier free guidance in prior net
 
-        nk, nv = repeat_many(self.null_kv.unbind(dim = -2), 'd -> b h 1 d', h = self.heads,  b = b)
+        nk, nv = map(lambda t: repeat(t, 'd -> b h 1 d', h = self.heads,  b = b), self.null_kv.unbind(dim = -2))
 
         k = torch.cat((nk, k), dim = -2)
         v = torch.cat((nv, v), dim = -2)
 
-        q = q * self.scale
-
         # cosine sim attention
 
-        if self.cosine_sim_attn:
-            q, k = map(l2norm, (q, k))
+        q, k = map(l2norm, (q, k))
+        q = q * self.q_scale
+        k = k * self.k_scale
 
         # similarities
 
-        sim = einsum('b h i d, b h j d -> b h i j', q, k) * self.cosine_sim_scale
+        sim = einsum('b h i d, b h j d -> b h i j', q, k) * self.scale
 
         # masking
 
         max_neg_value = -torch.finfo(sim.dtype).max
 
         if exists(mask):
             mask = F.pad(mask, (1, 0), value = True)
@@ -802,19 +838,19 @@
         b, n, device = *x.shape[:2], x.device
 
         x = self.norm(x)
         context = self.norm_context(context)
 
         q, k, v = (self.to_q(x), *self.to_kv(context).chunk(2, dim = -1))
 
-        q, k, v = rearrange_many((q, k, v), 'b n (h d) -> (b h) n d', h = self.heads)
+        q, k, v = map(lambda t: rearrange(t, 'b n (h d) -> (b h) n d', h = self.heads), (q, k, v))
 
         # add null key / value for classifier free guidance in prior net
 
-        nk, nv = repeat_many(self.null_kv.unbind(dim = -2), 'd -> (b h) 1 d', h = self.heads,  b = b)
+        nk, nv = map(lambda t: repeat(t, 'd -> (b h) 1 d', h = self.heads,  b = b), self.null_kv.unbind(dim = -2))
 
         k = torch.cat((nk, k), dim = -2)
         v = torch.cat((nv, v), dim = -2)
 
         # masking
 
         max_neg_value = -torch.finfo(x.dtype).max
@@ -881,20 +917,20 @@
         )
 
     def forward(self, fmap, context = None):
         h, x, y = self.heads, *fmap.shape[-2:]
 
         fmap = self.norm(fmap)
         q, k, v = map(lambda fn: fn(fmap), (self.to_q, self.to_k, self.to_v))
-        q, k, v = rearrange_many((q, k, v), 'b (h c) x y -> (b h) (x y) c', h = h)
+        q, k, v = map(lambda t: rearrange(t, 'b (h c) x y -> (b h) (x y) c', h = h), (q, k, v))
 
         if exists(context):
             assert exists(self.to_context)
             ck, cv = self.to_context(context).chunk(2, dim = -1)
-            ck, cv = rearrange_many((ck, cv), 'b n (h d) -> (b h) n d', h = h)
+            ck, cv = map(lambda t: rearrange(t, 'b n (h d) -> (b h) n d', h = h), (ck, cv))
             k = torch.cat((k, ck), dim = -2)
             v = torch.cat((v, cv), dim = -2)
 
         q = q.softmax(dim = -1)
         k = k.softmax(dim = -2)
 
         q = q * self.scale
@@ -924,15 +960,15 @@
             nn.SiLU(),
             nn.Conv2d(hidden_dim, dim_out, 1),
             nn.Sigmoid()
         )
 
     def forward(self, x):
         context = self.to_k(x)
-        x, context = rearrange_many((x, context), 'b n ... -> b n (...)')
+        x, context = map(lambda t: rearrange(t, 'b n ... -> b n (...)'), (x, context))
         out = einsum('b i n, b c n -> b c i', context.softmax(dim = -1), x)
         out = rearrange(out, '... -> ... 1')
         return self.net(out)
 
 def FeedForward(dim, mult = 2):
     hidden_dim = int(dim * mult)
     return nn.Sequential(
@@ -958,30 +994,35 @@
         self,
         dim,
         *,
         depth = 1,
         heads = 8,
         dim_head = 32,
         ff_mult = 2,
-        context_dim = None,
-        cosine_sim_attn = False
+        context_dim = None
     ):
         super().__init__()
         self.layers = nn.ModuleList([])
 
         for _ in range(depth):
             self.layers.append(nn.ModuleList([
-                EinopsToAndFrom('b c h w', 'b (h w) c', Attention(dim = dim, heads = heads, dim_head = dim_head, context_dim = context_dim, cosine_sim_attn = cosine_sim_attn)),
-                ChanFeedForward(dim = dim, mult = ff_mult)
+                Attention(dim = dim, heads = heads, dim_head = dim_head, context_dim = context_dim),
+                FeedForward(dim = dim, mult = ff_mult)
             ]))
 
     def forward(self, x, context = None):
+        x = rearrange(x, 'b c h w -> b h w c')
+        x, ps = pack([x], 'b * c')
+
         for attn, ff in self.layers:
             x = attn(x, context = context) + x
             x = ff(x) + x
+
+        x, = unpack(x, ps, 'b * c')
+        x = rearrange(x, 'b h w c -> b c h w')
         return x
 
 class LinearAttentionTransformerBlock(nn.Module):
     def __init__(
         self,
         dim,
         *,
@@ -1069,15 +1110,14 @@
         return torch.cat((x, *outs), dim = 1)
 
 class Unet(nn.Module):
     def __init__(
         self,
         *,
         dim,
-        image_embed_dim = 1024,
         text_embed_dim = get_encoded_dim(DEFAULT_T5_NAME),
         num_resnet_blocks = 1,
         cond_dim = None,
         num_image_tokens = 4,
         num_time_tokens = 2,
         learned_sinu_pos_emb_dim = 16,
         out_dim = None,
@@ -1087,41 +1127,41 @@
         channels_out = None,
         attn_dim_head = 64,
         attn_heads = 8,
         ff_mult = 2.,
         lowres_cond = False,                # for cascading diffusion - https://cascaded-diffusion.github.io/
         layer_attns = True,
         layer_attns_depth = 1,
+        layer_mid_attns_depth = 1,
         layer_attns_add_text_cond = True,   # whether to condition the self-attention blocks with the text embeddings, as described in Appendix D.3.1
         attend_at_middle = True,            # whether to have a layer of attention at the bottleneck (can turn off for higher resolution in cascading DDPM, before bringing in efficient attention)
         layer_cross_attns = True,
         use_linear_attn = False,
         use_linear_cross_attn = False,
         cond_on_text = True,
         max_text_len = 256,
         init_dim = None,
-        resnet_groups = 8,
         init_conv_kernel_size = 7,          # kernel size of initial conv, if not using cross embed
         init_cross_embed = True,
         init_cross_embed_kernel_sizes = (3, 7, 15),
         cross_embed_downsample = False,
         cross_embed_downsample_kernel_sizes = (2, 4),
         attn_pool_text = True,
         attn_pool_num_latents = 32,
         dropout = 0.,
         memory_efficient = False,
         init_conv_to_final_conv_residual = False,
         use_global_context_attn = True,
         scale_skip_connection = True,
         final_resnet_block = True,
         final_conv_kernel_size = 3,
-        cosine_sim_attn = False,
         self_cond = False,
+        resize_mode = 'nearest',
         combine_upsample_fmaps = False,      # combine feature maps from all upsample blocks, used in unet squared successfully
-        pixel_shuffle_upsample = True        # may address checkboard artifacts
+        pixel_shuffle_upsample = True,       # may address checkboard artifacts
     ):
         super().__init__()
 
         # guide researchers
 
         assert attn_heads > 1, 'you need to have more than 1 attention head, ideally at least 4 or 8'
 
@@ -1221,15 +1261,15 @@
 
         # finer control over whether to condition on text encodings
 
         self.cond_on_text = cond_on_text
 
         # attention pooling
 
-        self.attn_pool = PerceiverResampler(dim = cond_dim, depth = 2, dim_head = attn_dim_head, heads = attn_heads, num_latents = attn_pool_num_latents, cosine_sim_attn = cosine_sim_attn) if attn_pool_text else None
+        self.attn_pool = PerceiverResampler(dim = cond_dim, depth = 2, dim_head = attn_dim_head, heads = attn_heads, num_latents = attn_pool_num_latents) if attn_pool_text else None
 
         # for classifier free guidance
 
         self.max_text_len = max_text_len
 
         self.null_text_embed = nn.Parameter(torch.randn(1, max_text_len, cond_dim))
         self.null_text_hidden = nn.Parameter(torch.randn(1, time_cond_dim))
@@ -1244,66 +1284,72 @@
                 nn.Linear(cond_dim, time_cond_dim),
                 nn.SiLU(),
                 nn.Linear(time_cond_dim, time_cond_dim)
             )
 
         # attention related params
 
-        attn_kwargs = dict(heads = attn_heads, dim_head = attn_dim_head, cosine_sim_attn = cosine_sim_attn)
+        attn_kwargs = dict(heads = attn_heads, dim_head = attn_dim_head)
 
         num_layers = len(in_out)
 
         # resnet block klass
 
         num_resnet_blocks = cast_tuple(num_resnet_blocks, num_layers)
-        resnet_groups = cast_tuple(resnet_groups, num_layers)
 
         resnet_klass = partial(ResnetBlock, **attn_kwargs)
 
         layer_attns = cast_tuple(layer_attns, num_layers)
         layer_attns_depth = cast_tuple(layer_attns_depth, num_layers)
         layer_cross_attns = cast_tuple(layer_cross_attns, num_layers)
 
-        assert all([layers == num_layers for layers in list(map(len, (resnet_groups, layer_attns, layer_cross_attns)))])
+        use_linear_attn = cast_tuple(use_linear_attn, num_layers)
+        use_linear_cross_attn = cast_tuple(use_linear_cross_attn, num_layers)
+
+        assert all([layers == num_layers for layers in list(map(len, (layer_attns, layer_cross_attns)))])
 
         # downsample klass
 
         downsample_klass = Downsample
 
         if cross_embed_downsample:
             downsample_klass = partial(CrossEmbedLayer, kernel_sizes = cross_embed_downsample_kernel_sizes)
 
         # initial resnet block (for memory efficient unet)
 
-        self.init_resnet_block = resnet_klass(init_dim, init_dim, time_cond_dim = time_cond_dim, groups = resnet_groups[0], use_gca = use_global_context_attn) if memory_efficient else None
+        self.init_resnet_block = resnet_klass(init_dim, init_dim, time_cond_dim = time_cond_dim, use_gca = use_global_context_attn) if memory_efficient else None
 
         # scale for resnet skip connections
 
         self.skip_connect_scale = 1. if not scale_skip_connection else (2 ** -0.5)
 
         # layers
 
         self.downs = nn.ModuleList([])
         self.ups = nn.ModuleList([])
         num_resolutions = len(in_out)
 
-        layer_params = [num_resnet_blocks, resnet_groups, layer_attns, layer_attns_depth, layer_cross_attns]
+        layer_params = [num_resnet_blocks, layer_attns, layer_attns_depth, layer_cross_attns, use_linear_attn, use_linear_cross_attn]
         reversed_layer_params = list(map(reversed, layer_params))
 
         # downsampling layers
 
         skip_connect_dims = [] # keep track of skip connection dimensions
 
-        for ind, ((dim_in, dim_out), layer_num_resnet_blocks, groups, layer_attn, layer_attn_depth, layer_cross_attn) in enumerate(zip(in_out, *layer_params)):
+        for ind, ((dim_in, dim_out), layer_num_resnet_blocks, layer_attn, layer_attn_depth, layer_cross_attn, layer_use_linear_attn, layer_use_linear_cross_attn) in enumerate(zip(in_out, *layer_params)):
             is_last = ind >= (num_resolutions - 1)
 
-            layer_use_linear_cross_attn = not layer_cross_attn and use_linear_cross_attn
             layer_cond_dim = cond_dim if layer_cross_attn or layer_use_linear_cross_attn else None
 
-            transformer_block_klass = TransformerBlock if layer_attn else (LinearAttentionTransformerBlock if use_linear_attn else Identity)
+            if layer_attn:
+                transformer_block_klass = TransformerBlock
+            elif layer_use_linear_attn:
+                transformer_block_klass = LinearAttentionTransformerBlock
+            else:
+                transformer_block_klass = Identity
 
             current_dim = dim_in
 
             # whether to pre-downsample, from memory efficient unet
 
             pre_downsample = None
 
@@ -1317,49 +1363,55 @@
 
             post_downsample = None
             if not memory_efficient:
                 post_downsample = downsample_klass(current_dim, dim_out) if not is_last else Parallel(nn.Conv2d(dim_in, dim_out, 3, padding = 1), nn.Conv2d(dim_in, dim_out, 1))
 
             self.downs.append(nn.ModuleList([
                 pre_downsample,
-                resnet_klass(current_dim, current_dim, cond_dim = layer_cond_dim, linear_attn = layer_use_linear_cross_attn, time_cond_dim = time_cond_dim, groups = groups),
-                nn.ModuleList([ResnetBlock(current_dim, current_dim, time_cond_dim = time_cond_dim, groups = groups, use_gca = use_global_context_attn) for _ in range(layer_num_resnet_blocks)]),
+                resnet_klass(current_dim, current_dim, cond_dim = layer_cond_dim, linear_attn = layer_use_linear_cross_attn, time_cond_dim = time_cond_dim),
+                nn.ModuleList([ResnetBlock(current_dim, current_dim, time_cond_dim = time_cond_dim, use_gca = use_global_context_attn) for _ in range(layer_num_resnet_blocks)]),
                 transformer_block_klass(dim = current_dim, depth = layer_attn_depth, ff_mult = ff_mult, context_dim = cond_dim, **attn_kwargs),
                 post_downsample
             ]))
 
         # middle layers
 
         mid_dim = dims[-1]
 
-        self.mid_block1 = ResnetBlock(mid_dim, mid_dim, cond_dim = cond_dim, time_cond_dim = time_cond_dim, groups = resnet_groups[-1])
-        self.mid_attn = EinopsToAndFrom('b c h w', 'b (h w) c', Residual(Attention(mid_dim, **attn_kwargs))) if attend_at_middle else None
-        self.mid_block2 = ResnetBlock(mid_dim, mid_dim, cond_dim = cond_dim, time_cond_dim = time_cond_dim, groups = resnet_groups[-1])
+        self.mid_block1 = ResnetBlock(mid_dim, mid_dim, cond_dim = cond_dim, time_cond_dim = time_cond_dim)
+        self.mid_attn = TransformerBlock(mid_dim, depth = layer_mid_attns_depth, **attn_kwargs) if attend_at_middle else None
+        self.mid_block2 = ResnetBlock(mid_dim, mid_dim, cond_dim = cond_dim, time_cond_dim = time_cond_dim)
 
         # upsample klass
 
         upsample_klass = Upsample if not pixel_shuffle_upsample else PixelShuffleUpsample
 
         # upsampling layers
 
         upsample_fmap_dims = []
 
-        for ind, ((dim_in, dim_out), layer_num_resnet_blocks, groups, layer_attn, layer_attn_depth, layer_cross_attn) in enumerate(zip(reversed(in_out), *reversed_layer_params)):
+        for ind, ((dim_in, dim_out), layer_num_resnet_blocks, layer_attn, layer_attn_depth, layer_cross_attn, layer_use_linear_attn, layer_use_linear_cross_attn) in enumerate(zip(reversed(in_out), *reversed_layer_params)):
             is_last = ind == (len(in_out) - 1)
-            layer_use_linear_cross_attn = not layer_cross_attn and use_linear_cross_attn
+
             layer_cond_dim = cond_dim if layer_cross_attn or layer_use_linear_cross_attn else None
-            transformer_block_klass = TransformerBlock if layer_attn else (LinearAttentionTransformerBlock if use_linear_attn else Identity)
+
+            if layer_attn:
+                transformer_block_klass = TransformerBlock
+            elif layer_use_linear_attn:
+                transformer_block_klass = LinearAttentionTransformerBlock
+            else:
+                transformer_block_klass = Identity
 
             skip_connect_dim = skip_connect_dims.pop()
 
             upsample_fmap_dims.append(dim_out)
 
             self.ups.append(nn.ModuleList([
-                resnet_klass(dim_out + skip_connect_dim, dim_out, cond_dim = layer_cond_dim, linear_attn = layer_use_linear_cross_attn, time_cond_dim = time_cond_dim, groups = groups),
-                nn.ModuleList([ResnetBlock(dim_out + skip_connect_dim, dim_out, time_cond_dim = time_cond_dim, groups = groups, use_gca = use_global_context_attn) for _ in range(layer_num_resnet_blocks)]),
+                resnet_klass(dim_out + skip_connect_dim, dim_out, cond_dim = layer_cond_dim, linear_attn = layer_use_linear_cross_attn, time_cond_dim = time_cond_dim),
+                nn.ModuleList([ResnetBlock(dim_out + skip_connect_dim, dim_out, time_cond_dim = time_cond_dim, use_gca = use_global_context_attn) for _ in range(layer_num_resnet_blocks)]),
                 transformer_block_klass(dim = dim_out, depth = layer_attn_depth, ff_mult = ff_mult, context_dim = cond_dim, **attn_kwargs),
                 upsample_klass(dim_out, dim_in) if not is_last or memory_efficient else Identity()
             ]))
 
         # whether to combine feature maps from all upsample blocks before final resnet block out
 
         self.upsample_combiner = UpsampleCombiner(
@@ -1372,23 +1424,27 @@
         # whether to do a final residual from initial conv to the final resnet block out
 
         self.init_conv_to_final_conv_residual = init_conv_to_final_conv_residual
         final_conv_dim = self.upsample_combiner.dim_out + (dim if init_conv_to_final_conv_residual else 0)
 
         # final optional resnet block and convolution out
 
-        self.final_res_block = ResnetBlock(final_conv_dim, dim, time_cond_dim = time_cond_dim, groups = resnet_groups[0], use_gca = True) if final_resnet_block else None
+        self.final_res_block = ResnetBlock(final_conv_dim, dim, time_cond_dim = time_cond_dim, use_gca = True) if final_resnet_block else None
 
         final_conv_dim_in = dim if final_resnet_block else final_conv_dim
         final_conv_dim_in += (channels if lowres_cond else 0)
 
         self.final_conv = nn.Conv2d(final_conv_dim_in, self.channels_out, final_conv_kernel_size, padding = final_conv_kernel_size // 2)
 
         zero_init_(self.final_conv)
 
+        # resize mode
+
+        self.resize_mode = resize_mode
+
     # if the current settings for the unet are not correct
     # for cascading DDPM, then reinit the unet with the right settings
     def cast_model_parameters(
         self,
         *,
         lowres_cond,
         text_embed_dim,
@@ -1496,15 +1552,15 @@
 
         # condition on input image
 
         assert not (self.has_cond_image ^ exists(cond_images)), 'you either requested to condition on an image on the unet, but the conditioning image is not supplied, or vice versa'
 
         if exists(cond_images):
             assert cond_images.shape[1] == self.cond_images_channels, 'the number of channels on the conditioning image you are passing in does not match what you specified on initialiation of the unet'
-            cond_images = resize_image_to(cond_images, x.shape[-1])
+            cond_images = resize_image_to(cond_images, x.shape[-1], mode = self.resize_mode)
             x = torch.cat((cond_images, x), dim = 1)
 
         # initial convolution
 
         x = self.init_conv(x)
 
         # init conv residual
@@ -1546,15 +1602,15 @@
             text_keep_mask_hidden = rearrange(text_keep_mask, 'b -> b 1')
 
             # calculate text embeds
 
             text_tokens = self.text_to_cond(text_embeds)
 
             text_tokens = text_tokens[:, :self.max_text_len]
-            
+
             if exists(text_mask):
                 text_mask = text_mask[:, :self.max_text_len]
 
             text_tokens_len = text_tokens.shape[1]
             remainder = self.max_text_len - text_tokens_len
 
             if remainder > 0:
@@ -1744,19 +1800,22 @@
         pred_objectives = 'noise',
         random_crop_sizes = None,
         lowres_noise_schedule = 'linear',
         lowres_sample_noise_level = 0.2,            # in the paper, they present a new trick where they noise the lowres conditioning image, and at sample time, fix it to a certain level (0.1 or 0.3) - the unets are also made to be conditioned on this noise level
         per_sample_random_aug_noise_level = False,  # unclear when conditioning on augmentation noise level, whether each batch element receives a random aug noise value - turning off due to @marunine's find
         condition_on_text = True,
         auto_normalize_img = True,                  # whether to take care of normalizing the image from [0, 1] to [-1, 1] and back automatically - you can turn this off if you want to pass in the [-1, 1] ranged image yourself from the dataloader
-        p2_loss_weight_gamma = 0.5,                 # p2 loss weight, from https://arxiv.org/abs/2204.00227 - 0 is equivalent to weight of 1 across time
-        p2_loss_weight_k = 1,
         dynamic_thresholding = True,
         dynamic_thresholding_percentile = 0.95,     # unsure what this was based on perusal of paper
-        only_train_unet_number = None
+        only_train_unet_number = None,
+        temporal_downsample_factor = 1,
+        resize_cond_video_frames = True,
+        resize_mode = 'nearest',
+        min_snr_loss_weight = True,                 # https://arxiv.org/abs/2303.09556
+        min_snr_gamma = 5
     ):
         super().__init__()
 
         # loss
 
         if loss_type == 'l1':
             loss_fn = F.l1_loss
@@ -1856,15 +1915,28 @@
 
         # determine whether we are training on images or video
 
         is_video = any([isinstance(unet, Unet3D) for unet in self.unets])
         self.is_video = is_video
 
         self.right_pad_dims_to_datatype = partial(rearrange, pattern = ('b -> b 1 1 1' if not is_video else 'b -> b 1 1 1 1'))
+
         self.resize_to = resize_video_to if is_video else resize_image_to
+        self.resize_to = partial(self.resize_to, mode = resize_mode)
+
+        # temporal interpolation
+
+        temporal_downsample_factor = cast_tuple(temporal_downsample_factor, num_unets)
+        self.temporal_downsample_factor = temporal_downsample_factor
+
+        self.resize_cond_video_frames = resize_cond_video_frames
+        self.temporal_downsample_divisor = temporal_downsample_factor[0]
+
+        assert temporal_downsample_factor[-1] == 1, 'downsample factor of last stage must be 1'
+        assert tuple(sorted(temporal_downsample_factor, reverse = True)) == temporal_downsample_factor, 'temporal downsample factor must be in order of descending'
 
         # cascading ddpm related stuff
 
         lowres_conditions = tuple(map(lambda t: t.lowres_cond, self.unets))
         assert lowres_conditions == (False, *((True,) * (num_unets - 1))), 'the first unet must be unconditioned (by low resolution image), and the rest of the unets must have `lowres_cond` set to True'
 
         self.lowres_sample_noise_level = lowres_sample_noise_level
@@ -1882,29 +1954,37 @@
         self.input_image_range = (0. if auto_normalize_img else -1., 1.)
 
         # dynamic thresholding
 
         self.dynamic_thresholding = cast_tuple(dynamic_thresholding, num_unets)
         self.dynamic_thresholding_percentile = dynamic_thresholding_percentile
 
-        # p2 loss weight
+        # min snr loss weight
 
-        self.p2_loss_weight_k = p2_loss_weight_k
-        self.p2_loss_weight_gamma = cast_tuple(p2_loss_weight_gamma, num_unets)
+        min_snr_loss_weight = cast_tuple(min_snr_loss_weight, num_unets)
+        min_snr_gamma = cast_tuple(min_snr_gamma, num_unets)
 
-        assert all([(gamma_value <= 2) for gamma_value in self.p2_loss_weight_gamma]), 'in paper, they noticed any gamma greater than 2 is harmful'
+        assert len(min_snr_loss_weight) == len(min_snr_gamma) == num_unets
+        self.min_snr_gamma = tuple((gamma if use_min_snr else None) for use_min_snr, gamma in zip(min_snr_loss_weight, min_snr_gamma))
 
         # one temp parameter for keeping track of device
 
         self.register_buffer('_temp', torch.tensor([0.]), persistent = False)
 
         # default to device of unets passed in
 
         self.to(next(self.unets.parameters()).device)
 
+    def force_unconditional_(self):
+        self.condition_on_text = False
+        self.unconditional = True
+
+        for unet in self.unets:
+            unet.cond_on_text = False
+
     @property
     def device(self):
         return self._temp.device
 
     def get_unet(self, unet_number):
         assert 0 < unet_number <= len(self.unets)
         index = unet_number - 1
@@ -1931,16 +2011,19 @@
     @contextmanager
     def one_unet_in_gpu(self, unet_number = None, unet = None):
         assert exists(unet_number) ^ exists(unet)
 
         if exists(unet_number):
             unet = self.unets[unet_number - 1]
 
+        cpu = torch.device('cpu')
+
         devices = [module_device(unet) for unet in self.unets]
-        self.unets.cpu()
+
+        self.unets.to(cpu)
         unet.to(self.device)
 
         yield
 
         for unet, device in zip(self.unets, devices):
             unet.to(device)
 
@@ -1962,31 +2045,53 @@
         x,
         t,
         *,
         noise_scheduler,
         text_embeds = None,
         text_mask = None,
         cond_images = None,
+        cond_video_frames = None,
+        post_cond_video_frames = None,
         lowres_cond_img = None,
         self_cond = None,
         lowres_noise_times = None,
         cond_scale = 1.,
         model_output = None,
         t_next = None,
         pred_objective = 'noise',
         dynamic_threshold = True
     ):
         assert not (cond_scale != 1. and not self.can_classifier_guidance), 'imagen was not trained with conditional dropout, and thus one cannot use classifier free guidance (cond_scale anything other than 1)'
 
-        pred = default(model_output, lambda: unet.forward_with_cond_scale(x, noise_scheduler.get_condition(t), text_embeds = text_embeds, text_mask = text_mask, cond_images = cond_images, cond_scale = cond_scale, lowres_cond_img = lowres_cond_img, self_cond = self_cond, lowres_noise_times = self.lowres_noise_schedule.get_condition(lowres_noise_times)))
+        video_kwargs = dict()
+        if self.is_video:
+            video_kwargs = dict(
+                cond_video_frames = cond_video_frames,
+                post_cond_video_frames = post_cond_video_frames,
+            )
+
+        pred = default(model_output, lambda: unet.forward_with_cond_scale(
+            x,
+            noise_scheduler.get_condition(t),
+            text_embeds = text_embeds,
+            text_mask = text_mask,
+            cond_images = cond_images,
+            cond_scale = cond_scale,
+            lowres_cond_img = lowres_cond_img,
+            self_cond = self_cond,
+            lowres_noise_times = self.lowres_noise_schedule.get_condition(lowres_noise_times),
+            **video_kwargs
+        ))
 
         if pred_objective == 'noise':
             x_start = noise_scheduler.predict_start_from_noise(x, t = t, noise = pred)
         elif pred_objective == 'x_start':
             x_start = pred
+        elif pred_objective == 'v':
+            x_start = noise_scheduler.predict_start_from_v(x, t = t, v = pred)
         else:
             raise ValueError(f'unknown objective {pred_objective}')
 
         if dynamic_threshold:
             # following pseudocode in appendix
             # s is the dynamic threshold, determined by percentile of absolute values of reconstructed sample per batch element
             s = torch.quantile(
@@ -2012,23 +2117,50 @@
         t,
         *,
         noise_scheduler,
         t_next = None,
         text_embeds = None,
         text_mask = None,
         cond_images = None,
+        cond_video_frames = None,
+        post_cond_video_frames = None,
         cond_scale = 1.,
         self_cond = None,
         lowres_cond_img = None,
         lowres_noise_times = None,
         pred_objective = 'noise',
         dynamic_threshold = True
     ):
         b, *_, device = *x.shape, x.device
-        (model_mean, _, model_log_variance), x_start = self.p_mean_variance(unet, x = x, t = t, t_next = t_next, noise_scheduler = noise_scheduler, text_embeds = text_embeds, text_mask = text_mask, cond_images = cond_images, cond_scale = cond_scale, lowres_cond_img = lowres_cond_img, self_cond = self_cond, lowres_noise_times = lowres_noise_times, pred_objective = pred_objective, dynamic_threshold = dynamic_threshold)
+
+        video_kwargs = dict()
+        if self.is_video:
+            video_kwargs = dict(
+                cond_video_frames = cond_video_frames,
+                post_cond_video_frames = post_cond_video_frames,
+            )
+
+        (model_mean, _, model_log_variance), x_start = self.p_mean_variance(
+            unet,
+            x = x,
+            t = t,
+            t_next = t_next,
+            noise_scheduler = noise_scheduler,
+            text_embeds = text_embeds,
+            text_mask = text_mask,
+            cond_images = cond_images,
+            cond_scale = cond_scale,
+            lowres_cond_img = lowres_cond_img,
+            self_cond = self_cond,
+            lowres_noise_times = lowres_noise_times,
+            pred_objective = pred_objective,
+            dynamic_threshold = dynamic_threshold,
+            **video_kwargs
+        )
+
         noise = torch.randn_like(x)
         # no noise when t == 0
         is_last_sampling_timestep = (t_next == 0) if isinstance(noise_scheduler, GaussianDiffusionContinuousTimes) else (t == 0)
         nonzero_mask = (1 - is_last_sampling_timestep.float()).reshape(b, *((1,) * (len(x.shape) - 1)))
         pred = model_mean + nonzero_mask * (0.5 * model_log_variance).exp() * noise
         return pred, x_start
 
@@ -2040,65 +2172,85 @@
         *,
         noise_scheduler,
         lowres_cond_img = None,
         lowres_noise_times = None,
         text_embeds = None,
         text_mask = None,
         cond_images = None,
+        cond_video_frames = None,
+        post_cond_video_frames = None,
         inpaint_images = None,
+        inpaint_videos = None,
         inpaint_masks = None,
         inpaint_resample_times = 5,
         init_images = None,
         skip_steps = None,
         cond_scale = 1,
         pred_objective = 'noise',
         dynamic_threshold = True,
         use_tqdm = True
     ):
         device = self.device
 
         batch = shape[0]
         img = torch.randn(shape, device = device)
 
+        # video
+
+        is_video = len(shape) == 5
+        frames = shape[-3] if is_video else None
+        resize_kwargs = dict(target_frames = frames) if exists(frames) else dict()
+
         # for initialization with an image or video
 
         if exists(init_images):
             img += init_images
 
         # keep track of x0, for self conditioning
 
         x_start = None
 
         # prepare inpainting
 
+        inpaint_images = default(inpaint_videos, inpaint_images)
+
         has_inpainting = exists(inpaint_images) and exists(inpaint_masks)
         resample_times = inpaint_resample_times if has_inpainting else 1
 
         if has_inpainting:
             inpaint_images = self.normalize_img(inpaint_images)
-            inpaint_images = self.resize_to(inpaint_images, shape[-1])
-            inpaint_masks = self.resize_to(rearrange(inpaint_masks, 'b ... -> b 1 ...').float(), shape[-1]).bool()
+            inpaint_images = self.resize_to(inpaint_images, shape[-1], **resize_kwargs)
+            inpaint_masks = self.resize_to(rearrange(inpaint_masks, 'b ... -> b 1 ...').float(), shape[-1], **resize_kwargs).bool()
 
         # time
 
         timesteps = noise_scheduler.get_sampling_timesteps(batch, device = device)
 
         # whether to skip any steps
 
         skip_steps = default(skip_steps, 0)
         timesteps = timesteps[skip_steps:]
 
+        # video conditioning kwargs
+
+        video_kwargs = dict()
+        if self.is_video:
+            video_kwargs = dict(
+                cond_video_frames = cond_video_frames,
+                post_cond_video_frames = post_cond_video_frames,
+            )
+
         for times, times_next in tqdm(timesteps, desc = 'sampling loop time step', total = len(timesteps), disable = not use_tqdm):
             is_last_timestep = times_next == 0
 
             for r in reversed(range(resample_times)):
                 is_last_resample_step = r == 0
 
                 if has_inpainting:
-                    noised_inpaint_images, _ = noise_scheduler.q_sample(inpaint_images, t = times)
+                    noised_inpaint_images, *_ = noise_scheduler.q_sample(inpaint_images, t = times)
                     img = img * ~inpaint_masks + noised_inpaint_images * inpaint_masks
 
                 self_cond = x_start if unet.self_cond else None
 
                 img, x_start = self.p_sample(
                     unet,
                     img,
@@ -2109,15 +2261,16 @@
                     cond_images = cond_images,
                     cond_scale = cond_scale,
                     self_cond = self_cond,
                     lowres_cond_img = lowres_cond_img,
                     lowres_noise_times = lowres_noise_times,
                     noise_scheduler = noise_scheduler,
                     pred_objective = pred_objective,
-                    dynamic_threshold = dynamic_threshold
+                    dynamic_threshold = dynamic_threshold,
+                    **video_kwargs
                 )
 
                 if has_inpainting and not (is_last_resample_step or torch.all(is_last_timestep)):
                     renoised_img = noise_scheduler.q_sample_from_to(img, times_next, times)
 
                     img = torch.where(
                         self.right_pad_dims_to_datatype(is_last_timestep),
@@ -2133,54 +2286,73 @@
             img = img * ~inpaint_masks + inpaint_images * inpaint_masks
 
         unnormalize_img = self.unnormalize_img(img)
         return unnormalize_img
 
     @torch.no_grad()
     @eval_decorator
+    @beartype
     def sample(
         self,
-        texts: List[str] = None,
+        texts: Optional[List[str]] = None,
         text_masks = None,
         text_embeds = None,
         video_frames = None,
         cond_images = None,
+        cond_video_frames = None,
+        post_cond_video_frames = None,
+        inpaint_videos = None,
         inpaint_images = None,
         inpaint_masks = None,
         inpaint_resample_times = 5,
         init_images = None,
         skip_steps = None,
         batch_size = 1,
         cond_scale = 1.,
         lowres_sample_noise_level = None,
         start_at_unet_number = 1,
         start_image_or_video = None,
         stop_at_unet_number = None,
         return_all_unet_outputs = False,
         return_pil_images = False,
         device = None,
-        use_tqdm = True
+        use_tqdm = True,
+        use_one_unet_in_gpu = True
     ):
         device = default(device, self.device)
         self.reset_unets_all_one_device(device = device)
 
         cond_images = maybe(cast_uint8_images_to_float)(cond_images)
 
         if exists(texts) and not exists(text_embeds) and not self.unconditional:
+            assert all([*map(len, texts)]), 'text cannot be empty'
+
             with autocast(enabled = False):
                 text_embeds, text_masks = self.encode_text(texts, return_attn_mask = True)
 
             text_embeds, text_masks = map(lambda t: t.to(device), (text_embeds, text_masks))
 
         if not self.unconditional:
-            text_masks = default(text_masks, lambda: torch.any(text_embeds != 0., dim = -1))
+            assert exists(text_embeds), 'text must be passed in if the network was not trained without text `condition_on_text` must be set to `False` when training'
 
-        if not self.unconditional:
+            text_masks = default(text_masks, lambda: torch.any(text_embeds != 0., dim = -1))
             batch_size = text_embeds.shape[0]
 
+        # inpainting
+
+        inpaint_images = default(inpaint_videos, inpaint_images)
+
+        if exists(inpaint_images):
+            if self.unconditional:
+                if batch_size == 1: # assume researcher wants to broadcast along inpainted images
+                    batch_size = inpaint_images.shape[0]
+
+            assert inpaint_images.shape[0] == batch_size, 'number of inpainting images must be equal to the specified batch size on sample `sample(batch_size=<int>)``'
+            assert not (self.condition_on_text and inpaint_images.shape[0] != text_embeds.shape[0]), 'number of inpainting images must be equal to the number of text to be conditioned on'
+
         assert not (self.condition_on_text and not exists(text_embeds)), 'text or text encodings must be passed into imagen if specified'
         assert not (not self.condition_on_text and exists(text_embeds)), 'imagen specified not to be conditioned on text, yet it is presented'
         assert not (exists(text_embeds) and text_embeds.shape[-1] != self.text_embed_dim), f'invalid text embedding dimension being passed in (should be {self.text_embed_dim})'
 
         assert not (exists(inpaint_images) ^ exists(inpaint_masks)),  'inpaint images and masks must be both passed in to do inpainting'
 
         outputs = []
@@ -2194,17 +2366,27 @@
 
         # condition scaling
 
         cond_scale = cast_tuple(cond_scale, num_unets)
 
         # add frame dimension for video
 
+        if self.is_video and exists(inpaint_images):
+            video_frames = inpaint_images.shape[2]
+
+            if inpaint_masks.ndim == 3:
+                inpaint_masks = repeat(inpaint_masks, 'b h w -> b f h w', f = video_frames)
+
+            assert inpaint_masks.shape[1] == video_frames
+
         assert not (self.is_video and not exists(video_frames)), 'video_frames must be passed in on sample time if training on video'
 
-        frame_dims = (video_frames,) if self.is_video else tuple()
+        all_frame_dims = calc_all_frame_dims(self.temporal_downsample_factor, video_frames)
+
+        frames_to_resize_kwargs = lambda frames: dict(target_frames = frames) if exists(frames) else dict()
 
         # for initial image and skipping steps
 
         init_images = cast_tuple(init_images, num_unets)
         init_images = [maybe(self.normalize_img)(init_image) for init_image in init_images]
 
         skip_steps = cast_tuple(skip_steps, num_unets)
@@ -2213,41 +2395,69 @@
 
         if start_at_unet_number > 1:
             assert start_at_unet_number <= num_unets, 'must start a unet that is less than the total number of unets'
             assert not exists(stop_at_unet_number) or start_at_unet_number <= stop_at_unet_number
             assert exists(start_image_or_video), 'starting image or video must be supplied if only doing upscaling'
 
             prev_image_size = self.image_sizes[start_at_unet_number - 2]
-            img = self.resize_to(start_image_or_video, prev_image_size)
+            prev_frame_size = all_frame_dims[start_at_unet_number - 2][0] if self.is_video else None
+            img = self.resize_to(start_image_or_video, prev_image_size, **frames_to_resize_kwargs(prev_frame_size))
+
 
         # go through each unet in cascade
 
-        for unet_number, unet, channel, image_size, noise_scheduler, pred_objective, dynamic_threshold, unet_cond_scale, unet_init_images, unet_skip_steps in tqdm(zip(range(1, num_unets + 1), self.unets, self.sample_channels, self.image_sizes, self.noise_schedulers, self.pred_objectives, self.dynamic_thresholding, cond_scale, init_images, skip_steps), disable = not use_tqdm):
+        for unet_number, unet, channel, image_size, frame_dims, noise_scheduler, pred_objective, dynamic_threshold, unet_cond_scale, unet_init_images, unet_skip_steps in tqdm(zip(range(1, num_unets + 1), self.unets, self.sample_channels, self.image_sizes, all_frame_dims, self.noise_schedulers, self.pred_objectives, self.dynamic_thresholding, cond_scale, init_images, skip_steps), disable = not use_tqdm):
 
             if unet_number < start_at_unet_number:
                 continue
 
             assert not isinstance(unet, NullUnet), 'one cannot sample from null / placeholder unets'
 
-            context = self.one_unet_in_gpu(unet = unet) if is_cuda else nullcontext()
+            context = self.one_unet_in_gpu(unet = unet) if is_cuda and use_one_unet_in_gpu else nullcontext()
 
             with context:
+                # video kwargs
+
+                video_kwargs = dict()
+                if self.is_video:
+                    video_kwargs = dict(
+                        cond_video_frames = cond_video_frames,
+                        post_cond_video_frames = post_cond_video_frames,
+                    )
+
+                    video_kwargs = compact(video_kwargs)
+
+                if self.is_video and self.resize_cond_video_frames:
+                    downsample_scale = self.temporal_downsample_factor[unet_number - 1]
+                    temporal_downsample_fn = partial(scale_video_time, downsample_scale = downsample_scale)
+
+                    video_kwargs = maybe_transform_dict_key(video_kwargs, 'cond_video_frames', temporal_downsample_fn)
+                    video_kwargs = maybe_transform_dict_key(video_kwargs, 'post_cond_video_frames', temporal_downsample_fn)
+
+                # low resolution conditioning
+
                 lowres_cond_img = lowres_noise_times = None
                 shape = (batch_size, channel, *frame_dims, image_size, image_size)
 
+                resize_kwargs = dict(target_frames = frame_dims[0]) if self.is_video else dict()
+
                 if unet.lowres_cond:
                     lowres_noise_times = self.lowres_noise_schedule.get_times(batch_size, lowres_sample_noise_level, device = device)
 
-                    lowres_cond_img = self.resize_to(img, image_size)
+                    lowres_cond_img = self.resize_to(img, image_size, **resize_kwargs)
 
                     lowres_cond_img = self.normalize_img(lowres_cond_img)
-                    lowres_cond_img, _ = self.lowres_noise_schedule.q_sample(x_start = lowres_cond_img, t = lowres_noise_times, noise = torch.randn_like(lowres_cond_img))
+                    lowres_cond_img, *_ = self.lowres_noise_schedule.q_sample(x_start = lowres_cond_img, t = lowres_noise_times, noise = torch.randn_like(lowres_cond_img))
+
+                # init images or video
 
                 if exists(unet_init_images):
-                    unet_init_images = self.resize_to(unet_init_images, image_size)
+                    unet_init_images = self.resize_to(unet_init_images, image_size, **resize_kwargs)
+
+                # shape of stage
 
                 shape = (batch_size, self.channels, *frame_dims, image_size, image_size)
 
                 img = self.p_sample_loop(
                     unet,
                     shape,
                     text_embeds = text_embeds,
@@ -2260,15 +2470,16 @@
                     skip_steps = unet_skip_steps,
                     cond_scale = unet_cond_scale,
                     lowres_cond_img = lowres_cond_img,
                     lowres_noise_times = lowres_noise_times,
                     noise_scheduler = noise_scheduler,
                     pred_objective = pred_objective,
                     dynamic_threshold = dynamic_threshold,
-                    use_tqdm = use_tqdm
+                    use_tqdm = use_tqdm,
+                    **video_kwargs
                 )
 
                 outputs.append(img)
 
             if exists(stop_at_unet_number) and stop_at_unet_number == unet_number:
                 break
 
@@ -2282,31 +2493,33 @@
 
         assert not self.is_video, 'converting sampled video tensor to video file is not supported yet'
 
         pil_images = list(map(lambda img: list(map(T.ToPILImage(), img.unbind(dim = 0))), outputs))
 
         return pil_images[output_index] # now you have a bunch of pillow images you can just .save(/where/ever/you/want.png)
 
+    @beartype
     def p_losses(
         self,
-        unet,
+        unet: Union[Unet, Unet3D, NullUnet, DistributedDataParallel],
         x_start,
         times,
         *,
         noise_scheduler,
         lowres_cond_img = None,
         lowres_aug_times = None,
         text_embeds = None,
         text_mask = None,
         cond_images = None,
         noise = None,
         times_next = None,
         pred_objective = 'noise',
-        p2_loss_weight_gamma = 0.,
-        random_crop_size = None
+        min_snr_gamma = None,
+        random_crop_size = None,
+        **kwargs
     ):
         is_video = x_start.ndim == 5
 
         noise = default(noise, lambda: torch.randn_like(x_start))
 
         # normalize to [-1, 1]
 
@@ -2315,57 +2528,63 @@
 
         # random cropping during training
         # for upsamplers
 
         if exists(random_crop_size):
             if is_video:
                 frames = x_start.shape[2]
-                x_start, lowres_cond_img, noise = rearrange_many((x_start, lowres_cond_img, noise), 'b c f h w -> (b f) c h w')
+                x_start, lowres_cond_img, noise = map(lambda t: rearrange(t, 'b c f h w -> (b f) c h w'), (x_start, lowres_cond_img, noise))
 
             aug = K.RandomCrop((random_crop_size, random_crop_size), p = 1.)
 
             # make sure low res conditioner and image both get augmented the same way
             # detailed https://kornia.readthedocs.io/en/latest/augmentation.module.html?highlight=randomcrop#kornia.augmentation.RandomCrop
             x_start = aug(x_start)
             lowres_cond_img = aug(lowres_cond_img, params = aug._params)
             noise = aug(noise, params = aug._params)
 
             if is_video:
-                x_start, lowres_cond_img, noise = rearrange_many((x_start, lowres_cond_img, noise), '(b f) c h w -> b c f h w', f = frames)
+                x_start, lowres_cond_img, noise = map(lambda t: rearrange(t, '(b f) c h w -> b c f h w', f = frames), (x_start, lowres_cond_img, noise))
 
         # get x_t
 
-        x_noisy, log_snr = noise_scheduler.q_sample(x_start = x_start, t = times, noise = noise)
+        x_noisy, log_snr, alpha, sigma = noise_scheduler.q_sample(x_start = x_start, t = times, noise = noise)
 
         # also noise the lowres conditioning image
         # at sample time, they then fix the noise level of 0.1 - 0.3
 
         lowres_cond_img_noisy = None
         if exists(lowres_cond_img):
             lowres_aug_times = default(lowres_aug_times, times)
-            lowres_cond_img_noisy, _ = self.lowres_noise_schedule.q_sample(x_start = lowres_cond_img, t = lowres_aug_times, noise = torch.randn_like(lowres_cond_img))
+            lowres_cond_img_noisy, *_ = self.lowres_noise_schedule.q_sample(x_start = lowres_cond_img, t = lowres_aug_times, noise = torch.randn_like(lowres_cond_img))
 
         # time condition
 
         noise_cond = noise_scheduler.get_condition(times)
 
         # unet kwargs
 
         unet_kwargs = dict(
             text_embeds = text_embeds,
             text_mask = text_mask,
             cond_images = cond_images,
             lowres_noise_times = self.lowres_noise_schedule.get_condition(lowres_aug_times),
             lowres_cond_img = lowres_cond_img_noisy,
             cond_drop_prob = self.cond_drop_prob,
+            **kwargs
         )
 
         # self condition if needed
 
-        if unet.self_cond and random() < 0.5:
+        # Because 'unet' can be an instance of DistributedDataParallel coming from the
+        # ImagenTrainer.unet_being_trained when invoking ImagenTrainer.forward(), we need to
+        # access the member 'module' of the wrapped unet instance.
+        self_cond = unet.module.self_cond if isinstance(unet, DistributedDataParallel) else unet.self_cond
+
+        if self_cond and random() < 0.5:
             with torch.no_grad():
                 pred = unet.forward(
                     x_noisy,
                     noise_cond,
                     **unet_kwargs
                 ).detach()
 
@@ -2383,71 +2602,101 @@
 
         # prediction objective
 
         if pred_objective == 'noise':
             target = noise
         elif pred_objective == 'x_start':
             target = x_start
+        elif pred_objective == 'v':
+            # derivation detailed in Appendix D of Progressive Distillation paper
+            # https://arxiv.org/abs/2202.00512
+            # this makes distillation viable as well as solve an issue with color shifting in upresoluting unets, noted in imagen-video
+            target = alpha * noise - sigma * x_start
         else:
             raise ValueError(f'unknown objective {pred_objective}')
 
         # losses
 
         losses = self.loss_fn(pred, target, reduction = 'none')
         losses = reduce(losses, 'b ... -> b', 'mean')
 
-        # p2 loss reweighting
+        # min snr loss reweighting
+
+        snr = log_snr.exp()
+        maybe_clipped_snr = snr.clone()
 
-        if p2_loss_weight_gamma > 0:
-            loss_weight = (self.p2_loss_weight_k + log_snr.exp()) ** -p2_loss_weight_gamma
-            losses = losses * loss_weight
+        if exists(min_snr_gamma):
+            maybe_clipped_snr.clamp_(max = min_snr_gamma)
 
+        if pred_objective == 'noise':
+            loss_weight = maybe_clipped_snr / snr
+        elif pred_objective == 'x_start':
+            loss_weight = maybe_clipped_snr
+        elif pred_objective == 'v':
+            loss_weight = maybe_clipped_snr / (snr + 1)
+
+        losses = losses * loss_weight
         return losses.mean()
 
+    @beartype
     def forward(
         self,
-        images,
-        unet: Union[Unet, Unet3D, NullUnet] = None,
-        texts: List[str] = None,
+        images, # rename to images or video
+        unet: Union[Unet, Unet3D, NullUnet, DistributedDataParallel] = None,
+        texts: Optional[List[str]] = None,
         text_embeds = None,
         text_masks = None,
         unet_number = None,
-        cond_images = None
+        cond_images = None,
+        **kwargs
     ):
+        if self.is_video and images.ndim == 4:
+            images = rearrange(images, 'b c h w -> b c 1 h w')
+            kwargs.update(ignore_time = True)
+
         assert images.shape[-1] == images.shape[-2], f'the images you pass in must be a square, but received dimensions of {images.shape[2]}, {images.shape[-1]}'
         assert not (len(self.unets) > 1 and not exists(unet_number)), f'you must specify which unet you want trained, from a range of 1 to {len(self.unets)}, if you are training cascading DDPM (multiple unets)'
         unet_number = default(unet_number, 1)
         assert not exists(self.only_train_unet_number) or self.only_train_unet_number == unet_number, 'you can only train on unet #{self.only_train_unet_number}'
 
         images = cast_uint8_images_to_float(images)
         cond_images = maybe(cast_uint8_images_to_float)(cond_images)
 
+        assert images.dtype == torch.float or images.dtype == torch.half, f'images tensor needs to be floats but {images.dtype} dtype found instead'
+
         unet_index = unet_number - 1
-        
+
         unet = default(unet, lambda: self.get_unet(unet_number))
 
         assert not isinstance(unet, NullUnet), 'null unet cannot and should not be trained'
 
         noise_scheduler      = self.noise_schedulers[unet_index]
-        p2_loss_weight_gamma = self.p2_loss_weight_gamma[unet_index]
+        min_snr_gamma        = self.min_snr_gamma[unet_index]
         pred_objective       = self.pred_objectives[unet_index]
         target_image_size    = self.image_sizes[unet_index]
         random_crop_size     = self.random_crop_sizes[unet_index]
         prev_image_size      = self.image_sizes[unet_index - 1] if unet_index > 0 else None
 
         b, c, *_, h, w, device, is_video = *images.shape, images.device, images.ndim == 5
 
-        check_shape(images, 'b c ...', c = self.channels)
+        assert images.shape[1] == self.channels
         assert h >= target_image_size and w >= target_image_size
 
-        frames = images.shape[2] if is_video else None
+        frames              = images.shape[2] if is_video else None
+        all_frame_dims      = tuple(safe_get_tuple_index(el, 0) for el in calc_all_frame_dims(self.temporal_downsample_factor, frames))
+        ignore_time         = kwargs.get('ignore_time', False)
+
+        target_frame_size   = all_frame_dims[unet_index] if is_video and not ignore_time else None
+        prev_frame_size     = all_frame_dims[unet_index - 1] if is_video and not ignore_time and unet_index > 0 else None
+        frames_to_resize_kwargs = lambda frames: dict(target_frames = frames) if exists(frames) else dict()
 
         times = noise_scheduler.sample_random_times(b, device = device)
 
         if exists(texts) and not exists(text_embeds) and not self.unconditional:
+            assert all([*map(len, texts)]), 'text cannot be empty'
             assert len(texts) == len(images), 'number of text captions does not match up with the number of images given'
 
             with autocast(enabled = False):
                 text_embeds, text_masks = self.encode_text(texts, return_attn_mask = True)
 
             text_embeds, text_masks = map(lambda t: t.to(images.device), (text_embeds, text_masks))
 
@@ -2455,21 +2704,31 @@
             text_masks = default(text_masks, lambda: torch.any(text_embeds != 0., dim = -1))
 
         assert not (self.condition_on_text and not exists(text_embeds)), 'text or text encodings must be passed into decoder if specified'
         assert not (not self.condition_on_text and exists(text_embeds)), 'decoder specified not to be conditioned on text, yet it is presented'
 
         assert not (exists(text_embeds) and text_embeds.shape[-1] != self.text_embed_dim), f'invalid text embedding dimension being passed in (should be {self.text_embed_dim})'
 
+        # handle video frame conditioning
+
+        if self.is_video and self.resize_cond_video_frames:
+            downsample_scale = self.temporal_downsample_factor[unet_index]
+            temporal_downsample_fn = partial(scale_video_time, downsample_scale = downsample_scale)
+            kwargs = maybe_transform_dict_key(kwargs, 'cond_video_frames', temporal_downsample_fn)
+            kwargs = maybe_transform_dict_key(kwargs, 'post_cond_video_frames', temporal_downsample_fn)
+
+        # handle low resolution conditioning
+
         lowres_cond_img = lowres_aug_times = None
         if exists(prev_image_size):
-            lowres_cond_img = self.resize_to(images, prev_image_size, clamp_range = self.input_image_range)
-            lowres_cond_img = self.resize_to(lowres_cond_img, target_image_size, clamp_range = self.input_image_range)
+            lowres_cond_img = self.resize_to(images, prev_image_size, **frames_to_resize_kwargs(prev_frame_size), clamp_range = self.input_image_range)
+            lowres_cond_img = self.resize_to(lowres_cond_img, target_image_size, **frames_to_resize_kwargs(target_frame_size), clamp_range = self.input_image_range)
 
             if self.per_sample_random_aug_noise_level:
                 lowres_aug_times = self.lowres_noise_schedule.sample_random_times(b, device = device)
             else:
                 lowres_aug_time = self.lowres_noise_schedule.sample_random_times(1, device = device)
                 lowres_aug_times = repeat(lowres_aug_time, '1 -> b', b = b)
 
-        images = self.resize_to(images, target_image_size)
+        images = self.resize_to(images, target_image_size, **frames_to_resize_kwargs(target_frame_size))
 
-        return self.p_losses(unet, images, times, text_embeds = text_embeds, text_mask = text_masks, cond_images = cond_images, noise_scheduler = noise_scheduler, lowres_cond_img = lowres_cond_img, lowres_aug_times = lowres_aug_times, pred_objective = pred_objective, p2_loss_weight_gamma = p2_loss_weight_gamma, random_crop_size = random_crop_size)
+        return self.p_losses(unet, images, times, text_embeds = text_embeds, text_mask = text_masks, cond_images = cond_images, noise_scheduler = noise_scheduler, lowres_cond_img = lowres_cond_img, lowres_aug_times = lowres_aug_times, pred_objective = pred_objective, min_snr_gamma = min_snr_gamma, random_crop_size = random_crop_size, **kwargs)
```

### Comparing `imagen-pytorch-1.9.7/imagen_pytorch/imagen_video/imagen_video.py` & `imagen_pytorch-2.0.0/imagen_pytorch/imagen_video.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 import math
-import copy
-from typing import List
-from tqdm import tqdm
+import operator
+import functools
+from tqdm.auto import tqdm
 from functools import partial, wraps
-from contextlib import contextmanager, nullcontext
-from collections import namedtuple
 from pathlib import Path
 
 import torch
 import torch.nn.functional as F
 from torch import nn, einsum
 
-from einops import rearrange, repeat, reduce
-from einops.layers.torch import Rearrange, Reduce
-from einops_exts import rearrange_many, repeat_many, check_shape
-from einops_exts.torch import EinopsToAndFrom
+from einops import rearrange, repeat, pack, unpack
+from einops.layers.torch import Rearrange
 
 from imagen_pytorch.t5 import t5_encode_text, get_encoded_dim, DEFAULT_T5_NAME
 
 # helper functions
 
 def exists(val):
     return val is not None
@@ -27,14 +23,17 @@
     return t
 
 def first(arr, d = None):
     if len(arr) == 0:
         return d
     return arr[0]
 
+def divisible_by(numer, denom):
+    return (numer % denom) == 0
+
 def maybe(fn):
     @wraps(fn)
     def inner(x):
         if not exists(x):
             return x
         return fn(x)
     return inner
@@ -101,14 +100,17 @@
 class Identity(nn.Module):
     def __init__(self, *args, **kwargs):
         super().__init__()
 
     def forward(self, x, *args, **kwargs):
         return x
 
+def Sequential(*modules):
+    return nn.Sequential(*filter(exists, modules))
+
 # tensor helpers
 
 def log(t, eps: float = 1e-12):
     return torch.log(t.clamp(min = eps))
 
 def l2norm(t):
     return F.normalize(t, dim = -1)
@@ -128,34 +130,57 @@
     masked_t = t.masked_fill(~mask, 0.)
 
     return masked_t.sum(dim = dim) / denom.clamp(min = 1e-5)
 
 def resize_video_to(
     video,
     target_image_size,
-    clamp_range = None
+    target_frames = None,
+    clamp_range = None,
+    mode = 'nearest'
 ):
     orig_video_size = video.shape[-1]
 
-    if orig_video_size == target_image_size:
-        return video
+    frames = video.shape[2]
+    target_frames = default(target_frames, frames)
 
+    target_shape = (target_frames, target_image_size, target_image_size)
 
-    frames = video.shape[2]
-    video = rearrange(video, 'b c f h w -> (b f) c h w')
+    if tuple(video.shape[-3:]) == target_shape:
+        return video
 
-    out = F.interpolate(video, target_image_size, mode = 'nearest')
+    out = F.interpolate(video, target_shape, mode = mode)
 
     if exists(clamp_range):
         out = out.clamp(*clamp_range)
-
-    out = rearrange(out, '(b f) c h w -> b c f h w', f = frames)
         
     return out
 
+def scale_video_time(
+    video,
+    downsample_scale = 1,
+    mode = 'nearest'
+):
+    if downsample_scale == 1:
+        return video
+
+    image_size, frames = video.shape[-1], video.shape[-3]
+    assert divisible_by(frames, downsample_scale), f'trying to temporally downsample a conditioning video frames of length {frames} by {downsample_scale}, however it is not neatly divisible'
+
+    target_frames = frames // downsample_scale
+
+    resized_video = resize_video_to(
+        video,
+        image_size,
+        target_frames = target_frames,
+        mode = mode
+    )
+
+    return resized_video
+
 # classifier free guidance functions
 
 def prob_mask_like(shape, prob, device):
     if prob == 1:
         return torch.ones(shape, device = device, dtype = torch.bool)
     elif prob == 0:
         return torch.zeros(shape, device = device, dtype = torch.bool)
@@ -175,14 +200,23 @@
             x = x / x.amax(dim = -1, keepdim = True).detach()
 
         eps = 1e-5 if x.dtype == torch.float32 else 1e-3
         var = torch.var(x, dim = -1, unbiased = False, keepdim = True)
         mean = torch.mean(x, dim = -1, keepdim = True)
         return (x - mean) * (var + eps).rsqrt() * self.g
 
+class ChanRMSNorm(nn.Module):
+    def __init__(self, dim):
+        super().__init__()
+        self.scale = dim ** 0.5
+        self.gamma = nn.Parameter(torch.ones(dim, 1, 1, 1))
+
+    def forward(self, x):
+        return F.normalize(x, dim = 1) * self.scale * self.gamma
+
 class ChanLayerNorm(nn.Module):
     def __init__(self, dim, stable = False):
         super().__init__()
         self.stable = stable
         self.g = nn.Parameter(torch.ones(1, dim, 1, 1, 1))
 
     def forward(self, x):
@@ -214,39 +248,57 @@
         super().__init__()
         self.fns = nn.ModuleList(fns)
 
     def forward(self, x):
         outputs = [fn(x) for fn in self.fns]
         return sum(outputs)
 
+# rearranging
+
+class RearrangeTimeCentric(nn.Module):
+    def __init__(self, fn):
+        super().__init__()
+        self.fn = fn
+
+    def forward(self, x):
+        x = rearrange(x, 'b c f ... -> b ... f c')
+        x, ps = pack([x], '* f c')
+
+        x = self.fn(x)
+
+        x, = unpack(x, ps, '* f c')
+        x = rearrange(x, 'b ... f c -> b c f ...')
+        return x
+
 # attention pooling
 
 class PerceiverAttention(nn.Module):
     def __init__(
         self,
         *,
         dim,
         dim_head = 64,
         heads = 8,
-        cosine_sim_attn = False
+        scale = 8
     ):
         super().__init__()
-        self.scale = dim_head ** -0.5 if not cosine_sim_attn else 1
-        self.cosine_sim_attn = cosine_sim_attn
-        self.cosine_sim_scale = 16 if cosine_sim_attn else 1
+        self.scale = scale
 
         self.heads = heads
         inner_dim = dim_head * heads
 
         self.norm = nn.LayerNorm(dim)
         self.norm_latents = nn.LayerNorm(dim)
 
         self.to_q = nn.Linear(dim, inner_dim, bias = False)
         self.to_kv = nn.Linear(dim, inner_dim * 2, bias = False)
 
+        self.q_scale = nn.Parameter(torch.ones(dim_head))
+        self.k_scale = nn.Parameter(torch.ones(dim_head))
+
         self.to_out = nn.Sequential(
             nn.Linear(inner_dim, dim, bias = False),
             nn.LayerNorm(dim)
         )
 
     def forward(self, x, latents, mask = None):
         x = self.norm(x)
@@ -256,26 +308,25 @@
 
         q = self.to_q(latents)
 
         # the paper differs from Perceiver in which they also concat the key / values derived from the latents to be attended to
         kv_input = torch.cat((x, latents), dim = -2)
         k, v = self.to_kv(kv_input).chunk(2, dim = -1)
 
-        q, k, v = rearrange_many((q, k, v), 'b n (h d) -> b h n d', h = h)
+        q, k, v = map(lambda t: rearrange(t, 'b n (h d) -> b h n d', h = h), (q, k, v))
 
-        q = q * self.scale
+        # qk rmsnorm
 
-        # cosine sim attention
-
-        if self.cosine_sim_attn:
-            q, k = map(l2norm, (q, k))
+        q, k = map(l2norm, (q, k))
+        q = q * self.q_scale
+        k = k * self.k_scale
 
         # similarities and masking
 
-        sim = einsum('... i d, ... j d  -> ... i j', q, k) * self.cosine_sim_scale
+        sim = einsum('... i d, ... j d  -> ... i j', q, k) * self.scale
 
         if exists(mask):
             max_neg_value = -torch.finfo(sim.dtype).max
             mask = F.pad(mask, (0, latents.shape[-2]), value = True)
             mask = rearrange(mask, 'b j -> b 1 1 j')
             sim = sim.masked_fill(~mask, max_neg_value)
 
@@ -294,16 +345,15 @@
         dim,
         depth,
         dim_head = 64,
         heads = 8,
         num_latents = 64,
         num_latents_mean_pooled = 4, # number of latents derived from mean pooled representation of the sequence
         max_seq_len = 512,
-        ff_mult = 4,
-        cosine_sim_attn = False
+        ff_mult = 4
     ):
         super().__init__()
         self.pos_emb = nn.Embedding(max_seq_len, dim)
 
         self.latents = nn.Parameter(torch.randn(num_latents, dim))
 
         self.to_latents_from_mean_pooled_seq = None
@@ -314,15 +364,15 @@
                 nn.Linear(dim, dim * num_latents_mean_pooled),
                 Rearrange('b (n d) -> b n d', n = num_latents_mean_pooled)
             )
 
         self.layers = nn.ModuleList([])
         for _ in range(depth):
             self.layers.append(nn.ModuleList([
-                PerceiverAttention(dim = dim, dim_head = dim_head, heads = heads, cosine_sim_attn = cosine_sim_attn),
+                PerceiverAttention(dim = dim, dim_head = dim_head, heads = heads),
                 FeedForward(dim = dim, mult = ff_mult)
             ]))
 
     def forward(self, x, mask = None):
         n, device = x.shape[1], x.device
         pos_emb = self.pos_emb(torch.arange(n, device = device))
 
@@ -337,86 +387,162 @@
 
         for attn, ff in self.layers:
             latents = attn(x_with_pos, latents, mask = mask) + latents
             latents = ff(latents) + latents
 
         return latents
 
+# main contribution from make-a-video - pseudo conv3d
+# axial space-time convolutions, but made causal to keep in line with the design decisions of imagen-video paper
+
+class Conv3d(nn.Module):
+    def __init__(
+        self,
+        dim,
+        dim_out = None,
+        kernel_size = 3,
+        *,
+        temporal_kernel_size = None,
+        **kwargs
+    ):
+        super().__init__()
+        dim_out = default(dim_out, dim)
+        temporal_kernel_size = default(temporal_kernel_size, kernel_size)
+
+        self.spatial_conv = nn.Conv2d(dim, dim_out, kernel_size = kernel_size, padding = kernel_size // 2)
+        self.temporal_conv = nn.Conv1d(dim_out, dim_out, kernel_size = temporal_kernel_size) if kernel_size > 1 else None
+        self.kernel_size = kernel_size
+
+        if exists(self.temporal_conv):
+            nn.init.dirac_(self.temporal_conv.weight.data) # initialized to be identity
+            nn.init.zeros_(self.temporal_conv.bias.data)
+
+    def forward(
+        self,
+        x,
+        ignore_time = False
+    ):
+        b, c, *_, h, w = x.shape
+
+        is_video = x.ndim == 5
+        ignore_time &= is_video
+
+        if is_video:
+            x = rearrange(x, 'b c f h w -> (b f) c h w')
+
+        x = self.spatial_conv(x)
+
+        if is_video:
+            x = rearrange(x, '(b f) c h w -> b c f h w', b = b)
+
+        if ignore_time or not exists(self.temporal_conv):
+            return x
+
+        x = rearrange(x, 'b c f h w -> (b h w) c f')
+
+        # causal temporal convolution - time is causal in imagen-video
+
+        if self.kernel_size > 1:
+            x = F.pad(x, (self.kernel_size - 1, 0))
+
+        x = self.temporal_conv(x)
+
+        x = rearrange(x, '(b h w) c f -> b c f h w', h = h, w = w)
+
+        return x
+
 # attention
 
 class Attention(nn.Module):
     def __init__(
         self,
         dim,
         *,
         dim_head = 64,
         heads = 8,
         causal = False,
         context_dim = None,
-        cosine_sim_attn = False
+        rel_pos_bias = False,
+        rel_pos_bias_mlp_depth = 2,
+        init_zero = False,
+        scale = 8
     ):
         super().__init__()
-        self.scale = dim_head ** -0.5 if not cosine_sim_attn else 1.
+        self.scale = scale
         self.causal = causal
 
-        self.cosine_sim_attn = cosine_sim_attn
-        self.cosine_sim_scale = 16 if cosine_sim_attn else 1
+        self.rel_pos_bias = DynamicPositionBias(dim = dim, heads = heads, depth = rel_pos_bias_mlp_depth) if rel_pos_bias else None
 
         self.heads = heads
         inner_dim = dim_head * heads
 
         self.norm = LayerNorm(dim)
 
         self.null_attn_bias = nn.Parameter(torch.randn(heads))
 
         self.null_kv = nn.Parameter(torch.randn(2, dim_head))
         self.to_q = nn.Linear(dim, inner_dim, bias = False)
         self.to_kv = nn.Linear(dim, dim_head * 2, bias = False)
 
+        self.q_scale = nn.Parameter(torch.ones(dim_head))
+        self.k_scale = nn.Parameter(torch.ones(dim_head))
+
         self.to_context = nn.Sequential(nn.LayerNorm(context_dim), nn.Linear(context_dim, dim_head * 2)) if exists(context_dim) else None
 
         self.to_out = nn.Sequential(
             nn.Linear(inner_dim, dim, bias = False),
             LayerNorm(dim)
         )
 
-    def forward(self, x, context = None, mask = None, attn_bias = None):
+        if init_zero:
+            nn.init.zeros_(self.to_out[-1].g)
+
+    def forward(
+        self,
+        x,
+        context = None,
+        mask = None,
+        attn_bias = None
+    ):
         b, n, device = *x.shape[:2], x.device
 
         x = self.norm(x)
         q, k, v = (self.to_q(x), *self.to_kv(x).chunk(2, dim = -1))
 
         q = rearrange(q, 'b n (h d) -> b h n d', h = self.heads)
-        q = q * self.scale
 
         # add null key / value for classifier free guidance in prior net
 
-        nk, nv = repeat_many(self.null_kv.unbind(dim = -2), 'd -> b 1 d', b = b)
+        nk, nv = map(lambda t: repeat(t, 'd -> b 1 d', b = b), self.null_kv.unbind(dim = -2))
         k = torch.cat((nk, k), dim = -2)
         v = torch.cat((nv, v), dim = -2)
 
         # add text conditioning, if present
 
         if exists(context):
             assert exists(self.to_context)
             ck, cv = self.to_context(context).chunk(2, dim = -1)
             k = torch.cat((ck, k), dim = -2)
             v = torch.cat((cv, v), dim = -2)
 
-        # cosine sim attention
+        # qk rmsnorm
 
-        if self.cosine_sim_attn:
-            q, k = map(l2norm, (q, k))
+        q, k = map(l2norm, (q, k))
+        q = q * self.q_scale
+        k = k * self.k_scale
 
         # calculate query / key similarities
 
-        sim = einsum('b h i d, b j d -> b h i j', q, k) * self.cosine_sim_scale
+        sim = einsum('b h i d, b j d -> b h i j', q, k) * self.scale
 
         # relative positional encoding (T5 style)
 
+        if not exists(attn_bias) and exists(self.rel_pos_bias):
+            attn_bias = self.rel_pos_bias(n, device = device, dtype = q.dtype)
+
         if exists(attn_bias):
             null_attn_bias = repeat(self.null_attn_bias, 'h -> h n 1', n = n)
             attn_bias = torch.cat((null_attn_bias, attn_bias), dim = -1)
             sim = sim + attn_bias
 
         # masking
 
@@ -509,15 +635,61 @@
         frames = x.shape[2]
         out = rearrange(out, 'b c f h w -> (b f) c h w')
         out = self.pixel_shuffle(out)
         return rearrange(out, '(b f) c h w -> b c f h w', f = frames)
 
 def Downsample(dim, dim_out = None):
     dim_out = default(dim_out, dim)
-    return Conv2d(dim, dim_out, 4, 2, 1)
+    return nn.Sequential(
+        Rearrange('b c f (h p1) (w p2) -> b (c p1 p2) f h w', p1 = 2, p2 = 2),
+        Conv2d(dim * 4, dim_out, 1)
+    )
+
+# temporal up and downsamples
+
+class TemporalPixelShuffleUpsample(nn.Module):
+    def __init__(self, dim, dim_out = None, stride = 2):
+        super().__init__()
+        self.stride = stride
+        dim_out = default(dim_out, dim)
+        conv = nn.Conv1d(dim, dim_out * stride, 1)
+
+        self.net = nn.Sequential(
+            conv,
+            nn.SiLU()
+        )
+
+        self.pixel_shuffle = Rearrange('b (c r) n -> b c (n r)', r = stride)
+
+        self.init_conv_(conv)
+
+    def init_conv_(self, conv):
+        o, i, f = conv.weight.shape
+        conv_weight = torch.empty(o // self.stride, i, f)
+        nn.init.kaiming_uniform_(conv_weight)
+        conv_weight = repeat(conv_weight, 'o ... -> (o r) ...', r = self.stride)
+
+        conv.weight.data.copy_(conv_weight)
+        nn.init.zeros_(conv.bias.data)
+
+    def forward(self, x):
+        b, c, f, h, w = x.shape
+        x = rearrange(x, 'b c f h w -> (b h w) c f')
+        out = self.net(x)
+        out = self.pixel_shuffle(out)
+        return rearrange(out, '(b h w) c f -> b c f h w', h = h, w = w)
+
+def TemporalDownsample(dim, dim_out = None, stride = 2):
+    dim_out = default(dim_out, dim)
+    return nn.Sequential(
+        Rearrange('b c (f p) h w -> b (c p) f h w', p = stride),
+        Conv2d(dim * stride, dim_out, 1)
+    )
+
+# positional embedding
 
 class SinusoidalPosEmb(nn.Module):
     def __init__(self, dim):
         super().__init__()
         self.dim = dim
 
     def forward(self, x):
@@ -542,41 +714,44 @@
         return fouriered
 
 class Block(nn.Module):
     def __init__(
         self,
         dim,
         dim_out,
-        groups = 8,
         norm = True
     ):
         super().__init__()
-        self.groupnorm = nn.GroupNorm(groups, dim) if norm else Identity()
+        self.norm = ChanRMSNorm(dim) if norm else Identity()
         self.activation = nn.SiLU()
-        self.project = Conv2d(dim, dim_out, 3, padding = 1)
+        self.project = Conv3d(dim, dim_out, 3, padding = 1)
 
-    def forward(self, x, scale_shift = None):
-        x = self.groupnorm(x)
+    def forward(
+        self,
+        x,
+        scale_shift = None,
+        ignore_time = False
+    ):
+        x = self.norm(x)
 
         if exists(scale_shift):
             scale, shift = scale_shift
             x = x * (scale + 1) + shift
 
         x = self.activation(x)
-        return self.project(x)
+        return self.project(x, ignore_time = ignore_time)
 
 class ResnetBlock(nn.Module):
     def __init__(
         self,
         dim,
         dim_out,
         *,
         cond_dim = None,
         time_cond_dim = None,
-        groups = 8,
         linear_attn = False,
         use_gca = False,
         squeeze_excite = False,
         **attn_kwargs
     ):
         super().__init__()
 
@@ -589,112 +764,120 @@
             )
 
         self.cross_attn = None
 
         if exists(cond_dim):
             attn_klass = CrossAttention if not linear_attn else LinearCrossAttention
 
-            self.cross_attn = EinopsToAndFrom(
-                'b c f h w',
-                'b (f h w) c',
-                attn_klass(
-                    dim = dim_out,
-                    context_dim = cond_dim,
-                    **attn_kwargs
-                )
+            self.cross_attn = attn_klass(
+                dim = dim_out,
+                context_dim = cond_dim,
+                **attn_kwargs
             )
 
-        self.block1 = Block(dim, dim_out, groups = groups)
-        self.block2 = Block(dim_out, dim_out, groups = groups)
+        self.block1 = Block(dim, dim_out)
+        self.block2 = Block(dim_out, dim_out)
 
         self.gca = GlobalContext(dim_in = dim_out, dim_out = dim_out) if use_gca else Always(1)
 
         self.res_conv = Conv2d(dim, dim_out, 1) if dim != dim_out else Identity()
 
 
-    def forward(self, x, time_emb = None, cond = None):
+    def forward(
+        self,
+        x,
+        time_emb = None,
+        cond = None,
+        ignore_time = False
+    ):
 
         scale_shift = None
         if exists(self.time_mlp) and exists(time_emb):
             time_emb = self.time_mlp(time_emb)
             time_emb = rearrange(time_emb, 'b c -> b c 1 1 1')
             scale_shift = time_emb.chunk(2, dim = 1)
 
-        h = self.block1(x)
+        h = self.block1(x, ignore_time = ignore_time)
 
         if exists(self.cross_attn):
             assert exists(cond)
+            h = rearrange(h, 'b c ... -> b ... c')
+            h, ps = pack([h], 'b * c')
+
             h = self.cross_attn(h, context = cond) + h
 
-        h = self.block2(h, scale_shift = scale_shift)
+            h, = unpack(h, ps, 'b * c')
+            h = rearrange(h, 'b ... c -> b c ...')
+
+        h = self.block2(h, scale_shift = scale_shift, ignore_time = ignore_time)
 
         h = h * self.gca(h)
 
         return h + self.res_conv(x)
 
 class CrossAttention(nn.Module):
     def __init__(
         self,
         dim,
         *,
         context_dim = None,
         dim_head = 64,
         heads = 8,
         norm_context = False,
-        cosine_sim_attn = False
+        scale = 8
     ):
         super().__init__()
-        self.scale = dim_head ** -0.5 if not cosine_sim_attn else 1.
-        self.cosine_sim_attn = cosine_sim_attn
-        self.cosine_sim_scale = 16 if cosine_sim_attn else 1
+        self.scale = scale
 
         self.heads = heads
         inner_dim = dim_head * heads
 
         context_dim = default(context_dim, dim)
 
         self.norm = LayerNorm(dim)
         self.norm_context = LayerNorm(context_dim) if norm_context else Identity()
 
         self.null_kv = nn.Parameter(torch.randn(2, dim_head))
         self.to_q = nn.Linear(dim, inner_dim, bias = False)
         self.to_kv = nn.Linear(context_dim, inner_dim * 2, bias = False)
 
+        self.q_scale = nn.Parameter(torch.ones(dim_head))
+        self.k_scale = nn.Parameter(torch.ones(dim_head))
+
         self.to_out = nn.Sequential(
             nn.Linear(inner_dim, dim, bias = False),
             LayerNorm(dim)
         )
 
     def forward(self, x, context, mask = None):
         b, n, device = *x.shape[:2], x.device
 
         x = self.norm(x)
         context = self.norm_context(context)
 
         q, k, v = (self.to_q(x), *self.to_kv(context).chunk(2, dim = -1))
 
-        q, k, v = rearrange_many((q, k, v), 'b n (h d) -> b h n d', h = self.heads)
+        q, k, v = map(lambda t: rearrange(t, 'b n (h d) -> b h n d', h = self.heads), (q, k, v))
 
         # add null key / value for classifier free guidance in prior net
 
-        nk, nv = repeat_many(self.null_kv.unbind(dim = -2), 'd -> b h 1 d', h = self.heads,  b = b)
+        nk, nv = map(lambda t: repeat(t, 'd -> b h 1 d', h = self.heads,  b = b), self.null_kv.unbind(dim = -2))
 
         k = torch.cat((nk, k), dim = -2)
         v = torch.cat((nv, v), dim = -2)
 
-        q = q * self.scale
+        # qk rmsnorm
 
-        # cosine sim attention
-
-        if self.cosine_sim_attn:
-            q, k = map(l2norm, (q, k))
+        q, k = map(l2norm, (q, k))
+        q = q * self.q_scale
+        k = k * self.k_scale
 
         # similarities
 
-        sim = einsum('b h i d, b h j d -> b h i j', q, k) * self.cosine_sim_scale
+        sim = einsum('b h i d, b h j d -> b h i j', q, k) * self.scale
 
         # masking
 
         max_neg_value = -torch.finfo(sim.dtype).max
 
         if exists(mask):
             mask = F.pad(mask, (1, 0), value = True)
@@ -712,19 +895,19 @@
         b, n, device = *x.shape[:2], x.device
 
         x = self.norm(x)
         context = self.norm_context(context)
 
         q, k, v = (self.to_q(x), *self.to_kv(context).chunk(2, dim = -1))
 
-        q, k, v = rearrange_many((q, k, v), 'b n (h d) -> (b h) n d', h = self.heads)
+        q, k, v = map(lambda t: rearrange(t, 'b n (h d) -> (b h) n d', h = self.heads), (q, k, v))
 
         # add null key / value for classifier free guidance in prior net
 
-        nk, nv = repeat_many(self.null_kv.unbind(dim = -2), 'd -> (b h) 1 d', h = self.heads,  b = b)
+        nk, nv = map(lambda t: repeat(t, 'd -> (b h) 1 d', h = self.heads,  b = b), self.null_kv.unbind(dim = -2))
 
         k = torch.cat((nk, k), dim = -2)
         v = torch.cat((nv, v), dim = -2)
 
         # masking
 
         max_neg_value = -torch.finfo(x.dtype).max
@@ -791,20 +974,20 @@
         )
 
     def forward(self, fmap, context = None):
         h, x, y = self.heads, *fmap.shape[-2:]
 
         fmap = self.norm(fmap)
         q, k, v = map(lambda fn: fn(fmap), (self.to_q, self.to_k, self.to_v))
-        q, k, v = rearrange_many((q, k, v), 'b (h c) x y -> (b h) (x y) c', h = h)
+        q, k, v = map(lambda t: rearrange(t, 'b (h c) x y -> (b h) (x y) c', h = h), (q, k, v))
 
         if exists(context):
             assert exists(self.to_context)
             ck, cv = self.to_context(context).chunk(2, dim = -1)
-            ck, cv = rearrange_many((ck, cv), 'b n (h d) -> (b h) n d', h = h)
+            ck, cv = map(lambda t: rearrange(t, 'b n (h d) -> (b h) n d', h = h), (ck, cv))
             k = torch.cat((k, ck), dim = -2)
             v = torch.cat((v, cv), dim = -2)
 
         q = q.softmax(dim = -1)
         k = k.softmax(dim = -2)
 
         q = q * self.scale
@@ -834,85 +1017,103 @@
             nn.SiLU(),
             Conv2d(hidden_dim, dim_out, 1),
             nn.Sigmoid()
         )
 
     def forward(self, x):
         context = self.to_k(x)
-        x, context = rearrange_many((x, context), 'b n ... -> b n (...)')
+        x, context = map(lambda t: rearrange(t, 'b n ... -> b n (...)'), (x, context))
         out = einsum('b i n, b c n -> b c i', context.softmax(dim = -1), x)
         out = rearrange(out, '... -> ... 1 1')
         return self.net(out)
 
 def FeedForward(dim, mult = 2):
     hidden_dim = int(dim * mult)
     return nn.Sequential(
         LayerNorm(dim),
         nn.Linear(dim, hidden_dim, bias = False),
         nn.GELU(),
         LayerNorm(hidden_dim),
         nn.Linear(hidden_dim, dim, bias = False)
     )
 
-def ChanFeedForward(dim, mult = 2):  # in paper, it seems for self attention layers they did feedforwards with twice channel width
+class TimeTokenShift(nn.Module):
+    def forward(self, x):
+        if x.ndim != 5:
+            return x
+
+        x, x_shift = x.chunk(2, dim = 1)
+        x_shift = F.pad(x_shift, (0, 0, 0, 0, 1, -1), value = 0.)
+        return torch.cat((x, x_shift), dim = 1)
+
+def ChanFeedForward(dim, mult = 2, time_token_shift = True):  # in paper, it seems for self attention layers they did feedforwards with twice channel width
     hidden_dim = int(dim * mult)
-    return nn.Sequential(
+    return Sequential(
         ChanLayerNorm(dim),
         Conv2d(dim, hidden_dim, 1, bias = False),
         nn.GELU(),
+        TimeTokenShift() if time_token_shift else None,
         ChanLayerNorm(hidden_dim),
         Conv2d(hidden_dim, dim, 1, bias = False)
     )
 
 class TransformerBlock(nn.Module):
     def __init__(
         self,
         dim,
         *,
         depth = 1,
         heads = 8,
         dim_head = 32,
         ff_mult = 2,
-        context_dim = None,
-        cosine_sim_attn = False
+        ff_time_token_shift = True,
+        context_dim = None
     ):
         super().__init__()
         self.layers = nn.ModuleList([])
 
         for _ in range(depth):
             self.layers.append(nn.ModuleList([
-                EinopsToAndFrom('b c f h w', 'b (f h w) c', Attention(dim = dim, heads = heads, dim_head = dim_head, context_dim = context_dim, cosine_sim_attn = cosine_sim_attn)),
-                ChanFeedForward(dim = dim, mult = ff_mult)
+                Attention(dim = dim, heads = heads, dim_head = dim_head, context_dim = context_dim),
+                ChanFeedForward(dim = dim, mult = ff_mult, time_token_shift = ff_time_token_shift)
             ]))
 
     def forward(self, x, context = None):
         for attn, ff in self.layers:
+            x = rearrange(x, 'b c ... -> b ... c')
+            x, ps = pack([x], 'b * c')
+
             x = attn(x, context = context) + x
+
+            x, = unpack(x, ps, 'b * c')
+            x = rearrange(x, 'b ... c -> b c ...')
+
             x = ff(x) + x
         return x
 
 class LinearAttentionTransformerBlock(nn.Module):
     def __init__(
         self,
         dim,
         *,
         depth = 1,
         heads = 8,
         dim_head = 32,
         ff_mult = 2,
+        ff_time_token_shift = True,
         context_dim = None,
         **kwargs
     ):
         super().__init__()
         self.layers = nn.ModuleList([])
 
         for _ in range(depth):
             self.layers.append(nn.ModuleList([
                 LinearAttention(dim = dim, heads = heads, dim_head = dim_head, context_dim = context_dim),
-                ChanFeedForward(dim = dim, mult = ff_mult)
+                ChanFeedForward(dim = dim, mult = ff_mult, time_token_shift = ff_time_token_shift)
             ]))
 
     def forward(self, x, context = None):
         for attn, ff in self.layers:
             x = attn(x, context = context) + x
             x = ff(x) + x
         return x
@@ -1022,61 +1223,61 @@
         return bias
 
 class Unet3D(nn.Module):
     def __init__(
         self,
         *,
         dim,
-        image_embed_dim = 1024,
         text_embed_dim = get_encoded_dim(DEFAULT_T5_NAME),
         num_resnet_blocks = 1,
         cond_dim = None,
         num_image_tokens = 4,
         num_time_tokens = 2,
         learned_sinu_pos_emb_dim = 16,
         out_dim = None,
-        dim_mults=(1, 2, 4, 8),
+        dim_mults = (1, 2, 4, 8),
+        temporal_strides = 1,
         cond_images_channels = 0,
         channels = 3,
         channels_out = None,
         attn_dim_head = 64,
         attn_heads = 8,
         ff_mult = 2.,
+        ff_time_token_shift = True,         # this would do a token shift along time axis, at the hidden layer within feedforwards - from successful use in RWKV (Peng et al), and other token shift video transformer works
         lowres_cond = False,                # for cascading diffusion - https://cascaded-diffusion.github.io/
         layer_attns = False,
         layer_attns_depth = 1,
         layer_attns_add_text_cond = True,   # whether to condition the self-attention blocks with the text embeddings, as described in Appendix D.3.1
         attend_at_middle = True,            # whether to have a layer of attention at the bottleneck (can turn off for higher resolution in cascading DDPM, before bringing in efficient attention)
         time_rel_pos_bias_depth = 2,
         time_causal_attn = True,
         layer_cross_attns = True,
         use_linear_attn = False,
         use_linear_cross_attn = False,
         cond_on_text = True,
         max_text_len = 256,
         init_dim = None,
-        resnet_groups = 8,
         init_conv_kernel_size = 7,          # kernel size of initial conv, if not using cross embed
         init_cross_embed = True,
         init_cross_embed_kernel_sizes = (3, 7, 15),
         cross_embed_downsample = False,
         cross_embed_downsample_kernel_sizes = (2, 4),
         attn_pool_text = True,
         attn_pool_num_latents = 32,
         dropout = 0.,
         memory_efficient = False,
         init_conv_to_final_conv_residual = False,
         use_global_context_attn = True,
         scale_skip_connection = True,
         final_resnet_block = True,
         final_conv_kernel_size = 3,
-        cosine_sim_attn = False,
         self_cond = False,
         combine_upsample_fmaps = False,      # combine feature maps from all upsample blocks, used in unet squared successfully
-        pixel_shuffle_upsample = True        # may address checkboard artifacts
+        pixel_shuffle_upsample = True,       # may address checkboard artifacts
+        resize_mode = 'nearest'
     ):
         super().__init__()
 
         # guide researchers
 
         assert attn_heads > 1, 'you need to have more than 1 attention head, ideally at least 4 or 8'
 
@@ -1176,15 +1377,15 @@
 
         # finer control over whether to condition on text encodings
 
         self.cond_on_text = cond_on_text
 
         # attention pooling
 
-        self.attn_pool = PerceiverResampler(dim = cond_dim, depth = 2, dim_head = attn_dim_head, heads = attn_heads, num_latents = attn_pool_num_latents, cosine_sim_attn = cosine_sim_attn) if attn_pool_text else None
+        self.attn_pool = PerceiverResampler(dim = cond_dim, depth = 2, dim_head = attn_dim_head, heads = attn_heads, num_latents = attn_pool_num_latents) if attn_pool_text else None
 
         # for classifier free guidance
 
         self.max_text_len = max_text_len
 
         self.null_text_embed = nn.Parameter(torch.randn(1, max_text_len, cond_dim))
         self.null_text_hidden = nn.Parameter(torch.randn(1, time_cond_dim))
@@ -1199,74 +1400,74 @@
                 nn.Linear(cond_dim, time_cond_dim),
                 nn.SiLU(),
                 nn.Linear(time_cond_dim, time_cond_dim)
             )
 
         # attention related params
 
-        attn_kwargs = dict(heads = attn_heads, dim_head = attn_dim_head, cosine_sim_attn = cosine_sim_attn)
+        attn_kwargs = dict(heads = attn_heads, dim_head = attn_dim_head)
 
         num_layers = len(in_out)
 
         # temporal attention - attention across video frames
 
         temporal_peg_padding = (0, 0, 0, 0, 2, 0) if time_causal_attn else (0, 0, 0, 0, 1, 1)
         temporal_peg = lambda dim: Residual(nn.Sequential(Pad(temporal_peg_padding), nn.Conv3d(dim, dim, (3, 1, 1), groups = dim)))
 
-        temporal_attn = lambda dim: EinopsToAndFrom('b c f h w', '(b h w) f c', Residual(Attention(dim, **{**attn_kwargs, 'causal': time_causal_attn})))
-
-        # temporal attention relative positional encoding
-
-        self.time_rel_pos_bias = DynamicPositionBias(dim = dim * 2, heads = attn_heads, depth = time_rel_pos_bias_depth)
+        temporal_attn = lambda dim: RearrangeTimeCentric(Residual(Attention(dim, **{**attn_kwargs, 'causal': time_causal_attn, 'init_zero': True, 'rel_pos_bias': True})))
 
         # resnet block klass
 
         num_resnet_blocks = cast_tuple(num_resnet_blocks, num_layers)
-        resnet_groups = cast_tuple(resnet_groups, num_layers)
 
         resnet_klass = partial(ResnetBlock, **attn_kwargs)
 
         layer_attns = cast_tuple(layer_attns, num_layers)
         layer_attns_depth = cast_tuple(layer_attns_depth, num_layers)
         layer_cross_attns = cast_tuple(layer_cross_attns, num_layers)
 
-        assert all([layers == num_layers for layers in list(map(len, (resnet_groups, layer_attns, layer_cross_attns)))])
+        assert all([layers == num_layers for layers in list(map(len, (layer_attns, layer_cross_attns)))])
+
+        # temporal downsample config
+
+        temporal_strides = cast_tuple(temporal_strides, num_layers)
+        self.total_temporal_divisor = functools.reduce(operator.mul, temporal_strides, 1)
 
         # downsample klass
 
         downsample_klass = Downsample
 
         if cross_embed_downsample:
             downsample_klass = partial(CrossEmbedLayer, kernel_sizes = cross_embed_downsample_kernel_sizes)
 
         # initial resnet block (for memory efficient unet)
 
-        self.init_resnet_block = resnet_klass(init_dim, init_dim, time_cond_dim = time_cond_dim, groups = resnet_groups[0], use_gca = use_global_context_attn) if memory_efficient else None
+        self.init_resnet_block = resnet_klass(init_dim, init_dim, time_cond_dim = time_cond_dim, use_gca = use_global_context_attn) if memory_efficient else None
 
         self.init_temporal_peg = temporal_peg(init_dim)
         self.init_temporal_attn = temporal_attn(init_dim)
 
         # scale for resnet skip connections
 
         self.skip_connect_scale = 1. if not scale_skip_connection else (2 ** -0.5)
 
         # layers
 
         self.downs = nn.ModuleList([])
         self.ups = nn.ModuleList([])
         num_resolutions = len(in_out)
 
-        layer_params = [num_resnet_blocks, resnet_groups, layer_attns, layer_attns_depth, layer_cross_attns]
+        layer_params = [num_resnet_blocks, layer_attns, layer_attns_depth, layer_cross_attns, temporal_strides]
         reversed_layer_params = list(map(reversed, layer_params))
 
         # downsampling layers
 
         skip_connect_dims = [] # keep track of skip connection dimensions
 
-        for ind, ((dim_in, dim_out), layer_num_resnet_blocks, groups, layer_attn, layer_attn_depth, layer_cross_attn) in enumerate(zip(in_out, *layer_params)):
+        for ind, ((dim_in, dim_out), layer_num_resnet_blocks, layer_attn, layer_attn_depth, layer_cross_attn, temporal_stride) in enumerate(zip(in_out, *layer_params)):
             is_last = ind >= (num_resolutions - 1)
 
             layer_use_linear_cross_attn = not layer_cross_attn and use_linear_cross_attn
             layer_cond_dim = cond_dim if layer_cross_attn or layer_use_linear_cross_attn else None
 
             transformer_block_klass = TransformerBlock if layer_attn else (LinearAttentionTransformerBlock if use_linear_attn else Identity)
 
@@ -1286,56 +1487,58 @@
 
             post_downsample = None
             if not memory_efficient:
                 post_downsample = downsample_klass(current_dim, dim_out) if not is_last else Parallel(Conv2d(dim_in, dim_out, 3, padding = 1), Conv2d(dim_in, dim_out, 1))
 
             self.downs.append(nn.ModuleList([
                 pre_downsample,
-                resnet_klass(current_dim, current_dim, cond_dim = layer_cond_dim, linear_attn = layer_use_linear_cross_attn, time_cond_dim = time_cond_dim, groups = groups),
-                nn.ModuleList([ResnetBlock(current_dim, current_dim, time_cond_dim = time_cond_dim, groups = groups, use_gca = use_global_context_attn) for _ in range(layer_num_resnet_blocks)]),
-                transformer_block_klass(dim = current_dim, depth = layer_attn_depth, ff_mult = ff_mult, context_dim = cond_dim, **attn_kwargs),
+                resnet_klass(current_dim, current_dim, cond_dim = layer_cond_dim, linear_attn = layer_use_linear_cross_attn, time_cond_dim = time_cond_dim),
+                nn.ModuleList([ResnetBlock(current_dim, current_dim, time_cond_dim = time_cond_dim, use_gca = use_global_context_attn) for _ in range(layer_num_resnet_blocks)]),
+                transformer_block_klass(dim = current_dim, depth = layer_attn_depth, ff_mult = ff_mult, ff_time_token_shift = ff_time_token_shift, context_dim = cond_dim, **attn_kwargs),
                 temporal_peg(current_dim),
                 temporal_attn(current_dim),
+                TemporalDownsample(current_dim, stride = temporal_stride) if temporal_stride > 1 else None,
                 post_downsample
             ]))
 
         # middle layers
 
         mid_dim = dims[-1]
 
-        self.mid_block1 = ResnetBlock(mid_dim, mid_dim, cond_dim = cond_dim, time_cond_dim = time_cond_dim, groups = resnet_groups[-1])
-        self.mid_attn = EinopsToAndFrom('b c f h w', 'b (f h w) c', Residual(Attention(mid_dim, **attn_kwargs))) if attend_at_middle else None
+        self.mid_block1 = ResnetBlock(mid_dim, mid_dim, cond_dim = cond_dim, time_cond_dim = time_cond_dim)
+        self.mid_attn = Residual(Attention(mid_dim, **attn_kwargs)) if attend_at_middle else None
         self.mid_temporal_peg = temporal_peg(mid_dim)
         self.mid_temporal_attn = temporal_attn(mid_dim)
-        self.mid_block2 = ResnetBlock(mid_dim, mid_dim, cond_dim = cond_dim, time_cond_dim = time_cond_dim, groups = resnet_groups[-1])
+        self.mid_block2 = ResnetBlock(mid_dim, mid_dim, cond_dim = cond_dim, time_cond_dim = time_cond_dim)
 
         # upsample klass
 
         upsample_klass = Upsample if not pixel_shuffle_upsample else PixelShuffleUpsample
 
         # upsampling layers
 
         upsample_fmap_dims = []
 
-        for ind, ((dim_in, dim_out), layer_num_resnet_blocks, groups, layer_attn, layer_attn_depth, layer_cross_attn) in enumerate(zip(reversed(in_out), *reversed_layer_params)):
+        for ind, ((dim_in, dim_out), layer_num_resnet_blocks, layer_attn, layer_attn_depth, layer_cross_attn, temporal_stride) in enumerate(zip(reversed(in_out), *reversed_layer_params)):
             is_last = ind == (len(in_out) - 1)
             layer_use_linear_cross_attn = not layer_cross_attn and use_linear_cross_attn
             layer_cond_dim = cond_dim if layer_cross_attn or layer_use_linear_cross_attn else None
             transformer_block_klass = TransformerBlock if layer_attn else (LinearAttentionTransformerBlock if use_linear_attn else Identity)
 
             skip_connect_dim = skip_connect_dims.pop()
 
             upsample_fmap_dims.append(dim_out)
 
             self.ups.append(nn.ModuleList([
-                resnet_klass(dim_out + skip_connect_dim, dim_out, cond_dim = layer_cond_dim, linear_attn = layer_use_linear_cross_attn, time_cond_dim = time_cond_dim, groups = groups),
-                nn.ModuleList([ResnetBlock(dim_out + skip_connect_dim, dim_out, time_cond_dim = time_cond_dim, groups = groups, use_gca = use_global_context_attn) for _ in range(layer_num_resnet_blocks)]),
-                transformer_block_klass(dim = dim_out, depth = layer_attn_depth, ff_mult = ff_mult, context_dim = cond_dim, **attn_kwargs),
+                resnet_klass(dim_out + skip_connect_dim, dim_out, cond_dim = layer_cond_dim, linear_attn = layer_use_linear_cross_attn, time_cond_dim = time_cond_dim),
+                nn.ModuleList([ResnetBlock(dim_out + skip_connect_dim, dim_out, time_cond_dim = time_cond_dim, use_gca = use_global_context_attn) for _ in range(layer_num_resnet_blocks)]),
+                transformer_block_klass(dim = dim_out, depth = layer_attn_depth, ff_mult = ff_mult,  ff_time_token_shift = ff_time_token_shift, context_dim = cond_dim, **attn_kwargs),
                 temporal_peg(dim_out),
                 temporal_attn(dim_out),
+                TemporalPixelShuffleUpsample(dim_out, stride = temporal_stride) if temporal_stride > 1 else None,
                 upsample_klass(dim_out, dim_in) if not is_last or memory_efficient else Identity()
             ]))
 
         # whether to combine feature maps from all upsample blocks before final resnet block out
 
         self.upsample_combiner = UpsampleCombiner(
             dim = dim,
@@ -1347,23 +1550,27 @@
         # whether to do a final residual from initial conv to the final resnet block out
 
         self.init_conv_to_final_conv_residual = init_conv_to_final_conv_residual
         final_conv_dim = self.upsample_combiner.dim_out + (dim if init_conv_to_final_conv_residual else 0)
 
         # final optional resnet block and convolution out
 
-        self.final_res_block = ResnetBlock(final_conv_dim, dim, time_cond_dim = time_cond_dim, groups = resnet_groups[0], use_gca = True) if final_resnet_block else None
+        self.final_res_block = ResnetBlock(final_conv_dim, dim, time_cond_dim = time_cond_dim, use_gca = True) if final_resnet_block else None
 
         final_conv_dim_in = dim if final_resnet_block else final_conv_dim
         final_conv_dim_in += (channels if lowres_cond else 0)
 
         self.final_conv = Conv2d(final_conv_dim_in, self.channels_out, final_conv_kernel_size, padding = final_conv_kernel_size // 2)
 
         zero_init_(self.final_conv)
 
+        # resize mode
+
+        self.resize_mode = resize_mode
+
     # if the current settings for the unet are not correct
     # for cascading DDPM, then reinit the unet with the right settings
     def cast_model_parameters(
         self,
         *,
         lowres_cond,
         text_embed_dim,
@@ -1446,54 +1653,100 @@
         time,
         *,
         lowres_cond_img = None,
         lowres_noise_times = None,
         text_embeds = None,
         text_mask = None,
         cond_images = None,
+        cond_video_frames = None,
+        post_cond_video_frames = None,
         self_cond = None,
-        cond_drop_prob = 0.
+        cond_drop_prob = 0.,
+        ignore_time = False
     ):
         assert x.ndim == 5, 'input to 3d unet must have 5 dimensions (batch, channels, time, height, width)'
 
         batch_size, frames, device, dtype = x.shape[0], x.shape[2], x.device, x.dtype
 
+        assert ignore_time or divisible_by(frames, self.total_temporal_divisor), f'number of input frames {frames} must be divisible by {self.total_temporal_divisor}'
+
         # add self conditioning if needed
 
         if self.self_cond:
             self_cond = default(self_cond, lambda: torch.zeros_like(x))
             x = torch.cat((x, self_cond), dim = 1)
 
         # add low resolution conditioning, if present
 
         assert not (self.lowres_cond and not exists(lowres_cond_img)), 'low resolution conditioning image must be present'
         assert not (self.lowres_cond and not exists(lowres_noise_times)), 'low resolution conditioning noise time must be present'
 
         if exists(lowres_cond_img):
             x = torch.cat((x, lowres_cond_img), dim = 1)
 
+            if exists(cond_video_frames):
+                lowres_cond_img = torch.cat((cond_video_frames, lowres_cond_img), dim = 2)
+                cond_video_frames = torch.cat((cond_video_frames, cond_video_frames), dim = 1)
+
+            if exists(post_cond_video_frames):
+                lowres_cond_img = torch.cat((lowres_cond_img, post_cond_video_frames), dim = 2)
+                post_cond_video_frames = torch.cat((post_cond_video_frames, post_cond_video_frames), dim = 1)
+
+        # conditioning on video frames as a prompt
+
+        num_preceding_frames = 0
+        if exists(cond_video_frames):
+            cond_video_frames_len = cond_video_frames.shape[2]
+
+            assert divisible_by(cond_video_frames_len, self.total_temporal_divisor)
+
+            cond_video_frames = resize_video_to(cond_video_frames, x.shape[-1])
+            x = torch.cat((cond_video_frames, x), dim = 2)
+
+            num_preceding_frames = cond_video_frames_len
+
+        # conditioning on video frames as a prompt
+
+        num_succeeding_frames = 0
+        if exists(post_cond_video_frames):
+            cond_video_frames_len = post_cond_video_frames.shape[2]
+
+            assert divisible_by(cond_video_frames_len, self.total_temporal_divisor)
+
+            post_cond_video_frames = resize_video_to(post_cond_video_frames, x.shape[-1])
+            x = torch.cat((post_cond_video_frames, x), dim = 2)
+
+            num_succeeding_frames = cond_video_frames_len
+
         # condition on input image
 
         assert not (self.has_cond_image ^ exists(cond_images)), 'you either requested to condition on an image on the unet, but the conditioning image is not supplied, or vice versa'
 
         if exists(cond_images):
+            assert cond_images.ndim == 4, 'conditioning images must have 4 dimensions only, if you want to condition on frames of video, use `cond_video_frames` instead'
             assert cond_images.shape[1] == self.cond_images_channels, 'the number of channels on the conditioning image you are passing in does not match what you specified on initialiation of the unet'
-            cond_images = resize_video_to(cond_images, x.shape[-1])
+
+            cond_images = repeat(cond_images, 'b c h w -> b c f h w', f = x.shape[2])
+            cond_images = resize_video_to(cond_images, x.shape[-1], mode = self.resize_mode)
+
             x = torch.cat((cond_images, x), dim = 1)
 
-        # get time relative positions
+        # ignoring time in pseudo 3d resnet blocks
 
-        time_attn_bias = self.time_rel_pos_bias(frames, device = device, dtype = dtype)
+        conv_kwargs = dict(
+            ignore_time = ignore_time
+        )
 
         # initial convolution
 
         x = self.init_conv(x)
 
-        x = self.init_temporal_peg(x)
-        x = self.init_temporal_attn(x, attn_bias = time_attn_bias)
+        if not ignore_time:
+            x = self.init_temporal_peg(x)
+            x = self.init_temporal_attn(x)
 
         # init conv residual
 
         if self.init_conv_to_final_conv_residual:
             init_conv_residual = x.clone()
 
         # time conditioning
@@ -1586,77 +1839,103 @@
         # normalize conditioning tokens
 
         c = self.norm_cond(c)
 
         # initial resnet block (for memory efficient unet)
 
         if exists(self.init_resnet_block):
-            x = self.init_resnet_block(x, t)
+            x = self.init_resnet_block(x, t, **conv_kwargs)
 
         # go through the layers of the unet, down and up
 
         hiddens = []
 
-        for pre_downsample, init_block, resnet_blocks, attn_block, temporal_peg, temporal_attn, post_downsample in self.downs:
+        for pre_downsample, init_block, resnet_blocks, attn_block, temporal_peg, temporal_attn, temporal_downsample, post_downsample in self.downs:
             if exists(pre_downsample):
                 x = pre_downsample(x)
 
-            x = init_block(x, t, c)
+            x = init_block(x, t, c, **conv_kwargs)
 
             for resnet_block in resnet_blocks:
-                x = resnet_block(x, t)
+                x = resnet_block(x, t, **conv_kwargs)
                 hiddens.append(x)
 
             x = attn_block(x, c)
-            x = temporal_peg(x)
-            x = temporal_attn(x, attn_bias = time_attn_bias)
+
+            if not ignore_time:
+                x = temporal_peg(x)
+                x = temporal_attn(x)
 
             hiddens.append(x)
 
+            if exists(temporal_downsample) and not ignore_time:
+                x = temporal_downsample(x)
+
             if exists(post_downsample):
                 x = post_downsample(x)
 
-        x = self.mid_block1(x, t, c)
+        x = self.mid_block1(x, t, c, **conv_kwargs)
 
         if exists(self.mid_attn):
+            x = rearrange(x, 'b c f h w -> b f h w c')
+            x, ps = pack([x], 'b * c')
+
             x = self.mid_attn(x)
 
-        x = self.mid_temporal_peg(x)
-        x = self.mid_temporal_attn(x, attn_bias = time_attn_bias)
+            x, = unpack(x, ps, 'b * c')
+            x = rearrange(x, 'b f h w c -> b c f h w')
+
+        if not ignore_time:
+            x = self.mid_temporal_peg(x)
+            x = self.mid_temporal_attn(x)
 
-        x = self.mid_block2(x, t, c)
+        x = self.mid_block2(x, t, c, **conv_kwargs)
 
         add_skip_connection = lambda x: torch.cat((x, hiddens.pop() * self.skip_connect_scale), dim = 1)
 
         up_hiddens = []
 
-        for init_block, resnet_blocks, attn_block, temporal_peg, temporal_attn, upsample in self.ups:
+        for init_block, resnet_blocks, attn_block, temporal_peg, temporal_attn, temporal_upsample, upsample in self.ups:
+            if exists(temporal_upsample) and not ignore_time:
+                x = temporal_upsample(x)
+
             x = add_skip_connection(x)
-            x = init_block(x, t, c)
+            x = init_block(x, t, c, **conv_kwargs)
 
             for resnet_block in resnet_blocks:
                 x = add_skip_connection(x)
-                x = resnet_block(x, t)
+                x = resnet_block(x, t, **conv_kwargs)
 
             x = attn_block(x, c)
-            x = temporal_peg(x)
-            x = temporal_attn(x, attn_bias = time_attn_bias)
+
+            if not ignore_time:
+                x = temporal_peg(x)
+                x = temporal_attn(x)
 
             up_hiddens.append(x.contiguous())
+
             x = upsample(x)
 
         # whether to combine all feature maps from upsample blocks
 
         x = self.upsample_combiner(x, up_hiddens)
 
         # final top-most residual if needed
 
         if self.init_conv_to_final_conv_residual:
             x = torch.cat((x, init_conv_residual), dim = 1)
 
         if exists(self.final_res_block):
-            x = self.final_res_block(x, t)
+            x = self.final_res_block(x, t, **conv_kwargs)
 
         if exists(lowres_cond_img):
             x = torch.cat((x, lowres_cond_img), dim = 1)
 
-        return self.final_conv(x)
+        out = self.final_conv(x)
+
+        if num_preceding_frames > 0:
+            out = out[:, :, num_preceding_frames:]
+
+        if num_succeeding_frames > 0:
+            out = out[:, :, :-num_succeeding_frames]
+
+        return out
```

### Comparing `imagen-pytorch-1.9.7/imagen_pytorch/t5.py` & `imagen_pytorch-2.0.0/imagen_pytorch/t5.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 DEFAULT_T5_NAME = 'google/t5-v1_1-base'
 
 T5_CONFIGS = {}
 
 # singleton globals
 
 def get_tokenizer(name):
-    tokenizer = T5Tokenizer.from_pretrained(name)
+    tokenizer = T5Tokenizer.from_pretrained(name, model_max_length=MAX_LENGTH)
     return tokenizer
 
 def get_model(name):
     model = T5EncoderModel.from_pretrained(name)
     return model
 
 def get_model_and_tokenizer(name):
```

### Comparing `imagen-pytorch-1.9.7/imagen_pytorch/trainer.py` & `imagen_pytorch-2.0.0/imagen_pytorch/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 import os
-import time
-import copy
-from pathlib import Path
 from math import ceil
 from contextlib import contextmanager, nullcontext
 from functools import partial, wraps
 from collections.abc import Iterable
 
 import torch
 from torch import nn
@@ -42,15 +39,15 @@
     if exists(val):
         return val
     return d() if callable(d) else d
 
 def cast_tuple(val, length = 1):
     if isinstance(val, list):
         val = tuple(val)
-    
+
     return val if isinstance(val, tuple) else ((val,) * length)
 
 def find_first(fn, arr):
     for ind, el in enumerate(arr):
         if fn(el):
             return ind
     return -1
@@ -123,15 +120,15 @@
         split_kwargs_index = len(all_args) - len(kwargs_keys)
         all_args = tuple(map(lambda t: torch.from_numpy(t) if exists(t) and isinstance(t, np.ndarray) else t, all_args))
 
         if cast_device:
             all_args = tuple(map(lambda t: t.to(device) if exists(t) and isinstance(t, torch.Tensor) else t, all_args))
 
         if should_cast_fp16:
-            all_args = tuple(map(lambda t: t.half() if exists(t) and isinstance(t, torch.Tensor) else t, all_args))
+            all_args = tuple(map(lambda t: t.half() if exists(t) and isinstance(t, torch.Tensor) and t.dtype != torch.bool else t, all_args))
 
         args, kwargs_values = all_args[:split_kwargs_index], all_args[split_kwargs_index:]
         kwargs = dict(tuple(zip(kwargs_keys, kwargs_values)))
 
         out = fn(model, *args, **kwargs)
         return out
     return inner
@@ -174,15 +171,15 @@
     num_chunks = ceil(batch_size / split_size)
 
     dict_len = len(kwargs)
     dict_keys = kwargs.keys()
     split_kwargs_index = len_all_args - dict_len
 
     split_all_args = [split(arg, split_size = split_size) if exists(arg) and isinstance(arg, (torch.Tensor, Iterable)) else ((arg,) * num_chunks) for arg in all_args]
-    chunk_sizes = tuple(map(len, split_all_args[0]))
+    chunk_sizes = num_to_groups(batch_size, split_size)
 
     for (chunk_size, *chunked_all_args) in tuple(zip(chunk_sizes, *split_all_args)):
         chunked_args, chunked_kwargs_values = chunked_all_args[:split_kwargs_index], chunked_all_args[split_kwargs_index:]
         chunked_kwargs = dict(tuple(zip(dict_keys, chunked_kwargs_values)))
         chunk_size_frac = chunk_size / batch_size
         yield chunk_size_frac, (chunked_args, chunked_kwargs)
 
@@ -330,14 +327,15 @@
 
         # be able to finely customize learning rate, weight decay
         # per unet
 
         lr, eps, warmup_steps, cosine_decay_max_steps = map(partial(cast_tuple, length = self.num_unets), (lr, eps, warmup_steps, cosine_decay_max_steps))
 
         for ind, (unet, unet_lr, unet_eps, unet_warmup_steps, unet_cosine_decay_max_steps) in enumerate(zip(self.imagen.unets, lr, eps, warmup_steps, cosine_decay_max_steps)):
+
             optimizer = Adam(
                 unet.parameters(),
                 lr = unet_lr,
                 eps = unet_eps,
                 betas = (beta1, beta2),
                 **kwargs
             )
@@ -396,16 +394,21 @@
                 self.fs.mkdir(bucket)
 
             self.load_from_checkpoint_folder()
 
         # only allowing training for unet
 
         self.only_train_unet_number = only_train_unet_number
-        self.validate_and_set_unet_being_trained(only_train_unet_number)
+        self.prepared = False
+
 
+    def prepare(self):
+        assert not self.prepared, f'The trainer is allready prepared'
+        self.validate_and_set_unet_being_trained(self.only_train_unet_number)
+        self.prepared = True
     # computed values
 
     @property
     def device(self):
         return self.accelerator.device
 
     @property
@@ -451,39 +454,50 @@
         self.wrap_unet(unet_number)
 
     def wrap_unet(self, unet_number):
         if hasattr(self, 'one_unet_wrapped'):
             return
 
         unet = self.imagen.get_unet(unet_number)
-        self.unet_being_trained = self.accelerator.prepare(unet)
         unet_index = unet_number - 1
 
         optimizer = getattr(self, f'optim{unet_index}')
         scheduler = getattr(self, f'scheduler{unet_index}')
 
-        optimizer = self.accelerator.prepare(optimizer)
+        if self.train_dl:
+            self.unet_being_trained, self.train_dl, optimizer = self.accelerator.prepare(unet, self.train_dl, optimizer)
+        else:
+            self.unet_being_trained, optimizer = self.accelerator.prepare(unet, optimizer)
 
         if exists(scheduler):
             scheduler = self.accelerator.prepare(scheduler)
 
         setattr(self, f'optim{unet_index}', optimizer)
         setattr(self, f'scheduler{unet_index}', scheduler)
 
         self.one_unet_wrapped = True
 
     # hacking accelerator due to not having separate gradscaler per optimizer
 
     def set_accelerator_scaler(self, unet_number):
+        def patch_optimizer_step(accelerated_optimizer, method):
+            def patched_step(*args, **kwargs):
+                accelerated_optimizer._accelerate_step_called = True
+                return method(*args, **kwargs)
+            return patched_step
+
         unet_number = self.validate_unet_number(unet_number)
         scaler = getattr(self, f'scaler{unet_number - 1}')
 
         self.accelerator.scaler = scaler
         for optimizer in self.accelerator._optimizers:
             optimizer.scaler = scaler
+            optimizer._accelerate_step_called = False
+            optimizer._optimizer_original_step_method = optimizer.optimizer.step
+            optimizer._optimizer_patched_step_method = patch_optimizer_step(optimizer, optimizer.optimizer.step)
 
     # helper print
 
     def print(self, msg):
         if not self.is_main:
             return
 
@@ -525,22 +539,24 @@
     # data related functions
 
     def add_train_dataloader(self, dl = None):
         if not exists(dl):
             return
 
         assert not exists(self.train_dl), 'training dataloader was already added'
-        self.train_dl = self.accelerator.prepare(dl)
+        assert not self.prepared, f'You need to add the dataset before preperation'
+        self.train_dl = dl
 
     def add_valid_dataloader(self, dl):
         if not exists(dl):
             return
 
         assert not exists(self.valid_dl), 'validation dataloader was already added'
-        self.valid_dl = self.accelerator.prepare(dl)
+        assert not self.prepared, f'You need to add the dataset before preperation'
+        self.valid_dl = dl
 
     def add_train_dataset(self, ds = None, *, batch_size, **dl_kwargs):
         if not exists(ds):
             return
 
         assert not exists(self.train_dl), 'training dataloader was already added'
 
@@ -549,29 +565,29 @@
             train_size = int((1 - self.split_valid_fraction) * len(ds))
             valid_size = len(ds) - train_size
 
             ds, valid_ds = random_split(ds, [train_size, valid_size], generator = torch.Generator().manual_seed(self.split_random_seed))
             self.print(f'training with dataset of {len(ds)} samples and validating with randomly splitted {len(valid_ds)} samples')
 
         dl = DataLoader(ds, batch_size = batch_size, **dl_kwargs)
-        self.train_dl = self.accelerator.prepare(dl)
+        self.add_train_dataloader(dl)
 
         if not self.split_valid_from_train:
             return
 
         self.add_valid_dataset(valid_ds, batch_size = batch_size, **dl_kwargs)
 
     def add_valid_dataset(self, ds, *, batch_size, **dl_kwargs):
         if not exists(ds):
             return
 
         assert not exists(self.valid_dl), 'validation dataloader was already added'
 
         dl = DataLoader(ds, batch_size = batch_size, **dl_kwargs)
-        self.valid_dl = self.accelerator.prepare(dl)
+        self.add_valid_dataloader(dl)
 
     def create_train_iter(self):
         assert exists(self.train_dl), 'training dataloader has not been registered with the trainer yet'
 
         if exists(self.train_dl_iter):
             return
 
@@ -581,27 +597,31 @@
         assert exists(self.valid_dl), 'validation dataloader has not been registered with the trainer yet'
 
         if exists(self.valid_dl_iter):
             return
 
         self.valid_dl_iter = cycle(self.valid_dl)
 
-    def train_step(self, unet_number = None, **kwargs):
+    def train_step(self, *, unet_number = None, **kwargs):
+        if not self.prepared:
+            self.prepare()
         self.create_train_iter()
-        loss = self.step_with_dl_iter(self.train_dl_iter, unet_number = unet_number, **kwargs)
+
+        kwargs = {'unet_number': unet_number, **kwargs}
+        loss = self.step_with_dl_iter(self.train_dl_iter, **kwargs)
         self.update(unet_number = unet_number)
         return loss
 
     @torch.no_grad()
     @eval_decorator
     def valid_step(self, **kwargs):
+        if not self.prepared:
+            self.prepare()
         self.create_valid_iter()
-
         context = self.use_ema_unets if kwargs.pop('use_ema_unets', False) else nullcontext
-
         with context():
             loss = self.step_with_dl_iter(self.valid_dl_iter, **kwargs)
         return loss
 
     def step_with_dl_iter(self, dl_iter, **kwargs):
         dl_tuple_output = cast_tuple(next(dl_iter))
         model_input = dict(list(zip(self.dl_tuple_output_keywords_names, dl_tuple_output)))
@@ -926,18 +946,21 @@
 
     @torch.no_grad()
     @cast_torch_tensor
     @imagen_sample_in_chunks
     def sample(self, *args, **kwargs):
         context = nullcontext if  kwargs.pop('use_non_ema', False) else self.use_ema_unets
 
-        self.print_untrained_unets()        
+        self.print_untrained_unets()
+
+        if not self.is_main:
+            kwargs['use_tqdm'] = False
 
         with context():
-            output = self.imagen.sample(*args, device = self.device, use_tqdm = self.is_main, **kwargs)
+            output = self.imagen.sample(*args, device = self.device, **kwargs)
 
         return output
 
     @partial(cast_torch_tensor, cast_fp16 = True)
     def forward(
         self,
         *args,
```

### Comparing `imagen-pytorch-1.9.7/imagen_pytorch/utils.py` & `imagen_pytorch-2.0.0/imagen_pytorch/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     imagen_type = safeget(loaded, 'imagen_type')
 
     if imagen_type == 'original':
         imagen_klass = ImagenConfig
     elif imagen_type == 'elucidated':
         imagen_klass = ElucidatedImagenConfig
     else:
-        raise ValueError(f'unknown imagen type {imagen_type}')
+        raise ValueError(f'unknown imagen type {imagen_type} - you need to instantiate your Imagen with configurations, using classes ImagenConfig or ElucidatedImagenConfig')
 
     assert exists(imagen_params) and exists(imagen_type), 'imagen type and configuration not saved in this checkpoint'
 
     imagen = imagen_klass(**imagen_params).create()
 
     if not load_weights:
         return imagen
```

### Comparing `imagen-pytorch-1.9.7/imagen_pytorch.egg-info/SOURCES.txt` & `imagen_pytorch-2.0.0/imagen_pytorch.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 LICENSE
+MANIFEST.in
 README.md
 setup.py
 imagen_pytorch/__init__.py
 imagen_pytorch/cli.py
 imagen_pytorch/configs.py
 imagen_pytorch/data.py
+imagen_pytorch/default_config.json
 imagen_pytorch/elucidated_imagen.py
 imagen_pytorch/imagen_pytorch.py
+imagen_pytorch/imagen_video.py
 imagen_pytorch/t5.py
 imagen_pytorch/trainer.py
 imagen_pytorch/utils.py
 imagen_pytorch/version.py
 imagen_pytorch.egg-info/PKG-INFO
 imagen_pytorch.egg-info/SOURCES.txt
 imagen_pytorch.egg-info/dependency_links.txt
 imagen_pytorch.egg-info/entry_points.txt
 imagen_pytorch.egg-info/requires.txt
 imagen_pytorch.egg-info/top_level.txt
-imagen_pytorch/imagen_video/__init__.py
-imagen_pytorch/imagen_video/imagen_video.py
+imagen_pytorch/test/__init__.py
+imagen_pytorch/test/test_trainer.py
```

### Comparing `imagen-pytorch-1.9.7/setup.py` & `imagen_pytorch-2.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,26 +22,26 @@
     'artificial intelligence',
     'deep learning',
     'transformers',
     'text-to-image',
     'denoising-diffusion'
   ],
   install_requires=[
-    'accelerate',
+    'accelerate>=0.23.0',
+    'beartype',
     'click',
-    'einops>=0.4',
-    'einops-exts',
+    'datasets',
+    'einops>=0.7.0',
     'ema-pytorch>=0.0.3',
     'fsspec',
     'kornia',
     'numpy',
     'packaging',
     'pillow',
-    'pydantic',
-    'pytorch-lightning',
+    'pydantic>=2',
     'pytorch-warmup',
     'sentencepiece',
     'torch>=1.6',
     'torchvision',
     'transformers',
     'tqdm'
   ],
```


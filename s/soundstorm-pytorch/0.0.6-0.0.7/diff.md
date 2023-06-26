# Comparing `tmp/soundstorm-pytorch-0.0.6.tar.gz` & `tmp/soundstorm-pytorch-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soundstorm-pytorch-0.0.6.tar", last modified: Thu May 18 19:17:47 2023, max compression
+gzip compressed data, was "soundstorm-pytorch-0.0.7.tar", last modified: Thu May 18 21:27:01 2023, max compression
```

## Comparing `soundstorm-pytorch-0.0.6.tar` & `soundstorm-pytorch-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:17:47.145687 soundstorm-pytorch-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-18 19:17:34.000000 soundstorm-pytorch-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-18 19:17:47.145687 soundstorm-pytorch-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-05-18 19:17:34.000000 soundstorm-pytorch-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 19:17:47.145687 soundstorm-pytorch-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-18 19:17:34.000000 soundstorm-pytorch-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:17:47.145687 soundstorm-pytorch-0.0.6/soundstorm_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-18 19:17:34.000000 soundstorm-pytorch-0.0.6/soundstorm_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-05-18 19:17:34.000000 soundstorm-pytorch-0.0.6/soundstorm_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    14551 2023-05-18 19:17:34.000000 soundstorm-pytorch-0.0.6/soundstorm_pytorch/soundstorm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:17:47.145687 soundstorm-pytorch-0.0.6/soundstorm_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-18 19:17:47.000000 soundstorm-pytorch-0.0.6/soundstorm_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-18 19:17:47.000000 soundstorm-pytorch-0.0.6/soundstorm_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 19:17:47.000000 soundstorm-pytorch-0.0.6/soundstorm_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-18 19:17:47.000000 soundstorm-pytorch-0.0.6/soundstorm_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-18 19:17:47.000000 soundstorm-pytorch-0.0.6/soundstorm_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:27:01.605692 soundstorm-pytorch-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-18 21:26:50.000000 soundstorm-pytorch-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-18 21:27:01.605692 soundstorm-pytorch-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-05-18 21:26:50.000000 soundstorm-pytorch-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 21:27:01.605692 soundstorm-pytorch-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-18 21:26:50.000000 soundstorm-pytorch-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:27:01.601692 soundstorm-pytorch-0.0.7/soundstorm_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-18 21:26:50.000000 soundstorm-pytorch-0.0.7/soundstorm_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-05-18 21:26:50.000000 soundstorm-pytorch-0.0.7/soundstorm_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14873 2023-05-18 21:26:50.000000 soundstorm-pytorch-0.0.7/soundstorm_pytorch/soundstorm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:27:01.605692 soundstorm-pytorch-0.0.7/soundstorm_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-18 21:27:01.000000 soundstorm-pytorch-0.0.7/soundstorm_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-18 21:27:01.000000 soundstorm-pytorch-0.0.7/soundstorm_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 21:27:01.000000 soundstorm-pytorch-0.0.7/soundstorm_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-18 21:27:01.000000 soundstorm-pytorch-0.0.7/soundstorm_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-18 21:27:01.000000 soundstorm-pytorch-0.0.7/soundstorm_pytorch.egg-info/top_level.txt
```

### Comparing `soundstorm-pytorch-0.0.6/LICENSE` & `soundstorm-pytorch-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `soundstorm-pytorch-0.0.6/PKG-INFO` & `soundstorm-pytorch-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soundstorm-pytorch
-Version: 0.0.6
+Version: 0.0.7
 Summary: SoundStorm - Efficient Parallel Audio Generation from Google Deepmind, in Pytorch
 Home-page: https://github.com/lucidrains/soundstorm-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `soundstorm-pytorch-0.0.6/README.md` & `soundstorm-pytorch-0.0.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <img src="./soundstorm.png" width="450px"></img>
 
 ## Soundstorm - Pytorch (wip)
 
 Implementation of <a href="https://arxiv.org/abs/2305.09636">SoundStorm</a>, Efficient Parallel Audio Generation from Google Deepmind, in Pytorch.
 
-They basically applied <a href="https://arxiv.org/abs/2202.04200">MaskGiT</a> to the residual vector quantized latents from <a href="https://github.com/lucidrains/audiolm-pytorch#soundstream--encodec">Soundstream</a>. The transformer architecture they chose to use is one that fits well with the audio domain, named <a href="https://arxiv.org/abs/2005.08100">Conformer</a>
+They basically applied <a href="https://arxiv.org/abs/2202.04200">MaskGiT</a> to the residual vector quantized codes from <a href="https://github.com/lucidrains/audiolm-pytorch#soundstream--encodec">Soundstream</a>. The transformer architecture they chose to use is one that fits well with the audio domain, named <a href="https://arxiv.org/abs/2005.08100">Conformer</a>
 
 <a href="https://google-research.github.io/seanet/soundstorm/examples/">Project Page</a>
 
 ## Appreciation
 
 - <a href="https://stability.ai/">Stability</a> and <a href="https://huggingface.co/">🤗 Huggingface</a> for their generous sponsorships to work on and open source cutting edge artificial intelligence research
 
@@ -39,24 +39,24 @@
 
 model = SoundStorm(
     conformer,
     steps = 18,          # 18 steps, as in original maskgit paper
     schedule = 'cosine'  # currently the best schedule is cosine
 )
 
-# get your codes from the soundstream
+# get your pre-encoded codebook ids from the soundstream from a lot of raw audio
 
 codes = torch.randint(0, 1024, (2, 1024))
 
-# learn to de-mask
+# do the below in a loop for a ton of data
 
 loss, _ = model(codes)
 loss.backward()
 
-# generate by de-masking iteratively
+# model can now generate in 18 steps. ~2 seconds sounds reasonable
 
 generated = model.generate(1024, batch_size = 2) # (2, 1024)
 ```
 
 To directly train on raw audio, you need to pass in your pretrained `SoundStream` into `SoundStorm`. You can train your own `SoundStream` at <a href="https://github.com/lucidrains/audiolm-pytorch#soundstream--encodec">audiolm-pytorch</a>.
 
 ```python
@@ -80,29 +80,38 @@
 )
 
 model = SoundStorm(
     conformer,
     soundstream = soundstream   # pass in the soundstream
 )
 
-audio = torch.randn(2, 10080)   # now you have a raw audio that you directly pass into the model
+# find as much audio you'd like the model to learn
+
+audio = torch.randn(2, 10080)
+
+# course it through the model and take a gazillion tiny steps
 
 loss, _ = model(audio)
 loss.backward()
 
-generated_audio = model.generate(1024, batch_size = 2)  # generated audio is also a raw wave now
+# and now you can generate state-of-the-art speech
+
+generated_audio = model.generate(seconds = 30, batch_size = 2)  # generate 30 seconds of audio (it will calculate the length in seconds based off the sampling frequency and cumulative downsamples in the soundstream passed in above)
 ```
 
 ## Todo
 
 - [x] integrate soundstream
+- [x] when generating, and length can be defined in seconds (takes into sampling freq etc)
 
-- [ ] when generating, make sure it can return audio file, and length can be defined in seconds (takes into sampling freq etc)
+- [ ] option to return list of audio files when generating
 - [ ] turn it into a command line tool
 - [ ] add cross attention and adaptive layernorm conditioning (just copy paste in the entire conformer repository, if conditioning adds too much cruft to the other repo)
+- [ ] make sure grouped rvq is supported. concat embeddings rather than sum across group dimension
+- [ ] trainer with accelerate
 
 ## Citations
 
 ```bibtex
 @misc{borsos2023soundstorm,
     title   = {SoundStorm: Efficient Parallel Audio Generation}, 
     author  = {Zalán Borsos and Matt Sharifi and Damien Vincent and Eugene Kharitonov and Neil Zeghidour and Marco Tagliasacchi},
```

#### html2text {}

```diff
@@ -1,58 +1,64 @@
 [./soundstorm.png] ## Soundstorm - Pytorch (wip) Implementation of SoundStorm,
 Efficient Parallel Audio Generation from Google Deepmind, in Pytorch. They
-basically applied MaskGiT to the residual vector quantized latents from
+basically applied MaskGiT to the residual vector quantized codes from
 Soundstream. The transformer architecture they chose to use is one that fits
 well with the audio domain, named Conformer Project_Page ## Appreciation -
 Stability and ð¤_Huggingface for their generous sponsorships to work on and
 open source cutting edge artificial intelligence research - ð¤_Accelerate for
 providing a simple and powerful solution for training - Einops for the
 indispensable abstraction that makes building neural networks fun, easy, and
 uplifting ## Install ```bash $ pip install soundstorm-pytorch ``` ## Usage
 ```python import torch from soundstorm_pytorch import SoundStorm,
 ConformerWrapper conformer = ConformerWrapper( codebook_size = 1024,
 num_quantizers = 4, conformer = dict( dim = 512, depth = 2 ), ) model =
 SoundStorm( conformer, steps = 18, # 18 steps, as in original maskgit paper
-schedule = 'cosine' # currently the best schedule is cosine ) # get your codes
-from the soundstream codes = torch.randint(0, 1024, (2, 1024)) # learn to de-
-mask loss, _ = model(codes) loss.backward() # generate by de-masking
-iteratively generated = model.generate(1024, batch_size = 2) # (2, 1024) ``` To
-directly train on raw audio, you need to pass in your pretrained `SoundStream`
-into `SoundStorm`. You can train your own `SoundStream` at audiolm-pytorch.
-```python import torch from soundstorm_pytorch import SoundStorm,
-ConformerWrapper, Conformer, SoundStream conformer = ConformerWrapper
-( codebook_size = 1024, num_quantizers = 4, conformer = dict( dim = 512, depth
-= 2 ), ) soundstream = SoundStream( codebook_size = 1024, rq_num_quantizers =
-4, attn_window_size = 128, attn_depth = 2 ) model = SoundStorm( conformer,
-soundstream = soundstream # pass in the soundstream ) audio = torch.randn(2,
-10080) # now you have a raw audio that you directly pass into the model loss, _
-= model(audio) loss.backward() generated_audio = model.generate(1024,
-batch_size = 2) # generated audio is also a raw wave now ``` ## Todo - [x]
-integrate soundstream - [ ] when generating, make sure it can return audio
-file, and length can be defined in seconds (takes into sampling freq etc) - [ ]
-turn it into a command line tool - [ ] add cross attention and adaptive
-layernorm conditioning (just copy paste in the entire conformer repository, if
-conditioning adds too much cruft to the other repo) ## Citations ```bibtex
-@misc{borsos2023soundstorm, title = {SoundStorm: Efficient Parallel Audio
-Generation}, author = {ZalÃ¡n Borsos and Matt Sharifi and Damien Vincent and
-Eugene Kharitonov and Neil Zeghidour and Marco Tagliasacchi}, year = {2023},
-eprint = {2305.09636}, archivePrefix = {arXiv}, primaryClass = {cs.SD} } ```
-```bibtex @inproceedings{dao2022flashattention, title = {Flash{A}ttention: Fast
-and Memory-Efficient Exact Attention with {IO}-Awareness}, author = {Dao, Tri
-and Fu, Daniel Y. and Ermon, Stefano and Rudra, Atri and R{\'e}, Christopher},
-booktitle = {Advances in Neural Information Processing Systems}, year = {2022}
-} ``` ```bibtex @article{Chang2022MaskGITMG, title = {MaskGIT: Masked
-Generative Image Transformer}, author = {Huiwen Chang and Han Zhang and Lu
-Jiang and Ce Liu and William T. Freeman}, journal = {2022 IEEE/CVF Conference
-on Computer Vision and Pattern Recognition (CVPR)}, year = {2022}, pages =
-{11305-11315} } ``` ```bibtex @article{Lezama2022ImprovedMI, title = {Improved
-Masked Image Generation with Token-Critic}, author = {Jos{\'e} Lezama and
-Huiwen Chang and Lu Jiang and Irfan Essa}, journal = {ArXiv}, year = {2022},
-volume = {abs/2209.04439} } ``` ```bibtex @inproceedings{Nijkamp2021SCRIPTSP,
-title = {SCRIPT: Self-Critic PreTraining of Transformers}, author = {Erik
-Nijkamp and Bo Pang and Ying Nian Wu and Caiming Xiong}, booktitle = {North
-American Chapter of the Association for Computational Linguistics}, year =
-{2021} } ``` ```bibtex @inproceedings{rogozhnikov2022einops, title = {Einops:
-Clear and Reliable Tensor Manipulations with Einstein-like Notation}, author =
-{Alex Rogozhnikov}, booktitle = {International Conference on Learning
-Representations}, year = {2022}, url = {https://openreview.net/
-forum?id=oapKSVM2bcj} } ```
+schedule = 'cosine' # currently the best schedule is cosine ) # get your pre-
+encoded codebook ids from the soundstream from a lot of raw audio codes =
+torch.randint(0, 1024, (2, 1024)) # do the below in a loop for a ton of data
+loss, _ = model(codes) loss.backward() # model can now generate in 18 steps. ~2
+seconds sounds reasonable generated = model.generate(1024, batch_size = 2) #
+(2, 1024) ``` To directly train on raw audio, you need to pass in your
+pretrained `SoundStream` into `SoundStorm`. You can train your own
+`SoundStream` at audiolm-pytorch. ```python import torch from
+soundstorm_pytorch import SoundStorm, ConformerWrapper, Conformer, SoundStream
+conformer = ConformerWrapper( codebook_size = 1024, num_quantizers = 4,
+conformer = dict( dim = 512, depth = 2 ), ) soundstream = SoundStream
+( codebook_size = 1024, rq_num_quantizers = 4, attn_window_size = 128,
+attn_depth = 2 ) model = SoundStorm( conformer, soundstream = soundstream #
+pass in the soundstream ) # find as much audio you'd like the model to learn
+audio = torch.randn(2, 10080) # course it through the model and take a
+gazillion tiny steps loss, _ = model(audio) loss.backward() # and now you can
+generate state-of-the-art speech generated_audio = model.generate(seconds = 30,
+batch_size = 2) # generate 30 seconds of audio (it will calculate the length in
+seconds based off the sampling frequency and cumulative downsamples in the
+soundstream passed in above) ``` ## Todo - [x] integrate soundstream - [x] when
+generating, and length can be defined in seconds (takes into sampling freq etc)
+- [ ] option to return list of audio files when generating - [ ] turn it into a
+command line tool - [ ] add cross attention and adaptive layernorm conditioning
+(just copy paste in the entire conformer repository, if conditioning adds too
+much cruft to the other repo) - [ ] make sure grouped rvq is supported. concat
+embeddings rather than sum across group dimension - [ ] trainer with accelerate
+## Citations ```bibtex @misc{borsos2023soundstorm, title = {SoundStorm:
+Efficient Parallel Audio Generation}, author = {ZalÃ¡n Borsos and Matt Sharifi
+and Damien Vincent and Eugene Kharitonov and Neil Zeghidour and Marco
+Tagliasacchi}, year = {2023}, eprint = {2305.09636}, archivePrefix = {arXiv},
+primaryClass = {cs.SD} } ``` ```bibtex @inproceedings{dao2022flashattention,
+title = {Flash{A}ttention: Fast and Memory-Efficient Exact Attention with {IO}-
+Awareness}, author = {Dao, Tri and Fu, Daniel Y. and Ermon, Stefano and Rudra,
+Atri and R{\'e}, Christopher}, booktitle = {Advances in Neural Information
+Processing Systems}, year = {2022} } ``` ```bibtex @article{Chang2022MaskGITMG,
+title = {MaskGIT: Masked Generative Image Transformer}, author = {Huiwen Chang
+and Han Zhang and Lu Jiang and Ce Liu and William T. Freeman}, journal = {2022
+IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)}, year =
+{2022}, pages = {11305-11315} } ``` ```bibtex @article{Lezama2022ImprovedMI,
+title = {Improved Masked Image Generation with Token-Critic}, author = {Jos
+{\'e} Lezama and Huiwen Chang and Lu Jiang and Irfan Essa}, journal = {ArXiv},
+year = {2022}, volume = {abs/2209.04439} } ``` ```bibtex @inproceedings
+{Nijkamp2021SCRIPTSP, title = {SCRIPT: Self-Critic PreTraining of
+Transformers}, author = {Erik Nijkamp and Bo Pang and Ying Nian Wu and Caiming
+Xiong}, booktitle = {North American Chapter of the Association for
+Computational Linguistics}, year = {2021} } ``` ```bibtex @inproceedings
+{rogozhnikov2022einops, title = {Einops: Clear and Reliable Tensor
+Manipulations with Einstein-like Notation}, author = {Alex Rogozhnikov},
+booktitle = {International Conference on Learning Representations}, year =
+{2022}, url = {https://openreview.net/forum?id=oapKSVM2bcj} } ```
```

### Comparing `soundstorm-pytorch-0.0.6/setup.py` & `soundstorm-pytorch-0.0.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'soundstorm-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.0.6',
+  version = '0.0.7',
   license='MIT',
   description = 'SoundStorm - Efficient Parallel Audio Generation from Google Deepmind, in Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/soundstorm-pytorch',
   keywords = [
```

### Comparing `soundstorm-pytorch-0.0.6/soundstorm_pytorch/attend.py` & `soundstorm-pytorch-0.0.7/soundstorm_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `soundstorm-pytorch-0.0.6/soundstorm_pytorch/soundstorm.py` & `soundstorm-pytorch-0.0.7/soundstorm_pytorch/soundstorm.py`

 * *Files 2% similar despite different names*

```diff
@@ -272,41 +272,49 @@
             self.token_critic = LogitHead(net, 1)
 
         self.critic_loss_weight = critic_loss_weight
 
     @torch.no_grad()
     def generate(
         self,
-        max_seq_len,
+        seq_len = None,
+        *,
+        seconds = None,
         batch_size = None,
         start_temperature = 1.,
         filter_thres = 0.7,
         noise_level_scale = 1.,
         **kwargs
     ):
+        assert exists(seq_len) ^ exists(seconds)
+
+        if not exists(seq_len):
+            assert exists(self.soundstream), 'soundstream must be passed in to generate in seconds'
+            seq_len = (seconds * self.soundstream.target_sample_hz) //  self.soundstream.seq_len_multiple_of
+
         sample_one = not exists(batch_size)
         batch_size = default(batch_size, 1)
 
         device = next(self.net.parameters()).device
 
         was_training = self.training
         self.eval()
 
         times = torch.linspace(0., 1., self.steps + 1)
 
         # sequence starts off as all masked
 
-        shape = (batch_size, max_seq_len)
+        shape = (batch_size, seq_len)
 
         seq = torch.full(shape, self.mask_id, device = device)
         mask = torch.full(shape, True, device = device)
 
         # slowly demask
 
-        all_mask_num_tokens = (self.schedule_fn(times[1:]) * max_seq_len).long()
+        all_mask_num_tokens = (self.schedule_fn(times[1:]) * seq_len).long()
 
         # self conditioning
 
         has_self_cond = self.self_cond
         last_embed = self.null_embed if has_self_cond else None
 
         for mask_num_tokens, steps_until_x0 in zip(all_mask_num_tokens.tolist(), reversed(range(self.steps))):
```

### Comparing `soundstorm-pytorch-0.0.6/soundstorm_pytorch.egg-info/PKG-INFO` & `soundstorm-pytorch-0.0.7/soundstorm_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soundstorm-pytorch
-Version: 0.0.6
+Version: 0.0.7
 Summary: SoundStorm - Efficient Parallel Audio Generation from Google Deepmind, in Pytorch
 Home-page: https://github.com/lucidrains/soundstorm-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```


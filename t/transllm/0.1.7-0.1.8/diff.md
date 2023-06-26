# Comparing `tmp/transllm-0.1.7.tar.gz` & `tmp/transllm-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transllm-0.1.7.tar", last modified: Sat Jun 24 15:10:35 2023, max compression
+gzip compressed data, was "transllm-0.1.8.tar", last modified: Mon Jun 26 19:31:43 2023, max compression
```

## Comparing `transllm-0.1.7.tar` & `transllm-0.1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 15:10:35.168963 transllm-0.1.7/
--rw-rw-rw-   0        0        0     1089 2023-06-23 08:54:28.000000 transllm-0.1.7/LICENSE
--rw-rw-rw-   0        0        0     8476 2023-06-24 15:10:35.167950 transllm-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     7537 2023-06-24 14:00:52.000000 transllm-0.1.7/README.md
--rw-rw-rw-   0        0        0       42 2023-06-24 15:10:35.168963 transllm-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     2035 2023-06-24 15:10:12.000000 transllm-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-24 15:10:35.149854 transllm-0.1.7/transllm/
--rw-rw-rw-   0        0        0      192 2023-06-24 15:10:18.000000 transllm-0.1.7/transllm/__init__.py
--rw-rw-rw-   0        0        0     3629 2023-06-24 15:02:32.000000 transllm-0.1.7/transllm/core.py
-drwxrwxrwx   0        0        0        0 2023-06-24 15:10:35.165277 transllm-0.1.7/transllm.egg-info/
--rw-rw-rw-   0        0        0     8476 2023-06-24 15:10:35.000000 transllm-0.1.7/transllm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-06-24 15:10:35.000000 transllm-0.1.7/transllm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 15:10:35.000000 transllm-0.1.7/transllm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-06-24 15:10:35.000000 transllm-0.1.7/transllm.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      122 2023-06-24 15:10:35.000000 transllm-0.1.7/transllm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-24 15:10:35.000000 transllm-0.1.7/transllm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 19:31:43.162720 transllm-0.1.8/
+-rw-rw-rw-   0        0        0     1089 2023-06-23 08:54:28.000000 transllm-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0    10521 2023-06-26 19:31:43.161718 transllm-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     9582 2023-06-26 18:51:05.000000 transllm-0.1.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-26 19:31:43.162720 transllm-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     2035 2023-06-26 19:31:39.000000 transllm-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 19:31:43.148718 transllm-0.1.8/transllm/
+-rw-rw-rw-   0        0        0      192 2023-06-26 19:31:41.000000 transllm-0.1.8/transllm/__init__.py
+-rw-rw-rw-   0        0        0     3926 2023-06-26 18:50:39.000000 transllm-0.1.8/transllm/core.py
+drwxrwxrwx   0        0        0        0 2023-06-26 19:31:43.159719 transllm-0.1.8/transllm.egg-info/
+-rw-rw-rw-   0        0        0    10521 2023-06-26 19:31:43.000000 transllm-0.1.8/transllm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-06-26 19:31:43.000000 transllm-0.1.8/transllm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 19:31:43.000000 transllm-0.1.8/transllm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-06-26 19:31:43.000000 transllm-0.1.8/transllm.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      122 2023-06-26 19:31:43.000000 transllm-0.1.8/transllm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-26 19:31:43.000000 transllm-0.1.8/transllm.egg-info/top_level.txt
```

### Comparing `transllm-0.1.7/LICENSE` & `transllm-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `transllm-0.1.7/PKG-INFO` & `transllm-0.1.8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transllm
-Version: 0.1.7
+Version: 0.1.8
 Summary: LLMtranslator translates and generates text in multiple languages.
 Home-page: https://github.com/dsdanielpark/hf-transllm
 Author: daniel park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Python,API,Bard,Google Bard,Large Language Model,Chatbot API,Google API,Chatbot
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -28,15 +28,15 @@
 <a><img alt="PyPI package" src="https://img.shields.io/badge/pypi-transllm-black"></a>
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 <a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2Fhf-transllm&count_bg=%23000000&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false"/></a>
 <a href="https://pypi.org/project/transllm/"><img alt="PyPI" src="https://img.shields.io/pypi/v/transllm"></a>
 </p>
 
 
-> LLMtranslator translates and generates text in multiple languages.
+> LLMtranslator translates and generates text in multiple languages using LLMs(Large Language Models) on hugging-face repository.
 
 ![](assets/transllm.png)
 
 ### Introducing hf-transllm: Unlock the Power of Multilingual Exploration
 
 Discover the hf-transllm package, a seamless integration of Hugging Face's inference module and translation APIs. Overcome limitations in retraining and evaluating large language models in different languages. Explore diverse results effortlessly, leveraging translation API services. Emphasizing versatility over efficiency, hf-transllm enables you to delve into the outcomes of Hugging Face's models in various languages.
 
@@ -53,81 +53,106 @@
 Or
 ```
 pip install git+https://github.com/dsdanielpark/hf-trnasllm.git
 ```
 
 <br>
 
-If you wish to use the various features and CLI:
+## CLI
+If you wish to use CLI:
 ```
-pip install git+https://github.com/dsdanielpark/hf-transllm.git
+git clone https://github.com/dsdanielpark/hf-transllm
 cd hf-transllm
 pip install -r requirements.txt
 ```
-There can be issues with various dependencies such as Hugging Face's Transformers, SentencePiece, Torch, and CUDA. Please set up the appropriate environment by searching online.
 ```bash
 python main.py --hfmodel <openlm-research/open_llama_3b> --lang <ko> --translator <google>
 ```
+There can be issues with various dependencies such as Hugging Face's Transformers, SentencePiece, Torch, and CUDA. Please set up the appropriate environment by searching online.
 <br>
 
 <br>
 
-## Usage 
-Applying LLMs to the majority of Hugging Face repositories is generally feasible. However, it can be challenging to apply them to objects that require unique tokenizers or inference processes. In such cases, it is recommended to customize the usage by incorporating a translation module for prompts.
+## Usage    
 
-In other words, if you are familiar with the inference process or code from Hugging Face repositories, you can customize the translation object by adding a translation module before and after the known inference process or code.
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1117ikGEmU4FncBDl1xCC2IhPPDOr75lX?usp=sharing) 
+> Simple Usage
+```python
+from transllm import LLMtranslator
+
+open_llama3b_kor = LLMtranslator('openlm-research/open_llama_3b', target_lang='ko', translator='google') # Korean
 
-Google Trnaslator
-- Support Languages: https://github.com/ssut/py-googletrans/blob/master/googletrans/constants.py
+trnaslated_answer = open_llama3b_kor.generate("나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘")
+print(trnaslated_answer)
+```
+<br>
+
+> Official Google Translation API
+- Support Languages: https://cloud.google.com/translate/docs/languages?hl=ko
+> Unofficial Google Trnaslator for non-profit purposes (such as feature testing)
+- Support Languages: https://github.com/nidhaloff/deep-translator/blob/master/deep_translator/constants.py
 ```python
 from transllm import LLMtranslator
 
 # Set huggingface repository
 model_path = 'openlm-research/open_llama_3b'
 # model_path = 'openlm-research/open_llama_7b'
 # model_path = 'openlm-research/open_llama_13b'
 
-# Get TransLLM Object
-open_llama3b_kor = LLMtranslator(model_path, target_lang='ko', translator='google')
+# Get TransLLM Object (Korean)
+# open_llama3b_kor = LLMtranslator(model_path, target_lang='ko', translator='google_official', google_api_key='xxxxxx') # Official Google Cloud Translation API 
+open_llama3b_kor = LLMtranslator(model_path, target_lang='ko', translator='google') # Unofficial test
+
+
 
 # Using Prompt in multi-language
 prompt = "나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘"
 trnaslated_answer = open_llama3b_kor.generate(prompt)
 print(trnaslated_answer)
 ```
 
 <br>
 
-DeepL
+> DeepL, Open AI, Bard
 - Support Languages: https://www.deepl.com/pro/select-country?cta=header-pro-button/#developer
 
 Open AI, Bard use pre-prompt for translation.
 ```python
 from transllm import LLMtranslator
 
 # Set huggingface repository
 model_path = 'openlm-research/open_llama_3b'
 # model_path = 'openlm-research/open_llama_7b'
 # model_path = 'openlm-research/open_llama_13b'
 
 # Choose Translate Service API: DeepL, OpenAI, Bard
-open_llama3b_kor = LLMtranslator(model_path, target_lang='EN', translator='deepl', deepl_api='xxxxxxx') 
+open_llama3b_kor = LLMtranslator(model_path, target_lang='ES', translator='deepl', deepl_api='xxxxxxx') # Language == Spanish
 # open_llama3b_kor = LLMtranslator(model_path, target_lang='korean', translator='openai', openai_api='xxxxxxx', openai_model='gpt-3.5-turbo')
 # open_llama3b_kor = LLMtranslator(model_path, target_lang='korean', translator='bard', bard_api='xxxxxxx')
 
 # Using Prompt in multi-language
 prompt = "나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘"
 trnaslated_answer = open_llama3b_kor.generate(prompt)
 print(trnaslated_answer)
 ```
 
 <br>
 
+
+> Google Colab Example
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1117ikGEmU4FncBDl1xCC2IhPPDOr75lX?usp=sharing) 
+![](assets/hf-transllm-colab.png)
+
+<br><br>
+
+
 ## Customized Inference
+Applying LLMs to the majority of Hugging Face repositories is generally feasible. However, it can be challenging to apply them to objects that require unique tokenizers or inference processes. In such cases, it is recommended to customize the usage by incorporating a translation module for prompts.
+
+In other words, if you are familiar with the inference process or code from Hugging Face repositories, you can customize the translation object by adding a translation module before and after the known inference process or code. Check [translang repository](https://github.com/dsdanielpark/translang) for more details.
 ```python
 import torch
 from trnasllm import LLMtranslator
 
 
 class MyLLMtranslator(LLMtranslator):
     def __init__(
@@ -162,14 +187,20 @@
 
         answer = customizing_process(prompt)
         # Custom inference logic...
         
         return answer
 ```
 
+<br>
+
+## About Google Translator
+Commercial use or official use of the Google Translate service is chargeable. Please provide the `translator="google_official"` and `google_api_key={YOUR_API_KEY}` arguments. Please responsibly use the `translator="google"` argument for the purpose of simple functionality verification. Refer to the following [notebook file](https://github.com/dsdanielpark/translang/blob/main/scripts/google_official.ipynb) and [official link](https://cloud.google.com/translate?utm_source=google&utm_medium=cpc&utm_campaign=japac-KR-all-en-dr-BKWS-all-mv-trial-EXA-dr-1605216&utm_content=text-ad-none-none-DEV_c-CRE_631260646738-ADGP_Hybrid%20%7C%20BKWS%20-%20EXA%20%7C%20Txt%20~%20AI%20&%20ML_Translation%20AI_google%20translate%20api_main-KWID_43700073965169292-kwd-14329410560&userloc_1009871-network_g&utm_term=KW_google%20translate%20api&gclid=Cj0KCQjwy9-kBhCHARIsAHpBjHjTvBCM7NNcf4fYGsog4ViQErgJvACFXB5JCNUT0h_EpQ5kyUT-SrIaApZBEALw_wcB&gclsrc=aw.ds&hl=ko) for more information. Use the google argument only for some basic functionality testing.
+
+
 ## [FAQs](./documents/FAQs.md)
 Use `Ctrl`+`F` for help in this `FAQs.md`.
 
 ## Contributors
 
 I would like to express my sincere gratitude for the contributions made by all the contributors.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: transllm Version: 0.1.7 Summary: LLMtranslator
+Metadata-Version: 2.1 Name: transllm Version: 0.1.8 Summary: LLMtranslator
 translates and generates text in multiple languages. Home-page: https://
 github.com/dsdanielpark/hf-transllm Author: daniel park Author-email:
 parkminwoo1991@gmail.com Keywords: Python,API,Bard,Google Bard,Large Language
 Model,Chatbot API,Google API,Chatbot Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Science/Research Classifier: Natural
 Language :: English Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
@@ -12,81 +12,111 @@
 Intelligence Requires-Python: >=3.6 Description-Content-Type: text/markdown
 License-File: LICENSE Development Status :: 3 - Alpha # Python Package: hf-
 transllm
 [PyPI package] [Code_style:_black] [https://hits.seeyoufarm.com/api/count/incr/
 badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2Fhf-
 transllm&count_bg=%23000000&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false]
 [PyPI]
-> LLMtranslator translates and generates text in multiple languages. ![]
-(assets/transllm.png) ### Introducing hf-transllm: Unlock the Power of
-Multilingual Exploration Discover the hf-transllm package, a seamless
-integration of Hugging Face's inference module and translation APIs. Overcome
-limitations in retraining and evaluating large language models in different
-languages. Explore diverse results effortlessly, leveraging translation API
-services. Emphasizing versatility over efficiency, hf-transllm enables you to
-delve into the outcomes of Hugging Face's models in various languages.
+> LLMtranslator translates and generates text in multiple languages using LLMs
+(Large Language Models) on hugging-face repository. ![](assets/transllm.png)
+### Introducing hf-transllm: Unlock the Power of Multilingual Exploration
+Discover the hf-transllm package, a seamless integration of Hugging Face's
+inference module and translation APIs. Overcome limitations in retraining and
+evaluating large language models in different languages. Explore diverse
+results effortlessly, leveraging translation API services. Emphasizing
+versatility over efficiency, hf-transllm enables you to delve into the outcomes
+of Hugging Face's models in various languages.
 
 ## Installation ``` pip install transllm ``` Or ``` pip install git+https://
 github.com/dsdanielpark/hf-trnasllm.git ```
-If you wish to use the various features and CLI: ``` pip install git+https://
-github.com/dsdanielpark/hf-transllm.git cd hf-transllm pip install -
-r requirements.txt ``` There can be issues with various dependencies such as
-Hugging Face's Transformers, SentencePiece, Torch, and CUDA. Please set up the
-appropriate environment by searching online. ```bash python main.py --hfmodel
-pen_llama_3b> --lang  --translator  ```
+## CLI If you wish to use CLI: ``` git clone https://github.com/dsdanielpark/
+hf-transllm cd hf-transllm pip install -r requirements.txt ``` ```bash python
+main.py --hfmodel
+pen_llama_3b> --lang  --translator  ``` There can be issues with various
+dependencies such as Hugging Face's Transformers, SentencePiece, Torch, and
+CUDA. Please set up the appropriate environment by searching online.
 
-## Usage Applying LLMs to the majority of Hugging Face repositories is
-generally feasible. However, it can be challenging to apply them to objects
-that require unique tokenizers or inference processes. In such cases, it is
-recommended to customize the usage by incorporating a translation module for
-prompts. In other words, if you are familiar with the inference process or code
-from Hugging Face repositories, you can customize the translation object by
-adding a translation module before and after the known inference process or
-code. [![Open In Colab](https://colab.research.google.com/assets/colab-
-badge.svg)](https://colab.research.google.com/drive/
-1117ikGEmU4FncBDl1xCC2IhPPDOr75lX?usp=sharing) Google Trnaslator - Support
-Languages: https://github.com/ssut/py-googletrans/blob/master/googletrans/
-constants.py ```python from transllm import LLMtranslator # Set huggingface
+## Usage > Simple Usage ```python from transllm import LLMtranslator
+open_llama3b_kor = LLMtranslator('openlm-research/open_llama_3b',
+target_lang='ko', translator='google') # Korean trnaslated_answer =
+open_llama3b_kor.generate("ëì ë´ ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì
+ëí´ì ìë ¤ì¤") print(trnaslated_answer) ```
+> Official Google Translation API - Support Languages: https://
+cloud.google.com/translate/docs/languages?hl=ko > Unofficial Google Trnaslator
+for non-profit purposes (such as feature testing) - Support Languages: https://
+github.com/nidhaloff/deep-translator/blob/master/deep_translator/constants.py
+```python from transllm import LLMtranslator # Set huggingface repository
+model_path = 'openlm-research/open_llama_3b' # model_path = 'openlm-research/
+open_llama_7b' # model_path = 'openlm-research/open_llama_13b' # Get TransLLM
+Object (Korean) # open_llama3b_kor = LLMtranslator(model_path,
+target_lang='ko', translator='google_official', google_api_key='xxxxxx') #
+Official Google Cloud Translation API open_llama3b_kor = LLMtranslator
+(model_path, target_lang='ko', translator='google') # Unofficial test # Using
+Prompt in multi-language prompt = "ëì ë´ ëëë°°ë¤ì´ ì¢ìíë
+ë´ì§ì¤ì ëí´ì ìë ¤ì¤" trnaslated_answer = open_llama3b_kor.generate
+(prompt) print(trnaslated_answer) ```
+> DeepL, Open AI, Bard - Support Languages: https://www.deepl.com/pro/select-
+country?cta=header-pro-button/#developer Open AI, Bard use pre-prompt for
+translation. ```python from transllm import LLMtranslator # Set huggingface
 repository model_path = 'openlm-research/open_llama_3b' # model_path = 'openlm-
-research/open_llama_7b' # model_path = 'openlm-research/open_llama_13b' # Get
-TransLLM Object open_llama3b_kor = LLMtranslator(model_path, target_lang='ko',
-translator='google') # Using Prompt in multi-language prompt = "ëì ë´
-ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì ìë ¤ì¤"
-trnaslated_answer = open_llama3b_kor.generate(prompt) print(trnaslated_answer)
-```
-DeepL - Support Languages: https://www.deepl.com/pro/select-country?cta=header-
-pro-button/#developer Open AI, Bard use pre-prompt for translation. ```python
-from transllm import LLMtranslator # Set huggingface repository model_path =
-'openlm-research/open_llama_3b' # model_path = 'openlm-research/open_llama_7b'
-# model_path = 'openlm-research/open_llama_13b' # Choose Translate Service API:
-DeepL, OpenAI, Bard open_llama3b_kor = LLMtranslator(model_path,
-target_lang='EN', translator='deepl', deepl_api='xxxxxxx') # open_llama3b_kor =
-LLMtranslator(model_path, target_lang='korean', translator='openai',
-openai_api='xxxxxxx', openai_model='gpt-3.5-turbo') # open_llama3b_kor =
-LLMtranslator(model_path, target_lang='korean', translator='bard',
-bard_api='xxxxxxx') # Using Prompt in multi-language prompt = "ëì ë´
-ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì ìë ¤ì¤"
-trnaslated_answer = open_llama3b_kor.generate(prompt) print(trnaslated_answer)
-```
-## Customized Inference ```python import torch from trnasllm import
-LLMtranslator class MyLLMtranslator(LLMtranslator): def __init__( self,
+research/open_llama_7b' # model_path = 'openlm-research/open_llama_13b' #
+Choose Translate Service API: DeepL, OpenAI, Bard open_llama3b_kor =
+LLMtranslator(model_path, target_lang='ES', translator='deepl',
+deepl_api='xxxxxxx') # Language == Spanish # open_llama3b_kor = LLMtranslator
+(model_path, target_lang='korean', translator='openai', openai_api='xxxxxxx',
+openai_model='gpt-3.5-turbo') # open_llama3b_kor = LLMtranslator(model_path,
+target_lang='korean', translator='bard', bard_api='xxxxxxx') # Using Prompt in
+multi-language prompt = "ëì ë´ ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì
+ëí´ì ìë ¤ì¤" trnaslated_answer = open_llama3b_kor.generate(prompt)
+print(trnaslated_answer) ```
+> Google Colab Example [![Open In Colab](https://colab.research.google.com/
+assets/colab-badge.svg)](https://colab.research.google.com/drive/
+1117ikGEmU4FncBDl1xCC2IhPPDOr75lX?usp=sharing) ![](assets/hf-transllm-
+colab.png)
+
+## Customized Inference Applying LLMs to the majority of Hugging Face
+repositories is generally feasible. However, it can be challenging to apply
+them to objects that require unique tokenizers or inference processes. In such
+cases, it is recommended to customize the usage by incorporating a translation
+module for prompts. In other words, if you are familiar with the inference
+process or code from Hugging Face repositories, you can customize the
+translation object by adding a translation module before and after the known
+inference process or code. Check [translang repository](https://github.com/
+dsdanielpark/translang) for more details. ```python import torch from trnasllm
+import LLMtranslator class MyLLMtranslator(LLMtranslator): def __init__( self,
 model_path, target_lang="ko", translator="google", torch_dtype=torch.float16,
 device_map="auto", deepl_api=None, bard_api=None, openai_model="gpt-3.5-turbo",
 openai_api=None ): super().__init__( model_path=model_path,
 target_lang=target_lang, translator=translator, torch_dtype=torch_dtype,
 device_map=device_map, deepl_api=deepl_api, bard_api=bard_api,
 openai_model=openai_model, openai_api=openai_api ) def inference(self, prompt:
 str) -> str: # Custom logic for inference # You can override the implementation
 of the inference method here # and provide your own logic for generating the
 translated answer # Remember to return the translated answer as a string.
 answer = customizing_process(prompt) # Custom inference logic... return answer
-``` ## [FAQs](./documents/FAQs.md) Use `Ctrl`+`F` for help in this `FAQs.md`.
-## Contributors I would like to express my sincere gratitude for the
-contributions made by all the contributors. [https://contrib.rocks/
-image?repo=dsdanielpark/hf-transllm]
+```
+## About Google Translator Commercial use or official use of the Google
+Translate service is chargeable. Please provide the
+`translator="google_official"` and `google_api_key={YOUR_API_KEY}` arguments.
+Please responsibly use the `translator="google"` argument for the purpose of
+simple functionality verification. Refer to the following [notebook file]
+(https://github.com/dsdanielpark/translang/blob/main/scripts/
+google_official.ipynb) and [official link](https://cloud.google.com/
+translate?utm_source=google&utm_medium=cpc&utm_campaign=japac-KR-all-en-dr-
+BKWS-all-mv-trial-EXA-dr-1605216&utm_content=text-ad-none-none-DEV_c-
+CRE_631260646738-ADGP_Hybrid%20%7C%20BKWS%20-
+%20EXA%20%7C%20Txt%20~%20AI%20&%20ML_Translation%20AI_google%20translate%20api_main-
+KWID_43700073965169292-kwd-14329410560&userloc_1009871-
+network_g&utm_term=KW_google%20translate%20api&gclid=Cj0KCQjwy9-
+kBhCHARIsAHpBjHjTvBCM7NNcf4fYGsog4ViQErgJvACFXB5JCNUT0h_EpQ5kyUT-
+SrIaApZBEALw_wcB&gclsrc=aw.ds&hl=ko) for more information. Use the google
+argument only for some basic functionality testing. ## [FAQs](./documents/
+FAQs.md) Use `Ctrl`+`F` for help in this `FAQs.md`. ## Contributors I would
+like to express my sincere gratitude for the contributions made by all the
+contributors. [https://contrib.rocks/image?repo=dsdanielpark/hf-transllm]
 ## License [MIT](https://opensource.org/license/mit/)
 I hold no legal responsibility; ``` The MIT License (MIT) Copyright (c) 2023
 Minwoo Park Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including without
 limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom
```

### Comparing `transllm-0.1.7/README.md` & `transllm-0.1.8/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 <a><img alt="PyPI package" src="https://img.shields.io/badge/pypi-transllm-black"></a>
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 <a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2Fhf-transllm&count_bg=%23000000&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false"/></a>
 <a href="https://pypi.org/project/transllm/"><img alt="PyPI" src="https://img.shields.io/pypi/v/transllm"></a>
 </p>
 
 
-> LLMtranslator translates and generates text in multiple languages.
+> LLMtranslator translates and generates text in multiple languages using LLMs(Large Language Models) on hugging-face repository.
 
 ![](assets/transllm.png)
 
 ### Introducing hf-transllm: Unlock the Power of Multilingual Exploration
 
 Discover the hf-transllm package, a seamless integration of Hugging Face's inference module and translation APIs. Overcome limitations in retraining and evaluating large language models in different languages. Explore diverse results effortlessly, leveraging translation API services. Emphasizing versatility over efficiency, hf-transllm enables you to delve into the outcomes of Hugging Face's models in various languages.
 
@@ -31,81 +31,106 @@
 Or
 ```
 pip install git+https://github.com/dsdanielpark/hf-trnasllm.git
 ```
 
 <br>
 
-If you wish to use the various features and CLI:
+## CLI
+If you wish to use CLI:
 ```
-pip install git+https://github.com/dsdanielpark/hf-transllm.git
+git clone https://github.com/dsdanielpark/hf-transllm
 cd hf-transllm
 pip install -r requirements.txt
 ```
-There can be issues with various dependencies such as Hugging Face's Transformers, SentencePiece, Torch, and CUDA. Please set up the appropriate environment by searching online.
 ```bash
 python main.py --hfmodel <openlm-research/open_llama_3b> --lang <ko> --translator <google>
 ```
+There can be issues with various dependencies such as Hugging Face's Transformers, SentencePiece, Torch, and CUDA. Please set up the appropriate environment by searching online.
 <br>
 
 <br>
 
-## Usage 
-Applying LLMs to the majority of Hugging Face repositories is generally feasible. However, it can be challenging to apply them to objects that require unique tokenizers or inference processes. In such cases, it is recommended to customize the usage by incorporating a translation module for prompts.
+## Usage    
 
-In other words, if you are familiar with the inference process or code from Hugging Face repositories, you can customize the translation object by adding a translation module before and after the known inference process or code.
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1117ikGEmU4FncBDl1xCC2IhPPDOr75lX?usp=sharing) 
+> Simple Usage
+```python
+from transllm import LLMtranslator
+
+open_llama3b_kor = LLMtranslator('openlm-research/open_llama_3b', target_lang='ko', translator='google') # Korean
 
-Google Trnaslator
-- Support Languages: https://github.com/ssut/py-googletrans/blob/master/googletrans/constants.py
+trnaslated_answer = open_llama3b_kor.generate("나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘")
+print(trnaslated_answer)
+```
+<br>
+
+> Official Google Translation API
+- Support Languages: https://cloud.google.com/translate/docs/languages?hl=ko
+> Unofficial Google Trnaslator for non-profit purposes (such as feature testing)
+- Support Languages: https://github.com/nidhaloff/deep-translator/blob/master/deep_translator/constants.py
 ```python
 from transllm import LLMtranslator
 
 # Set huggingface repository
 model_path = 'openlm-research/open_llama_3b'
 # model_path = 'openlm-research/open_llama_7b'
 # model_path = 'openlm-research/open_llama_13b'
 
-# Get TransLLM Object
-open_llama3b_kor = LLMtranslator(model_path, target_lang='ko', translator='google')
+# Get TransLLM Object (Korean)
+# open_llama3b_kor = LLMtranslator(model_path, target_lang='ko', translator='google_official', google_api_key='xxxxxx') # Official Google Cloud Translation API 
+open_llama3b_kor = LLMtranslator(model_path, target_lang='ko', translator='google') # Unofficial test
+
+
 
 # Using Prompt in multi-language
 prompt = "나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘"
 trnaslated_answer = open_llama3b_kor.generate(prompt)
 print(trnaslated_answer)
 ```
 
 <br>
 
-DeepL
+> DeepL, Open AI, Bard
 - Support Languages: https://www.deepl.com/pro/select-country?cta=header-pro-button/#developer
 
 Open AI, Bard use pre-prompt for translation.
 ```python
 from transllm import LLMtranslator
 
 # Set huggingface repository
 model_path = 'openlm-research/open_llama_3b'
 # model_path = 'openlm-research/open_llama_7b'
 # model_path = 'openlm-research/open_llama_13b'
 
 # Choose Translate Service API: DeepL, OpenAI, Bard
-open_llama3b_kor = LLMtranslator(model_path, target_lang='EN', translator='deepl', deepl_api='xxxxxxx') 
+open_llama3b_kor = LLMtranslator(model_path, target_lang='ES', translator='deepl', deepl_api='xxxxxxx') # Language == Spanish
 # open_llama3b_kor = LLMtranslator(model_path, target_lang='korean', translator='openai', openai_api='xxxxxxx', openai_model='gpt-3.5-turbo')
 # open_llama3b_kor = LLMtranslator(model_path, target_lang='korean', translator='bard', bard_api='xxxxxxx')
 
 # Using Prompt in multi-language
 prompt = "나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘"
 trnaslated_answer = open_llama3b_kor.generate(prompt)
 print(trnaslated_answer)
 ```
 
 <br>
 
+
+> Google Colab Example
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1117ikGEmU4FncBDl1xCC2IhPPDOr75lX?usp=sharing) 
+![](assets/hf-transllm-colab.png)
+
+<br><br>
+
+
 ## Customized Inference
+Applying LLMs to the majority of Hugging Face repositories is generally feasible. However, it can be challenging to apply them to objects that require unique tokenizers or inference processes. In such cases, it is recommended to customize the usage by incorporating a translation module for prompts.
+
+In other words, if you are familiar with the inference process or code from Hugging Face repositories, you can customize the translation object by adding a translation module before and after the known inference process or code. Check [translang repository](https://github.com/dsdanielpark/translang) for more details.
 ```python
 import torch
 from trnasllm import LLMtranslator
 
 
 class MyLLMtranslator(LLMtranslator):
     def __init__(
@@ -140,14 +165,20 @@
 
         answer = customizing_process(prompt)
         # Custom inference logic...
         
         return answer
 ```
 
+<br>
+
+## About Google Translator
+Commercial use or official use of the Google Translate service is chargeable. Please provide the `translator="google_official"` and `google_api_key={YOUR_API_KEY}` arguments. Please responsibly use the `translator="google"` argument for the purpose of simple functionality verification. Refer to the following [notebook file](https://github.com/dsdanielpark/translang/blob/main/scripts/google_official.ipynb) and [official link](https://cloud.google.com/translate?utm_source=google&utm_medium=cpc&utm_campaign=japac-KR-all-en-dr-BKWS-all-mv-trial-EXA-dr-1605216&utm_content=text-ad-none-none-DEV_c-CRE_631260646738-ADGP_Hybrid%20%7C%20BKWS%20-%20EXA%20%7C%20Txt%20~%20AI%20&%20ML_Translation%20AI_google%20translate%20api_main-KWID_43700073965169292-kwd-14329410560&userloc_1009871-network_g&utm_term=KW_google%20translate%20api&gclid=Cj0KCQjwy9-kBhCHARIsAHpBjHjTvBCM7NNcf4fYGsog4ViQErgJvACFXB5JCNUT0h_EpQ5kyUT-SrIaApZBEALw_wcB&gclsrc=aw.ds&hl=ko) for more information. Use the google argument only for some basic functionality testing.
+
+
 ## [FAQs](./documents/FAQs.md)
 Use `Ctrl`+`F` for help in this `FAQs.md`.
 
 ## Contributors
 
 I would like to express my sincere gratitude for the contributions made by all the contributors.
```

#### html2text {}

```diff
@@ -1,79 +1,109 @@
 Development Status :: 3 - Alpha # Python Package: hf-transllm
 [PyPI package] [Code_style:_black] [https://hits.seeyoufarm.com/api/count/incr/
 badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2Fhf-
 transllm&count_bg=%23000000&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false]
 [PyPI]
-> LLMtranslator translates and generates text in multiple languages. ![]
-(assets/transllm.png) ### Introducing hf-transllm: Unlock the Power of
-Multilingual Exploration Discover the hf-transllm package, a seamless
-integration of Hugging Face's inference module and translation APIs. Overcome
-limitations in retraining and evaluating large language models in different
-languages. Explore diverse results effortlessly, leveraging translation API
-services. Emphasizing versatility over efficiency, hf-transllm enables you to
-delve into the outcomes of Hugging Face's models in various languages.
+> LLMtranslator translates and generates text in multiple languages using LLMs
+(Large Language Models) on hugging-face repository. ![](assets/transllm.png)
+### Introducing hf-transllm: Unlock the Power of Multilingual Exploration
+Discover the hf-transllm package, a seamless integration of Hugging Face's
+inference module and translation APIs. Overcome limitations in retraining and
+evaluating large language models in different languages. Explore diverse
+results effortlessly, leveraging translation API services. Emphasizing
+versatility over efficiency, hf-transllm enables you to delve into the outcomes
+of Hugging Face's models in various languages.
 
 ## Installation ``` pip install transllm ``` Or ``` pip install git+https://
 github.com/dsdanielpark/hf-trnasllm.git ```
-If you wish to use the various features and CLI: ``` pip install git+https://
-github.com/dsdanielpark/hf-transllm.git cd hf-transllm pip install -
-r requirements.txt ``` There can be issues with various dependencies such as
-Hugging Face's Transformers, SentencePiece, Torch, and CUDA. Please set up the
-appropriate environment by searching online. ```bash python main.py --hfmodel
-pen_llama_3b> --lang  --translator  ```
+## CLI If you wish to use CLI: ``` git clone https://github.com/dsdanielpark/
+hf-transllm cd hf-transllm pip install -r requirements.txt ``` ```bash python
+main.py --hfmodel
+pen_llama_3b> --lang  --translator  ``` There can be issues with various
+dependencies such as Hugging Face's Transformers, SentencePiece, Torch, and
+CUDA. Please set up the appropriate environment by searching online.
 
-## Usage Applying LLMs to the majority of Hugging Face repositories is
-generally feasible. However, it can be challenging to apply them to objects
-that require unique tokenizers or inference processes. In such cases, it is
-recommended to customize the usage by incorporating a translation module for
-prompts. In other words, if you are familiar with the inference process or code
-from Hugging Face repositories, you can customize the translation object by
-adding a translation module before and after the known inference process or
-code. [![Open In Colab](https://colab.research.google.com/assets/colab-
-badge.svg)](https://colab.research.google.com/drive/
-1117ikGEmU4FncBDl1xCC2IhPPDOr75lX?usp=sharing) Google Trnaslator - Support
-Languages: https://github.com/ssut/py-googletrans/blob/master/googletrans/
-constants.py ```python from transllm import LLMtranslator # Set huggingface
+## Usage > Simple Usage ```python from transllm import LLMtranslator
+open_llama3b_kor = LLMtranslator('openlm-research/open_llama_3b',
+target_lang='ko', translator='google') # Korean trnaslated_answer =
+open_llama3b_kor.generate("ëì ë´ ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì
+ëí´ì ìë ¤ì¤") print(trnaslated_answer) ```
+> Official Google Translation API - Support Languages: https://
+cloud.google.com/translate/docs/languages?hl=ko > Unofficial Google Trnaslator
+for non-profit purposes (such as feature testing) - Support Languages: https://
+github.com/nidhaloff/deep-translator/blob/master/deep_translator/constants.py
+```python from transllm import LLMtranslator # Set huggingface repository
+model_path = 'openlm-research/open_llama_3b' # model_path = 'openlm-research/
+open_llama_7b' # model_path = 'openlm-research/open_llama_13b' # Get TransLLM
+Object (Korean) # open_llama3b_kor = LLMtranslator(model_path,
+target_lang='ko', translator='google_official', google_api_key='xxxxxx') #
+Official Google Cloud Translation API open_llama3b_kor = LLMtranslator
+(model_path, target_lang='ko', translator='google') # Unofficial test # Using
+Prompt in multi-language prompt = "ëì ë´ ëëë°°ë¤ì´ ì¢ìíë
+ë´ì§ì¤ì ëí´ì ìë ¤ì¤" trnaslated_answer = open_llama3b_kor.generate
+(prompt) print(trnaslated_answer) ```
+> DeepL, Open AI, Bard - Support Languages: https://www.deepl.com/pro/select-
+country?cta=header-pro-button/#developer Open AI, Bard use pre-prompt for
+translation. ```python from transllm import LLMtranslator # Set huggingface
 repository model_path = 'openlm-research/open_llama_3b' # model_path = 'openlm-
-research/open_llama_7b' # model_path = 'openlm-research/open_llama_13b' # Get
-TransLLM Object open_llama3b_kor = LLMtranslator(model_path, target_lang='ko',
-translator='google') # Using Prompt in multi-language prompt = "ëì ë´
-ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì ìë ¤ì¤"
-trnaslated_answer = open_llama3b_kor.generate(prompt) print(trnaslated_answer)
-```
-DeepL - Support Languages: https://www.deepl.com/pro/select-country?cta=header-
-pro-button/#developer Open AI, Bard use pre-prompt for translation. ```python
-from transllm import LLMtranslator # Set huggingface repository model_path =
-'openlm-research/open_llama_3b' # model_path = 'openlm-research/open_llama_7b'
-# model_path = 'openlm-research/open_llama_13b' # Choose Translate Service API:
-DeepL, OpenAI, Bard open_llama3b_kor = LLMtranslator(model_path,
-target_lang='EN', translator='deepl', deepl_api='xxxxxxx') # open_llama3b_kor =
-LLMtranslator(model_path, target_lang='korean', translator='openai',
-openai_api='xxxxxxx', openai_model='gpt-3.5-turbo') # open_llama3b_kor =
-LLMtranslator(model_path, target_lang='korean', translator='bard',
-bard_api='xxxxxxx') # Using Prompt in multi-language prompt = "ëì ë´
-ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì ìë ¤ì¤"
-trnaslated_answer = open_llama3b_kor.generate(prompt) print(trnaslated_answer)
-```
-## Customized Inference ```python import torch from trnasllm import
-LLMtranslator class MyLLMtranslator(LLMtranslator): def __init__( self,
+research/open_llama_7b' # model_path = 'openlm-research/open_llama_13b' #
+Choose Translate Service API: DeepL, OpenAI, Bard open_llama3b_kor =
+LLMtranslator(model_path, target_lang='ES', translator='deepl',
+deepl_api='xxxxxxx') # Language == Spanish # open_llama3b_kor = LLMtranslator
+(model_path, target_lang='korean', translator='openai', openai_api='xxxxxxx',
+openai_model='gpt-3.5-turbo') # open_llama3b_kor = LLMtranslator(model_path,
+target_lang='korean', translator='bard', bard_api='xxxxxxx') # Using Prompt in
+multi-language prompt = "ëì ë´ ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì
+ëí´ì ìë ¤ì¤" trnaslated_answer = open_llama3b_kor.generate(prompt)
+print(trnaslated_answer) ```
+> Google Colab Example [![Open In Colab](https://colab.research.google.com/
+assets/colab-badge.svg)](https://colab.research.google.com/drive/
+1117ikGEmU4FncBDl1xCC2IhPPDOr75lX?usp=sharing) ![](assets/hf-transllm-
+colab.png)
+
+## Customized Inference Applying LLMs to the majority of Hugging Face
+repositories is generally feasible. However, it can be challenging to apply
+them to objects that require unique tokenizers or inference processes. In such
+cases, it is recommended to customize the usage by incorporating a translation
+module for prompts. In other words, if you are familiar with the inference
+process or code from Hugging Face repositories, you can customize the
+translation object by adding a translation module before and after the known
+inference process or code. Check [translang repository](https://github.com/
+dsdanielpark/translang) for more details. ```python import torch from trnasllm
+import LLMtranslator class MyLLMtranslator(LLMtranslator): def __init__( self,
 model_path, target_lang="ko", translator="google", torch_dtype=torch.float16,
 device_map="auto", deepl_api=None, bard_api=None, openai_model="gpt-3.5-turbo",
 openai_api=None ): super().__init__( model_path=model_path,
 target_lang=target_lang, translator=translator, torch_dtype=torch_dtype,
 device_map=device_map, deepl_api=deepl_api, bard_api=bard_api,
 openai_model=openai_model, openai_api=openai_api ) def inference(self, prompt:
 str) -> str: # Custom logic for inference # You can override the implementation
 of the inference method here # and provide your own logic for generating the
 translated answer # Remember to return the translated answer as a string.
 answer = customizing_process(prompt) # Custom inference logic... return answer
-``` ## [FAQs](./documents/FAQs.md) Use `Ctrl`+`F` for help in this `FAQs.md`.
-## Contributors I would like to express my sincere gratitude for the
-contributions made by all the contributors. [https://contrib.rocks/
-image?repo=dsdanielpark/hf-transllm]
+```
+## About Google Translator Commercial use or official use of the Google
+Translate service is chargeable. Please provide the
+`translator="google_official"` and `google_api_key={YOUR_API_KEY}` arguments.
+Please responsibly use the `translator="google"` argument for the purpose of
+simple functionality verification. Refer to the following [notebook file]
+(https://github.com/dsdanielpark/translang/blob/main/scripts/
+google_official.ipynb) and [official link](https://cloud.google.com/
+translate?utm_source=google&utm_medium=cpc&utm_campaign=japac-KR-all-en-dr-
+BKWS-all-mv-trial-EXA-dr-1605216&utm_content=text-ad-none-none-DEV_c-
+CRE_631260646738-ADGP_Hybrid%20%7C%20BKWS%20-
+%20EXA%20%7C%20Txt%20~%20AI%20&%20ML_Translation%20AI_google%20translate%20api_main-
+KWID_43700073965169292-kwd-14329410560&userloc_1009871-
+network_g&utm_term=KW_google%20translate%20api&gclid=Cj0KCQjwy9-
+kBhCHARIsAHpBjHjTvBCM7NNcf4fYGsog4ViQErgJvACFXB5JCNUT0h_EpQ5kyUT-
+SrIaApZBEALw_wcB&gclsrc=aw.ds&hl=ko) for more information. Use the google
+argument only for some basic functionality testing. ## [FAQs](./documents/
+FAQs.md) Use `Ctrl`+`F` for help in this `FAQs.md`. ## Contributors I would
+like to express my sincere gratitude for the contributions made by all the
+contributors. [https://contrib.rocks/image?repo=dsdanielpark/hf-transllm]
 ## License [MIT](https://opensource.org/license/mit/)
 I hold no legal responsibility; ``` The MIT License (MIT) Copyright (c) 2023
 Minwoo Park Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including without
 limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom
```

### Comparing `transllm-0.1.7/setup.py` & `transllm-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 version = get_version()
 
 
 setup(
     name="transllm",
-    version="0.1.7",
+    version="0.1.8",
     author="daniel park",
     author_email="parkminwoo1991@gmail.com",
     description="LLMtranslator translates and generates text in multiple languages.",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/dsdanielpark/hf-transllm",
     packages=find_packages(exclude=[]),
```

### Comparing `transllm-0.1.7/transllm/core.py` & `transllm-0.1.8/transllm/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,39 +6,41 @@
 class LLMtranslator(TranslationService):
     """
     LLMtranslator is a translation service based on the Llama language model.
     It extends the TranslationService class and provides translation functionality using Llama.
 
     Args:
         model_path (str): The path to the Llama model.
-        target_lang (str, optional): The target language for translation (default: "ko").
+        target_lang (str, optional): The target language for translation (default: "en").
         translator (str, optional): The translation service to use (default: "google").
         torch_dtype (torch.dtype, optional): The data type for torch (default: torch.float16).
         device_map (str, optional): The device map for torch (default: "auto").
         deepl_api_key (str, optional): DeepL API key (if required).
         bard_api_key (str, optional): Bard API key (if required).
         openai_model (str, optional): OpenAI model name (default: "gpt-3.5-turbo").
         openai_api_key (str, optional): OpenAI API key (if required).
     """
 
     def __init__(
         self,
         model_path,
-        target_lang="ko",
+        target_lang="en",
         translator="google",
         torch_dtype=torch.float16,
         offload_folder=None,
         device_map="auto",
+        google_api_key=None,
         deepl_api_key=None,
         bard_api_key=None,
         openai_api_key=None,
         openai_model="gpt-3.5-turbo",
     ):
         super().__init__(
             translator=translator,
+            google_api_key=google_api_key,
             deepl_api_key=deepl_api_key,
             bard_api_key=bard_api_key,
             openai_api_key=openai_api_key,
             openai_model=openai_model,
         )
         self.model_path = model_path
         self.target_lang = target_lang
@@ -79,26 +81,31 @@
         Args:
             prompt (str): The prompt text.
 
         Returns:
             str: The translated answer.
         """
         input_ids = self.tokenizer(prompt, return_tensors="pt").input_ids
+        
+        # Different from this class's generate method is the generate method of the Hugging Face model.
         with torch.no_grad():
-            generation_output = self.model.generate(input_ids=input_ids, max_length=32)
+            generation_output = self.model.generate(input_ids=input_ids, max_length=32) 
         answer = self.tokenizer.decode(generation_output[0])
         return answer
 
     def generate(self, prompt: str) -> str:
         """
         Generates the translated answer for the given prompt.
 
         Args:
             prompt (str): The prompt text.
 
         Returns:
             str: The translated answer.
         """
-        translated_prompt = self.process_prompt(prompt)
-        answer = self.inference(translated_prompt)
-        translated_answer = self.process_answer(answer)
+        if self.target_lang =='en':
+            return self.inference(prompt)
+        else:
+            translated_prompt = self.process_prompt(prompt)
+            answer = self.inference(translated_prompt)
+            translated_answer = self.process_answer(answer)
         return translated_answer
```

### Comparing `transllm-0.1.7/transllm.egg-info/PKG-INFO` & `transllm-0.1.8/transllm.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transllm
-Version: 0.1.7
+Version: 0.1.8
 Summary: LLMtranslator translates and generates text in multiple languages.
 Home-page: https://github.com/dsdanielpark/hf-transllm
 Author: daniel park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Python,API,Bard,Google Bard,Large Language Model,Chatbot API,Google API,Chatbot
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -28,15 +28,15 @@
 <a><img alt="PyPI package" src="https://img.shields.io/badge/pypi-transllm-black"></a>
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 <a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2Fhf-transllm&count_bg=%23000000&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false"/></a>
 <a href="https://pypi.org/project/transllm/"><img alt="PyPI" src="https://img.shields.io/pypi/v/transllm"></a>
 </p>
 
 
-> LLMtranslator translates and generates text in multiple languages.
+> LLMtranslator translates and generates text in multiple languages using LLMs(Large Language Models) on hugging-face repository.
 
 ![](assets/transllm.png)
 
 ### Introducing hf-transllm: Unlock the Power of Multilingual Exploration
 
 Discover the hf-transllm package, a seamless integration of Hugging Face's inference module and translation APIs. Overcome limitations in retraining and evaluating large language models in different languages. Explore diverse results effortlessly, leveraging translation API services. Emphasizing versatility over efficiency, hf-transllm enables you to delve into the outcomes of Hugging Face's models in various languages.
 
@@ -53,81 +53,106 @@
 Or
 ```
 pip install git+https://github.com/dsdanielpark/hf-trnasllm.git
 ```
 
 <br>
 
-If you wish to use the various features and CLI:
+## CLI
+If you wish to use CLI:
 ```
-pip install git+https://github.com/dsdanielpark/hf-transllm.git
+git clone https://github.com/dsdanielpark/hf-transllm
 cd hf-transllm
 pip install -r requirements.txt
 ```
-There can be issues with various dependencies such as Hugging Face's Transformers, SentencePiece, Torch, and CUDA. Please set up the appropriate environment by searching online.
 ```bash
 python main.py --hfmodel <openlm-research/open_llama_3b> --lang <ko> --translator <google>
 ```
+There can be issues with various dependencies such as Hugging Face's Transformers, SentencePiece, Torch, and CUDA. Please set up the appropriate environment by searching online.
 <br>
 
 <br>
 
-## Usage 
-Applying LLMs to the majority of Hugging Face repositories is generally feasible. However, it can be challenging to apply them to objects that require unique tokenizers or inference processes. In such cases, it is recommended to customize the usage by incorporating a translation module for prompts.
+## Usage    
 
-In other words, if you are familiar with the inference process or code from Hugging Face repositories, you can customize the translation object by adding a translation module before and after the known inference process or code.
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1117ikGEmU4FncBDl1xCC2IhPPDOr75lX?usp=sharing) 
+> Simple Usage
+```python
+from transllm import LLMtranslator
+
+open_llama3b_kor = LLMtranslator('openlm-research/open_llama_3b', target_lang='ko', translator='google') # Korean
 
-Google Trnaslator
-- Support Languages: https://github.com/ssut/py-googletrans/blob/master/googletrans/constants.py
+trnaslated_answer = open_llama3b_kor.generate("나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘")
+print(trnaslated_answer)
+```
+<br>
+
+> Official Google Translation API
+- Support Languages: https://cloud.google.com/translate/docs/languages?hl=ko
+> Unofficial Google Trnaslator for non-profit purposes (such as feature testing)
+- Support Languages: https://github.com/nidhaloff/deep-translator/blob/master/deep_translator/constants.py
 ```python
 from transllm import LLMtranslator
 
 # Set huggingface repository
 model_path = 'openlm-research/open_llama_3b'
 # model_path = 'openlm-research/open_llama_7b'
 # model_path = 'openlm-research/open_llama_13b'
 
-# Get TransLLM Object
-open_llama3b_kor = LLMtranslator(model_path, target_lang='ko', translator='google')
+# Get TransLLM Object (Korean)
+# open_llama3b_kor = LLMtranslator(model_path, target_lang='ko', translator='google_official', google_api_key='xxxxxx') # Official Google Cloud Translation API 
+open_llama3b_kor = LLMtranslator(model_path, target_lang='ko', translator='google') # Unofficial test
+
+
 
 # Using Prompt in multi-language
 prompt = "나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘"
 trnaslated_answer = open_llama3b_kor.generate(prompt)
 print(trnaslated_answer)
 ```
 
 <br>
 
-DeepL
+> DeepL, Open AI, Bard
 - Support Languages: https://www.deepl.com/pro/select-country?cta=header-pro-button/#developer
 
 Open AI, Bard use pre-prompt for translation.
 ```python
 from transllm import LLMtranslator
 
 # Set huggingface repository
 model_path = 'openlm-research/open_llama_3b'
 # model_path = 'openlm-research/open_llama_7b'
 # model_path = 'openlm-research/open_llama_13b'
 
 # Choose Translate Service API: DeepL, OpenAI, Bard
-open_llama3b_kor = LLMtranslator(model_path, target_lang='EN', translator='deepl', deepl_api='xxxxxxx') 
+open_llama3b_kor = LLMtranslator(model_path, target_lang='ES', translator='deepl', deepl_api='xxxxxxx') # Language == Spanish
 # open_llama3b_kor = LLMtranslator(model_path, target_lang='korean', translator='openai', openai_api='xxxxxxx', openai_model='gpt-3.5-turbo')
 # open_llama3b_kor = LLMtranslator(model_path, target_lang='korean', translator='bard', bard_api='xxxxxxx')
 
 # Using Prompt in multi-language
 prompt = "나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘"
 trnaslated_answer = open_llama3b_kor.generate(prompt)
 print(trnaslated_answer)
 ```
 
 <br>
 
+
+> Google Colab Example
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1117ikGEmU4FncBDl1xCC2IhPPDOr75lX?usp=sharing) 
+![](assets/hf-transllm-colab.png)
+
+<br><br>
+
+
 ## Customized Inference
+Applying LLMs to the majority of Hugging Face repositories is generally feasible. However, it can be challenging to apply them to objects that require unique tokenizers or inference processes. In such cases, it is recommended to customize the usage by incorporating a translation module for prompts.
+
+In other words, if you are familiar with the inference process or code from Hugging Face repositories, you can customize the translation object by adding a translation module before and after the known inference process or code. Check [translang repository](https://github.com/dsdanielpark/translang) for more details.
 ```python
 import torch
 from trnasllm import LLMtranslator
 
 
 class MyLLMtranslator(LLMtranslator):
     def __init__(
@@ -162,14 +187,20 @@
 
         answer = customizing_process(prompt)
         # Custom inference logic...
         
         return answer
 ```
 
+<br>
+
+## About Google Translator
+Commercial use or official use of the Google Translate service is chargeable. Please provide the `translator="google_official"` and `google_api_key={YOUR_API_KEY}` arguments. Please responsibly use the `translator="google"` argument for the purpose of simple functionality verification. Refer to the following [notebook file](https://github.com/dsdanielpark/translang/blob/main/scripts/google_official.ipynb) and [official link](https://cloud.google.com/translate?utm_source=google&utm_medium=cpc&utm_campaign=japac-KR-all-en-dr-BKWS-all-mv-trial-EXA-dr-1605216&utm_content=text-ad-none-none-DEV_c-CRE_631260646738-ADGP_Hybrid%20%7C%20BKWS%20-%20EXA%20%7C%20Txt%20~%20AI%20&%20ML_Translation%20AI_google%20translate%20api_main-KWID_43700073965169292-kwd-14329410560&userloc_1009871-network_g&utm_term=KW_google%20translate%20api&gclid=Cj0KCQjwy9-kBhCHARIsAHpBjHjTvBCM7NNcf4fYGsog4ViQErgJvACFXB5JCNUT0h_EpQ5kyUT-SrIaApZBEALw_wcB&gclsrc=aw.ds&hl=ko) for more information. Use the google argument only for some basic functionality testing.
+
+
 ## [FAQs](./documents/FAQs.md)
 Use `Ctrl`+`F` for help in this `FAQs.md`.
 
 ## Contributors
 
 I would like to express my sincere gratitude for the contributions made by all the contributors.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: transllm Version: 0.1.7 Summary: LLMtranslator
+Metadata-Version: 2.1 Name: transllm Version: 0.1.8 Summary: LLMtranslator
 translates and generates text in multiple languages. Home-page: https://
 github.com/dsdanielpark/hf-transllm Author: daniel park Author-email:
 parkminwoo1991@gmail.com Keywords: Python,API,Bard,Google Bard,Large Language
 Model,Chatbot API,Google API,Chatbot Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Science/Research Classifier: Natural
 Language :: English Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
@@ -12,81 +12,111 @@
 Intelligence Requires-Python: >=3.6 Description-Content-Type: text/markdown
 License-File: LICENSE Development Status :: 3 - Alpha # Python Package: hf-
 transllm
 [PyPI package] [Code_style:_black] [https://hits.seeyoufarm.com/api/count/incr/
 badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2Fhf-
 transllm&count_bg=%23000000&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false]
 [PyPI]
-> LLMtranslator translates and generates text in multiple languages. ![]
-(assets/transllm.png) ### Introducing hf-transllm: Unlock the Power of
-Multilingual Exploration Discover the hf-transllm package, a seamless
-integration of Hugging Face's inference module and translation APIs. Overcome
-limitations in retraining and evaluating large language models in different
-languages. Explore diverse results effortlessly, leveraging translation API
-services. Emphasizing versatility over efficiency, hf-transllm enables you to
-delve into the outcomes of Hugging Face's models in various languages.
+> LLMtranslator translates and generates text in multiple languages using LLMs
+(Large Language Models) on hugging-face repository. ![](assets/transllm.png)
+### Introducing hf-transllm: Unlock the Power of Multilingual Exploration
+Discover the hf-transllm package, a seamless integration of Hugging Face's
+inference module and translation APIs. Overcome limitations in retraining and
+evaluating large language models in different languages. Explore diverse
+results effortlessly, leveraging translation API services. Emphasizing
+versatility over efficiency, hf-transllm enables you to delve into the outcomes
+of Hugging Face's models in various languages.
 
 ## Installation ``` pip install transllm ``` Or ``` pip install git+https://
 github.com/dsdanielpark/hf-trnasllm.git ```
-If you wish to use the various features and CLI: ``` pip install git+https://
-github.com/dsdanielpark/hf-transllm.git cd hf-transllm pip install -
-r requirements.txt ``` There can be issues with various dependencies such as
-Hugging Face's Transformers, SentencePiece, Torch, and CUDA. Please set up the
-appropriate environment by searching online. ```bash python main.py --hfmodel
-pen_llama_3b> --lang  --translator  ```
+## CLI If you wish to use CLI: ``` git clone https://github.com/dsdanielpark/
+hf-transllm cd hf-transllm pip install -r requirements.txt ``` ```bash python
+main.py --hfmodel
+pen_llama_3b> --lang  --translator  ``` There can be issues with various
+dependencies such as Hugging Face's Transformers, SentencePiece, Torch, and
+CUDA. Please set up the appropriate environment by searching online.
 
-## Usage Applying LLMs to the majority of Hugging Face repositories is
-generally feasible. However, it can be challenging to apply them to objects
-that require unique tokenizers or inference processes. In such cases, it is
-recommended to customize the usage by incorporating a translation module for
-prompts. In other words, if you are familiar with the inference process or code
-from Hugging Face repositories, you can customize the translation object by
-adding a translation module before and after the known inference process or
-code. [![Open In Colab](https://colab.research.google.com/assets/colab-
-badge.svg)](https://colab.research.google.com/drive/
-1117ikGEmU4FncBDl1xCC2IhPPDOr75lX?usp=sharing) Google Trnaslator - Support
-Languages: https://github.com/ssut/py-googletrans/blob/master/googletrans/
-constants.py ```python from transllm import LLMtranslator # Set huggingface
+## Usage > Simple Usage ```python from transllm import LLMtranslator
+open_llama3b_kor = LLMtranslator('openlm-research/open_llama_3b',
+target_lang='ko', translator='google') # Korean trnaslated_answer =
+open_llama3b_kor.generate("ëì ë´ ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì
+ëí´ì ìë ¤ì¤") print(trnaslated_answer) ```
+> Official Google Translation API - Support Languages: https://
+cloud.google.com/translate/docs/languages?hl=ko > Unofficial Google Trnaslator
+for non-profit purposes (such as feature testing) - Support Languages: https://
+github.com/nidhaloff/deep-translator/blob/master/deep_translator/constants.py
+```python from transllm import LLMtranslator # Set huggingface repository
+model_path = 'openlm-research/open_llama_3b' # model_path = 'openlm-research/
+open_llama_7b' # model_path = 'openlm-research/open_llama_13b' # Get TransLLM
+Object (Korean) # open_llama3b_kor = LLMtranslator(model_path,
+target_lang='ko', translator='google_official', google_api_key='xxxxxx') #
+Official Google Cloud Translation API open_llama3b_kor = LLMtranslator
+(model_path, target_lang='ko', translator='google') # Unofficial test # Using
+Prompt in multi-language prompt = "ëì ë´ ëëë°°ë¤ì´ ì¢ìíë
+ë´ì§ì¤ì ëí´ì ìë ¤ì¤" trnaslated_answer = open_llama3b_kor.generate
+(prompt) print(trnaslated_answer) ```
+> DeepL, Open AI, Bard - Support Languages: https://www.deepl.com/pro/select-
+country?cta=header-pro-button/#developer Open AI, Bard use pre-prompt for
+translation. ```python from transllm import LLMtranslator # Set huggingface
 repository model_path = 'openlm-research/open_llama_3b' # model_path = 'openlm-
-research/open_llama_7b' # model_path = 'openlm-research/open_llama_13b' # Get
-TransLLM Object open_llama3b_kor = LLMtranslator(model_path, target_lang='ko',
-translator='google') # Using Prompt in multi-language prompt = "ëì ë´
-ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì ìë ¤ì¤"
-trnaslated_answer = open_llama3b_kor.generate(prompt) print(trnaslated_answer)
-```
-DeepL - Support Languages: https://www.deepl.com/pro/select-country?cta=header-
-pro-button/#developer Open AI, Bard use pre-prompt for translation. ```python
-from transllm import LLMtranslator # Set huggingface repository model_path =
-'openlm-research/open_llama_3b' # model_path = 'openlm-research/open_llama_7b'
-# model_path = 'openlm-research/open_llama_13b' # Choose Translate Service API:
-DeepL, OpenAI, Bard open_llama3b_kor = LLMtranslator(model_path,
-target_lang='EN', translator='deepl', deepl_api='xxxxxxx') # open_llama3b_kor =
-LLMtranslator(model_path, target_lang='korean', translator='openai',
-openai_api='xxxxxxx', openai_model='gpt-3.5-turbo') # open_llama3b_kor =
-LLMtranslator(model_path, target_lang='korean', translator='bard',
-bard_api='xxxxxxx') # Using Prompt in multi-language prompt = "ëì ë´
-ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì ìë ¤ì¤"
-trnaslated_answer = open_llama3b_kor.generate(prompt) print(trnaslated_answer)
-```
-## Customized Inference ```python import torch from trnasllm import
-LLMtranslator class MyLLMtranslator(LLMtranslator): def __init__( self,
+research/open_llama_7b' # model_path = 'openlm-research/open_llama_13b' #
+Choose Translate Service API: DeepL, OpenAI, Bard open_llama3b_kor =
+LLMtranslator(model_path, target_lang='ES', translator='deepl',
+deepl_api='xxxxxxx') # Language == Spanish # open_llama3b_kor = LLMtranslator
+(model_path, target_lang='korean', translator='openai', openai_api='xxxxxxx',
+openai_model='gpt-3.5-turbo') # open_llama3b_kor = LLMtranslator(model_path,
+target_lang='korean', translator='bard', bard_api='xxxxxxx') # Using Prompt in
+multi-language prompt = "ëì ë´ ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì
+ëí´ì ìë ¤ì¤" trnaslated_answer = open_llama3b_kor.generate(prompt)
+print(trnaslated_answer) ```
+> Google Colab Example [![Open In Colab](https://colab.research.google.com/
+assets/colab-badge.svg)](https://colab.research.google.com/drive/
+1117ikGEmU4FncBDl1xCC2IhPPDOr75lX?usp=sharing) ![](assets/hf-transllm-
+colab.png)
+
+## Customized Inference Applying LLMs to the majority of Hugging Face
+repositories is generally feasible. However, it can be challenging to apply
+them to objects that require unique tokenizers or inference processes. In such
+cases, it is recommended to customize the usage by incorporating a translation
+module for prompts. In other words, if you are familiar with the inference
+process or code from Hugging Face repositories, you can customize the
+translation object by adding a translation module before and after the known
+inference process or code. Check [translang repository](https://github.com/
+dsdanielpark/translang) for more details. ```python import torch from trnasllm
+import LLMtranslator class MyLLMtranslator(LLMtranslator): def __init__( self,
 model_path, target_lang="ko", translator="google", torch_dtype=torch.float16,
 device_map="auto", deepl_api=None, bard_api=None, openai_model="gpt-3.5-turbo",
 openai_api=None ): super().__init__( model_path=model_path,
 target_lang=target_lang, translator=translator, torch_dtype=torch_dtype,
 device_map=device_map, deepl_api=deepl_api, bard_api=bard_api,
 openai_model=openai_model, openai_api=openai_api ) def inference(self, prompt:
 str) -> str: # Custom logic for inference # You can override the implementation
 of the inference method here # and provide your own logic for generating the
 translated answer # Remember to return the translated answer as a string.
 answer = customizing_process(prompt) # Custom inference logic... return answer
-``` ## [FAQs](./documents/FAQs.md) Use `Ctrl`+`F` for help in this `FAQs.md`.
-## Contributors I would like to express my sincere gratitude for the
-contributions made by all the contributors. [https://contrib.rocks/
-image?repo=dsdanielpark/hf-transllm]
+```
+## About Google Translator Commercial use or official use of the Google
+Translate service is chargeable. Please provide the
+`translator="google_official"` and `google_api_key={YOUR_API_KEY}` arguments.
+Please responsibly use the `translator="google"` argument for the purpose of
+simple functionality verification. Refer to the following [notebook file]
+(https://github.com/dsdanielpark/translang/blob/main/scripts/
+google_official.ipynb) and [official link](https://cloud.google.com/
+translate?utm_source=google&utm_medium=cpc&utm_campaign=japac-KR-all-en-dr-
+BKWS-all-mv-trial-EXA-dr-1605216&utm_content=text-ad-none-none-DEV_c-
+CRE_631260646738-ADGP_Hybrid%20%7C%20BKWS%20-
+%20EXA%20%7C%20Txt%20~%20AI%20&%20ML_Translation%20AI_google%20translate%20api_main-
+KWID_43700073965169292-kwd-14329410560&userloc_1009871-
+network_g&utm_term=KW_google%20translate%20api&gclid=Cj0KCQjwy9-
+kBhCHARIsAHpBjHjTvBCM7NNcf4fYGsog4ViQErgJvACFXB5JCNUT0h_EpQ5kyUT-
+SrIaApZBEALw_wcB&gclsrc=aw.ds&hl=ko) for more information. Use the google
+argument only for some basic functionality testing. ## [FAQs](./documents/
+FAQs.md) Use `Ctrl`+`F` for help in this `FAQs.md`. ## Contributors I would
+like to express my sincere gratitude for the contributions made by all the
+contributors. [https://contrib.rocks/image?repo=dsdanielpark/hf-transllm]
 ## License [MIT](https://opensource.org/license/mit/)
 I hold no legal responsibility; ``` The MIT License (MIT) Copyright (c) 2023
 Minwoo Park Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including without
 limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom
```


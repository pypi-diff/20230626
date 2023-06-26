# Comparing `tmp/bardapi-0.1.8.tar.gz` & `tmp/bardapi-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bardapi-0.1.8.tar", last modified: Thu May 18 08:10:10 2023, max compression
+gzip compressed data, was "bardapi-0.1.9.tar", last modified: Sun May 21 16:24:45 2023, max compression
```

## Comparing `bardapi-0.1.8.tar` & `bardapi-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 08:10:10.525894 bardapi-0.1.8/
--rw-rw-rw-   0        0        0     1087 2023-04-13 16:54:50.000000 bardapi-0.1.8/LICENSE
--rw-rw-rw-   0        0        0     7995 2023-05-18 08:10:10.524723 bardapi-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     7046 2023-05-18 08:07:41.000000 bardapi-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 08:10:10.509779 bardapi-0.1.8/bardapi/
--rw-rw-rw-   0        0        0      208 2023-05-18 08:08:56.000000 bardapi-0.1.8/bardapi/__init__.py
--rw-rw-rw-   0        0        0     4212 2023-05-18 08:06:55.000000 bardapi-0.1.8/bardapi/core.py
-drwxrwxrwx   0        0        0        0 2023-05-18 08:10:10.522717 bardapi-0.1.8/bardapi.egg-info/
--rw-rw-rw-   0        0        0     7995 2023-05-18 08:10:10.000000 bardapi-0.1.8/bardapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2023-05-18 08:10:10.000000 bardapi-0.1.8/bardapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 08:10:10.000000 bardapi-0.1.8/bardapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-05-18 08:10:10.000000 bardapi-0.1.8/bardapi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-05-18 08:10:10.000000 bardapi-0.1.8/bardapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-18 08:10:10.000000 bardapi-0.1.8/bardapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 08:10:10.526905 bardapi-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1783 2023-05-18 08:08:59.000000 bardapi-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 16:24:45.591613 bardapi-0.1.9/
+-rw-rw-rw-   0        0        0     1087 2023-04-13 16:54:50.000000 bardapi-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0    11005 2023-05-21 16:24:45.590615 bardapi-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0    10056 2023-05-21 16:21:01.000000 bardapi-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-21 16:24:45.575938 bardapi-0.1.9/bardapi/
+-rw-rw-rw-   0        0        0      263 2023-05-21 16:21:59.000000 bardapi-0.1.9/bardapi/__init__.py
+-rw-rw-rw-   0        0        0     5959 2023-05-21 16:20:19.000000 bardapi-0.1.9/bardapi/core.py
+-rw-rw-rw-   0        0        0     1077 2023-05-21 16:13:32.000000 bardapi-0.1.9/bardapi/tranlsator.py
+drwxrwxrwx   0        0        0        0 2023-05-21 16:24:45.588614 bardapi-0.1.9/bardapi.egg-info/
+-rw-rw-rw-   0        0        0    11005 2023-05-21 16:24:45.000000 bardapi-0.1.9/bardapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-05-21 16:24:45.000000 bardapi-0.1.9/bardapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 16:24:45.000000 bardapi-0.1.9/bardapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-05-21 16:24:45.000000 bardapi-0.1.9/bardapi.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       21 2023-05-21 16:24:45.000000 bardapi-0.1.9/bardapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-21 16:24:45.000000 bardapi-0.1.9/bardapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-21 16:24:45.591613 bardapi-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1798 2023-05-21 16:21:46.000000 bardapi-0.1.9/setup.py
```

### Comparing `bardapi-0.1.8/LICENSE` & `bardapi-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bardapi-0.1.8/PKG-INFO` & `bardapi-0.1.9/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: bardapi
-Version: 0.1.8
-Summary: The python package that returns Response of Google Bard through API.
-Home-page: https://github.com/dsdanielpark/Bard-API
-Author: daniel park
-Author-email: parkminwoo1991@gmail.com
-Keywords: Python,API,Bard,Google Bard,Large Language Model,Chatbot API,Google API,Chatbot
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 Development Status :: 5 - Production/Stable
 
 
 # Google <a href="https://bard.google.com/"><img src="https://camo.githubusercontent.com/adb54264fe2ad5067d07d0752fc32600b4e6250073b01ce8c386575b431e3f06/68747470733a2f2f7777772e677374617469632e636f6d2f6c616d64612f696d616765732f66617669636f6e5f76315f31353031363063646466663766323934636533302e737667" height="20px"></a> Bard API 
 
 
 <p align="left">
@@ -36,18 +14,19 @@
 </p>
 
 > The python package that returns response of [Google Bard](https://bard.google.com/) through API.
 
 ![](./assets/bard_api.gif)
 
 
-I referred to [this github repository(github.com/acheong08/Bard)](https://github.com/acheong08/Bard) where inference process of Bard was reverse engineered. Using `__Secure-1PSID`, you can ask questions and get answers from Google Bard. This package is designed for application to the Python package [ExceptNotifier](https://github.com/dsdanielpark/ExceptNotifier) and [Co-Coder](https://github.com/dsdanielpark/Co-Coder). 
+I referred to [this github repository(github.com/acheong08/Bard)](https://github.com/acheong08/Bard) where inference process of Bard was reverse engineered. Using `__Secure-1PSID`, you can ask questions and get answers from Google Bard. This package is designed for application to the Python package [ExceptNotifier](https://github.com/dsdanielpark/ExceptNotifier) and [Co-Coder](https://github.com/dsdanielpark/Co-Coder). Please note that the bardapi is not a free service, but rather a tool provided to assist developers with testing certain functionalities due to the delayed development and release of Google Bard's API. It has been designed with a lightweight structure that can easily adapt to the emergence of an official API. Therefore, I strongly discourage using it for any other purposes.
 
 <br>
 
+
 Do not expose the `__Secure-1PSID`
 > Note that while I referred to `__Secure-1PSID` value as an API KEY for convenience, it is not an officially provided API KEY. 
 
 <br>
 
 ##  [Amazing Bard Prompts](https://github.com/dsdanielpark/amazing-bard-prompts) Is All You Need!
 - Helpful prompts for Google Bard
@@ -70,15 +49,15 @@
 1. Visit https://bard.google.com/
 2. F12 for console
 3. Session: Application → Cookies → Copy the value of  `__Secure-1PSID` cookie.
 
 <br>
 
 ## Usage 
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1YIMA8aBmEQSSk90bB0Q9tznaLLQcluGA?usp=share_link) 
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1zzzlTIh0kt2MdjLzvXRby1rWbHzmog8t?usp=sharing) 
 
 
 Simple Usage
 
 ```python
 from bardapi import Bard
 
@@ -130,19 +109,20 @@
 ```python
 from bardapi import Bard
 import os
 os.environ['_BARD_API_KEY']="xxxxxxxx"
 
 # Change 'http://127.0.0.1:1080' to your http proxy
 # timeout in seconds
-bard = Bard(proxies={'http':'http://127.0.0.1:1080', 'https':'http://127.0.0.1:1080'}, timeout=10)
+bard = Bard(proxies={'http':'http://127.0.0.1:1080', 'https':'http://127.0.0.1:1080'}, timeout=30)
 bard.get_answer("나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘")['content']
 ```
 
 ### Reusable session object
+You can continue the conversation through a reusable session.
 ```python
 from bardapi import Bard
 import os
 import requests
 os.environ['_BARD_API_KEY'] = 'xxxxxxxxxxx'
 # token='xxxxxxxxxxx'
 
@@ -156,42 +136,92 @@
             "Referer": "https://bard.google.com/",
         }
 session.cookies.set("__Secure-1PSID", os.getenv("_BARD_API_KEY")) 
 # session.cookies.set("__Secure-1PSID", token) 
 
 bard = Bard(session=session, timeout=30)
 bard.get_answer("나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘")['content']
+
+# Continued conversation without set new session
+bard.get_answer("What is my last prompt??")['content']
+```
+
+
+### Other languages
+To detect and translate using the Google Bard in unofficial languages, the Python package [googletrans](https://github.com/ssut/py-googletrans) is utilized.
+
+```python
+from bardapi import Bard
+token = 'xxxxxxx'
+bard = Bard(token=token, language='arabic')
+res = bard.get_answer("هل تعرف الكيمتشي")
 ```
 
 Simple Example
 <br>
 
-<a href="https://bard.google.com/"><img src="./assets/bardimg.png" height="600px">
+<a href="https://bard.google.com/"><img src="./assets/bard_img.png">
 
 <br>
 
+## Translation to Another Programming Language
+Please check the translation results in [this folder](https://github.com/dsdanielpark/Bard-API/tree/main/translate_to).
+- Copy the code of [Core.py](https://github.com/dsdanielpark/Bard-API/blob/main/bardapi/core.py).
+- Ask ChatGPT to translate like "Translate to Swift."
+- Ask ChatGPT to optimize the code or provide any desired instructions until you're satisfied.<br>
 
+![](./assets/translate.png)
+            
+            
 ## Scripts
-In the scripts [folder](./scripts/), I have released a script to help you compare [OpenAI-ChatGPT](./scripts/openai_api.ipynb) and [Google-Bard](./scripts/google_api.ipynb). I hope they will help more developers.
+In the scripts [folder](./scripts/), I have released a script to help you compare [OpenAI-ChatGPT](./scripts/openai_api.ipynb), [Microsoft-EdgeGPT](./scripts/microsoft_api.ipynb) and [Google-Bard](./scripts/google_api.ipynb). I hope they will help more developers.
 
+## Shifting Service Policies: Bard and Google's Dynamics 
+Bard's service status and Google's API interfaces are in constant flux. *The number of replies is currently limited, but certain users,* such as those utilizing VPNs or proxy servers, have reported slightly higher message caps. Adaptability is crucial in navigating these dynamic service policies. Please note that the cookie values used in this package are not official API values.
+            
+            
 ## License
 [MIT](https://opensource.org/license/mit/) <br>
 I hold no legal responsibility; for more information, please refer to the bottom of the readme file. I just want you to give me and [them](https://github.com/acheong08/Bard) a star.
+```
+The MIT License (MIT)
 
+Copyright (c) 2023 Minwoo Park
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+```
 
 ## Bugs and Issues
 Sincerely grateful for any reports on new features or bugs. Your valuable feedback on the code is highly appreciated.
 
 ## Contacts
 - Core maintainer: [Daniel Park, South Korea](https://github.com/DSDanielPark) <br>
 - E-mail: parkminwoo1991@gmail.com <br>
 
 ## Reference 
 [1] https://github.com/acheong08/Bard
   
+<br>
+            
 ### Important Notice
   The user assumes all legal responsibilities associated with using the BardAPI package. This Python package merely facilitates easy access to Google Bard for developers. Users are solely responsible for managing data and using the package appropriately. For further information, please consult the Google Bard Official Document.
   
 
 #### Could you kindly add this badge to your repository?
 markdown
 ```
```

#### html2text {}

```diff
@@ -1,51 +1,44 @@
-Metadata-Version: 2.1 Name: bardapi Version: 0.1.8 Summary: The python package
-that returns Response of Google Bard through API. Home-page: https://
-github.com/dsdanielpark/Bard-API Author: daniel park Author-email:
-parkminwoo1991@gmail.com Keywords: Python,API,Bard,Google Bard,Large Language
-Model,Chatbot API,Google API,Chatbot Classifier: Development Status :: 5 -
-Production/Stable Classifier: Intended Audience :: Science/Research Classifier:
-Natural Language :: English Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: MIT License Classifier: Programming
-Language :: Python :: 3.6 Classifier: Topic :: Scientific/Engineering ::
-Artificial Intelligence Requires-Python: >=3.6 Description-Content-Type: text/
-markdown License-File: LICENSE Development Status :: 5 - Production/Stable #
-Google [https://camo.githubusercontent.com/
+Development Status :: 5 - Production/Stable # Google [https://
+camo.githubusercontent.com/
 adb54264fe2ad5067d07d0752fc32600b4e6250073b01ce8c386575b431e3f06/
 68747470733a2f2f7777772e677374617469632e636f6d2f6c616d64612f696d616765732f66617669636f6e5f76315f31353031363063646466663766323934636533302e737667]
 Bard API
 [PyPI package]   [Code_style:_black] [https://hits.seeyoufarm.com/api/count/
 incr/
 badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2FBARD_API&count_bg=%23000000&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=BardAPI&edge_flat=false]
 [PyPI]
 > The python package that returns response of [Google Bard](https://
 bard.google.com/) through API. ![](./assets/bard_api.gif) I referred to [this
 github repository(github.com/acheong08/Bard)](https://github.com/acheong08/
 Bard) where inference process of Bard was reverse engineered. Using `__Secure-
 1PSID`, you can ask questions and get answers from Google Bard. This package is
 designed for application to the Python package [ExceptNotifier](https://
 github.com/dsdanielpark/ExceptNotifier) and [Co-Coder](https://github.com/
-dsdanielpark/Co-Coder).
+dsdanielpark/Co-Coder). Please note that the bardapi is not a free service, but
+rather a tool provided to assist developers with testing certain
+functionalities due to the delayed development and release of Google Bard's
+API. It has been designed with a lightweight structure that can easily adapt to
+the emergence of an official API. Therefore, I strongly discourage using it for
+any other purposes.
 Do not expose the `__Secure-1PSID` > Note that while I referred to `__Secure-
 1PSID` value as an API KEY for convenience, it is not an officially provided
 API KEY.
 ## [Amazing Bard Prompts](https://github.com/dsdanielpark/amazing-bard-prompts)
 Is All You Need! - Helpful prompts for Google Bard
 ## Install The latest stable release (and required dependencies) can be
 installed from PyPI: ``` pip install bardapi ``` You may instead want to use
 the development version from Github: ``` pip install git+https://github.com/
 dsdanielpark/Bard-API.git ```
 ## Authentication 1. Visit https://bard.google.com/ 2. F12 for console 3.
 Session: Application â Cookies â Copy the value of `__Secure-1PSID` cookie.
 
 ## Usage [![Open In Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/drive/
-1YIMA8aBmEQSSk90bB0Q9tznaLLQcluGA?usp=share_link) Simple Usage ```python from
+1zzzlTIh0kt2MdjLzvXRby1rWbHzmog8t?usp=sharing) Simple Usage ```python from
 bardapi import Bard token = 'xxxxxxxxxx' bard = Bard(token=token)
 bard.get_answer("ëì ë´ ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì
 ìë ¤ì¤")['content'] ``` Or you can use this ```python from bardapi import
 Bard import os os.environ['_BARD_API_KEY']="xxxxxxxx" Bard().get_answer("ëì
 ë´ ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì ìë ¤ì¤")['content']
 ``` To get reponse dictionary ```python import bardapi import os # set your
 __Secure-1PSID value to key token = 'xxxxxxxxxx' # set your input text
@@ -58,41 +51,74 @@
 ['_BARD_API_KEY']="xxxxxxxx" bard = Bard(timeout=30) # Set timeout in seconds
 bard.get_answer("ëì ë´ ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì
 ìë ¤ì¤")['content'] ```
 ## Futher ### Behind a proxy If you are working behind a proxy, use the
 following. ```python from bardapi import Bard import os os.environ
 ['_BARD_API_KEY']="xxxxxxxx" # Change 'http://127.0.0.1:1080' to your http
 proxy # timeout in seconds bard = Bard(proxies={'http':'http://127.0.0.1:1080',
-'https':'http://127.0.0.1:1080'}, timeout=10) bard.get_answer("ëì ë´
+'https':'http://127.0.0.1:1080'}, timeout=30) bard.get_answer("ëì ë´
 ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì ìë ¤ì¤")['content'] ```
-### Reusable session object ```python from bardapi import Bard import os import
-requests os.environ['_BARD_API_KEY'] = 'xxxxxxxxxxx' # token='xxxxxxxxxxx'
-session = requests.Session() session.headers = { "Host": "bard.google.com", "X-
-Same-Domain": "1", "User-Agent": "Mozilla/5.0 (Windows NT 10.0; WOW64)
-AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.114 Safari/537.36",
-"Content-Type": "application/x-www-form-urlencoded;charset=UTF-8", "Origin":
-"https://bard.google.com", "Referer": "https://bard.google.com/", }
-session.cookies.set("__Secure-1PSID", os.getenv("_BARD_API_KEY")) #
-session.cookies.set("__Secure-1PSID", token) bard = Bard(session=session,
-timeout=30) bard.get_answer("ëì ë´ ëëë°°ë¤ì´ ì¢ìíë
-ë´ì§ì¤ì ëí´ì ìë ¤ì¤")['content'] ``` Simple Example
-[./assets/bardimg.png]_
-##_Scripts_In_the_scripts_[folder](./scripts/),_I_have_released_a_script_to
-help_you_compare_[OpenAI-ChatGPT](./scripts/openai_api.ipynb)_and_[Google-Bard]
-(./scripts/google_api.ipynb)._I_hope_they_will_help_more_developers._##_License
+### Reusable session object You can continue the conversation through a
+reusable session. ```python from bardapi import Bard import os import requests
+os.environ['_BARD_API_KEY'] = 'xxxxxxxxxxx' # token='xxxxxxxxxxx' session =
+requests.Session() session.headers = { "Host": "bard.google.com", "X-Same-
+Domain": "1", "User-Agent": "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/
+537.36 (KHTML, like Gecko) Chrome/91.0.4472.114 Safari/537.36", "Content-Type":
+"application/x-www-form-urlencoded;charset=UTF-8", "Origin": "https://
+bard.google.com", "Referer": "https://bard.google.com/", } session.cookies.set
+("__Secure-1PSID", os.getenv("_BARD_API_KEY")) # session.cookies.set("__Secure-
+1PSID", token) bard = Bard(session=session, timeout=30) bard.get_answer("ëì
+ë´ ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì ìë ¤ì¤")['content']
+# Continued conversation without set new session bard.get_answer("What is my
+last prompt??")['content'] ``` ### Other languages To detect and translate
+using the Google Bard in unofficial languages, the Python package [googletrans]
+(https://github.com/ssut/py-googletrans) is utilized. ```python from bardapi
+import Bard token = 'xxxxxxx' bard = Bard(token=token, language='arabic') res =
+bard.get_answer("ÙÙ ØªØ¹Ø±Ù Ø§ÙÙÙÙØªØ´Ù") ``` Simple Example
+[./assets/bard_img.png]_
+##_Translation_to_Another_Programming_Language_Please_check_the_translation
+results_in_[this_folder](https://github.com/dsdanielpark/Bard-API/tree/main/
+translate_to)._-_Copy_the_code_of_[Core.py](https://github.com/dsdanielpark/
+Bard-API/blob/main/bardapi/core.py)._-_Ask_ChatGPT_to_translate_like_"Translate
+to_Swift."_-_Ask_ChatGPT_to_optimize_the_code_or_provide_any_desired
+instructions_until_you're_satisfied.
+![](./assets/translate.png)_##_Scripts_In_the_scripts_[folder](./scripts/),_I
+have_released_a_script_to_help_you_compare_[OpenAI-ChatGPT](./scripts/
+openai_api.ipynb),_[Microsoft-EdgeGPT](./scripts/microsoft_api.ipynb)_and_
+[Google-Bard](./scripts/google_api.ipynb)._I_hope_they_will_help_more
+developers._##_Shifting_Service_Policies:_Bard_and_Google's_Dynamics_Bard's
+service_status_and_Google's_API_interfaces_are_in_constant_flux._*The_number_of
+replies_is_currently_limited,_but_certain_users,*_such_as_those_utilizing_VPNs
+or_proxy_servers,_have_reported_slightly_higher_message_caps._Adaptability_is
+crucial_in_navigating_these_dynamic_service_policies._Please_note_that_the
+cookie_values_used_in_this_package_are_not_official_API_values._##_License_
 [MIT](https://opensource.org/license/mit/)_
 I_hold_no_legal_responsibility;_for_more_information,_please_refer_to_the
 bottom_of_the_readme_file._I_just_want_you_to_give_me_and_[them](https://
-github.com/acheong08/Bard)_a_star._##_Bugs_and_Issues_Sincerely_grateful_for
-any_reports_on_new_features_or_bugs._Your_valuable_feedback_on_the_code_is
-highly_appreciated._##_Contacts_-_Core_maintainer:_[Daniel_Park,_South_Korea]
-(https://github.com/DSDanielPark)_
+github.com/acheong08/Bard)_a_star._```_The_MIT_License_(MIT)_Copyright_(c)_2023
+Minwoo_Park_Permission_is_hereby_granted,_free_of_charge,_to_any_person
+obtaining_a_copy_of_this_software_and_associated_documentation_files_(the
+"Software"),_to_deal_in_the_Software_without_restriction,_including_without
+limitation_the_rights_to_use,_copy,_modify,_merge,_publish,_distribute,
+sublicense,_and/or_sell_copies_of_the_Software,_and_to_permit_persons_to_whom
+the_Software_is_furnished_to_do_so,_subject_to_the_following_conditions:_The
+above_copyright_notice_and_this_permission_notice_shall_be_included_in_all
+copies_or_substantial_portions_of_the_Software._THE_SOFTWARE_IS_PROVIDED_"AS
+IS",_WITHOUT_WARRANTY_OF_ANY_KIND,_EXPRESS_OR_IMPLIED,_INCLUDING_BUT_NOT
+LIMITED_TO_THE_WARRANTIES_OF_MERCHANTABILITY,_FITNESS_FOR_A_PARTICULAR_PURPOSE
+AND_NONINFRINGEMENT._IN_NO_EVENT_SHALL_THE_AUTHORS_OR_COPYRIGHT_HOLDERS_BE
+LIABLE_FOR_ANY_CLAIM,_DAMAGES_OR_OTHER_LIABILITY,_WHETHER_IN_AN_ACTION_OF
+CONTRACT,_TORT_OR_OTHERWISE,_ARISING_FROM,_OUT_OF_OR_IN_CONNECTION_WITH_THE
+SOFTWARE_OR_THE_USE_OR_OTHER_DEALINGS_IN_THE_SOFTWARE._```_##_Bugs_and_Issues
+Sincerely_grateful_for_any_reports_on_new_features_or_bugs._Your_valuable
+feedback_on_the_code_is_highly_appreciated._##_Contacts_-_Core_maintainer:_
+[Daniel_Park,_South_Korea](https://github.com/DSDanielPark)_
 -_E-mail:_parkminwoo1991@gmail.com_
-##_Reference_[1]_https://github.com/acheong08/Bard_###_Important_Notice_The
-user_assumes_all_legal_responsibilities_associated_with_using_the_BardAPI
-package._This_Python_package_merely_facilitates_easy_access_to_Google_Bard_for
-developers._Users_are_solely_responsible_for_managing_data_and_using_the
-package_appropriately._For_further_information,_please_consult_the_Google_Bard
-Official_Document._####_Could_you_kindly_add_this_badge_to_your_repository?
-markdown_```_![BardAPI](https://img.shields.io/badge/pypi-BardAPI-black)_```
-html_```_[PyPI_package]_```_Thank_you_for_your_interest._*Copyright_(c)_2023
-MinWoo_Park,_South_Korea*
+##_Reference_[1]_https://github.com/acheong08/Bard_
+###_Important_Notice_The_user_assumes_all_legal_responsibilities_associated
+with_using_the_BardAPI_package._This_Python_package_merely_facilitates_easy
+access_to_Google_Bard_for_developers._Users_are_solely_responsible_for_managing
+data_and_using_the_package_appropriately._For_further_information,_please
+consult_the_Google_Bard_Official_Document._####_Could_you_kindly_add_this_badge
+to_your_repository?_markdown_```_![BardAPI](https://img.shields.io/badge/pypi-
+BardAPI-black)_```_html_```_[PyPI_package]_```_Thank_you_for_your_interest.
+*Copyright_(c)_2023_MinWoo_Park,_South_Korea*
```

### Comparing `bardapi-0.1.8/bardapi.egg-info/PKG-INFO` & `bardapi-0.1.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bardapi
-Version: 0.1.8
+Version: 0.1.9
 Summary: The python package that returns Response of Google Bard through API.
 Home-page: https://github.com/dsdanielpark/Bard-API
 Author: daniel park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Python,API,Bard,Google Bard,Large Language Model,Chatbot API,Google API,Chatbot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -36,18 +36,19 @@
 </p>
 
 > The python package that returns response of [Google Bard](https://bard.google.com/) through API.
 
 ![](./assets/bard_api.gif)
 
 
-I referred to [this github repository(github.com/acheong08/Bard)](https://github.com/acheong08/Bard) where inference process of Bard was reverse engineered. Using `__Secure-1PSID`, you can ask questions and get answers from Google Bard. This package is designed for application to the Python package [ExceptNotifier](https://github.com/dsdanielpark/ExceptNotifier) and [Co-Coder](https://github.com/dsdanielpark/Co-Coder). 
+I referred to [this github repository(github.com/acheong08/Bard)](https://github.com/acheong08/Bard) where inference process of Bard was reverse engineered. Using `__Secure-1PSID`, you can ask questions and get answers from Google Bard. This package is designed for application to the Python package [ExceptNotifier](https://github.com/dsdanielpark/ExceptNotifier) and [Co-Coder](https://github.com/dsdanielpark/Co-Coder). Please note that the bardapi is not a free service, but rather a tool provided to assist developers with testing certain functionalities due to the delayed development and release of Google Bard's API. It has been designed with a lightweight structure that can easily adapt to the emergence of an official API. Therefore, I strongly discourage using it for any other purposes.
 
 <br>
 
+
 Do not expose the `__Secure-1PSID`
 > Note that while I referred to `__Secure-1PSID` value as an API KEY for convenience, it is not an officially provided API KEY. 
 
 <br>
 
 ##  [Amazing Bard Prompts](https://github.com/dsdanielpark/amazing-bard-prompts) Is All You Need!
 - Helpful prompts for Google Bard
@@ -70,15 +71,15 @@
 1. Visit https://bard.google.com/
 2. F12 for console
 3. Session: Application → Cookies → Copy the value of  `__Secure-1PSID` cookie.
 
 <br>
 
 ## Usage 
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1YIMA8aBmEQSSk90bB0Q9tznaLLQcluGA?usp=share_link) 
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1zzzlTIh0kt2MdjLzvXRby1rWbHzmog8t?usp=sharing) 
 
 
 Simple Usage
 
 ```python
 from bardapi import Bard
 
@@ -130,19 +131,20 @@
 ```python
 from bardapi import Bard
 import os
 os.environ['_BARD_API_KEY']="xxxxxxxx"
 
 # Change 'http://127.0.0.1:1080' to your http proxy
 # timeout in seconds
-bard = Bard(proxies={'http':'http://127.0.0.1:1080', 'https':'http://127.0.0.1:1080'}, timeout=10)
+bard = Bard(proxies={'http':'http://127.0.0.1:1080', 'https':'http://127.0.0.1:1080'}, timeout=30)
 bard.get_answer("나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘")['content']
 ```
 
 ### Reusable session object
+You can continue the conversation through a reusable session.
 ```python
 from bardapi import Bard
 import os
 import requests
 os.environ['_BARD_API_KEY'] = 'xxxxxxxxxxx'
 # token='xxxxxxxxxxx'
 
@@ -156,42 +158,92 @@
             "Referer": "https://bard.google.com/",
         }
 session.cookies.set("__Secure-1PSID", os.getenv("_BARD_API_KEY")) 
 # session.cookies.set("__Secure-1PSID", token) 
 
 bard = Bard(session=session, timeout=30)
 bard.get_answer("나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘")['content']
+
+# Continued conversation without set new session
+bard.get_answer("What is my last prompt??")['content']
+```
+
+
+### Other languages
+To detect and translate using the Google Bard in unofficial languages, the Python package [googletrans](https://github.com/ssut/py-googletrans) is utilized.
+
+```python
+from bardapi import Bard
+token = 'xxxxxxx'
+bard = Bard(token=token, language='arabic')
+res = bard.get_answer("هل تعرف الكيمتشي")
 ```
 
 Simple Example
 <br>
 
-<a href="https://bard.google.com/"><img src="./assets/bardimg.png" height="600px">
+<a href="https://bard.google.com/"><img src="./assets/bard_img.png">
 
 <br>
 
+## Translation to Another Programming Language
+Please check the translation results in [this folder](https://github.com/dsdanielpark/Bard-API/tree/main/translate_to).
+- Copy the code of [Core.py](https://github.com/dsdanielpark/Bard-API/blob/main/bardapi/core.py).
+- Ask ChatGPT to translate like "Translate to Swift."
+- Ask ChatGPT to optimize the code or provide any desired instructions until you're satisfied.<br>
 
+![](./assets/translate.png)
+            
+            
 ## Scripts
-In the scripts [folder](./scripts/), I have released a script to help you compare [OpenAI-ChatGPT](./scripts/openai_api.ipynb) and [Google-Bard](./scripts/google_api.ipynb). I hope they will help more developers.
+In the scripts [folder](./scripts/), I have released a script to help you compare [OpenAI-ChatGPT](./scripts/openai_api.ipynb), [Microsoft-EdgeGPT](./scripts/microsoft_api.ipynb) and [Google-Bard](./scripts/google_api.ipynb). I hope they will help more developers.
 
+## Shifting Service Policies: Bard and Google's Dynamics 
+Bard's service status and Google's API interfaces are in constant flux. *The number of replies is currently limited, but certain users,* such as those utilizing VPNs or proxy servers, have reported slightly higher message caps. Adaptability is crucial in navigating these dynamic service policies. Please note that the cookie values used in this package are not official API values.
+            
+            
 ## License
 [MIT](https://opensource.org/license/mit/) <br>
 I hold no legal responsibility; for more information, please refer to the bottom of the readme file. I just want you to give me and [them](https://github.com/acheong08/Bard) a star.
+```
+The MIT License (MIT)
 
+Copyright (c) 2023 Minwoo Park
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+```
 
 ## Bugs and Issues
 Sincerely grateful for any reports on new features or bugs. Your valuable feedback on the code is highly appreciated.
 
 ## Contacts
 - Core maintainer: [Daniel Park, South Korea](https://github.com/DSDanielPark) <br>
 - E-mail: parkminwoo1991@gmail.com <br>
 
 ## Reference 
 [1] https://github.com/acheong08/Bard
   
+<br>
+            
 ### Important Notice
   The user assumes all legal responsibilities associated with using the BardAPI package. This Python package merely facilitates easy access to Google Bard for developers. Users are solely responsible for managing data and using the package appropriately. For further information, please consult the Google Bard Official Document.
   
 
 #### Could you kindly add this badge to your repository?
 markdown
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bardapi Version: 0.1.8 Summary: The python package
+Metadata-Version: 2.1 Name: bardapi Version: 0.1.9 Summary: The python package
 that returns Response of Google Bard through API. Home-page: https://
 github.com/dsdanielpark/Bard-API Author: daniel park Author-email:
 parkminwoo1991@gmail.com Keywords: Python,API,Bard,Google Bard,Large Language
 Model,Chatbot API,Google API,Chatbot Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Science/Research Classifier:
 Natural Language :: English Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
@@ -22,30 +22,35 @@
 > The python package that returns response of [Google Bard](https://
 bard.google.com/) through API. ![](./assets/bard_api.gif) I referred to [this
 github repository(github.com/acheong08/Bard)](https://github.com/acheong08/
 Bard) where inference process of Bard was reverse engineered. Using `__Secure-
 1PSID`, you can ask questions and get answers from Google Bard. This package is
 designed for application to the Python package [ExceptNotifier](https://
 github.com/dsdanielpark/ExceptNotifier) and [Co-Coder](https://github.com/
-dsdanielpark/Co-Coder).
+dsdanielpark/Co-Coder). Please note that the bardapi is not a free service, but
+rather a tool provided to assist developers with testing certain
+functionalities due to the delayed development and release of Google Bard's
+API. It has been designed with a lightweight structure that can easily adapt to
+the emergence of an official API. Therefore, I strongly discourage using it for
+any other purposes.
 Do not expose the `__Secure-1PSID` > Note that while I referred to `__Secure-
 1PSID` value as an API KEY for convenience, it is not an officially provided
 API KEY.
 ## [Amazing Bard Prompts](https://github.com/dsdanielpark/amazing-bard-prompts)
 Is All You Need! - Helpful prompts for Google Bard
 ## Install The latest stable release (and required dependencies) can be
 installed from PyPI: ``` pip install bardapi ``` You may instead want to use
 the development version from Github: ``` pip install git+https://github.com/
 dsdanielpark/Bard-API.git ```
 ## Authentication 1. Visit https://bard.google.com/ 2. F12 for console 3.
 Session: Application â Cookies â Copy the value of `__Secure-1PSID` cookie.
 
 ## Usage [![Open In Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/drive/
-1YIMA8aBmEQSSk90bB0Q9tznaLLQcluGA?usp=share_link) Simple Usage ```python from
+1zzzlTIh0kt2MdjLzvXRby1rWbHzmog8t?usp=sharing) Simple Usage ```python from
 bardapi import Bard token = 'xxxxxxxxxx' bard = Bard(token=token)
 bard.get_answer("ëì ë´ ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì
 ìë ¤ì¤")['content'] ``` Or you can use this ```python from bardapi import
 Bard import os os.environ['_BARD_API_KEY']="xxxxxxxx" Bard().get_answer("ëì
 ë´ ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì ìë ¤ì¤")['content']
 ``` To get reponse dictionary ```python import bardapi import os # set your
 __Secure-1PSID value to key token = 'xxxxxxxxxx' # set your input text
@@ -58,41 +63,74 @@
 ['_BARD_API_KEY']="xxxxxxxx" bard = Bard(timeout=30) # Set timeout in seconds
 bard.get_answer("ëì ë´ ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì
 ìë ¤ì¤")['content'] ```
 ## Futher ### Behind a proxy If you are working behind a proxy, use the
 following. ```python from bardapi import Bard import os os.environ
 ['_BARD_API_KEY']="xxxxxxxx" # Change 'http://127.0.0.1:1080' to your http
 proxy # timeout in seconds bard = Bard(proxies={'http':'http://127.0.0.1:1080',
-'https':'http://127.0.0.1:1080'}, timeout=10) bard.get_answer("ëì ë´
+'https':'http://127.0.0.1:1080'}, timeout=30) bard.get_answer("ëì ë´
 ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì ìë ¤ì¤")['content'] ```
-### Reusable session object ```python from bardapi import Bard import os import
-requests os.environ['_BARD_API_KEY'] = 'xxxxxxxxxxx' # token='xxxxxxxxxxx'
-session = requests.Session() session.headers = { "Host": "bard.google.com", "X-
-Same-Domain": "1", "User-Agent": "Mozilla/5.0 (Windows NT 10.0; WOW64)
-AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.114 Safari/537.36",
-"Content-Type": "application/x-www-form-urlencoded;charset=UTF-8", "Origin":
-"https://bard.google.com", "Referer": "https://bard.google.com/", }
-session.cookies.set("__Secure-1PSID", os.getenv("_BARD_API_KEY")) #
-session.cookies.set("__Secure-1PSID", token) bard = Bard(session=session,
-timeout=30) bard.get_answer("ëì ë´ ëëë°°ë¤ì´ ì¢ìíë
-ë´ì§ì¤ì ëí´ì ìë ¤ì¤")['content'] ``` Simple Example
-[./assets/bardimg.png]_
-##_Scripts_In_the_scripts_[folder](./scripts/),_I_have_released_a_script_to
-help_you_compare_[OpenAI-ChatGPT](./scripts/openai_api.ipynb)_and_[Google-Bard]
-(./scripts/google_api.ipynb)._I_hope_they_will_help_more_developers._##_License
+### Reusable session object You can continue the conversation through a
+reusable session. ```python from bardapi import Bard import os import requests
+os.environ['_BARD_API_KEY'] = 'xxxxxxxxxxx' # token='xxxxxxxxxxx' session =
+requests.Session() session.headers = { "Host": "bard.google.com", "X-Same-
+Domain": "1", "User-Agent": "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/
+537.36 (KHTML, like Gecko) Chrome/91.0.4472.114 Safari/537.36", "Content-Type":
+"application/x-www-form-urlencoded;charset=UTF-8", "Origin": "https://
+bard.google.com", "Referer": "https://bard.google.com/", } session.cookies.set
+("__Secure-1PSID", os.getenv("_BARD_API_KEY")) # session.cookies.set("__Secure-
+1PSID", token) bard = Bard(session=session, timeout=30) bard.get_answer("ëì
+ë´ ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì ìë ¤ì¤")['content']
+# Continued conversation without set new session bard.get_answer("What is my
+last prompt??")['content'] ``` ### Other languages To detect and translate
+using the Google Bard in unofficial languages, the Python package [googletrans]
+(https://github.com/ssut/py-googletrans) is utilized. ```python from bardapi
+import Bard token = 'xxxxxxx' bard = Bard(token=token, language='arabic') res =
+bard.get_answer("ÙÙ ØªØ¹Ø±Ù Ø§ÙÙÙÙØªØ´Ù") ``` Simple Example
+[./assets/bard_img.png]_
+##_Translation_to_Another_Programming_Language_Please_check_the_translation
+results_in_[this_folder](https://github.com/dsdanielpark/Bard-API/tree/main/
+translate_to)._-_Copy_the_code_of_[Core.py](https://github.com/dsdanielpark/
+Bard-API/blob/main/bardapi/core.py)._-_Ask_ChatGPT_to_translate_like_"Translate
+to_Swift."_-_Ask_ChatGPT_to_optimize_the_code_or_provide_any_desired
+instructions_until_you're_satisfied.
+![](./assets/translate.png)_##_Scripts_In_the_scripts_[folder](./scripts/),_I
+have_released_a_script_to_help_you_compare_[OpenAI-ChatGPT](./scripts/
+openai_api.ipynb),_[Microsoft-EdgeGPT](./scripts/microsoft_api.ipynb)_and_
+[Google-Bard](./scripts/google_api.ipynb)._I_hope_they_will_help_more
+developers._##_Shifting_Service_Policies:_Bard_and_Google's_Dynamics_Bard's
+service_status_and_Google's_API_interfaces_are_in_constant_flux._*The_number_of
+replies_is_currently_limited,_but_certain_users,*_such_as_those_utilizing_VPNs
+or_proxy_servers,_have_reported_slightly_higher_message_caps._Adaptability_is
+crucial_in_navigating_these_dynamic_service_policies._Please_note_that_the
+cookie_values_used_in_this_package_are_not_official_API_values._##_License_
 [MIT](https://opensource.org/license/mit/)_
 I_hold_no_legal_responsibility;_for_more_information,_please_refer_to_the
 bottom_of_the_readme_file._I_just_want_you_to_give_me_and_[them](https://
-github.com/acheong08/Bard)_a_star._##_Bugs_and_Issues_Sincerely_grateful_for
-any_reports_on_new_features_or_bugs._Your_valuable_feedback_on_the_code_is
-highly_appreciated._##_Contacts_-_Core_maintainer:_[Daniel_Park,_South_Korea]
-(https://github.com/DSDanielPark)_
+github.com/acheong08/Bard)_a_star._```_The_MIT_License_(MIT)_Copyright_(c)_2023
+Minwoo_Park_Permission_is_hereby_granted,_free_of_charge,_to_any_person
+obtaining_a_copy_of_this_software_and_associated_documentation_files_(the
+"Software"),_to_deal_in_the_Software_without_restriction,_including_without
+limitation_the_rights_to_use,_copy,_modify,_merge,_publish,_distribute,
+sublicense,_and/or_sell_copies_of_the_Software,_and_to_permit_persons_to_whom
+the_Software_is_furnished_to_do_so,_subject_to_the_following_conditions:_The
+above_copyright_notice_and_this_permission_notice_shall_be_included_in_all
+copies_or_substantial_portions_of_the_Software._THE_SOFTWARE_IS_PROVIDED_"AS
+IS",_WITHOUT_WARRANTY_OF_ANY_KIND,_EXPRESS_OR_IMPLIED,_INCLUDING_BUT_NOT
+LIMITED_TO_THE_WARRANTIES_OF_MERCHANTABILITY,_FITNESS_FOR_A_PARTICULAR_PURPOSE
+AND_NONINFRINGEMENT._IN_NO_EVENT_SHALL_THE_AUTHORS_OR_COPYRIGHT_HOLDERS_BE
+LIABLE_FOR_ANY_CLAIM,_DAMAGES_OR_OTHER_LIABILITY,_WHETHER_IN_AN_ACTION_OF
+CONTRACT,_TORT_OR_OTHERWISE,_ARISING_FROM,_OUT_OF_OR_IN_CONNECTION_WITH_THE
+SOFTWARE_OR_THE_USE_OR_OTHER_DEALINGS_IN_THE_SOFTWARE._```_##_Bugs_and_Issues
+Sincerely_grateful_for_any_reports_on_new_features_or_bugs._Your_valuable
+feedback_on_the_code_is_highly_appreciated._##_Contacts_-_Core_maintainer:_
+[Daniel_Park,_South_Korea](https://github.com/DSDanielPark)_
 -_E-mail:_parkminwoo1991@gmail.com_
-##_Reference_[1]_https://github.com/acheong08/Bard_###_Important_Notice_The
-user_assumes_all_legal_responsibilities_associated_with_using_the_BardAPI
-package._This_Python_package_merely_facilitates_easy_access_to_Google_Bard_for
-developers._Users_are_solely_responsible_for_managing_data_and_using_the
-package_appropriately._For_further_information,_please_consult_the_Google_Bard
-Official_Document._####_Could_you_kindly_add_this_badge_to_your_repository?
-markdown_```_![BardAPI](https://img.shields.io/badge/pypi-BardAPI-black)_```
-html_```_[PyPI_package]_```_Thank_you_for_your_interest._*Copyright_(c)_2023
-MinWoo_Park,_South_Korea*
+##_Reference_[1]_https://github.com/acheong08/Bard_
+###_Important_Notice_The_user_assumes_all_legal_responsibilities_associated
+with_using_the_BardAPI_package._This_Python_package_merely_facilitates_easy
+access_to_Google_Bard_for_developers._Users_are_solely_responsible_for_managing
+data_and_using_the_package_appropriately._For_further_information,_please
+consult_the_Google_Bard_Official_Document._####_Could_you_kindly_add_this_badge
+to_your_repository?_markdown_```_![BardAPI](https://img.shields.io/badge/pypi-
+BardAPI-black)_```_html_```_[PyPI_package]_```_Thank_you_for_your_interest.
+*Copyright_(c)_2023_MinWoo_Park,_South_Korea*
```

### Comparing `bardapi-0.1.8/setup.py` & `bardapi-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,24 +21,24 @@
 
 
 version = get_version()
 
 
 setup(
     name="bardapi",
-    version="0.1.8",
+    version="0.1.9",
     author="daniel park",
     author_email="parkminwoo1991@gmail.com",
     description="The python package that returns Response of Google Bard through API.",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/dsdanielpark/Bard-API",
     packages=find_packages(exclude=[]),
     python_requires=">=3.6",
-    install_requires=["requests"],
+    install_requires=["requests", "googletrans"],
     keywords="Python, API, Bard, Google Bard, Large Language Model, Chatbot API, Google API, Chatbot",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Science/Research",
         "Natural Language :: English",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.6",
```


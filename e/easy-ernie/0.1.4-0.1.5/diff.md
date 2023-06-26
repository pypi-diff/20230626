# Comparing `tmp/easy-ernie-0.1.4.tar.gz` & `tmp/easy-ernie-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy-ernie-0.1.4.tar", last modified: Sat May  6 11:25:52 2023, max compression
+gzip compressed data, was "easy-ernie-0.1.5.tar", last modified: Mon Jun 26 11:28:14 2023, max compression
```

## Comparing `easy-ernie-0.1.4.tar` & `easy-ernie-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 xiaoxinyo   (501) staff       (20)        0 2023-05-06 11:25:52.825613 easy-ernie-0.1.4/
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)     1065 2023-04-26 08:52:25.000000 easy-ernie-0.1.4/LICENSE
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)     1960 2023-05-06 11:25:52.825431 easy-ernie-0.1.4/PKG-INFO
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)     1347 2023-04-29 09:02:38.000000 easy-ernie-0.1.4/README.md
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)       38 2023-05-06 11:25:52.825659 easy-ernie-0.1.4/setup.cfg
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)      936 2023-04-29 09:58:19.000000 easy-ernie-0.1.4/setup.py
-drwxr-xr-x   0 xiaoxinyo   (501) staff       (20)        0 2023-05-06 11:25:52.818039 easy-ernie-0.1.4/src/
-drwxr-xr-x   0 xiaoxinyo   (501) staff       (20)        0 2023-05-06 11:25:52.819390 easy-ernie-0.1.4/src/easy_ernie/
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)      126 2023-04-27 13:27:18.000000 easy-ernie-0.1.4/src/easy_ernie/__init__.py
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)     7146 2023-05-06 10:46:35.000000 easy-ernie-0.1.4/src/easy_ernie/ernie.py
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)      985 2023-05-06 11:25:07.000000 easy-ernie-0.1.4/src/easy_ernie/fast_ernie.py
-drwxr-xr-x   0 xiaoxinyo   (501) staff       (20)        0 2023-05-06 11:25:52.820228 easy-ernie-0.1.4/src/easy_ernie.egg-info/
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)     1960 2023-05-06 11:25:52.000000 easy-ernie-0.1.4/src/easy_ernie.egg-info/PKG-INFO
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)      311 2023-05-06 11:25:52.000000 easy-ernie-0.1.4/src/easy_ernie.egg-info/SOURCES.txt
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)        1 2023-05-06 11:25:52.000000 easy-ernie-0.1.4/src/easy_ernie.egg-info/dependency_links.txt
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)        9 2023-05-06 11:25:52.000000 easy-ernie-0.1.4/src/easy_ernie.egg-info/requires.txt
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)       11 2023-05-06 11:25:52.000000 easy-ernie-0.1.4/src/easy_ernie.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 11:28:14.929861 easy-ernie-0.1.5/
+-rw-rw-rw-   0        0        0     1065 2023-04-26 08:52:25.000000 easy-ernie-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     2226 2023-06-26 11:28:14.929371 easy-ernie-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1548 2023-05-12 11:13:36.000000 easy-ernie-0.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-26 11:28:14.929861 easy-ernie-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      936 2023-05-06 11:29:36.000000 easy-ernie-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 11:28:14.922357 easy-ernie-0.1.5/src/
+drwxrwxrwx   0        0        0        0 2023-06-26 11:28:14.928871 easy-ernie-0.1.5/src/easy_ernie/
+-rw-rw-rw-   0        0        0      126 2023-05-06 11:29:23.000000 easy-ernie-0.1.5/src/easy_ernie/__init__.py
+-rw-rw-rw-   0        0        0     7248 2023-06-26 09:57:08.000000 easy-ernie-0.1.5/src/easy_ernie/ernie.py
+-rw-rw-rw-   0        0        0      985 2023-05-13 09:56:44.000000 easy-ernie-0.1.5/src/easy_ernie/fast_ernie.py
+drwxrwxrwx   0        0        0        0 2023-06-26 11:28:14.927371 easy-ernie-0.1.5/src/easy_ernie.egg-info/
+-rw-rw-rw-   0        0        0     2226 2023-06-26 11:28:14.000000 easy-ernie-0.1.5/src/easy_ernie.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      341 2023-06-26 11:28:14.000000 easy-ernie-0.1.5/src/easy_ernie.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 11:28:14.000000 easy-ernie-0.1.5/src/easy_ernie.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-26 11:28:14.000000 easy-ernie-0.1.5/src/easy_ernie.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-26 11:28:14.000000 easy-ernie-0.1.5/src/easy_ernie.egg-info/top_level.txt
```

### Comparing `easy-ernie-0.1.4/LICENSE` & `easy-ernie-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `easy-ernie-0.1.4/PKG-INFO` & `easy-ernie-0.1.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,62 +1,65 @@
-Metadata-Version: 2.1
-Name: easy-ernie
-Version: 0.1.4
-Summary: 简洁的调用文心一言的WebAPI
-Home-page: https://github.com/XiaoXinYo/Easy-Ernie
-Author: XiaoXinYo
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-![Release](https://img.shields.io/badge/Release-0.1.4-blue)
----
-## 介绍
-简洁的调用文心一言的WebAPI
-## 需求
-1. 语言: Python3.8+.
-2. 包: requests.
-3. 其他: 文心一言账户.
-## 安装
-pip3 install easy-ernie --upgrade
-## Cookie
-![图片1](https://s1.ax1x.com/2023/04/26/p9KDUYR.md.png)
-1. 访问[文心一言](https://yiyan.baidu.com).
-2. 打开开发者工具.
-3. 找到应用程序(Application).
-4. 在左侧点击存储(Storage)-Cookies-https://yiyan.baidu.com.
-5. 在列表中点击BAIDUID.
-6. 复制下方Cookie Value的值.
-7. BDUSS_BFESS同理.
-## 使用
-### Ernie
-```python
-from easy_ernie import Ernie
-
-if __name__ == '__main__':
-    ernie = Ernie('BAIDUID', 'BDUSS_BFESS')
-    sessionId = ernie.newConversation('测试')
-    print(ernie.ask(question, '你好', '0'))
-    ernie.deleteConversation(sessionId)
-```
-### FastErinie
-```python
-from easy_ernie import FastErnie
-
-if __name__ == '__main__':
-    fastErnie = FastErnie('BAIDUID', 'BDUSS_BFESS')
-    print(fastErnie.ask('你好'))
-    fastErnie.close()
-```
-更多方法查看[Wiki](https://github.com/XiaoXinYo/Easy-Ernie/wiki).
-## Acs-Token
-由于文心一言的Acs-Token算法中的参数不定时的变化,所以包里调用了API.感兴趣的可以联系我.
-## 感谢
-灵感来源自[acheong08](https://github.com/acheong08),[ls233](https://github.com/lss233).
+Metadata-Version: 2.1
+Name: easy-ernie
+Version: 0.1.5
+Summary: 简洁的调用文心一言的WebAPI
+Home-page: https://github.com/XiaoXinYo/Easy-Ernie
+Author: XiaoXinYo
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+## 提示
+1. 有封号风险.
+2. 由于文心一言的Acs-Token算法的参数不定时的变化,所以包里调用了API.感兴趣的或有自动更新方法的可以联系我.
+3. 若出现了`用户访问被限制`请到[Isuue](https://github.com/XiaoXinYo/Easy-Ernie/issues/6)回复,我会及时更新Acs-Token算法的参数.
+---
+![Release](https://img.shields.io/badge/Release-0.1.5-blue)
+---
+## 介绍
+简洁的调用文心一言的WebAPI
+## 需求
+1. 语言: Python3.8+.
+2. 包: requests.
+3. 其他: 文心一言账户.
+## 安装
+pip3 install easy-ernie --upgrade
+## Cookie
+![图片1](https://s1.ax1x.com/2023/04/26/p9KDUYR.md.png)
+1. 访问[文心一言](https://yiyan.baidu.com).
+2. 打开开发者工具.
+3. 找到应用程序(Application).
+4. 在左侧点击存储(Storage)-Cookies-https://yiyan.baidu.com.
+5. 在列表中点击BAIDUID.
+6. 复制下方Cookie Value的值.
+7. BDUSS_BFESS同理.
+## 使用
+### Ernie
+```python
+from easy_ernie import Ernie
+
+if __name__ == '__main__':
+    ernie = Ernie('BAIDUID', 'BDUSS_BFESS')
+    sessionId = ernie.newConversation('测试')
+    print(ernie.ask('你好', sessionId, '0'))
+    ernie.deleteConversation(sessionId)
+```
+### FastErinie
+```python
+from easy_ernie import FastErnie
+
+if __name__ == '__main__':
+    fastErnie = FastErnie('BAIDUID', 'BDUSS_BFESS')
+    print(fastErnie.ask('你好'))
+    fastErnie.close()
+```
+更多方法查看[Wiki](https://github.com/XiaoXinYo/Easy-Ernie/wiki).
+## 感谢
+灵感来源自[acheong08](https://github.com/acheong08),[ls233](https://github.com/lss233).
```

### Comparing `easy-ernie-0.1.4/README.md` & `easy-ernie-0.1.5/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-![Release](https://img.shields.io/badge/Release-0.1.4-blue)
+## 提示
+1. 有封号风险.
+2. 由于文心一言的Acs-Token算法的参数不定时的变化,所以包里调用了API.感兴趣的或有自动更新方法的可以联系我.
+3. 若出现了`用户访问被限制`请到[Isuue](https://github.com/XiaoXinYo/Easy-Ernie/issues/6)回复,我会及时更新Acs-Token算法的参数.
+---
+![Release](https://img.shields.io/badge/Release-0.1.5-blue)
 ---
 ## 介绍
 简洁的调用文心一言的WebAPI
 ## 需求
 1. 语言: Python3.8+.
 2. 包: requests.
 3. 其他: 文心一言账户.
@@ -21,24 +26,22 @@
 ### Ernie
 ```python
 from easy_ernie import Ernie
 
 if __name__ == '__main__':
     ernie = Ernie('BAIDUID', 'BDUSS_BFESS')
     sessionId = ernie.newConversation('测试')
-    print(ernie.ask(question, '你好', '0'))
+    print(ernie.ask('你好', sessionId, '0'))
     ernie.deleteConversation(sessionId)
 ```
 ### FastErinie
 ```python
 from easy_ernie import FastErnie
 
 if __name__ == '__main__':
     fastErnie = FastErnie('BAIDUID', 'BDUSS_BFESS')
     print(fastErnie.ask('你好'))
     fastErnie.close()
 ```
 更多方法查看[Wiki](https://github.com/XiaoXinYo/Easy-Ernie/wiki).
-## Acs-Token
-由于文心一言的Acs-Token算法中的参数不定时的变化,所以包里调用了API.感兴趣的可以联系我.
 ## 感谢
 灵感来源自[acheong08](https://github.com/acheong08),[ls233](https://github.com/lss233).
```

### Comparing `easy-ernie-0.1.4/setup.py` & `easy-ernie-0.1.5/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('./README.md', 'r', encoding='utf-8') as file:
     long_description = file.read()
 
 setup(
     name='easy-ernie',
-    version='0.1.4',
+    version='0.1.5',
     description='简洁的调用文心一言的WebAPI',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='XiaoXinYo',
     url='https://github.com/XiaoXinYo/Easy-Ernie',
     packages=find_packages('./src'),
     license='MIT',
```

### Comparing `easy-ernie-0.1.4/src/easy_ernie/ernie.py` & `easy-ernie-0.1.5/src/easy_ernie/ernie.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,16 @@
 
     def newConversation(self, name: str) -> str:
         data = self.post(
             'https://yiyan.baidu.com/eb/session/new',
             {
                 'sessionName': name,
                 'timestamp': getTimestamp(),
-                'deviceType': 'pc'
+                'deviceType': 'pc',
+                'plugins': []
             }
         ).json()
         return data['data']['sessionId']
     
     def deleteConversation(self, sessionId: str) -> bool:
         data = self.post(
             'https://yiyan.baidu.com/eb/session/delete',
@@ -119,15 +120,15 @@
                 'deviceType': 'pc'
             }
         ).json()
         return data['data']['currentChatId']
 
     def askStream(self, question: str, sessionId: str, parentChatId: str) -> Generator:
         self.post(
-            'https://yiyan.baidu.com/eb/chat/check',
+            'https://yiyan.baidu.com/eb/chat/checkAndBan',
             {
                 'text': question,
                 'timestamp': getTimestamp(),
                 'deviceType': 'pc'
             }
         )
 
@@ -141,15 +142,17 @@
                 'parentChatId': parentChatId,
                 'type': 10,
                 'timestamp': getTimestamp(),
                 'deviceType': 'pc',
                 'code': 0,
                 'msg': '',
                 'jt': '',
-                'sign': sign
+                'sign': sign,
+                'pluginInfo': [],
+                'plugins': []
             }
         ).json()
         botChatId = data['data']['botChat']['id']
         botParentChatId = data['data']['botChat']['parent']
 
         fullAnswer = ''
         pattern = r'<img[^>]*\ssrc=[\'"]([^\'"]+)[\'"][^>]*\s/>'
```

### Comparing `easy-ernie-0.1.4/src/easy_ernie/fast_ernie.py` & `easy-ernie-0.1.5/src/easy_ernie/fast_ernie.py`

 * *Files identical despite different names*

### Comparing `easy-ernie-0.1.4/src/easy_ernie.egg-info/PKG-INFO` & `easy-ernie-0.1.5/src/easy_ernie.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,62 +1,65 @@
-Metadata-Version: 2.1
-Name: easy-ernie
-Version: 0.1.4
-Summary: 简洁的调用文心一言的WebAPI
-Home-page: https://github.com/XiaoXinYo/Easy-Ernie
-Author: XiaoXinYo
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-![Release](https://img.shields.io/badge/Release-0.1.4-blue)
----
-## 介绍
-简洁的调用文心一言的WebAPI
-## 需求
-1. 语言: Python3.8+.
-2. 包: requests.
-3. 其他: 文心一言账户.
-## 安装
-pip3 install easy-ernie --upgrade
-## Cookie
-![图片1](https://s1.ax1x.com/2023/04/26/p9KDUYR.md.png)
-1. 访问[文心一言](https://yiyan.baidu.com).
-2. 打开开发者工具.
-3. 找到应用程序(Application).
-4. 在左侧点击存储(Storage)-Cookies-https://yiyan.baidu.com.
-5. 在列表中点击BAIDUID.
-6. 复制下方Cookie Value的值.
-7. BDUSS_BFESS同理.
-## 使用
-### Ernie
-```python
-from easy_ernie import Ernie
-
-if __name__ == '__main__':
-    ernie = Ernie('BAIDUID', 'BDUSS_BFESS')
-    sessionId = ernie.newConversation('测试')
-    print(ernie.ask(question, '你好', '0'))
-    ernie.deleteConversation(sessionId)
-```
-### FastErinie
-```python
-from easy_ernie import FastErnie
-
-if __name__ == '__main__':
-    fastErnie = FastErnie('BAIDUID', 'BDUSS_BFESS')
-    print(fastErnie.ask('你好'))
-    fastErnie.close()
-```
-更多方法查看[Wiki](https://github.com/XiaoXinYo/Easy-Ernie/wiki).
-## Acs-Token
-由于文心一言的Acs-Token算法中的参数不定时的变化,所以包里调用了API.感兴趣的可以联系我.
-## 感谢
-灵感来源自[acheong08](https://github.com/acheong08),[ls233](https://github.com/lss233).
+Metadata-Version: 2.1
+Name: easy-ernie
+Version: 0.1.5
+Summary: 简洁的调用文心一言的WebAPI
+Home-page: https://github.com/XiaoXinYo/Easy-Ernie
+Author: XiaoXinYo
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+## 提示
+1. 有封号风险.
+2. 由于文心一言的Acs-Token算法的参数不定时的变化,所以包里调用了API.感兴趣的或有自动更新方法的可以联系我.
+3. 若出现了`用户访问被限制`请到[Isuue](https://github.com/XiaoXinYo/Easy-Ernie/issues/6)回复,我会及时更新Acs-Token算法的参数.
+---
+![Release](https://img.shields.io/badge/Release-0.1.5-blue)
+---
+## 介绍
+简洁的调用文心一言的WebAPI
+## 需求
+1. 语言: Python3.8+.
+2. 包: requests.
+3. 其他: 文心一言账户.
+## 安装
+pip3 install easy-ernie --upgrade
+## Cookie
+![图片1](https://s1.ax1x.com/2023/04/26/p9KDUYR.md.png)
+1. 访问[文心一言](https://yiyan.baidu.com).
+2. 打开开发者工具.
+3. 找到应用程序(Application).
+4. 在左侧点击存储(Storage)-Cookies-https://yiyan.baidu.com.
+5. 在列表中点击BAIDUID.
+6. 复制下方Cookie Value的值.
+7. BDUSS_BFESS同理.
+## 使用
+### Ernie
+```python
+from easy_ernie import Ernie
+
+if __name__ == '__main__':
+    ernie = Ernie('BAIDUID', 'BDUSS_BFESS')
+    sessionId = ernie.newConversation('测试')
+    print(ernie.ask('你好', sessionId, '0'))
+    ernie.deleteConversation(sessionId)
+```
+### FastErinie
+```python
+from easy_ernie import FastErnie
+
+if __name__ == '__main__':
+    fastErnie = FastErnie('BAIDUID', 'BDUSS_BFESS')
+    print(fastErnie.ask('你好'))
+    fastErnie.close()
+```
+更多方法查看[Wiki](https://github.com/XiaoXinYo/Easy-Ernie/wiki).
+## 感谢
+灵感来源自[acheong08](https://github.com/acheong08),[ls233](https://github.com/lss233).
```


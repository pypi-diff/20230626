# Comparing `tmp/yandex_reviews_parser-0.1.0.tar.gz` & `tmp/yandex_reviews_parser-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yandex_reviews_parser-0.1.0.tar", max compression
+gzip compressed data, was "yandex_reviews_parser-0.1.1.tar", max compression
```

## Comparing `yandex_reviews_parser-0.1.0.tar` & `yandex_reviews_parser-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      472 2023-06-26 12:21:04.112244 yandex_reviews_parser-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1163 2023-06-15 13:03:56.663408 yandex_reviews_parser-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-26 11:09:42.496887 yandex_reviews_parser-0.1.0/src/__init__.py
--rw-r--r--   0        0        0      622 2023-06-15 12:55:11.760000 yandex_reviews_parser-0.1.0/src/helpers.py
--rw-r--r--   0        0        0      285 2023-06-26 11:10:55.777540 yandex_reviews_parser-0.1.0/src/main.py
--rw-r--r--   0        0        0     8371 2023-06-23 08:38:19.391000 yandex_reviews_parser-0.1.0/src/parsers.py
--rw-r--r--   0        0        0      292 2023-06-26 11:06:20.067000 yandex_reviews_parser-0.1.0/src/storage.py
--rw-r--r--   0        0        0     1755 2023-06-23 08:42:18.704000 yandex_reviews_parser-0.1.0/src/utils.py
--rw-r--r--   0        0        0     1804 1970-01-01 00:00:00.000000 yandex_reviews_parser-0.1.0/setup.py
--rw-r--r--   0        0        0     1712 1970-01-01 00:00:00.000000 yandex_reviews_parser-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      472 2023-06-26 12:28:10.684380 yandex_reviews_parser-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1662 2023-06-26 12:27:06.795070 yandex_reviews_parser-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-26 11:09:42.496887 yandex_reviews_parser-0.1.1/src/__init__.py
+-rw-r--r--   0        0        0      622 2023-06-15 12:55:11.760000 yandex_reviews_parser-0.1.1/src/helpers.py
+-rw-r--r--   0        0        0      285 2023-06-26 11:10:55.777540 yandex_reviews_parser-0.1.1/src/main.py
+-rw-r--r--   0        0        0     8371 2023-06-23 08:38:19.391000 yandex_reviews_parser-0.1.1/src/parsers.py
+-rw-r--r--   0        0        0      292 2023-06-26 11:06:20.067000 yandex_reviews_parser-0.1.1/src/storage.py
+-rw-r--r--   0        0        0     1755 2023-06-23 08:42:18.704000 yandex_reviews_parser-0.1.1/src/utils.py
+-rw-r--r--   0        0        0     2307 1970-01-01 00:00:00.000000 yandex_reviews_parser-0.1.1/setup.py
+-rw-r--r--   0        0        0     2200 1970-01-01 00:00:00.000000 yandex_reviews_parser-0.1.1/PKG-INFO
```

### Comparing `yandex_reviews_parser-0.1.0/README.md` & `yandex_reviews_parser-0.1.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Парсер отзывов c Yandex Карт
 
 Скрипт парсит отзывы с Yandex Карт<br>
 Для парсинга необходимо указать id компании в начале обработки скрипта
 
-По результатам выполнения, создается файл result.json, в котором:
+По результатам выполнения, возвращается объект, в котором:
 ```json
 {
   "company_info": {
     "name": "Дилерский центр Hyundai",
     "rating": 5.0,
     "count_rating": 380,
     "stars": 5
@@ -15,24 +15,35 @@
   "company_reviews": [
     {
       "name": "Иван Иванов",
       "icon_href": "https://avatars.mds.yandex.net/get-yapic/51381/cs8Tx0sigtfayYhRQBDJkavzJU-1/islands-68",
       "date": 1681992580.04,
       "text": "Выражаю огромную благодарность работникам ",
       "stars": 5
+    },
+    {
+      "name": "Иван Иванов",
+      "icon_href": "https://avatars.mds.yandex.net/get-yapic/51381/cs8Tx0sigtfayYhRQBDJkavzJU-1/islands-68",
+      "date": 1681992580.04,
+      "text": "Выражаю огромную благодарность работникам ",
+      "stars": 5
     }
   ]
 }
 ```
 
 
-Необходимо установить пакеты<br>
+Необходимо установить библиотеку<br>
 ```shell
-pip install -R requirements.txt
+pip install yandex-reviews-parser
 ```
 
-Далее запусить main.py
-```shell
-python main.py
-```
-Вводим ID компании которую нужно спарсить.<br>
-И получаем результат
+```python
+import YandexParser
+
+id_ya = 1234 #ID Компании Yandex
+parser = YandexParser(id_ya)
+
+all_data = parser.parse() #Получаем все данные
+company = parser.parse(type_parse='company') #Получаем данные по компании
+reviews = parser.parse(type_parse='company') #Получаем список отзывов
+```
```

### Comparing `yandex_reviews_parser-0.1.0/src/helpers.py` & `yandex_reviews_parser-0.1.1/src/helpers.py`

 * *Files identical despite different names*

### Comparing `yandex_reviews_parser-0.1.0/src/parsers.py` & `yandex_reviews_parser-0.1.1/src/parsers.py`

 * *Files identical despite different names*

### Comparing `yandex_reviews_parser-0.1.0/src/utils.py` & `yandex_reviews_parser-0.1.1/src/utils.py`

 * *Files identical despite different names*

### Comparing `yandex_reviews_parser-0.1.0/setup.py` & `yandex_reviews_parser-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['undetected-chromedriver>=3.5.0,<4.0.0']
 
 setup_kwargs = {
     'name': 'yandex-reviews-parser',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'Python yandex company reviews parser',
-    'long_description': '# Парсер отзывов c Yandex Карт\n\nСкрипт парсит отзывы с Yandex Карт<br>\nДля парсинга необходимо указать id компании в начале обработки скрипта\n\nПо результатам выполнения, создается файл result.json, в котором:\n```json\n{\n  "company_info": {\n    "name": "Дилерский центр Hyundai",\n    "rating": 5.0,\n    "count_rating": 380,\n    "stars": 5\n  },\n  "company_reviews": [\n    {\n      "name": "Иван Иванов",\n      "icon_href": "https://avatars.mds.yandex.net/get-yapic/51381/cs8Tx0sigtfayYhRQBDJkavzJU-1/islands-68",\n      "date": 1681992580.04,\n      "text": "Выражаю огромную благодарность работникам ",\n      "stars": 5\n    }\n  ]\n}\n```\n\n\nНеобходимо установить пакеты<br>\n```shell\npip install -R requirements.txt\n```\n\nДалее запусить main.py\n```shell\npython main.py\n```\nВводим ID компании которую нужно спарсить.<br>\nИ получаем результат',
+    'long_description': '# Парсер отзывов c Yandex Карт\n\nСкрипт парсит отзывы с Yandex Карт<br>\nДля парсинга необходимо указать id компании в начале обработки скрипта\n\nПо результатам выполнения, возвращается объект, в котором:\n```json\n{\n  "company_info": {\n    "name": "Дилерский центр Hyundai",\n    "rating": 5.0,\n    "count_rating": 380,\n    "stars": 5\n  },\n  "company_reviews": [\n    {\n      "name": "Иван Иванов",\n      "icon_href": "https://avatars.mds.yandex.net/get-yapic/51381/cs8Tx0sigtfayYhRQBDJkavzJU-1/islands-68",\n      "date": 1681992580.04,\n      "text": "Выражаю огромную благодарность работникам ",\n      "stars": 5\n    },\n    {\n      "name": "Иван Иванов",\n      "icon_href": "https://avatars.mds.yandex.net/get-yapic/51381/cs8Tx0sigtfayYhRQBDJkavzJU-1/islands-68",\n      "date": 1681992580.04,\n      "text": "Выражаю огромную благодарность работникам ",\n      "stars": 5\n    }\n  ]\n}\n```\n\n\nНеобходимо установить библиотеку<br>\n```shell\npip install yandex-reviews-parser\n```\n\n```python\nimport YandexParser\n\nid_ya = 1234 #ID Компании Yandex\nparser = YandexParser(id_ya)\n\nall_data = parser.parse() #Получаем все данные\ncompany = parser.parse(type_parse=\'company\') #Получаем данные по компании\nreviews = parser.parse(type_parse=\'company\') #Получаем список отзывов\n```',
     'author': 'Daniil',
     'author_email': 'danil16m@mail.ru',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `yandex_reviews_parser-0.1.0/PKG-INFO` & `yandex_reviews_parser-0.1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yandex-reviews-parser
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python yandex company reviews parser
 License: MIT
 Keywords: python,yandex,parser,reviews
 Author: Daniil
 Author-email: danil16m@mail.ru
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -16,15 +16,15 @@
 Description-Content-Type: text/markdown
 
 # Парсер отзывов c Yandex Карт
 
 Скрипт парсит отзывы с Yandex Карт<br>
 Для парсинга необходимо указать id компании в начале обработки скрипта
 
-По результатам выполнения, создается файл result.json, в котором:
+По результатам выполнения, возвращается объект, в котором:
 ```json
 {
   "company_info": {
     "name": "Дилерский центр Hyundai",
     "rating": 5.0,
     "count_rating": 380,
     "stars": 5
@@ -32,24 +32,35 @@
   "company_reviews": [
     {
       "name": "Иван Иванов",
       "icon_href": "https://avatars.mds.yandex.net/get-yapic/51381/cs8Tx0sigtfayYhRQBDJkavzJU-1/islands-68",
       "date": 1681992580.04,
       "text": "Выражаю огромную благодарность работникам ",
       "stars": 5
+    },
+    {
+      "name": "Иван Иванов",
+      "icon_href": "https://avatars.mds.yandex.net/get-yapic/51381/cs8Tx0sigtfayYhRQBDJkavzJU-1/islands-68",
+      "date": 1681992580.04,
+      "text": "Выражаю огромную благодарность работникам ",
+      "stars": 5
     }
   ]
 }
 ```
 
 
-Необходимо установить пакеты<br>
+Необходимо установить библиотеку<br>
 ```shell
-pip install -R requirements.txt
+pip install yandex-reviews-parser
 ```
 
-Далее запусить main.py
-```shell
-python main.py
+```python
+import YandexParser
+
+id_ya = 1234 #ID Компании Yandex
+parser = YandexParser(id_ya)
+
+all_data = parser.parse() #Получаем все данные
+company = parser.parse(type_parse='company') #Получаем данные по компании
+reviews = parser.parse(type_parse='company') #Получаем список отзывов
 ```
-Вводим ID компании которую нужно спарсить.<br>
-И получаем результат
```


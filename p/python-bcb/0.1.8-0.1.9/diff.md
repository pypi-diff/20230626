# Comparing `tmp/python-bcb-0.1.8.tar.gz` & `tmp/python_bcb-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-bcb-0.1.8.tar", max compression
+gzip compressed data, was "python_bcb-0.1.9.tar", max compression
```

## Comparing `python-bcb-0.1.8.tar` & `python_bcb-0.1.9.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0    16017 2022-09-10 20:51:17.353666 python-bcb-0.1.8/bcb/__init__.py
--rw-r--r--   0        0        0     5888 2022-09-10 20:51:28.515769 python-bcb-0.1.8/bcb/currency.py
--rw-r--r--   0        0        0    15443 2022-09-10 20:51:40.176864 python-bcb-0.1.8/bcb/odata.py
--rw-r--r--   0        0        0     4422 2022-09-10 20:21:41.556905 python-bcb-0.1.8/bcb/sgs.py
--rw-r--r--   0        0        0     1089 2022-09-10 20:51:53.559187 python-bcb-0.1.8/bcb/utils.py
--rw-r--r--   0        0        0     1070 2021-01-16 19:16:53.504736 python-bcb-0.1.8/LICENSE
--rw-r--r--   0        0        0      738 2022-09-10 20:55:06.820978 python-bcb-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2065 2022-03-30 10:14:29.317008 python-bcb-0.1.8/README.md
--rw-r--r--   0        0        0     2734 1970-01-01 00:00:00.000000 python-bcb-0.1.8/setup.py
--rw-r--r--   0        0        0     2558 1970-01-01 00:00:00.000000 python-bcb-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    16003 2022-09-11 20:49:09.883282 python_bcb-0.1.9/bcb/__init__.py
+-rw-r--r--   0        0        0     5888 2022-09-10 20:51:28.515769 python_bcb-0.1.9/bcb/currency.py
+-rw-r--r--   0        0        0    15443 2022-09-10 20:51:40.176864 python_bcb-0.1.9/bcb/odata.py
+-rw-r--r--   0        0        0     4513 2022-09-13 08:18:17.540281 python_bcb-0.1.9/bcb/sgs.py
+-rw-r--r--   0        0        0     1089 2022-09-10 20:51:53.559187 python_bcb-0.1.9/bcb/utils.py
+-rw-r--r--   0        0        0     1070 2021-01-16 19:16:53.504736 python_bcb-0.1.9/LICENSE
+-rw-r--r--   0        0        0      761 2023-06-26 20:21:16.356313 python_bcb-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2065 2022-03-30 10:14:29.317008 python_bcb-0.1.9/README.md
+-rw-r--r--   0        0        0     2510 1970-01-01 00:00:00.000000 python_bcb-0.1.9/PKG-INFO
```

### Comparing `python-bcb-0.1.8/bcb/__init__.py` & `python_bcb-0.1.9/bcb/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,28 +125,28 @@
         ------
         ValueError
             Se o *endpoint* fornecido é errado.
         """
         return Endpoint(self.service[endpoint], self.service.url)
 
 
-class GenericODataAPI(BaseODataAPI):
+class ODataAPI(BaseODataAPI):
     """
     Classe que abstrai qualquer API OData
 
     Essa classe pode ser acessada diretamente passando
     uma URL válida para uma API OData.
 
     Uma boa alternativa para acessar APIs que ainda
     não possuem implementação específica.
     """
 
     def __init__(self, url):
         """
-        GenericODataAPI construtor
+        ODataAPI construtor
 
         Parameters
         ----------
 
         url : str
             URL de API OData
```

### Comparing `python-bcb-0.1.8/bcb/currency.py` & `python_bcb-0.1.9/bcb/currency.py`

 * *Files identical despite different names*

### Comparing `python-bcb-0.1.8/bcb/odata.py` & `python_bcb-0.1.9/bcb/odata.py`

 * *Files identical despite different names*

### Comparing `python-bcb-0.1.8/bcb/sgs.py` & `python_bcb-0.1.9/bcb/sgs.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from io import StringIO
 
 import requests
 import pandas as pd
 
 from .utils import Date
 
@@ -38,60 +37,56 @@
             yield SGSCode(cd[1], cd[0]) if _ist else SGSCode(cd)
     elif isinstance(codes, dict):
         for cd in codes:
             yield SGSCode(codes[cd], cd)
 
 
 def _get_url_and_payload(code, start_date, end_date, last):
-    payload = {'formato': 'json'}
+    payload = {"formato": "json"}
     if last == 0:
         if start_date is not None or end_date is not None:
-            payload['dataInicial'] = Date(start_date).date.strftime('%d/%m/%Y')
-            end_date = end_date if end_date else 'today'
-            payload['dataFinal'] = Date(end_date).date.strftime('%d/%m/%Y')
-        url = 'http://api.bcb.gov.br/dados/serie/bcdata.sgs.{}/dados'\
-            .format(code)
+            payload["dataInicial"] = Date(start_date).date.strftime("%d/%m/%Y")
+            end_date = end_date if end_date else "today"
+            payload["dataFinal"] = Date(end_date).date.strftime("%d/%m/%Y")
+        url = "http://api.bcb.gov.br/dados/serie/bcdata.sgs.{}/dados".format(code)
     else:
-        url = ('http://api.bcb.gov.br/dados/serie/bcdata.sgs.{}/dados'
-               '/ultimos/{}').format(code, last)
+        url = (
+            "http://api.bcb.gov.br/dados/serie/bcdata.sgs.{}/dados" "/ultimos/{}"
+        ).format(code, last)
 
-    return {
-        'payload': payload,
-        'url': url
-    }
+    return {"payload": payload, "url": url}
 
 
 def _format_df(df, code, freq):
-    cns = {'data': 'Date', 'valor': code.name, 'datafim': 'enddate'}
+    cns = {"data": "Date", "valor": code.name, "datafim": "enddate"}
     df = df.rename(columns=cns)
-    if 'Date' in df:
-        df['Date'] = pd.to_datetime(df['Date'], format='%d/%m/%Y')
-    if 'enddate' in df:
-        df['enddate'] = pd.to_datetime(df['enddate'], format='%d/%m/%Y')
-    df = df.set_index('Date')
+    if "Date" in df:
+        df["Date"] = pd.to_datetime(df["Date"], format="%d/%m/%Y")
+    if "enddate" in df:
+        df["enddate"] = pd.to_datetime(df["enddate"], format="%d/%m/%Y")
+    df = df.set_index("Date")
     if freq:
         df.index = df.index.to_period(freq)
     return df
 
 
 def get(codes, start=None, end=None, last=0, multi=True, freq=None):
-    '''
+    """
     Retorna um DataFrame pandas com séries temporais obtidas do SGS.
 
     Parameters
     ----------
 
-    symbols : {int, List[int], List[str], Dict[str:int]}
+    codes : {int, List[int], List[str], Dict[str:int]}
         Este argumento pode ser uma das opções:
 
-        ``int`` : código da série temporal
-
-        ``list`` ou ``tuple`` : lista ou tupla com pares ``('nome', código)``
-
-        ``dict`` : dicionário com pares ``{'nome': código}``
+        * ``int`` : código da série temporal
+        * ``list`` ou ``tuple`` : lista ou tupla com códigos
+        * ``list`` ou ``tuple`` : lista ou tupla com pares ``('nome', código)``
+        * ``dict`` : dicionário com pares ``{'nome': código}``
 
         Com códigos numéricos é interessante utilizar os nomes com os códigos
         para definir os nomes nas colunas das séries temporais.
     start : str, int, date, datetime, Timestamp
         Data de início da série.
         Interpreta diferentes tipos e formatos de datas.
     end : string, int, date, datetime, Timestamp
@@ -108,26 +103,26 @@
         Define a frequência a ser utilizada na série temporal
 
     Returns
     -------
 
     ``DataFrame`` :
         série temporal univariada ou multivariada,
-        quando solicitado mais de uma série.
+        quando solicitado mais de uma série (parâmetro ``multi=True``).
 
     ``list`` :
         lista com séries temporais univariadas,
-        quando solicitado mais de uma série.
-    '''
+        quando solicitado mais de uma série (parâmetro ``multi=False``).
+    """
     dfs = []
     for code in _codes(codes):
         urd = _get_url_and_payload(code.value, start, end, last)
-        res = requests.get(urd['url'], params=urd['payload'])
+        res = requests.get(urd["url"], params=urd["payload"])
         if res.status_code != 200:
-            raise Exception('Download error: code = {}'.format(code.value))
+            raise Exception("Download error: code = {}".format(code.value))
         df = pd.read_json(StringIO(res.text))
         df = _format_df(df, code, freq)
         dfs.append(df)
     if len(dfs) == 1:
         return dfs[0]
     else:
         if multi:
```

### Comparing `python-bcb-0.1.8/bcb/utils.py` & `python_bcb-0.1.9/bcb/utils.py`

 * *Files identical despite different names*

### Comparing `python-bcb-0.1.8/LICENSE` & `python_bcb-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `python-bcb-0.1.8/pyproject.toml` & `python_bcb-0.1.9/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 [tool.poetry]
 name = "python-bcb"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["wilsonfreitas <wilson.freitas@gmail.com>"]
 readme = "README.md"
 packages = [{include = "bcb"}]
 
 [tool.poetry.dependencies]
-python = "^3.8"
-httpx = "^0.23.0"
-lxml = "^4.9.1"
-pandas = "^1.4.4"
-requests = "^2.28.1"
+python = "^3.10"
+httpx = "^0.24.0"
+lxml = "^4.9.2"
+pandas = "^2.0.0"
+requests = "^2.31.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.1.3"
 
 [tool.poetry.group.docs.dependencies]
 Sphinx = "^5.1.1"
 pydata-sphinx-theme = "^0.10.1"
 matplotlib = "^3.5.3"
-ipython = "^8.5.0"
+ipython = "^8.14.0"
+furo = "^2022.6.21"
 
 
 [tool.poetry.group.dev.dependencies]
 pycodestyle = "^2.9.1"
 ipykernel = "^6.15.2"
 black = {version = "^22.8.0", allow-prereleases = true}
```

### Comparing `python-bcb-0.1.8/README.md` & `python_bcb-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `python-bcb-0.1.8/PKG-INFO` & `python_bcb-0.1.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: python-bcb
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: wilsonfreitas
 Author-email: wilson.freitas@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: httpx (>=0.23.0,<0.24.0)
-Requires-Dist: lxml (>=4.9.1,<5.0.0)
-Requires-Dist: pandas (>=1.4.4,<2.0.0)
-Requires-Dist: requests (>=2.28.1,<3.0.0)
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: httpx (>=0.24.0,<0.25.0)
+Requires-Dist: lxml (>=4.9.2,<5.0.0)
+Requires-Dist: pandas (>=2.0.0,<3.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # python-bcb
 
 **python-bcb** é uma interface em Python estruturada para obter informações
 da API de dados abertos do [Banco Central do Brasil](https://www.bcb.gov.br).
```


# Comparing `tmp/abin_sim-0.3.0.tar.gz` & `tmp/abin_sim-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abin_sim-0.3.0.tar", max compression
+gzip compressed data, was "abin_sim-1.0.0.tar", max compression
```

## Comparing `abin_sim-0.3.0.tar` & `abin_sim-1.0.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      260 2023-06-23 12:59:01.261627 abin_sim-0.3.0/LICENSE
--rw-r--r--   0        0        0     7485 2023-06-23 12:59:01.261627 abin_sim-0.3.0/README.md
--rw-r--r--   0        0        0       21 2023-06-23 12:59:01.261627 abin_sim-0.3.0/abin_sim/__init__.py
--rw-r--r--   0        0        0     6693 2023-06-23 12:59:01.261627 abin_sim-0.3.0/abin_sim/cli.py
--rw-r--r--   0        0        0      194 2023-06-23 12:59:01.261627 abin_sim-0.3.0/abin_sim/config.py
--rw-r--r--   0        0        0      783 2023-06-23 12:59:01.261627 abin_sim-0.3.0/abin_sim/core/file_manager.py
--rw-r--r--   0        0        0     3224 2023-06-23 12:59:01.261627 abin_sim-0.3.0/abin_sim/core/functions.py
--rw-r--r--   0        0        0     1190 2023-06-23 12:59:01.261627 abin_sim-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     8374 1970-01-01 00:00:00.000000 abin_sim-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      260 2023-06-26 17:15:54.510261 abin_sim-1.0.0/LICENSE
+-rw-r--r--   0        0        0     7972 2023-06-26 17:15:54.510261 abin_sim-1.0.0/README.md
+-rw-r--r--   0        0        0       21 2023-06-26 17:15:54.510261 abin_sim-1.0.0/abin_sim/__init__.py
+-rw-r--r--   0        0        0     7472 2023-06-26 17:15:54.510261 abin_sim-1.0.0/abin_sim/cli.py
+-rw-r--r--   0        0        0      194 2023-06-26 17:15:54.510261 abin_sim-1.0.0/abin_sim/config.py
+-rw-r--r--   0        0        0     1174 2023-06-26 17:15:54.510261 abin_sim-1.0.0/abin_sim/core/file_manager.py
+-rw-r--r--   0        0        0     4337 2023-06-26 17:15:54.510261 abin_sim-1.0.0/abin_sim/core/functions.py
+-rw-r--r--   0        0        0     1190 2023-06-26 17:15:54.510261 abin_sim-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     8861 1970-01-01 00:00:00.000000 abin_sim-1.0.0/PKG-INFO
```

### Comparing `abin_sim-0.3.0/README.md` & `abin_sim-1.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # ABIN
 [![CI](https://github.com/SIM-Rede/abin-sim/actions/workflows/pipeline.yaml/badge.svg)](https://github.com/SIM-Rede/abin-sim/actions/workflows/pipeline.yaml)
 [![PyPI version](https://badge.fury.io/py/abin-sim.svg)](https://badge.fury.io/py/abin-sim)
 
 ## Instalação
 
+Utilize o pipx para instalar o abin no seu computador.
 ```
 sudo apt install pipx
 pipx install abin_sim
 
 ```
 A versão da aplicação no README será atualizada sempre que um novo build rodar.
 
@@ -44,15 +45,27 @@
 * Clique em **Sign in**
 
 Após o login clique no boneco localizao no canto superior direito e, após, clique em **Copy Token**
 
 **Importante:** O Token é válido por 30 dias, portanto lembre de renová-lo.
 
 ## Funções
-    
+
+### DESCRITIVO
+    Uso: abin
+
+    Retorna uma breve explicação sobre a funcionalidade do CLI.
+    Traz exemplos de uso e link para projeto no GitHub
+
+### VERSION
+    Uso: abin --version
+
+### CONFIGURE
+    Uso: abin --configure
+   
 ### GET
     Usage: abin get [OPTIONS]                                                                                                                            
                                                                                                                                                       
     ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
     │ *  --app                  TEXT  Nome da aplicação que deseja recuperar os secrets. [default: None] [required]                                        │
     │ *  --env                  TEXT  Ambiente da aplicação que deseja recuperar (Envs possíveis: dev, qa, main). [default: None] [required]               │
     │ *  --proj                 TEXT  Projeto que deseja conectar para recuperar os secrets (Projs possíveis: simlabs, charrua) [default: None] [required] │
@@ -69,20 +82,21 @@
 ### UPDATE
     Usage: abin update [OPTIONS] 
                                                
     ╭─ Options─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
     │ *  --app         TEXT  Nome da aplicação que deseja recuperar os secrets. [default: None]  [required]                                        │
     │ *  --env         TEXT  Ambiente da aplicação que deseja recuperar (Envs possíveis: dev, qa, main). [default: None] [required]                │
     │ *  --proj        TEXT  Projeto que deseja conectar para recuperar os secrets (Projs possíveis: simlabs, charrua) [default: None] [required]  │
+    │    --secret      TEXT  Secret que será atualizada no Vault (Ex.: env, gcp.json, config.yaml ...) [default: env]                              │
     │ *  --file        TEXT  Arquivo com variárias de ambiente [default: None] [required]                                                          │
     │    --help              Show this message and exit.                                                                                           │
     ╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 
     For example:
-        abin update --app api-auth --env dev --proj simlabs --file .env
+        abin update --app api-auth --env dev --proj simlabs --file .env  (para atualizar outro secret use --secret NOME)
 
 ### COMPARE
     Usage: abin compare [OPTIONS]
 
     ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
     │ *  --app                  TEXT  Nome da aplicação que deseja recuperar os secrets. [default: None] [required]                                            │
     │ *  --env                  TEXT  Ambiente da aplicação que deseja recuperar (Envs possíveis: dev, qa, main). [default: None] [required]                   │
```

### Comparing `abin_sim-0.3.0/abin_sim/core/functions.py` & `abin_sim-1.0.0/abin_sim/core/functions.py`

 * *Files 19% similar despite different names*

```diff
@@ -75,30 +75,56 @@
 
     return json.dumps(contentDict)
 
 def update_secret(
     app: str,
     env: str,
     proj: str,
+    secret: str,
     token: str,
     vault_url: str,
     file: dict,
 ) -> dict:
     headers = {'X-Vault-Token': token}
-    json_file = Path('json_file.json')
-    json_file.touch()
-    json_file.write_text('{"data":'+file+'}')
-    payload = open('json_file.json', 'rb').read()
-    try:
-        ret = requests.request(
-            'POST', url=vault_url + f'/v1/{env}-{proj}/data/{app}/env', headers=headers, data=payload
-        )
-    except Exception as e:
-        return {'Status': e}
-    json_file.unlink()
+    match secret:
+        case 'env':
+            json_file = Path('json_file.json')
+            json_file.touch()
+            json_file.write_text('{"data":'+file+'}')
+            payload = open('json_file.json', 'rb').read()
+            try:
+                ret = requests.request(
+                    'POST', url=vault_url + f'/v1/{env}-{proj}/data/{app}/{secret}', headers=headers, data=payload
+                )
+            except Exception as e:
+                return {'Status': e}
+            json_file.unlink()
+        case _:            
+            with open(file, 'r') as f:
+                content = f.readlines()
+            converted = ''
+            # contentList = [x.strip().split('#')[0].split('=', 1) for x in content if '=' in x.split('#')[0]]
+            for line in content:
+                if converted == '':
+                    converted = f'{line}'.strip()+'\\n'
+                else:
+                    converted = f'{converted}{line}'.strip()+'\\n'
+
+            json_file = Path('json_file.json')
+            json_file.touch()
+            json_file.write_text('{"data": {"content": "'+converted+'"} }')
+
+            payload = open('json_file.json', 'rb').read()
+            try:
+                ret = requests.request(
+                    'POST', url=vault_url + f'/v1/{env}-{proj}/data/{app}/{secret}', headers=headers, data=payload
+                )
+            except Exception as e:
+                return {'Status': e}
+            json_file.unlink()
 
     if ret.status_code == 200:
         return {'Status': 'Success'}
     else:
         return {'Status': (ret.text)}
 
 def make_conf() -> dict:
```

### Comparing `abin_sim-0.3.0/pyproject.toml` & `abin_sim-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "abin-sim"
-version = "0.3.0"
+version = "1.0.0"
 description = "ABIN é um CLI para interagir com a API do Vault e auxiliar os Desenvolvedores nos projetos da SIMTech"
 license = "BeerWare"
 authors = ["Bonatto <andrebonatto@gmail.com>"]
 readme = "README.md"
 packages = [{include = "abin_sim"}]
 classifiers = [
     "Topic :: Utilities",
```

### Comparing `abin_sim-0.3.0/PKG-INFO` & `abin_sim-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abin-sim
-Version: 0.3.0
+Version: 1.0.0
 Summary: ABIN é um CLI para interagir com a API do Vault e auxiliar os Desenvolvedores nos projetos da SIMTech
 License: Beerware
 Author: Bonatto
 Author-email: andrebonatto@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -23,14 +23,15 @@
 
 # ABIN
 [![CI](https://github.com/SIM-Rede/abin-sim/actions/workflows/pipeline.yaml/badge.svg)](https://github.com/SIM-Rede/abin-sim/actions/workflows/pipeline.yaml)
 [![PyPI version](https://badge.fury.io/py/abin-sim.svg)](https://badge.fury.io/py/abin-sim)
 
 ## Instalação
 
+Utilize o pipx para instalar o abin no seu computador.
 ```
 sudo apt install pipx
 pipx install abin_sim
 
 ```
 A versão da aplicação no README será atualizada sempre que um novo build rodar.
 
@@ -67,15 +68,27 @@
 * Clique em **Sign in**
 
 Após o login clique no boneco localizao no canto superior direito e, após, clique em **Copy Token**
 
 **Importante:** O Token é válido por 30 dias, portanto lembre de renová-lo.
 
 ## Funções
-    
+
+### DESCRITIVO
+    Uso: abin
+
+    Retorna uma breve explicação sobre a funcionalidade do CLI.
+    Traz exemplos de uso e link para projeto no GitHub
+
+### VERSION
+    Uso: abin --version
+
+### CONFIGURE
+    Uso: abin --configure
+   
 ### GET
     Usage: abin get [OPTIONS]                                                                                                                            
                                                                                                                                                       
     ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
     │ *  --app                  TEXT  Nome da aplicação que deseja recuperar os secrets. [default: None] [required]                                        │
     │ *  --env                  TEXT  Ambiente da aplicação que deseja recuperar (Envs possíveis: dev, qa, main). [default: None] [required]               │
     │ *  --proj                 TEXT  Projeto que deseja conectar para recuperar os secrets (Projs possíveis: simlabs, charrua) [default: None] [required] │
@@ -92,20 +105,21 @@
 ### UPDATE
     Usage: abin update [OPTIONS] 
                                                
     ╭─ Options─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
     │ *  --app         TEXT  Nome da aplicação que deseja recuperar os secrets. [default: None]  [required]                                        │
     │ *  --env         TEXT  Ambiente da aplicação que deseja recuperar (Envs possíveis: dev, qa, main). [default: None] [required]                │
     │ *  --proj        TEXT  Projeto que deseja conectar para recuperar os secrets (Projs possíveis: simlabs, charrua) [default: None] [required]  │
+    │    --secret      TEXT  Secret que será atualizada no Vault (Ex.: env, gcp.json, config.yaml ...) [default: env]                              │
     │ *  --file        TEXT  Arquivo com variárias de ambiente [default: None] [required]                                                          │
     │    --help              Show this message and exit.                                                                                           │
     ╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 
     For example:
-        abin update --app api-auth --env dev --proj simlabs --file .env
+        abin update --app api-auth --env dev --proj simlabs --file .env  (para atualizar outro secret use --secret NOME)
 
 ### COMPARE
     Usage: abin compare [OPTIONS]
 
     ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
     │ *  --app                  TEXT  Nome da aplicação que deseja recuperar os secrets. [default: None] [required]                                            │
     │ *  --env                  TEXT  Ambiente da aplicação que deseja recuperar (Envs possíveis: dev, qa, main). [default: None] [required]                   │
```


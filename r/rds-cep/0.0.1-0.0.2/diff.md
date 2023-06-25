# Comparing `tmp/rds-cep-0.0.1.tar.gz` & `tmp/rds-cep-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rds-cep-0.0.1.tar", last modified: Thu Apr 27 01:12:03 2023, max compression
+gzip compressed data, was "rds-cep-0.0.2.tar", last modified: Sun Jun 25 23:10:53 2023, max compression
```

## Comparing `rds-cep-0.0.1.tar` & `rds-cep-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:12:03.179679 rds-cep-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 01:11:45.000000 rds-cep-0.0.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-27 01:12:03.179679 rds-cep-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-27 01:11:45.000000 rds-cep-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-27 01:11:45.000000 rds-cep-0.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:12:03.175679 rds-cep-0.0.1/rds_cep/
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-04-27 01:11:45.000000 rds-cep-0.0.1/rds_cep/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:12:03.179679 rds-cep-0.0.1/rds_cep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-27 01:12:03.000000 rds-cep-0.0.1/rds_cep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-27 01:12:03.000000 rds-cep-0.0.1/rds_cep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 01:12:03.000000 rds-cep-0.0.1/rds_cep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 01:12:03.000000 rds-cep-0.0.1/rds_cep.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-27 01:12:03.000000 rds-cep-0.0.1/rds_cep.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-27 01:12:03.179679 rds-cep-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-27 01:11:45.000000 rds-cep-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:10:53.664138 rds-cep-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 23:10:37.000000 rds-cep-0.0.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-25 23:10:53.664138 rds-cep-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-25 23:10:37.000000 rds-cep-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-25 23:10:37.000000 rds-cep-0.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:10:53.664138 rds-cep-0.0.2/rds_cep/
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-06-25 23:10:37.000000 rds-cep-0.0.2/rds_cep/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:10:53.664138 rds-cep-0.0.2/rds_cep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-25 23:10:53.000000 rds-cep-0.0.2/rds_cep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-25 23:10:53.000000 rds-cep-0.0.2/rds_cep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 23:10:53.000000 rds-cep-0.0.2/rds_cep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-25 23:10:53.000000 rds-cep-0.0.2/rds_cep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-25 23:10:53.000000 rds-cep-0.0.2/rds_cep.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-25 23:10:53.664138 rds-cep-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-06-25 23:10:37.000000 rds-cep-0.0.2/setup.py
```

### Comparing `rds-cep-0.0.1/PKG-INFO` & `rds-cep-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: rds-cep
-Version: 0.0.1
+Version: 0.0.2
 Summary: Framework para serviços do Rede de Dados em Saúde do LAIS
-Home-page: UNKNOWN
+Home-page: https://github.com/lais-huol/rds-cep-python
 Author: Kelson da Costa Medeiros
 Author-email: kelson.medeiros@lais.huol.ufrn.br
 License: UNKNOWN
+Download-URL: https://github.com/lais-huol/rds-cep-python/tags
+Description: É uma biblioteca pública em Python que condensa um conjunto de boas práticas para o desenvolvimento das aplicações que compõem a Rede da Dados em Saúde (RDS) RDS do Laboratório de Inovação Tecnológica em Saúde (LAIS) e dos parceiros que contam com o LAIS para fazer suas próprias RDS, a exemplo RDS-RN e RDS-ES.
 Keywords: rds,cache,config,helper,searchengine
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.9
-License-File: LICENSE.md
-
-É uma biblioteca pública em Python que condensa um conjunto de boas práticas para o desenvolvimento das aplicações que compõem a Rede da Dados em Saúde (RDS) RDS do Laboratório de Inovação Tecnológica em Saúde (LAIS) e dos parceiros que contam com o LAIS para fazer suas próprias RDS, a exemplo RDS-RN e RDS-ES.
-
+Requires-Python: >=3.8
```

### Comparing `rds-cep-0.0.1/README.md` & `rds-cep-0.0.2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -11,22 +11,23 @@
 ## Como desenvolver
 
 Crie uma nova branch, clone o código, crie uma venv para desenvolvimento, instale os pacotes de desenvolvimento, teste o código, commit as mudanças na branch, envie para o repositório, solicite um Pull Request.
 
 ```bash
 mkvirtualenv rds-core
 pip install -r requirements-dev.txt
+pre-commit install
+pre-commit clean
 ```
 
 Caso você deseje alterar o código do rds-core e testar como reflete aqui
 
 ```bash
 # Prepare
 pip install -e ../rds-core
-
 ```
 
 Teste as alterações
 
 ```bash
 # Teste o software conforme os padrões de arquitetura
 pre-commit run --all-files -v
```

### Comparing `rds-cep-0.0.1/pyproject.toml` & `rds-cep-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rds-cep-0.0.1/rds_cep/__init__.py` & `rds-cep-0.0.2/rds_cep/__init__.py`

 * *Files identical despite different names*

### Comparing `rds-cep-0.0.1/rds_cep.egg-info/PKG-INFO` & `rds-cep-0.0.2/rds_cep.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: rds-cep
-Version: 0.0.1
+Version: 0.0.2
 Summary: Framework para serviços do Rede de Dados em Saúde do LAIS
-Home-page: UNKNOWN
+Home-page: https://github.com/lais-huol/rds-cep-python
 Author: Kelson da Costa Medeiros
 Author-email: kelson.medeiros@lais.huol.ufrn.br
 License: UNKNOWN
+Download-URL: https://github.com/lais-huol/rds-cep-python/tags
+Description: É uma biblioteca pública em Python que condensa um conjunto de boas práticas para o desenvolvimento das aplicações que compõem a Rede da Dados em Saúde (RDS) RDS do Laboratório de Inovação Tecnológica em Saúde (LAIS) e dos parceiros que contam com o LAIS para fazer suas próprias RDS, a exemplo RDS-RN e RDS-ES.
 Keywords: rds,cache,config,helper,searchengine
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.9
-License-File: LICENSE.md
-
-É uma biblioteca pública em Python que condensa um conjunto de boas práticas para o desenvolvimento das aplicações que compõem a Rede da Dados em Saúde (RDS) RDS do Laboratório de Inovação Tecnológica em Saúde (LAIS) e dos parceiros que contam com o LAIS para fazer suas próprias RDS, a exemplo RDS-RN e RDS-ES.
-
+Requires-Python: >=3.8
```

### Comparing `rds-cep-0.0.1/setup.py` & `rds-cep-0.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,17 @@
         subfolders.extend(fast_scandir(dirname))
     return subfolders
 
 
 def package_data_dirs(root, data_dirs):
     data_dirs_path = [x + "/*" for x in data_dirs]
     for data_dir in data_dirs:
-        data_dirs_path += [x.replace(f"{root}/", "") + "/*" for x in fast_scandir(f"{root}/{data_dir}")]
+        data_dirs_path += [
+            x.replace(f"{root}/", "") + "/*" for x in fast_scandir(f"{root}/{data_dir}")
+        ]
 
     return {root: data_dirs_path}
 
 
 requirements = [
     # config
     "rds-core>=0.0.16",
@@ -25,37 +27,40 @@
 
 with open("requirements.txt", "w") as file1:
     for requirement in requirements:
         file1.write(f"{requirement}\n")
 
 setup(
     name="rds-cep",
-    version="0.0.1",
+    version="0.0.2",
     description="Framework para serviços do Rede de Dados em Saúde do LAIS",
     long_description="É uma biblioteca pública em Python que condensa um conjunto de boas práticas para o"
     " desenvolvimento das aplicações que compõem a Rede da Dados em Saúde (RDS) RDS do Laboratório de"
     " Inovação Tecnológica em Saúde (LAIS) e dos parceiros que contam com o LAIS para fazer suas próprias"
     " RDS, a exemplo RDS-RN e RDS-ES.",
     author="Kelson da Costa Medeiros",
     author_email="kelson.medeiros@lais.huol.ufrn.br",
     keywords=["rds", "cache", "config", "helper", "searchengine"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
+        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Internet :: WWW/HTTP :: Indexing/Search",
         "Topic :: Software Development :: Libraries",
     ],
-    python_requires=">=3.9",
+    python_requires=">=3.8",
     install_requires=requirements,
     packages=[
         "rds_cep",
     ],
     package_dir={"rds_cep": "rds_cep"},
     package_data=package_data_dirs("rds_cep", []),
+    download_url="https://github.com/lais-huol/rds-cep-python/tags",
+    url="https://github.com/lais-huol/rds-cep-python",
 )
```


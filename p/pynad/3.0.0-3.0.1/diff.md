# Comparing `tmp/pynad-3.0.0.tar.gz` & `tmp/pynad-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynad-3.0.0.tar", last modified: Sun Jun 25 14:53:22 2023, max compression
+gzip compressed data, was "pynad-3.0.1.tar", last modified: Mon Jun 26 13:26:07 2023, max compression
```

## Comparing `pynad-3.0.0.tar` & `pynad-3.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2023-06-25 14:53:22.956679 pynad-3.0.0/
--rw-r--r--   0 rafael    (1000) rafael    (1000)    35152 2020-04-21 13:59:39.000000 pynad-3.0.0/LICENSE
--rw-r--r--   0 rafael    (1000) rafael    (1000)       22 2023-06-25 13:22:31.000000 pynad-3.0.0/MANIFEST.in
--rw-rw-r--   0 rafael    (1000) rafael    (1000)     4057 2023-06-25 14:53:22.956679 pynad-3.0.0/PKG-INFO
--rw-r--r--   0 rafael    (1000) rafael    (1000)     3636 2023-06-25 14:51:28.000000 pynad-3.0.0/README.rst
--rw-r--r--   0 rafael    (1000) rafael    (1000)      803 2023-06-25 13:21:18.000000 pynad-3.0.0/changelog.txt
-drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2023-06-25 14:53:22.956679 pynad-3.0.0/pynad/
--rw-r--r--   0 rafael    (1000) rafael    (1000)      103 2023-06-25 14:09:36.000000 pynad-3.0.0/pynad/__init__.py
--rw-r--r--   0 rafael    (1000) rafael    (1000)     2542 2023-06-13 23:56:24.000000 pynad-3.0.0/pynad/auxiliares.py
--rw-r--r--   0 rafael    (1000) rafael    (1000)    11436 2023-06-25 14:11:15.000000 pynad-3.0.0/pynad/converter.py
--rw-r--r--   0 rafael    (1000) rafael    (1000)    10210 2023-06-25 14:11:15.000000 pynad-3.0.0/pynad/copia_local.py
--rw-r--r--   0 rafael    (1000) rafael    (1000)    12078 2023-06-25 14:11:15.000000 pynad-3.0.0/pynad/metadados.py
--rw-r--r--   0 rafael    (1000) rafael    (1000)    20460 2023-06-25 14:11:15.000000 pynad-3.0.0/pynad/paineis.py
--rw-rw-r--   0 rafael    (1000) rafael    (1000)    24138 2023-06-25 14:11:15.000000 pynad-3.0.0/pynad/paineis_id.py
--rw-r--r--   0 rafael    (1000) rafael    (1000)    10619 2023-06-25 14:47:47.000000 pynad-3.0.0/pynad/pynad.py
-drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2023-06-25 14:53:22.956679 pynad-3.0.0/pynad.egg-info/
--rw-rw-r--   0 rafael    (1000) rafael    (1000)     4057 2023-06-25 14:53:22.000000 pynad-3.0.0/pynad.egg-info/PKG-INFO
--rw-rw-r--   0 rafael    (1000) rafael    (1000)      394 2023-06-25 14:53:22.000000 pynad-3.0.0/pynad.egg-info/SOURCES.txt
--rw-rw-r--   0 rafael    (1000) rafael    (1000)        1 2023-06-25 14:53:22.000000 pynad-3.0.0/pynad.egg-info/dependency_links.txt
--rw-rw-r--   0 rafael    (1000) rafael    (1000)       47 2023-06-25 14:53:22.000000 pynad-3.0.0/pynad.egg-info/entry_points.txt
--rw-rw-r--   0 rafael    (1000) rafael    (1000)       13 2023-06-25 14:53:22.000000 pynad-3.0.0/pynad.egg-info/requires.txt
--rw-rw-r--   0 rafael    (1000) rafael    (1000)        6 2023-06-25 14:53:22.000000 pynad-3.0.0/pynad.egg-info/top_level.txt
--rw-r--r--   0 rafael    (1000) rafael    (1000)      104 2021-10-14 15:54:16.000000 pynad-3.0.0/pyproject.toml
--rw-r--r--   0 rafael    (1000) rafael    (1000)      617 2023-06-25 14:53:22.956679 pynad-3.0.0/setup.cfg
+drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2023-06-26 13:26:07.562101 pynad-3.0.1/
+-rw-r--r--   0 rafael    (1000) rafael    (1000)    35152 2020-04-21 13:59:39.000000 pynad-3.0.1/LICENSE
+-rw-r--r--   0 rafael    (1000) rafael    (1000)       22 2023-06-25 13:22:31.000000 pynad-3.0.1/MANIFEST.in
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)     4057 2023-06-26 13:26:07.562101 pynad-3.0.1/PKG-INFO
+-rw-r--r--   0 rafael    (1000) rafael    (1000)     3636 2023-06-25 14:51:28.000000 pynad-3.0.1/README.rst
+-rw-r--r--   0 rafael    (1000) rafael    (1000)      854 2023-06-26 13:25:14.000000 pynad-3.0.1/changelog.txt
+drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2023-06-26 13:26:07.562101 pynad-3.0.1/pynad/
+-rw-r--r--   0 rafael    (1000) rafael    (1000)      103 2023-06-25 14:09:36.000000 pynad-3.0.1/pynad/__init__.py
+-rw-r--r--   0 rafael    (1000) rafael    (1000)     2542 2023-06-13 23:56:24.000000 pynad-3.0.1/pynad/auxiliares.py
+-rw-r--r--   0 rafael    (1000) rafael    (1000)    11436 2023-06-25 14:11:15.000000 pynad-3.0.1/pynad/converter.py
+-rw-r--r--   0 rafael    (1000) rafael    (1000)    10210 2023-06-25 14:11:15.000000 pynad-3.0.1/pynad/copia_local.py
+-rw-r--r--   0 rafael    (1000) rafael    (1000)    12078 2023-06-25 14:11:15.000000 pynad-3.0.1/pynad/metadados.py
+-rw-r--r--   0 rafael    (1000) rafael    (1000)    20460 2023-06-25 14:11:15.000000 pynad-3.0.1/pynad/paineis.py
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)    24138 2023-06-25 14:11:15.000000 pynad-3.0.1/pynad/paineis_id.py
+-rw-r--r--   0 rafael    (1000) rafael    (1000)    10640 2023-06-26 13:23:30.000000 pynad-3.0.1/pynad/pynad.py
+drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2023-06-26 13:26:07.562101 pynad-3.0.1/pynad.egg-info/
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)     4057 2023-06-26 13:26:07.000000 pynad-3.0.1/pynad.egg-info/PKG-INFO
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)      394 2023-06-26 13:26:07.000000 pynad-3.0.1/pynad.egg-info/SOURCES.txt
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)        1 2023-06-26 13:26:07.000000 pynad-3.0.1/pynad.egg-info/dependency_links.txt
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)       47 2023-06-26 13:26:07.000000 pynad-3.0.1/pynad.egg-info/entry_points.txt
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)       13 2023-06-26 13:26:07.000000 pynad-3.0.1/pynad.egg-info/requires.txt
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)        6 2023-06-26 13:26:07.000000 pynad-3.0.1/pynad.egg-info/top_level.txt
+-rw-r--r--   0 rafael    (1000) rafael    (1000)      104 2021-10-14 15:54:16.000000 pynad-3.0.1/pyproject.toml
+-rw-r--r--   0 rafael    (1000) rafael    (1000)      617 2023-06-26 13:26:07.562101 pynad-3.0.1/setup.cfg
```

### Comparing `pynad-3.0.0/LICENSE` & `pynad-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pynad-3.0.0/PKG-INFO` & `pynad-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynad
-Version: 3.0.0
+Version: 3.0.1
 Summary: An application to manage Pnadc microdata and setup its panels
 Author: Rafael Guerreiro Osorio
 Author-email: rafael.osorio@ipea.gov.br
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `pynad-3.0.0/README.rst` & `pynad-3.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `pynad-3.0.0/changelog.txt` & `pynad-3.0.1/changelog.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 Pynad
 
+v3.0.1 - Pequeno ajuste para funcionar em Windows.
 v3.0.0 - Volta para interface com linha de comando; tira seleção de arquivos; operações com pyarrow e arquivos parquet; somente arquivo de painel deitado
          e sem pesos BS; mais rápido
 v2.2.0 - Separação dos pesos de bootstrap em arquivos por domicílio; correção do comportamento de seleção de arquivos na árvore - exibe sempre os arquivos remotos, arquivos que existem na cópia local mas não no IBGE não são exibidos
 v2.1.0 - Resolvido problema do registro da seleção de arquivos para garantir que novos arquivos estejam sempre marcados para download
 v2.0.14 - Resolvidos problemas em arquivos de configuração do pacote para download com pip
 v2.0.0 - Primeira versão com interface gráfica
 v1.x.x - Versões inciais sem interface gráfica (quase todas tem algum bug)
```

### Comparing `pynad-3.0.0/pynad/auxiliares.py` & `pynad-3.0.1/pynad/auxiliares.py`

 * *Files identical despite different names*

### Comparing `pynad-3.0.0/pynad/converter.py` & `pynad-3.0.1/pynad/converter.py`

 * *Files identical despite different names*

### Comparing `pynad-3.0.0/pynad/copia_local.py` & `pynad-3.0.1/pynad/copia_local.py`

 * *Files identical despite different names*

### Comparing `pynad-3.0.0/pynad/metadados.py` & `pynad-3.0.1/pynad/metadados.py`

 * *Files identical despite different names*

### Comparing `pynad-3.0.0/pynad/paineis.py` & `pynad-3.0.1/pynad/paineis.py`

 * *Files identical despite different names*

### Comparing `pynad-3.0.0/pynad/paineis_id.py` & `pynad-3.0.1/pynad/paineis_id.py`

 * *Files identical despite different names*

### Comparing `pynad-3.0.0/pynad/pynad.py` & `pynad-3.0.1/pynad/pynad.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,23 +24,14 @@
 from .copia_local import register, verify, sync
 from .copia_local import COPIA_LOCAL, IDFILE, LSFILE, MPFILE
 from .converter import sync_microdados, MICRO
 from .metadados import generate, META
 from .paineis import sync_paineis, PAINEIS
 
 
-# ativar terminal escape sequences no Windows
-if system() == 'Windows':
-    from ctypes import windll
-    windll.kernel32.SetConsoleMode(windll.kernel32.GetStdHandle(-11), 7)
-
-# dimensiona o terminal
-print(f'\033[8;24;{TCOLS}t', end='')
-
-
 def cli_copia_local(folder, data):
     """Info da cópia local."""
     # COPIA LOCAL
     print(COPIA_B + COPIA_F, end='')
     for _linha in range(4):
         print(' ' * TCOLS, end='')
     print('\n\033[4A\033[K', end='')
@@ -120,14 +111,20 @@
         resp = input(f'{UPCLR}Digite a opção {ARROW} ').lower()
     cli_main()
     return menu[resp][1](folder)
 
 
 def main_script():
     """Inicia quando roda como script."""
+    # ativar terminal escape sequences no Windows
+    if system() == 'Windows':
+        from ctypes import windll
+        windll.kernel32.SetConsoleMode(windll.kernel32.GetStdHandle(-11), 7)
+    # dimensiona o terminal
+    print(f'\033[8;24;{TCOLS}t', end='')
     folder = data = ''
     loop = True
     while loop:
         loop, folder, data = main(folder, data)
 
 
 def menu_ajuda(folder):
```

### Comparing `pynad-3.0.0/pynad.egg-info/PKG-INFO` & `pynad-3.0.1/pynad.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynad
-Version: 3.0.0
+Version: 3.0.1
 Summary: An application to manage Pnadc microdata and setup its panels
 Author: Rafael Guerreiro Osorio
 Author-email: rafael.osorio@ipea.gov.br
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `pynad-3.0.0/setup.cfg` & `pynad-3.0.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pynad
-version = 3.0.0
+version = 3.0.1
 author = Rafael Guerreiro Osorio
 author_email = rafael.osorio@ipea.gov.br
 description = An application to manage Pnadc microdata and setup its panels
 long_description = file: README.rst
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```


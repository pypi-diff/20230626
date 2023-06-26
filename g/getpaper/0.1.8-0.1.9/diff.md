# Comparing `tmp/getpaper-0.1.8.tar.gz` & `tmp/getpaper-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getpaper-0.1.8.tar", last modified: Sat Jun 24 00:24:34 2023, max compression
+gzip compressed data, was "getpaper-0.1.9.tar", last modified: Mon Jun 26 00:56:42 2023, max compression
```

## Comparing `getpaper-0.1.8.tar` & `getpaper-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-24 00:24:34.633205 getpaper-0.1.8/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1072 2023-06-20 19:48:29.000000 getpaper-0.1.8/LICENSE
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     4491 2023-06-24 00:24:34.633205 getpaper-0.1.8/PKG-INFO
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     3876 2023-06-23 23:00:00.000000 getpaper-0.1.8/README.md
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-24 00:24:34.633205 getpaper-0.1.8/getpaper/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 20:08:46.000000 getpaper-0.1.8/getpaper/__init__.py
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     7695 2023-06-23 22:48:27.000000 getpaper-0.1.8/getpaper/download.py
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     6249 2023-06-23 22:51:14.000000 getpaper-0.1.8/getpaper/index.py
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)    11749 2023-06-24 00:24:03.000000 getpaper-0.1.8/getpaper/parse.py
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1069 2023-06-21 21:08:34.000000 getpaper-0.1.8/getpaper/splitter.py
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-24 00:24:34.633205 getpaper-0.1.8/getpaper.egg-info/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     4491 2023-06-24 00:24:34.000000 getpaper-0.1.8/getpaper.egg-info/PKG-INFO
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      319 2023-06-24 00:24:34.000000 getpaper-0.1.8/getpaper.egg-info/SOURCES.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        1 2023-06-24 00:24:34.000000 getpaper-0.1.8/getpaper.egg-info/dependency_links.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      105 2023-06-24 00:24:34.000000 getpaper-0.1.8/getpaper.egg-info/entry_points.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      201 2023-06-24 00:24:34.000000 getpaper-0.1.8/getpaper.egg-info/requires.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        9 2023-06-24 00:24:34.000000 getpaper-0.1.8/getpaper.egg-info/top_level.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       38 2023-06-24 00:24:34.633205 getpaper-0.1.8/setup.cfg
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     1586 2023-06-24 00:24:17.000000 getpaper-0.1.8/setup.py
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-26 00:56:42.271819 getpaper-0.1.9/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1072 2023-06-20 19:48:29.000000 getpaper-0.1.9/LICENSE
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     4482 2023-06-26 00:56:42.271819 getpaper-0.1.9/PKG-INFO
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     3867 2023-06-26 00:46:48.000000 getpaper-0.1.9/README.md
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-26 00:56:42.271819 getpaper-0.1.9/getpaper/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 20:08:46.000000 getpaper-0.1.9/getpaper/__init__.py
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     5288 2023-06-26 00:35:31.000000 getpaper-0.1.9/getpaper/clean.py
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      425 2023-06-25 23:33:14.000000 getpaper-0.1.9/getpaper/config.py
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     7695 2023-06-25 18:19:53.000000 getpaper-0.1.9/getpaper/download.py
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     6368 2023-06-26 00:56:26.000000 getpaper-0.1.9/getpaper/index.py
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)    10469 2023-06-26 00:44:45.000000 getpaper-0.1.9/getpaper/parse.py
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     3008 2023-06-26 00:25:48.000000 getpaper-0.1.9/getpaper/splitting.py
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-26 00:56:42.271819 getpaper-0.1.9/getpaper.egg-info/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     4482 2023-06-26 00:56:42.000000 getpaper-0.1.9/getpaper.egg-info/PKG-INFO
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      357 2023-06-26 00:56:42.000000 getpaper-0.1.9/getpaper.egg-info/SOURCES.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        1 2023-06-26 00:56:42.000000 getpaper-0.1.9/getpaper.egg-info/dependency_links.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      105 2023-06-26 00:56:42.000000 getpaper-0.1.9/getpaper.egg-info/entry_points.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      201 2023-06-26 00:56:42.000000 getpaper-0.1.9/getpaper.egg-info/requires.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        9 2023-06-26 00:56:42.000000 getpaper-0.1.9/getpaper.egg-info/top_level.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       38 2023-06-26 00:56:42.271819 getpaper-0.1.9/setup.cfg
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     1586 2023-06-26 00:40:32.000000 getpaper-0.1.9/setup.py
```

### Comparing `getpaper-0.1.8/LICENSE` & `getpaper-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `getpaper-0.1.8/PKG-INFO` & `getpaper-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getpaper
-Version: 0.1.8
+Version: 0.1.9
 Summary: getpaper - papers download made easy!
 Author: antonkulaga (Anton Kulaga)
 Author-email: <antonkulaga@gmail.com>
 Keywords: python,utils,files,papers,download
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
@@ -73,15 +73,15 @@
 download download_papers --dois "10.3390/ijms22031073" --dois "10.1038/s41597-020-00710-z" --dois "wrong" --folder "data/output/test/papers" --threads 5
 ```
 
 ## Parsing the papers
 
 You can parse the downloaded papers with the unstructured library. For example if the papers are in the folder test, you can run:
 ```bash
-getpaper/parse.py parse_folder --folder data/output/test/papers --threads 5
+getpaper/parse.py parse_folder --folder data/output/test/papers --cores 5
 ```
 You can also parse papers on a per-file basis, for example:
 ```bash
 getpaper/parse.py parse_paper --paper data/output/test/papers/10.3390/ijms22031073.pdf
 ```
 
 ## Count tokens
@@ -94,15 +94,15 @@
 
 ## Indexing papers
 
 We also provide features to index the papers with openai or lambda embeddings and save them in chromadb vector store.
 For openai embeddings to work you have to create .env file and specify your openai key there, see .env.template as example
 For example if you have your papers inside data/output/test/papers folder, and you want to make a ChromaDB index at data/output/test/index you can do it by:
 ```bash
-python getpaper/index.py index_papers --papers data/output/test/papers --folder data/output/test/index --collection mypapers --chunk_size 6000
+getpaper/index.py index_papers --papers data/output/test/papers --folder data/output/test/index --collection mypapers --chunk_size 6000
 ```
 
 # Examples
 
 You can run examples.py to see usage examples
 
 # Additional requirements
```

### Comparing `getpaper-0.1.8/README.md` & `getpaper-0.1.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 download download_papers --dois "10.3390/ijms22031073" --dois "10.1038/s41597-020-00710-z" --dois "wrong" --folder "data/output/test/papers" --threads 5
 ```
 
 ## Parsing the papers
 
 You can parse the downloaded papers with the unstructured library. For example if the papers are in the folder test, you can run:
 ```bash
-getpaper/parse.py parse_folder --folder data/output/test/papers --threads 5
+getpaper/parse.py parse_folder --folder data/output/test/papers --cores 5
 ```
 You can also parse papers on a per-file basis, for example:
 ```bash
 getpaper/parse.py parse_paper --paper data/output/test/papers/10.3390/ijms22031073.pdf
 ```
 
 ## Count tokens
@@ -76,15 +76,15 @@
 
 ## Indexing papers
 
 We also provide features to index the papers with openai or lambda embeddings and save them in chromadb vector store.
 For openai embeddings to work you have to create .env file and specify your openai key there, see .env.template as example
 For example if you have your papers inside data/output/test/papers folder, and you want to make a ChromaDB index at data/output/test/index you can do it by:
 ```bash
-python getpaper/index.py index_papers --papers data/output/test/papers --folder data/output/test/index --collection mypapers --chunk_size 6000
+getpaper/index.py index_papers --papers data/output/test/papers --folder data/output/test/index --collection mypapers --chunk_size 6000
 ```
 
 # Examples
 
 You can run examples.py to see usage examples
 
 # Additional requirements
```

### Comparing `getpaper-0.1.8/getpaper/download.py` & `getpaper-0.1.9/getpaper/download.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     :param doi:
     :param destination: where to put the results
     :param skip_if_exist:
     :param name:
     :return: Try monad with the result
     """
     doi_url = f"https://doi.org/{doi}"
-    paper = (destination / f"{doi}.pdf").absolute().resolve() if name is None else (destination / f"{name.replace(',pdf', '')}.pdf").absolute().resolve()
+    paper = (destination / f"{doi}.pdf").absolute().resolve() if name is None else (destination / f"{name.replace('.pdf', '')}.pdf").absolute().resolve()
     if skip_if_exist and paper.exists():
         print(f"Paper {paper} for {doi} already exists!")
         return Try.of(lambda: paper)
     return Try.of(lambda: scihub_download(doi_url, paper_type="doi", out=str(paper))).map(lambda _: paper)
 
 def download_pubmed(pubmed: str, destination: Path, skip_if_exist: bool = True, name: Optional[str] = None):
     """
```

### Comparing `getpaper-0.1.8/getpaper/index.py` & `getpaper-0.1.9/getpaper/index.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,22 @@
 #!/usr/bin/env python3
 
 from pathlib import Path
-import dotenv
-from dotenv import load_dotenv
-import os
+
 import click
 from click import Context
-from langchain.document_loaders import DataFrameLoader
 from langchain.embeddings import OpenAIEmbeddings, LlamaCppEmbeddings, VertexAIEmbeddings
 from langchain.embeddings.base import Embeddings
 from langchain.schema import Document
 from langchain.text_splitter import TextSplitter
 from langchain.vectorstores import Chroma
 from pycomfort.files import *
 
-from getpaper.parse import papers_to_documents
-from getpaper.splitter import RecursiveSplitterWithSource
-
-
-def load_environment_keys(debug: bool = True):
-    e = dotenv.find_dotenv()
-    if debug:
-        print(f"environment found at {e}")
-    has_env: bool = load_dotenv(e, verbose=True, override=True)
-    if not has_env:
-        print("Did not found environment file, using system OpenAI key (if exists)")
-    openai_key = os.getenv('OPENAI_API_KEY')
-    return openai_key
+#from getpaper.config import load_environment_keys
+from getpaper.splitting import OpenAISplitter, SourceTextSplitter, papers_to_documents
 
 
 def resolve_embeddings(embeddings_name: str) -> Embeddings:
     if embeddings_name == "openai":
         return OpenAIEmbeddings()
     elif embeddings_name == "lambda":
         return LlamaCppEmbeddings()
@@ -69,25 +55,26 @@
     db.add_texts(texts=texts, metadatas=metadatas, ids=ids)
     return db
 
 
 def write_db(persist_directory: Path,
              collection_name: str,
              documents: list[Document],
-             chunk_size: int = 6000,
+             splitter: TextSplitter,
              debug: bool = False,
              id_field: Optional[str] = None,
              embeddings: Optional[Embeddings] = None):
     """
     Writes the provided documents to a database.
 
     Args:
         persist_directory (Path): The directory where the database should be saved.
         collection_name (str): The name of the collection in the database.
         documents (list[Document]): The list of documents to be added to the database.
+        splitter: TextSplitter
         chunk_size (int): The size of the text chunks to split the documents into. Default is 6000.
         debug (bool): If True, print debug information. Default is False.
         id_field (Optional[str]): The name of the field to use as the document ID. Default is None.
         embeddings (Optional[Embeddings]): The embeddings to use. If not provided, defaults to OpenAIEmbeddings.
 
     Returns:
         Path: The directory where the database was saved.
@@ -100,17 +87,14 @@
     # If no embeddings were provided, default to OpenAIEmbeddings
     if embeddings is None:
         embeddings = OpenAIEmbeddings()
 
     # Create a Chroma database with the specified collection name and embeddings, and save it in the specified directory
     db = Chroma(collection_name=collection_name, persist_directory=str(where), embedding_function=embeddings)
 
-    # Create a RecursiveSplitterWithSource to split the documents into chunks of the specified size
-    splitter = RecursiveSplitterWithSource(chunk_size=chunk_size)
-
     # Add the documents to the database
     db_updated = db_with_documents(db, documents, splitter, debug, id_field)
 
     # Persist the changes to the database
     db_updated.persist()
 
     # Return the directory where the database was saved
@@ -122,33 +106,44 @@
 def app(ctx: Context):
     # if ctx.invoked_subcommand is None:
     #    click.echo('Running the default command...')
     #    test_index()
     pass
 
 
-def index_papers(papers_folder: Path, index: Path, collection: str, chunk_size: int, embeddings: str) -> Path:
+def index_papers(papers_folder: Path, index: Path, collection: str, splitter: SourceTextSplitter, embeddings: str) -> Path:
     index.mkdir(exist_ok=True)
     openai_key = load_environment_keys()
     embeddings_function = resolve_embeddings(embeddings)
     print(f"embeddings are {embeddings}")
-    where = index / f"{embeddings}_{chunk_size}_chunk"
+    where = index / f"{embeddings}_{splitter.chunk_size}_chunk"
     where.mkdir(exist_ok=True, parents=True)
     print(f"writing index of papers to {where}")
     documents = papers_to_documents(papers_folder)
-    return write_db(where, collection, documents, chunk_size, embeddings=embeddings_function)
+    return write_db(where, collection, documents, splitter, embeddings=embeddings_function)
 
 
 @app.command("index_papers")
 @click.option('--papers', type=click.Path(exists=True), help="papers folder to index")
 @click.option('--folder', type=click.Path(), help="folder to put chroma indexes to")
 @click.option('--collection', default='papers', help='papers collection name')
-@click.option('--chunk_size', type=click.INT, default=6000, help='size of the chunk for splitting')
+@click.option('--splitter', type=click.Choice(["openai", "recursive"]), default="openai", help='which splitter to choose for the text splitting')
+@click.option('--chunk_size', type=click.INT, default=3000, help='size of the chunk for splitting (characters for recursive spliiter and tokens for openai one)')
 @click.option('--embeddings', type=click.Choice(["openai", "lambda", "vertexai"]), default="openai",
               help='size of the chunk for splitting')
-def index_papers_command(papers: str, folder: str, collection: str, chunk_size: int, embeddings: str) -> Path:
+def index_papers_command(papers: str, folder: str, collection: str, splitter_name: str, chunk_size: int, embeddings: str) -> Path:
     index = Path(folder)
     papers_folder = Path(papers)
-    return index_papers(papers_folder, index, collection, chunk_size, embeddings)
+
+    if splitter_name == "recursive":
+        # Create a RecursiveSplitterWithSource to split the documents into chunks of the specified size
+        splitter = SourceTextSplitter(chunk_size=chunk_size)
+    elif splitter_name == "recursive":
+        splitter = OpenAISplitter(tokens=chunk_size)
+    else:
+        print(f"{splitter_name} is not supported, using openai tiktoken based splitter instead")
+        splitter = OpenAISplitter(tokens=chunk_size)
+    return index_papers(papers_folder, index, collection, splitter, embeddings)
+
 
 if __name__ == '__main__':
     app()
```

### Comparing `getpaper-0.1.8/getpaper/parse.py` & `getpaper-0.1.9/getpaper/parse.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 #!/usr/bin/env python3
 
+from functools import partial
+from multiprocessing import Pool, cpu_count
 from pathlib import Path
-from typing import Optional, List, Dict
+from typing import Optional, List
 
 import click
 import pynction.monads.try_monad
 import tiktoken
 from click import Context
 from functional import seq
 from langchain.document_loaders import UnstructuredPDFLoader
 from langchain.schema import Document
 from pycomfort.files import traverse
-from multiprocessing import Pool, cpu_count
-from functools import partial
-from deprecated import deprecated
-import asyncio
-from concurrent.futures import ThreadPoolExecutor
-
 from pynction import Try
 
 
 def num_tokens_openai(string: str, model: str, price_per_1k: float = 0.0001) -> (int, float):
     """Returns the number of tokens for a model"""
     encoding = tiktoken.encoding_for_model(model)
     n_tokens = len(encoding.encode(string))
@@ -35,19 +31,23 @@
 openai_prices_per_thousand = {
     "gpt-4-32k": None, #32,768 tokens
     "gpt-4": 0.03, #8,192 tokens
     "gpt-3.5-turbo-16k": None, #16,384 tokens,
     "gpt-3.5-turbo": None #4,096 tokens
 }
 
+def clean_text(text: str) -> str:
+    from unstructured.cleaners.core import clean, group_broken_paragraphs, replace_unicode_quotes
+    return clean(group_broken_paragraphs(replace_unicode_quotes(text)))
+
 
 def parse_paper(paper: Path, folder: Optional[Path] = None,
                 mode: str = "single", strategy: str = "auto",
                 pdf_infer_table_structure: bool = True,
-                include_page_breaks: bool = False, recreate_parent: bool = False
+                include_page_breaks: bool = False, recreate_parent: bool = False, cleaning: bool = True
                 ) -> List[Path]:
     """
     Parses the paper using Unstructured paper parser
     :param paper:
     :param folder:
     :param mode: can be single or paged
     :param recreate_parent: can be useful if we grouped papers by subfolders (for example for dois)
@@ -56,41 +56,45 @@
     bin_file = open(str(paper), "rb")
     loader = UnstructuredPDFLoader(file_path=None, file = bin_file,  mode=mode,
                                    pdf_infer_table_structure=pdf_infer_table_structure,
                                    strategy = strategy, include_page_breaks = include_page_breaks)
     where = paper.parent if folder is None else folder / paper.parent.name if recreate_parent else folder
     where.mkdir(parents=True, exist_ok=True)
     docs: list[Document] = loader.load()
+
+
     if len(docs) ==1:
         name = f"{paper.stem}.txt"
         f = where / name
         print(f"writing {f}")
-        f.write_text(docs[0].page_content)
+        text = clean_text(docs[0].page_content) if cleaning else docs[0].page_content
+        f.write_text(text)
         return [f]
     else:
         acc = []
         for i, doc in enumerate(docs):
             name = f"{paper.stem}_{i}.txt"
             f = (where / name)
             print(f"writing {f}")
-            f.write_text(doc.page_content)
+            text = clean_text(doc.page_content) if cleaning else doc.page_content
+            f.write_text(text)
             acc.append(f)
         return acc
 
 def try_parse_paper(paper: Path, folder: Optional[Path] = None,
                     mode: str = "single", strategy: str = "auto",
                     pdf_infer_table_structure: bool = True,
-                    include_page_breaks: bool = False, recreate_parent: bool = False) -> Try[List[Path]]:
-    return Try.of(lambda: parse_paper(paper, folder, mode, strategy, pdf_infer_table_structure, include_page_breaks, recreate_parent))
+                    include_page_breaks: bool = False, recreate_parent: bool = False, cleaning: bool = True) -> Try[List[Path]]:
+    return Try.of(lambda: parse_paper(paper, folder, mode, strategy, pdf_infer_table_structure, include_page_breaks, recreate_parent, cleaning))
 
 
 def parse_papers(parse_folder: Path, destination: Optional[Path] = None,
                  mode: str = "single", strategy: str = "auto",
                  pdf_infer_table_structure: bool = True,
-                 include_page_breaks: bool = False, recreate_parent: bool = False, cores: Optional[int] = None):
+                 include_page_breaks: bool = False, recreate_parent: bool = False, cores: Optional[int] = None, cleaning: bool = True):
     """
     Function to parse multiple papers using multiple cores.
     The function employs multiprocessing to speed up the process.
 
     Args:
         parse_folder (Path): The folder where the papers (PDF files) are located.
         destination (Optional[Path]): The destination folder where parsed papers will be saved.
@@ -110,75 +114,30 @@
     parsed = []
     errors = []
 
     cores = cpu_count() if cores is None else min(cpu_count(), cores)
     with Pool(cores) as p:
         parse_func = partial(try_parse_paper, folder=destination, mode=mode, strategy=strategy,
                              pdf_infer_table_structure=pdf_infer_table_structure,
-                             include_page_breaks=include_page_breaks, recreate_parent = recreate_parent)
+                             include_page_breaks=include_page_breaks, recreate_parent = recreate_parent, cleaning = cleaning)
         results = p.map(parse_func, papers)
         for result in results:
             if isinstance(result, pynction.monads.try_monad.Success):
                 parsed = parsed + result._value
             elif isinstance(result, pynction.monads.try_monad.Failure):
                 errors.append(result._e)
             else:
                 print(f"unpredicted type of the {result}")
 
     print("papers parsing finished!")
-    if len(errors) >0:
+    if len(errors) > 0:
         print(f"errors discovered: {errors}")
     return results, errors
 
 
-def papers_to_documents(folder: Path, suffix: str = ""):
-    txt = traverse(folder, lambda p: "txt" in p.suffix)
-    texts = [t for t in txt if suffix in t.name] if suffix != "" else txt
-    docs: List[Document] = []
-    for t in texts:
-        doi = f"http://doi.org/{t.parent.name}/{t.stem}"
-        with open(t, 'r', encoding="utf-8") as file:
-            text = file.read()
-            if len(text)<10:
-                print("TOO SHORT TEXT")
-            else:
-                doc = Document(
-                    page_content = text,
-                    metadata={"source": doi}
-                )
-                docs.append(doc)
-    return docs
-
-
-@deprecated(version='0.1.6', reason="parse_papers function was rewritten with multiprocessors support")
-def parse_papers_async(parse_folder: Path, destination: Optional[Path] = None,
-                 mode: str = "single", strategy: str = "auto",
-                 pdf_infer_table_structure: bool = True,
-                 include_page_breaks: bool = False,
-                 threads: int = 5):
-    papers: list[Path] = traverse(parse_folder, lambda p: "pdf" in p.suffix)
-    print(f"indexing {len(papers)} papers")
-
-    async def async_parse_paper(paper):
-        loop = asyncio.get_running_loop()
-        where = destination if destination is not None else paper.parent
-        return await loop.run_in_executor(
-            executor, parse_paper, paper, where, mode, strategy, pdf_infer_table_structure, include_page_breaks
-        )
-
-    executor = ThreadPoolExecutor(max_workers=threads)
-
-    loop = asyncio.get_event_loop()
-    tasks = [async_parse_paper(paper) for paper in papers]
-    parsed_papers = loop.run_until_complete(asyncio.gather(*tasks))
-
-    print("papers parsing finished!")
-    return parsed_papers
-
-
 @click.group(invoke_without_command=False)
 @click.pass_context
 def app(ctx: Context):
     #if ctx.invoked_subcommand is None:
     #    click.echo('Running the default command...')
     #    test_index()
     pass
@@ -219,25 +178,27 @@
 @click.option('--recreate_parent', type=click.BOOL, default=False, help="if parent folder should be recreated in the new destination")
 def parse_paper_command(paper: str, destination: str, mode: str, strategy: str, infer_tables: bool, include_page_breaks: bool, recreate_parent: bool):
     paper_file = Path(paper)
     destination_folder = Path(destination)
     print(f"parsing paper {paper} with mode={mode} {'' if destination_folder is None else 'destination folder ' + destination}")
     return parse_paper(paper_file, None, mode, strategy, infer_tables, include_page_breaks, recreate_parent)
 
+
 @app.command("parse_folder")
 @click.option('--folder', type=click.Path(exists=True), help="folder to parse papers in")
 @click.option('--destination', type=click.STRING, default=None, help="destination folder")
 @click.option('--mode', type=click.Choice(["single", "elements", "paged"]), default="single", help="paper mode to be used")
 @click.option('--strategy', type=click.Choice(["auto", "hi_res", "fast"]), default="auto", help="parsing strategy to be used, auto by default")
 @click.option('--infer_tables', type=click.BOOL, default=True, help="if the table structure should be inferred")
 @click.option('--include_page_breaks', type=click.BOOL, default=False, help="if page breaks should be included")
 @click.option('--cores', '-t', type=int, default=None, help='Number of cores to use')
 @click.option('--recreate_parent', type=click.BOOL, default=False, help="if parent folder should be recreated in the new destination")
-def parse_paper_command(folder: str, destination: str, mode: str, strategy: str, infer_tables: bool, include_page_breaks: bool, cores: Optional[int], recreate_parent: bool):
+@click.option('--cleaning', type=click.BOOL, default=True, help="if we should use basic cleaning for the text")
+def parse_folder_command(folder: str, destination: str, mode: str, strategy: str, infer_tables: bool, include_page_breaks: bool, cores: Optional[int], recreate_parent: bool, cleaning: bool):
     parse_folder = Path(folder)
     destination_folder = Path(destination) if destination is not None else None
     print(f"parsing paper {folder} with mode={mode} {'' if destination_folder is None else 'destination folder ' + destination}")
-    return parse_papers(parse_folder, destination_folder, mode, strategy, infer_tables, include_page_breaks, recreate_parent, cores = cores)
+    return parse_papers(parse_folder, destination_folder, mode, strategy, infer_tables, include_page_breaks, recreate_parent, cores = cores, cleaning=cleaning)
 
 
 if __name__ == '__main__':
     app()
```

### Comparing `getpaper-0.1.8/getpaper.egg-info/PKG-INFO` & `getpaper-0.1.9/getpaper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getpaper
-Version: 0.1.8
+Version: 0.1.9
 Summary: getpaper - papers download made easy!
 Author: antonkulaga (Anton Kulaga)
 Author-email: <antonkulaga@gmail.com>
 Keywords: python,utils,files,papers,download
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
@@ -73,15 +73,15 @@
 download download_papers --dois "10.3390/ijms22031073" --dois "10.1038/s41597-020-00710-z" --dois "wrong" --folder "data/output/test/papers" --threads 5
 ```
 
 ## Parsing the papers
 
 You can parse the downloaded papers with the unstructured library. For example if the papers are in the folder test, you can run:
 ```bash
-getpaper/parse.py parse_folder --folder data/output/test/papers --threads 5
+getpaper/parse.py parse_folder --folder data/output/test/papers --cores 5
 ```
 You can also parse papers on a per-file basis, for example:
 ```bash
 getpaper/parse.py parse_paper --paper data/output/test/papers/10.3390/ijms22031073.pdf
 ```
 
 ## Count tokens
@@ -94,15 +94,15 @@
 
 ## Indexing papers
 
 We also provide features to index the papers with openai or lambda embeddings and save them in chromadb vector store.
 For openai embeddings to work you have to create .env file and specify your openai key there, see .env.template as example
 For example if you have your papers inside data/output/test/papers folder, and you want to make a ChromaDB index at data/output/test/index you can do it by:
 ```bash
-python getpaper/index.py index_papers --papers data/output/test/papers --folder data/output/test/index --collection mypapers --chunk_size 6000
+getpaper/index.py index_papers --papers data/output/test/papers --folder data/output/test/index --collection mypapers --chunk_size 6000
 ```
 
 # Examples
 
 You can run examples.py to see usage examples
 
 # Additional requirements
```

### Comparing `getpaper-0.1.8/setup.py` & `getpaper-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.8'
+VERSION = '0.1.9'
 DESCRIPTION = 'getpaper - papers download made easy!'
 LONG_DESCRIPTION = 'A package with python functions for downloading papers'
 
 # Setting up
 setup(
     name="getpaper",
     version=VERSION,
```


# Comparing `tmp/gpubs-3.tar.gz` & `tmp/gpubs-4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpubs-3.tar", last modified: Fri Jun 23 21:26:59 2023, max compression
+gzip compressed data, was "gpubs-4.tar", last modified: Sat Jun 24 04:35:53 2023, max compression
```

## Comparing `gpubs-3.tar` & `gpubs-4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 krobasky  (1000) krobasky  (1000)        0 2023-06-23 21:26:59.471773 gpubs-3/
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)       28 2023-06-23 03:40:04.000000 gpubs-3/MANIFEST.in
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)      261 2023-06-23 21:26:59.471773 gpubs-3/PKG-INFO
-drwxr-xr-x   0 krobasky  (1000) krobasky  (1000)        0 2023-06-23 21:26:59.471773 gpubs-3/gpubs/
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)      129 2023-06-23 03:11:20.000000 gpubs-3/gpubs/__init__.py
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)       18 2023-06-23 21:26:59.000000 gpubs-3/gpubs/_version.py
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)    15302 2023-06-23 21:11:44.000000 gpubs-3/gpubs/api.py
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)     1829 2023-06-21 14:00:14.000000 gpubs-3/gpubs/fetch.py
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)      210 2023-06-21 02:49:51.000000 gpubs-3/gpubs/log.py
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)     6583 2023-06-23 20:45:43.000000 gpubs-3/gpubs/models.py
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)     3989 2023-06-23 21:12:15.000000 gpubs-3/gpubs/parse.py
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)     1292 2023-06-21 13:33:20.000000 gpubs-3/gpubs/reference.py
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)     1939 2023-06-21 02:50:26.000000 gpubs-3/gpubs/search_words.py
-drwxr-xr-x   0 krobasky  (1000) krobasky  (1000)        0 2023-06-23 21:26:59.471773 gpubs-3/gpubs.egg-info/
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)      261 2023-06-23 21:26:59.000000 gpubs-3/gpubs.egg-info/PKG-INFO
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)      411 2023-06-23 21:26:59.000000 gpubs-3/gpubs.egg-info/SOURCES.txt
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)        1 2023-06-23 21:26:59.000000 gpubs-3/gpubs.egg-info/dependency_links.txt
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)       76 2023-06-23 21:26:59.000000 gpubs-3/gpubs.egg-info/requires.txt
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)        6 2023-06-23 21:26:59.000000 gpubs-3/gpubs.egg-info/top_level.txt
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)      359 2023-06-23 21:26:38.000000 gpubs-3/release-info.json
-drwxr-xr-x   0 krobasky  (1000) krobasky  (1000)        0 2023-06-23 21:26:59.471773 gpubs-3/scripts/
--rwxr-xr-x   0 krobasky  (1000) krobasky  (1000)     4101 2023-06-21 02:46:43.000000 gpubs-3/scripts/create_search_terms_file.sh
--rwxr-xr-x   0 krobasky  (1000) krobasky  (1000)     5195 2023-06-21 02:46:43.000000 gpubs-3/scripts/download_pubs.sh
--rwxr-xr-x   0 krobasky  (1000) krobasky  (1000)     1892 2023-06-21 02:46:43.000000 gpubs-3/scripts/search.awk
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)       38 2023-06-23 21:26:59.471773 gpubs-3/setup.cfg
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)     1164 2023-06-23 04:40:13.000000 gpubs-3/setup.py
+drwxr-xr-x   0 krobasky  (1000) krobasky  (1000)        0 2023-06-24 04:35:53.032247 gpubs-4/
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)       28 2023-06-23 03:40:04.000000 gpubs-4/MANIFEST.in
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)      261 2023-06-24 04:35:53.032247 gpubs-4/PKG-INFO
+drwxr-xr-x   0 krobasky  (1000) krobasky  (1000)        0 2023-06-24 04:35:53.032247 gpubs-4/gpubs/
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)      129 2023-06-23 03:11:20.000000 gpubs-4/gpubs/__init__.py
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)       18 2023-06-24 04:35:52.000000 gpubs-4/gpubs/_version.py
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)    19754 2023-06-24 04:34:36.000000 gpubs-4/gpubs/api.py
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)     2111 2023-06-24 02:02:55.000000 gpubs-4/gpubs/fetch.py
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)      209 2023-06-24 01:55:43.000000 gpubs-4/gpubs/log.py
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)     7035 2023-06-24 02:40:36.000000 gpubs-4/gpubs/models.py
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)     4066 2023-06-24 02:04:02.000000 gpubs-4/gpubs/parse.py
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)     1301 2023-06-24 01:55:43.000000 gpubs-4/gpubs/reference.py
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)     1899 2023-06-24 03:41:23.000000 gpubs-4/gpubs/search_words.py
+drwxr-xr-x   0 krobasky  (1000) krobasky  (1000)        0 2023-06-24 04:35:53.032247 gpubs-4/gpubs.egg-info/
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)      261 2023-06-24 04:35:52.000000 gpubs-4/gpubs.egg-info/PKG-INFO
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)      411 2023-06-24 04:35:52.000000 gpubs-4/gpubs.egg-info/SOURCES.txt
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)        1 2023-06-24 04:35:52.000000 gpubs-4/gpubs.egg-info/dependency_links.txt
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)       76 2023-06-24 04:35:52.000000 gpubs-4/gpubs.egg-info/requires.txt
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)        6 2023-06-24 04:35:52.000000 gpubs-4/gpubs.egg-info/top_level.txt
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)      359 2023-06-23 21:37:20.000000 gpubs-4/release-info.json
+drwxr-xr-x   0 krobasky  (1000) krobasky  (1000)        0 2023-06-24 04:35:53.032247 gpubs-4/scripts/
+-rwxr-xr-x   0 krobasky  (1000) krobasky  (1000)     4101 2023-06-21 02:46:43.000000 gpubs-4/scripts/create_search_terms_file.sh
+-rwxr-xr-x   0 krobasky  (1000) krobasky  (1000)     5195 2023-06-21 02:46:43.000000 gpubs-4/scripts/download_pubs.sh
+-rwxr-xr-x   0 krobasky  (1000) krobasky  (1000)     1892 2023-06-21 02:46:43.000000 gpubs-4/scripts/search.awk
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)       38 2023-06-24 04:35:53.032247 gpubs-4/setup.cfg
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)     1141 2023-06-24 02:06:26.000000 gpubs-4/setup.py
```

### Comparing `gpubs-3/gpubs/api.py` & `gpubs-4/gpubs/api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,74 @@
-from typing import List, Dict, Set
+from typing import List
 import os
 
 from gpubs.models import ReferenceData
 from gpubs.log import msg1, msg2
 from gpubs.reference import download_gene_symbols, extract_gene_data
-from gpubs.search_words import fetch_brown_corpus, create_stop_words, read_search_stop, filter_search_terms
+from gpubs.search_words import (
+    fetch_brown_corpus,
+    create_stop_words,
+    read_search_stop,
+    filter_search_terms,
+)
 from gpubs.fetch import check_disk_space, download_file, verify_md5
 from gpubs.parse import parse_pubs
 
+
 def create_gene_reference_data(m: ReferenceData):
-    
+    """Gets gene reference data into a convenient format for creating a m.filtered_terms_files, and ultimately, tagging abstracts with gene information.
+
+    Performs the following:
+
+      1. Downloads gene_info.gz from m.ncbi_gene_info_url
+
+      2. Parses gene_info.gz to create the following files:
+
+        - m.reference_path()/m.gene_symbols_filename [default = v1/reference/gene_symbols.txt]
+        - m.reference_path()/m.gene_synonyms_filename [default = v1/reference/gene_synonyms.txt]
+        - m.dbxref_path()/*.txt [default = v1/reference/dbxrefs/*.txt]
+
+    """
+
     raw_gene_info_filepath = os.path.join(m.raw_path(), m.gene_info_filename)
-    reference_gene_symbols_filepath = os.path.join(m.reference_path(), m.gene_symbols_filename)
-    reference_gene_synonyms_filepath = os.path.join(m.reference_path(), m.gene_synonyms_filename)
+    reference_gene_symbols_filepath = os.path.join(
+        m.reference_path(), m.gene_symbols_filename
+    )
+    reference_gene_synonyms_filepath = os.path.join(
+        m.reference_path(), m.gene_synonyms_filename
+    )
     dbxref_path = m.dbxref_path()
     verbose = m.verbose
     url = m.ncbi_gene_info_url
-    
+
     # Download the gene symbols file
-    download_gene_symbols(output_filepath = raw_gene_info_filepath, url = url, verbose = verbose)
+    download_gene_symbols(
+        output_filepath=raw_gene_info_filepath, url=url, verbose=verbose
+    )
 
     # Extract gene data
-    gene_symbols, dbxrefs, gene_synonyms = extract_gene_data(filepath = raw_gene_info_filepath)
+    gene_symbols, dbxrefs, gene_synonyms = extract_gene_data(
+        filepath=raw_gene_info_filepath
+    )
 
     # Save gene symbols to a file
     with open(reference_gene_symbols_filepath, "w") as file:
         for symbol in gene_symbols:
             file.write(symbol + "\n")
 
     msg2(verbose, f"Gene symbols saved to {reference_gene_symbols_filepath}")
 
     # Save dbXrefs to separate files
     for identifier in dbxrefs:
-            identifier_parts = identifier.split(":")
-            identifier_type = identifier_parts[0].replace('/','_')
-            identifier_value = ":".join(identifier_parts[1:])
-            filename = f"{dbxref_path}/{identifier_type}.txt"
-            with open(filename, "a") as file:
-                file.write(identifier_value + "\n")
+        identifier_parts = identifier.split(":")
+        identifier_type = identifier_parts[0].replace("/", "_")
+        identifier_value = ":".join(identifier_parts[1:])
+        filename = f"{dbxref_path}/{identifier_type}.txt"
+        with open(filename, "a") as file:
+            file.write(identifier_value + "\n")
 
     """
     for identifiers in dbxrefs:
         for identifier in identifiers:
             identifier_parts = identifier.split(":")
             identifier_type = identifier_parts[0].replace('/','_')
             identifier_value = ":".join(identifier_parts[1:])
@@ -54,157 +81,218 @@
     # Save gene synonyms to a file
     with open(reference_gene_synonyms_filepath, "w") as file:
         for synonym in gene_synonyms:
             file.write(synonym + "\n")
 
     msg2(verbose, f"Gene synonyms saved to {reference_gene_synonyms_filepath}")
 
+
 def create_frequency_list(m: ReferenceData) -> List:
-    
+    """Creates a file that lists the most common English words, up to (m.corpus_stop_word_list_length) in size,
+    and saves to m.search_path()/m.frequency_list_filename [default = v1/data/search_terms/frequency_list.txt]
+
+    Returns:
+
+      A list of most common words, most common first, all lower case
+
+    """
     frequency_list_outpath = os.path.join(m.search_path(), m.frequency_list_filename)
     stop_word_list_length = m.corpus_stop_word_list_length
     verbose = m.verbose
-    
-    import nltk
+
     from nltk import FreqDist
     import string
 
     words = fetch_brown_corpus()
 
     # Remove punctuation and convert to lowercase
-    words = [word.lower() for word in words if word not in string.punctuation and word.isalnum()]
+    words = [
+        word.lower()
+        for word in words
+        if word not in string.punctuation and word.isalnum()
+    ]
 
     # Compute the frequency distribution of words
     freq_dist = FreqDist(words)
 
     # Get the most frequent words
     most_common_words = freq_dist.most_common(stop_word_list_length)
 
     # Write the frequency list to a file
-    with open(frequency_list_outpath, 'w') as file:
+    with open(frequency_list_outpath, "w") as file:
         for word, frequency in most_common_words:
-            file.write(word + '\n')
+            file.write(word + "\n")
     msg2(verbose, f"Wrote {frequency_list_outpath}")
     return most_common_words
 
+
 def create_search_terms_file(m: ReferenceData):
+    """Uses the files from `create_gene_reference_data` to generate the list of terms for searching each abstract.
+
+    Each abstract is searched for gene symbols, synonyms, and
+    dbxref's. The file created here lists all the gene info terms to
+    use for that search. The file is saved to
+    m.search_path()/m.search_terms_filename [default =
+    `v1/data/search_terms/search_terms.txt`].
+
+    The file f"{m.search_path()/m.search_terms_filename}.unsorted" is a byproduct and can be discarded.
+
+    Returns:
+
+      A list of the search terms (gene symbols, synonyms and accession IDs)
+
+    """
+
     import os
 
     dbxrefs = m.dbxrefs
-    dbxrefs_path = m.dbxref_path()  
+    dbxrefs_path = m.dbxref_path()
     gene_symbols_filepath = os.path.join(m.reference_path(), m.gene_symbols_filename)
     gene_synonyms_filepath = os.path.join(m.reference_path(), m.gene_synonyms_filename)
     search_terms_filepath = os.path.join(m.search_path(), m.search_terms_filename)
     verbose = m.verbose
 
     if dbxrefs == []:
         # Get a list of all files in the directory
         dbxrefs = os.listdir(dbxrefs_path)
         # Filter out directories from the list
         dbxrefs = [f for f in dbxrefs if os.path.isfile(os.path.join(dbxrefs_path, f))]
-  
-    
+
     with open(f"{search_terms_filepath}.unsorted", "w") as outfile:
         for ref in dbxrefs:
             with open(os.path.join(dbxrefs_path, ref)) as infile:
                 sorted_lines = sorted(set(infile.readlines()))
                 outfile.writelines(sorted_lines)
-                #outfile.write(infile.read())
+                # outfile.write(infile.read())
 
         with open(gene_symbols_filepath) as infile:
             sorted_lines = sorted(set(infile.readlines()))
             outfile.writelines(sorted_lines)
-            #outfile.write(infile.read())
+            # outfile.write(infile.read())
 
         with open(gene_synonyms_filepath) as infile:
             sorted_lines = sorted(set(infile.readlines()))
             outfile.writelines(sorted_lines)
-            #outfile.write(infile.read())
+            # outfile.write(infile.read())
 
     # Sort and remove duplicates from the search terms file
     search_terms_unsorted_filepath = f"{search_terms_filepath}.unsorted"
-    os.system(f"sort -u {search_terms_unsorted_filepath} | grep -v not > {search_terms_filepath}")
+    os.system(
+        f"sort -u {search_terms_unsorted_filepath} | grep -v not > {search_terms_filepath}"
+    )
 
     msg2(verbose, f"Created {search_terms_filepath}.")
     msg2(verbose, f"Created {search_terms_unsorted_filepath} - can be removed.")
     line_count = sum(1 for line in open(search_terms_filepath))
     msg2(verbose, f"Number of lines in {search_terms_filepath}: {line_count}")
 
+
 def create_filtered_search_terms(m: ReferenceData) -> List:
-    
+    """Filters search_terms against m.frequency_list_filename and m.custom_stop_words.
+
+    If the search term (e.g., gene name) is also a stop word (e.g.,
+    'DANGER'), then retain the term's original case. Otherwise,
+    lowercase the term. Either way, add it to the list of terms to be returned.
+
+    Ultimately, when an abstract is searched for a filtered_term, it
+    will only match case if the term is a stop_word. This allows for
+    more permissive matching against gene names in abstracts that use
+    peculiar case.
+
+    Returns:
+
+      List of the terms, all lowercase, accept for those that matched an English language word in the frequency_list.
+
+    """
+
     search_file = os.path.join(m.search_path(), m.search_terms_filename)
     frequency_list_outpath = os.path.join(m.search_path(), m.frequency_list_filename)
     custom_words = m.custom_stop_words
     final_file = os.path.join(m.search_path(), m.filtered_terms_filename)
     verbose = m.verbose
-    
+
     stop_words = create_stop_words(frequency_list_outpath, custom_words)
-    
-    search_terms = read_search_stop(search_file = search_file, stop_words = stop_words)
+
+    search_terms = read_search_stop(search_file=search_file, stop_words=stop_words)
     msg2(verbose, f"Number of original search_terms:{len(search_terms)}")
-    final_terms, filtered_terms, matched_stop_words = filter_search_terms(search_terms, stop_words)
-    msg2(verbose, f"number of filtered_terms:{len(filtered_terms)}\nfinal number of final_terms:{len(final_terms)}\n number of matched_stop_words:{len(matched_stop_words)}\nmatched_stop_words={matched_stop_words}")
+    final_terms, filtered_terms, matched_stop_words = filter_search_terms(
+        search_terms, stop_words
+    )
+    msg2(
+        verbose,
+        f"number of filtered_terms:{len(filtered_terms)}\nfinal number of final_terms:{len(final_terms)}\n number of matched_stop_words:{len(matched_stop_words)}\nmatched_stop_words={matched_stop_words}",
+    )
     if final_file is not None:
         with open(final_file, "w") as f:
-            f.writelines('\n'.join(final_terms))
+            f.writelines("\n".join(final_terms))
     msg2(verbose, f"Created {final_file}")
     return final_terms
 
 
-def fetch_abstracts(m: ReferenceData, get_updates: bool = False):
-    """ Downloads files from m.ncbi_ftp_host. 
+def fetch_abstracts(m: ReferenceData, get_updates: bool = False):  # noqa: C901
+    """Downloads files from m.ncbi_ftp_host.
 
     ARGS:
 
       get_updates: If True then download the updatefiles, otherwise get the baseline. See : https://ftp.ncbi.nlm.nih.gov/pubmed/baseline/README.txt
 
     """
     import subprocess
-    
+
     num_files = m.num_abstract_xml_files
     refresh = m.refresh_abstract_xml_files
     ftp_host = m.ncbi_ftp_host
     download_dir = m.pub_inpath()
     verbose = m.verbose
     if get_updates:
         download_dir = os.path.join(download_dir, m.abstract_updatefiles_inpath)
         ftp_path = m.ncbi_ftp_updatefiles_path
         msg2(verbose, f"! Getting update files, download_dir={download_dir}.")
     else:
         ftp_path = m.ncbi_ftp_baseline_path
-    
-    """ This can probably be done faster with download_files.sh """ 
+
+    """ This can probably be done faster with download_files.sh """
     msg2(verbose, f"Download Directory: {download_dir}")
     msg2(verbose, f"Number of abstracts to ensure have been downloaded: {num_files}")
     msg2(verbose, f"Refresh: {refresh}")
 
-
     # Retrieve file names and find the largest number
-    #file_list = subprocess.check_output(['curl', '-s', f"ftp://{ftp_host}{ftp_path}"]).decode().splitlines()
-    
-    output = subprocess.check_output(['curl', '-s', f"ftp://{ftp_host}{ftp_path}"]).decode()
+    # file_list = subprocess.check_output(['curl', '-s', f"ftp://{ftp_host}{ftp_path}"]).decode().splitlines()
+
+    output = subprocess.check_output(
+        ["curl", "-s", f"ftp://{ftp_host}{ftp_path}"]
+    ).decode()
     msg2(verbose, f"file_list curl: curl -s ftp://{ftp_host}{ftp_path}")
-    file_list = [line.split()[-1] for line in output.splitlines() if line.endswith(".xml.gz")]
+    file_list = [
+        line.split()[-1] for line in output.splitlines() if line.endswith(".xml.gz")
+    ]
 
     msg2(verbose, f"Total number of NCBI abstract XML files: {len(file_list)}")
-    latest_files = [file_name for file_name in file_list if file_name.startswith("pubmed23n") and file_name.endswith(".xml.gz")]
+    latest_files = [
+        file_name
+        for file_name in file_list
+        if file_name.startswith("pubmed23n") and file_name.endswith(".xml.gz")
+    ]
     latest_files.sort(reverse=True)
     latest_files = latest_files[:num_files]
     msg2(verbose, f"latest_files {num_files}: {latest_files}")
 
     # Check if enough files are available
     import sys
+
     if len(latest_files) == 0:
         msg1(verbose, "Error: Insufficient number of files available!")
         sys.exit(1)
 
     # Calculate total predicted size
     total_size = 0
     for file_name in latest_files:
-        response = subprocess.check_output(['curl', '-sI', f"ftp://{ftp_host}{ftp_path}{file_name}"]).decode()
+        response = subprocess.check_output(
+            ["curl", "-sI", f"ftp://{ftp_host}{ftp_path}{file_name}"]
+        ).decode()
         file_size = int(response.split("Content-Length: ")[1].split("\r")[0])
         total_size += file_size
 
     # Check disk space before downloading
     check_disk_space(total_size, download_dir, verbose=verbose)
 
     # Download and check files
@@ -225,136 +313,193 @@
                 msg1(verbose, f"ERROR: Missing - {file_path}; re-downloading now")
 
             if os.path.isfile(file_path) and os.path.isfile(md5_file_path):
                 msg1(verbose, f"SKIP: {file_path} exists.")
                 continue
 
         # Check file size
-        response = subprocess.check_output(['curl', '-sI', f"ftp://{ftp_host}{ftp_path}{file_name}"]).decode()
+        response = subprocess.check_output(
+            ["curl", "-sI", f"ftp://{ftp_host}{ftp_path}{file_name}"]
+        ).decode()
         file_size = int(response.split("Content-Length: ")[1].split("\r")[0])
 
         msg2(verbose, f"File: {file_name}, Size: {file_size} bytes")
 
         # Download file
         msg2(verbose, f"WARNING: Downloading: {file_name} to {download_dir}")
         if os.path.isfile(file_path):
             os.remove(file_path)
         download_file(f"ftp://{ftp_host}{ftp_path}{file_name}", file_path, verbose)
 
         # Download MD5 file
         if os.path.isfile(md5_file_path):
             os.remove(md5_file_path)
-        download_file(f"ftp://{ftp_host}{ftp_path}{md5_file_name}", md5_file_path, verbose)
+        download_file(
+            f"ftp://{ftp_host}{ftp_path}{md5_file_name}", md5_file_path, verbose
+        )
 
         # Check MD5
         verify_md5(file_path, md5_file_path, verbose)
 
-    total_size_human = subprocess.check_output(['numfmt', '--to=iec-i', '--suffix=B', str(total_size)]).decode().strip()
+    total_size_human = (
+        subprocess.check_output(["numfmt", "--to=iec-i", "--suffix=B", str(total_size)])
+        .decode()
+        .strip()
+    )
     msg2(verbose, f"Total size of abstract files: {total_size_human}")
 
+
 def create_pubcsv_dataset(m: ReferenceData, parse_updates: bool = False) -> List:
-    """ Takes about 14min for 30 (2-3 per minute) 
+    """Parse all the XML files into csv files. Overwites anything previously written. Takes about 14min for 30 (2-3 per minute)
 
     ARGS:
 
       parse_updates: If True then parse the updatefiles, otherwise parse the baseline. See : https://ftp.ncbi.nlm.nih.gov/pubmed/baseline/README.txt
-      
+
     """
     import os
-    
+
     abstract_length_threshold = m.abstract_length_threshold
     pub_inpath = m.pub_inpath()
     pub_updatefiles_inpath = os.path.join(m.pub_inpath(), m.abstract_updatefiles_inpath)
     if parse_updates:
         pub_inpath = os.path.join(pub_inpath, m.abstract_updatefiles_inpath)
     pub_outpath = m.pub_outpath()
     verbose = m.verbose
-    
+
     csv_list = []
 
     # Iterate through files in the directory
-    csv_list = parse_pubs(inpath=pub_inpath, outpath=pub_outpath, length_threshold = abstract_length_threshold, csv_list=csv_list, verbose=verbose)
+    csv_list = parse_pubs(
+        inpath=pub_inpath,
+        outpath=pub_outpath,
+        length_threshold=abstract_length_threshold,
+        csv_list=csv_list,
+        verbose=verbose,
+    )
 
     # Repeat for 'updatefiles'
-    csv_list = parse_pubs(inpath=pub_updatefiles_inpath, outpath=pub_outpath, length_threshold = abstract_length_threshold, csv_list=csv_list, verbose=verbose)
-            
-    return(csv_list)
+    csv_list = parse_pubs(
+        inpath=pub_updatefiles_inpath,
+        outpath=pub_outpath,
+        length_threshold=abstract_length_threshold,
+        csv_list=csv_list,
+        verbose=verbose,
+    )
+
+    return csv_list
+
 
 def create_gene_files(m: ReferenceData):
-    """ Calls the search.awk script in gpubs/scripts """
-    
+    """Calls the search.awk script in gpubs/scripts. This results in
+    all the abstracts files being tagged with the gene
+    name/identifier, if present. Uses the m.filtered_terms_filename for search terms.
+
+    If the search term is also a 'stop word', then search.awk matches
+    case from filtered_terms.txt (which ultimately comes from NCBI's
+    gene_info.gz). Otherwise, case is permissive to accommodate
+    abstracts that use peculiar case for a gene. Note that terms in
+    filtered_terms.txt are also all lowercase for performance, accept
+    those that are stop words.
+
+    Note - to use a custom list of gene symbols/synonyms/accession
+    ids, just filter everything out of the filtered_terms.txt except
+    the genes of interest. Find the filtered_terms.txt file in
+    m.search_path()/m.filtered_terms_filename [default:
+    v1/data/search_terms/filtered_terms.txt]
+
+    This is the last setp of the pipeline
+
+    Exmample usage:
+
+    >>> m = ReferenceData()
+    >>> create_gene_reference_data(m) # get gene_info from NCBI
+    >>> _ = create_frequency_list(m)  # create English stop words from 'brown' corpus
+    >>> create_search_terms_file(m)   # combine the files parsed out of gene_info to get search terms
+    >>> _ = create_filtered_search_terms(m)  # filter search terms with stop words
+    >>> fetch_abstracts(m)            # download abstract XML files from NCBI
+    >>> fetch_abstracts(m, get_updates=True) # download abstract XML "updatefiles" from NCBI
+    >>> _ = create_pubcsv_dataset(m)  # translate abstract XML files to csv
+    >>> # NOTE: keep only genes of interest in v1/data/search_terms/filtered_terms.txt
+    >>> create_gene_files(m)          # tag abstracts with the search terms (genes) from filtered_terms.txt
+    >>> # final files in m.genes_outpath [default= v1/data/csvpubs/genes]
+
+    """
+
     filtered_terms_file = os.path.join(m.search_path(), m.filtered_terms_filename)
     csv_inpath = m.pub_outpath()
     csv_outpath = m.genes_outpath()
     verbose = m.verbose
-    
+
     import glob
     import subprocess
+
     awk_script = "search.awk"
     # Check if awk_script is under ./scripts - e.g., this is being run from the notebook from inside the repo
     # otherwise awk_script should be in path - e.g. gpubs has been pip install'd
     if os.path.isfile(os.path.join("scripts", awk_script)):
         awk_script = os.path.join("scripts", awk_script)
-    for file_name_path in glob.glob(os.path.join(csv_inpath,"pubmed*.xml.gz.csv")):
+    for file_name_path in glob.glob(os.path.join(csv_inpath, "pubmed*.xml.gz.csv")):
         file_name = os.path.basename(file_name_path)
         input_csv_file = os.path.join(csv_inpath, file_name)
         output_csv_file = os.path.join(csv_outpath, file_name)
         msg2(verbose, f"Creating {output_csv_file}")
         error_file = os.path.join(csv_outpath, f"{file_name}.err")
         # xxx test this out, then run make to install version 2
         command = [awk_script, filtered_terms_file, input_csv_file]
         with open(output_csv_file, "w") as output, open(error_file, "w") as error:
             subprocess.run(command, stdout=output, stderr=error)
 
+
 def pipeline(m: ReferenceData):
-    """ 
-    Run the whole data pipeline, end to end. See QuickStart notebook for step-by-step outputs
+    """Run the whole data pipeline, end to end. See QuickStart notebook for step-by-step outputs
 
-    Example:
+    Example usage:
 
-      import gpubs
-      from gpubs.models import ReferenceData
-      from gpubs.api import pipeline
-
-      # Create data model
-      m = ReferenceData(version = "../../v1",       # make data root above any git repo
-                        verbose = 2,                # print all the info messages
-                        num_abstract_xml_files = 3, # only fetch 3 files from NCBI
-                        dbxrefs = ["AllianceGenome.txt", "Ensembl.txt", "HGNC.txt", "IMGT_GENE-DB.txt"]  # exclude miRNA and MIM
-                 )
-      pipeline(m)
+      >>> import gpubs
+      >>> from gpubs.models import ReferenceData
+      >>> from gpubs.api import pipeline
+      >>>
+      >>> # Create data model
+      >>> # exclude miRNA and MIM dbxrefs
+      >>> m = ReferenceData(version = "../../v1",       # put data above the github repo
+      >>>                   verbose = 2,                # print info messages
+      >>>                   num_abstract_xml_files = 3, # only download 3 abstract XML files from NCBI
+      >>>                   dbxrefs = ["AllianceGenome.txt", "Ensembl.txt", "HGNC.txt", "IMGT_GENE-DB.txt"])
+      >>> pipeline(m)
 
     """
 
-    # Fetch data/raw/gene_info.gz 
+    # Fetch data/raw/gene_info.gz
     # and create the human genes lists under data/reference (gene_symbols.txt, gene_synonyms.txt, dbxrefs/*)
     create_gene_reference_data(m)
 
-
-    # The goal of the following 3 calls is to 
+    # The goal of the following 3 calls is to
     # create data/search_terms/filtered_terms.txt from english language corpus
 
     # Create a word frequency list from an English language corpus
     _ = create_frequency_list(m)
 
     # Create the file of gene search terms (data/search_terms/search_terms.txt) using stop words from frequency list
     create_search_terms_file(m)
 
     # Create the filtered_terms.txt file
-    final_terms = create_filtered_search_terms(m)
+    _ = create_filtered_search_terms(m)
 
-
-    # Fetch NCBI articl zips
-    # - There are about 1100 files with about 15000 abstracts each.
+    # Fetch NCBI article zips
+    # - There are 1165 files (2023) with about 15000 abstracts each.
     # - ~60GB is needed to get all files
-    # - At about 2 min/file ... ~ 2 days to get 'em all
+    # - On AWS you can get them all in under an hour. 5 hours on consumer-grade wifi.
     fetch_abstracts(m)
 
+    # Get NCBI
+    # ~ 222 abstracts in June 2023
+    fetch_abstracts(m, get_updates=True)
+
     # Create CSVs from XMLs
     # - This takes about 3 minutes to do 10 files; or about 5 hours to do them all
-    csv_list = create_pubcsv_dataset(m)
-
+    _ = create_pubcsv_dataset(m)
 
     # Create new CSVs that include GENES column under data/csvpubs/genes
     # - Takes about 40s for 10 files, which is much slower than just running the awk script
     # - With default settings, it filters out about 42% of the abstracts, most of which are 2022
     create_gene_files(m)
```

### Comparing `gpubs-3/gpubs/models.py` & `gpubs-4/gpubs/models.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,155 +1,287 @@
 import os
-from typing import List, Dict, Set
+from typing import List, Dict
 from pydantic import BaseModel, root_validator
 
-from gpubs.log import msg1,msg2
+from gpubs.log import msg2
+
 
 class ReferenceData(BaseModel):
     """
     Files for retrieving and transforming reference gene information
     """
-    
+
     def __init__(self, *args, **kwargs):
         super(ReferenceData, self).__init__(*args, **kwargs)
 
         self.version_root = os.path.join(os.getcwd(), str(self.version), self.data_root)
         msg2(self.verbose, f"version_root={self.version_root}")
-        
+
         # make directory structure
         os.makedirs(self.version_root, exist_ok=True)
         os.makedirs(self.raw_path(), exist_ok=True)
         os.makedirs(self.reference_path(), exist_ok=True)
         os.makedirs(self.dbxref_path(), exist_ok=True)
         os.makedirs(self.search_path(), exist_ok=True)
         os.makedirs(self.pub_inpath(), exist_ok=True)
-        os.makedirs(os.path.join(self.pub_inpath(),self.abstract_updatefiles_inpath), exist_ok=True)
+        os.makedirs(
+            os.path.join(self.pub_inpath(), self.abstract_updatefiles_inpath),
+            exist_ok=True,
+        )
         os.makedirs(self.pub_outpath(), exist_ok=True)
         os.makedirs(self.genes_outpath(), exist_ok=True)
-        
+
         msg2(self.verbose, "Created directory structure.")
 
     ncbi_gene_info_url: str = "https://ftp.ncbi.nlm.nih.gov/gene/DATA/GENE_INFO/Mammalia/Homo_sapiens.gene_info.gz"
 
     ncbi_ftp_host: str = "ftp.ncbi.nlm.nih.gov"
 
     ncbi_ftp_baseline_path: str = "/pubmed/baseline/"
 
     ncbi_ftp_updatefiles_path: str = "/pubmed/updatefiles/"
-    
-    data_root: str  = "data/"
-    """ full path to where all the raw, reference, and generated data are stored """
-    
+
+    data_root: str = "data/"
+    """ Full path to where all the raw, reference, and generated data are stored """
+
     raw_data_path: str = "raw/"
-    
+
     reference_data_path: str = "reference/"
-    
+
     dbxref_reference_data_path: str = "dbxrefs/"
-    
-    dbxrefs: List = [] 
-    """ if empty, it will just get filled with a list of all the files created in the m.dbxref_path() """
-        
+
+    dbxrefs: List = []
+    """ If empty, it will just get filled with a list of all the files created in the m.dbxref_path() """
+
     gene_info_filename: str = "gene_info.gz"
-    
+
     gene_symbols_filename: str = "gene_symbols.txt"
-    
+
     gene_synonyms_filename: str = "gene_synonyms.txt"
-    
+
     search_terms_path: str = "search_terms/"
-    
+
     frequency_list_filename: str = "frequency_list.txt"
-    
-    corpus_stop_word_list_length:int = 4000
-    
-    # old lsit
-    #custom_stop_words:List = ['ago', 'aim', 'amid', 'april', 'arch', 'bed', 'bite', 'bug', 'co', 'crop', 'damage', 'et', 
-    #                'fast', 'fat', 'fate', 'gap', 'genesis', 'ii', 'iv', 'lamp', 'laser', 'mater', 'melt', 'mice', 'minor', 'mv', 'net', 
-    #                'not', 'race', 'rank', 'se', 'sink', 'soft', 'spatial', 'steel', 'stop', 'tau', 'traits', 'via']
-    
+
+    corpus_stop_word_list_length: int = 4000
+
     # may overlap somewhat with stop words
-    custom_stop_words:List = ['ago', 'aim', 'amid', 'april', 'arch', 'bed', 'bite', 'bug', 'cage', 'co', 'crop',
-                    'damage', 'danger', 'digit', 'et', 'fast', 'fat', 'fate', 'fire', 'flower', 'gap', 'genesis', 'gov', 'gpa', 'grasp',
-                    'ii', 'inos', 'iv', 'killer', 'lab', 'lamp', 'laser', 'map', 'mask', 'mater', 'melt', 'mice', 'minor', 'miss', 'mv',
-                    'nail', 'net', 'not', 'osf', 'pan', 'par', 'pha', 'rab', 'race', 'rain', 'rank',
-                    'san', 'sand', 'se', 'sink', 'soft', 'spatial', 'spin', 'spp', 'steel', 'stop',
-                    'storm', 'tactile', 'tau', 'theta', 'tip', 'traits', 'via', 
-                              "apex", "app", "apps", "args", "ash", "bar", "bit", "cast", "cats", "cava", "cd", "clock", "coil", "cope", "cord", "delta", "eat", "eg", "fats", "fish", "fix", "flame", "flap", "fuse", "grid", "gum", "heal", "hip", "hits", "hub", "igm", "li", "maps", "mets", "mix", "mn", "ms", "nm", "nodal", "pigs", "prey", "pros", "pt", "pva", "ray", "sac", "scar", "sea", "sea", "sp", "steep", "tank", "tied", "toll", "trap", "wire"]
+    custom_stop_words: List = [
+        "ago",
+        "aim",
+        "amid",
+        "april",
+        "arch",
+        "bed",
+        "bite",
+        "bug",
+        "cage",
+        "co",
+        "crop",
+        "damage",
+        "danger",
+        "digit",
+        "et",
+        "fast",
+        "fat",
+        "fate",
+        "fire",
+        "flower",
+        "gap",
+        "genesis",
+        "gov",
+        "gpa",
+        "grasp",
+        "ii",
+        "inos",
+        "iv",
+        "killer",
+        "lab",
+        "lamp",
+        "laser",
+        "map",
+        "mask",
+        "mater",
+        "melt",
+        "mice",
+        "minor",
+        "miss",
+        "mv",
+        "nail",
+        "net",
+        "not",
+        "osf",
+        "pan",
+        "par",
+        "pha",
+        "rab",
+        "race",
+        "rain",
+        "rank",
+        "san",
+        "sand",
+        "se",
+        "sink",
+        "soft",
+        "spatial",
+        "spin",
+        "spp",
+        "steel",
+        "stop",
+        "storm",
+        "tactile",
+        "tau",
+        "theta",
+        "tip",
+        "traits",
+        "via",
+        "apex",
+        "app",
+        "apps",
+        "args",
+        "ash",
+        "bar",
+        "bit",
+        "cast",
+        "cats",
+        "cava",
+        "cd",
+        "clock",
+        "coil",
+        "cope",
+        "cord",
+        "delta",
+        "eat",
+        "eg",
+        "fats",
+        "fish",
+        "fix",
+        "flame",
+        "flap",
+        "fuse",
+        "grid",
+        "gum",
+        "heal",
+        "hip",
+        "hits",
+        "hub",
+        "igm",
+        "li",
+        "maps",
+        "mets",
+        "mix",
+        "mn",
+        "ms",
+        "nm",
+        "nodal",
+        "pigs",
+        "prey",
+        "pros",
+        "pt",
+        "pva",
+        "ray",
+        "sac",
+        "scar",
+        "sea",
+        "sea",
+        "sp",
+        "steep",
+        "tank",
+        "tied",
+        "toll",
+        "trap",
+        "wire",
+    ]
 
     search_terms_filename: str = "search_terms.txt"
-    
+
     filtered_terms_filename: str = "filtered_terms.txt"
-    
+
     abstract_inpath: str = "pubs/"
 
     abstract_updatefiles_inpath: str = "updates/"
     """ This path gets added on to abstract_inpath (or pub_inpath) """
-    
+
     refresh_abstract_xml_files: bool = False
     """ Set to True to overwrite downloaded NCBI XML abstract files and checksum files """
-    
+
     num_abstract_xml_files: int
     """ Number of NCBI XML files to download; Set this to -1 to get all abstracts """
-    
+
     abstract_outpath: str = "csvpubs/"
 
     abstract_length_threshold: int = 405
 
     abstract_genes_outpath: str = "genes/"
 
-    
-    #path functions
+    # path functions
     def raw_path(self):
         return os.path.join(os.getcwd(), self.version_root, self.raw_data_path)
+
     def reference_path(self):
         return os.path.join(os.getcwd(), self.version_root, self.reference_data_path)
+
     def dbxref_path(self):
-        return os.path.join(os.getcwd(), self.version_root, self.reference_data_path, self.dbxref_reference_data_path)
+        return os.path.join(
+            os.getcwd(),
+            self.version_root,
+            self.reference_data_path,
+            self.dbxref_reference_data_path,
+        )
+
     def search_path(self):
         return os.path.join(os.getcwd(), self.version_root, self.search_terms_path)
+
     def pub_inpath(self):
-        return os.path.join(os.getcwd(), self.version_root, self.raw_data_path, self.abstract_inpath)
+        return os.path.join(
+            os.getcwd(), self.version_root, self.raw_data_path, self.abstract_inpath
+        )
+
     def pub_outpath(self):
         return os.path.join(os.getcwd(), self.version_root, self.abstract_outpath)
+
     def genes_outpath(self):
         return os.path.join(self.pub_outpath(), self.abstract_genes_outpath)
 
     verbose: int = 0
     """ 0 prints nothing, 1 prints errors and warnings, 2 prints info """
-    
+
     debug: bool = False
     """ Prints very detailed debuggin messages """
-    
+
     version: str = None
     """ If None, version will e set to timestamp """
-    
+
     rand_seed: int = 42
-    """ if None, reproducible within the same release"""
-    
+    """ If None, reproducible within the same release"""
+
     version_root: str = None
-    """ leave this alone it will be computed as data_root/version """
-    
-    
+    """ Leave this alone it will be computed as data_root/version """
+
     @root_validator(pre=False, skip_on_failure=True)
     def valid_paths_for_data_tree(cls, v: Dict) -> Dict:
         data_root = v.get("data_root")
         version = v.get("version")
-        
+
         import os
-        
+
         if version is None:
             import subprocess
-            
+
             # use miliseconds and create new directory structure
-            version = str(subprocess.check_output(["date", "+%1N.%S_%M_%H_%Y_%m_%d"]).strip().decode())
+            version = str(
+                subprocess.check_output(["date", "+%1N.%S_%M_%H_%Y_%m_%d"])
+                .strip()
+                .decode()
+            )
             v["version"] = version
-        
+
         if data_root is None:
             raise Exception("Error: data_root cannot be None.")
-            
+
         version_root = os.path.join(os.getcwd(), data_root, str(version))
         v["version_root"] = version_root
-        
+
         if os.path.exists(version_root):
             msg2(f"Using existing data director {version_root}")
-            
+
         return v
-
```

### Comparing `gpubs-3/gpubs/parse.py` & `gpubs-4/gpubs/parse.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,93 +1,110 @@
-import pandas as pd
-import numpy as np
-import re
 import os
 
-from gpubs.log import msg1, msg2
+from gpubs.log import msg2
+
 
 def extract_data(element):
     data = {}
-    data['PMID'] = element.findtext('MedlineCitation/PMID')
-    data['Title'] = element.findtext('MedlineCitation/Article/ArticleTitle')
-    data['Abstract'] = element.findtext('MedlineCitation/Article/Abstract/AbstractText')
-    data['Journal'] = element.findtext('MedlineCitation/Article/Journal/Title')
-    data['PublicationDate'] = element.findtext('MedlineCitation/Article/Journal/JournalIssue/PubDate/Year')
-    data['JournalTitle'] = element.findtext('MedlineCitation/Article/Journal/Title')
-    data['ArticleType'] = element.findtext('MedlineCitation/Article/PublicationTypeList/PublicationType')
-    
+    data["PMID"] = element.findtext("MedlineCitation/PMID")
+    data["Title"] = element.findtext("MedlineCitation/Article/ArticleTitle")
+    data["Abstract"] = element.findtext("MedlineCitation/Article/Abstract/AbstractText")
+    data["Journal"] = element.findtext("MedlineCitation/Article/Journal/Title")
+    data["PublicationDate"] = element.findtext(
+        "MedlineCitation/Article/Journal/JournalIssue/PubDate/Year"
+    )
+    data["JournalTitle"] = element.findtext("MedlineCitation/Article/Journal/Title")
+    data["ArticleType"] = element.findtext(
+        "MedlineCitation/Article/PublicationTypeList/PublicationType"
+    )
+
     # Extract the descriptor names and qualifier names from the XML
-    mesh_headings = element.findall('.//MeshHeading')
+    mesh_headings = element.findall(".//MeshHeading")
     mesh_heading_list = []
     for heading in mesh_headings:
-        descriptor_name = heading.findtext('DescriptorName')
-        qualifier_names = [qualifier.text for qualifier in heading.findall('QualifierName')]
+        descriptor_name = heading.findtext("DescriptorName")
+        qualifier_names = [
+            qualifier.text for qualifier in heading.findall("QualifierName")
+        ]
         mesh_heading_list.append(descriptor_name)
         mesh_heading_list.extend(qualifier_names)
-    data['MeshHeadingList'] = ','.join(mesh_heading_list)
-                                        
-    publication_types = element.findall('MedlineCitation/Article/PublicationTypeList/PublicationType')
-    data['PublicationTypeList'] = ",".join([ptype.text for ptype in publication_types])
-    
+    data["MeshHeadingList"] = ",".join(mesh_heading_list)
+
+    publication_types = element.findall(
+        "MedlineCitation/Article/PublicationTypeList/PublicationType"
+    )
+    data["PublicationTypeList"] = ",".join([ptype.text for ptype in publication_types])
+
     return data
 
-def prune_df(df, length_threshold = 405, verbose=2):
+
+def prune_df(df, length_threshold=405, verbose=2):
     # exclude articles with no abstract, no date, or abstracts that are too short (less than length_threshold letters)
-    pruned_df = df[df['Abstract'].notna() & df['PublicationDate'].notna()]
+    pruned_df = df[df["Abstract"].notna() & df["PublicationDate"].notna()]
 
     # cut out any short articles
     all_pruned = len(pruned_df)
-    msg2(verbose, f"Number of all abstracts before pruning short articles = {all_pruned}")
-    pruned_df = pruned_df[pruned_df['Abstract'].str.len() >= length_threshold]
+    msg2(
+        verbose, f"Number of all abstracts before pruning short articles = {all_pruned}"
+    )
+    pruned_df = pruned_df[pruned_df["Abstract"].str.len() >= length_threshold]
     long_pruned = len(pruned_df)
     msg2(verbose, f"Number after pruning short articles = {long_pruned}")
     msg2(verbose, f"Number discarded for being too short: {all_pruned - long_pruned}")
 
     return pruned_df
 
-def get_pub_df(filename, inpath, outpath, length_threshold, prune=True,verbose=0):
+
+def get_pub_df(filename, inpath, outpath, length_threshold, prune=True, verbose=0):
     import gzip
     import xml.etree.ElementTree as ET
     import pandas as pd
 
     pubmed_filepath = os.path.join(inpath, filename)
     # Open the gzip'd XML file
-    with gzip.open(pubmed_filepath, 'rb') as f:
+    with gzip.open(pubmed_filepath, "rb") as f:
         # Read the contents of the gzip'd file
         gzip_content = f.read()
 
     # Parse the XML content using ElementTree
     root = ET.fromstring(gzip_content)
 
     # Extract data from each article and store in a list
     articles = []
-    for article in root.findall('.//PubmedArticle'):
+    for article in root.findall(".//PubmedArticle"):
         articles.append(extract_data(article))
 
     # Create a DataFrame from the list of articles
     df = pd.DataFrame(articles)
     df = df.drop_duplicates()
     if prune:
         msg2(verbose, f"Number of all articles:{len(df)}")
-        df = prune_df(df, length_threshold = length_threshold, verbose=verbose)
+        df = prune_df(df, length_threshold=length_threshold, verbose=verbose)
         msg2(verbose, f"Number of pruned articles:{len(df)}")
-    
+
     # convert objects to simple types
-    df['PublicationDate'] = df['PublicationDate'].astype(int)
+    df["PublicationDate"] = df["PublicationDate"].astype(int)
 
     return df
 
+
 def parse_pubs(inpath, outpath, length_threshold, csv_list, verbose=0):
     import glob
 
     for filepath in glob.glob(os.path.join(inpath, "pubmed*.xml.gz")):
         msg2(verbose, f"Converting file {filepath}")
         if os.path.isfile(filepath):
             filename = os.path.basename(filepath)
-            df = get_pub_df(filename=filename, inpath=inpath, outpath= outpath, prune=True, length_threshold = length_threshold, verbose = verbose)
+            df = get_pub_df(
+                filename=filename,
+                inpath=inpath,
+                outpath=outpath,
+                prune=True,
+                length_threshold=length_threshold,
+                verbose=verbose,
+            )
             csv_filepath = os.path.join(outpath, f"{filename}.csv")
             df.to_csv(csv_filepath, header=False, index=False, sep="\t")
             msg2(verbose, f"Wrote file:{csv_filepath}")
             csv_list.append(csv_filepath)
 
     return csv_list
-
```

### Comparing `gpubs-3/gpubs/reference.py` & `gpubs-4/gpubs/reference.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 from gpubs.log import msg2
 import requests
 
-def download_gene_symbols(output_filepath = "data/raw/gene_info.gz", url = "https://ftp.ncbi.nlm.nih.gov/gene/DATA/GENE_INFO/Mammalia/Homo_sapiens.gene_info.gz", verbose=0):
+
+def download_gene_symbols(
+    output_filepath="data/raw/gene_info.gz",
+    url="https://ftp.ncbi.nlm.nih.gov/gene/DATA/GENE_INFO/Mammalia/Homo_sapiens.gene_info.gz",
+    verbose=0,
+):
     response = requests.get(url)
     response.raise_for_status()
 
     with open(output_filepath, "wb") as file:
         file.write(response.content)
 
     msg2(verbose, "Download completed.")
 
-def extract_gene_data(filepath = "data/raw/gene_info.gz"):
-    """ returns 3 sets """
+
+def extract_gene_data(filepath="data/raw/gene_info.gz"):
+    """returns 3 sets"""
     import gzip
 
     gene_symbols = set()
     dbxrefs = set()
     gene_synonyms = set()
 
     with gzip.open(filepath, "rt") as file:
```

### Comparing `gpubs-3/gpubs/search_words.py` & `gpubs-4/gpubs/search_words.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,59 +1,61 @@
-from typing import List, Dict, Set
-
+from typing import Set
 import nltk
-from nltk import FreqDist
-import string
+
 
 def fetch_brown_corpus():
     from nltk.corpus import brown
-    corpus = 'brown'
+
+    corpus = "brown"
     # Select a specific category from the Brown Corpus for analysis
-    category = 'learned'
+    category = "learned"
     # Load the Brown Corpus
-    nltk.download('brown')
+    nltk.download(corpus)
     # Get the words from the selected category
     words = brown.words(categories=category)
     return words
 
+
 def read_search_stop(search_file, stop_words):
     # Load search terms from the file into a set
-    search_terms=[]
-    with open(search_file, 'r') as f:
+    search_terms = []
+    with open(search_file, "r") as f:
         search_terms = [line.strip() for line in f]
     return search_terms
 
+
 def filter_search_terms(search_terms, stop_words):
-    filtered_terms = []
+    filtered_terms = set()  # use a set to avoid duplicates
     matched_stop_words = []
-    
-    # get the matched stop words and keep in original case
+
     for term in search_terms:
         if term.lower() in stop_words:
+            # keep stop_words in original case
             matched_stop_words.append(term)
-
-    # get the filtered terms, lower case them
-    filtered_terms = [term.lower() for term in search_terms if term.lower() not in stop_words]
+        else:
+            # lower case non-stop_words for permissive matching
+            filtered_terms.add(term.lower())
 
     # add the two lists together so the matched terms retain original case
     # this will allow for finding genes that are also common english words
-    final_terms = filtered_terms + matched_stop_words
+    final_terms = list(filtered_terms) + matched_stop_words
     return (final_terms, filtered_terms, matched_stop_words)
 
+
 def create_stop_words(frequency_list_outpath, custom_words) -> Set:
     from nltk.corpus import stopwords
 
     # Download the stopwords corpus
-    nltk.download('stopwords')
+    nltk.download("stopwords")
 
     # Load the existing stop words
-    stop_words = set(stopwords.words('english'))
+    stop_words = set(stopwords.words("english"))
 
     # Read the words from the frequency_list.txt file
-    with open(frequency_list_outpath, 'r') as file:
+    with open(frequency_list_outpath, "r") as file:
         frequency_words = file.read().splitlines()
 
     # Add the frequency words to the stop words set
     stop_words.update(frequency_words)
 
     # Add custom words
     stop_words.update(custom_words)
```

### Comparing `gpubs-3/scripts/create_search_terms_file.sh` & `gpubs-4/scripts/create_search_terms_file.sh`

 * *Files identical despite different names*

### Comparing `gpubs-3/scripts/download_pubs.sh` & `gpubs-4/scripts/download_pubs.sh`

 * *Files identical despite different names*

### Comparing `gpubs-3/scripts/search.awk` & `gpubs-4/scripts/search.awk`

 * *Files identical despite different names*


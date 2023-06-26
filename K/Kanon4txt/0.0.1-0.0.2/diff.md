# Comparing `tmp/kanon4txt-0.0.1.tar.gz` & `tmp/Kanon4txt-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "Kanon4txt-0.0.2.tar", last modified: Mon Jun 26 09:23:06 2023, max compression
```

## Comparing `kanon4txt-0.0.1.tar` & `Kanon4txt-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,23 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kanon4txt-0.0.1/src/Kanon4txt/__init__.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 kanon4txt-0.0.1/src/Kanon4txt/example.py
--rw-r--r--   0        0        0     7265 2020-02-02 00:00:00.000000 kanon4txt-0.0.1/src/Kanon4txt/k_anonym_text.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kanon4txt-0.0.1/src/Kanon4txt/utils/__init__.py
--rw-r--r--   0        0        0    13225 2020-02-02 00:00:00.000000 kanon4txt-0.0.1/src/Kanon4txt/utils/anonym_utils.py
--rw-r--r--   0        0        0    13684 2020-02-02 00:00:00.000000 kanon4txt-0.0.1/src/Kanon4txt/utils/cluster_utils.py
--rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 kanon4txt-0.0.1/src/Kanon4txt/utils/llm_utils.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 kanon4txt-0.0.1/src/Kanon4txt/utils/models.py
--rw-r--r--   0        0        0    12844 2020-02-02 00:00:00.000000 kanon4txt-0.0.1/src/Kanon4txt/utils/nlp_utils.py
--rw-r--r--   0        0        0     5704 2020-02-02 00:00:00.000000 kanon4txt-0.0.1/src/Kanon4txt/utils/utilization_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kanon4txt-0.0.1/src/example_package_liortr30/__init__.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 kanon4txt-0.0.1/src/example_package_liortr30/example.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 kanon4txt-0.0.1/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 kanon4txt-0.0.1/LICENSE
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 kanon4txt-0.0.1/README.md
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 kanon4txt-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 kanon4txt-0.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-26 09:23:06.297793 Kanon4txt-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-06-26 09:23:06.240613 Kanon4txt-0.0.2/Kanon4txt/
+-rw-rw-rw-   0        0        0        0 2023-06-06 19:44:31.000000 Kanon4txt-0.0.2/Kanon4txt/__init__.py
+-rw-rw-rw-   0        0        0     8920 2023-06-26 07:43:27.000000 Kanon4txt-0.0.2/Kanon4txt/k_anonym_text.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:23:06.295611 Kanon4txt-0.0.2/Kanon4txt/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-27 08:18:12.000000 Kanon4txt-0.0.2/Kanon4txt/utils/__init__.py
+-rw-rw-rw-   0        0        0    19915 2023-06-19 08:12:01.000000 Kanon4txt-0.0.2/Kanon4txt/utils/anonym_utils.py
+-rw-rw-rw-   0        0        0    13766 2023-06-19 08:12:01.000000 Kanon4txt-0.0.2/Kanon4txt/utils/cluster_utils.py
+-rw-rw-rw-   0        0        0     7107 2023-06-19 08:12:01.000000 Kanon4txt-0.0.2/Kanon4txt/utils/llm_utils.py
+-rw-rw-rw-   0        0        0      485 2023-06-19 08:12:01.000000 Kanon4txt-0.0.2/Kanon4txt/utils/models.py
+-rw-rw-rw-   0        0        0    13040 2023-06-19 08:12:01.000000 Kanon4txt-0.0.2/Kanon4txt/utils/nlp_utils.py
+-rw-rw-rw-   0        0        0     6458 2023-06-19 08:12:01.000000 Kanon4txt-0.0.2/Kanon4txt/utils/utilization_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:23:06.277611 Kanon4txt-0.0.2/Kanon4txt.egg-info/
+-rw-rw-rw-   0        0        0      745 2023-06-26 09:23:06.000000 Kanon4txt-0.0.2/Kanon4txt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      463 2023-06-26 09:23:06.000000 Kanon4txt-0.0.2/Kanon4txt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 09:23:06.000000 Kanon4txt-0.0.2/Kanon4txt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      142 2023-06-26 09:23:06.000000 Kanon4txt-0.0.2/Kanon4txt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-26 09:23:06.000000 Kanon4txt-0.0.2/Kanon4txt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-06-06 20:01:19.000000 Kanon4txt-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      745 2023-06-26 09:23:06.298798 Kanon4txt-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4499 2023-06-21 09:41:31.000000 Kanon4txt-0.0.2/README.md
+-rw-rw-rw-   0        0        0       86 2023-06-26 09:23:06.304789 Kanon4txt-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1407 2023-06-26 09:22:22.000000 Kanon4txt-0.0.2/setup.py
```

### Comparing `kanon4txt-0.0.1/src/Kanon4txt/utils/cluster_utils.py` & `Kanon4txt-0.0.2/Kanon4txt/utils/cluster_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,37 +6,38 @@
 from kneed import KneeLocator
 import matplotlib.pyplot as plt
 #from nltk.corpus import stopwords
 from itertools import combinations
 import umap
 import hdbscan
 import sklearn.cluster as cluster
+import logging
 
 from . import models
-from . import nlp_utils
 
 # upload model:
 glove_model = models.glove_model
 
 def define_eps_cos(glove_model=glove_model):
     """Defines distance between pairs of words"""
     
     # Collecting distances of good pairs - cosine similarity
     sim_list_best = get_pairs_sim_cos(get_good_pairs(), glove_model)
-    print('mean similarity between good pairs\t', np.median(sim_list_best))
+    # print('mean similarity between good pairs\t', np.median(sim_list_best))
 
     # Collecting distances of bad pairs - cosine similarity
     sim_list_worst = get_pairs_sim_cos(get_bad_pairs(), glove_model)
-    print('mean similarity between bad pairs\t', np.median(sim_list_worst))
+    # print('mean similarity between bad pairs\t', np.median(sim_list_worst))
     
-    best_dist = 1 - np.mean(sim_list_best)
-    worst_dist = 1 - np.mean(sim_list_worst)
+    best_dist = 1 - np.median(sim_list_best)
+    worst_dist = 1 - np.median(sim_list_worst)
 
     # The  threshold for cluster max_dist should be in the middle of the two values above = 0.1765
     threshold = (best_dist + worst_dist)/2
+    
     return threshold
 
 
 def define_eps_euc(glove_model=glove_model):
     """Defines distance between pairs of words"""
     
     # Collecting distances of good pairs - Euclidean distance
@@ -67,15 +68,15 @@
         ['fast','quick'],
         ['big','huge'],
         ['item','product'],
         ['text','script'],
         ['john','julie'], # Adding names
         ['shirley','matthew'],
         ['joseph','smith'],
-        ['horton','sylvia'],
+        ['michael','sylvia'],
         ['bonnie','henry'],
         ['paul','jr'],
         ['duncan','kelly']]
     return best_pairs_ls
 
 
 def get_bad_pairs():
@@ -134,34 +135,34 @@
                 word_list.append(val['lemma'])
             else:
                 word_list.append(key)
             
     return list(set(word_list))  # Remove duplicates 
 
 
-def embed_corpus(word_dict):
+def embed_corpus(word_dict, stop_list):
     """ Embeds the corpus using glove """
 
     word_list = get_word_list_for_clustering(word_dict)
-    word_index = get_word_index_for_clustering(word_list)
+    word_index = get_word_index_for_clustering(word_list, stop_list)
 
     # Iterate over your dictionary of words and embed them using GloVe
     embedded_dict = {}
     for word, idx in word_index.items():
-        if word not in nlp_utils.stopword_list: # stopwords.words('english'):
+        if word not in stop_list: # stopwords.words('english'):
             try:
                 embedded_dict[word] = glove_model[word]
             except KeyError:
                 # If the word is not in the GloVe vocabulary, assign a default embedding or skip it
                 pass
     return embedded_dict
 
 
 def find_eps_val(embeddings, cosine = False):
-    """ Finds the EPS value for clustering """
+    """ Finds the EPS value for clustering based on knee """
 
     # Compute the k-distances for each point
     k = 10
     if cosine:
         neigh = NearestNeighbors(n_neighbors=k, metric = 'cosine')
     else:
         neigh = NearestNeighbors(n_neighbors=k)  # Using Euclidian distance
@@ -178,38 +179,39 @@
     # Find the elbow point
     kneedle = KneeLocator(range(len(sorted_distances)), sorted_distances, S=1.0, curve='concave', direction='increasing')
     eps = sorted_distances[kneedle.elbow]
 
     return eps
 
 
-def run_clustering(word_dict, cosine = False, eps = None):
+def run_clustering(word_dict, stop_list, cosine = False, eps = None, n_jobs = -1):
     """ Runs clustering """
     # point to think - min_points in cluster to be defined according to k?
     # Get embedding
-    embedded_dict = embed_corpus(word_dict)
+    embedded_dict = embed_corpus(word_dict, stop_list)
     # Convert to numpy array
     embeddings = np.array(list(embedded_dict.values()))
 
     if not eps:
         # Based on embedding distance / 2, since DBSCAN uses the epsilon as radius and not diameter.
         if cosine:
             eps = define_eps_cos() / 2
         else:
             eps = define_eps_euc() / 2 
             # eps = find_eps_val(embeddings, cosine=cosine)  # Based on knee method
+
+    logging.info(f'Pre-defined epsilon for DBSCAN: {eps}')
     
     # Chose 3 a min words per cluster (maybe reduce to 2?) Maybe according to k
     if cosine:
-        dbscan = DBSCAN(eps=eps, min_samples=2, metric='cosine') 
+        dbscan = DBSCAN(eps=eps, min_samples=2, metric='cosine', n_jobs=n_jobs) 
     else:
-        dbscan = DBSCAN(eps=eps, min_samples=2)  # Using Euclidian distance
+        dbscan = DBSCAN(eps=eps, min_samples=2, n_jobs=n_jobs)  # Using Euclidian distance
 
     dbscan.fit(embeddings)
-    print('epsilon\t', eps)
 
     labels = dbscan.labels_
     clusters = {}
     for i, key in enumerate(embedded_dict.keys()):
         cluster = labels[i]
         if cluster not in clusters:
             clusters[cluster] = []
@@ -308,20 +310,21 @@
     pca.fit(embeddings)
     X_pca = pca.transform(embeddings)
     plt.scatter(X_pca[:, 0], X_pca[:, 1], c=labels)
     plt.xlabel('PC1')
     plt.ylabel('PC2')
     plt.show()
 
-def get_word_index_for_clustering(all_words):
+
+def get_word_index_for_clustering(all_words, stop_list):
     """ Uses tokenizer to get word indexes """
     word_index = {}
     i = 0
     for word in all_words:
-        if word and (word not in nlp_utils.stopword_list): #  stopwords.words('english')):
+        if word and (word not in stop_list): #  stopwords.words('english')):
             word_index[word] = i
             i += 1
 
     return word_index
 
 
 def run_clustering_hdbscan(embedded_dict):
@@ -364,15 +367,14 @@
     """
     # NOT INCLUSING CLUSTER -1
     size_list = []
     copy_clusters = clusters
     if -1 in copy_clusters:
         del copy_clusters[-1]
 
-    print(len(copy_clusters), 'clusters')
     for l in copy_clusters.values():
       #print(l)
       if l == -1:
         continue
       else:
         size_list.append(len(l))
```

### Comparing `kanon4txt-0.0.1/src/Kanon4txt/utils/nlp_utils.py` & `Kanon4txt-0.0.2/Kanon4txt/utils/nlp_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,50 @@
 # Imports
 import pandas as pd
 import numpy as np
 import re
 from nltk.corpus import stopwords
-import matplotlib.pyplot as plt
+from nltk.tokenize import word_tokenize
 import spacy
 import re
 import bz2
 from collections import defaultdict
 import operator
+import logging
 from . import models
 
-# nltk.download('stopwords')
-
+# Defining some global variables
 stopword_list = None
 
+short_stopword_list = None
+long_stopword_list = None
 
-# Defining some global variables
 nlp = spacy.load('en_core_web_sm', disable=['ner', 'parser'])  # disabling Named Entity Recognition for speed
 glove_model = models.glove_model
 
+def get_list_from_file(file_name):
+    """"
+    Reads a file with words (each word on different line) and returns a list of these words.
+    """
+    try:
+        with open(file_name, 'r') as file:
+            
+            # reading the file
+            data = file.read()
+            
+            # replacing end splitting the text 
+            # when newline ('\n') is seen.
+            word_list = data.split("\n")
+    
+    except Exception as e:
+        logging.error(f'Could not read the file {file_name}: {e}')
+        word_list = None
+    return word_list
+
+
 def init_stopwords(file=None):
     """
     Initialized the stopword list
     """
     global stopword_list
 
     stopword_list = stopwords.words('english')
@@ -96,53 +117,71 @@
         jaccard = intersection / union
     else:
         # print('Warning: jaccard_index union = 0', sentence1, sentence2)
         jaccard = 0
     return jaccard
 
 
-def get_voc(corpus):
+def get_voc0(corpus):
     """ Gets corpus voccabulary """
     word_set = set([])
 
     for doc in corpus:
         doc = doc.split(' ')
         for word in doc:
             word_set.add(word)
     return word_set
 
 
+def get_voc(corpus):
+    """
+    Creates a set of unique words in a given corpus
+    """
+    word_set = set([])
+
+    for doc in corpus:
+            doc_words = set(word_tokenize(doc))
+            word_set = word_set.union(doc_words)
+    return word_set
+
+
 def get_lemma(word, nlp=nlp):
     """ Returns the lemma of the given word """
     word = nlp(word)
     txt = [token.lemma_ for token in word]
     lemma = txt[0]
     return lemma
 
 
-def create_word_dict(corpus):
+def create_word_dict(corpus, stop_list):
     """ Creates a word dictionary. Keys = words. Values = three boolians - stop/lemma/replaced"""
 
     all_words = get_voc(corpus)
 
+    logging.info('Got vocabulary')
+
     all_word_dict = {}
 
     for word in all_words:
         # Cleaning non AB characters
         word = replace_non_ab_chars(word)
+
+        # Creating the word dictionary
         word_dict = {
             'protected': None,
             'lemma': None,
             'replaced': None}
         if len(word) > 0:
-            if word in stopword_list:
+            if word in stop_list:
                 word_dict['protected'] = True
-            elif get_lemma(word) != word:
-                word_dict['lemma'] = get_lemma(word)
-            all_word_dict[word] = word_dict
+            else:
+                lemma = get_lemma(word)
+                if  lemma != word:
+                    word_dict['lemma'] = lemma
+                all_word_dict[word] = word_dict
 
     return all_word_dict
 
 
 def print_doc(doc, all_word_dict):
     """ Prints document based on the word dictionary """
     # out_str = 'Legend: (protected) [replaced] {lemmatized}\n'
@@ -165,20 +204,17 @@
 
 
 def replace_non_ab_chars(word):
     word = re.sub("[^A-Za-z']+", '', str(word)).lower()
     return word
 
 
-
-def cleaning(doc, break_doc=False):
+def cleaning(doc, stop_list):
     """Lemmatizing and removes stopwords"""
     # Defining the document
-    if break_doc:
-        doc = doc.replace(' ', '. ' )
     if doc:
         doc = nlp(doc)
 
         # Lemmatizes and removes stopwords
 
         # For some reason, sometimes the lemmatization is not consistent - 
         # identical words receive a different lemmatization (for example, acting is sometimes 
@@ -186,36 +222,35 @@
         # Apperantly, Spacy's lemmatization depends on the part of speech: 
         # https://stackoverflow.com/a/74176351
         # To overcome this, we added the break_doc parameter
 
         txt = []
         for token in doc:
             word = re.sub('\W+', '', str(token)).lower()
-            if word and (word not in stopword_list):
+            if word and (word not in stop_list):
                 txt.append(token.lemma_)
     
         clean_doc = ' '.join(txt)
     else:
         clean_doc = doc
 
     return clean_doc
 
 
-def lemmatize_doc(doc, break_doc=False):
+def lemmatize_doc(doc, stop_list):
     """Lemmatizes document"""
     # Breaking the document to allow consistent lemmatization (see function cleaning())
-    if break_doc:
-        doc = doc.replace(' ', '. ' )
+
     doc = nlp(doc)
 
     # Lemmatizes and removes stopwords
     # doc needs to be a spacy Doc object
     txt = []
     for token in doc:
-        if str(token) in stopword_list:  # Add stopword as it is
+        if str(token) in stop_list:  # Add stopword as it is
             txt.append(str(token))
         else:  # Lemmatize other words
             txt.append(token.lemma_)
     clean_doc = ' '.join(txt)
 
     return clean_doc
 
@@ -241,115 +276,108 @@
                 doc1_neighbors.append(jaccard_index(doc1, doc2))
         doc1_neighbors.sort(reverse=True)
         all_neighbors += doc1_neighbors[:k]
     avg = np.average(all_neighbors)
     return avg
 
 
-def plot_jaccard_hist(df_short_sentences, column = 'txt'):
-    """creat a hist of jaccard scores"""
-
-    indices_list = list(df_short_sentences.index)
-    indices_list_short_1 = indices_list
-
-    # Create a list of sentence texts
-    sentences = list(df_short_sentences[column].loc[indices_list_short_1])
-
-    # Compute the Jaccard index for all pairs of sentences
-    jaccard_index_dict = {(indices_list_short_1[i], indices_list_short_1[j]): jaccard_index(sentences[i], sentences[j])
-                          for i in range(len(sentences)) for j in range(i + 1, len(sentences))}
-
-    # Sort the dictionary by its values in descending order
-    sorted_dict = dict(sorted(jaccard_index_dict.items(), key=lambda item: item[1], reverse=True))
-    print(sorted_dict)
-    # extract the values from the dictionary
-    dic_values = list(sorted_dict.values())
-
-    # plot a histogram of the values
-    plt.hist(dic_values, bins=50, range=(0, 0.3))
-
-    # set labels and title
-    plt.xlabel('Values')
-    plt.ylabel('Counts')
-    plt.title('Histogram of Jaccard Indecs')
-
-    # display the plot
-    plt.show()
-
-
 def get_general_word_from_cluster(word_list, we_model):
     """ Finds the most similar words usind word embedding"""
-    # glove_words = list(we_model.index_to_key)
-    # For W2V
-    # known_words = [w for w in word_list if w in we_model.vocab]
-    # For GLOVE
-    known_words = [w for w in word_list if w in we_model.index_to_key]
-    print('known words:', len(known_words), 'word_list', len(word_list))
+    try:
+        # For W2V
+        known_words = [w for w in word_list if w in we_model.vocab]
+    except:
+        # For GloVe
+        known_words = [w for w in word_list if w in we_model.index_to_key]
+    word_vecs = []
+    for w in known_words:
+        word_vecs.append(we_model[w])
+    word_vecs = np.array(word_vecs)
+    
+    # Finding the centorid
+    centroid = np.mean(word_vecs, axis=0)
+
+    # print('known words:', len(known_words), 'word_list', len(word_list))
     if len(known_words) > 0:
-        we_word = we_model.most_similar(known_words, topn=1)[0][0]
+        # we_word = we_model.most_similar(known_words, topn=1)[0][0]
+        we_word = we_model.most_similar([centroid], topn=1)[0][0]
     else:
         we_word = None
     return we_word
 
 
 def add_general_word_to_word_dict(word_dict, word):
     """ Updating that the given words were replaced """
     word_dict[word] = {
         'protected': False,
         'lemma': False,
         'replaced': True}
     return word_dict
 
 
-def replace_words_in_df(df_0, cluster_dict, distance_dict, word_dict_0, update_stop=True):
+def replace_words_in_df(df_0, cluster_dict, distance_dict, word_dict_0, update_stop=True, prefix=None):
     """ Replaces the words in the dataframe """
 
-    global stopword_list
+    # global stopword_list
+    global long_stopword_list
+
+    if prefix:
+        output_file = f'outputs/{prefix}_replacements.txt'
+        f = open(output_file, "a")
+        f.write(f'\nUsing model {models.model_name}\nNumber of clusters: {len(cluster_dict)}\n # Protected words: {len(long_stopword_list)}\n')
+
 
     # Working with a copy of the df:
     df_copy = df_0
     word_dict_copy = word_dict_0.copy()
 
-    df_copy['anon_txt'] = df_copy['txt'].apply(lambda x: lemmatize_doc(x))
+    df_copy['anon_txt'] = df_copy['txt'].apply(lambda x: lemmatize_doc(x, stop_list=long_stopword_list))
+
+    logging.info('Going over clusters')
 
     for key, words in cluster_dict.items():
         if key >= 0:  # Ignoring the -1 label
             #if len(cluster_dict[key]) < 20:  # so it will make sense!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
             # Getting the general word
-            general_word = get_general_word_from_cluster(words, glove_model)
+            general_word = get_general_word_from_cluster(words, glove_model).lower()
 
-            if update_stop and (general_word not in stopword_list):
-                stopword_list.append(general_word)  # the list of new words
-            print('distance:', distance_dict[key], '\tcluster size:', len(words),'\treplacing', words, 'in', general_word)
+            if update_stop and (general_word not in long_stopword_list):
+                long_stopword_list.append(general_word)  # the list of new words
+            rep_str = f'distance: {distance_dict[key]} \tcluster size: {len(words)} \treplacing {words} in {general_word}'
+            logging.debug(rep_str)
+            # TEMP
+            if prefix:
+                f.write(rep_str + '\n')
+
+            # print('distance:', distance_dict[key], '\tcluster size:', len(words),'\treplacing', words, 'in', general_word)
             words_to_replace = []
             for word in words:
                 if word not in word_dict_copy:  # Lemmatized word
                     word_dict_copy[word] = {'protected': False, 'lemma': word, 'replaced':False}
                     
                 if not word_dict_copy[word]['protected']:
                     # Updaing the word dictionary that the words were replaced
                     word_dict_copy[word]['replaced'] = general_word  # Problem: greate in line 2 miss-identified as replaced
                 
-                df_copy['anon_txt'] = df_copy['anon_txt'].replace(fr'\b{word}\b', general_word, regex=True)
+                # df_copy['anon_txt'] = df_copy['anon_txt'].replace(fr'\b{word}\b', general_word, regex=True)
                 
                 words_to_replace.append(word)
 
             # Replacing whole words
-            # rep_str = '\b|\b'.join(words_to_replace)
-            # df_copy['anon_txt'] = df_copy['anon_txt'].replace(fr'\b{rep_str}\b', general_word, regex=True)
+            rep_str = '\b|\b'.join(words_to_replace)
+            df_copy['anon_txt'] = df_copy['anon_txt'].replace(fr'\b{rep_str}\b', general_word, regex=True)
 
-    # print('Final average Jaccard index:', get_average_jaccard(df_copy['anon_txt'], k=k))
+    logging.info('Creating history')
     df_copy['anon_txt_history'] = df_copy['txt'].apply(lambda x: print_doc(x, word_dict_copy))
-    # df_copy['num_replaced'] = df_copy['anon_txt_history'].apply(lambda x: len(re.findall(r'\[\w+\]', x)))
-    # df_copy['num_lemmatized'] = df_copy['anon_txt_history'].apply(lambda x: len(re.findall(r'\{\w+\}', x)))
-    # df_copy['num_protected'] = df_copy['anon_txt_history'].apply(lambda x: len(re.findall(r'\(\w+\)', x)))
-    # df_copy['num_no_change'] = df_copy['num_of_words'] - df_copy['num_replaced'] - df_copy['num_lemmatized'] - df_copy['num_protected']
 
     if update_stop:
-        print('Stop word list was updated')
+        logging.info('Stop word list was updated')
+    
+    if prefix:
+        f.close()
 
     return df_copy, word_dict_copy
 
 
 def get_stat(word_dict):
     """
     Returns the number of stop words, lemmatized and replaced words
```

### Comparing `kanon4txt-0.0.1/src/Kanon4txt/utils/utilization_utils.py` & `Kanon4txt-0.0.2/Kanon4txt/utils/utilization_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,66 @@
 # required imports
 from transformers import pipeline
 from sklearn.naive_bayes import MultinomialNB
 from sklearn.model_selection import train_test_split
 from sklearn.feature_extraction.text import CountVectorizer
 from sklearn.model_selection import cross_val_score
+# from sklearn.metrics.pairwise import cosine_similarity
+from scipy.spatial.distance import cosine
 import numpy as np
 import xgboost as xgb
 import matplotlib.pyplot as plt
 import numpy as np
 from numpy.linalg import norm
 from sentence_transformers import SentenceTransformer
+import logging
 
 from . import models
 
 analyzer = models.analyzer
 
-def get_mean_semantice_distance_for_corpus(cor1, cor2, prefix):
+def get_mean_semantice_distance_for_corpus(cor1, cor2, prefix=None):
     """
     Calculates the distance for each pair of documents
     """
     sem_model = SentenceTransformer('sentence-transformers/all-MiniLM-L12-v1')
+    cor1_embed = sem_model.encode(cor1, show_progress_bar=False)
+    cor2_embed = sem_model.encode(cor2, show_progress_bar=False)
+
     if len(cor1) != len(cor2):
-        print('Error: the two copuses must be in the same size.')
+        logging.error('The two copuses must be in the same size.')
         return
-    dist_list = []
-    for doc1, doc2 in zip(cor1, cor2):
-        dist_list.append(get_semantice_distance_for_docs(doc1, doc2, sem_model))
-    mean_dist = np.mean(dist_list)
+    
+    # dist_list = embedded_dist(cor1_embed, cor2_embed)
+    # dist_list = cosine(cor1_embed, cor2_embed)
+    # print('dist_list:', dist_list.shape)
+    # # compute cosine similarity
+    cosine_sim = np.sum(cor1_embed * cor2_embed, axis=1)/(norm(cor1_embed, axis=1)*norm(cor2_embed, axis=1))
+    cosine_dist = 1 - cosine_sim
+    
+    # print('cosine_dist:', cosine_dist.shape)
+    # dist_list = []
+    #
+    # for doc1, doc2 in zip(cor1, cor2):
+    #     dist_list.append(get_semantice_distance_for_docs(doc1, doc2, sem_model))
+    mean_dist = np.mean(cosine_dist)
 
     # Plotting a histogram
-    plot_hist(data=dist_list, xlabel='Semantic Distance', fig_name=f'plots/{prefix}.pdf')
+    if prefix:
+        plot_hist(data=cosine_dist, xlabel='Semantic Distance', fig_name=f'plots/{prefix}_semantic_hist.pdf')
+    
     return mean_dist
 
 
 def get_semantice_distance_for_docs(doc1, doc2, sem_model):
     """
     Generates sentence embedding and calculates the distance between them
     """
-    embed1 = sem_model.encode(doc1)
-    embed2 = sem_model.encode(doc2)
+    embed1 = sem_model.encode(doc1, show_progress_bar=False)
+    embed2 = sem_model.encode(doc2, show_progress_bar=False)
     dist = embedded_dist(embed1, embed2)
     return dist
 
 
 def plot_hist(data, xlabel, fig_name):
     """
     Plots a histogram and saves it.
```

### Comparing `kanon4txt-0.0.1/LICENSE` & `Kanon4txt-0.0.2/LICENSE`

 * *Files identical despite different names*


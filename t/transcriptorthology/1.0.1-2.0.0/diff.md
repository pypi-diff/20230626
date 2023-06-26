# Comparing `tmp/transcriptorthology-1.0.1.tar.gz` & `tmp/transcriptorthology-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/transcriptorthology-1.0.1.tar", last modified: Mon Mar 20 00:11:13 2023, max compression
+gzip compressed data, was "dist/transcriptorthology-2.0.0.tar", last modified: Mon Jun 26 04:17:55 2023, max compression
```

## Comparing `transcriptorthology-1.0.1.tar` & `transcriptorthology-2.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ouew2201 (1811316550) domain^users (1810891265)        0 2023-03-20 00:11:13.000000 transcriptorthology-1.0.1/
-drwxr-xr-x   0 ouew2201 (1811316550) domain^users (1810891265)        0 2023-03-20 00:11:13.000000 transcriptorthology-1.0.1/transcriptorthology/
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)    19439 2023-03-19 23:39:12.000000 transcriptorthology-1.0.1/transcriptorthology/tsmComputing.py
--rw-------   0 ouew2201 (1811316550) domain^users (1810891265)      121 2023-03-03 21:12:23.000000 transcriptorthology-1.0.1/transcriptorthology/__init__.py
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     2913 2023-03-03 21:11:09.000000 transcriptorthology-1.0.1/transcriptorthology/transcriptOrthology.py
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)    15634 2023-03-01 01:29:49.000000 transcriptorthology-1.0.1/transcriptorthology/Tclustering.py
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     1053 2023-03-20 00:10:40.000000 transcriptorthology-1.0.1/setup.py
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)      761 2023-03-20 00:11:13.000000 transcriptorthology-1.0.1/PKG-INFO
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)       38 2023-03-20 00:11:13.000000 transcriptorthology-1.0.1/setup.cfg
-drwxr-xr-x   0 ouew2201 (1811316550) domain^users (1810891265)        0 2023-03-20 00:11:13.000000 transcriptorthology-1.0.1/transcriptorthology.egg-info/
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)        1 2023-03-20 00:11:13.000000 transcriptorthology-1.0.1/transcriptorthology.egg-info/dependency_links.txt
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)      368 2023-03-20 00:11:13.000000 transcriptorthology-1.0.1/transcriptorthology.egg-info/SOURCES.txt
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)       41 2023-03-20 00:11:13.000000 transcriptorthology-1.0.1/transcriptorthology.egg-info/requires.txt
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)      761 2023-03-20 00:11:13.000000 transcriptorthology-1.0.1/transcriptorthology.egg-info/PKG-INFO
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)       20 2023-03-20 00:11:13.000000 transcriptorthology-1.0.1/transcriptorthology.egg-info/top_level.txt
+drwxr-xr-x   0 ouew2201 (1811316550) domain^users (1810891265)        0 2023-06-26 04:17:55.000000 transcriptorthology-2.0.0/
+drwxr-xr-x   0 ouew2201 (1811316550) domain^users (1810891265)        0 2023-06-26 04:17:55.000000 transcriptorthology-2.0.0/transcriptorthology/
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)    23446 2023-06-26 04:15:24.000000 transcriptorthology-2.0.0/transcriptorthology/tsmComputing.py
+-rw-------   0 ouew2201 (1811316550) domain^users (1810891265)      121 2023-03-03 21:12:23.000000 transcriptorthology-2.0.0/transcriptorthology/__init__.py
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     2911 2023-06-26 04:15:32.000000 transcriptorthology-2.0.0/transcriptorthology/transcriptOrthology.py
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)    15635 2023-06-26 04:15:41.000000 transcriptorthology-2.0.0/transcriptorthology/Tclustering.py
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     1053 2023-06-26 04:09:28.000000 transcriptorthology-2.0.0/setup.py
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)      761 2023-06-26 04:17:55.000000 transcriptorthology-2.0.0/PKG-INFO
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)       38 2023-06-26 04:17:55.000000 transcriptorthology-2.0.0/setup.cfg
+drwxr-xr-x   0 ouew2201 (1811316550) domain^users (1810891265)        0 2023-06-26 04:17:55.000000 transcriptorthology-2.0.0/transcriptorthology.egg-info/
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)        1 2023-06-26 04:17:55.000000 transcriptorthology-2.0.0/transcriptorthology.egg-info/dependency_links.txt
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)      368 2023-06-26 04:17:55.000000 transcriptorthology-2.0.0/transcriptorthology.egg-info/SOURCES.txt
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)       41 2023-06-26 04:17:55.000000 transcriptorthology-2.0.0/transcriptorthology.egg-info/requires.txt
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)      761 2023-06-26 04:17:55.000000 transcriptorthology-2.0.0/transcriptorthology.egg-info/PKG-INFO
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)       20 2023-06-26 04:17:55.000000 transcriptorthology-2.0.0/transcriptorthology.egg-info/top_level.txt
```

### Comparing `transcriptorthology-1.0.1/transcriptorthology/tsmComputing.py` & `transcriptorthology-2.0.0/transcriptorthology/tsmComputing.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,20 +6,21 @@
 > Reference:
 ======
     https://github.com/UdeS-CoBIUS/TranscriptOrthology
 """
 __authors__ = ("Wend Yam Donald Davy Ouedraogo")
 __contact__ = ("wend.yam.donald.davy.usherbrooke.ca")
 __copyright__ = "CoBIUS lab at Université de Sherbrooke, QC, CANADA"
-__date__ = "2022-12-19"
-__version__= "1.0.2"
+__date__ = "2023-06-26"
+__version__= "2.0.0"
 
 import pandas as pd
 import argparse
 import time
+import numpy as np
 
 def build_arg_parser():
     '''Parsing function'''
     parser = argparse.ArgumentParser(description="parsor program parameter")
     parser.add_argument('-talg', '--tralignment', default=None)
     parser.add_argument('-gtot', '--genetotranscripts', default=None)
     parser.add_argument('-tsm', '--tsmvalue', default=False)
@@ -215,85 +216,161 @@
         ##### arg4 : Pandas DataFrame = {columns=['id_transcript', 'blocks']} containing ids of transcripts and their representation into blocks
         ##### arg5 : Pandas DataFrame = {columns=['id_gene', 'blocks']} containing ids of genes and their representation into blocks
         ##### arg6 : Bool : True | False. if True compute the tsm otherwise tsm+.
         --- 
         Returns the matrix similarity score
     """
     transcripts = list(df_transcripts['id_transcript'].values)
-    matrix = []
+    matrix = np.zeros((len(transcripts), len(transcripts)))
     tsm_condition = int(tsm_condition)
+    used_indice = {}
 
     if tsm_condition == 1:
         """ tsm+unitary"""
-        for transcript_1 in transcripts:
-            row = []
-            for transcript_2 in transcripts:
-                # Compute the nucHOM score (unitary)
-                score_nuc_hom = round(compute_nuchom_score(transcript_1, transcript_2, df_transcripts),3)
-                row.append(score_nuc_hom)
-            matrix.append(row)
+        for i, transcript_1 in enumerate(transcripts):
+            for j, transcript_2 in enumerate(transcripts):
+                if transcript_1 == transcript_2:
+                    matrix[i,j] = 1.0
+                else:
+                    indice1 = transcript_1+'&'+transcript_2
+                    indice2 = transcript_2+'&'+transcript_1
+                    if indice1 not in list(used_indice.keys()) and indice2 not in list(used_indice.keys()):
+                        # Compute the nucHOM score (unitary)
+                        score_nuc_hom = round(compute_nuchom_score(transcript_1, transcript_2, df_transcripts),3)
+                        matrix[i, j] = score_nuc_hom
+                        used_indice[indice1] = score_nuc_hom
+                        used_indice[indice2] = score_nuc_hom
+                    else :
+                        matrix[i, j] = used_indice[indice1]
     elif tsm_condition == 2:
         """ tsm+length"""
-        for transcript_1 in transcripts:
-            row = []
-            for transcript_2 in transcripts:
-                # Compute the DegHOM score (length)
-                score_deg_hom = round(compute_deghom_score(transcript_1, transcript_2, df_blocks_transcripts),3)
-                row.append(score_deg_hom)
-            matrix.append(row)
+        for i, transcript_1 in enumerate(transcripts):
+            for j, transcript_2 in enumerate(transcripts):
+                if transcript_1 == transcript_2:
+                    matrix[i,j] = 1.0
+                else:
+                    indice1 = transcript_1+'&'+transcript_2
+                    indice2 = transcript_2+'&'+transcript_1
+                    if indice1 not in list(used_indice.keys()) and indice2 not in list(used_indice.keys()):
+                        # Compute the nucHOM score (unitary)
+                        score_deg_hom = round(compute_deghom_score(transcript_1, transcript_2, df_blocks_transcripts),3)
+                        matrix[i, j] = score_deg_hom
+                        used_indice[indice1] = score_deg_hom
+                        used_indice[indice2] = score_deg_hom
+                    else :
+                        matrix[i, j] = used_indice[indice1]
     elif tsm_condition == 3:
         """ tsm+mean"""
-        for transcript_1 in transcripts:
-            row = []
-            for transcript_2 in transcripts:
-                # Compute the nucHOM score (unitary)
-                score_nuc_hom = round(compute_nuchom_score(transcript_1, transcript_2, df_transcripts),3)
-                # Compute the DegHOM score (length)
-                score_deg_hom = round(compute_deghom_score(transcript_1, transcript_2, df_blocks_transcripts),3)
-                # Compute tsm (mean)
-                score = round(((score_nuc_hom+score_deg_hom)/2),3)
-                row.append(score)
-            matrix.append(row)
+        for i, transcript_1 in enumerate(transcripts):
+            for j, transcript_2 in enumerate(transcripts):
+                if transcript_1 == transcript_2:
+                    matrix[i,j] = 1.0
+                else:
+                    indice1 = transcript_1+'&'+transcript_2
+                    indice2 = transcript_2+'&'+transcript_1
+                    if indice1 not in list(used_indice.keys()) and indice2 not in list(used_indice.keys()):
+                        # Compute the nucHOM score (unitary)
+                        score_nuc_hom = round(compute_nuchom_score(transcript_1, transcript_2, df_transcripts),3)
+                        # Compute the DegHOM score (length)
+                        score_deg_hom = round(compute_deghom_score(transcript_1, transcript_2, df_blocks_transcripts),3)
+                        # Compute tsm (mean)
+                        score = round(((score_nuc_hom+score_deg_hom)/2),3)
+                        matrix[i, j] = score
+                        used_indice[indice1] = score
+                        used_indice[indice2] = score
+                    else :
+                        matrix[i, j] = used_indice[indice1]
     elif tsm_condition == 4:
         """ tsm++unitary"""
-        for transcript_1 in transcripts:
-            row = []
-            for transcript_2 in transcripts:
-                gene_tr_1 = df_gtot[df_gtot['id_transcript'] == transcript_1].id_gene.values[0]
-                gene_tr_2 = df_gtot[df_gtot['id_transcript'] == transcript_2].id_gene.values[0]
-                score_nuc_hom_v2 = round(compute_nuchom_score_tsmplus(transcript_1, transcript_2, df_transcripts, gene_tr_1, gene_tr_2, df_gtot),3)
-                row.append(score_nuc_hom_v2)
-            matrix.append(row)
+        gene_model = get_gene_model(df_gtot, df_transcripts)
+        for i, transcript_1 in enumerate(transcripts):
+            for j, transcript_2 in enumerate(transcripts):
+                if transcript_1 == transcript_2:
+                    matrix[i,j] = 1.0
+                else:
+                    indice1 = transcript_1+'&'+transcript_2
+                    indice2 = transcript_2+'&'+transcript_1
+                    if indice1 not in list(used_indice.keys()) and indice2 not in list(used_indice.keys()):
+                        gene_tr_1 = df_gtot[df_gtot['id_transcript'] == transcript_1].id_gene.values[0]
+                        gene_tr_2 = df_gtot[df_gtot['id_transcript'] == transcript_2].id_gene.values[0]
+                        score_nuc_hom_v2 = round(compute_nuchom_score_tsmplus(transcript_1, transcript_2, df_transcripts, gene_tr_1, gene_tr_2, gene_model),3)
+                        matrix[i, j] = score_nuc_hom_v2
+                        used_indice[indice1] = score_nuc_hom_v2
+                        used_indice[indice2] = score_nuc_hom_v2
+                    else :
+                        matrix[i, j] = used_indice[indice1]
     elif tsm_condition == 5:
         """ tsm++length"""
-        for transcript_1 in transcripts:
-            row = []
-            for transcript_2 in transcripts:
-                gene_tr_1 = df_gtot[df_gtot['id_transcript'] == transcript_1].id_gene.values[0]
-                gene_tr_2 = df_gtot[df_gtot['id_transcript'] == transcript_2].id_gene.values[0]
-                score_deg_hom_v2 = round(compute_deghom_score_tsmplus(transcript_1, transcript_2, df_blocks_transcripts, df_blocks_genes, gene_tr_1, gene_tr_2),3)
-                row.append(score_deg_hom_v2)
-            matrix.append(row)
+        for i, transcript_1 in enumerate(transcripts):
+            for j, transcript_2 in enumerate(transcripts):
+                if transcript_1 == transcript_2:
+                    matrix[i,j] = 1.0
+                else:
+                    indice1 = transcript_1+'&'+transcript_2
+                    indice2 = transcript_2+'&'+transcript_1
+                    if indice1 not in list(used_indice.keys()) and indice2 not in list(used_indice.keys()):
+                        gene_tr_1 = df_gtot[df_gtot['id_transcript'] == transcript_1].id_gene.values[0]
+                        gene_tr_2 = df_gtot[df_gtot['id_transcript'] == transcript_2].id_gene.values[0]
+                        score_deg_hom_v2 = round(compute_deghom_score_tsmplus(transcript_1, transcript_2, df_blocks_transcripts, df_blocks_genes, gene_tr_1, gene_tr_2),3)
+                        matrix[i, j] = score_deg_hom_v2
+                        used_indice[indice1] = score_deg_hom_v2
+                        used_indice[indice2] = score_deg_hom_v2
+                    else :
+                        matrix[i, j] = used_indice[indice1]
     elif tsm_condition == 6:
         """ tsm++mean"""
-        for transcript_1 in transcripts:
-            row = []
-            for transcript_2 in transcripts:
-                gene_tr_1 = df_gtot[df_gtot['id_transcript'] == transcript_1].id_gene.values[0]
-                gene_tr_2 = df_gtot[df_gtot['id_transcript'] == transcript_2].id_gene.values[0]
-                score_nuc_hom_v2 = round(compute_nuchom_score_tsmplus(transcript_1, transcript_2, df_transcripts, gene_tr_1, gene_tr_2, df_gtot),3)
-                score_deg_hom_v2 = round(compute_deghom_score_tsmplus(transcript_1, transcript_2, df_blocks_transcripts, df_blocks_genes, gene_tr_1, gene_tr_2),3)
-                score_tsmplus = round(((score_nuc_hom_v2+score_deg_hom_v2)/2),3)
-                row.append(score_tsmplus)
-            matrix.append(row)
+        gene_model = get_gene_model(df_gtot, df_transcripts)
+        for i, transcript_1 in enumerate(transcripts):
+            for j, transcript_2 in enumerate(transcripts):
+                if transcript_1 == transcript_2:
+                    matrix[i,j] = 1.0
+                else:
+                    indice1 = transcript_1+'&'+transcript_2
+                    indice2 = transcript_2+'&'+transcript_1
+                    if indice1 not in list(used_indice.keys()) and indice2 not in list(used_indice.keys()):
+                        gene_tr_1 = df_gtot[df_gtot['id_transcript'] == transcript_1].id_gene.values[0]
+                        gene_tr_2 = df_gtot[df_gtot['id_transcript'] == transcript_2].id_gene.values[0]
+                        score_nuc_hom_v2 = round(compute_nuchom_score_tsmplus(transcript_1, transcript_2, df_transcripts, gene_tr_1, gene_tr_2, gene_model),3)
+                        score_deg_hom_v2 = round(compute_deghom_score_tsmplus(transcript_1, transcript_2, df_blocks_transcripts, df_blocks_genes, gene_tr_1, gene_tr_2),3)
+                        score_tsmplus = round(((score_nuc_hom_v2+score_deg_hom_v2)/2),3)
+                        matrix[i, j] = score_tsmplus
+                        used_indice[indice1] = score_tsmplus
+                        used_indice[indice2] = score_tsmplus
+                    else :
+                        matrix[i, j] = used_indice[indice1]
     else:
         raise Exception('Error! the value of tsm parameter does not match!')
     df_matrix = pd.DataFrame(matrix, index=transcripts, columns=transcripts)
     return df_matrix
 
+def get_gene_model(df_gtot, df_transcripts):
+    list_all_distinct_genes = list(pd.Categorical(df_gtot['id_gene'].values))
+    list_save_id_gene = []
+    list_save_sequences = []
+    for distinct_gene in list_all_distinct_genes:
+        list_all_distinct_transcripts = list(pd.Categorical(df_gtot[df_gtot['id_gene']==distinct_gene].id_transcript.values))
+        list_all_alg_distinct_transcripts = list(df_transcripts[df_transcripts['id_transcript'].isin(list_all_distinct_transcripts)].alg.values)
+        length_seq = len(list_all_alg_distinct_transcripts[0])
+        list_save_id_gene.append(distinct_gene)
+        list_save_sequence = []
+        for position in range(length_seq):
+            is_conserved = True
+            for alg_distinct_transcript in list_all_alg_distinct_transcripts:
+                if alg_distinct_transcript[position] == '-':
+                    list_save_sequence.append('-')
+                    is_conserved = False
+                    break
+                if is_conserved:
+                    list_save_sequence.append('c')
+        list_save_sequences.append(''.join(list_save_sequence))
+    df = pd.DataFrame(columns=['id_gene','gene_model'])
+    df['id_gene'] = list_save_id_gene
+    df['gene_model'] = list_save_sequences
+    return df
+
 def compute_deghom_score_tsmplus(tr_id, tr_ref, transcripts_blocks,data_block_alg_gene, g_id, g_ref ):
     """
         Compute the degHom score (do not account for blocks not appearing at the gene level)
     """
     block_id = transcripts_blocks[transcripts_blocks['id_transcript']==tr_id].blocks.values[0].split('|')
     block_ref = transcripts_blocks[transcripts_blocks['id_transcript']==tr_ref].blocks.values[0].split('|')
     block_g_id = data_block_alg_gene[data_block_alg_gene['id_gene']==g_id].blocks.values[0].split('|')
@@ -303,41 +380,29 @@
     union_set = list(set(block_id).union(set(block_ref)))
     denum_list = [_ for _ in union_set if _ in block_g_id and _ in block_g_ref]
     if len(denum_list) == 0:
         return 0
     score = len(intersect_set)/len(denum_list)   
     return score
 
-def nucleotide_in_gene(gene_tr1, position, data_alg_seq, df_gtot):
-    transcripts_in_gene1 = list(pd.Categorical(df_gtot[df_gtot['id_gene']==gene_tr1].id_transcript.values))
-    #transcripts_in_gene2 = list(pd.Categorical(df_gtot[df_gtot['id_gene']==gene_tr2].id_transcript.values))
-    bool_nuc1 = False
-    #bool_nuc2 = False
-    for transcript1 in transcripts_in_gene1:
-        nuc1 = data_alg_seq[data_alg_seq['id_transcript']==transcript1].alg.values[0][position]
-        if nuc1 != '-':
-            bool_nuc1 = True
-            break
-    '''for transcript2 in transcripts_in_gene2:
-        nuc2 = data_alg_seq[data_alg_seq['id_transcript']==transcript2].alg.values[0][position]
-        if nuc2 != '-':
-            bool_nuc2 = True
-            break'''
-    
-    return bool_nuc1
+def nucleotide_in_gene(gene_tr, position, gene_model):
+    gene_model_seq = gene_model[gene_model['id_gene']==gene_tr].gene_model.values[0]
+    if gene_model_seq[position] == '-':
+        return False
+    elif gene_model_seq[position] == 'c':
+        return True
+    else:
+        raise ValueError('Could not find the conservation into the gene model')
 
-def compute_nuchom_score_tsmplus(transcript_1, transcript_2, data_alg_seq, gene_tr_1, gene_tr_2, df_gtot):
+def compute_nuchom_score_tsmplus(transcript_1, transcript_2, data_alg_seq, gene_tr_1, gene_tr_2, gene_model):
     """
         Compute nucHom score (do not account for nucleotides not appearing at the gene level)
     """
     alignment_tr1 = data_alg_seq[data_alg_seq['id_transcript']==transcript_1].alg.values[0]
     alignment_tr2 = data_alg_seq[data_alg_seq['id_transcript']==transcript_2].alg.values[0]
-
-    #alignment_g1 = data_alg_gene_seq[data_alg_gene_seq['id_gene']==gene_tr_1].alg.values[0]
-    #alignment_g2 = data_alg_gene_seq[data_alg_gene_seq['id_gene']==gene_tr_2].alg.values[0]
    
     length_alignment_tr1 = len(alignment_tr1)
     length_alignment_tr2 = len(alignment_tr2)
     if length_alignment_tr1 != length_alignment_tr2:
         return False
     else:
         matchs_mismatchs = 0
@@ -347,22 +412,19 @@
         for position in range(length_alignment_tr1):
             nucleotide_tr1 = alignment_tr1[position]
             nucleotide_tr2 = alignment_tr2[position]
             if((nucleotide_tr1 != '-') and (nucleotide_tr2 != '-')):
                 matchs_mismatchs += 1
             elif(((nucleotide_tr1 == '-') and (nucleotide_tr2 != '-'))) or ((nucleotide_tr1 != '-') and (nucleotide_tr2 == '-')):
                 indel += 1
-                #nuc_g1 = alignment_g1[position]
-                #nuc_g2 = alignment_g2[position]
-                #nuc_g1, nuc_g2 = nucleotide_in_gene(gene_tr_1, gene_tr_2, position, data_alg_seq, df_gtot)
                 if (nucleotide_tr1 != '-') and (nucleotide_tr2 == '-'):
-                    nuc_g2 = nucleotide_in_gene(gene_tr_2, position, data_alg_seq, df_gtot)
+                    nuc_g2 = nucleotide_in_gene(gene_tr_2, position, gene_model)
                     nuc_g1 = True
                 else:
-                    nuc_g1 = nucleotide_in_gene(gene_tr_1, position, data_alg_seq, df_gtot)
+                    nuc_g1 = nucleotide_in_gene(gene_tr_1, position, gene_model)
                     nuc_g2 = True
                     
                 if nuc_g1 and nuc_g2:
                     indel_denum += 1
             else:
                 gap_gap += 1
         if (matchs_mismatchs + indel_denum) == 0:
@@ -422,8 +484,8 @@
     args = build_arg_parser().parse_args()
     transcripts_msa_path = args.tralignment
     gtot_path = args.genetotranscripts
     tsm_conditions_path = int(args.tsmuncorrected)
     output_folder_path = args.outputfolder
 
     # compute the algorithm
-    get_matrix(transcripts_msa_path, gtot_path, tsm_conditions_path, output_folder_path)
+    get_matrix(transcripts_msa_path, gtot_path, tsm_conditions_path, output_folder_path)
```

### Comparing `transcriptorthology-1.0.1/transcriptorthology/transcriptOrthology.py` & `transcriptorthology-2.0.0/transcriptorthology/transcriptOrthology.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 > Reference:
 ======
     https://github.com/UdeS-CoBIUS/TranscriptOrthology
 """
 __authors__ = ("Wend Yam Donald Davy Ouedraogo")
 __contact__ = ("wend.yam.donald.davy.usherbrooke.ca")
 __copyright__ = "CoBIUS lab at Université de Sherbrooke, QC, CANADA"
-__date__ = "2022-12-19"
-__version__= "1.0.2"
+__date__ = "2023-06-26"
+__version__= "2.0.0"
 
 
 import argparse
-from .Tclustering import get_orthology_graph
-from .tsmComputing import get_matrix
+from Tclustering import get_orthology_graph
+from tsmComputing import get_matrix
 
 
 def build_arg_parser():
     '''Parsing function'''
     parser = argparse.ArgumentParser(description="program parameters")
     parser.add_argument('-talg', '--tralignment', default=None, help='Multiple Sequences Alignment of transcripts in FASTA format')
     parser.add_argument('-gtot', '--genetotranscripts', default=None, help="mappings transcripts to corresponding genes")
```

### Comparing `transcriptorthology-1.0.1/transcriptorthology/Tclustering.py` & `transcriptorthology-2.0.0/transcriptorthology/Tclustering.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 > Reference:
 ======
     https://github.com/UdeS-CoBIUS/TranscriptOrthology
 """
 __authors__ = ("Wend Yam Donald Davy Ouedraogo")
 __contact__ = ("wend.yam.donald.davy.usherbrooke.ca")
 __copyright__ = "CoBIUS lab at Université de Sherbrooke, QC, CANADA"
-__date__ = "2022-12-19"
-__version__= "1.0.2"
+__date__ = "2023-06-26"
+__version__= "2.0.0"
 
 import pandas as pd
 import networkx as nx
 import time
 from ete3 import Tree
 import matplotlib.pyplot as plt
 import argparse
@@ -304,8 +304,8 @@
     matrix_path = args.matrix
     gtot_path = args.genetotranscripts
     gt_path = args.nhxgenetree
     lower_bound = float(args.lowerbound)
     output_folder_path = args.outputfolder
 
     #compute the algorithm
-    get_orthology_graph(matrix_path, gtot_path, gt_path, lower_bound, output_folder_path)
+    get_orthology_graph(matrix_path, gtot_path, gt_path, lower_bound, output_folder_path)
```

### Comparing `transcriptorthology-1.0.1/setup.py` & `transcriptorthology-2.0.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.1'
+VERSION = '2.0.0'
 DESCRIPTION = 'A transcript orthologies inferring package'
 LONG_DESCRIPTION = 'A package that using Gene-level homology relationships to define different types of homology relationships between homologous transcripts'
 
 setup(
     name="transcriptorthology",
     version=VERSION,
     description=DESCRIPTION,
```

### Comparing `transcriptorthology-1.0.1/PKG-INFO` & `transcriptorthology-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: transcriptorthology
-Version: 1.0.1
+Version: 2.0.0
 Summary: A transcript orthologies inferring package
 Home-page: https://github.com/UdeS-CoBIUS/TranscriptOrthology
 Author: Wend Yam Donald Davy Ouedraogo
 Author-email: wend.yam.donald.davy.ouedraogo@usherbrooke.ca
 License: MIT
 Description: A package that using Gene-level homology relationships to define different types of homology relationships between homologous transcripts
 Keywords: clustering,alternative-splicing,orthoogy-inference,isoorthology,algorithm,evolution,computational-biology
```

### Comparing `transcriptorthology-1.0.1/transcriptorthology.egg-info/PKG-INFO` & `transcriptorthology-2.0.0/transcriptorthology.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: transcriptorthology
-Version: 1.0.1
+Version: 2.0.0
 Summary: A transcript orthologies inferring package
 Home-page: https://github.com/UdeS-CoBIUS/TranscriptOrthology
 Author: Wend Yam Donald Davy Ouedraogo
 Author-email: wend.yam.donald.davy.ouedraogo@usherbrooke.ca
 License: MIT
 Description: A package that using Gene-level homology relationships to define different types of homology relationships between homologous transcripts
 Keywords: clustering,alternative-splicing,orthoogy-inference,isoorthology,algorithm,evolution,computational-biology
```


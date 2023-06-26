# Comparing `tmp/hydrusvideodeduplicator-0.1.5.tar.gz` & `tmp/hydrusvideodeduplicator-0.1.6.tar.gz`

## Comparing `hydrusvideodeduplicator-0.1.5.tar` & `hydrusvideodeduplicator-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,22 @@
--rw-r--r--   0        0        0     4891 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.5/src/hydrusvideodeduplicator/README.md
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.5/src/hydrusvideodeduplicator/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.5/src/hydrusvideodeduplicator/__init__.py
--rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.5/src/hydrusvideodeduplicator/__main__.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.5/src/hydrusvideodeduplicator/config.py
--rw-r--r--   0        0        0    11276 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.5/src/hydrusvideodeduplicator/dedup.py
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.5/src/hydrusvideodeduplicator/dedup_util.py
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.5/src/hydrusvideodeduplicator/pdq_utils.py
--rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.5/src/hydrusvideodeduplicator/vpdq.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.5/src/hydrusvideodeduplicator/vpdq_brute_matcher.py
--rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.5/src/hydrusvideodeduplicator/vpdq_faiss.py
--rw-r--r--   0        0        0     5565 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.5/src/hydrusvideodeduplicator/vpdq_util.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.5/tests/__init__.py
--rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.5/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.5/LICENSE
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.5/README.md
--rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     4891 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/README.md
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/__init__.py
+-rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/__main__.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/config.py
+-rw-r--r--   0        0        0    11301 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/dedup.py
+-rw-r--r--   0        0        0     4036 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/dedup_util.py
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/pdq_utils.py
+-rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/vpdq.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/vpdq_brute_matcher.py
+-rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/vpdq_faiss.py
+-rw-r--r--   0        0        0     5565 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/vpdq_util.py
+-rw-r--r--   0        0        0    34519 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/hydrus_api/LICENSE
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/hydrus_api/README.md
+-rw-r--r--   0        0        0    36568 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/hydrus_api/__init__.py
+-rw-r--r--   0        0        0     5261 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/hydrus_api/utils.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.6/tests/__init__.py
+-rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.6/README.md
+-rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.6/PKG-INFO
```

### Comparing `hydrusvideodeduplicator-0.1.5/src/hydrusvideodeduplicator/README.md` & `hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/README.md`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.5/src/hydrusvideodeduplicator/__main__.py` & `hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 from typing import Optional, Annotated, List
 
 import typer
-import hydrus_api
+import hydrusvideodeduplicator.hydrus_api as hydrus_api
 from rich import print as rprint
 
 from .__about__ import __version__
 from .config import HYDRUS_API_KEY, HYDRUS_API_URL
 from .dedup import HydrusVideoDeduplicator
 
 from .vpdq_util import VPDQ_QUERY_MATCH_THRESHOLD_PERCENT
```

### Comparing `hydrusvideodeduplicator-0.1.5/src/hydrusvideodeduplicator/config.py` & `hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/config.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.5/src/hydrusvideodeduplicator/dedup.py` & `hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/dedup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import os
 from io import IOBase
 import logging
 import tempfile
 from itertools import islice
 import json
-from sqlitedict import SqliteDict
+from pathlib import Path
 
-import hydrus_api
-import hydrus_api.utils
+import hydrusvideodeduplicator.hydrus_api as hydrus_api
+import hydrusvideodeduplicator.hydrus_api.utils
 from tqdm import tqdm
 from rich import print as rprint
+from sqlitedict import SqliteDict
 
 from .config import DEDUP_DATABASE_FILE, DEDUP_DATABASE_DIR, DEDUP_DATABASE_NAME
 from .dedup_util import find_tag_in_tags, get_file_names_hydrus
 from .vpdq import VPDQSignal
 
 from .vpdq_util import (
     VPDQ_QUERY_MATCH_THRESHOLD_PERCENT,
@@ -59,25 +60,39 @@
         if custom_query is not None:
             custom_query = [x for x in custom_query if x.strip()] # Remove whitespace and empty strings
             if len(custom_query) > 0:
                 search_tags.extend(custom_query)
                 rprint(f"[yellow] Custom Query: {custom_query}")
 
         if not skip_hashing:
-            self._add_perceptual_hash_to_videos(overwrite=overwrite, custom_query=custom_query)
+            self._add_perceptual_hashes_to_db(overwrite=overwrite, custom_query=custom_query)
         else:
             rprint("[yellow] Skipping perceptual hashing")
 
         self._find_potential_duplicates()
         self.hydlog.info("Deduplication done.")
-
-    # Update perceptual hash for videos
-    # By default only adds missing phashes
-    # TODO: Allow batching, where if a video is already in the DB get another until no videos left or count is 0
-    def _add_perceptual_hash_to_videos(self, overwrite: bool, custom_query: list | None = None) -> None:
+    
+    @classmethod
+    # dir is where you're writing the video file
+    def _add_perceptual_hash_to_db(cls, video_hash: str, video: str | bytes, video_dir: Path | str, db) -> None:
+        with tempfile.NamedTemporaryFile(mode="w+b", dir=video_dir) as tmp_vid_file:
+            # Write video to file to be able to calculate hash
+            tmp_vid_file.write(video)
+            tmp_vid_file.seek(0)
+
+            # Set perceptual_hash column
+            perceptual_hash = VPDQSignal.hash_from_file(tmp_vid_file.name)
+
+            row = db.get(video_hash, {})
+            row["perceptual_hash"] = perceptual_hash
+            db[video_hash] = row
+            cls.hydlog.debug(f"Perceptual hash calculated and added to DB.")
+    
+    # Add perceptual hash for videos to the database
+    def _add_perceptual_hashes_to_db(self, overwrite: bool, custom_query: list | None = None) -> None:
 
         # Create database folder if it doesn't already exist
         if os.path.exists(DEDUP_DATABASE_FILE):
             with SqliteDict(str(DEDUP_DATABASE_FILE), tablename = "videos") as hashdb:
                 rprint(f"[green] Database found with {len(hashdb)} videos already hashed.")
                 self.hydlog.info(f"Found existing DB of length {len(hashdb)}, size {os.path.getsize(DEDUP_DATABASE_FILE)}")
         else:
@@ -86,66 +101,52 @@
             self.hydlog.info(f"Created DB dir {DEDUP_DATABASE_DIR}")
 
         search_tags = ["system:filetype=video"]
         if custom_query is not None:
             custom_query = [x for x in custom_query if x.strip()] # Remove whitespace and empty strings
             search_tags.extend(custom_query)
         
-        # GET video files SHA256 with no perceptual hash tag and store for later
-        print(f"Retrieving video file hashes from {self.client.api_url}")
-        # TODO: This could be absolutely massive. Chunk it somehow. Maybe with a query where hashes must not equal previous hashes processed?
-        percep_tagged_video_hashes = self.client.search_files(search_tags, return_hashes=True)["hashes"]
-        
-        print("Calculating perceptual hashes:")
-
         with SqliteDict(str(DEDUP_DATABASE_FILE), tablename = "videos") as hashdb:
-            with tempfile.TemporaryDirectory() as tmp_dir_name:
-                # Commit every n videos to avoid excessive writes
-                commit_interval = 8    
-                count_since_last_commit = 0
-                for video_hash in tqdm(percep_tagged_video_hashes):
-                    # don't calc new value unless overwrite is true
-                    if not overwrite and video_hash in hashdb:
-                        continue
-                    
-                    count_since_last_commit+=1
-
-                    # TODO: Check for valid request?
-                    video_response = self.client.get_file(hash_=video_hash)
-                    try:
-                        # spooled file means it stays in RAM unless it's too big
-                        with tempfile.NamedTemporaryFile(mode="w+b", dir=tmp_dir_name) as tmp_vid_file:
-                            tmp_vid_file.write(video_response.content)
-                            tmp_vid_file.seek(0)
+            print(f"Retrieving video file hashes...")
+            all_video_hashes = self.client.search_files(search_tags, file_sort_type=hydrus_api.FileSortType.FILE_SIZE, return_hashes=True, file_sort_asc=True, return_file_ids=False)["hashes"]
+            print("Calculating perceptual hashes:")
+            with tqdm(dynamic_ncols=True, total=len(all_video_hashes), unit="video", colour="BLUE") as pbar:
+                with tempfile.TemporaryDirectory() as tmp_dir_name:
+                    for chunk_video_hashes in hydrus_api.utils.yield_chunks(all_video_hashes, chunk_size=16):
+                        for video_hash in chunk_video_hashes:
+                            pbar.update(1)
+                            # Only calculate new hash if it's missing or if overwrite is true
+                            if not overwrite and video_hash in hashdb and hashdb[video_hash].get("perceptual_hash", None) is not None:
+                                continue
                             
-                            # Set perceptual_hash column
-                            perceptual_hash = VPDQSignal.hash_from_file(tmp_vid_file.name)
                             try:
-                                row = hashdb[video_hash]
-                            except KeyError:
-                                hashdb[video_hash] = {}
-
-                            row = hashdb[video_hash]
-                            row["perceptual_hash"] = perceptual_hash
-                            hashdb[video_hash] = row
-                            self.hydlog.debug(f"Perceptual hash calculated and added to DB.")
-                    except KeyboardInterrupt:
-                        rprint("[red] Perceptual hash generation was interrupted!\n")
-                        break
-                    except:
-                        rprint("[red] Failed to calculate a perceptual hash.")
-                        self.hydlog.error(f"Errored file hash: {video_hash}")
-                    
-                    if count_since_last_commit >= commit_interval:
+                                video_response = self.client.get_file(hash_=video_hash)
+                                if video_response.content is None:
+                                    continue
+                            except hydrus_api.HydrusAPIException:
+                                rprint("[red] Error getting file from database.")
+                                continue
+
+                            try:
+                                self._add_perceptual_hash_to_db(video_hash=video_hash, video=video_response.content, video_dir=tmp_dir_name, db=hashdb)
+                            except KeyboardInterrupt:
+                                rprint("[red] Perceptual hash generation was interrupted!\n")
+                                hashdb.commit()
+                                return None
+                            except:
+                                rprint("[red] Failed to calculate a perceptual hash.")
+                                self.hydlog.error(f"Errored file hash: {video_hash}")
+                            
+                        # Commit at the end of a chunk
                         hashdb.commit()
-                        count_since_last_commit = 0
 
+            # Commit at the end of all processing
             hashdb.commit()
             
-        rprint("[green]All perceptual hash tags have been added to video files.\n")
+        rprint("[green] Finished perceptual hash processing.\n")
     
     def get_potential_duplicate_count_hydrus(self) -> int:
         return self.client.get_potentials_count(file_service_keys=[self.all_services["all_local_files"][0]["service_key"]])["potential_duplicates_count"]
     
     # Return similarity of two bitstrings given a threshold
     @staticmethod
     def is_similar(a: str, b: str, min_percent_similarity: float = 0.8) -> bool:
@@ -165,55 +166,50 @@
         except RuntimeError: # SqliteDict error when trying to create a table for a DB in read-only mode
             rprint(f"[red] Database does not exist. Cannot search for duplicates.")
             return None
 
         # TODO: Add support for query where it will get a list of the hashes from
         # the query and iterate over them instead of the entire hashdb
 
-        # TODO: This can be multithreaded
+        # TODO: This can be multiprocessed
 
         # Number of potential duplicates before adding more. Just for user info.
         pre_dedupe_count = self.get_potential_duplicate_count_hydrus()
 
         similar_files_found_count = 0
         
         video_counter = 0
         with SqliteDict(str(DEDUP_DATABASE_FILE), tablename="videos", flag="r") as hashdb:
-            # tqdm progress bar is broken for SqliteDict because len doesn't work
-            for i, video_hash in tqdm(enumerate(hashdb), desc="Finding duplicates"):
-                video_counter+=1
-                video_phash = hashdb[video_hash]["perceptual_hash"]
-                # TODO: Are sqlite databases ordered?
-                for video2_hash in islice(hashdb, i+1, None):
-                    video2_phash = hashdb[video2_hash]["perceptual_hash"]
-                    
-                    similar = HydrusVideoDeduplicator.is_similar(video_phash, video2_phash, self.threshold)
-                    
-                    if similar:
-                        similar_files_found_count += 1
-                        if self._DEBUG:
-                            file_names = get_file_names_hydrus(self.client, [video_hash, video2_hash])
-                            self.hydlog.info(f"Duplicates filenames: {file_names}")
-                            #self.hydlog.info(f"\"Duplicates hashes: {video_hash}\" and \"{video2_hash}\"")
+            with tqdm(dynamic_ncols=True, total=len(hashdb), desc="Finding duplicates", unit="video", colour="BLUE") as pbar:
+                for i, video_hash in enumerate(hashdb):
+                    pbar.update(1)
+                    video_counter+=1
+                    video_phash = hashdb[video_hash]["perceptual_hash"]
+                    # TODO: Are sqlite databases ordered?
+                    for video2_hash in islice(hashdb, i+1, None):
+                        video2_phash = hashdb[video2_hash]["perceptual_hash"]
+                        
+                        similar = HydrusVideoDeduplicator.is_similar(video_phash, video2_phash, self.threshold)
+                        
+                        if similar:
+                            similar_files_found_count += 1
+                            if self._DEBUG:
+                                file_names = get_file_names_hydrus(self.client, [video_hash, video2_hash])
+                                self.hydlog.info(f"Duplicates filenames: {file_names}")
+                                #self.hydlog.info(f"\"Duplicates hashes: {video_hash}\" and \"{video2_hash}\"")
+                            
+                            new_relationship = {
+                                "hash_a": str(video_hash),
+                                "hash_b": str(video2_hash),
+                                "relationship": int(hydrus_api.DuplicateStatus.POTENTIAL_DUPLICATES),
+                                "do_default_content_merge": True,
+                            }
                         
-                        new_relationship = {
-                            "hash_a": str(video_hash),
-                            "hash_b": str(video2_hash),
-                            "relationship": int(hydrus_api.DuplicateStatus.POTENTIAL_DUPLICATES),
-                            "do_default_content_merge": True,
-                        }
-                    
-                        # This throws always because set_file_relationships
-                        # in the Hydrus API doesn't have a response or something.
-                        # There is a pull request for this on the Hydrus API GitLab I should fork and merge
-                        # TODO: Defer this API call to speed up processing
-                        try:
+                            # TODO: Defer this API call to speed up processing
                             self.client.set_file_relationships([new_relationship])
-                        except json.decoder.JSONDecodeError:
-                            pass
 
         # Statistics for user
         # if user does duplicates processing while the script is running this count will be wrong.
         if similar_files_found_count > 0:
             rprint(f"[blue] {similar_files_found_count}/{video_counter} similar videos found")
             post_dedupe_count = self.get_potential_duplicate_count_hydrus()
             new_dedupes_count = post_dedupe_count-pre_dedupe_count
```

### Comparing `hydrusvideodeduplicator-0.1.5/src/hydrusvideodeduplicator/pdq_utils.py` & `hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/pdq_utils.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.5/src/hydrusvideodeduplicator/vpdq.py` & `hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/vpdq.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.5/src/hydrusvideodeduplicator/vpdq_brute_matcher.py` & `hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/vpdq_brute_matcher.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.5/src/hydrusvideodeduplicator/vpdq_faiss.py` & `hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/vpdq_faiss.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.5/src/hydrusvideodeduplicator/vpdq_util.py` & `hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/vpdq_util.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.5/.gitignore` & `hydrusvideodeduplicator-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.5/LICENSE` & `hydrusvideodeduplicator-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.5/README.md` & `hydrusvideodeduplicator-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.5/pyproject.toml` & `hydrusvideodeduplicator-0.1.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -18,29 +18,32 @@
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
     "appdirs",
-    "hydrus-api",
     "rich",
     "numpy",
     "tqdm",
     "python-dotenv",
     "typer",
     "vpdq",
     "sqlitedict",
+    "requests",
 ]
 
 [project.urls]
 Documentation = "https://github.com/appleappleapplenanner/hydrus-video-deduplicator#readme"
 Issues = "https://github.com/appleappleapplenanner/hydrus-video-deduplicator/issues"
 Source = "https://github.com/appleappleapplenanner/hydrus-video-deduplicator"
 
+[tool.hatch.dependencies]
+local_dependency = {path = "src/hydrusvideodeduplicator/hydrus_api"}
+
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.hatch.version]
 path = "src/hydrusvideodeduplicator/__about__.py"
 
 [tool.hatch.envs.default]
```

### Comparing `hydrusvideodeduplicator-0.1.5/PKG-INFO` & `hydrusvideodeduplicator-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: hydrusvideodeduplicator
-Version: 0.1.5
+Version: 0.1.6
 Summary: Video deduplicator utility for Hydrus Network
 Project-URL: Documentation, https://github.com/appleappleapplenanner/hydrus-video-deduplicator#readme
 Project-URL: Issues, https://github.com/appleappleapplenanner/hydrus-video-deduplicator/issues
 Project-URL: Source, https://github.com/appleappleapplenanner/hydrus-video-deduplicator
 Author: appleappleapplenanner
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Requires-Dist: appdirs
-Requires-Dist: hydrus-api
 Requires-Dist: numpy
 Requires-Dist: python-dotenv
+Requires-Dist: requests
 Requires-Dist: rich
 Requires-Dist: sqlitedict
 Requires-Dist: tqdm
 Requires-Dist: typer
 Requires-Dist: vpdq
 Description-Content-Type: text/markdown
```


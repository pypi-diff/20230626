# Comparing `tmp/microdata_tools-0.2.0.tar.gz` & `tmp/microdata_tools-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microdata_tools-0.2.0.tar", max compression
+gzip compressed data, was "microdata_tools-0.3.0.tar", max compression
```

## Comparing `microdata_tools-0.2.0.tar` & `microdata_tools-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1074 2023-06-23 13:29:09.501447 microdata_tools-0.2.0/LICENSE.md
--rw-r--r--   0        0        0     2232 2023-06-23 13:29:09.501447 microdata_tools-0.2.0/README.md
--rw-r--r--   0        0        0      176 2023-06-23 13:29:09.501447 microdata_tools-0.2.0/microdata_tools/__init__.py
--rw-r--r--   0        0        0     5722 2023-06-23 13:29:09.501447 microdata_tools-0.2.0/microdata_tools/_decrypt.py
--rw-r--r--   0        0        0     4562 2023-06-23 13:29:09.501447 microdata_tools-0.2.0/microdata_tools/_encrypt.py
--rw-r--r--   0        0        0      212 2023-06-23 13:29:09.501447 microdata_tools-0.2.0/microdata_tools/_utils.py
--rw-r--r--   0        0        0      141 2023-06-23 13:29:09.501447 microdata_tools-0.2.0/microdata_tools/exceptions.py
--rw-r--r--   0        0        0     1904 2023-06-23 13:29:09.501447 microdata_tools-0.2.0/microdata_tools/package_dataset.py
--rw-r--r--   0        0        0     2341 2023-06-23 13:29:09.501447 microdata_tools-0.2.0/microdata_tools/unpackage_dataset.py
--rw-r--r--   0        0        0      534 2023-06-23 13:29:09.501447 microdata_tools-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2798 1970-01-01 00:00:00.000000 microdata_tools-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-26 18:09:25.096910 microdata_tools-0.3.0/LICENSE.md
+-rw-r--r--   0        0        0     2238 2023-06-26 18:09:25.096910 microdata_tools-0.3.0/README.md
+-rw-r--r--   0        0        0      176 2023-06-26 18:09:25.096910 microdata_tools-0.3.0/microdata_tools/__init__.py
+-rw-r--r--   0        0        0     5947 2023-06-26 18:09:25.096910 microdata_tools-0.3.0/microdata_tools/_decrypt.py
+-rw-r--r--   0        0        0     4840 2023-06-26 18:09:25.096910 microdata_tools-0.3.0/microdata_tools/_encrypt.py
+-rw-r--r--   0        0        0     1159 2023-06-26 18:09:25.096910 microdata_tools-0.3.0/microdata_tools/_utils.py
+-rw-r--r--   0        0        0      193 2023-06-26 18:09:25.096910 microdata_tools-0.3.0/microdata_tools/exceptions.py
+-rw-r--r--   0        0        0     2243 2023-06-26 18:09:25.096910 microdata_tools-0.3.0/microdata_tools/package_dataset.py
+-rw-r--r--   0        0        0     2905 2023-06-26 18:09:25.096910 microdata_tools-0.3.0/microdata_tools/unpackage_dataset.py
+-rw-r--r--   0        0        0      534 2023-06-26 18:09:25.096910 microdata_tools-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2804 1970-01-01 00:00:00.000000 microdata_tools-0.3.0/PKG-INFO
```

### Comparing `microdata_tools-0.2.0/LICENSE.md` & `microdata_tools-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.2.0/README.md` & `microdata_tools-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -40,21 +40,22 @@
 
 Decryption uses the RSA private key located at ```RSA_KEY_DIR```.
 
 The packaged file is then stored in `output_dir/archive/unpackaged` after a successful run or `output_dir/archive/failed` after an unsuccessful run.
 
 ## Example
 Python script that uses a RSA public key named `microdata_public_key.pem` and packages a dataset:
+
 ```py
 from pathlib import Path
 from microdata_tools import package_dataset
 
 RSA_KEYS_DIRECTORY = Path("tests/resources/rsa_keys")
-DATASET_DIRECTORY = Path("tests/resources/input/DATASET_1")
+DATASET_DIRECTORY = Path("tests/resources/input_package/DATASET_1")
 OUTPUT_DIRECTORY = Path("tests/resources/output")
 
 package_dataset(
-    rsa_keys_dir=RSA_KEYS_DIRECTORY,
-    dataset_dir=DATASET_DIRECTORY,
-    output_dir=OUTPUT_DIRECTORY,
+   rsa_keys_dir=RSA_KEYS_DIRECTORY,
+   dataset_dir=DATASET_DIRECTORY,
+   output_dir=OUTPUT_DIRECTORY,
 )
 ```
```

### Comparing `microdata_tools-0.2.0/microdata_tools/_decrypt.py` & `microdata_tools-0.3.0/microdata_tools/_decrypt.py`

 * *Files 6% similar despite different names*

```diff
@@ -136,14 +136,20 @@
         chunk_files = [str for str in files if str.endswith(".csv.encr")]
 
         if len(chunk_files) == 0:
             raise InvalidTarFileContents(
                 f"Tar file for {dataset_name} does not contain any chunks files"
             )
 
+        if f"{dataset_name}.md5" not in files:
+            raise InvalidTarFileContents(
+                f"Tar file for {dataset_name} does not contain the required "
+                f"{dataset_name}.md5 file"
+            )
+
 
 def _combine_csv_files(input_dir: Path, output_file: Path) -> None:
     sorted_chunkpaths = _get_sorted_file_names(input_dir)
     logger.debug(f"\nCombining {len(sorted_chunkpaths)} files into {output_file}")
 
     with open(output_file, "wb") as combined_file:
         for chunk_number, file_name in sorted_chunkpaths:
```

### Comparing `microdata_tools-0.2.0/microdata_tools/_encrypt.py` & `microdata_tools-0.3.0/microdata_tools/_encrypt.py`

 * *Files 3% similar despite different names*

```diff
@@ -128,15 +128,24 @@
     chunk_dir = dataset_dir / "chunks"
 
     if chunk_dir.exists():
         chunk_files = [file for file in chunk_dir.iterdir()]
         if len(chunk_files) == 0:
             raise ValidationException(f"No files found in {chunk_dir}")
 
-        files_to_tar.extend([dataset_dir / f"{dataset_name}.symkey.encr"])
+        md5_file = dataset_dir / f"{dataset_name}.md5"
+        if not md5_file.exists():
+            raise ValidationException(f"The required file {md5_file} is missing")
+
+        files_to_tar.extend(
+            [
+                dataset_dir / f"{dataset_name}.symkey.encr",
+                dataset_dir / f"{dataset_name}.md5",
+            ]
+        )
 
     with tarfile.open(full_tar_file_name, "w") as tar:
         for file in files_to_tar:
             tar.add(file, arcname=os.path.basename(file))
         if chunk_dir.exists():
             tar.add(chunk_dir, arcname=os.path.basename(chunk_dir))
```

### Comparing `microdata_tools-0.2.0/microdata_tools/package_dataset.py` & `microdata_tools-0.3.0/microdata_tools/package_dataset.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import logging
 import os
 import shutil
 from pathlib import Path
 
 from microdata_tools._encrypt import _tar_encrypted_dataset, encrypt_dataset
 from microdata_tools.exceptions import ValidationException
-from microdata_tools._utils import check_exists
+from microdata_tools._utils import check_exists, write_checksum_to_file
 
 logger = logging.getLogger()
 
 
 def package_dataset(rsa_keys_dir: Path, dataset_dir: Path, output_dir: Path) -> None:
     """
     Packages a dataset. It will encrypt and tar the dataset using
     the provided RSA public key. Only the CSV file will be encrypted.
+    Creates a checksum file for the CSV file.
 
     :param rsa_keys_dir:
         directory containing public key file microdata_public_key.pem
     :param dataset_dir:
         directory containing the dataset files (CSV and JSON)
     :param output_dir:
         output directory
@@ -36,23 +37,30 @@
         # Validate that there is only one csv file
         if len(csv_files) > 1:
             raise ValidationException(
                 f"There should only be one csv file in {dataset_dir}"
             )
 
         if len(csv_files) == 1:
+            write_checksum_to_file(csv_files[0])
             encrypt_dataset(
                 rsa_keys_dir=rsa_keys_dir,
                 dataset_dir=dataset_dir,
                 output_dir=output_dir,
             )
         else:
             if not dataset_output_dir.exists():
                 os.makedirs(dataset_output_dir)
 
+        if Path(dataset_dir / f"{dataset_name}.md5").exists():
+            shutil.copyfile(
+                dataset_dir / f"{dataset_name}.md5",
+                dataset_output_dir / f"{dataset_name}.md5",
+            )
+
         shutil.copyfile(
             dataset_dir / f"{dataset_name}.json",
             dataset_output_dir / f"{dataset_name}.json",
         )
         _tar_encrypted_dataset(input_dir=output_dir, dataset_name=dataset_name)
 
     except Exception as exe:
```

### Comparing `microdata_tools-0.2.0/microdata_tools/unpackage_dataset.py` & `microdata_tools-0.3.0/microdata_tools/unpackage_dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 import logging
 import os
 from pathlib import Path
 import shutil
 from typing import Union
-from microdata_tools._utils import check_exists
+from microdata_tools._utils import (
+    check_exists,
+    compare_checksum_with_file,
+    calculate_checksum,
+)
 from microdata_tools._decrypt import decrypt, untar_encrypted_dataset
 
 logger = logging.getLogger()
 
 
 def unpackage_dataset(
     packaged_file_path: Path,
     rsa_keys_dir: Path,
     output_dir: Path,
     archive_dir: Union[Path, None],
 ) -> None:
     """
     Unpackages a dataset. It will untar and decrypt the dataset using
     the provided RSA private key. Only the CSV file will be decrypted.
+    Validates the checksum of the CSV file.
 
     :param packaged_file_path:
         a Path to the .tar file containing the dataset files
     :param rsa_keys_dir:
         directory containing the private key file microdata_private_key.pem
     :param output_dir:
         output directory
@@ -42,23 +47,34 @@
     dataset_name = packaged_file_path.stem
     dataset_dir = packaged_file_path.parent / dataset_name
     logger.info(f"Unpackaging {packaged_file_path}")
 
     try:
         untar_encrypted_dataset(packaged_file_path, dataset_name, dataset_dir)
         decrypt(rsa_keys_dir, dataset_dir, output_dir)
+        _validate_csv_consistency(dataset_name, dataset_dir, output_dir)
         if archive_dir is not None:
             _archive(dataset_name, dataset_dir.parent, archive_dir, "unpackaged")
         logger.info(f"Unpackaged {packaged_file_path}")
     except Exception as exc:
         if archive_dir is not None:
             _archive(dataset_name, dataset_dir.parent, archive_dir, "failed")
         logger.exception(f"Failed to unpackage {dataset_name}", exc_info=exc)
 
 
+def _validate_csv_consistency(dataset_name, dataset_dir, output_dir):
+    if Path(output_dir / dataset_name / f"{dataset_name}.csv").exists():
+        calculated_checksum = calculate_checksum(
+            output_dir / dataset_name / f"{dataset_name}.csv"
+        )
+        compare_checksum_with_file(
+            dataset_dir / f"{dataset_name}.md5", calculated_checksum
+        )
+
+
 def _archive(
     dataset_name: str, input_dir: Path, archive_dir: Path, sub_dir: str
 ) -> None:
     archive_sub_dir = archive_dir / sub_dir
 
     if not archive_sub_dir.exists():
         os.makedirs(archive_sub_dir)
```

### Comparing `microdata_tools-0.2.0/pyproject.toml` & `microdata_tools-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "microdata-tools"
-version = "0.2.0"
+version = "0.3.0"
 description = "Tools for the microdata.no platform"
 authors = ["microdata-developers"]
 license = "MIT License"
 readme = "README.md"
 packages = [{include = "microdata_tools"}]
 
 [tool.poetry.dependencies]
```

### Comparing `microdata_tools-0.2.0/PKG-INFO` & `microdata_tools-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microdata-tools
-Version: 0.2.0
+Version: 0.3.0
 Summary: Tools for the microdata.no platform
 License: MIT
 Author: microdata-developers
 Requires-Python: >=3.7.2,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -56,22 +56,23 @@
 
 Decryption uses the RSA private key located at ```RSA_KEY_DIR```.
 
 The packaged file is then stored in `output_dir/archive/unpackaged` after a successful run or `output_dir/archive/failed` after an unsuccessful run.
 
 ## Example
 Python script that uses a RSA public key named `microdata_public_key.pem` and packages a dataset:
+
 ```py
 from pathlib import Path
 from microdata_tools import package_dataset
 
 RSA_KEYS_DIRECTORY = Path("tests/resources/rsa_keys")
-DATASET_DIRECTORY = Path("tests/resources/input/DATASET_1")
+DATASET_DIRECTORY = Path("tests/resources/input_package/DATASET_1")
 OUTPUT_DIRECTORY = Path("tests/resources/output")
 
 package_dataset(
-    rsa_keys_dir=RSA_KEYS_DIRECTORY,
-    dataset_dir=DATASET_DIRECTORY,
-    output_dir=OUTPUT_DIRECTORY,
+   rsa_keys_dir=RSA_KEYS_DIRECTORY,
+   dataset_dir=DATASET_DIRECTORY,
+   output_dir=OUTPUT_DIRECTORY,
 )
 ```
```


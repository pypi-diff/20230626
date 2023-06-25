# Comparing `tmp/ngitl_common_py-0.3.0.tar.gz` & `tmp/ngitl_common_py-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngitl_common_py-0.3.0.tar", last modified: Fri Jun 16 22:48:46 2023, max compression
+gzip compressed data, was "ngitl_common_py-0.4.2.tar", last modified: Sun Jun 25 22:37:16 2023, max compression
```

## Comparing `ngitl_common_py-0.3.0.tar` & `ngitl_common_py-0.4.2.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 22:48:46.780965 ngitl_common_py-0.3.0/
--rw-rw-rw-   0        0        0      274 2023-06-16 22:48:46.781606 ngitl_common_py-0.3.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-16 22:48:46.783957 ngitl_common_py-0.3.0/ngitl_common_py/
--rw-rw-rw-   0        0        0       76 2023-06-13 08:53:12.000000 ngitl_common_py-0.3.0/ngitl_common_py/__init__.py
--rw-rw-rw-   0        0        0      518 2023-06-16 22:48:46.783957 ngitl_common_py-0.3.0/ngitl_common_py/_version.py
--rw-rw-rw-   0        0        0     2089 2023-06-06 08:26:25.000000 ngitl_common_py-0.3.0/ngitl_common_py/autostart.py
--rw-rw-rw-   0        0        0     2618 2023-06-16 22:04:14.000000 ngitl_common_py-0.3.0/ngitl_common_py/config.py
--rw-rw-rw-   0        0        0      895 2023-06-13 09:00:23.000000 ngitl_common_py-0.3.0/ngitl_common_py/file_viewer_starter.py
--rw-rw-rw-   0        0        0     1775 2023-06-16 21:27:15.000000 ngitl_common_py-0.3.0/ngitl_common_py/log.py
-drwxrwxrwx   0        0        0        0 2023-06-16 22:48:46.750105 ngitl_common_py-0.3.0/ngitl_common_py.egg-info/
--rw-rw-rw-   0        0        0      274 2023-06-16 22:48:46.000000 ngitl_common_py-0.3.0/ngitl_common_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      475 2023-06-16 22:48:46.000000 ngitl_common_py-0.3.0/ngitl_common_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 22:48:46.000000 ngitl_common_py-0.3.0/ngitl_common_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-16 22:48:46.000000 ngitl_common_py-0.3.0/ngitl_common_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-06-16 22:48:46.000000 ngitl_common_py-0.3.0/ngitl_common_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      220 2023-06-16 22:48:46.782966 ngitl_common_py-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      555 2023-06-13 09:11:28.000000 ngitl_common_py-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-16 22:48:46.779010 ngitl_common_py-0.3.0/tests/
--rw-rw-rw-   0        0        0        0 2023-06-13 08:56:23.000000 ngitl_common_py-0.3.0/tests/__init__.py
--rw-rw-rw-   0        0        0     1406 2023-06-06 07:13:53.000000 ngitl_common_py-0.3.0/tests/test_autostart.py
--rw-rw-rw-   0        0        0     2604 2023-06-16 12:57:57.000000 ngitl_common_py-0.3.0/tests/test_log.py
--rw-rw-rw-   0        0        0    83607 2023-06-07 21:51:31.000000 ngitl_common_py-0.3.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:37:16.361214 ngitl_common_py-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-25 22:36:59.000000 ngitl_common_py-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-25 22:37:16.361214 ngitl_common_py-0.4.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:37:16.361214 ngitl_common_py-0.4.2/ngitl_common_py/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-25 22:36:59.000000 ngitl_common_py-0.4.2/ngitl_common_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-25 22:37:16.361214 ngitl_common_py-0.4.2/ngitl_common_py/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-25 22:36:59.000000 ngitl_common_py-0.4.2/ngitl_common_py/autostart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-25 22:36:59.000000 ngitl_common_py-0.4.2/ngitl_common_py/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-25 22:36:59.000000 ngitl_common_py-0.4.2/ngitl_common_py/file_viewer_starter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-25 22:36:59.000000 ngitl_common_py-0.4.2/ngitl_common_py/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 22:36:59.000000 ngitl_common_py-0.4.2/ngitl_common_py/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:37:16.361214 ngitl_common_py-0.4.2/ngitl_common_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-25 22:37:16.000000 ngitl_common_py-0.4.2/ngitl_common_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-25 22:37:16.000000 ngitl_common_py-0.4.2/ngitl_common_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 22:37:16.000000 ngitl_common_py-0.4.2/ngitl_common_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-25 22:37:16.000000 ngitl_common_py-0.4.2/ngitl_common_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-25 22:37:16.000000 ngitl_common_py-0.4.2/ngitl_common_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-25 22:37:16.361214 ngitl_common_py-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-25 22:36:59.000000 ngitl_common_py-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:37:16.361214 ngitl_common_py-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 22:36:59.000000 ngitl_common_py-0.4.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-25 22:36:59.000000 ngitl_common_py-0.4.2/tests/test_autostart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-06-25 22:36:59.000000 ngitl_common_py-0.4.2/tests/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83436 2023-06-25 22:36:59.000000 ngitl_common_py-0.4.2/versioneer.py
```

### Comparing `ngitl_common_py-0.3.0/ngitl_common_py/config.py` & `ngitl_common_py-0.4.2/ngitl_common_py/config.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,91 +1,91 @@
-# Copyright (C) 2023, NG:ITL
-import json
-import os
-from pathlib import Path
-from typing import Optional, Any
-from ngitl_common_py.log import LOG_LEVELS
-
-DEFAULT_CONFIG_SEARCH_PATHS = [Path.cwd(), Path.home()]
-
-__config = {}
-
-
-class ConfigEntryError(Exception):
-    def __init__(self, msg: str, *args):
-        super().__init__(args)
-        self.msg = msg
-
-    def __str__(self):
-        return self.msg
-
-
-class ConfigEntryInvalidLogLevelError(ConfigEntryError):
-    def __init__(self, log_level: str, *args):
-        super().__init__(
-            f"Invalid log level requested: {log_level}, available log level: {LOG_LEVELS}",
-            args,
-        )
-
-
-class ConfigEntryNotADirectoryError(ConfigEntryError):
-    def __init__(self, directory_path: Path, *args):
-        super().__init__(
-            f'Invalid config entry, directory "{directory_path}" is not a valid directory!',
-            args,
-        )
-
-
-class ConfigEntryFileNotFoundError(ConfigEntryError):
-    def __init__(self, file_path: Path, *args):
-        super().__init__(f'Invalid config entry, file "{file_path}" is not a valid file!', args)
-
-
-def find_config_file(config_filename: str) -> Optional[Path]:
-    for search_path in DEFAULT_CONFIG_SEARCH_PATHS:
-        filepath_to_check = search_path / config_filename
-        if filepath_to_check.exists():
-            return filepath_to_check
-    return None
-
-
-def read_config(config_file_path: Path):
-    with open(config_file_path) as json_data_file:
-        global __config
-        __config = json.load(json_data_file)
-
-
-def write_config_to_file(config_file_path: Path):
-    with open(config_file_path, "w") as output_file:
-        json.dump(__config, output_file, indent=4)
-
-
-def validate_directory_path(directory_path: Path, required_permission: int):
-    if not os.path.isdir(directory_path):
-        raise ConfigEntryNotADirectoryError(directory_path)
-    elif not os.access(directory_path, required_permission):
-        raise PermissionError(directory_path)
-
-
-def validate_file_path(file_path: Path):
-    if not os.path.isfile(file_path):
-        raise ConfigEntryFileNotFoundError(file_path)
-
-
-def validate_log_level(log_level_str: str):
-    if log_level_str not in LOG_LEVELS:
-        raise ConfigEntryInvalidLogLevelError(log_level_str)
-
-
-def get_config() -> dict:
-    global __config
-    return __config
-
-
-def get_config_param(name: str) -> Any:
-    global __config
-    return __config[name]
-
-
-def set_config_param(name: str, value: Any) -> None:
-    global __config
-    __config[name] = value
+# Copyright (C) 2023, NG:ITL
+import json
+import os
+from pathlib import Path
+from typing import Optional, Any
+from ngitl_common_py.log import LOG_LEVELS
+
+DEFAULT_CONFIG_SEARCH_PATHS = [Path.cwd(), Path.home()]
+
+__config = {}
+
+
+class ConfigEntryError(Exception):
+    def __init__(self, msg: str, *args):
+        super().__init__(args)
+        self.msg = msg
+
+    def __str__(self):
+        return self.msg
+
+
+class ConfigEntryInvalidLogLevelError(ConfigEntryError):
+    def __init__(self, log_level: str, *args):
+        super().__init__(
+            f"Invalid log level requested: {log_level}, available log level: {LOG_LEVELS}",
+            args,
+        )
+
+
+class ConfigEntryNotADirectoryError(ConfigEntryError):
+    def __init__(self, directory_path: Path, *args):
+        super().__init__(
+            f'Invalid config entry, directory "{directory_path}" is not a valid directory!',
+            args,
+        )
+
+
+class ConfigEntryFileNotFoundError(ConfigEntryError):
+    def __init__(self, file_path: Path, *args):
+        super().__init__(f'Invalid config entry, file "{file_path}" is not a valid file!', args)
+
+
+def find_config_file(config_filename: str) -> Optional[Path]:
+    for search_path in DEFAULT_CONFIG_SEARCH_PATHS:
+        filepath_to_check = search_path / config_filename
+        if filepath_to_check.exists():
+            return filepath_to_check
+    return None
+
+
+def read_config(config_file_path: Path):
+    with open(config_file_path) as json_data_file:
+        global __config
+        __config = json.load(json_data_file)
+
+
+def write_config_to_file(config_file_path: Path):
+    with open(config_file_path, "w") as output_file:
+        json.dump(__config, output_file, indent=4)
+
+
+def validate_directory_path(directory_path: Path, required_permission: int):
+    if not os.path.isdir(directory_path):
+        raise ConfigEntryNotADirectoryError(directory_path)
+    elif not os.access(directory_path, required_permission):
+        raise PermissionError(directory_path)
+
+
+def validate_file_path(file_path: Path):
+    if not os.path.isfile(file_path):
+        raise ConfigEntryFileNotFoundError(file_path)
+
+
+def validate_log_level(log_level_str: str):
+    if log_level_str not in LOG_LEVELS:
+        raise ConfigEntryInvalidLogLevelError(log_level_str)
+
+
+def get_config() -> dict:
+    global __config
+    return __config
+
+
+def get_config_param(name: str) -> Any:
+    global __config
+    return __config[name]
+
+
+def set_config_param(name: str, value: Any) -> None:
+    global __config
+    __config[name] = value
```

### Comparing `ngitl_common_py-0.3.0/ngitl_common_py/file_viewer_starter.py` & `ngitl_common_py-0.4.2/ngitl_common_py/file_viewer_starter.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# Copyright (C) 2023, NG:ITL
-import os.path
-import subprocess
-from pathlib import Path
-
-
-NOTEPAD_EXECUTABLE_PATH = Path(r"C:\Windows\System32\notepad.exe")
-NOTEPADPP_EXECUTABLE_PATH = Path(r"C:\Program Files (x86)\Notepad++\notepad++.exe")
-
-
-def _is_notepadpp_available() -> bool:
-    return os.path.isfile(NOTEPADPP_EXECUTABLE_PATH)
-
-
-def _open_file_with_notepadpp(filepath: Path) -> None:
-    subprocess.Popen(
-        [NOTEPADPP_EXECUTABLE_PATH, "-nosession", filepath],
-        creationflags=subprocess.DETACHED_PROCESS,
-    )
-
-
-def _open_file_with_notepad(filepath: Path) -> None:
-    subprocess.Popen([NOTEPAD_EXECUTABLE_PATH, filepath], creationflags=subprocess.DETACHED_PROCESS)
-
-
-def open_file_viewer(filepath: Path) -> None:
-    if _is_notepadpp_available():
-        _open_file_with_notepadpp(filepath)
-    else:
-        _open_file_with_notepad(filepath)
+# Copyright (C) 2023, NG:ITL
+import os.path
+import subprocess
+from pathlib import Path
+
+
+NOTEPAD_EXECUTABLE_PATH = Path(r"C:\Windows\System32\notepad.exe")
+NOTEPADPP_EXECUTABLE_PATH = Path(r"C:\Program Files (x86)\Notepad++\notepad++.exe")
+
+
+def _is_notepadpp_available() -> bool:
+    return os.path.isfile(NOTEPADPP_EXECUTABLE_PATH)
+
+
+def _open_file_with_notepadpp(filepath: Path) -> None:
+    subprocess.Popen(
+        [NOTEPADPP_EXECUTABLE_PATH, "-nosession", filepath],
+        creationflags=subprocess.DETACHED_PROCESS,
+    )
+
+
+def _open_file_with_notepad(filepath: Path) -> None:
+    subprocess.Popen([NOTEPAD_EXECUTABLE_PATH, filepath], creationflags=subprocess.DETACHED_PROCESS)
+
+
+def open_file_viewer(filepath: Path) -> None:
+    if _is_notepadpp_available():
+        _open_file_with_notepadpp(filepath)
+    else:
+        _open_file_with_notepad(filepath)
```

### Comparing `ngitl_common_py-0.3.0/ngitl_common_py/log.py` & `ngitl_common_py-0.4.2/ngitl_common_py/log.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,57 +1,58 @@
-# Copyright (C) 2023, NG:ITL
-import logging
-import datetime
-import sys
-from pathlib import Path
-from typing import Optional
-
-LOG_LEVELS = {"DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"}
-LOG_FORMAT = "%(asctime)s [%(levelname)s][%(module)s]: %(message)s"
-EMERGENCY_LOGGING_LOG_LEVEL = "DEBUG"
-
-log_filepath: Optional[Path] = None
-
-
-def init_logging(component_name: str, log_file_directory: Path, logging_level: str):
-    global log_filepath
-    timestamp = datetime.datetime.now()
-    timestamp_prefix = timestamp.strftime("%Y%m%d-%H%M%S")
-    log_filepath = log_file_directory / f"{timestamp_prefix}_{component_name}.log"
-    stdout_handler = logging.StreamHandler(sys.stdout)
-    file_handler = logging.FileHandler(log_filepath)
-    logging.basicConfig(
-        force=True,
-        handlers=[stdout_handler, file_handler],
-        level=logging_level,
-        format=LOG_FORMAT,
-    )
-    logging.info("Logging initialized!")
-
-
-def init_emergency_logging(component_name: str, log_file_directory: Path = Path.cwd()):
-    global log_filepath
-    log_filepath = log_file_directory / f"{component_name}_emergency.log"
-    stdout_handler = logging.StreamHandler(sys.stdout)
-    file_handler = logging.FileHandler(log_filepath)
-    logging.basicConfig(
-        force=True,
-        handlers=[stdout_handler, file_handler],
-        level=EMERGENCY_LOGGING_LOG_LEVEL,
-        format=LOG_FORMAT,
-    )
-    logging.error("Emergency log initialized!")
-
-
-def validate_log_level(log_level: str) -> bool:
-    return log_level in LOG_LEVELS
-
-
-def get_log_filepath() -> Path:
-    global log_filepath
-    return log_filepath
-
-
-def flush():
-    logger = logging.getLogger()
-    for handler in logger.handlers:
-        handler.flush()
+# Copyright (C) 2023, NG:ITL
+import logging
+import datetime
+import sys
+from pathlib import Path
+from typing import Optional
+
+LOG_LEVELS = {"DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"}
+LOG_FORMAT = "%(asctime)s [%(levelname)s][%(module)s]: %(message)s"
+EMERGENCY_LOGGING_LOG_LEVEL = "DEBUG"
+
+log_filepath: Optional[Path] = None
+
+
+def init_logging(component_name: str, log_file_directory: Path, logging_level: str):
+    global log_filepath
+    timestamp = datetime.datetime.now()
+    timestamp_prefix = timestamp.strftime("%Y%m%d-%H%M%S")
+    log_filepath = log_file_directory / f"{timestamp_prefix}_{component_name}.log"
+    stdout_handler = logging.StreamHandler(sys.stdout)
+    file_handler = logging.FileHandler(log_filepath)
+    logging.basicConfig(
+        force=True,
+        handlers=[stdout_handler, file_handler],
+        level=logging_level,
+        format=LOG_FORMAT,
+    )
+    logging.info("Logging initialized!")
+
+
+def init_emergency_logging(component_name: str, log_file_directory: Path = Path.cwd()):
+    global log_filepath
+    log_filepath = log_file_directory / f"{component_name}_emergency.log"
+    stdout_handler = logging.StreamHandler(sys.stdout)
+    file_handler = logging.FileHandler(log_filepath)
+    logging.basicConfig(
+        force=True,
+        handlers=[stdout_handler, file_handler],
+        level=EMERGENCY_LOGGING_LOG_LEVEL,
+        format=LOG_FORMAT,
+    )
+    logging.error("Emergency log initialized!")
+
+
+def validate_log_level(log_level: str) -> bool:
+    return log_level in LOG_LEVELS
+
+
+def get_log_filepath() -> Path:
+    global log_filepath
+    assert log_filepath
+    return log_filepath
+
+
+def flush():
+    logger = logging.getLogger()
+    for handler in logger.handlers:
+        handler.flush()
```

### Comparing `ngitl_common_py-0.3.0/setup.py` & `ngitl_common_py-0.4.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-#!/usr/bin/env python
-# Copyright (C) 2022, NG:ITL
-import versioneer
-from setuptools import find_packages, setup
-
-
-setup(
-    name="ngitl_common_py",
-    version=versioneer.get_version(),
-    cmdclass=versioneer.get_cmdclass(),
-    description="Helper classes and functions for common python problems",
-    author="NG:ITL",
-    license="GPLv3",
-    author_email="torsten.wylegala@volkswagen.de",
-    url="https://github.com/vw-wob-it-edu-ngitl/ngitl_common_py/",
-    packages=find_packages("."),
-    install_requires=["pywin32==306"],
-)
+#!/usr/bin/env python
+# Copyright (C) 2022, NG:ITL
+from pathlib import Path
+
+import versioneer
+from setuptools import find_packages, setup
+
+setup(
+    name="ngitl_common_py",
+    version=versioneer.get_version(),
+    cmdclass=versioneer.get_cmdclass(),
+    description="Helper classes and functions for common python problems",
+    long_description="Helper classes and functions for common python problems",
+    author="NG:ITL",
+    license="GPLv3",
+    author_email="torsten.wylegala@volkswagen.de",
+    url="https://github.com/vw-wob-it-edu-ngitl/ngitl_common_py/",
+    packages=find_packages("."),
+    install_requires=["pywin32==306"],
+)
```

### Comparing `ngitl_common_py-0.3.0/tests/test_autostart.py` & `ngitl_common_py-0.4.2/tests/test_autostart.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,38 @@
-# Copyright (C) 2023, NG:ITL
-import os
-import tempfile
-import unittest
-from pathlib import Path
-
-from ngitl_common_py import autostart
-
-
-class WindowsAutostartTest(unittest.TestCase):
-
-    def setUp(self) -> None:
-        tmp_dir = tempfile.mkdtemp()
-        autostart_dir = os.path.join(tmp_dir, 'autostart')
-        os.mkdir(autostart_dir)
-        self.test_link_file = Path(os.path.join(autostart_dir, 'test.lnk'))
-        self.test_target_file = Path(__file__)
-
-    def enable_autostart(self):
-        autostart.activate_autostart(self.test_target_file, self.test_link_file)
-
-    def disable_autostart(self):
-        autostart.deactivate_autostart(self.test_link_file)
-
-    def test_AutostartEnabled_IsAutostartIsEnabled_ReturnTrue(self):
-        self.enable_autostart()
-        self.assertTrue(autostart.is_autostart_enabled(self.test_link_file))
-
-    def test_AutostartDisabled_IsAutostartIsEnabled_ReturnFalse(self):
-        self.disable_autostart()
-        self.assertFalse(autostart.is_autostart_enabled(self.test_link_file))
-
-    def test_AutostartEnabled_IsLinkFileExisting_FileExisting(self):
-        self.enable_autostart()
-        self.assertTrue(os.path.isfile(self.test_link_file))
-
-    def test_AutostartDisabled_IsLinkFileExisting_FileNotExisting(self):
-        self.disable_autostart()
-        self.assertFalse(os.path.isfile(self.test_link_file))
+# Copyright (C) 2023, NG:ITL
+import os
+import tempfile
+import unittest
+from pathlib import Path
+
+from ngitl_common_py import autostart
+
+
+class WindowsAutostartTest(unittest.TestCase):
+    def setUp(self) -> None:
+        tmp_dir = tempfile.mkdtemp()
+        autostart_dir = os.path.join(tmp_dir, "autostart")
+        os.mkdir(autostart_dir)
+        self.test_link_file = Path(os.path.join(autostart_dir, "test.lnk"))
+        self.test_target_file = Path(__file__)
+
+    def enable_autostart(self):
+        autostart.activate_autostart(self.test_target_file, self.test_link_file)
+
+    def disable_autostart(self):
+        autostart.deactivate_autostart(self.test_link_file)
+
+    def test_AutostartEnabled_IsAutostartIsEnabled_ReturnTrue(self):
+        self.enable_autostart()
+        self.assertTrue(autostart.is_autostart_enabled(self.test_link_file))
+
+    def test_AutostartDisabled_IsAutostartIsEnabled_ReturnFalse(self):
+        self.disable_autostart()
+        self.assertFalse(autostart.is_autostart_enabled(self.test_link_file))
+
+    def test_AutostartEnabled_IsLinkFileExisting_FileExisting(self):
+        self.enable_autostart()
+        self.assertTrue(os.path.isfile(self.test_link_file))
+
+    def test_AutostartDisabled_IsLinkFileExisting_FileNotExisting(self):
+        self.disable_autostart()
+        self.assertFalse(os.path.isfile(self.test_link_file))
```

### Comparing `ngitl_common_py-0.3.0/tests/test_log.py` & `ngitl_common_py-0.4.2/tests/test_log.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,80 +1,75 @@
-# Copyright (C) 2023, NG:ITL
-import logging
-import tempfile
-import unittest
-import re
-import abc
-
-from pathlib import Path
-
-from ngitl_common_py.log import init_logging, init_emergency_logging, get_log_filepath, flush
-
-
-class LogTest(unittest.TestCase):
-
-    TEST_COMPONENT_NAME = "unittest"
-
-    def setUp(self) -> None:
-        self.tmp_dir = Path(tempfile.mkdtemp())
-        self.init_log()
-
-    @abc.abstractmethod
-    def init_log(self):
-        raise NotImplementedError
-
-    # def find_log_file(self) -> Optional[Path]:
-    #     elements = os.listdir(self.tmp_dir)
-    #     for element in elements:
-    #         if re.search(r"(\d{8}-\d{6}_|)unittest(_emergency|)\.log", element):
-    #             return self.tmp_dir / element
-
-    def log_test_lines(self):
-        logging.debug("log line 1")
-        logging.info("log line 2")
-        logging.warning("log line 3")
-        logging.error("log line 4")
-
-    def assert_log_line(self, expected_line_as_regex: str):
-        flush()
-        with open(get_log_filepath(), "r") as log_file:
-            lines = log_file.readlines()
-            for line in lines:
-                if re.search(expected_line_as_regex, line):
-                    return
-            self.fail(f"Unable to find expected line in log file: \"{expected_line_as_regex}\"")
-
-    def assert_test_log_lines(self):
-        self.assert_log_line(r"\[DEBUG\]\[test_log\]: log line 1$")
-        self.assert_log_line(r"\[INFO\]\[test_log\]: log line 2$")
-        self.assert_log_line(r"\[WARNING\]\[test_log\]: log line 3$")
-        self.assert_log_line(r"\[ERROR\]\[test_log\]: log line 4$")
-
-class RegularLogTest(LogTest):
-
-    def init_log(self):
-        init_logging(self.TEST_COMPONENT_NAME, self.tmp_dir, "DEBUG")
-
-    def assert_regular_welcome_log_line(self):
-        self.assert_log_line("Logging initialized!")
-
-    def test_RegularLogInitialized_PrintLogLines_ExpectedLinesLogged(self) -> None:
-        self.log_test_lines()
-        self.assert_regular_welcome_log_line()
-        self.assert_test_log_lines()
-
-
-class EmergencyLogTest(LogTest):
-
-    def init_log(self):
-        init_emergency_logging(self.TEST_COMPONENT_NAME, log_file_directory=self.tmp_dir)
-
-    def assert_emergency_welcome_log_line(self):
-        self.assert_log_line("\[ERROR\]\[log\]: Emergency log initialized!$")
-
-    def test_RegularLogInitialized_PrintLogLines_ExpectedLinesLogged(self) -> None:
-        self.log_test_lines()
-        self.assert_emergency_welcome_log_line()
-        self.assert_test_log_lines()
-
-
-
+# Copyright (C) 2023, NG:ITL
+import logging
+import tempfile
+import unittest
+import re
+import abc
+
+from pathlib import Path
+
+from ngitl_common_py.log import init_logging, init_emergency_logging, get_log_filepath, flush
+
+
+class LogTest(unittest.TestCase):
+    TEST_COMPONENT_NAME = "unittest"
+
+    def setUp(self) -> None:
+        self.tmp_dir = Path(tempfile.mkdtemp())
+        self.init_log()
+
+    @abc.abstractmethod
+    def init_log(self):
+        raise NotImplementedError
+
+    # def find_log_file(self) -> Optional[Path]:
+    #     elements = os.listdir(self.tmp_dir)
+    #     for element in elements:
+    #         if re.search(r"(\d{8}-\d{6}_|)unittest(_emergency|)\.log", element):
+    #             return self.tmp_dir / element
+
+    def log_test_lines(self):
+        logging.debug("log line 1")
+        logging.info("log line 2")
+        logging.warning("log line 3")
+        logging.error("log line 4")
+
+    def assert_log_line(self, expected_line_as_regex: str):
+        flush()
+        with open(get_log_filepath(), "r") as log_file:
+            lines = log_file.readlines()
+            for line in lines:
+                if re.search(expected_line_as_regex, line):
+                    return
+            self.fail(f'Unable to find expected line in log file: "{expected_line_as_regex}"')
+
+    def assert_test_log_lines(self):
+        self.assert_log_line(r"\[DEBUG\]\[test_log\]: log line 1$")
+        self.assert_log_line(r"\[INFO\]\[test_log\]: log line 2$")
+        self.assert_log_line(r"\[WARNING\]\[test_log\]: log line 3$")
+        self.assert_log_line(r"\[ERROR\]\[test_log\]: log line 4$")
+
+
+class RegularLogTest(LogTest):
+    def init_log(self):
+        init_logging(self.TEST_COMPONENT_NAME, self.tmp_dir, "DEBUG")
+
+    def assert_regular_welcome_log_line(self):
+        self.assert_log_line("Logging initialized!")
+
+    def test_RegularLogInitialized_PrintLogLines_ExpectedLinesLogged(self) -> None:
+        self.log_test_lines()
+        self.assert_regular_welcome_log_line()
+        self.assert_test_log_lines()
+
+
+class EmergencyLogTest(LogTest):
+    def init_log(self):
+        init_emergency_logging(self.TEST_COMPONENT_NAME, log_file_directory=self.tmp_dir)
+
+    def assert_emergency_welcome_log_line(self):
+        self.assert_log_line("\[ERROR\]\[log\]: Emergency log initialized!$")
+
+    def test_RegularLogInitialized_PrintLogLines_ExpectedLinesLogged(self) -> None:
+        self.log_test_lines()
+        self.assert_emergency_welcome_log_line()
+        self.assert_test_log_lines()
```

### Comparing `ngitl_common_py-0.3.0/versioneer.py` & `ngitl_common_py-0.4.2/versioneer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 # Version: 0.28
 
 """The Versioneer - like a rocketeer, but for versions.
 
 The Versioneer
 ==============
 
@@ -304,14 +303,16 @@
 """
 # pylint:disable=invalid-name,import-outside-toplevel,missing-function-docstring
 # pylint:disable=missing-class-docstring,too-many-branches,too-many-statements
 # pylint:disable=raise-missing-from,too-many-lines,too-many-locals,import-error
 # pylint:disable=too-few-public-methods,redefined-outer-name,consider-using-with
 # pylint:disable=attribute-defined-outside-init,too-many-arguments
 
+# mypy: ignore-errors
+
 import configparser
 import errno
 import json
 import os
 import re
 import subprocess
 import sys
@@ -344,33 +345,34 @@
     versioneer_py = os.path.join(root, "versioneer.py")
     if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
         # allow 'python path/to/setup.py COMMAND'
         root = os.path.dirname(os.path.realpath(os.path.abspath(sys.argv[0])))
         setup_py = os.path.join(root, "setup.py")
         versioneer_py = os.path.join(root, "versioneer.py")
     if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
-        err = ("Versioneer was unable to run the project root directory. "
-               "Versioneer requires setup.py to be executed from "
-               "its immediate directory (like 'python setup.py COMMAND'), "
-               "or in a way that lets it use sys.argv[0] to find the root "
-               "(like 'python path/to/setup.py COMMAND').")
+        err = (
+            "Versioneer was unable to run the project root directory. "
+            "Versioneer requires setup.py to be executed from "
+            "its immediate directory (like 'python setup.py COMMAND'), "
+            "or in a way that lets it use sys.argv[0] to find the root "
+            "(like 'python path/to/setup.py COMMAND')."
+        )
         raise VersioneerBadRootError(err)
     try:
         # Certain runtime workflows (setup.py install/develop in a setuptools
         # tree) execute all dependencies in a single python process, so
         # "versioneer" may be imported multiple times, and python's shared
         # module-import table will cache the first one. So we can't use
         # os.path.dirname(__file__), as that will find whichever
         # versioneer.py was first imported, even in later projects.
         my_path = os.path.realpath(os.path.abspath(__file__))
         me_dir = os.path.normcase(os.path.splitext(my_path)[0])
         vsr_dir = os.path.normcase(os.path.splitext(versioneer_py)[0])
         if me_dir != vsr_dir and "VERSIONEER_PEP518" not in globals():
-            print("Warning: build in %s is using versioneer.py from %s"
-                  % (os.path.dirname(my_path), versioneer_py))
+            print("Warning: build in %s is using versioneer.py from %s" % (os.path.dirname(my_path), versioneer_py))
     except NameError:
         pass
     return root
 
 
 def get_config_from_root(root):
     """Read the project setup.cfg file to determine Versioneer config."""
@@ -380,29 +382,29 @@
     # the top of versioneer.py for instructions on writing your setup.cfg .
     root = Path(root)
     pyproject_toml = root / "pyproject.toml"
     setup_cfg = root / "setup.cfg"
     section = None
     if pyproject_toml.exists() and have_tomllib:
         try:
-            with open(pyproject_toml, 'rb') as fobj:
+            with open(pyproject_toml, "rb") as fobj:
                 pp = tomllib.load(fobj)
-            section = pp['tool']['versioneer']
+            section = pp["tool"]["versioneer"]
         except (tomllib.TOMLDecodeError, KeyError):
             pass
     if not section:
         parser = configparser.ConfigParser()
         with open(setup_cfg) as cfg_file:
             parser.read_file(cfg_file)
         parser.get("versioneer", "VCS")  # raise error if missing
 
         section = parser["versioneer"]
 
     cfg = VersioneerConfig()
-    cfg.VCS = section['VCS']
+    cfg.VCS = section["VCS"]
     cfg.style = section.get("style", "")
     cfg.versionfile_source = section.get("versionfile_source")
     cfg.versionfile_build = section.get("versionfile_build")
     cfg.tag_prefix = section.get("tag_prefix")
     if cfg.tag_prefix in ("''", '""', None):
         cfg.tag_prefix = ""
     cfg.parentdir_prefix = section.get("parentdir_prefix")
@@ -417,23 +419,24 @@
 # these dictionaries contain VCS-specific tools
 LONG_VERSION_PY: Dict[str, str] = {}
 HANDLERS: Dict[str, Dict[str, Callable]] = {}
 
 
 def register_vcs_handler(vcs, method):  # decorator
     """Create decorator to mark a method as the handler of a VCS."""
+
     def decorate(f):
         """Store f in HANDLERS[vcs][method]."""
         HANDLERS.setdefault(vcs, {})[method] = f
         return f
+
     return decorate
 
 
-def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
-                env=None):
+def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False, env=None):
     """Call the given command(s)."""
     assert isinstance(commands, list)
     process = None
 
     popen_kwargs = {}
     if sys.platform == "win32":
         # This hides the console window if pythonw.exe is used
@@ -441,18 +444,22 @@
         startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
         popen_kwargs["startupinfo"] = startupinfo
 
     for command in commands:
         try:
             dispcmd = str([command] + args)
             # remember shell=False, so use git.cmd on windows, not just git
-            process = subprocess.Popen([command] + args, cwd=cwd, env=env,
-                                       stdout=subprocess.PIPE,
-                                       stderr=(subprocess.PIPE if hide_stderr
-                                               else None), **popen_kwargs)
+            process = subprocess.Popen(
+                [command] + args,
+                cwd=cwd,
+                env=env,
+                stdout=subprocess.PIPE,
+                stderr=(subprocess.PIPE if hide_stderr else None),
+                **popen_kwargs,
+            )
             break
         except OSError:
             e = sys.exc_info()[1]
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %s" % dispcmd)
@@ -467,15 +474,17 @@
         if verbose:
             print("unable to run %s (error)" % dispcmd)
             print("stdout was %s" % stdout)
         return None, process.returncode
     return stdout, process.returncode
 
 
-LONG_VERSION_PY['git'] = r'''
+LONG_VERSION_PY[
+    "git"
+] = r'''
 # This file helps to compute a version number in source trees obtained from
 # git-archive tarball (such as those provided by githubs download-from-tag
 # feature). Distribution tarballs (built by setup.py sdist) and build
 # directories (produced by setup.py build) will contain a much shorter file
 # that just contains the computed version number.
 
 # This file is released into the public domain.
@@ -1183,49 +1192,56 @@
         if verbose:
             print("keywords are unexpanded, not using")
         raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
     refs = {r.strip() for r in refnames.strip("()").split(",")}
     # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
     # just "foo-1.0". If we see a "tag: " prefix, prefer those.
     TAG = "tag: "
-    tags = {r[len(TAG):] for r in refs if r.startswith(TAG)}
+    tags = {r[len(TAG) :] for r in refs if r.startswith(TAG)}
     if not tags:
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
-        tags = {r for r in refs if re.search(r'\d', r)}
+        tags = {r for r in refs if re.search(r"\d", r)}
         if verbose:
             print("discarding '%s', no digits" % ",".join(refs - tags))
     if verbose:
         print("likely tags: %s" % ",".join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
-            r = ref[len(tag_prefix):]
+            r = ref[len(tag_prefix) :]
             # Filter out refs that exactly match prefix or that don't start
             # with a number once the prefix is stripped (mostly a concern
             # when prefix is '')
-            if not re.match(r'\d', r):
+            if not re.match(r"\d", r):
                 continue
             if verbose:
                 print("picking %s" % r)
-            return {"version": r,
-                    "full-revisionid": keywords["full"].strip(),
-                    "dirty": False, "error": None,
-                    "date": date}
+            return {
+                "version": r,
+                "full-revisionid": keywords["full"].strip(),
+                "dirty": False,
+                "error": None,
+                "date": date,
+            }
     # no suitable tags, so version is "0+unknown", but full hex is still there
     if verbose:
         print("no suitable tags, using unknown + full revision id")
-    return {"version": "0+unknown",
-            "full-revisionid": keywords["full"].strip(),
-            "dirty": False, "error": "no suitable tags", "date": None}
+    return {
+        "version": "0+unknown",
+        "full-revisionid": keywords["full"].strip(),
+        "dirty": False,
+        "error": "no suitable tags",
+        "date": None,
+    }
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
 def git_pieces_from_vcs(tag_prefix, root, verbose, runner=run_command):
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
@@ -1239,43 +1255,40 @@
     # GIT_DIR can interfere with correct operation of Versioneer.
     # It may be intended to be passed to the Versioneer-versioned project,
     # but that should not change where we get our version from.
     env = os.environ.copy()
     env.pop("GIT_DIR", None)
     runner = functools.partial(runner, env=env)
 
-    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root,
-                   hide_stderr=not verbose)
+    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root, hide_stderr=not verbose)
     if rc != 0:
         if verbose:
             print("Directory %s not under git control" % root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = runner(GITS, [
-        "describe", "--tags", "--dirty", "--always", "--long",
-        "--match", f"{tag_prefix}[[:digit:]]*"
-    ], cwd=root)
+    describe_out, rc = runner(
+        GITS, ["describe", "--tags", "--dirty", "--always", "--long", "--match", f"{tag_prefix}[[:digit:]]*"], cwd=root
+    )
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
     full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
     full_out = full_out.strip()
 
     pieces = {}
     pieces["long"] = full_out
     pieces["short"] = full_out[:7]  # maybe improved later
     pieces["error"] = None
 
-    branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"],
-                             cwd=root)
+    branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"], cwd=root)
     # --abbrev-ref was added in git-1.6.3
     if rc != 0 or branch_name is None:
         raise NotThisMethod("'git rev-parse --abbrev-ref' returned error")
     branch_name = branch_name.strip()
 
     if branch_name == "HEAD":
         # If we aren't exactly on a branch, pick a branch which represents
@@ -1307,37 +1320,35 @@
     # TAG might have hyphens.
     git_describe = describe_out
 
     # look for -dirty suffix
     dirty = git_describe.endswith("-dirty")
     pieces["dirty"] = dirty
     if dirty:
-        git_describe = git_describe[:git_describe.rindex("-dirty")]
+        git_describe = git_describe[: git_describe.rindex("-dirty")]
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
-        mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
+        mo = re.search(r"^(.+)-(\d+)-g([0-9a-f]+)$", git_describe)
         if not mo:
             # unparsable. Maybe git-describe is misbehaving?
-            pieces["error"] = ("unable to parse git-describe output: '%s'"
-                               % describe_out)
+            pieces["error"] = "unable to parse git-describe output: '%s'" % describe_out
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
             if verbose:
                 fmt = "tag '%s' doesn't start with prefix '%s'"
                 print(fmt % (full_tag, tag_prefix))
-            pieces["error"] = ("tag '%s' doesn't start with prefix '%s'"
-                               % (full_tag, tag_prefix))
+            pieces["error"] = "tag '%s' doesn't start with prefix '%s'" % (full_tag, tag_prefix)
             return pieces
-        pieces["closest-tag"] = full_tag[len(tag_prefix):]
+        pieces["closest-tag"] = full_tag[len(tag_prefix) :]
 
         # distance: number of commits since tag
         pieces["distance"] = int(mo.group(2))
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
@@ -1403,23 +1414,26 @@
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
 
     for _ in range(3):
         dirname = os.path.basename(root)
         if dirname.startswith(parentdir_prefix):
-            return {"version": dirname[len(parentdir_prefix):],
-                    "full-revisionid": None,
-                    "dirty": False, "error": None, "date": None}
+            return {
+                "version": dirname[len(parentdir_prefix) :],
+                "full-revisionid": None,
+                "dirty": False,
+                "error": None,
+                "date": None,
+            }
         rootdirs.append(root)
         root = os.path.dirname(root)  # up a level
 
     if verbose:
-        print("Tried directories %s but none started with prefix %s" %
-              (str(rootdirs), parentdir_prefix))
+        print("Tried directories %s but none started with prefix %s" % (str(rootdirs), parentdir_prefix))
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
 SHORT_VERSION_PY = """
 # This file was generated by 'versioneer.py' (0.28) from
 # revision-control system data, or from the parent directory name of an
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
@@ -1440,29 +1454,26 @@
 def versions_from_file(filename):
     """Try to determine the version from _version.py if present."""
     try:
         with open(filename) as f:
             contents = f.read()
     except OSError:
         raise NotThisMethod("unable to read _version.py")
-    mo = re.search(r"version_json = '''\n(.*)'''  # END VERSION_JSON",
-                   contents, re.M | re.S)
+    mo = re.search(r"version_json = '''\n(.*)'''  # END VERSION_JSON", contents, re.M | re.S)
     if not mo:
-        mo = re.search(r"version_json = '''\r\n(.*)'''  # END VERSION_JSON",
-                       contents, re.M | re.S)
+        mo = re.search(r"version_json = '''\r\n(.*)'''  # END VERSION_JSON", contents, re.M | re.S)
     if not mo:
         raise NotThisMethod("no version_json in _version.py")
     return json.loads(mo.group(1))
 
 
 def write_to_version_file(filename, versions):
     """Write the given version number to the given _version.py file."""
     os.unlink(filename)
-    contents = json.dumps(versions, sort_keys=True,
-                          indent=1, separators=(",", ": "))
+    contents = json.dumps(versions, sort_keys=True, indent=1, separators=(",", ": "))
     with open(filename, "w") as f:
         f.write(SHORT_VERSION_PY % contents)
 
     print("set %s to '%s'" % (filename, versions["version"]))
 
 
 def plus_or_dot(pieces):
@@ -1486,16 +1497,15 @@
         if pieces["distance"] or pieces["dirty"]:
             rendered += plus_or_dot(pieces)
             rendered += "%d.g%s" % (pieces["distance"], pieces["short"])
             if pieces["dirty"]:
                 rendered += ".dirty"
     else:
         # exception #1
-        rendered = "0+untagged.%d.g%s" % (pieces["distance"],
-                                          pieces["short"])
+        rendered = "0+untagged.%d.g%s" % (pieces["distance"], pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
 def render_pep440_branch(pieces):
     """TAG[[.dev0]+DISTANCE.gHEX[.dirty]] .
@@ -1516,16 +1526,15 @@
             if pieces["dirty"]:
                 rendered += ".dirty"
     else:
         # exception #1
         rendered = "0"
         if pieces["branch"] != "master":
             rendered += ".dev0"
-        rendered += "+untagged.%d.g%s" % (pieces["distance"],
-                                          pieces["short"])
+        rendered += "+untagged.%d.g%s" % (pieces["distance"], pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
 def pep440_split_post(ver):
     """Split pep440 version string at the post-release segment.
@@ -1678,19 +1687,21 @@
         rendered += "-dirty"
     return rendered
 
 
 def render(pieces, style):
     """Render the given version pieces into the requested style."""
     if pieces["error"]:
-        return {"version": "unknown",
-                "full-revisionid": pieces.get("long"),
-                "dirty": None,
-                "error": pieces["error"],
-                "date": None}
+        return {
+            "version": "unknown",
+            "full-revisionid": pieces.get("long"),
+            "dirty": None,
+            "error": pieces["error"],
+            "date": None,
+        }
 
     if not style or style == "default":
         style = "pep440"  # the default
 
     if style == "pep440":
         rendered = render_pep440(pieces)
     elif style == "pep440-branch":
@@ -1706,17 +1717,21 @@
     elif style == "git-describe":
         rendered = render_git_describe(pieces)
     elif style == "git-describe-long":
         rendered = render_git_describe_long(pieces)
     else:
         raise ValueError("unknown style '%s'" % style)
 
-    return {"version": rendered, "full-revisionid": pieces["long"],
-            "dirty": pieces["dirty"], "error": None,
-            "date": pieces.get("date")}
+    return {
+        "version": rendered,
+        "full-revisionid": pieces["long"],
+        "dirty": pieces["dirty"],
+        "error": None,
+        "date": pieces.get("date"),
+    }
 
 
 class VersioneerBadRootError(Exception):
     """The project root directory is unknown or missing key files."""
 
 
 def get_versions(verbose=False):
@@ -1731,16 +1746,15 @@
     root = get_root()
     cfg = get_config_from_root(root)
 
     assert cfg.VCS is not None, "please set [versioneer]VCS= in setup.cfg"
     handlers = HANDLERS.get(cfg.VCS)
     assert handlers, "unrecognized VCS '%s'" % cfg.VCS
     verbose = verbose or cfg.verbose
-    assert cfg.versionfile_source is not None, \
-        "please set versioneer.versionfile_source"
+    assert cfg.versionfile_source is not None, "please set versioneer.versionfile_source"
     assert cfg.tag_prefix is not None, "please set versioneer.tag_prefix"
 
     versionfile_abs = os.path.join(root, cfg.versionfile_source)
 
     # extract version from first of: _version.py, VCS command (e.g. 'git
     # describe'), parentdir. This is meant to work for developers using a
     # source checkout, for users of a tarball created by 'setup.py sdist',
@@ -1786,17 +1800,21 @@
             return ver
     except NotThisMethod:
         pass
 
     if verbose:
         print("unable to compute version")
 
-    return {"version": "0+unknown", "full-revisionid": None,
-            "dirty": None, "error": "unable to compute version",
-            "date": None}
+    return {
+        "version": "0+unknown",
+        "full-revisionid": None,
+        "dirty": None,
+        "error": "unable to compute version",
+        "date": None,
+    }
 
 
 def get_version():
     """Get the short version string for this project."""
     return get_versions()["version"]
 
 
@@ -1841,14 +1859,15 @@
             vers = get_versions(verbose=True)
             print("Version: %s" % vers["version"])
             print(" full-revisionid: %s" % vers.get("full-revisionid"))
             print(" dirty: %s" % vers.get("dirty"))
             print(" date: %s" % vers.get("date"))
             if vers["error"]:
                 print(" error: %s" % vers["error"])
+
     cmds["version"] = cmd_version
 
     # we override "build_py" in setuptools
     #
     # most invocation pathways end up running build_py:
     #  distutils/build -> build_py
     #  distutils/install -> distutils/build ->..
@@ -1862,16 +1881,16 @@
     #   then does setup.py bdist_wheel, or sometimes setup.py install
     #  setup.py egg_info -> ?
 
     # pip install -e . and setuptool/editable_wheel will invoke build_py
     # but the build_py command is not expected to copy any files.
 
     # we override different "build_py" commands for both environments
-    if 'build_py' in cmds:
-        _build_py = cmds['build_py']
+    if "build_py" in cmds:
+        _build_py = cmds["build_py"]
     else:
         from setuptools.command.build_py import build_py as _build_py
 
     class cmd_build_py(_build_py):
         def run(self):
             root = get_root()
             cfg = get_config_from_root(root)
@@ -1880,22 +1899,22 @@
             if getattr(self, "editable_mode", False):
                 # During editable installs `.py` and data files are
                 # not copied to build_lib
                 return
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
             if cfg.versionfile_build:
-                target_versionfile = os.path.join(self.build_lib,
-                                                  cfg.versionfile_build)
+                target_versionfile = os.path.join(self.build_lib, cfg.versionfile_build)
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
+
     cmds["build_py"] = cmd_build_py
 
-    if 'build_ext' in cmds:
-        _build_ext = cmds['build_ext']
+    if "build_ext" in cmds:
+        _build_ext = cmds["build_ext"]
     else:
         from setuptools.command.build_ext import build_ext as _build_ext
 
     class cmd_build_ext(_build_ext):
         def run(self):
             root = get_root()
             cfg = get_config_from_root(root)
@@ -1907,27 +1926,30 @@
                 # As in place builds will already have a _version.py
                 # in the module dir, we do not need to write one.
                 return
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
             if not cfg.versionfile_build:
                 return
-            target_versionfile = os.path.join(self.build_lib,
-                                              cfg.versionfile_build)
+            target_versionfile = os.path.join(self.build_lib, cfg.versionfile_build)
             if not os.path.exists(target_versionfile):
-                print(f"Warning: {target_versionfile} does not exist, skipping "
-                      "version update. This can happen if you are running build_ext "
-                      "without first running build_py.")
+                print(
+                    f"Warning: {target_versionfile} does not exist, skipping "
+                    "version update. This can happen if you are running build_ext "
+                    "without first running build_py."
+                )
                 return
             print("UPDATING %s" % target_versionfile)
             write_to_version_file(target_versionfile, versions)
+
     cmds["build_ext"] = cmd_build_ext
 
     if "cx_Freeze" in sys.modules:  # cx_freeze enabled?
         from cx_Freeze.dist import build_exe as _build_exe
+
         # nczeczulin reports that py2exe won't like the pep440-style string
         # as FILEVERSION, but it can be used for PRODUCTVERSION, e.g.
         # setup(console=[{
         #   "version": versioneer.get_version().split("+", 1)[0], # FILEVERSION
         #   "product_version": versioneer.get_version(),
         #   ...
 
@@ -1940,25 +1962,29 @@
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
                 _build_exe.run(self)
                 os.unlink(target_versionfile)
                 with open(cfg.versionfile_source, "w") as f:
                     LONG = LONG_VERSION_PY[cfg.VCS]
-                    f.write(LONG %
-                            {"DOLLAR": "$",
-                             "STYLE": cfg.style,
-                             "TAG_PREFIX": cfg.tag_prefix,
-                             "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                             "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                             })
+                    f.write(
+                        LONG
+                        % {
+                            "DOLLAR": "$",
+                            "STYLE": cfg.style,
+                            "TAG_PREFIX": cfg.tag_prefix,
+                            "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                            "VERSIONFILE_SOURCE": cfg.versionfile_source,
+                        }
+                    )
+
         cmds["build_exe"] = cmd_build_exe
         del cmds["build_py"]
 
-    if 'py2exe' in sys.modules:  # py2exe enabled?
+    if "py2exe" in sys.modules:  # py2exe enabled?
         try:
             from py2exe.setuptools_buildexe import py2exe as _py2exe
         except ImportError:
             from py2exe.distutils_buildexe import py2exe as _py2exe
 
         class cmd_py2exe(_py2exe):
             def run(self):
@@ -1969,63 +1995,67 @@
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
                 _py2exe.run(self)
                 os.unlink(target_versionfile)
                 with open(cfg.versionfile_source, "w") as f:
                     LONG = LONG_VERSION_PY[cfg.VCS]
-                    f.write(LONG %
-                            {"DOLLAR": "$",
-                             "STYLE": cfg.style,
-                             "TAG_PREFIX": cfg.tag_prefix,
-                             "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                             "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                             })
+                    f.write(
+                        LONG
+                        % {
+                            "DOLLAR": "$",
+                            "STYLE": cfg.style,
+                            "TAG_PREFIX": cfg.tag_prefix,
+                            "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                            "VERSIONFILE_SOURCE": cfg.versionfile_source,
+                        }
+                    )
+
         cmds["py2exe"] = cmd_py2exe
 
     # sdist farms its file list building out to egg_info
-    if 'egg_info' in cmds:
-        _egg_info = cmds['egg_info']
+    if "egg_info" in cmds:
+        _egg_info = cmds["egg_info"]
     else:
         from setuptools.command.egg_info import egg_info as _egg_info
 
     class cmd_egg_info(_egg_info):
         def find_sources(self):
             # egg_info.find_sources builds the manifest list and writes it
             # in one shot
             super().find_sources()
 
             # Modify the filelist and normalize it
             root = get_root()
             cfg = get_config_from_root(root)
-            self.filelist.append('versioneer.py')
+            self.filelist.append("versioneer.py")
             if cfg.versionfile_source:
                 # There are rare cases where versionfile_source might not be
                 # included by default, so we must be explicit
                 self.filelist.append(cfg.versionfile_source)
             self.filelist.sort()
             self.filelist.remove_duplicates()
 
             # The write method is hidden in the manifest_maker instance that
             # generated the filelist and was thrown away
             # We will instead replicate their final normalization (to unicode,
             # and POSIX-style paths)
             from setuptools import unicode_utils
-            normalized = [unicode_utils.filesys_decode(f).replace(os.sep, '/')
-                          for f in self.filelist.files]
 
-            manifest_filename = os.path.join(self.egg_info, 'SOURCES.txt')
-            with open(manifest_filename, 'w') as fobj:
-                fobj.write('\n'.join(normalized))
+            normalized = [unicode_utils.filesys_decode(f).replace(os.sep, "/") for f in self.filelist.files]
+
+            manifest_filename = os.path.join(self.egg_info, "SOURCES.txt")
+            with open(manifest_filename, "w") as fobj:
+                fobj.write("\n".join(normalized))
 
-    cmds['egg_info'] = cmd_egg_info
+    cmds["egg_info"] = cmd_egg_info
 
     # we override different "sdist" commands for both environments
-    if 'sdist' in cmds:
-        _sdist = cmds['sdist']
+    if "sdist" in cmds:
+        _sdist = cmds["sdist"]
     else:
         from setuptools.command.sdist import sdist as _sdist
 
     class cmd_sdist(_sdist):
         def run(self):
             versions = get_versions()
             self._versioneer_generated_versions = versions
@@ -2039,16 +2069,16 @@
             cfg = get_config_from_root(root)
             _sdist.make_release_tree(self, base_dir, files)
             # now locate _version.py in the new base_dir directory
             # (remembering that it may be a hardlink) and replace it with an
             # updated value
             target_versionfile = os.path.join(base_dir, cfg.versionfile_source)
             print("UPDATING %s" % target_versionfile)
-            write_to_version_file(target_versionfile,
-                                  self._versioneer_generated_versions)
+            write_to_version_file(target_versionfile, self._versioneer_generated_versions)
+
     cmds["sdist"] = cmd_sdist
 
     return cmds
 
 
 CONFIG_ERROR = """
 setup.cfg is missing the necessary Versioneer configuration. You need
@@ -2100,36 +2130,37 @@
 
 
 def do_setup():
     """Do main VCS-independent setup function for installing Versioneer."""
     root = get_root()
     try:
         cfg = get_config_from_root(root)
-    except (OSError, configparser.NoSectionError,
-            configparser.NoOptionError) as e:
+    except (OSError, configparser.NoSectionError, configparser.NoOptionError) as e:
         if isinstance(e, (OSError, configparser.NoSectionError)):
-            print("Adding sample versioneer config to setup.cfg",
-                  file=sys.stderr)
+            print("Adding sample versioneer config to setup.cfg", file=sys.stderr)
             with open(os.path.join(root, "setup.cfg"), "a") as f:
                 f.write(SAMPLE_CONFIG)
         print(CONFIG_ERROR, file=sys.stderr)
         return 1
 
     print(" creating %s" % cfg.versionfile_source)
     with open(cfg.versionfile_source, "w") as f:
         LONG = LONG_VERSION_PY[cfg.VCS]
-        f.write(LONG % {"DOLLAR": "$",
-                        "STYLE": cfg.style,
-                        "TAG_PREFIX": cfg.tag_prefix,
-                        "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                        "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                        })
+        f.write(
+            LONG
+            % {
+                "DOLLAR": "$",
+                "STYLE": cfg.style,
+                "TAG_PREFIX": cfg.tag_prefix,
+                "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                "VERSIONFILE_SOURCE": cfg.versionfile_source,
+            }
+        )
 
-    ipy = os.path.join(os.path.dirname(cfg.versionfile_source),
-                       "__init__.py")
+    ipy = os.path.join(os.path.dirname(cfg.versionfile_source), "__init__.py")
     if os.path.exists(ipy):
         try:
             with open(ipy, "r") as f:
                 old = f.read()
         except OSError:
             old = ""
         module = os.path.splitext(os.path.basename(cfg.versionfile_source))[0]
```


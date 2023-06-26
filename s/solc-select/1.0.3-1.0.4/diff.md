# Comparing `tmp/solc-select-1.0.3.tar.gz` & `tmp/solc-select-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solc-select-1.0.3.tar", last modified: Fri Feb  3 01:41:51 2023, max compression
+gzip compressed data, was "solc-select-1.0.4.tar", last modified: Mon Jun 26 16:27:33 2023, max compression
```

## Comparing `solc-select-1.0.3.tar` & `solc-select-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:41:51.829124 solc-select-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    34522 2023-02-03 01:41:40.000000 solc-select-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-02-03 01:41:51.829124 solc-select-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-02-03 01:41:40.000000 solc-select-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-02-03 01:41:40.000000 solc-select-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-03 01:41:51.829124 solc-select-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-02-03 01:41:40.000000 solc-select-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:41:51.829124 solc-select-1.0.3/solc_select/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 01:41:40.000000 solc-select-1.0.3/solc_select/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-02-03 01:41:40.000000 solc-select-1.0.3/solc_select/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-02-03 01:41:40.000000 solc-select-1.0.3/solc_select/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-02-03 01:41:40.000000 solc-select-1.0.3/solc_select/solc_select.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:41:51.829124 solc-select-1.0.3/solc_select.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-02-03 01:41:51.000000 solc-select-1.0.3/solc_select.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-02-03 01:41:51.000000 solc-select-1.0.3/solc_select.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 01:41:51.000000 solc-select-1.0.3/solc_select.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-02-03 01:41:51.000000 solc-select-1.0.3/solc_select.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-03 01:41:51.000000 solc-select-1.0.3/solc_select.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-03 01:41:51.000000 solc-select-1.0.3/solc_select.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:27:33.534569 solc-select-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    34522 2023-06-26 16:27:21.000000 solc-select-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-06-26 16:27:33.534569 solc-select-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-06-26 16:27:21.000000 solc-select-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-26 16:27:21.000000 solc-select-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 16:27:33.534569 solc-select-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-26 16:27:21.000000 solc-select-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:27:33.534569 solc-select-1.0.4/solc_select/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 16:27:21.000000 solc-select-1.0.4/solc_select/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-06-26 16:27:21.000000 solc-select-1.0.4/solc_select/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-26 16:27:21.000000 solc-select-1.0.4/solc_select/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9837 2023-06-26 16:27:21.000000 solc-select-1.0.4/solc_select/solc_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-26 16:27:21.000000 solc-select-1.0.4/solc_select/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:27:33.534569 solc-select-1.0.4/solc_select.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-06-26 16:27:33.000000 solc-select-1.0.4/solc_select.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-26 16:27:33.000000 solc-select-1.0.4/solc_select.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 16:27:33.000000 solc-select-1.0.4/solc_select.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-26 16:27:33.000000 solc-select-1.0.4/solc_select.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-26 16:27:33.000000 solc-select-1.0.4/solc_select.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-26 16:27:33.000000 solc-select-1.0.4/solc_select.egg-info/top_level.txt
```

### Comparing `solc-select-1.0.3/LICENSE` & `solc-select-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `solc-select-1.0.3/PKG-INFO` & `solc-select-1.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solc-select
-Version: 1.0.3
+Version: 1.0.4
 Summary: Manage multiple Solidity compiler versions.
 Home-page: https://github.com/crytic/solc-select
 Author: Trail of Bits
 License: AGPL-3.0
 Requires-Python: >=3.6
 License-File: LICENSE
 
@@ -14,22 +14,28 @@
 The tool is split into two CLI utilities:
 - `solc-select`: manages installing and setting different `solc` compiler versions
 - `solc`: wrapper around `solc` which picks the right version according to what was set via `solc-select`
 
 The `solc` binaries are downloaded from https://binaries.soliditylang.org/ which contains
 official artifacts for many historial and modern `solc` versions for Linux and macOS.
 
-The downloaded binaries are stored in `~/.solc-select/artifacts/`.
+The versioned binaries are stored in `~/.solc-select/artifacts/`.
 
 ## Quickstart
 
 ```
 pip3 install solc-select
 ```
 
+To automatically install and use a version, run `solc-select use <version> --always-install`. 
+
+### Running on ARM (Mac M1/M2)
+
+`solc` requires Rosetta to be installed. See the FAQ on [how to install Rosetta](#oserror-errno-86-bad-cpu-type-in-executable).
+
 ## Usage
 
 The global version of `solc` can be set with the `solc-select use <version>` command:
 ```
 $ solc --version
 solc, the solidity compiler commandline interface
 Version: 0.5.2+commit.1df8f40c.Linux.g++
@@ -64,27 +70,48 @@
 And install the one you need with `solc-select install <version>`:
 ```
 $ solc-select install 0.8.1
 Installing '0.8.1'...
 Version '0.8.1' installed.
 ```
 
+You can also install the latest version with `solc-select install latest`
+and use the latest version with `solc-select use latest`
+
 Display the currently installed versions:
 ```
 $ solc-select versions
 0.8.0
 0.4.2 (current, set by /Users/artur/.solc-select/global-version)
 ```
 
 ## Getting Help
 
 Feel free to stop by our [Slack channel](https://empirehacking.slack.com/) for help on using or extending `solc-select`.
 
 ## FAQ
 
+### OSError: [Errno 86] Bad CPU type in executable
+
+On newer `solc-select` versions, this might show as `solc binaries for macOS are
+Intel-only. Please install Rosetta on your Mac to continue.`
+
+`solc` requires Rosetta to be installed. To see whether you have Rosetta
+installed on your Mac, run
+
+```bash
+pgrep -q oahd && echo Rosetta is installed || echo Rosetta is NOT installed
+```
+
+If it is not installed, it can be installed with the command
+
+```bash
+/usr/sbin/softwareupdate --install-rosetta --agree-to-license
+```
+
 ### solc-version not changing after running `solc-select use [version]` or setting `SOLC_VERSION`
 
 Uninstall other installations of solc on your machine. `solc-select` re-installs solc binaries for your operating system and acts as a wrapper for solc. With duplicate solc installations, this may result in your `solc` version not being up to date.
 
 ### "Unsupported Platform" on Windows 
 
 The solc-select version that supports Windows is currently in beta. Uninstall `solc-select` through `pip3 uninstall solc-select` and run
```

### Comparing `solc-select-1.0.3/README.md` & `solc-select-1.0.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -4,22 +4,28 @@
 The tool is split into two CLI utilities:
 - `solc-select`: manages installing and setting different `solc` compiler versions
 - `solc`: wrapper around `solc` which picks the right version according to what was set via `solc-select`
 
 The `solc` binaries are downloaded from https://binaries.soliditylang.org/ which contains
 official artifacts for many historial and modern `solc` versions for Linux and macOS.
 
-The downloaded binaries are stored in `~/.solc-select/artifacts/`.
+The versioned binaries are stored in `~/.solc-select/artifacts/`.
 
 ## Quickstart
 
 ```
 pip3 install solc-select
 ```
 
+To automatically install and use a version, run `solc-select use <version> --always-install`. 
+
+### Running on ARM (Mac M1/M2)
+
+`solc` requires Rosetta to be installed. See the FAQ on [how to install Rosetta](#oserror-errno-86-bad-cpu-type-in-executable).
+
 ## Usage
 
 The global version of `solc` can be set with the `solc-select use <version>` command:
 ```
 $ solc --version
 solc, the solidity compiler commandline interface
 Version: 0.5.2+commit.1df8f40c.Linux.g++
@@ -54,27 +60,48 @@
 And install the one you need with `solc-select install <version>`:
 ```
 $ solc-select install 0.8.1
 Installing '0.8.1'...
 Version '0.8.1' installed.
 ```
 
+You can also install the latest version with `solc-select install latest`
+and use the latest version with `solc-select use latest`
+
 Display the currently installed versions:
 ```
 $ solc-select versions
 0.8.0
 0.4.2 (current, set by /Users/artur/.solc-select/global-version)
 ```
 
 ## Getting Help
 
 Feel free to stop by our [Slack channel](https://empirehacking.slack.com/) for help on using or extending `solc-select`.
 
 ## FAQ
 
+### OSError: [Errno 86] Bad CPU type in executable
+
+On newer `solc-select` versions, this might show as `solc binaries for macOS are
+Intel-only. Please install Rosetta on your Mac to continue.`
+
+`solc` requires Rosetta to be installed. To see whether you have Rosetta
+installed on your Mac, run
+
+```bash
+pgrep -q oahd && echo Rosetta is installed || echo Rosetta is NOT installed
+```
+
+If it is not installed, it can be installed with the command
+
+```bash
+/usr/sbin/softwareupdate --install-rosetta --agree-to-license
+```
+
 ### solc-version not changing after running `solc-select use [version]` or setting `SOLC_VERSION`
 
 Uninstall other installations of solc on your machine. `solc-select` re-installs solc binaries for your operating system and acts as a wrapper for solc. With duplicate solc installations, this may result in your `solc` version not being up to date.
 
 ### "Unsupported Platform" on Windows 
 
 The solc-select version that supports Windows is currently in beta. Uninstall `solc-select` through `pip3 uninstall solc-select` and run
```

### Comparing `solc-select-1.0.3/setup.py` & `solc-select-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 setup(
     name="solc-select",
     description="Manage multiple Solidity compiler versions.",
     url="https://github.com/crytic/solc-select",
     author="Trail of Bits",
-    version="1.0.3",
+    version="1.0.4",
     packages=find_packages(),
     python_requires=">=3.6",
     license="AGPL-3.0",
     # pylint: disable=consider-using-with
     long_description=open("README.md", encoding="utf8").read(),
     entry_points={
         "console_scripts": [
```

### Comparing `solc-select-1.0.3/solc_select/__main__.py` & `solc-select-1.0.4/solc_select/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     valid_install_arg,
     valid_version,
     get_installable_versions,
     install_artifacts,
     switch_global_version,
     current_version,
     installed_versions,
+    halt_incompatible_system,
     halt_old_architecture,
     upgrade_architecture,
 )
 
 # pylint: disable=too-many-branches
 def solc_select() -> None:
     parser = argparse.ArgumentParser()
@@ -27,15 +28,15 @@
         help="Allows users to install and quickly switch between Solidity compiler versions"
     )
     parser_install = subparsers.add_parser(
         "install", help="list and install available solc versions"
     )
     parser_install.add_argument(
         INSTALL_VERSIONS,
-        help='specific versions you want to install "0.4.25" or "all"',
+        help='specific versions you want to install "0.4.25", "all" or "latest"',
         nargs="*",
         default=[],
         type=valid_install_arg,
     )
     parser_use = subparsers.add_parser("use", help="change the version of global solc compiler")
     parser_use.add_argument(
         USE_VERSION, help="solc version you want to use (eg: 0.4.25)", type=valid_version, nargs="?"
@@ -57,35 +58,42 @@
         else:
             install_artifacts(args.get(INSTALL_VERSIONS))
 
     elif args.get(USE_VERSION) is not None:
         switch_global_version(args.get(USE_VERSION), args.get("always_install"))
 
     elif args.get(SHOW_VERSIONS) is not None:
-        res = current_version()
-        if res:
-            (current_ver, source) = res
-        for version in reversed(sorted(installed_versions())):
-            if res and version == current_ver:
-                print(f"{version} (current, set by {source})")
-            else:
-                print(version)
+        versions_installed = installed_versions()
+        if versions_installed:
+            res = current_version()
+            if res:
+                (current_ver, source) = res
+            for version in reversed(sorted(versions_installed)):
+                if res and version == current_ver:
+                    print(f"{version} (current, set by {source})")
+                else:
+                    print(version)
+        else:
+            print(
+                "No solc version installed. Run `solc-select install --help` for more information"
+            )
     elif args.get(UPGRADE) is not None:
         upgrade_architecture()
     else:
         parser.parse_args(["--help"])
         sys.exit(0)
 
 
 def solc() -> None:
     res = current_version()
     if res:
         (version, _) = res
         path = ARTIFACTS_DIR.joinpath(f"solc-{version}", f"solc-{version}")
         halt_old_architecture(path)
+        halt_incompatible_system()
         try:
             subprocess.run(
                 [str(path)] + sys.argv[1:],
                 check=True,
             )
         except subprocess.CalledProcessError as e:
             sys.exit(e.returncode)
```

### Comparing `solc-select-1.0.3/solc_select/constants.py` & `solc-select-1.0.4/solc_select/constants.py`

 * *Files identical despite different names*

### Comparing `solc-select-1.0.3/solc_select/solc_select.py` & `solc-select-1.0.4/solc_select/solc_select.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,25 +16,34 @@
     WINDOWS_AMD64,
     EARLIEST_RELEASE,
     SOLC_SELECT_DIR,
     ARTIFACTS_DIR,
     CRYTIC_SOLC_ARTIFACTS,
     CRYTIC_SOLC_JSON,
 )
+from .utils import mac_can_run_intel_binaries
 
 Path.mkdir(ARTIFACTS_DIR, parents=True, exist_ok=True)
 
 
 def halt_old_architecture(path: Path) -> None:
     if not Path.is_file(path):
         raise argparse.ArgumentTypeError(
             "solc-select is out of date. Please run `solc-select upgrade`"
         )
 
 
+def halt_incompatible_system() -> None:
+    if soliditylang_platform() == MACOSX_AMD64 and not mac_can_run_intel_binaries():
+        raise argparse.ArgumentTypeError(
+            "solc binaries for macOS are Intel-only. Please install Rosetta on your Mac to continue. Refer to the solc-select README for instructions."
+        )
+    # TODO: check for Linux aarch64 (e.g. RPi), presence of QEMU+binfmt
+
+
 def upgrade_architecture() -> None:
     currently_installed = installed_versions()
     if len(currently_installed) > 0:
         if Path.is_file(ARTIFACTS_DIR.joinpath(f"solc-{currently_installed[0]}")):
             shutil.rmtree(ARTIFACTS_DIR)
             Path.mkdir(ARTIFACTS_DIR, exist_ok=True)
             install_artifacts(currently_installed)
@@ -42,56 +51,70 @@
         else:
             print("solc-select is already up to date")
     else:
         raise argparse.ArgumentTypeError("Run `solc-select install --help` for more information")
 
 
 def current_version() -> (str, str):
-    version = os.environ.get("SOLC_VERSION")
     source = "SOLC_VERSION"
-    if version:
-        if version not in installed_versions():
-            raise argparse.ArgumentTypeError(
-                f"Version '{version}' not installed (set by {source}). Run `solc-select install {version}`."
-            )
-    else:
-        source = SOLC_SELECT_DIR.joinpath("global-version")
-        if Path.is_file(source):
-            with open(source, encoding="utf-8") as f:
+    version = os.environ.get(source)
+    if not version:
+        source_path = SOLC_SELECT_DIR.joinpath("global-version")
+        source = source_path.as_posix()
+        if Path.is_file(source_path):
+            with open(source_path, encoding="utf-8") as f:
                 version = f.read()
         else:
             raise argparse.ArgumentTypeError(
                 "No solc version set. Run `solc-select use VERSION` or set SOLC_VERSION environment variable."
             )
+    versions = installed_versions()
+    if version not in versions:
+        raise argparse.ArgumentTypeError(
+            f"\nVersion '{version}' not installed (set by {source})."
+            f"\nRun `solc-select install {version}`."
+            f"\nOr use one of the following versions: {versions}"
+        )
     return version, source
 
 
 def installed_versions() -> [str]:
     return [
         f.replace("solc-", "") for f in sorted(os.listdir(ARTIFACTS_DIR)) if f.startswith("solc-")
     ]
 
 
+def artifact_path(version: str) -> Path:
+    return ARTIFACTS_DIR.joinpath(f"solc-{version}", f"solc-{version}")
+
+
 def install_artifacts(versions: [str]) -> bool:
     releases = get_available_versions()
+    versions = [get_latest_release() if ver == "latest" else ver for ver in versions]
+
+    if "all" not in versions:
+        not_available_versions = list(set(versions).difference([*releases]))
+        if not_available_versions:
+            print(f"{', '.join(not_available_versions)} solc versions are not available.")
+            return False
 
     for version, artifact in releases.items():
         if "all" not in versions:
             if versions and version not in versions:
                 continue
 
         (url, _) = get_url(version, artifact)
 
         if is_linux_0818(version):
             url = CRYTIC_SOLC_ARTIFACTS + artifact
             print(url)
 
         artifact_file_dir = ARTIFACTS_DIR.joinpath(f"solc-{version}")
         Path.mkdir(artifact_file_dir, parents=True, exist_ok=True)
-        print(f"Installing '{version}'...")
+        print(f"Installing solc '{version}'...")
         urllib.request.urlretrieve(url, artifact_file_dir.joinpath(f"solc-{version}"))
 
         verify_checksum(version)
 
         if is_older_windows(version):
             with ZipFile(artifact_file_dir.joinpath(f"solc-{version}"), "r") as zip_ref:
                 zip_ref.extractall(path=artifact_file_dir)
@@ -180,29 +203,30 @@
         else:
             raise argparse.ArgumentTypeError(f"'{version}' must be installed prior to use.")
     else:
         raise argparse.ArgumentTypeError(f"Unknown version '{version}'")
 
 
 def valid_version(version: str) -> str:
+    if version in installed_versions():
+        return version
+    latest_release = get_latest_release()
+    if version == "latest":
+        return latest_release
     match = re.search(r"^(\d+)\.(\d+)\.(\d+)$", version)
 
     if match is None:
         raise argparse.ArgumentTypeError(f"Invalid version '{version}'.")
 
     if Version(version) < Version(EARLIEST_RELEASE[soliditylang_platform()]):
         raise argparse.ArgumentTypeError(
             f"Invalid version - only solc versions above '{EARLIEST_RELEASE[soliditylang_platform()]}' are available"
         )
 
     # pylint: disable=consider-using-with
-    (_, list_url) = get_url()
-    list_json = urllib.request.urlopen(list_url).read()
-    latest_release = json.loads(list_json)["latestRelease"]
-    # pylint: disable=consider-using-with
     if Version(version) > Version(latest_release):
         raise argparse.ArgumentTypeError(
             f"Invalid version '{latest_release}' is the latest available version"
         )
 
     return version
 
@@ -240,7 +264,14 @@
     elif sys.platform == "darwin":
         platform = MACOSX_AMD64
     elif sys.platform in ["win32", "cygwin"]:
         platform = WINDOWS_AMD64
     else:
         raise argparse.ArgumentTypeError("Unsupported platform")
     return platform
+
+
+def get_latest_release() -> str:
+    (_, list_url) = get_url()
+    list_json = urllib.request.urlopen(list_url).read()
+    latest_release = json.loads(list_json)["latestRelease"]
+    return latest_release
```

### Comparing `solc-select-1.0.3/solc_select.egg-info/PKG-INFO` & `solc-select-1.0.4/solc_select.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solc-select
-Version: 1.0.3
+Version: 1.0.4
 Summary: Manage multiple Solidity compiler versions.
 Home-page: https://github.com/crytic/solc-select
 Author: Trail of Bits
 License: AGPL-3.0
 Requires-Python: >=3.6
 License-File: LICENSE
 
@@ -14,22 +14,28 @@
 The tool is split into two CLI utilities:
 - `solc-select`: manages installing and setting different `solc` compiler versions
 - `solc`: wrapper around `solc` which picks the right version according to what was set via `solc-select`
 
 The `solc` binaries are downloaded from https://binaries.soliditylang.org/ which contains
 official artifacts for many historial and modern `solc` versions for Linux and macOS.
 
-The downloaded binaries are stored in `~/.solc-select/artifacts/`.
+The versioned binaries are stored in `~/.solc-select/artifacts/`.
 
 ## Quickstart
 
 ```
 pip3 install solc-select
 ```
 
+To automatically install and use a version, run `solc-select use <version> --always-install`. 
+
+### Running on ARM (Mac M1/M2)
+
+`solc` requires Rosetta to be installed. See the FAQ on [how to install Rosetta](#oserror-errno-86-bad-cpu-type-in-executable).
+
 ## Usage
 
 The global version of `solc` can be set with the `solc-select use <version>` command:
 ```
 $ solc --version
 solc, the solidity compiler commandline interface
 Version: 0.5.2+commit.1df8f40c.Linux.g++
@@ -64,27 +70,48 @@
 And install the one you need with `solc-select install <version>`:
 ```
 $ solc-select install 0.8.1
 Installing '0.8.1'...
 Version '0.8.1' installed.
 ```
 
+You can also install the latest version with `solc-select install latest`
+and use the latest version with `solc-select use latest`
+
 Display the currently installed versions:
 ```
 $ solc-select versions
 0.8.0
 0.4.2 (current, set by /Users/artur/.solc-select/global-version)
 ```
 
 ## Getting Help
 
 Feel free to stop by our [Slack channel](https://empirehacking.slack.com/) for help on using or extending `solc-select`.
 
 ## FAQ
 
+### OSError: [Errno 86] Bad CPU type in executable
+
+On newer `solc-select` versions, this might show as `solc binaries for macOS are
+Intel-only. Please install Rosetta on your Mac to continue.`
+
+`solc` requires Rosetta to be installed. To see whether you have Rosetta
+installed on your Mac, run
+
+```bash
+pgrep -q oahd && echo Rosetta is installed || echo Rosetta is NOT installed
+```
+
+If it is not installed, it can be installed with the command
+
+```bash
+/usr/sbin/softwareupdate --install-rosetta --agree-to-license
+```
+
 ### solc-version not changing after running `solc-select use [version]` or setting `SOLC_VERSION`
 
 Uninstall other installations of solc on your machine. `solc-select` re-installs solc binaries for your operating system and acts as a wrapper for solc. With duplicate solc installations, this may result in your `solc` version not being up to date.
 
 ### "Unsupported Platform" on Windows 
 
 The solc-select version that supports Windows is currently in beta. Uninstall `solc-select` through `pip3 uninstall solc-select` and run
```


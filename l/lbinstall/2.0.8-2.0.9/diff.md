# Comparing `tmp/lbinstall-2.0.8.tar.gz` & `tmp/lbinstall-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "public/lbinstall/lbinstall-2.0.8.tar", last modified: Fri Sep 27 10:09:05 2019, max compression
+gzip compressed data, was "public/lbinstall/lbinstall-2.0.9.tar", last modified: Tue Oct  1 14:45:01 2019, max compression
```

## Comparing `lbinstall-2.0.8.tar` & `lbinstall-2.0.9.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-09-27 10:09:05.000000 lbinstall-2.0.8/
--rw-rw-rw-   0 root         (0) root         (0)     3477 2019-09-27 10:07:37.000000 lbinstall-2.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-09-27 10:09:05.000000 lbinstall-2.0.8/lbinstall/
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-09-27 10:09:05.000000 lbinstall-2.0.8/lbinstall/test/
--rw-rw-rw-   0 root         (0) root         (0)     4775 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/test/TestInstallerUpdate.py
--rw-rw-rw-   0 root         (0) root         (0)     2787 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/test/TestInstallerRemove.py
--rw-rw-rw-   0 root         (0) root         (0)     6464 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/test/TestLbInstall.py
--rw-rw-rw-   0 root         (0) root         (0)     6732 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/test/TestComparison.py
--rw-rw-rw-   0 root         (0) root         (0)     8979 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/test/TestInstaller.py
--rw-rw-rw-   0 root         (0) root         (0)     5192 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/test/TestDependencyManager.py
--rw-rw-rw-   0 root         (0) root         (0)     2329 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/test/TestFullLbInstall.py
--rw-rw-rw-   0 root         (0) root         (0)      180 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-09-27 10:09:05.000000 lbinstall-2.0.8/lbinstall/test/dir1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-09-27 10:09:05.000000 lbinstall-2.0.8/lbinstall/test/dir1/dir3/
--rw-rw-rw-   0 root         (0) root         (0)       10 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/test/dir1/dir3/testfile.txt
--rw-rw-rw-   0 root         (0) root         (0)     3910 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/test/TestPackageManager.py
--rw-rw-rw-   0 root         (0) root         (0)    14827 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/test/TestRepo.xml
--rw-rw-rw-   0 root         (0) root         (0)     8334 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/Graph.py
--rw-rw-rw-   0 root         (0) root         (0)    10557 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/InstallAreaManager.py
--rw-rw-rw-   0 root         (0) root         (0)       14 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     8516 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/RpmTarTool.py
--rwxrwxrwx   0 root         (0) root         (0)    46866 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/DependencyManager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-09-27 10:09:05.000000 lbinstall-2.0.8/lbinstall/rpmfile/
--rw-rw-rw-   0 root         (0) root         (0)       72 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/rpmfile/README.md
--rw-rw-rw-   0 root         (0) root         (0)       85 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/rpmfile/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     6341 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/rpmfile/headers.py
--rw-rw-rw-   0 root         (0) root         (0)     1502 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/rpmfile/rpmdefs.py
--rw-rw-rw-   0 root         (0) root         (0)     2061 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/rpmfile/io_extra.py
--rw-rw-rw-   0 root         (0) root         (0)     9011 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/rpmfile/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-09-27 10:09:05.000000 lbinstall-2.0.8/lbinstall/rpmfile/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/rpmfile/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1021 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/rpmfile/tests/test_subfile.py
--rw-rw-rw-   0 root         (0) root         (0)    17725 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/rpmfile/cpiofile.py
--rw-rw-rw-   0 root         (0) root         (0)     7543 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/LCGYumConsistency.py
--rwxrwxrwx   0 root         (0) root         (0)    25243 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/LbInstall.py
--rw-rw-rw-   0 root         (0) root         (0)    15280 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/LbYumConsistency.py
--rw-rw-rw-   0 root         (0) root         (0)     5018 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/LHCbConfig.py
--rwxrwxrwx   0 root         (0) root         (0)    62685 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/Installer.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5996 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/LbRpmTarCompare.py
--rw-rw-rw-   0 root         (0) root         (0)    25027 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/PackageManager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-09-27 10:09:05.000000 lbinstall-2.0.8/lbinstall/extra/
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-09-27 10:09:05.000000 lbinstall-2.0.8/lbinstall/extra/test/
--rw-rw-rw-   0 root         (0) root         (0)     2602 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/extra/test/TestThreadPoolManager.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/extra/test/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2281 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/extra/test/TestRPMExtractor.py
--rw-rw-rw-   0 root         (0) root         (0)     2077 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/extra/test/TestInstallAreaImporter.py
--rw-rw-rw-   0 root         (0) root         (0)     6400 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/extra/Utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3298 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/extra/ThreadPoolManager.py
--rwxrwxrwx   0 root         (0) root         (0)     7000 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/extra/RPMExtractor.py
--rw-rw-rw-   0 root         (0) root         (0)     2549 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/extra/ExtractionChecker.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/extra/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    17470 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/Model.py
--rw-rw-rw-   0 root         (0) root         (0)    19499 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/YumChecker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-09-27 10:09:05.000000 lbinstall-2.0.8/lbinstall/db/
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-09-27 10:09:05.000000 lbinstall-2.0.8/lbinstall/db/test/
--rw-rw-rw-   0 root         (0) root         (0)     2970 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/db/test/TestDB.py
--rw-rw-rw-   0 root         (0) root         (0)       26 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/db/test/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     3573 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/db/test/TestDBManagerRemove.py
--rw-rw-rw-   0 root         (0) root         (0)     3980 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/db/test/TestChainedDBOps.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/db/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3518 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/db/test/TestChainedDBManager.py
--rw-rw-rw-   0 root         (0) root         (0)     2847 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/db/test/TestDBManager.py
--rw-rw-rw-   0 root         (0) root         (0)     3656 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/db/test/TestChainedDB.py
--rw-rw-rw-   0 root         (0) root         (0)     3353 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/db/test/TestDBManagerDep.py
--rw-rw-rw-   0 root         (0) root         (0)       14 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/db/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)    26097 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/db/DBManager.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/db/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4149 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/db/model.py
--rw-rw-rw-   0 root         (0) root         (0)     3621 2019-09-27 10:07:37.000000 lbinstall-2.0.8/lbinstall/db/ChainedDBManager.py
--rw-rw-rw-   0 root         (0) root         (0)     3868 2019-09-27 10:07:37.000000 lbinstall-2.0.8/.gitlab-ci.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-09-27 10:09:05.000000 lbinstall-2.0.8/lbinstall.egg-info/
--rw-r--r--   0 root         (0) root         (0)      237 2019-09-27 10:09:05.000000 lbinstall-2.0.8/lbinstall.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)     2759 2019-09-27 10:09:05.000000 lbinstall-2.0.8/lbinstall.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       10 2019-09-27 10:09:05.000000 lbinstall-2.0.8/lbinstall.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      579 2019-09-27 10:09:05.000000 lbinstall-2.0.8/lbinstall.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       30 2019-09-27 10:09:05.000000 lbinstall-2.0.8/lbinstall.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2019-09-27 10:09:05.000000 lbinstall-2.0.8/lbinstall.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)       29 2019-09-27 10:07:37.000000 lbinstall-2.0.8/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-09-27 10:09:05.000000 lbinstall-2.0.8/doc/
--rw-rw-rw-   0 root         (0) root         (0)      381 2019-09-27 10:07:37.000000 lbinstall-2.0.8/doc/Makefile
--rw-rw-rw-   0 root         (0) root         (0)   443207 2019-09-27 10:07:37.000000 lbinstall-2.0.8/doc/classes.png
--rw-rw-rw-   0 root         (0) root         (0)    72716 2019-09-27 10:07:37.000000 lbinstall-2.0.8/doc/packages.png
--rw-rw-rw-   0 root         (0) root         (0)      214 2019-09-27 10:07:37.000000 lbinstall-2.0.8/doc/LCGYumCheckTutorial.md
--rw-rw-rw-   0 root         (0) root         (0)      360 2019-09-27 10:07:37.000000 lbinstall-2.0.8/.project
--rw-r--r--   0 root         (0) root         (0)      579 2019-09-27 10:09:05.000000 lbinstall-2.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2019-09-27 10:09:05.000000 lbinstall-2.0.8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-09-27 10:09:05.000000 lbinstall-2.0.8/docs/
--rw-rw-rw-   0 root         (0) root         (0)      625 2019-09-27 10:07:37.000000 lbinstall-2.0.8/docs/Lbinstall_main.rst
--rw-rw-rw-   0 root         (0) root         (0)     7760 2019-09-27 10:07:37.000000 lbinstall-2.0.8/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)     8335 2019-09-27 10:07:37.000000 lbinstall-2.0.8/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-09-27 10:09:05.000000 lbinstall-2.0.8/docs/lbinstall.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)      163 2019-09-27 10:07:37.000000 lbinstall-2.0.8/docs/lbinstall.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2019-09-27 10:07:37.000000 lbinstall-2.0.8/docs/lbinstall.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      566 2019-09-27 10:07:37.000000 lbinstall-2.0.8/docs/lbinstall.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       26 2019-09-27 10:07:37.000000 lbinstall-2.0.8/docs/lbinstall.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2019-09-27 10:07:37.000000 lbinstall-2.0.8/docs/lbinstall.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      509 2019-09-27 10:07:37.000000 lbinstall-2.0.8/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1490 2019-09-27 10:07:37.000000 lbinstall-2.0.8/docs/lbinstall.rst
--rw-rw-rw-   0 root         (0) root         (0)      908 2019-09-27 10:07:37.000000 lbinstall-2.0.8/docs/lbinstall.extra.rst
--rw-rw-rw-   0 root         (0) root         (0)    11497 2019-09-27 10:07:37.000000 lbinstall-2.0.8/docs/Usage.rst
--rw-rw-rw-   0 root         (0) root         (0)      995 2019-09-27 10:07:37.000000 lbinstall-2.0.8/docs/Design.rst
--rw-rw-rw-   0 root         (0) root         (0)     5418 2019-09-27 10:07:37.000000 lbinstall-2.0.8/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      211 2019-09-27 10:07:37.000000 lbinstall-2.0.8/docs/Installation.rst
--rw-rw-rw-   0 root         (0) root         (0)      669 2019-09-27 10:07:37.000000 lbinstall-2.0.8/docs/lbinstall.db.rst
--rw-rw-rw-   0 root         (0) root         (0)       70 2019-09-27 10:07:37.000000 lbinstall-2.0.8/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)      423 2019-09-27 10:07:37.000000 lbinstall-2.0.8/.pydevproject
--rwxrwxrwx   0 root         (0) root         (0)     3062 2019-09-27 10:07:37.000000 lbinstall-2.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-09-27 10:09:05.000000 lbinstall-2.0.8/tools/
--rw-rw-rw-   0 root         (0) root         (0)     2469 2019-09-27 10:07:37.000000 lbinstall-2.0.8/tools/importInstallAreaPackages.py
--rw-rw-rw-   0 root         (0) root         (0)     2511 2019-09-27 10:07:37.000000 lbinstall-2.0.8/tools/listDataPackagesInstalled.py
--rw-rw-rw-   0 root         (0) root         (0)     2732 2019-09-27 10:07:37.000000 lbinstall-2.0.8/tools/checkextraction.py
--rw-rw-rw-   0 root         (0) root         (0)      666 2019-09-27 10:07:37.000000 lbinstall-2.0.8/tools/checkrpmfile.py
--rw-rw-rw-   0 root         (0) root         (0)     2358 2019-09-27 10:07:37.000000 lbinstall-2.0.8/tools/installFromJson.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-09-27 10:09:05.000000 lbinstall-2.0.8/bin/
--rwxrwxrwx   0 root         (0) root         (0)      125 2019-09-27 10:07:37.000000 lbinstall-2.0.8/bin/lbinstall
--rw-rw-rw-   0 root         (0) root         (0)      131 2019-09-27 10:07:37.000000 lbinstall-2.0.8/bin/lbtarrpmcompare
--rwxrwxrwx   0 root         (0) root         (0)      133 2019-09-27 10:07:37.000000 lbinstall-2.0.8/bin/lcgyumcheck
--rwxrwxrwx   0 root         (0) root         (0)      132 2019-09-27 10:07:37.000000 lbinstall-2.0.8/bin/lbyumcheck
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-01 14:45:01.000000 lbinstall-2.0.9/
+-rw-rw-rw-   0 root         (0) root         (0)     3477 2019-10-01 14:43:39.000000 lbinstall-2.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-01 14:45:01.000000 lbinstall-2.0.9/lbinstall/
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-01 14:45:01.000000 lbinstall-2.0.9/lbinstall/test/
+-rw-rw-rw-   0 root         (0) root         (0)     4775 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/test/TestInstallerUpdate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2787 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/test/TestInstallerRemove.py
+-rw-rw-rw-   0 root         (0) root         (0)     6464 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/test/TestLbInstall.py
+-rw-rw-rw-   0 root         (0) root         (0)     6732 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/test/TestComparison.py
+-rw-rw-rw-   0 root         (0) root         (0)     8979 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/test/TestInstaller.py
+-rw-rw-rw-   0 root         (0) root         (0)     5192 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/test/TestDependencyManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2329 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/test/TestFullLbInstall.py
+-rw-rw-rw-   0 root         (0) root         (0)      180 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-01 14:45:01.000000 lbinstall-2.0.9/lbinstall/test/dir1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-01 14:45:01.000000 lbinstall-2.0.9/lbinstall/test/dir1/dir3/
+-rw-rw-rw-   0 root         (0) root         (0)       10 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/test/dir1/dir3/testfile.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3910 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/test/TestPackageManager.py
+-rw-rw-rw-   0 root         (0) root         (0)    14827 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/test/TestRepo.xml
+-rw-rw-rw-   0 root         (0) root         (0)     8334 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/Graph.py
+-rw-rw-rw-   0 root         (0) root         (0)    10557 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/InstallAreaManager.py
+-rw-rw-rw-   0 root         (0) root         (0)       14 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     8516 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/RpmTarTool.py
+-rwxrwxrwx   0 root         (0) root         (0)    47010 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/DependencyManager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-01 14:45:01.000000 lbinstall-2.0.9/lbinstall/rpmfile/
+-rw-rw-rw-   0 root         (0) root         (0)       72 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/rpmfile/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       85 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/rpmfile/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     6341 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/rpmfile/headers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1502 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/rpmfile/rpmdefs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2061 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/rpmfile/io_extra.py
+-rw-rw-rw-   0 root         (0) root         (0)     9011 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/rpmfile/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-01 14:45:01.000000 lbinstall-2.0.9/lbinstall/rpmfile/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/rpmfile/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1021 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/rpmfile/tests/test_subfile.py
+-rw-rw-rw-   0 root         (0) root         (0)    17725 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/rpmfile/cpiofile.py
+-rw-rw-rw-   0 root         (0) root         (0)     7543 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/LCGYumConsistency.py
+-rwxrwxrwx   0 root         (0) root         (0)    25243 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/LbInstall.py
+-rw-rw-rw-   0 root         (0) root         (0)    15280 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/LbYumConsistency.py
+-rw-rw-rw-   0 root         (0) root         (0)     5018 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/LHCbConfig.py
+-rwxrwxrwx   0 root         (0) root         (0)    62685 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/Installer.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5996 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/LbRpmTarCompare.py
+-rw-rw-rw-   0 root         (0) root         (0)    25027 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/PackageManager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-01 14:45:01.000000 lbinstall-2.0.9/lbinstall/extra/
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-01 14:45:01.000000 lbinstall-2.0.9/lbinstall/extra/test/
+-rw-rw-rw-   0 root         (0) root         (0)     2602 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/extra/test/TestThreadPoolManager.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/extra/test/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2281 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/extra/test/TestRPMExtractor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2077 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/extra/test/TestInstallAreaImporter.py
+-rw-rw-rw-   0 root         (0) root         (0)     6400 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/extra/Utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3298 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/extra/ThreadPoolManager.py
+-rwxrwxrwx   0 root         (0) root         (0)     7000 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/extra/RPMExtractor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2549 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/extra/ExtractionChecker.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/extra/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    17470 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/Model.py
+-rw-rw-rw-   0 root         (0) root         (0)    19499 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/YumChecker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-01 14:45:01.000000 lbinstall-2.0.9/lbinstall/db/
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-01 14:45:01.000000 lbinstall-2.0.9/lbinstall/db/test/
+-rw-rw-rw-   0 root         (0) root         (0)     2970 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/db/test/TestDB.py
+-rw-rw-rw-   0 root         (0) root         (0)       26 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/db/test/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     3573 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/db/test/TestDBManagerRemove.py
+-rw-rw-rw-   0 root         (0) root         (0)     3980 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/db/test/TestChainedDBOps.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/db/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3518 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/db/test/TestChainedDBManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2847 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/db/test/TestDBManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     3656 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/db/test/TestChainedDB.py
+-rw-rw-rw-   0 root         (0) root         (0)     3353 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/db/test/TestDBManagerDep.py
+-rw-rw-rw-   0 root         (0) root         (0)       14 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/db/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)    26097 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/db/DBManager.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/db/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4149 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/db/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3621 2019-10-01 14:43:39.000000 lbinstall-2.0.9/lbinstall/db/ChainedDBManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     3868 2019-10-01 14:43:39.000000 lbinstall-2.0.9/.gitlab-ci.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-01 14:45:01.000000 lbinstall-2.0.9/lbinstall.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      237 2019-10-01 14:45:01.000000 lbinstall-2.0.9/lbinstall.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)     2759 2019-10-01 14:45:01.000000 lbinstall-2.0.9/lbinstall.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2019-10-01 14:45:01.000000 lbinstall-2.0.9/lbinstall.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      579 2019-10-01 14:45:01.000000 lbinstall-2.0.9/lbinstall.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       30 2019-10-01 14:45:01.000000 lbinstall-2.0.9/lbinstall.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2019-10-01 14:45:01.000000 lbinstall-2.0.9/lbinstall.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)       29 2019-10-01 14:43:39.000000 lbinstall-2.0.9/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-01 14:45:01.000000 lbinstall-2.0.9/doc/
+-rw-rw-rw-   0 root         (0) root         (0)      381 2019-10-01 14:43:39.000000 lbinstall-2.0.9/doc/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)   443207 2019-10-01 14:43:39.000000 lbinstall-2.0.9/doc/classes.png
+-rw-rw-rw-   0 root         (0) root         (0)    72716 2019-10-01 14:43:39.000000 lbinstall-2.0.9/doc/packages.png
+-rw-rw-rw-   0 root         (0) root         (0)      214 2019-10-01 14:43:39.000000 lbinstall-2.0.9/doc/LCGYumCheckTutorial.md
+-rw-rw-rw-   0 root         (0) root         (0)      360 2019-10-01 14:43:39.000000 lbinstall-2.0.9/.project
+-rw-r--r--   0 root         (0) root         (0)      579 2019-10-01 14:45:01.000000 lbinstall-2.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2019-10-01 14:45:01.000000 lbinstall-2.0.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-01 14:45:01.000000 lbinstall-2.0.9/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      625 2019-10-01 14:43:39.000000 lbinstall-2.0.9/docs/Lbinstall_main.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7760 2019-10-01 14:43:39.000000 lbinstall-2.0.9/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)     8335 2019-10-01 14:43:39.000000 lbinstall-2.0.9/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-01 14:45:01.000000 lbinstall-2.0.9/docs/lbinstall.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)      163 2019-10-01 14:43:39.000000 lbinstall-2.0.9/docs/lbinstall.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2019-10-01 14:43:39.000000 lbinstall-2.0.9/docs/lbinstall.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      566 2019-10-01 14:43:39.000000 lbinstall-2.0.9/docs/lbinstall.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       26 2019-10-01 14:43:39.000000 lbinstall-2.0.9/docs/lbinstall.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2019-10-01 14:43:39.000000 lbinstall-2.0.9/docs/lbinstall.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      509 2019-10-01 14:43:39.000000 lbinstall-2.0.9/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1490 2019-10-01 14:43:39.000000 lbinstall-2.0.9/docs/lbinstall.rst
+-rw-rw-rw-   0 root         (0) root         (0)      908 2019-10-01 14:43:39.000000 lbinstall-2.0.9/docs/lbinstall.extra.rst
+-rw-rw-rw-   0 root         (0) root         (0)    11497 2019-10-01 14:43:39.000000 lbinstall-2.0.9/docs/Usage.rst
+-rw-rw-rw-   0 root         (0) root         (0)      995 2019-10-01 14:43:39.000000 lbinstall-2.0.9/docs/Design.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5418 2019-10-01 14:43:39.000000 lbinstall-2.0.9/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      211 2019-10-01 14:43:39.000000 lbinstall-2.0.9/docs/Installation.rst
+-rw-rw-rw-   0 root         (0) root         (0)      669 2019-10-01 14:43:39.000000 lbinstall-2.0.9/docs/lbinstall.db.rst
+-rw-rw-rw-   0 root         (0) root         (0)       70 2019-10-01 14:43:39.000000 lbinstall-2.0.9/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)      423 2019-10-01 14:43:39.000000 lbinstall-2.0.9/.pydevproject
+-rwxrwxrwx   0 root         (0) root         (0)     3062 2019-10-01 14:43:39.000000 lbinstall-2.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-01 14:45:01.000000 lbinstall-2.0.9/tools/
+-rw-rw-rw-   0 root         (0) root         (0)     2469 2019-10-01 14:43:39.000000 lbinstall-2.0.9/tools/importInstallAreaPackages.py
+-rw-rw-rw-   0 root         (0) root         (0)     2511 2019-10-01 14:43:39.000000 lbinstall-2.0.9/tools/listDataPackagesInstalled.py
+-rw-rw-rw-   0 root         (0) root         (0)     2732 2019-10-01 14:43:39.000000 lbinstall-2.0.9/tools/checkextraction.py
+-rw-rw-rw-   0 root         (0) root         (0)      666 2019-10-01 14:43:39.000000 lbinstall-2.0.9/tools/checkrpmfile.py
+-rw-rw-rw-   0 root         (0) root         (0)     2358 2019-10-01 14:43:39.000000 lbinstall-2.0.9/tools/installFromJson.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-01 14:45:01.000000 lbinstall-2.0.9/bin/
+-rwxrwxrwx   0 root         (0) root         (0)      125 2019-10-01 14:43:39.000000 lbinstall-2.0.9/bin/lbinstall
+-rw-rw-rw-   0 root         (0) root         (0)      131 2019-10-01 14:43:39.000000 lbinstall-2.0.9/bin/lbtarrpmcompare
+-rwxrwxrwx   0 root         (0) root         (0)      133 2019-10-01 14:43:39.000000 lbinstall-2.0.9/bin/lcgyumcheck
+-rwxrwxrwx   0 root         (0) root         (0)      132 2019-10-01 14:43:39.000000 lbinstall-2.0.9/bin/lbyumcheck
```

### Comparing `lbinstall-2.0.8/README.md` & `lbinstall-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/lbinstall/test/TestInstallerUpdate.py` & `lbinstall-2.0.9/lbinstall/test/TestInstallerUpdate.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/lbinstall/test/TestInstallerRemove.py` & `lbinstall-2.0.9/lbinstall/test/TestInstallerRemove.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/lbinstall/test/TestLbInstall.py` & `lbinstall-2.0.9/lbinstall/test/TestLbInstall.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/lbinstall/test/TestComparison.py` & `lbinstall-2.0.9/lbinstall/test/TestComparison.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/lbinstall/test/TestInstaller.py` & `lbinstall-2.0.9/lbinstall/test/TestInstaller.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/lbinstall/test/TestDependencyManager.py` & `lbinstall-2.0.9/lbinstall/test/TestDependencyManager.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/lbinstall/test/TestFullLbInstall.py` & `lbinstall-2.0.9/lbinstall/test/TestFullLbInstall.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/lbinstall/test/TestPackageManager.py` & `lbinstall-2.0.9/lbinstall/test/TestPackageManager.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/lbinstall/test/TestRepo.xml` & `lbinstall-2.0.9/lbinstall/test/TestRepo.xml`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/lbinstall/Graph.py` & `lbinstall-2.0.9/lbinstall/Graph.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/lbinstall/InstallAreaManager.py` & `lbinstall-2.0.9/lbinstall/InstallAreaManager.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/lbinstall/RpmTarTool.py` & `lbinstall-2.0.9/lbinstall/RpmTarTool.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/lbinstall/DependencyManager.py` & `lbinstall-2.0.9/lbinstall/DependencyManager.py`

 * *Files 1% similar despite different names*

```diff
@@ -879,24 +879,27 @@
         allpackages = []
         cursor = self.mDBConnection.cursor()
         # request to find the entry in the package table
         sq = """select p.pkgkey, p.name, p.version, p.release, p.epoch,
              p.rpm_group, p.arch, p.location_href
              from packages p, provides r
              where p.pkgkey = r.pkgkey
-             and r.name = ?
-             and r.version = ? """
+             and r.name = ? """
 
-        if provide.release is not None:
-            sq += " and r.release = ? "
-            res = cursor.execute(sq, [provide.name,
-                                      provide.version,
-                                      provide.release])
+        if provide.version is not None:
+            sq += " and r.version = ? "
+            if provide.release is not None:
+                sq += " and r.release = ? "
+                res = cursor.execute(sq, [provide.name,
+                                          provide.version,
+                                          provide.release])
+            else:
+                res = cursor.execute(sq, [provide.name, provide.version])
         else:
-            res = cursor.execute(sq, [provide.name, provide.version])
+            res = cursor.execute(sq, [provide.name])
 
         # Getting the results
         for (pkgkey, pname, version, release,
              epoch, rpm_group, arch, location_href) in res:
             # Creating the package object
             pa = Package(pname, version, release,
                          epoch, None, rpm_group, arch, location_href)
```

### Comparing `lbinstall-2.0.8/lbinstall/rpmfile/headers.py` & `lbinstall-2.0.9/lbinstall/rpmfile/headers.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/lbinstall/rpmfile/rpmdefs.py` & `lbinstall-2.0.9/lbinstall/rpmfile/rpmdefs.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/lbinstall/rpmfile/io_extra.py` & `lbinstall-2.0.9/lbinstall/rpmfile/io_extra.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/lbinstall/rpmfile/__init__.py` & `lbinstall-2.0.9/lbinstall/rpmfile/__init__.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/lbinstall/rpmfile/tests/test_subfile.py` & `lbinstall-2.0.9/lbinstall/rpmfile/tests/test_subfile.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/lbinstall/rpmfile/cpiofile.py` & `lbinstall-2.0.9/lbinstall/rpmfile/cpiofile.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/lbinstall/LCGYumConsistency.py` & `lbinstall-2.0.9/lbinstall/LCGYumConsistency.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/lbinstall/LbInstall.py` & `lbinstall-2.0.9/lbinstall/LbInstall.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/lbinstall/LbYumConsistency.py` & `lbinstall-2.0.9/lbinstall/LbYumConsistency.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/lbinstall/LHCbConfig.py` & `lbinstall-2.0.9/lbinstall/LHCbConfig.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/lbinstall/Installer.py` & `lbinstall-2.0.9/lbinstall/Installer.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/lbinstall/LbRpmTarCompare.py` & `lbinstall-2.0.9/lbinstall/LbRpmTarCompare.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/lbinstall/PackageManager.py` & `lbinstall-2.0.9/lbinstall/PackageManager.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/lbinstall/extra/test/TestThreadPoolManager.py` & `lbinstall-2.0.9/lbinstall/extra/test/TestThreadPoolManager.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/lbinstall/extra/test/TestRPMExtractor.py` & `lbinstall-2.0.9/lbinstall/extra/test/TestRPMExtractor.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/lbinstall/extra/test/TestInstallAreaImporter.py` & `lbinstall-2.0.9/lbinstall/extra/test/TestInstallAreaImporter.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/lbinstall/extra/Utils.py` & `lbinstall-2.0.9/lbinstall/extra/Utils.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/lbinstall/extra/ThreadPoolManager.py` & `lbinstall-2.0.9/lbinstall/extra/ThreadPoolManager.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/lbinstall/extra/RPMExtractor.py` & `lbinstall-2.0.9/lbinstall/extra/RPMExtractor.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/lbinstall/extra/ExtractionChecker.py` & `lbinstall-2.0.9/lbinstall/extra/ExtractionChecker.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/lbinstall/Model.py` & `lbinstall-2.0.9/lbinstall/Model.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/lbinstall/YumChecker.py` & `lbinstall-2.0.9/lbinstall/YumChecker.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/lbinstall/db/test/TestDB.py` & `lbinstall-2.0.9/lbinstall/db/test/TestDB.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/lbinstall/db/test/TestDBManagerRemove.py` & `lbinstall-2.0.9/lbinstall/db/test/TestDBManagerRemove.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/lbinstall/db/test/TestChainedDBOps.py` & `lbinstall-2.0.9/lbinstall/db/test/TestChainedDBOps.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/lbinstall/db/test/TestChainedDBManager.py` & `lbinstall-2.0.9/lbinstall/db/test/TestChainedDBManager.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/lbinstall/db/test/TestDBManager.py` & `lbinstall-2.0.9/lbinstall/db/test/TestDBManager.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/lbinstall/db/test/TestChainedDB.py` & `lbinstall-2.0.9/lbinstall/db/test/TestChainedDB.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/lbinstall/db/test/TestDBManagerDep.py` & `lbinstall-2.0.9/lbinstall/db/test/TestDBManagerDep.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/lbinstall/db/DBManager.py` & `lbinstall-2.0.9/lbinstall/db/DBManager.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/lbinstall/db/model.py` & `lbinstall-2.0.9/lbinstall/db/model.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/lbinstall/db/ChainedDBManager.py` & `lbinstall-2.0.9/lbinstall/db/ChainedDBManager.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/.gitlab-ci.yml` & `lbinstall-2.0.9/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/lbinstall.egg-info/SOURCES.txt` & `lbinstall-2.0.9/lbinstall.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/lbinstall.egg-info/PKG-INFO` & `lbinstall-2.0.9/lbinstall.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: lbinstall
-Version: 2.0.8
+Version: 2.0.9
 Summary: LHCb package installation tool
 Home-page: https://gitlab.cern.ch/lhcb-core/lbinstall
 Author: CERN - LHCb Core Software
 Author-email: lhcb-core-soft@cern.ch
 License: GPL
 Description: LHCb package installation tool
 Keywords: LHCb
```

### Comparing `lbinstall-2.0.8/doc/classes.png` & `lbinstall-2.0.9/doc/classes.png`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/doc/packages.png` & `lbinstall-2.0.9/doc/packages.png`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/PKG-INFO` & `lbinstall-2.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: lbinstall
-Version: 2.0.8
+Version: 2.0.9
 Summary: LHCb package installation tool
 Home-page: https://gitlab.cern.ch/lhcb-core/lbinstall
 Author: CERN - LHCb Core Software
 Author-email: lhcb-core-soft@cern.ch
 License: GPL
 Description: LHCb package installation tool
 Keywords: LHCb
```

### Comparing `lbinstall-2.0.8/docs/Lbinstall_main.rst` & `lbinstall-2.0.9/docs/Lbinstall_main.rst`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/docs/make.bat` & `lbinstall-2.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/docs/Makefile` & `lbinstall-2.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/docs/lbinstall.egg-info/PKG-INFO` & `lbinstall-2.0.9/docs/lbinstall.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/docs/lbinstall.rst` & `lbinstall-2.0.9/docs/lbinstall.rst`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/docs/lbinstall.extra.rst` & `lbinstall-2.0.9/docs/lbinstall.extra.rst`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/docs/Usage.rst` & `lbinstall-2.0.9/docs/Usage.rst`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/docs/Design.rst` & `lbinstall-2.0.9/docs/Design.rst`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/docs/conf.py` & `lbinstall-2.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/docs/lbinstall.db.rst` & `lbinstall-2.0.9/docs/lbinstall.db.rst`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/setup.py` & `lbinstall-2.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/tools/importInstallAreaPackages.py` & `lbinstall-2.0.9/tools/importInstallAreaPackages.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/tools/listDataPackagesInstalled.py` & `lbinstall-2.0.9/tools/listDataPackagesInstalled.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/tools/checkextraction.py` & `lbinstall-2.0.9/tools/checkextraction.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/tools/checkrpmfile.py` & `lbinstall-2.0.9/tools/checkrpmfile.py`

 * *Files identical despite different names*

### Comparing `lbinstall-2.0.8/tools/installFromJson.py` & `lbinstall-2.0.9/tools/installFromJson.py`

 * *Files identical despite different names*


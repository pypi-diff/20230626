# Comparing `tmp/amici-0.9.4.tar.gz` & `tmp/amici-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/travis/build/ICB-DCM/AMICI/build/python/amici-0.9.4.tar", last modified: Mon Feb 11 10:52:33 2019, max compression
+gzip compressed data, was "/home/travis/build/ICB-DCM/AMICI/build/python/amici-0.9.5.tar", last modified: Tue Feb 26 15:58:31 2019, max compression
```

## Comparing `amici-0.9.4.tar` & `amici-0.9.5.tar`

### file list

```diff
@@ -1,668 +1,670 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2306 2019-02-11 10:47:09.000000 amici-0.9.4/README.md
--rwxrwxr-x   0 travis    (2000) travis    (2000)     9787 2019-02-11 10:47:09.000000 amici-0.9.4/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9242 2019-02-11 10:47:09.000000 amici-0.9.4/setup_clibs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-02-11 10:52:33.000000 amici-0.9.4/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      327 2019-02-11 10:47:09.000000 amici-0.9.4/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)        6 2019-02-11 10:47:09.000000 amici-0.9.4/version.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     3289 2019-02-11 10:52:33.000000 amici-0.9.4/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/sundials/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/sundials/include/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/sundials/include/cvode/
--rw-rw-r--   0 travis    (2000) travis    (2000)    15635 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/cvode/cvode_spils.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     7108 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/cvode/cvode_sparse.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     5493 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/cvode/cvode_bandpre.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3259 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/cvode/cvode_superlumt.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    34904 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/cvode/cvode.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2657 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/cvode/cvode_sptfqmr.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4537 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/cvode/cvode_klu.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3290 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/cvode/cvode_lapack.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    11368 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/cvode/cvode_direct.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2714 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/cvode/cvode_spgmr.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4093 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/cvode/cvode_diag.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2642 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/cvode/cvode_spbcgs.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2037 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/cvode/cvode_dense.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    11272 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/cvode/cvode_bbdpre.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2297 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/cvode/cvode_band.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/sundials/include/kinsol/
--rw-rw-r--   0 travis    (2000) travis    (2000)    35227 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/kinsol/kinsol.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    10365 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/kinsol/kinsol_direct.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    13749 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/kinsol/kinsol_spils.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2182 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/kinsol/kinsol_band.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     6303 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/kinsol/kinsol_sparse.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     9419 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/kinsol/kinsol_bbdpre.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2032 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/kinsol/kinsol_dense.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3759 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/kinsol/kinsol_spbcgs.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4575 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/kinsol/kinsol_klu.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3350 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/kinsol/kinsol_superlumt.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3618 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/kinsol/kinsol_spgmr.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3600 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/kinsol/kinsol_spfgmr.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3235 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/kinsol/kinsol_lapack.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3863 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/kinsol/kinsol_sptfqmr.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/sundials/include/idas/
--rw-rw-r--   0 travis    (2000) travis    (2000)   101122 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/idas/idas.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     6374 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/idas/idas_klu.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3913 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/idas/idas_spgmr.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3307 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/idas/idas_sptfqmr.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4468 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/idas/idas_superlumt.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    10774 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/idas/idas_sparse.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    20847 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/idas/idas_spils.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3286 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/idas/idas_spbcgs.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3177 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/idas/idas_dense.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4099 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/idas/idas_lapack.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    13626 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/idas/idas_bbdpre.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3767 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/idas/idas_band.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    19665 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/idas/idas_direct.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/sundials/include/nvector/
--rw-rw-r--   0 travis    (2000) travis    (2000)    13296 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/nvector/nvector_parallel.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     9159 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/nvector/nvector_parhyp.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    11218 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/nvector/nvector_openmp.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     8962 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/nvector/nvector_petsc.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    12227 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/nvector/nvector_pthreads.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    10779 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/nvector/nvector_serial.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/sundials/include/cvodes/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2779 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/cvodes/cvodes_band.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2459 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/cvodes/cvodes_dense.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    16143 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/cvodes/cvodes_direct.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4317 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/cvodes/cvodes_superlumt.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     9859 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/cvodes/cvodes_sparse.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     6382 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/cvodes/cvodes_klu.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4130 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/cvodes/cvodes_lapack.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    85245 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/cvodes/cvodes.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3774 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/cvodes/cvodes_sptfqmr.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     6880 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/cvodes/cvodes_bandpre.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3744 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/cvodes/cvodes_spbcgs.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    13593 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/cvodes/cvodes_bbdpre.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    21740 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/cvodes/cvodes_spils.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3704 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/cvodes/cvodes_spgmr.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     5182 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/cvodes/cvodes_diag.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/sundials/include/arkode/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5390 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/arkode/arkode_bandpre.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    21316 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/arkode/arkode_spils.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     8236 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/arkode/arkode_klu.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    10705 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/arkode/arkode_bbdpre.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3068 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/arkode/arkode_band.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4302 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/arkode/arkode_spfgmr.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3934 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/arkode/arkode_sptfqmr.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     5201 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/arkode/arkode_superlumt.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    14392 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/arkode/arkode_direct.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2724 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/arkode/arkode_dense.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3936 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/arkode/arkode_spgmr.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3898 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/arkode/arkode_spbcgs.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4432 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/arkode/arkode_pcg.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    62001 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/arkode/arkode.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4818 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/arkode/arkode_lapack.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     8853 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/arkode/arkode_sparse.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/sundials/include/sundials/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11844 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/sundials/sundials_spfgmr.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     8016 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/sundials/sundials_spbcgs.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    12500 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/sundials/sundials_spgmr.h
--rw-rw-r--   0 travis    (2000) travis    (2000)      189 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/sundials/sundials_config.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    10522 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/sundials/sundials_sptfqmr.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     1685 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/sundials/sundials_klu_impl.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    16923 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/sundials/sundials_nvector.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     1429 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/sundials/sundials_fnvector.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     7724 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/sundials/sundials_band.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     6280 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/sundials/sundials_pcg.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     5039 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/sundials/sundials_lapack.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     8965 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/sundials/sundials_sparse.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     1738 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/sundials/sundials_superlumt_impl.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    13357 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/sundials/sundials_iterative.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     8972 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/sundials/sundials_dense.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3752 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/sundials/sundials_types.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4515 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/sundials/sundials_math.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    13478 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/sundials/sundials_direct.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/sundials/include/ida/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3822 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/ida/ida_superlumt.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4974 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/ida/ida_klu.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    14232 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/ida/ida_spils.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2869 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/ida/ida_spgmr.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2232 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/ida/ida_sptfqmr.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3068 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/ida/ida_lapack.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2223 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/ida/ida_spbcgs.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2692 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/ida/ida_dense.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    11550 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/ida/ida_bbdpre.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    49843 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/ida/ida.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    15199 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/ida/ida_direct.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    10707 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/ida/ida_sparse.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2824 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/include/ida/ida_band.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3221 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/LICENSE
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/sundials/build/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/sundials/build/CMakeFiles/
--rw-rw-r--   0 travis    (2000) travis    (2000)      688 2019-02-11 10:48:58.000000 amici-0.9.4/amici/ThirdParty/sundials/build/CMakeFiles/feature_tests.c
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/sundials/build/CMakeFiles/3.9.2/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/sundials/build/CMakeFiles/3.9.2/CompilerIdC/
--rw-rw-r--   0 travis    (2000) travis    (2000)    17086 2019-02-11 10:48:57.000000 amici-0.9.4/amici/ThirdParty/sundials/build/CMakeFiles/3.9.2/CompilerIdC/CMakeCCompilerId.c
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/sundials/build/include/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/sundials/build/include/idas/
--rw-r--r--   0 travis    (2000) travis    (2000)   101122 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/build/include/idas/idas.h
--rw-r--r--   0 travis    (2000) travis    (2000)     6374 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/build/include/idas/idas_klu.h
--rw-r--r--   0 travis    (2000) travis    (2000)     3913 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/build/include/idas/idas_spgmr.h
--rw-r--r--   0 travis    (2000) travis    (2000)     3307 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/build/include/idas/idas_sptfqmr.h
--rw-r--r--   0 travis    (2000) travis    (2000)    44997 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/build/include/idas/idas_impl.h
--rw-r--r--   0 travis    (2000) travis    (2000)    10774 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/build/include/idas/idas_sparse.h
--rw-r--r--   0 travis    (2000) travis    (2000)    20847 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/build/include/idas/idas_spils.h
--rw-r--r--   0 travis    (2000) travis    (2000)     3286 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/build/include/idas/idas_spbcgs.h
--rw-r--r--   0 travis    (2000) travis    (2000)     3177 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/build/include/idas/idas_dense.h
--rw-r--r--   0 travis    (2000) travis    (2000)    13626 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/build/include/idas/idas_bbdpre.h
--rw-r--r--   0 travis    (2000) travis    (2000)     3767 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/build/include/idas/idas_band.h
--rw-r--r--   0 travis    (2000) travis    (2000)    19665 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/build/include/idas/idas_direct.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/sundials/build/include/nvector/
--rw-r--r--   0 travis    (2000) travis    (2000)    10779 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/build/include/nvector/nvector_serial.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/sundials/build/include/cvodes/
--rw-r--r--   0 travis    (2000) travis    (2000)     2779 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/build/include/cvodes/cvodes_band.h
--rw-r--r--   0 travis    (2000) travis    (2000)     2459 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/build/include/cvodes/cvodes_dense.h
--rw-r--r--   0 travis    (2000) travis    (2000)    16143 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/build/include/cvodes/cvodes_direct.h
--rw-r--r--   0 travis    (2000) travis    (2000)     9859 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/build/include/cvodes/cvodes_sparse.h
--rw-r--r--   0 travis    (2000) travis    (2000)     6382 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/build/include/cvodes/cvodes_klu.h
--rw-r--r--   0 travis    (2000) travis    (2000)    85245 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/build/include/cvodes/cvodes.h
--rw-r--r--   0 travis    (2000) travis    (2000)     3774 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/build/include/cvodes/cvodes_sptfqmr.h
--rw-r--r--   0 travis    (2000) travis    (2000)     6880 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/build/include/cvodes/cvodes_bandpre.h
--rw-r--r--   0 travis    (2000) travis    (2000)     3744 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/build/include/cvodes/cvodes_spbcgs.h
--rw-r--r--   0 travis    (2000) travis    (2000)    48057 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/build/include/cvodes/cvodes_impl.h
--rw-r--r--   0 travis    (2000) travis    (2000)    13593 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/build/include/cvodes/cvodes_bbdpre.h
--rw-r--r--   0 travis    (2000) travis    (2000)    21740 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/build/include/cvodes/cvodes_spils.h
--rw-r--r--   0 travis    (2000) travis    (2000)     3704 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/build/include/cvodes/cvodes_spgmr.h
--rw-r--r--   0 travis    (2000) travis    (2000)     5182 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/build/include/cvodes/cvodes_diag.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/sundials/build/include/sundials/
--rw-r--r--   0 travis    (2000) travis    (2000)    11844 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/build/include/sundials/sundials_spfgmr.h
--rw-r--r--   0 travis    (2000) travis    (2000)     8016 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/build/include/sundials/sundials_spbcgs.h
--rw-r--r--   0 travis    (2000) travis    (2000)    12500 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/build/include/sundials/sundials_spgmr.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3142 2019-02-11 10:48:58.000000 amici-0.9.4/amici/ThirdParty/sundials/build/include/sundials/sundials_config.h
--rw-r--r--   0 travis    (2000) travis    (2000)    10522 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/build/include/sundials/sundials_sptfqmr.h
--rw-r--r--   0 travis    (2000) travis    (2000)    16923 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/build/include/sundials/sundials_nvector.h
--rw-r--r--   0 travis    (2000) travis    (2000)     1429 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/build/include/sundials/sundials_fnvector.h
--rw-r--r--   0 travis    (2000) travis    (2000)     7724 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/build/include/sundials/sundials_band.h
--rw-r--r--   0 travis    (2000) travis    (2000)     6280 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/build/include/sundials/sundials_pcg.h
--rw-r--r--   0 travis    (2000) travis    (2000)     8965 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/build/include/sundials/sundials_sparse.h
--rw-r--r--   0 travis    (2000) travis    (2000)    13357 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/build/include/sundials/sundials_iterative.h
--rw-r--r--   0 travis    (2000) travis    (2000)     8972 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/build/include/sundials/sundials_dense.h
--rw-r--r--   0 travis    (2000) travis    (2000)     3752 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/build/include/sundials/sundials_types.h
--rw-r--r--   0 travis    (2000) travis    (2000)     4515 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/build/include/sundials/sundials_math.h
--rw-r--r--   0 travis    (2000) travis    (2000)    13478 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/build/include/sundials/sundials_direct.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/sundials/build/KLUTest/
--rw-rw-r--   0 travis    (2000) travis    (2000)       85 2019-02-11 10:48:58.000000 amici-0.9.4/amici/ThirdParty/sundials/build/KLUTest/ltest.c
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/sundials/src/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/sundials/src/nvec_openmp/
--rw-rw-r--   0 travis    (2000) travis    (2000)    31177 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/nvec_openmp/nvector_openmp.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     3120 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/nvec_openmp/fnvector_openmp.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4105 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/nvec_openmp/fnvector_openmp.c
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/sundials/src/nvec_parhyp/
--rw-rw-r--   0 travis    (2000) travis    (2000)    27468 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/nvec_parhyp/nvector_parhyp.c
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvode/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3776 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvode/cvode_sparse_impl.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    10537 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvode/cvode_dense.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     4677 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvode/cvode_sparse.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    20246 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvode/cvode_lapack.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    14712 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvode/cvode_spgmr.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    19410 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvode/cvode_klu.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     2937 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvode/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)    14784 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvode/cvode_sptfqmr.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     4546 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvode/cvode_direct_impl.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    17258 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvode/cvode_superlumt.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     5847 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvode/cvode_spils_impl.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    15617 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvode/cvode_bandpre.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     2544 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvode/cvode_diag_impl.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    18012 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvode/cvode_bbdpre.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    19767 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvode/cvode_spils.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    13334 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvode/cvode_direct.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    12643 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvode/cvode_diag.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    11124 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvode/cvode_band.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    24673 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvode/cvode_impl.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    23222 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvode/cvode_io.c
--rw-rw-r--   0 travis    (2000) travis    (2000)   117856 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvode/cvode.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    14569 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvode/cvode_spbcgs.c
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvode/fcmix/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2772 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvode/fcmix/fcvroot.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     1803 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvode/fcmix/fcvklu.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     3518 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvode/fcmix/fcvlapdense.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     2594 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvode/fcmix/fcvsparse.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     2473 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvode/fcmix/fcvbp.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    16030 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvode/fcmix/fcvbbd.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3856 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvode/fcmix/fcvband.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     1537 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvode/fcmix/fcvsuperlumt.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     5422 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvode/fcmix/fcvbbd.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    44359 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvode/fcmix/fcvode.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     1860 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvode/fcmix/fcvlapack.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    18789 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvode/fcmix/fcvode.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     5269 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvode/fcmix/fcvroot.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2384 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvode/fcmix/fcvewt.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     5185 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvode/fcmix/fcvpreco.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     3888 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvode/fcmix/fcvlapband.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    11183 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvode/fcmix/fcvbp.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3449 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvode/fcmix/fcvjtimes.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     3476 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvode/fcmix/fcvdense.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     2450 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvode/cvode_bandpre_impl.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2631 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvode/cvode_bbdpre_impl.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/
--rw-rw-r--   0 travis    (2000) travis    (2000)    18164 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/kinsol_spils.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    16152 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/kinsol_superlumt.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    13681 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/kinsol_spgmr.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    13652 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/kinsol_sptfqmr.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     4733 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/kinsol_sparse.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     2891 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)    11136 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/kinsol_band.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     6549 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/kinsol_spils_impl.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    18519 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/kinsol_klu.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     3215 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/kinsol_sparse_impl.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    14931 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/kinsol_spfgmr.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     4026 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/kinsol_direct_impl.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    14767 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/kinsol_direct.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    19154 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/kinsol_lapack.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    23740 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/kinsol_impl.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    13652 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/kinsol_spbcgs.c
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/fcmix/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3582 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinlapdense.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     2302 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinsparse.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     4645 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinpreco.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    14130 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinsol.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    33109 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinsol.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3489 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/fcmix/fkindense.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     4553 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinbbd.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     3693 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinband.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     1547 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinsuperlumt.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     2703 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinjtimes.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    13588 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinbbd.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3773 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinlapband.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     1599 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinlapack.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     1815 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinklu.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    10360 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/kinsol_dense.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    16936 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/kinsol_bbdpre.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    25595 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/kinsol_io.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     2770 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/kinsol_bbdpre_impl.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    70466 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/kinsol.c
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/sundials/src/idas/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11897 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/idas/idas_dense.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    42768 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/idas/idas_spils.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    20558 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/idas/idaa_io.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    22565 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/idas/idas_lapack.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    12653 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/idas/idas_band.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     2858 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/idas/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     3448 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/idas/idas_bbdpre_impl.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     5576 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/idas/idas_direct_impl.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    20596 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/idas/idas_superlumt.c
--rw-rw-r--   0 travis    (2000) travis    (2000)   203121 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/idas/idas.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    23545 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/idas/idas_klu.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    44695 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/idas/idas_ic.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    44997 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/idas/idas_impl.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    26477 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/idas/idas_bbdpre.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    12558 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/idas/idas_sparse.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    44840 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/idas/idas_io.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     8282 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/idas/idas_spils_impl.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    17953 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/idas/idas_sptfqmr.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    17413 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/idas/idas_spgmr.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    31915 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/idas/idas_direct.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    17821 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/idas/idas_spbcgs.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     4412 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/idas/idas_sparse_impl.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    89337 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/idas/idaa.c
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/sundials/src/nvec_par/
--rw-rw-r--   0 travis    (2000) travis    (2000)    25314 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/nvec_par/nvector_parallel.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     3192 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/nvec_par/fnvector_parallel.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4752 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/nvec_par/fnvector_parallel.c
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/sundials/src/nvec_ser/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3882 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/nvec_ser/fnvector_serial.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     2995 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/nvec_ser/fnvector_serial.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    21746 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/nvec_ser/nvector_serial.c
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4719 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodes_sparse_impl.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    17489 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodes_sptfqmr.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    12991 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodes_dense.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     3205 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodes_bbdpre_impl.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2912 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     2547 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodes_bandpre_impl.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    41527 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodes_spils.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    17312 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodes_bandpre.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     5969 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodes_direct_impl.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    11110 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodes_sparse.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    17243 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodes_spbcgs.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    21228 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodes_superlumt.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    48057 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodes_impl.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2534 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodes_diag_impl.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     7324 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodes_spils_impl.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    41655 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodes_io.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    17358 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodes_spgmr.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    13641 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodes_band.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    18860 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodea_io.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    76858 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodea.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    14211 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodes_diag.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    24703 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodes_klu.c
--rw-rw-r--   0 travis    (2000) travis    (2000)   246483 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodes.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    24699 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodes_lapack.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    24115 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodes_bbdpre.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    26743 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodes_direct.c
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/sundials/src/nvec_petsc/
--rw-rw-r--   0 travis    (2000) travis    (2000)    21745 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/nvec_petsc/nvector_petsc.c
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/sundials/src/nvec_pthreads/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4135 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/nvec_pthreads/fnvector_pthreads.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    81736 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/nvec_pthreads/nvector_pthreads.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     3140 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/nvec_pthreads/fnvector_pthreads.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/
--rw-rw-r--   0 travis    (2000) travis    (2000)    25841 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode_sptfqmr.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    25736 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode_spfgmr.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    89467 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode_io.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     4633 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode_sparse_impl.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    44247 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode_lapack.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    25260 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode_spbcgs.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     1608 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)    19953 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode_dense.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    21629 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode_band.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     8053 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode_spils_impl.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     7999 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode_sparse.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    19033 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode_direct.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    35954 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode_superlumt.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    42102 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode_klu.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    25348 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode_pcg.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     2289 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode_bandpre_impl.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    25462 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode_spgmr.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    37861 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode_butcher.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    15210 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode_bandpre.c
--rw-rw-r--   0 travis    (2000) travis    (2000)   213453 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     5836 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode_direct_impl.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2474 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode_bbdpre_impl.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3078 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farkband.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     2319 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farklapack.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     5216 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farkroot.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2378 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farkexpstab.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     2290 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farkklu.c
--rw-rw-r--   0 travis    (2000) travis    (2000)   102933 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farkode.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2636 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farksparsemass.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    25715 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farkbbd.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3150 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farklapdense.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     2873 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farkjtimes.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     2586 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farklapdensemass.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     2956 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farkroot.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     3545 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farklapband.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     2630 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farkadapt.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    18391 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farkbp.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2521 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farkmtimes.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     2555 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farkdensemass.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     2788 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farklapbandmass.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     2053 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farkbp.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     2746 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farkbandmass.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     3508 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farkmasspreco.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     2829 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farksparse.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     4176 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farkbbd.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     2940 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farkdense.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     1891 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farksuperlumt.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     2298 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farkewt.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    37395 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farkode.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     4040 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farkpreco.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    40041 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode_impl.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    35930 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode_spils.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    17593 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode_bbdpre.c
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/sundials/src/sundials/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6505 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/sundials/sundials_direct.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     5405 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/sundials/sundials_pcg.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    15056 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/sundials/sundials_sptfqmr.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     3217 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/sundials/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     5087 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/sundials/sundials_nvector.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    11285 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/sundials/sundials_spfgmr.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     8008 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/sundials/sundials_iterative.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     6842 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/sundials/sundials_band.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     9168 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/sundials/sundials_dense.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    21603 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/sundials/sundials_sparse.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    12796 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/sundials/sundials_spgmr.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     2765 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/sundials/sundials_math.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     9934 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/sundials/sundials_spbcgs.c
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/sundials/src/ida/
--rw-rw-r--   0 travis    (2000) travis    (2000)    19259 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/ida/ida_bbdpre.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     4457 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/ida/ida_sparse_impl.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     9311 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/ida/ida_dense.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     4323 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/ida/ida_direct_impl.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2851 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/ida/ida_bbdpre_impl.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2887 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/ida/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)    99418 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/ida/ida.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    24802 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/ida/ida_impl.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    16638 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/ida/ida_superlumt.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    17861 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/ida/ida_spils.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     9990 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/ida/ida_band.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    15114 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/ida/ida_spbcgs.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    24541 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/ida/ida_ic.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    17547 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/ida/ida_lapack.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    16438 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/ida/ida_direct.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    18328 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/ida/ida_klu.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    26856 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/ida/ida_io.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     6939 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/ida/ida_spils_impl.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    14936 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/ida/ida_spgmr.c
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/sundials/src/ida/fcmix/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2692 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/ida/fcmix/fidasparse.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    44068 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/ida/fcmix/fida.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     5399 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/ida/fcmix/fidaroot.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3772 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/ida/fcmix/fidalapband.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     1800 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/ida/fcmix/fidaklu.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     4882 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/ida/fcmix/fidabbd.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     3624 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/ida/fcmix/fidadense.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     5144 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/ida/fcmix/fidapreco.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    16910 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/ida/fcmix/fidabbd.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    20358 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/ida/fcmix/fida.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     3685 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/ida/fcmix/fidalapdense.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     2993 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/ida/fcmix/fidaroot.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     1678 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/ida/fcmix/fidalapack.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     3837 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/ida/fcmix/fidajtimes.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     3682 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/ida/fcmix/fidaband.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     1532 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/ida/fcmix/fidasuperlumt.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     2681 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/ida/fcmix/fidaewt.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    15284 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/ida/ida_sptfqmr.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     4737 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/sundials/src/ida/ida_sparse.c
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/
--rw-rw-r--   0 travis    (2000) travis    (2000)    49018 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/LICENSE.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/BTF/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/BTF/Include/
--rw-rw-r--   0 travis    (2000) travis    (2000)    12382 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/BTF/Include/btf.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     1427 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/BTF/Include/btf_internal.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/BTF/MATLAB/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3160 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/BTF/MATLAB/maxtrans.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     5805 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/BTF/MATLAB/strongcomp.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     4605 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/BTF/MATLAB/btf.c
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/BTF/Source/
--rw-rw-r--   0 travis    (2000) travis    (2000)    24167 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/BTF/Source/btf_strongcomp.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     5073 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/BTF/Source/btf_order.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    15950 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/BTF/Source/btf_maxtrans.c
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/include/
--rw-r--r--   0 travis    (2000) travis    (2000)     8361 2019-02-11 10:48:49.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/include/colamd.h
--rw-r--r--   0 travis    (2000) travis    (2000)    12382 2019-02-11 10:48:44.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/include/btf.h
--rw-r--r--   0 travis    (2000) travis    (2000)    29762 2019-02-11 10:48:57.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/include/klu.h
--rw-r--r--   0 travis    (2000) travis    (2000)    17821 2019-02-11 10:48:46.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/include/amd.h
--rw-r--r--   0 travis    (2000) travis    (2000)     8927 2019-02-11 10:48:43.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/include/SuiteSparse_config.h
--rw-r--r--   0 travis    (2000) travis    (2000)    17343 2019-02-11 10:48:48.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/include/camd.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/COLAMD/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/COLAMD/Include/
--rw-rw-r--   0 travis    (2000) travis    (2000)     8361 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/COLAMD/Include/colamd.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/COLAMD/Demo/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5871 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/COLAMD/Demo/colamd_l_example.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     5786 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/COLAMD/Demo/colamd_example.c
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/COLAMD/MATLAB/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5972 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/COLAMD/MATLAB/symamdmex.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    14048 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/COLAMD/MATLAB/colamdtestmex.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     6630 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/COLAMD/MATLAB/colamdmex.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    12718 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/COLAMD/MATLAB/symamdtestmex.c
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/COLAMD/Source/
--rw-rw-r--   0 travis    (2000) travis    (2000)   107525 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/COLAMD/Source/colamd.c
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Include/
--rw-rw-r--   0 travis    (2000) travis    (2000)    29762 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Include/klu.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     6581 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Include/klu_internal.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    19461 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Include/klu_version.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Demo/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11374 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Demo/kluldemo.c
--rw-rw-r--   0 travis    (2000) travis    (2000)      814 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Demo/klu_simple.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    11164 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Demo/kludemo.c
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/MATLAB/
--rw-rw-r--   0 travis    (2000) travis    (2000)    80061 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/MATLAB/klu_mex.c
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/User/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3258 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/User/klu_cholmod.c
--rw-rw-r--   0 travis    (2000) travis    (2000)      249 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/User/klu_cholmod.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3368 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/User/klu_l_cholmod.c
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Tcov/
--rw-rw-r--   0 travis    (2000) travis    (2000)    44021 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Tcov/klutest.c
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Source/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4261 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Source/klu_sort.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    16659 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Source/klu_diagnostics.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     8011 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Source/klu_extract.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    13209 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Source/klu_solve.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     4627 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Source/klu_scale.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     1923 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Source/klu_defaults.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    17034 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Source/klu_refactor.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     7002 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Source/klu_memory.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     1992 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Source/klu_free_numeric.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    24701 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Source/klu.c
--rw-rw-r--   0 travis    (2000) travis    (2000)      982 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Source/klu_free_symbolic.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    18700 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Source/klu_factor.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    11585 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Source/klu_analyze_given.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    16732 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Source/klu_analyze.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    15641 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Source/klu_tsolve.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    34162 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Source/klu_kernel.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     4560 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Source/klu_dump.c
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/CAMD/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/CAMD/Include/
--rw-rw-r--   0 travis    (2000) travis    (2000)     8248 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/CAMD/Include/camd_internal.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    17343 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/CAMD/Include/camd.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/CAMD/Demo/
--rw-rw-r--   0 travis    (2000) travis    (2000)      780 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/CAMD/Demo/camd_simple.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     5499 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/CAMD/Demo/camd_l_demo.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     5447 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/CAMD/Demo/camd_demo.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     6472 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/CAMD/Demo/camd_demo2.c
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/CAMD/MATLAB/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6275 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/CAMD/MATLAB/camd_mex.c
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/CAMD/Source/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1909 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_postorder.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     4885 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_aat.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     1872 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_control.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     6026 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_1.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     6125 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_order.c
--rw-rw-r--   0 travis    (2000) travis    (2000)      856 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_global.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     4338 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_info.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     5405 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_dump.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     1274 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_defaults.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    70615 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_2.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     3293 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_valid.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     3832 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_preprocess.c
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/SuiteSparse_config/
--rw-rw-r--   0 travis    (2000) travis    (2000)    16448 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/SuiteSparse_config/SuiteSparse_config.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     8927 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/SuiteSparse_config/SuiteSparse_config.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/SuiteSparse_config/xerbla/
--rw-rw-r--   0 travis    (2000) travis    (2000)       82 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/SuiteSparse_config/xerbla/xerbla.h
--rw-rw-r--   0 travis    (2000) travis    (2000)      135 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/SuiteSparse_config/xerbla/xerbla.c
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/AMD/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/AMD/Include/
--rw-rw-r--   0 travis    (2000) travis    (2000)     8238 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/AMD/Include/amd_internal.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    17821 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/AMD/Include/amd.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/AMD/Demo/
--rw-rw-r--   0 travis    (2000) travis    (2000)      731 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/AMD/Demo/amd_simple.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     6158 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/AMD/Demo/amd_demo2.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     5578 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/AMD/Demo/amd_demo.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     5635 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/AMD/Demo/amd_l_demo.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     2797 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/AMD/Demo/amd_f77wrapper.c
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/AMD/MATLAB/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5827 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/AMD/MATLAB/amd_mex.c
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/AMD/Source/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4293 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/AMD/Source/amd_info.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     3703 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/AMD/Source/amd_post_tree.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     3808 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/AMD/Source/amd_preprocess.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     1867 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/AMD/Source/amd_control.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     5012 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/AMD/Source/amd_dump.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     5509 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/AMD/Source/amd_postorder.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     6031 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/AMD/Source/amd_order.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    64825 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/AMD/Source/amd_2.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     1253 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/AMD/Source/amd_defaults.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     4847 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/AMD/Source/amd_aat.c
--rw-rw-r--   0 travis    (2000) travis    (2000)      837 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/AMD/Source/amd_global.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     5710 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/AMD/Source/amd_1.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     2980 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ThirdParty/SuiteSparse/AMD/Source/amd_valid.c
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/include/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/include/amici/
--rw-rw-r--   0 travis    (2000) travis    (2000)    18255 2019-02-11 10:47:09.000000 amici-0.9.4/amici/include/amici/model_dae.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    25734 2019-02-11 10:47:09.000000 amici-0.9.4/amici/include/amici/abstract_model.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2747 2019-02-11 10:47:09.000000 amici-0.9.4/amici/include/amici/sundials_matrix_wrapper.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     9833 2019-02-11 10:47:09.000000 amici-0.9.4/amici/include/amici/rdata.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3469 2019-02-11 10:47:09.000000 amici-0.9.4/amici/include/amici/defines.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    50129 2019-02-11 10:47:09.000000 amici-0.9.4/amici/include/amici/model.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4448 2019-02-11 10:47:09.000000 amici-0.9.4/amici/include/amici/newton_solver.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    15101 2019-02-11 10:47:09.000000 amici-0.9.4/amici/include/amici/edata.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2687 2019-02-11 10:47:09.000000 amici-0.9.4/amici/include/amici/misc.h
--rw-rw-r--   0 travis    (2000) travis    (2000)      481 2019-02-11 10:47:09.000000 amici-0.9.4/amici/include/amici/spline.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4862 2019-02-11 10:47:09.000000 amici-0.9.4/amici/include/amici/steadystateproblem.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    15261 2019-02-11 10:47:09.000000 amici-0.9.4/amici/include/amici/model_ode.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4522 2019-02-11 10:47:09.000000 amici-0.9.4/amici/include/amici/backwardproblem.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     7471 2019-02-11 10:47:09.000000 amici-0.9.4/amici/include/amici/hdf5.h
--rw-rw-r--   0 travis    (2000) travis    (2000)      818 2019-02-11 10:47:09.000000 amici-0.9.4/amici/include/amici/cblas.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     8843 2019-02-11 10:47:09.000000 amici-0.9.4/amici/include/amici/vector.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     7732 2019-02-11 10:47:09.000000 amici-0.9.4/amici/include/amici/exception.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2047 2019-02-11 10:47:09.000000 amici-0.9.4/amici/include/amici/interface_matlab.h
--rw-rw-r--   0 travis    (2000) travis    (2000)      885 2019-02-11 10:47:09.000000 amici-0.9.4/amici/include/amici/symbolic_functions.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     7951 2019-02-11 10:47:09.000000 amici-0.9.4/amici/include/amici/solver_idas.h
--rw-rw-r--   0 travis    (2000) travis    (2000)       97 2019-02-11 10:47:09.000000 amici-0.9.4/amici/include/amici/version.in.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     1675 2019-02-11 10:47:09.000000 amici-0.9.4/amici/include/amici/returndata_matlab.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    39212 2019-02-11 10:47:09.000000 amici-0.9.4/amici/include/amici/solver.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     8764 2019-02-11 10:47:09.000000 amici-0.9.4/amici/include/amici/serialization.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     7997 2019-02-11 10:47:09.000000 amici-0.9.4/amici/include/amici/solver_cvodes.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     7325 2019-02-11 10:47:09.000000 amici-0.9.4/amici/include/amici/forwardproblem.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     1764 2019-02-11 10:47:09.000000 amici-0.9.4/amici/include/amici/amici.h
--rw-rw-r--   0 travis    (2000) travis    (2000)  3081170 2019-02-11 10:52:27.000000 amici-0.9.4/amici/amici_wrap_without_hdf5.cxx
--rw-rw-r--   0 travis    (2000) travis    (2000)      675 2019-02-11 10:47:09.000000 amici-0.9.4/amici/__init__.template.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5626 2019-02-11 10:47:09.000000 amici-0.9.4/amici/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1584 2019-02-11 10:47:09.000000 amici-0.9.4/amici/plotting.py
--rw-rw-r--   0 travis    (2000) travis    (2000)  3166071 2019-02-11 10:52:33.000000 amici-0.9.4/amici/amici_wrap.cxx
--rw-rw-r--   0 travis    (2000) travis    (2000)     6150 2019-02-11 10:47:09.000000 amici-0.9.4/amici/numpy.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28556 2019-02-11 10:47:09.000000 amici-0.9.4/amici/pysb_import.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/swig/
--rw-rw-r--   0 travis    (2000) travis    (2000)      182 2019-02-11 10:47:09.000000 amici-0.9.4/amici/swig/model_dae.i
--rw-rw-r--   0 travis    (2000) travis    (2000)      169 2019-02-11 10:47:09.000000 amici-0.9.4/amici/swig/edata.i
--rw-rw-r--   0 travis    (2000) travis    (2000)     3550 2019-02-11 10:47:09.000000 amici-0.9.4/amici/swig/amici.i
--rw-rw-r--   0 travis    (2000) travis    (2000)      193 2019-02-11 10:47:09.000000 amici-0.9.4/amici/swig/solver_cvodes.i
--rw-rw-r--   0 travis    (2000) travis    (2000)      256 2019-02-11 10:47:09.000000 amici-0.9.4/amici/swig/modelname.template.i
--rw-rw-r--   0 travis    (2000) travis    (2000)      187 2019-02-11 10:47:09.000000 amici-0.9.4/amici/swig/solver_idas.i
--rw-rw-r--   0 travis    (2000) travis    (2000)      166 2019-02-11 10:47:09.000000 amici-0.9.4/amici/swig/hdf5.i
--rw-rw-r--   0 travis    (2000) travis    (2000)      201 2019-02-11 10:47:09.000000 amici-0.9.4/amici/swig/solver.i
--rw-rw-r--   0 travis    (2000) travis    (2000)      169 2019-02-11 10:47:09.000000 amici-0.9.4/amici/swig/model.i
--rw-rw-r--   0 travis    (2000) travis    (2000)      872 2019-02-11 10:47:09.000000 amici-0.9.4/amici/swig/std_unique_ptr.i
--rw-rw-r--   0 travis    (2000) travis    (2000)      184 2019-02-11 10:47:09.000000 amici-0.9.4/amici/swig/model_ode.i
--rw-rw-r--   0 travis    (2000) travis    (2000)      169 2019-02-11 10:47:09.000000 amici-0.9.4/amici/swig/rdata.i
--rw-rw-r--   0 travis    (2000) travis    (2000)       58 2019-02-11 10:47:09.000000 amici-0.9.4/amici/swig/abstract_model.i
--rw-rw-r--   0 travis    (2000) travis    (2000)      919 2019-02-11 10:47:09.000000 amici-0.9.4/amici/swig/CMakeLists_model.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     4470 2019-02-11 10:47:09.000000 amici-0.9.4/amici/swig/stdvec2numpy.h
--rw-rw-r--   0 travis    (2000) travis    (2000)        7 2019-02-11 10:52:33.000000 amici-0.9.4/amici/git_version.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     5951 2019-02-11 10:47:09.000000 amici-0.9.4/amici/setuptools.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13534 2019-02-11 10:47:09.000000 amici-0.9.4/amici/pandas.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        6 2019-02-11 10:47:09.000000 amici-0.9.4/amici/version.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     4193 2019-02-11 10:47:09.000000 amici-0.9.4/amici/setup.template.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    39835 2019-02-11 10:47:09.000000 amici-0.9.4/amici/sbml_import.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   148616 2019-02-11 10:52:33.000000 amici-0.9.4/amici/amici.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   145182 2019-02-11 10:52:27.000000 amici-0.9.4/amici/amici_without_hdf5.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici/src/
--rw-rw-r--   0 travis    (2000) travis    (2000)    22664 2019-02-11 10:47:09.000000 amici-0.9.4/amici/src/forwardproblem.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2831 2019-02-11 10:47:09.000000 amici-0.9.4/amici/src/misc.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    12874 2019-02-11 10:47:09.000000 amici-0.9.4/amici/src/steadystateproblem.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1979 2019-02-11 10:47:09.000000 amici-0.9.4/amici/src/CMakeLists.template.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     9068 2019-02-11 10:47:09.000000 amici-0.9.4/amici/src/spline.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    30923 2019-02-11 10:47:09.000000 amici-0.9.4/amici/src/solver_idas.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    35506 2019-02-11 10:47:09.000000 amici-0.9.4/amici/src/model_header.ODE_template.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    12967 2019-02-11 10:47:09.000000 amici-0.9.4/amici/src/rdata.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     5439 2019-02-11 10:47:09.000000 amici-0.9.4/amici/src/amici.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2476 2019-02-11 10:47:09.000000 amici-0.9.4/amici/src/sundials_matrix_wrapper.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    11984 2019-02-11 10:47:09.000000 amici-0.9.4/amici/src/model_ode.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    12971 2019-02-11 10:47:09.000000 amici-0.9.4/amici/src/model_dae.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    29422 2019-02-11 10:47:09.000000 amici-0.9.4/amici/src/hdf5.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     5839 2019-02-11 10:47:09.000000 amici-0.9.4/amici/src/backwardproblem.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    13839 2019-02-11 10:47:09.000000 amici-0.9.4/amici/src/symbolic_functions.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    13984 2019-02-11 10:47:09.000000 amici-0.9.4/amici/src/abstract_model.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)      168 2019-02-11 10:47:09.000000 amici-0.9.4/amici/src/wrapfunctions.template.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    29383 2019-02-11 10:47:09.000000 amici-0.9.4/amici/src/solver_cvodes.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3305 2019-02-11 10:47:09.000000 amici-0.9.4/amici/src/cblas.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    57284 2019-02-11 10:47:09.000000 amici-0.9.4/amici/src/model.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)      295 2019-02-11 10:47:09.000000 amici-0.9.4/amici/src/wrapfunctions.ODE_template.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    17033 2019-02-11 10:47:09.000000 amici-0.9.4/amici/src/newton_solver.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    12670 2019-02-11 10:47:09.000000 amici-0.9.4/amici/src/edata.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3864 2019-02-11 10:47:09.000000 amici-0.9.4/amici/src/main.template.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    22880 2019-02-11 10:47:09.000000 amici-0.9.4/amici/src/solver.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    81026 2019-02-11 10:47:09.000000 amici-0.9.4/amici/ode_export.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-11 10:52:33.000000 amici-0.9.4/amici.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)       43 2019-02-11 10:52:33.000000 amici-0.9.4/amici.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-02-11 10:52:33.000000 amici-0.9.4/amici.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)       75 2019-02-11 10:52:33.000000 amici-0.9.4/amici.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     3289 2019-02-11 10:52:33.000000 amici-0.9.4/amici.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-02-11 10:52:33.000000 amici-0.9.4/amici.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    29408 2019-02-11 10:52:33.000000 amici-0.9.4/amici.egg-info/SOURCES.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      327 2019-02-26 15:52:20.000000 amici-0.9.5/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3289 2019-02-26 15:58:31.000000 amici-0.9.5/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2306 2019-02-26 15:52:20.000000 amici-0.9.5/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/AMD/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/AMD/Demo/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5578 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/AMD/Demo/amd_demo.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6158 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/AMD/Demo/amd_demo2.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2797 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/AMD/Demo/amd_f77wrapper.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5635 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/AMD/Demo/amd_l_demo.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)      731 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/AMD/Demo/amd_simple.c
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/AMD/Include/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17821 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/AMD/Include/amd.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8238 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/AMD/Include/amd_internal.h
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/AMD/MATLAB/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5827 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/AMD/MATLAB/amd_mex.c
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/AMD/Source/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5710 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/AMD/Source/amd_1.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    64825 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/AMD/Source/amd_2.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4847 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/AMD/Source/amd_aat.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1867 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/AMD/Source/amd_control.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1253 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/AMD/Source/amd_defaults.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5012 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/AMD/Source/amd_dump.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)      837 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/AMD/Source/amd_global.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4293 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/AMD/Source/amd_info.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6031 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/AMD/Source/amd_order.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3703 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/AMD/Source/amd_post_tree.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5509 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/AMD/Source/amd_postorder.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3808 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/AMD/Source/amd_preprocess.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2980 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/AMD/Source/amd_valid.c
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/BTF/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/BTF/Include/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12382 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/BTF/Include/btf.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1427 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/BTF/Include/btf_internal.h
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/BTF/MATLAB/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4605 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/BTF/MATLAB/btf.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3160 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/BTF/MATLAB/maxtrans.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5805 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/BTF/MATLAB/strongcomp.c
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/BTF/Source/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15950 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/BTF/Source/btf_maxtrans.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5073 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/BTF/Source/btf_order.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24167 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/BTF/Source/btf_strongcomp.c
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/CAMD/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/CAMD/Demo/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5447 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/CAMD/Demo/camd_demo.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6472 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/CAMD/Demo/camd_demo2.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5499 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/CAMD/Demo/camd_l_demo.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)      780 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/CAMD/Demo/camd_simple.c
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/CAMD/Include/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17343 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/CAMD/Include/camd.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8248 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/CAMD/Include/camd_internal.h
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/CAMD/MATLAB/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6275 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/CAMD/MATLAB/camd_mex.c
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/CAMD/Source/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6026 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_1.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    70615 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_2.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4885 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_aat.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1872 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_control.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1274 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_defaults.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5405 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_dump.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)      856 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_global.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4338 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_info.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6125 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_order.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1909 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_postorder.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3832 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_preprocess.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3293 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_valid.c
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/COLAMD/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/COLAMD/Demo/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5786 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/COLAMD/Demo/colamd_example.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5871 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/COLAMD/Demo/colamd_l_example.c
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/COLAMD/Include/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8361 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/COLAMD/Include/colamd.h
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/COLAMD/MATLAB/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6630 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/COLAMD/MATLAB/colamdmex.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14048 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/COLAMD/MATLAB/colamdtestmex.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5972 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/COLAMD/MATLAB/symamdmex.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12718 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/COLAMD/MATLAB/symamdtestmex.c
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/COLAMD/Source/
+-rw-rw-r--   0 travis    (2000) travis    (2000)   107525 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/COLAMD/Source/colamd.c
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Demo/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      814 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Demo/klu_simple.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11164 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Demo/kludemo.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11374 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Demo/kluldemo.c
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Include/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29762 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Include/klu.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6581 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Include/klu_internal.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19461 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Include/klu_version.h
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/MATLAB/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    80061 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/MATLAB/klu_mex.c
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Source/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24701 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Source/klu.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16732 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Source/klu_analyze.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11585 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Source/klu_analyze_given.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1923 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Source/klu_defaults.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16659 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Source/klu_diagnostics.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4560 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Source/klu_dump.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8011 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Source/klu_extract.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18700 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Source/klu_factor.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1992 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Source/klu_free_numeric.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)      982 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Source/klu_free_symbolic.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34162 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Source/klu_kernel.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7002 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Source/klu_memory.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17034 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Source/klu_refactor.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4627 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Source/klu_scale.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13209 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Source/klu_solve.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4261 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Source/klu_sort.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15641 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Source/klu_tsolve.c
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Tcov/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    44021 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Tcov/klutest.c
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/User/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3258 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/User/klu_cholmod.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)      249 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/User/klu_cholmod.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3368 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/User/klu_l_cholmod.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    49018 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/LICENSE.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/SuiteSparse_config/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16448 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/SuiteSparse_config/SuiteSparse_config.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8927 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/SuiteSparse_config/SuiteSparse_config.h
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/SuiteSparse_config/xerbla/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      135 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/SuiteSparse_config/xerbla/xerbla.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)       82 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/SuiteSparse_config/xerbla/xerbla.h
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/include/
+-rw-r--r--   0 travis    (2000) travis    (2000)     8927 2019-02-26 15:55:52.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/include/SuiteSparse_config.h
+-rw-r--r--   0 travis    (2000) travis    (2000)    17821 2019-02-26 15:55:54.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/include/amd.h
+-rw-r--r--   0 travis    (2000) travis    (2000)    12382 2019-02-26 15:55:52.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/include/btf.h
+-rw-r--r--   0 travis    (2000) travis    (2000)    17343 2019-02-26 15:55:57.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/include/camd.h
+-rw-r--r--   0 travis    (2000) travis    (2000)     8361 2019-02-26 15:55:58.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/include/colamd.h
+-rw-r--r--   0 travis    (2000) travis    (2000)    29762 2019-02-26 15:56:06.000000 amici-0.9.5/amici/ThirdParty/SuiteSparse/include/klu.h
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/sundials/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3221 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/LICENSE
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/sundials/build/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/sundials/build/CMakeFiles/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/sundials/build/CMakeFiles/3.12.4/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/sundials/build/CMakeFiles/3.12.4/CompilerIdC/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18988 2019-02-26 15:56:06.000000 amici-0.9.5/amici/ThirdParty/sundials/build/CMakeFiles/3.12.4/CompilerIdC/CMakeCCompilerId.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)      688 2019-02-26 15:56:06.000000 amici-0.9.5/amici/ThirdParty/sundials/build/CMakeFiles/feature_tests.c
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/sundials/build/KLUTest/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       85 2019-02-26 15:56:06.000000 amici-0.9.5/amici/ThirdParty/sundials/build/KLUTest/ltest.c
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/sundials/build/include/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/sundials/build/include/cvodes/
+-rw-r--r--   0 travis    (2000) travis    (2000)    85245 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/build/include/cvodes/cvodes.h
+-rw-r--r--   0 travis    (2000) travis    (2000)     2779 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/build/include/cvodes/cvodes_band.h
+-rw-r--r--   0 travis    (2000) travis    (2000)     6880 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/build/include/cvodes/cvodes_bandpre.h
+-rw-r--r--   0 travis    (2000) travis    (2000)    13593 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/build/include/cvodes/cvodes_bbdpre.h
+-rw-r--r--   0 travis    (2000) travis    (2000)     2459 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/build/include/cvodes/cvodes_dense.h
+-rw-r--r--   0 travis    (2000) travis    (2000)     5182 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/build/include/cvodes/cvodes_diag.h
+-rw-r--r--   0 travis    (2000) travis    (2000)    16143 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/build/include/cvodes/cvodes_direct.h
+-rw-r--r--   0 travis    (2000) travis    (2000)    48057 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/build/include/cvodes/cvodes_impl.h
+-rw-r--r--   0 travis    (2000) travis    (2000)     6382 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/build/include/cvodes/cvodes_klu.h
+-rw-r--r--   0 travis    (2000) travis    (2000)     9859 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/build/include/cvodes/cvodes_sparse.h
+-rw-r--r--   0 travis    (2000) travis    (2000)     3744 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/build/include/cvodes/cvodes_spbcgs.h
+-rw-r--r--   0 travis    (2000) travis    (2000)     3704 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/build/include/cvodes/cvodes_spgmr.h
+-rw-r--r--   0 travis    (2000) travis    (2000)    21740 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/build/include/cvodes/cvodes_spils.h
+-rw-r--r--   0 travis    (2000) travis    (2000)     3774 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/build/include/cvodes/cvodes_sptfqmr.h
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/sundials/build/include/idas/
+-rw-r--r--   0 travis    (2000) travis    (2000)   101122 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/build/include/idas/idas.h
+-rw-r--r--   0 travis    (2000) travis    (2000)     3767 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/build/include/idas/idas_band.h
+-rw-r--r--   0 travis    (2000) travis    (2000)    13626 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/build/include/idas/idas_bbdpre.h
+-rw-r--r--   0 travis    (2000) travis    (2000)     3177 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/build/include/idas/idas_dense.h
+-rw-r--r--   0 travis    (2000) travis    (2000)    19665 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/build/include/idas/idas_direct.h
+-rw-r--r--   0 travis    (2000) travis    (2000)    44997 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/build/include/idas/idas_impl.h
+-rw-r--r--   0 travis    (2000) travis    (2000)     6374 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/build/include/idas/idas_klu.h
+-rw-r--r--   0 travis    (2000) travis    (2000)    10774 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/build/include/idas/idas_sparse.h
+-rw-r--r--   0 travis    (2000) travis    (2000)     3286 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/build/include/idas/idas_spbcgs.h
+-rw-r--r--   0 travis    (2000) travis    (2000)     3913 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/build/include/idas/idas_spgmr.h
+-rw-r--r--   0 travis    (2000) travis    (2000)    20847 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/build/include/idas/idas_spils.h
+-rw-r--r--   0 travis    (2000) travis    (2000)     3307 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/build/include/idas/idas_sptfqmr.h
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/sundials/build/include/nvector/
+-rw-r--r--   0 travis    (2000) travis    (2000)    10779 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/build/include/nvector/nvector_serial.h
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/sundials/build/include/sundials/
+-rw-r--r--   0 travis    (2000) travis    (2000)     7724 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/build/include/sundials/sundials_band.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3142 2019-02-26 15:56:06.000000 amici-0.9.5/amici/ThirdParty/sundials/build/include/sundials/sundials_config.h
+-rw-r--r--   0 travis    (2000) travis    (2000)     8972 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/build/include/sundials/sundials_dense.h
+-rw-r--r--   0 travis    (2000) travis    (2000)    13478 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/build/include/sundials/sundials_direct.h
+-rw-r--r--   0 travis    (2000) travis    (2000)     1429 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/build/include/sundials/sundials_fnvector.h
+-rw-r--r--   0 travis    (2000) travis    (2000)    13357 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/build/include/sundials/sundials_iterative.h
+-rw-r--r--   0 travis    (2000) travis    (2000)     4515 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/build/include/sundials/sundials_math.h
+-rw-r--r--   0 travis    (2000) travis    (2000)    16923 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/build/include/sundials/sundials_nvector.h
+-rw-r--r--   0 travis    (2000) travis    (2000)     6280 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/build/include/sundials/sundials_pcg.h
+-rw-r--r--   0 travis    (2000) travis    (2000)     8965 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/build/include/sundials/sundials_sparse.h
+-rw-r--r--   0 travis    (2000) travis    (2000)     8016 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/build/include/sundials/sundials_spbcgs.h
+-rw-r--r--   0 travis    (2000) travis    (2000)    11844 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/build/include/sundials/sundials_spfgmr.h
+-rw-r--r--   0 travis    (2000) travis    (2000)    12500 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/build/include/sundials/sundials_spgmr.h
+-rw-r--r--   0 travis    (2000) travis    (2000)    10522 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/build/include/sundials/sundials_sptfqmr.h
+-rw-r--r--   0 travis    (2000) travis    (2000)     3752 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/build/include/sundials/sundials_types.h
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/sundials/include/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/sundials/include/arkode/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    62001 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/arkode/arkode.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3068 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/arkode/arkode_band.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5390 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/arkode/arkode_bandpre.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10705 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/arkode/arkode_bbdpre.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2724 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/arkode/arkode_dense.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14392 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/arkode/arkode_direct.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8236 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/arkode/arkode_klu.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4818 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/arkode/arkode_lapack.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4432 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/arkode/arkode_pcg.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8853 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/arkode/arkode_sparse.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3898 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/arkode/arkode_spbcgs.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4302 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/arkode/arkode_spfgmr.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3936 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/arkode/arkode_spgmr.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21316 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/arkode/arkode_spils.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3934 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/arkode/arkode_sptfqmr.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5201 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/arkode/arkode_superlumt.h
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/sundials/include/cvode/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34904 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/cvode/cvode.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2297 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/cvode/cvode_band.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5493 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/cvode/cvode_bandpre.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11272 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/cvode/cvode_bbdpre.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2037 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/cvode/cvode_dense.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4093 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/cvode/cvode_diag.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11368 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/cvode/cvode_direct.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4537 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/cvode/cvode_klu.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3290 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/cvode/cvode_lapack.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7108 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/cvode/cvode_sparse.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2642 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/cvode/cvode_spbcgs.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2714 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/cvode/cvode_spgmr.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15635 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/cvode/cvode_spils.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2657 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/cvode/cvode_sptfqmr.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3259 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/cvode/cvode_superlumt.h
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/sundials/include/cvodes/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    85245 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/cvodes/cvodes.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2779 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/cvodes/cvodes_band.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6880 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/cvodes/cvodes_bandpre.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13593 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/cvodes/cvodes_bbdpre.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2459 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/cvodes/cvodes_dense.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5182 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/cvodes/cvodes_diag.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16143 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/cvodes/cvodes_direct.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6382 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/cvodes/cvodes_klu.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4130 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/cvodes/cvodes_lapack.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9859 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/cvodes/cvodes_sparse.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3744 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/cvodes/cvodes_spbcgs.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3704 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/cvodes/cvodes_spgmr.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21740 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/cvodes/cvodes_spils.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3774 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/cvodes/cvodes_sptfqmr.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4317 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/cvodes/cvodes_superlumt.h
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/sundials/include/ida/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    49843 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/ida/ida.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2824 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/ida/ida_band.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11550 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/ida/ida_bbdpre.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2692 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/ida/ida_dense.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15199 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/ida/ida_direct.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4974 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/ida/ida_klu.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3068 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/ida/ida_lapack.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10707 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/ida/ida_sparse.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2223 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/ida/ida_spbcgs.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2869 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/ida/ida_spgmr.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14232 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/ida/ida_spils.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2232 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/ida/ida_sptfqmr.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3822 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/ida/ida_superlumt.h
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/sundials/include/idas/
+-rw-rw-r--   0 travis    (2000) travis    (2000)   101122 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/idas/idas.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3767 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/idas/idas_band.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13626 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/idas/idas_bbdpre.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3177 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/idas/idas_dense.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19665 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/idas/idas_direct.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6374 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/idas/idas_klu.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4099 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/idas/idas_lapack.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10774 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/idas/idas_sparse.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3286 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/idas/idas_spbcgs.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3913 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/idas/idas_spgmr.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20847 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/idas/idas_spils.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3307 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/idas/idas_sptfqmr.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4468 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/idas/idas_superlumt.h
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/sundials/include/kinsol/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35227 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/kinsol/kinsol.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2182 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/kinsol/kinsol_band.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9419 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/kinsol/kinsol_bbdpre.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2032 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/kinsol/kinsol_dense.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10365 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/kinsol/kinsol_direct.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4575 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/kinsol/kinsol_klu.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3235 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/kinsol/kinsol_lapack.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6303 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/kinsol/kinsol_sparse.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3759 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/kinsol/kinsol_spbcgs.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3600 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/kinsol/kinsol_spfgmr.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3618 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/kinsol/kinsol_spgmr.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13749 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/kinsol/kinsol_spils.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3863 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/kinsol/kinsol_sptfqmr.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3350 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/kinsol/kinsol_superlumt.h
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/sundials/include/nvector/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11218 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/nvector/nvector_openmp.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13296 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/nvector/nvector_parallel.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9159 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/nvector/nvector_parhyp.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8962 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/nvector/nvector_petsc.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12227 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/nvector/nvector_pthreads.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10779 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/nvector/nvector_serial.h
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/sundials/include/sundials/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7724 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/sundials/sundials_band.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)      189 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/sundials/sundials_config.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8972 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/sundials/sundials_dense.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13478 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/sundials/sundials_direct.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1429 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/sundials/sundials_fnvector.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13357 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/sundials/sundials_iterative.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1685 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/sundials/sundials_klu_impl.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5039 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/sundials/sundials_lapack.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4515 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/sundials/sundials_math.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16923 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/sundials/sundials_nvector.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6280 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/sundials/sundials_pcg.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8965 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/sundials/sundials_sparse.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8016 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/sundials/sundials_spbcgs.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11844 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/sundials/sundials_spfgmr.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12500 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/sundials/sundials_spgmr.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10522 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/sundials/sundials_sptfqmr.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1738 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/sundials/sundials_superlumt_impl.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3752 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/include/sundials/sundials_types.h
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/sundials/src/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1608 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)   213453 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21629 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode_band.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15210 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode_bandpre.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2289 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode_bandpre_impl.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17593 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode_bbdpre.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2474 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode_bbdpre_impl.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37861 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode_butcher.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19953 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode_dense.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19033 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode_direct.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5836 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode_direct_impl.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    40041 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode_impl.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    89467 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode_io.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42102 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode_klu.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    44247 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode_lapack.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25348 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode_pcg.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7999 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode_sparse.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4633 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode_sparse_impl.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25260 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode_spbcgs.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25736 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode_spfgmr.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25462 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode_spgmr.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35930 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode_spils.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8053 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode_spils_impl.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25841 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode_sptfqmr.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35954 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode_superlumt.c
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2630 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farkadapt.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3078 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farkband.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2746 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farkbandmass.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4176 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farkbbd.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25715 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farkbbd.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2053 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farkbp.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18391 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farkbp.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2940 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farkdense.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2555 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farkdensemass.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2298 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farkewt.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2378 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farkexpstab.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2873 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farkjtimes.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2290 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farkklu.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2319 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farklapack.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3545 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farklapband.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2788 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farklapbandmass.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3150 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farklapdense.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2586 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farklapdensemass.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3508 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farkmasspreco.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2521 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farkmtimes.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37395 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farkode.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)   102933 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farkode.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4040 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farkpreco.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2956 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farkroot.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5216 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farkroot.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2829 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farksparse.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2636 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farksparsemass.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1891 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farksuperlumt.c
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvode/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2937 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvode/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)   117856 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvode/cvode.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11124 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvode/cvode_band.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15617 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvode/cvode_bandpre.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2450 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvode/cvode_bandpre_impl.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18012 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvode/cvode_bbdpre.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2631 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvode/cvode_bbdpre_impl.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10537 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvode/cvode_dense.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12643 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvode/cvode_diag.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2544 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvode/cvode_diag_impl.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13334 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvode/cvode_direct.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4546 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvode/cvode_direct_impl.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24673 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvode/cvode_impl.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23222 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvode/cvode_io.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19410 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvode/cvode_klu.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20246 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvode/cvode_lapack.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4677 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvode/cvode_sparse.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3776 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvode/cvode_sparse_impl.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14569 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvode/cvode_spbcgs.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14712 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvode/cvode_spgmr.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19767 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvode/cvode_spils.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5847 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvode/cvode_spils_impl.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14784 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvode/cvode_sptfqmr.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17258 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvode/cvode_superlumt.c
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvode/fcmix/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3856 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvode/fcmix/fcvband.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5422 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvode/fcmix/fcvbbd.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16030 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvode/fcmix/fcvbbd.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2473 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvode/fcmix/fcvbp.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11183 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvode/fcmix/fcvbp.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3476 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvode/fcmix/fcvdense.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2384 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvode/fcmix/fcvewt.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3449 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvode/fcmix/fcvjtimes.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1803 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvode/fcmix/fcvklu.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1860 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvode/fcmix/fcvlapack.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3888 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvode/fcmix/fcvlapband.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3518 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvode/fcmix/fcvlapdense.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18789 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvode/fcmix/fcvode.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    44359 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvode/fcmix/fcvode.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5185 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvode/fcmix/fcvpreco.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2772 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvode/fcmix/fcvroot.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5269 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvode/fcmix/fcvroot.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2594 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvode/fcmix/fcvsparse.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1537 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvode/fcmix/fcvsuperlumt.c
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2912 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)    76858 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodea.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18860 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodea_io.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)   246483 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodes.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13641 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodes_band.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17312 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodes_bandpre.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2547 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodes_bandpre_impl.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24115 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodes_bbdpre.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3205 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodes_bbdpre_impl.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12991 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodes_dense.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14211 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodes_diag.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2534 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodes_diag_impl.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26743 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodes_direct.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5969 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodes_direct_impl.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48057 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodes_impl.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41655 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodes_io.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24703 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodes_klu.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24699 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodes_lapack.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11110 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodes_sparse.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4719 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodes_sparse_impl.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17243 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodes_spbcgs.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17358 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodes_spgmr.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41527 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodes_spils.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7324 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodes_spils_impl.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17489 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodes_sptfqmr.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21228 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodes_superlumt.c
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/sundials/src/ida/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2887 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/ida/LICENSE
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/sundials/src/ida/fcmix/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20358 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/ida/fcmix/fida.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    44068 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/ida/fcmix/fida.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3682 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/ida/fcmix/fidaband.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4882 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/ida/fcmix/fidabbd.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16910 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/ida/fcmix/fidabbd.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3624 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/ida/fcmix/fidadense.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2681 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/ida/fcmix/fidaewt.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3837 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/ida/fcmix/fidajtimes.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1800 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/ida/fcmix/fidaklu.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1678 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/ida/fcmix/fidalapack.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3772 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/ida/fcmix/fidalapband.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3685 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/ida/fcmix/fidalapdense.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5144 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/ida/fcmix/fidapreco.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2993 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/ida/fcmix/fidaroot.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5399 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/ida/fcmix/fidaroot.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2692 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/ida/fcmix/fidasparse.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1532 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/ida/fcmix/fidasuperlumt.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    99418 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/ida/ida.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9990 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/ida/ida_band.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19259 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/ida/ida_bbdpre.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2851 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/ida/ida_bbdpre_impl.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9311 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/ida/ida_dense.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16438 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/ida/ida_direct.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4323 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/ida/ida_direct_impl.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24541 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/ida/ida_ic.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24802 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/ida/ida_impl.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26856 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/ida/ida_io.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18328 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/ida/ida_klu.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17547 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/ida/ida_lapack.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4737 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/ida/ida_sparse.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4457 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/ida/ida_sparse_impl.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15114 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/ida/ida_spbcgs.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14936 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/ida/ida_spgmr.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17861 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/ida/ida_spils.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6939 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/ida/ida_spils_impl.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15284 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/ida/ida_sptfqmr.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16638 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/ida/ida_superlumt.c
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/sundials/src/idas/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2858 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/idas/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)    89337 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/idas/idaa.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20558 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/idas/idaa_io.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)   203121 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/idas/idas.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12653 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/idas/idas_band.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26477 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/idas/idas_bbdpre.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3448 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/idas/idas_bbdpre_impl.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11897 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/idas/idas_dense.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    31915 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/idas/idas_direct.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5576 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/idas/idas_direct_impl.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    44695 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/idas/idas_ic.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    44997 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/idas/idas_impl.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    44840 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/idas/idas_io.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23545 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/idas/idas_klu.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22565 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/idas/idas_lapack.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12558 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/idas/idas_sparse.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4412 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/idas/idas_sparse_impl.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17821 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/idas/idas_spbcgs.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17413 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/idas/idas_spgmr.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42768 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/idas/idas_spils.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8282 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/idas/idas_spils_impl.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17953 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/idas/idas_sptfqmr.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20596 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/idas/idas_superlumt.c
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2891 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/LICENSE
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/fcmix/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3693 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinband.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4553 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinbbd.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13588 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinbbd.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3489 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/fcmix/fkindense.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2703 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinjtimes.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1815 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinklu.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1599 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinlapack.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3773 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinlapband.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3582 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinlapdense.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4645 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinpreco.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14130 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinsol.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    33109 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinsol.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2302 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinsparse.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1547 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinsuperlumt.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    70466 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/kinsol.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11136 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/kinsol_band.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16936 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/kinsol_bbdpre.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2770 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/kinsol_bbdpre_impl.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10360 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/kinsol_dense.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14767 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/kinsol_direct.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4026 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/kinsol_direct_impl.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23740 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/kinsol_impl.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25595 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/kinsol_io.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18519 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/kinsol_klu.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19154 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/kinsol_lapack.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4733 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/kinsol_sparse.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3215 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/kinsol_sparse_impl.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13652 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/kinsol_spbcgs.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14931 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/kinsol_spfgmr.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13681 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/kinsol_spgmr.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18164 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/kinsol_spils.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6549 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/kinsol_spils_impl.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13652 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/kinsol_sptfqmr.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16152 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/kinsol_superlumt.c
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/sundials/src/nvec_openmp/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4105 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/nvec_openmp/fnvector_openmp.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3120 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/nvec_openmp/fnvector_openmp.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    31177 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/nvec_openmp/nvector_openmp.c
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/sundials/src/nvec_par/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4752 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/nvec_par/fnvector_parallel.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3192 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/nvec_par/fnvector_parallel.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25314 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/nvec_par/nvector_parallel.c
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/sundials/src/nvec_parhyp/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27468 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/nvec_parhyp/nvector_parhyp.c
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/sundials/src/nvec_petsc/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21745 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/nvec_petsc/nvector_petsc.c
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/sundials/src/nvec_pthreads/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4135 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/nvec_pthreads/fnvector_pthreads.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3140 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/nvec_pthreads/fnvector_pthreads.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    81736 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/nvec_pthreads/nvector_pthreads.c
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/sundials/src/nvec_ser/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3882 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/nvec_ser/fnvector_serial.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2995 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/nvec_ser/fnvector_serial.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21746 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/nvec_ser/nvector_serial.c
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/ThirdParty/sundials/src/sundials/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3217 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/sundials/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6842 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/sundials/sundials_band.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9168 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/sundials/sundials_dense.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6505 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/sundials/sundials_direct.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8008 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/sundials/sundials_iterative.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2765 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/sundials/sundials_math.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5087 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/sundials/sundials_nvector.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5405 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/sundials/sundials_pcg.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21603 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/sundials/sundials_sparse.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9934 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/sundials/sundials_spbcgs.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11285 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/sundials/sundials_spfgmr.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12796 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/sundials/sundials_spgmr.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15056 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ThirdParty/sundials/src/sundials/sundials_sptfqmr.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5790 2019-02-26 15:52:20.000000 amici-0.9.5/amici/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      675 2019-02-26 15:52:20.000000 amici-0.9.5/amici/__init__.template.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   148616 2019-02-26 15:58:31.000000 amici-0.9.5/amici/amici.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   145182 2019-02-26 15:58:26.000000 amici-0.9.5/amici/amici_without_hdf5.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)  3166071 2019-02-26 15:58:31.000000 amici-0.9.5/amici/amici_wrap.cxx
+-rw-rw-r--   0 travis    (2000) travis    (2000)  3081170 2019-02-26 15:58:26.000000 amici-0.9.5/amici/amici_wrap_without_hdf5.cxx
+-rw-rw-r--   0 travis    (2000) travis    (2000)        7 2019-02-26 15:58:31.000000 amici-0.9.5/amici/git_version.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/include/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/include/amici/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25734 2019-02-26 15:52:20.000000 amici-0.9.5/amici/include/amici/abstract_model.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1764 2019-02-26 15:52:20.000000 amici-0.9.5/amici/include/amici/amici.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4522 2019-02-26 15:52:20.000000 amici-0.9.5/amici/include/amici/backwardproblem.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)      818 2019-02-26 15:52:20.000000 amici-0.9.5/amici/include/amici/cblas.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3469 2019-02-26 15:52:20.000000 amici-0.9.5/amici/include/amici/defines.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15101 2019-02-26 15:52:20.000000 amici-0.9.5/amici/include/amici/edata.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7732 2019-02-26 15:52:20.000000 amici-0.9.5/amici/include/amici/exception.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7325 2019-02-26 15:52:20.000000 amici-0.9.5/amici/include/amici/forwardproblem.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7471 2019-02-26 15:52:20.000000 amici-0.9.5/amici/include/amici/hdf5.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2047 2019-02-26 15:52:20.000000 amici-0.9.5/amici/include/amici/interface_matlab.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2687 2019-02-26 15:52:20.000000 amici-0.9.5/amici/include/amici/misc.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    50129 2019-02-26 15:52:20.000000 amici-0.9.5/amici/include/amici/model.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18255 2019-02-26 15:52:20.000000 amici-0.9.5/amici/include/amici/model_dae.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15261 2019-02-26 15:52:20.000000 amici-0.9.5/amici/include/amici/model_ode.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4448 2019-02-26 15:52:20.000000 amici-0.9.5/amici/include/amici/newton_solver.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9833 2019-02-26 15:52:20.000000 amici-0.9.5/amici/include/amici/rdata.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1675 2019-02-26 15:52:20.000000 amici-0.9.5/amici/include/amici/returndata_matlab.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8764 2019-02-26 15:52:20.000000 amici-0.9.5/amici/include/amici/serialization.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    39212 2019-02-26 15:52:20.000000 amici-0.9.5/amici/include/amici/solver.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7997 2019-02-26 15:52:20.000000 amici-0.9.5/amici/include/amici/solver_cvodes.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7951 2019-02-26 15:52:20.000000 amici-0.9.5/amici/include/amici/solver_idas.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)      481 2019-02-26 15:52:20.000000 amici-0.9.5/amici/include/amici/spline.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4862 2019-02-26 15:52:20.000000 amici-0.9.5/amici/include/amici/steadystateproblem.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2747 2019-02-26 15:52:20.000000 amici-0.9.5/amici/include/amici/sundials_matrix_wrapper.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)      885 2019-02-26 15:52:20.000000 amici-0.9.5/amici/include/amici/symbolic_functions.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8843 2019-02-26 15:52:20.000000 amici-0.9.5/amici/include/amici/vector.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)       97 2019-02-26 15:52:20.000000 amici-0.9.5/amici/include/amici/version.in.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6150 2019-02-26 15:52:20.000000 amici-0.9.5/amici/numpy.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    82144 2019-02-26 15:52:20.000000 amici-0.9.5/amici/ode_export.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19041 2019-02-26 15:52:20.000000 amici-0.9.5/amici/pandas.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1584 2019-02-26 15:52:20.000000 amici-0.9.5/amici/plotting.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34479 2019-02-26 15:52:20.000000 amici-0.9.5/amici/pysb_import.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    38571 2019-02-26 15:52:20.000000 amici-0.9.5/amici/sbml_import.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4193 2019-02-26 15:52:20.000000 amici-0.9.5/amici/setup.template.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5951 2019-02-26 15:52:20.000000 amici-0.9.5/amici/setuptools.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/src/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1979 2019-02-26 15:52:20.000000 amici-0.9.5/amici/src/CMakeLists.template.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13984 2019-02-26 15:52:20.000000 amici-0.9.5/amici/src/abstract_model.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5439 2019-02-26 15:52:20.000000 amici-0.9.5/amici/src/amici.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5838 2019-02-26 15:52:20.000000 amici-0.9.5/amici/src/backwardproblem.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3305 2019-02-26 15:52:20.000000 amici-0.9.5/amici/src/cblas.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12670 2019-02-26 15:52:20.000000 amici-0.9.5/amici/src/edata.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22664 2019-02-26 15:52:20.000000 amici-0.9.5/amici/src/forwardproblem.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29422 2019-02-26 15:52:20.000000 amici-0.9.5/amici/src/hdf5.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3864 2019-02-26 15:52:20.000000 amici-0.9.5/amici/src/main.template.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2831 2019-02-26 15:52:20.000000 amici-0.9.5/amici/src/misc.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    57284 2019-02-26 15:52:20.000000 amici-0.9.5/amici/src/model.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12971 2019-02-26 15:52:20.000000 amici-0.9.5/amici/src/model_dae.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35506 2019-02-26 15:52:20.000000 amici-0.9.5/amici/src/model_header.ODE_template.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11984 2019-02-26 15:52:20.000000 amici-0.9.5/amici/src/model_ode.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17051 2019-02-26 15:52:20.000000 amici-0.9.5/amici/src/newton_solver.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12967 2019-02-26 15:52:20.000000 amici-0.9.5/amici/src/rdata.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22880 2019-02-26 15:52:20.000000 amici-0.9.5/amici/src/solver.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29383 2019-02-26 15:52:20.000000 amici-0.9.5/amici/src/solver_cvodes.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30923 2019-02-26 15:52:20.000000 amici-0.9.5/amici/src/solver_idas.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9068 2019-02-26 15:52:20.000000 amici-0.9.5/amici/src/spline.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12874 2019-02-26 15:52:20.000000 amici-0.9.5/amici/src/steadystateproblem.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2476 2019-02-26 15:52:20.000000 amici-0.9.5/amici/src/sundials_matrix_wrapper.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13839 2019-02-26 15:52:20.000000 amici-0.9.5/amici/src/symbolic_functions.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)      295 2019-02-26 15:52:20.000000 amici-0.9.5/amici/src/wrapfunctions.ODE_template.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)      168 2019-02-26 15:52:20.000000 amici-0.9.5/amici/src/wrapfunctions.template.cpp
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici/swig/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      919 2019-02-26 15:52:20.000000 amici-0.9.5/amici/swig/CMakeLists_model.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       58 2019-02-26 15:52:20.000000 amici-0.9.5/amici/swig/abstract_model.i
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3550 2019-02-26 15:52:20.000000 amici-0.9.5/amici/swig/amici.i
+-rw-rw-r--   0 travis    (2000) travis    (2000)      169 2019-02-26 15:52:20.000000 amici-0.9.5/amici/swig/edata.i
+-rw-rw-r--   0 travis    (2000) travis    (2000)      166 2019-02-26 15:52:20.000000 amici-0.9.5/amici/swig/hdf5.i
+-rw-rw-r--   0 travis    (2000) travis    (2000)      169 2019-02-26 15:52:20.000000 amici-0.9.5/amici/swig/model.i
+-rw-rw-r--   0 travis    (2000) travis    (2000)      182 2019-02-26 15:52:20.000000 amici-0.9.5/amici/swig/model_dae.i
+-rw-rw-r--   0 travis    (2000) travis    (2000)      184 2019-02-26 15:52:20.000000 amici-0.9.5/amici/swig/model_ode.i
+-rw-rw-r--   0 travis    (2000) travis    (2000)      256 2019-02-26 15:52:20.000000 amici-0.9.5/amici/swig/modelname.template.i
+-rw-rw-r--   0 travis    (2000) travis    (2000)      169 2019-02-26 15:52:20.000000 amici-0.9.5/amici/swig/rdata.i
+-rw-rw-r--   0 travis    (2000) travis    (2000)      201 2019-02-26 15:52:20.000000 amici-0.9.5/amici/swig/solver.i
+-rw-rw-r--   0 travis    (2000) travis    (2000)      193 2019-02-26 15:52:20.000000 amici-0.9.5/amici/swig/solver_cvodes.i
+-rw-rw-r--   0 travis    (2000) travis    (2000)      187 2019-02-26 15:52:20.000000 amici-0.9.5/amici/swig/solver_idas.i
+-rw-rw-r--   0 travis    (2000) travis    (2000)      872 2019-02-26 15:52:20.000000 amici-0.9.5/amici/swig/std_unique_ptr.i
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4470 2019-02-26 15:52:20.000000 amici-0.9.5/amici/swig/stdvec2numpy.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)        6 2019-02-26 15:52:20.000000 amici-0.9.5/amici/version.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/amici.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3289 2019-02-26 15:58:31.000000 amici-0.9.5/amici.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29435 2019-02-26 15:58:31.000000 amici-0.9.5/amici.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-02-26 15:58:31.000000 amici-0.9.5/amici.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-02-26 15:58:31.000000 amici-0.9.5/amici.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)       75 2019-02-26 15:58:31.000000 amici-0.9.5/amici.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       43 2019-02-26 15:58:31.000000 amici-0.9.5/amici.egg-info/top_level.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 15:58:31.000000 amici-0.9.5/bin/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     8532 2019-02-26 15:52:20.000000 amici-0.9.5/bin/amici_import_petab.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-02-26 15:58:31.000000 amici-0.9.5/setup.cfg
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    12058 2019-02-26 15:52:20.000000 amici-0.9.5/setup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9242 2019-02-26 15:52:20.000000 amici-0.9.5/setup_clibs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        6 2019-02-26 15:52:20.000000 amici-0.9.5/version.txt
```

### Comparing `amici-0.9.4/README.md` & `amici-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/setup.py` & `amici-0.9.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,24 +13,45 @@
 """
 
 from setuptools import find_packages, setup, Extension
 from setuptools.command.build_ext import build_ext
 from setuptools.command.sdist import sdist
 from setuptools.command.install_lib import install_lib
 from setuptools.command.develop import develop
+from setuptools.command.install import install
+from setuptools.command.build_clib import build_clib
 
 import os
 import sys
 import glob
 import sysconfig
 import subprocess
 from shutil import copyfile
-import numpy as np # for include directory
-import setup_clibs  # Must run from within containing directory
+import setup_clibs # Must run from within containing directory
 
+
+def try_install(package):
+    """Try installing the given package using pip. Exit on error."""
+    errno = subprocess.call([sys.executable, "-m", "pip", "install", package])
+    if errno:
+        print(f"Failed trying to install {package}. Please install manually.")
+        raise SystemExit(errno)
+
+
+try:
+    # required for include directory
+    import numpy as np
+except ImportError:
+    # We need numpy, but setup_requires fires too late
+    try_install('numpy')
+    # retry
+    import numpy as np
+
+
+sys.path.insert(0, os.getcwd())
 from amici import __version__
 
 from amici.setuptools import (
     getBlasConfig,
     getHdf5Config,
     addCoverageFlagsIfRequired,
     addDebugFlagsIfRequired,
@@ -110,33 +131,84 @@
         'amici/libs',  # clib target directory
     ],
     extra_compile_args=['-std=c++11', *cxx_flags],
     extra_link_args=amici_module_linker_flags
 )
 
 
+class my_install(install):
+    """Custom install to handle extra arguments"""
+
+    # Passing --no-clibs allows to install the Python-only part of AMICI
+    user_options = install.user_options + [
+        ('no-clibs', None, "Don't build AMICI C++ extension"),
+    ]
+
+    def initialize_options(self):
+        install.initialize_options(self)
+        self.no_clibs = False
+
+    def finalize_options(self):
+        if self.no_clibs:
+            self.no_clibs = True
+        install.finalize_options(self)
+
+    def run(self):
+        install.run(self)
+
+
+class my_build_clib(build_clib):
+    """Custom build_clib"""
+
+    def build_libraries(self, libraries):
+        no_clibs = self.get_finalized_command('develop').no_clibs
+        no_clibs |= self.get_finalized_command('install').no_clibs
+
+        if no_clibs:
+            return
+
+        build_clib.build_libraries(self, libraries)
+
+
 class my_develop(develop):
     """Custom develop to build clibs"""
-    def run(self):
 
-        generateSwigInterfaceFiles()
+    # Passing --no-clibs allows to install the Python-only part of AMICI
+    user_options = develop.user_options + [
+        ('no-clibs', None, "Don't build AMICI C++ extension"),
+    ]
+
+    def initialize_options(self):
+        develop.initialize_options(self)
+        self.no_clibs = False
+
+    def finalize_options(self):
+        if self.no_clibs:
+            self.no_clibs = True
+        develop.finalize_options(self)
+
+    def run(self):
+        if not self.no_clibs:
+            generateSwigInterfaceFiles()
+            self.run_command('build')
 
-        self.run_command('build')
         develop.run(self)
 
 
 class my_install_lib(install_lib):
     """Custom install to allow preserving of debug symbols"""
     def run(self):
         """strip debug symbols
 
         Returns:
 
         """
-        if 'ENABLE_AMICI_DEBUGGING' in os.environ and os.environ['ENABLE_AMICI_DEBUGGING'] == 'TRUE' and sys.platform == 'darwin':
+        if 'ENABLE_AMICI_DEBUGGING' in os.environ \
+                and os.environ['ENABLE_AMICI_DEBUGGING'] == 'TRUE' \
+                and sys.platform == 'darwin':
             search_dir = os.path.join(os.getcwd(),self.build_dir,'amici')
             for file in os.listdir(search_dir):
                 if file.endswith('.so'):
                     subprocess.run(['dsymutil',os.path.join(search_dir,file),
                                     '-o',os.path.join(search_dir,file + '.dSYM')])
 
 
@@ -149,14 +221,19 @@
 
     def run(self):
         """Copy the generated clibs to the extensions folder to be included in the wheel
 
         Returns:
 
         """
+        no_clibs = self.get_finalized_command('develop').no_clibs
+        no_clibs |= self.get_finalized_command('install').no_clibs
+
+        if no_clibs:
+            return
 
         if not self.dry_run:  # --dry-run
             libraries = []
             build_clib = ''
             if self.distribution.has_c_libraries():
                 # get the previously built static libraries
                 build_clib = self.get_finalized_command('build_clib')
@@ -174,16 +251,16 @@
             self.mkpath(target_dir)
 
             # Copy the generated libs
             for lib in libraries:
                 libfilenames = glob.glob(
                     '%s%s*%s.*' % (build_clib.build_clib, os.sep, lib)
                 )
-                assert len(
-                    libfilenames) == 1, "Found unexpected number of files: " % libfilenames
+                assert len(libfilenames) == 1, \
+                    "Found unexpected number of files: " % libfilenames
 
                 copyfile(libfilenames[0],
                          os.path.join(target_dir, os.path.basename(libfilenames[0])))
 
         # Continue with the actual extension building
         build_ext.run(self)
 
@@ -248,16 +325,18 @@
 
 
 def main():
     # Install
     setup(
         name='amici',
         cmdclass={
+            'install': my_install,
             'sdist': my_sdist,
             'build_ext': my_build_ext,
+            'build_clib': my_build_clib,
             'install_lib': my_install_lib,
             'develop': my_develop,
         },
         version=__version__,
         description='Advanced multi-language Interface to CVODES and IDAS (%s)',
         long_description=long_description,
         long_description_content_type="text/markdown",
@@ -268,14 +347,15 @@
         libraries=[libamici, libsundials, libsuitesparse],
         ext_modules=[amici_module],
         py_modules=['amici/amici',  # the swig interface
                     'amici/amici_without_hdf5',   # the swig interface
                     ],
         packages=find_packages(),
         package_dir={'amici': 'amici'},
+        scripts=['bin/amici_import_petab.py'],
         install_requires=['sympy',
                           'python-libsbml',
                           'h5py',
                           'pandas',
                           'setuptools>=40.6.3'],
         python_requires='>=3.6',
         extras_require={'wurlitzer': ['wurlitzer']},
```

### Comparing `amici-0.9.4/setup_clibs.py` & `amici-0.9.5/setup_clibs.py`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/PKG-INFO` & `amici-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amici
-Version: 0.9.4
+Version: 0.9.5
 Summary: Advanced multi-language Interface to CVODES and IDAS (%s)
 Home-page: https://github.com/ICB-DCM/AMICI
 Author: Fabian Froehlich, Jan Hasenauer, Daniel Weindl and Paul Stapor
 Author-email: fabian_froehlich@hms.harvard.edu
 License: BSD
 Description: # About AMICI
```

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/cvode/cvode_spils.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/cvode/cvode_spils.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/cvode/cvode_sparse.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/cvode/cvode_sparse.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/cvode/cvode_bandpre.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/cvode/cvode_bandpre.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/cvode/cvode_superlumt.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/cvode/cvode_superlumt.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/cvode/cvode.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/cvode/cvode.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/cvode/cvode_sptfqmr.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/cvode/cvode_sptfqmr.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/cvode/cvode_klu.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/cvode/cvode_klu.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/cvode/cvode_lapack.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/cvode/cvode_lapack.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/cvode/cvode_direct.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/cvode/cvode_direct.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/cvode/cvode_spgmr.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/cvode/cvode_spgmr.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/cvode/cvode_diag.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/cvode/cvode_diag.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/cvode/cvode_spbcgs.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/cvode/cvode_spbcgs.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/cvode/cvode_dense.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/cvode/cvode_dense.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/cvode/cvode_bbdpre.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/cvode/cvode_bbdpre.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/cvode/cvode_band.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/cvode/cvode_band.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/kinsol/kinsol.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/kinsol/kinsol.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/kinsol/kinsol_direct.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/kinsol/kinsol_direct.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/kinsol/kinsol_spils.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/kinsol/kinsol_spils.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/kinsol/kinsol_band.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/kinsol/kinsol_band.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/kinsol/kinsol_sparse.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/kinsol/kinsol_sparse.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/kinsol/kinsol_bbdpre.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/kinsol/kinsol_bbdpre.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/kinsol/kinsol_dense.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/kinsol/kinsol_dense.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/kinsol/kinsol_spbcgs.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/kinsol/kinsol_spbcgs.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/kinsol/kinsol_klu.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/kinsol/kinsol_klu.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/kinsol/kinsol_superlumt.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/kinsol/kinsol_superlumt.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/kinsol/kinsol_spgmr.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/kinsol/kinsol_spgmr.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/kinsol/kinsol_spfgmr.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/kinsol/kinsol_spfgmr.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/kinsol/kinsol_lapack.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/kinsol/kinsol_lapack.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/kinsol/kinsol_sptfqmr.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/kinsol/kinsol_sptfqmr.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/idas/idas.h` & `amici-0.9.5/amici/ThirdParty/sundials/build/include/idas/idas.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/idas/idas_klu.h` & `amici-0.9.5/amici/ThirdParty/sundials/build/include/idas/idas_klu.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/idas/idas_spgmr.h` & `amici-0.9.5/amici/ThirdParty/sundials/build/include/idas/idas_spgmr.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/idas/idas_sptfqmr.h` & `amici-0.9.5/amici/ThirdParty/sundials/build/include/idas/idas_sptfqmr.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/idas/idas_superlumt.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/idas/idas_superlumt.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/idas/idas_sparse.h` & `amici-0.9.5/amici/ThirdParty/sundials/build/include/idas/idas_sparse.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/idas/idas_spils.h` & `amici-0.9.5/amici/ThirdParty/sundials/build/include/idas/idas_spils.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/idas/idas_spbcgs.h` & `amici-0.9.5/amici/ThirdParty/sundials/build/include/idas/idas_spbcgs.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/idas/idas_dense.h` & `amici-0.9.5/amici/ThirdParty/sundials/build/include/idas/idas_dense.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/idas/idas_lapack.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/idas/idas_lapack.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/idas/idas_bbdpre.h` & `amici-0.9.5/amici/ThirdParty/sundials/build/include/idas/idas_bbdpre.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/idas/idas_band.h` & `amici-0.9.5/amici/ThirdParty/sundials/build/include/idas/idas_band.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/idas/idas_direct.h` & `amici-0.9.5/amici/ThirdParty/sundials/build/include/idas/idas_direct.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/nvector/nvector_parallel.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/nvector/nvector_parallel.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/nvector/nvector_parhyp.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/nvector/nvector_parhyp.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/nvector/nvector_openmp.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/nvector/nvector_openmp.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/nvector/nvector_petsc.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/nvector/nvector_petsc.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/nvector/nvector_pthreads.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/nvector/nvector_pthreads.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/nvector/nvector_serial.h` & `amici-0.9.5/amici/ThirdParty/sundials/build/include/nvector/nvector_serial.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/cvodes/cvodes_band.h` & `amici-0.9.5/amici/ThirdParty/sundials/build/include/cvodes/cvodes_band.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/cvodes/cvodes_dense.h` & `amici-0.9.5/amici/ThirdParty/sundials/build/include/cvodes/cvodes_dense.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/cvodes/cvodes_direct.h` & `amici-0.9.5/amici/ThirdParty/sundials/build/include/cvodes/cvodes_direct.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/cvodes/cvodes_superlumt.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/cvodes/cvodes_superlumt.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/cvodes/cvodes_sparse.h` & `amici-0.9.5/amici/ThirdParty/sundials/build/include/cvodes/cvodes_sparse.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/cvodes/cvodes_klu.h` & `amici-0.9.5/amici/ThirdParty/sundials/build/include/cvodes/cvodes_klu.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/cvodes/cvodes_lapack.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/cvodes/cvodes_lapack.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/cvodes/cvodes.h` & `amici-0.9.5/amici/ThirdParty/sundials/build/include/cvodes/cvodes.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/cvodes/cvodes_sptfqmr.h` & `amici-0.9.5/amici/ThirdParty/sundials/build/include/cvodes/cvodes_sptfqmr.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/cvodes/cvodes_bandpre.h` & `amici-0.9.5/amici/ThirdParty/sundials/build/include/cvodes/cvodes_bandpre.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/cvodes/cvodes_spbcgs.h` & `amici-0.9.5/amici/ThirdParty/sundials/build/include/cvodes/cvodes_spbcgs.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/cvodes/cvodes_bbdpre.h` & `amici-0.9.5/amici/ThirdParty/sundials/build/include/cvodes/cvodes_bbdpre.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/cvodes/cvodes_spils.h` & `amici-0.9.5/amici/ThirdParty/sundials/build/include/cvodes/cvodes_spils.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/cvodes/cvodes_spgmr.h` & `amici-0.9.5/amici/ThirdParty/sundials/build/include/cvodes/cvodes_spgmr.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/cvodes/cvodes_diag.h` & `amici-0.9.5/amici/ThirdParty/sundials/build/include/cvodes/cvodes_diag.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/arkode/arkode_bandpre.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/arkode/arkode_bandpre.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/arkode/arkode_spils.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/arkode/arkode_spils.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/arkode/arkode_klu.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/arkode/arkode_klu.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/arkode/arkode_bbdpre.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/arkode/arkode_bbdpre.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/arkode/arkode_band.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/arkode/arkode_band.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/arkode/arkode_spfgmr.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/arkode/arkode_spfgmr.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/arkode/arkode_sptfqmr.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/arkode/arkode_sptfqmr.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/arkode/arkode_superlumt.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/arkode/arkode_superlumt.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/arkode/arkode_direct.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/arkode/arkode_direct.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/arkode/arkode_dense.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/arkode/arkode_dense.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/arkode/arkode_spgmr.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/arkode/arkode_spgmr.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/arkode/arkode_spbcgs.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/arkode/arkode_spbcgs.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/arkode/arkode_pcg.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/arkode/arkode_pcg.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/arkode/arkode.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/arkode/arkode.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/arkode/arkode_lapack.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/arkode/arkode_lapack.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/arkode/arkode_sparse.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/arkode/arkode_sparse.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/sundials/sundials_spfgmr.h` & `amici-0.9.5/amici/ThirdParty/sundials/build/include/sundials/sundials_spfgmr.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/sundials/sundials_spbcgs.h` & `amici-0.9.5/amici/ThirdParty/sundials/build/include/sundials/sundials_spbcgs.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/sundials/sundials_spgmr.h` & `amici-0.9.5/amici/ThirdParty/sundials/build/include/sundials/sundials_spgmr.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/sundials/sundials_sptfqmr.h` & `amici-0.9.5/amici/ThirdParty/sundials/build/include/sundials/sundials_sptfqmr.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/sundials/sundials_klu_impl.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/sundials/sundials_klu_impl.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/sundials/sundials_nvector.h` & `amici-0.9.5/amici/ThirdParty/sundials/build/include/sundials/sundials_nvector.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/sundials/sundials_fnvector.h` & `amici-0.9.5/amici/ThirdParty/sundials/build/include/sundials/sundials_fnvector.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/sundials/sundials_band.h` & `amici-0.9.5/amici/ThirdParty/sundials/build/include/sundials/sundials_band.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/sundials/sundials_pcg.h` & `amici-0.9.5/amici/ThirdParty/sundials/build/include/sundials/sundials_pcg.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/sundials/sundials_lapack.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/sundials/sundials_lapack.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/sundials/sundials_sparse.h` & `amici-0.9.5/amici/ThirdParty/sundials/build/include/sundials/sundials_sparse.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/sundials/sundials_superlumt_impl.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/sundials/sundials_superlumt_impl.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/sundials/sundials_iterative.h` & `amici-0.9.5/amici/ThirdParty/sundials/build/include/sundials/sundials_iterative.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/sundials/sundials_dense.h` & `amici-0.9.5/amici/ThirdParty/sundials/build/include/sundials/sundials_dense.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/sundials/sundials_types.h` & `amici-0.9.5/amici/ThirdParty/sundials/build/include/sundials/sundials_types.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/sundials/sundials_math.h` & `amici-0.9.5/amici/ThirdParty/sundials/build/include/sundials/sundials_math.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/sundials/sundials_direct.h` & `amici-0.9.5/amici/ThirdParty/sundials/build/include/sundials/sundials_direct.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/ida/ida_superlumt.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/ida/ida_superlumt.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/ida/ida_klu.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/ida/ida_klu.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/ida/ida_spils.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/ida/ida_spils.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/ida/ida_spgmr.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/ida/ida_spgmr.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/ida/ida_sptfqmr.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/ida/ida_sptfqmr.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/ida/ida_lapack.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/ida/ida_lapack.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/ida/ida_spbcgs.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/ida/ida_spbcgs.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/ida/ida_dense.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/ida/ida_dense.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/ida/ida_bbdpre.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/ida/ida_bbdpre.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/ida/ida.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/ida/ida.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/ida/ida_direct.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/ida/ida_direct.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/ida/ida_sparse.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/ida/ida_sparse.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/include/ida/ida_band.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/ida/ida_band.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/LICENSE` & `amici-0.9.5/amici/ThirdParty/sundials/LICENSE`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/build/CMakeFiles/feature_tests.c` & `amici-0.9.5/amici/ThirdParty/sundials/build/CMakeFiles/feature_tests.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/build/CMakeFiles/3.9.2/CompilerIdC/CMakeCCompilerId.c` & `amici-0.9.5/amici/ThirdParty/sundials/build/CMakeFiles/3.12.4/CompilerIdC/CMakeCCompilerId.c`

 * *Files 6% similar despite different names*

```diff
@@ -102,32 +102,56 @@
   /* __DECC_VER = VVRRTPPPP */
 # define COMPILER_VERSION_MAJOR DEC(__DECC_VER/10000000)
 # define COMPILER_VERSION_MINOR DEC(__DECC_VER/100000  % 100)
 # define COMPILER_VERSION_PATCH DEC(__DECC_VER         % 10000)
 
 #elif defined(__IBMC__) && defined(__COMPILER_VER__)
 # define COMPILER_ID "zOS"
-  /* __IBMC__ = VRP */
-# define COMPILER_VERSION_MAJOR DEC(__IBMC__/100)
-# define COMPILER_VERSION_MINOR DEC(__IBMC__/10 % 10)
-# define COMPILER_VERSION_PATCH DEC(__IBMC__    % 10)
+# if defined(__ibmxl__)
+#  define COMPILER_VERSION_MAJOR DEC(__ibmxl_version__)
+#  define COMPILER_VERSION_MINOR DEC(__ibmxl_release__)
+#  define COMPILER_VERSION_PATCH DEC(__ibmxl_modification__)
+#  define COMPILER_VERSION_TWEAK DEC(__ibmxl_ptf_fix_level__)
+# else
+   /* __IBMC__ = VRP */
+#  define COMPILER_VERSION_MAJOR DEC(__IBMC__/100)
+#  define COMPILER_VERSION_MINOR DEC(__IBMC__/10 % 10)
+#  define COMPILER_VERSION_PATCH DEC(__IBMC__    % 10)
+# endif
+
 
-#elif defined(__IBMC__) && !defined(__COMPILER_VER__) && __IBMC__ >= 800
+#elif defined(__ibmxl__) || (defined(__IBMC__) && !defined(__COMPILER_VER__) && __IBMC__ >= 800)
 # define COMPILER_ID "XL"
-  /* __IBMC__ = VRP */
-# define COMPILER_VERSION_MAJOR DEC(__IBMC__/100)
-# define COMPILER_VERSION_MINOR DEC(__IBMC__/10 % 10)
-# define COMPILER_VERSION_PATCH DEC(__IBMC__    % 10)
+# if defined(__ibmxl__)
+#  define COMPILER_VERSION_MAJOR DEC(__ibmxl_version__)
+#  define COMPILER_VERSION_MINOR DEC(__ibmxl_release__)
+#  define COMPILER_VERSION_PATCH DEC(__ibmxl_modification__)
+#  define COMPILER_VERSION_TWEAK DEC(__ibmxl_ptf_fix_level__)
+# else
+   /* __IBMC__ = VRP */
+#  define COMPILER_VERSION_MAJOR DEC(__IBMC__/100)
+#  define COMPILER_VERSION_MINOR DEC(__IBMC__/10 % 10)
+#  define COMPILER_VERSION_PATCH DEC(__IBMC__    % 10)
+# endif
+
 
 #elif defined(__IBMC__) && !defined(__COMPILER_VER__) && __IBMC__ < 800
 # define COMPILER_ID "VisualAge"
-  /* __IBMC__ = VRP */
-# define COMPILER_VERSION_MAJOR DEC(__IBMC__/100)
-# define COMPILER_VERSION_MINOR DEC(__IBMC__/10 % 10)
-# define COMPILER_VERSION_PATCH DEC(__IBMC__    % 10)
+# if defined(__ibmxl__)
+#  define COMPILER_VERSION_MAJOR DEC(__ibmxl_version__)
+#  define COMPILER_VERSION_MINOR DEC(__ibmxl_release__)
+#  define COMPILER_VERSION_PATCH DEC(__ibmxl_modification__)
+#  define COMPILER_VERSION_TWEAK DEC(__ibmxl_ptf_fix_level__)
+# else
+   /* __IBMC__ = VRP */
+#  define COMPILER_VERSION_MAJOR DEC(__IBMC__/100)
+#  define COMPILER_VERSION_MINOR DEC(__IBMC__/10 % 10)
+#  define COMPILER_VERSION_PATCH DEC(__IBMC__    % 10)
+# endif
+
 
 #elif defined(__PGI)
 # define COMPILER_ID "PGI"
 # define COMPILER_VERSION_MAJOR DEC(__PGIC__)
 # define COMPILER_VERSION_MINOR DEC(__PGIC_MINOR__)
 # if defined(__PGIC_PATCHLEVEL__)
 #  define COMPILER_VERSION_PATCH DEC(__PGIC_PATCHLEVEL__)
@@ -219,16 +243,22 @@
 #if defined(__VISUALDSPVERSION__)
   /* __VISUALDSPVERSION__ = 0xVVRRPP00 */
 # define COMPILER_VERSION_MAJOR HEX(__VISUALDSPVERSION__>>24)
 # define COMPILER_VERSION_MINOR HEX(__VISUALDSPVERSION__>>16 & 0xFF)
 # define COMPILER_VERSION_PATCH HEX(__VISUALDSPVERSION__>>8  & 0xFF)
 #endif
 
-#elif defined(__IAR_SYSTEMS_ICC__ ) || defined(__IAR_SYSTEMS_ICC)
+#elif defined(__IAR_SYSTEMS_ICC__) || defined(__IAR_SYSTEMS_ICC)
 # define COMPILER_ID "IAR"
+# if defined(__VER__)
+#  define COMPILER_VERSION_MAJOR DEC((__VER__) / 1000000)
+#  define COMPILER_VERSION_MINOR DEC(((__VER__) / 1000) % 1000)
+#  define COMPILER_VERSION_PATCH DEC((__VER__) % 1000)
+#  define COMPILER_VERSION_INTERNAL DEC(__IAR_SYSTEMS_ICC__)
+# endif
 
 #elif defined(__ARMCC_VERSION)
 # define COMPILER_ID "ARMCC"
 #if __ARMCC_VERSION >= 1000000
   /* __ARMCC_VERSION = VRRPPPP */
   # define COMPILER_VERSION_MAJOR DEC(__ARMCC_VERSION/1000000)
   # define COMPILER_VERSION_MINOR DEC(__ARMCC_VERSION/10000 % 100)
@@ -411,14 +441,17 @@
 
 # elif defined(_M_X64) || defined(_M_AMD64)
 #  define ARCHITECTURE_ID "x64"
 
 # elif defined(_M_IX86)
 #  define ARCHITECTURE_ID "X86"
 
+# elif defined(_M_ARM64)
+#  define ARCHITECTURE_ID "ARM64"
+
 # elif defined(_M_ARM)
 #  if _M_ARM == 4
 #   define ARCHITECTURE_ID "ARMV4I"
 #  elif _M_ARM == 5
 #   define ARCHITECTURE_ID "ARMV5I"
 #  else
 #   define ARCHITECTURE_ID "ARMV" STRINGIFY(_M_ARM)
@@ -441,14 +474,24 @@
 # elif defined(_M_IX86)
 #  define ARCHITECTURE_ID "X86"
 
 # else /* unknown architecture */
 #  define ARCHITECTURE_ID ""
 # endif
 
+#elif defined(__IAR_SYSTEMS_ICC__) || defined(__IAR_SYSTEMS_ICC)
+# if defined(__ICCARM__)
+#  define ARCHITECTURE_ID "ARM"
+
+# elif defined(__ICCAVR__)
+#  define ARCHITECTURE_ID "AVR"
+
+# else /* unknown architecture */
+#  define ARCHITECTURE_ID ""
+# endif
 #else
 #  define ARCHITECTURE_ID
 #endif
 
 /* Convert integer to decimal digit literals.  */
 #define DEC(n)                   \
   ('0' + (((n) / 10000000)%10)), \
@@ -485,14 +528,23 @@
     '.', COMPILER_VERSION_TWEAK,
 #   endif
 #  endif
 # endif
   ']','\0'};
 #endif
 
+/* Construct a string literal encoding the internal version number. */
+#ifdef COMPILER_VERSION_INTERNAL
+char const info_version_internal[] = {
+  'I', 'N', 'F', 'O', ':',
+  'c','o','m','p','i','l','e','r','_','v','e','r','s','i','o','n','_',
+  'i','n','t','e','r','n','a','l','[',
+  COMPILER_VERSION_INTERNAL,']','\0'};
+#endif
+
 /* Construct a string literal encoding the version number components. */
 #ifdef SIMULATE_VERSION_MAJOR
 char const info_simulate_version[] = {
   'I', 'N', 'F', 'O', ':',
   's','i','m','u','l','a','t','e','_','v','e','r','s','i','o','n','[',
   SIMULATE_VERSION_MAJOR,
 # ifdef SIMULATE_VERSION_MINOR
@@ -514,15 +566,16 @@
 char const* info_platform = "INFO" ":" "platform[" PLATFORM_ID "]";
 char const* info_arch = "INFO" ":" "arch[" ARCHITECTURE_ID "]";
 
 
 
 
 #if !defined(__STDC__)
-# if defined(_MSC_VER) && !defined(__clang__)
+# if (defined(_MSC_VER) && !defined(__clang__)) \
+  || (defined(__ibmxl__) || defined(__IBMC__))
 #  define C_DIALECT "90"
 # else
 #  define C_DIALECT
 # endif
 #elif __STDC_VERSION__ >= 201000L
 # define C_DIALECT "11"
 #elif __STDC_VERSION__ >= 199901L
@@ -547,14 +600,17 @@
   int require = 0;
   require += info_compiler[argc];
   require += info_platform[argc];
   require += info_arch[argc];
 #ifdef COMPILER_VERSION_MAJOR
   require += info_version[argc];
 #endif
+#ifdef COMPILER_VERSION_INTERNAL
+  require += info_version_internal[argc];
+#endif
 #ifdef SIMULATE_ID
   require += info_simulate[argc];
 #endif
 #ifdef SIMULATE_VERSION_MAJOR
   require += info_simulate_version[argc];
 #endif
 #if defined(__CRAYXE) || defined(__CRAYXC)
```

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/build/include/idas/idas.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/idas/idas.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/build/include/idas/idas_klu.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/idas/idas_klu.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/build/include/idas/idas_spgmr.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/idas/idas_spgmr.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/build/include/idas/idas_sptfqmr.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/idas/idas_sptfqmr.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/build/include/idas/idas_impl.h` & `amici-0.9.5/amici/ThirdParty/sundials/build/include/idas/idas_impl.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/build/include/idas/idas_sparse.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/idas/idas_sparse.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/build/include/idas/idas_spils.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/idas/idas_spils.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/build/include/idas/idas_spbcgs.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/idas/idas_spbcgs.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/build/include/idas/idas_dense.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/idas/idas_dense.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/build/include/idas/idas_bbdpre.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/idas/idas_bbdpre.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/build/include/idas/idas_band.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/idas/idas_band.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/build/include/idas/idas_direct.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/idas/idas_direct.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/build/include/nvector/nvector_serial.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/nvector/nvector_serial.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/build/include/cvodes/cvodes_band.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/cvodes/cvodes_band.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/build/include/cvodes/cvodes_dense.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/cvodes/cvodes_dense.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/build/include/cvodes/cvodes_direct.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/cvodes/cvodes_direct.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/build/include/cvodes/cvodes_sparse.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/cvodes/cvodes_sparse.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/build/include/cvodes/cvodes_klu.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/cvodes/cvodes_klu.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/build/include/cvodes/cvodes.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/cvodes/cvodes.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/build/include/cvodes/cvodes_sptfqmr.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/cvodes/cvodes_sptfqmr.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/build/include/cvodes/cvodes_bandpre.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/cvodes/cvodes_bandpre.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/build/include/cvodes/cvodes_spbcgs.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/cvodes/cvodes_spbcgs.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/build/include/cvodes/cvodes_impl.h` & `amici-0.9.5/amici/ThirdParty/sundials/build/include/cvodes/cvodes_impl.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/build/include/cvodes/cvodes_bbdpre.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/cvodes/cvodes_bbdpre.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/build/include/cvodes/cvodes_spils.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/cvodes/cvodes_spils.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/build/include/cvodes/cvodes_spgmr.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/cvodes/cvodes_spgmr.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/build/include/cvodes/cvodes_diag.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/cvodes/cvodes_diag.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/build/include/sundials/sundials_spfgmr.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/sundials/sundials_spfgmr.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/build/include/sundials/sundials_spbcgs.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/sundials/sundials_spbcgs.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/build/include/sundials/sundials_spgmr.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/sundials/sundials_spgmr.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/build/include/sundials/sundials_config.h` & `amici-0.9.5/amici/ThirdParty/sundials/build/include/sundials/sundials_config.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/build/include/sundials/sundials_sptfqmr.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/sundials/sundials_sptfqmr.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/build/include/sundials/sundials_nvector.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/sundials/sundials_nvector.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/build/include/sundials/sundials_fnvector.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/sundials/sundials_fnvector.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/build/include/sundials/sundials_band.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/sundials/sundials_band.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/build/include/sundials/sundials_pcg.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/sundials/sundials_pcg.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/build/include/sundials/sundials_sparse.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/sundials/sundials_sparse.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/build/include/sundials/sundials_iterative.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/sundials/sundials_iterative.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/build/include/sundials/sundials_dense.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/sundials/sundials_dense.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/build/include/sundials/sundials_types.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/sundials/sundials_types.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/build/include/sundials/sundials_math.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/sundials/sundials_math.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/build/include/sundials/sundials_direct.h` & `amici-0.9.5/amici/ThirdParty/sundials/include/sundials/sundials_direct.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/nvec_openmp/nvector_openmp.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/nvec_openmp/nvector_openmp.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/nvec_openmp/fnvector_openmp.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/nvec_openmp/fnvector_openmp.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/nvec_openmp/fnvector_openmp.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/nvec_openmp/fnvector_openmp.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/nvec_parhyp/nvector_parhyp.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/nvec_parhyp/nvector_parhyp.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvode/cvode_sparse_impl.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvode/cvode_sparse_impl.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvode/cvode_dense.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvode/cvode_dense.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvode/cvode_sparse.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvode/cvode_sparse.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvode/cvode_lapack.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvode/cvode_lapack.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvode/cvode_spgmr.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvode/cvode_spgmr.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvode/cvode_klu.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvode/cvode_klu.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvode/LICENSE` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvode/LICENSE`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvode/cvode_sptfqmr.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvode/cvode_sptfqmr.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvode/cvode_direct_impl.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvode/cvode_direct_impl.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvode/cvode_superlumt.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvode/cvode_superlumt.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvode/cvode_spils_impl.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvode/cvode_spils_impl.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvode/cvode_bandpre.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvode/cvode_bandpre.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvode/cvode_diag_impl.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvode/cvode_diag_impl.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvode/cvode_bbdpre.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvode/cvode_bbdpre.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvode/cvode_spils.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvode/cvode_spils.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvode/cvode_direct.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvode/cvode_direct.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvode/cvode_diag.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvode/cvode_diag.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvode/cvode_band.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvode/cvode_band.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvode/cvode_impl.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvode/cvode_impl.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvode/cvode_io.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvode/cvode_io.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvode/cvode.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvode/cvode.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvode/cvode_spbcgs.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvode/cvode_spbcgs.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvode/fcmix/fcvroot.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvode/fcmix/fcvroot.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvode/fcmix/fcvklu.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvode/fcmix/fcvklu.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvode/fcmix/fcvlapdense.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvode/fcmix/fcvlapdense.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvode/fcmix/fcvsparse.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvode/fcmix/fcvsparse.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvode/fcmix/fcvbp.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvode/fcmix/fcvbp.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvode/fcmix/fcvbbd.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvode/fcmix/fcvbbd.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvode/fcmix/fcvband.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvode/fcmix/fcvband.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvode/fcmix/fcvsuperlumt.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvode/fcmix/fcvsuperlumt.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvode/fcmix/fcvbbd.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvode/fcmix/fcvbbd.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvode/fcmix/fcvode.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvode/fcmix/fcvode.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvode/fcmix/fcvlapack.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvode/fcmix/fcvlapack.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvode/fcmix/fcvode.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvode/fcmix/fcvode.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvode/fcmix/fcvroot.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvode/fcmix/fcvroot.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvode/fcmix/fcvewt.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvode/fcmix/fcvewt.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvode/fcmix/fcvpreco.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvode/fcmix/fcvpreco.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvode/fcmix/fcvlapband.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvode/fcmix/fcvlapband.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvode/fcmix/fcvbp.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvode/fcmix/fcvbp.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvode/fcmix/fcvjtimes.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvode/fcmix/fcvjtimes.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvode/fcmix/fcvdense.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvode/fcmix/fcvdense.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvode/cvode_bandpre_impl.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvode/cvode_bandpre_impl.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvode/cvode_bbdpre_impl.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvode/cvode_bbdpre_impl.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/kinsol_spils.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/kinsol_spils.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/kinsol_superlumt.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/kinsol_superlumt.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/kinsol_spgmr.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/kinsol_spgmr.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/kinsol_sptfqmr.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/kinsol_sptfqmr.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/kinsol_sparse.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/kinsol_sparse.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/LICENSE` & `amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/LICENSE`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/kinsol_band.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/kinsol_band.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/kinsol_spils_impl.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/kinsol_spils_impl.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/kinsol_klu.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/kinsol_klu.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/kinsol_sparse_impl.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/kinsol_sparse_impl.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/kinsol_spfgmr.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/kinsol_spfgmr.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/kinsol_direct_impl.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/kinsol_direct_impl.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/kinsol_direct.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/kinsol_direct.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/kinsol_lapack.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/kinsol_lapack.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/kinsol_impl.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/kinsol_impl.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/kinsol_spbcgs.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/kinsol_spbcgs.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinlapdense.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinlapdense.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinsparse.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinsparse.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinpreco.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinpreco.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinsol.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinsol.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinsol.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinsol.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/fcmix/fkindense.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/fcmix/fkindense.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinbbd.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinbbd.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinband.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinband.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinsuperlumt.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinsuperlumt.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinjtimes.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinjtimes.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinbbd.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinbbd.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinlapband.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinlapband.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinlapack.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinlapack.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinklu.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/fcmix/fkinklu.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/kinsol_dense.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/kinsol_dense.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/kinsol_bbdpre.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/kinsol_bbdpre.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/kinsol_io.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/kinsol_io.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/kinsol_bbdpre_impl.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/kinsol_bbdpre_impl.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/kinsol/kinsol.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/kinsol/kinsol.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/idas/idas_dense.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/idas/idas_dense.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/idas/idas_spils.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/idas/idas_spils.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/idas/idaa_io.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/idas/idaa_io.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/idas/idas_lapack.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/idas/idas_lapack.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/idas/idas_band.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/idas/idas_band.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/idas/LICENSE` & `amici-0.9.5/amici/ThirdParty/sundials/src/idas/LICENSE`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/idas/idas_bbdpre_impl.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/idas/idas_bbdpre_impl.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/idas/idas_direct_impl.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/idas/idas_direct_impl.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/idas/idas_superlumt.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/idas/idas_superlumt.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/idas/idas.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/idas/idas.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/idas/idas_klu.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/idas/idas_klu.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/idas/idas_ic.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/idas/idas_ic.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/idas/idas_impl.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/idas/idas_impl.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/idas/idas_bbdpre.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/idas/idas_bbdpre.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/idas/idas_sparse.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/idas/idas_sparse.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/idas/idas_io.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/idas/idas_io.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/idas/idas_spils_impl.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/idas/idas_spils_impl.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/idas/idas_sptfqmr.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/idas/idas_sptfqmr.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/idas/idas_spgmr.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/idas/idas_spgmr.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/idas/idas_direct.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/idas/idas_direct.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/idas/idas_spbcgs.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/idas/idas_spbcgs.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/idas/idas_sparse_impl.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/idas/idas_sparse_impl.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/idas/idaa.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/idas/idaa.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/nvec_par/nvector_parallel.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/nvec_par/nvector_parallel.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/nvec_par/fnvector_parallel.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/nvec_par/fnvector_parallel.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/nvec_par/fnvector_parallel.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/nvec_par/fnvector_parallel.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/nvec_ser/fnvector_serial.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/nvec_ser/fnvector_serial.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/nvec_ser/fnvector_serial.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/nvec_ser/fnvector_serial.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/nvec_ser/nvector_serial.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/nvec_ser/nvector_serial.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodes_sparse_impl.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodes_sparse_impl.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodes_sptfqmr.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodes_sptfqmr.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodes_dense.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodes_dense.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodes_bbdpre_impl.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodes_bbdpre_impl.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/LICENSE` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/LICENSE`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodes_bandpre_impl.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodes_bandpre_impl.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodes_spils.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodes_spils.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodes_bandpre.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodes_bandpre.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodes_direct_impl.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodes_direct_impl.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodes_sparse.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodes_sparse.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodes_spbcgs.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodes_spbcgs.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodes_superlumt.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodes_superlumt.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodes_impl.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodes_impl.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodes_diag_impl.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodes_diag_impl.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodes_spils_impl.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodes_spils_impl.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodes_io.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodes_io.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodes_spgmr.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodes_spgmr.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodes_band.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodes_band.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodea_io.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodea_io.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodea.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodea.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodes_diag.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodes_diag.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodes_klu.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodes_klu.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodes.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodes.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodes_lapack.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodes_lapack.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodes_bbdpre.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodes_bbdpre.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/cvodes/cvodes_direct.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/cvodes/cvodes_direct.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/nvec_petsc/nvector_petsc.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/nvec_petsc/nvector_petsc.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/nvec_pthreads/fnvector_pthreads.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/nvec_pthreads/fnvector_pthreads.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/nvec_pthreads/nvector_pthreads.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/nvec_pthreads/nvector_pthreads.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/nvec_pthreads/fnvector_pthreads.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/nvec_pthreads/fnvector_pthreads.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode_sptfqmr.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode_sptfqmr.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode_spfgmr.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode_spfgmr.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode_io.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode_io.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode_sparse_impl.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode_sparse_impl.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode_lapack.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode_lapack.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode_spbcgs.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode_spbcgs.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/LICENSE` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/LICENSE`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode_dense.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode_dense.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode_band.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode_band.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode_spils_impl.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode_spils_impl.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode_sparse.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode_sparse.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode_direct.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode_direct.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode_superlumt.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode_superlumt.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode_klu.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode_klu.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode_pcg.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode_pcg.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode_bandpre_impl.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode_bandpre_impl.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode_spgmr.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode_spgmr.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode_butcher.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode_butcher.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode_bandpre.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode_bandpre.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode_direct_impl.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode_direct_impl.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode_bbdpre_impl.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode_bbdpre_impl.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farkband.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farkband.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farklapack.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farklapack.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farkroot.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farkroot.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farkexpstab.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farkexpstab.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farkklu.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farkklu.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farkode.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farkode.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farksparsemass.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farksparsemass.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farkbbd.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farkbbd.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farklapdense.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farklapdense.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farkjtimes.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farkjtimes.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farklapdensemass.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farklapdensemass.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farkroot.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farkroot.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farklapband.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farklapband.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farkadapt.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farkadapt.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farkbp.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farkbp.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farkmtimes.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farkmtimes.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farkdensemass.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farkdensemass.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farklapbandmass.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farklapbandmass.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farkbp.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farkbp.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farkbandmass.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farkbandmass.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farkmasspreco.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farkmasspreco.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farksparse.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farksparse.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farkbbd.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farkbbd.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farkdense.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farkdense.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farksuperlumt.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farksuperlumt.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farkewt.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farkewt.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farkode.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farkode.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/fcmix/farkpreco.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/fcmix/farkpreco.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode_impl.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode_impl.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode_spils.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode_spils.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/arkode/arkode_bbdpre.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/arkode/arkode_bbdpre.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/sundials/sundials_direct.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/sundials/sundials_direct.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/sundials/sundials_pcg.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/sundials/sundials_pcg.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/sundials/sundials_sptfqmr.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/sundials/sundials_sptfqmr.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/sundials/LICENSE` & `amici-0.9.5/amici/ThirdParty/sundials/src/sundials/LICENSE`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/sundials/sundials_nvector.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/sundials/sundials_nvector.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/sundials/sundials_spfgmr.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/sundials/sundials_spfgmr.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/sundials/sundials_iterative.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/sundials/sundials_iterative.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/sundials/sundials_band.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/sundials/sundials_band.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/sundials/sundials_dense.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/sundials/sundials_dense.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/sundials/sundials_sparse.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/sundials/sundials_sparse.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/sundials/sundials_spgmr.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/sundials/sundials_spgmr.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/sundials/sundials_math.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/sundials/sundials_math.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/sundials/sundials_spbcgs.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/sundials/sundials_spbcgs.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/ida/ida_bbdpre.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/ida/ida_bbdpre.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/ida/ida_sparse_impl.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/ida/ida_sparse_impl.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/ida/ida_dense.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/ida/ida_dense.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/ida/ida_direct_impl.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/ida/ida_direct_impl.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/ida/ida_bbdpre_impl.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/ida/ida_bbdpre_impl.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/ida/LICENSE` & `amici-0.9.5/amici/ThirdParty/sundials/src/ida/LICENSE`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/ida/ida.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/ida/ida.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/ida/ida_impl.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/ida/ida_impl.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/ida/ida_superlumt.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/ida/ida_superlumt.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/ida/ida_spils.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/ida/ida_spils.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/ida/ida_band.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/ida/ida_band.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/ida/ida_spbcgs.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/ida/ida_spbcgs.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/ida/ida_ic.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/ida/ida_ic.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/ida/ida_lapack.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/ida/ida_lapack.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/ida/ida_direct.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/ida/ida_direct.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/ida/ida_klu.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/ida/ida_klu.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/ida/ida_io.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/ida/ida_io.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/ida/ida_spils_impl.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/ida/ida_spils_impl.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/ida/ida_spgmr.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/ida/ida_spgmr.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/ida/fcmix/fidasparse.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/ida/fcmix/fidasparse.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/ida/fcmix/fida.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/ida/fcmix/fida.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/ida/fcmix/fidaroot.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/ida/fcmix/fidaroot.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/ida/fcmix/fidalapband.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/ida/fcmix/fidalapband.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/ida/fcmix/fidaklu.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/ida/fcmix/fidaklu.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/ida/fcmix/fidabbd.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/ida/fcmix/fidabbd.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/ida/fcmix/fidadense.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/ida/fcmix/fidadense.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/ida/fcmix/fidapreco.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/ida/fcmix/fidapreco.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/ida/fcmix/fidabbd.h` & `amici-0.9.5/amici/ThirdParty/sundials/src/ida/fcmix/fidabbd.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/ida/fcmix/fida.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/ida/fcmix/fida.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/ida/fcmix/fidalapdense.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/ida/fcmix/fidalapdense.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/ida/fcmix/fidaroot.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/ida/fcmix/fidaroot.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/ida/fcmix/fidalapack.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/ida/fcmix/fidalapack.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/ida/fcmix/fidajtimes.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/ida/fcmix/fidajtimes.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/ida/fcmix/fidaband.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/ida/fcmix/fidaband.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/ida/fcmix/fidasuperlumt.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/ida/fcmix/fidasuperlumt.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/ida/fcmix/fidaewt.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/ida/fcmix/fidaewt.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/ida/ida_sptfqmr.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/ida/ida_sptfqmr.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/sundials/src/ida/ida_sparse.c` & `amici-0.9.5/amici/ThirdParty/sundials/src/ida/ida_sparse.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/LICENSE.txt` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/BTF/Include/btf.h` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/BTF/Include/btf.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/BTF/Include/btf_internal.h` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/BTF/Include/btf_internal.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/BTF/MATLAB/maxtrans.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/BTF/MATLAB/maxtrans.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/BTF/MATLAB/strongcomp.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/BTF/MATLAB/strongcomp.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/BTF/MATLAB/btf.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/BTF/MATLAB/btf.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/BTF/Source/btf_strongcomp.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/BTF/Source/btf_strongcomp.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/BTF/Source/btf_order.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/BTF/Source/btf_order.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/BTF/Source/btf_maxtrans.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/BTF/Source/btf_maxtrans.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/include/colamd.h` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/COLAMD/Include/colamd.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/include/btf.h` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/include/btf.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/include/klu.h` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Include/klu.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/include/amd.h` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/AMD/Include/amd.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/include/SuiteSparse_config.h` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/SuiteSparse_config/SuiteSparse_config.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/include/camd.h` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/CAMD/Include/camd.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/COLAMD/Include/colamd.h` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/include/colamd.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/COLAMD/Demo/colamd_l_example.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/COLAMD/Demo/colamd_l_example.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/COLAMD/Demo/colamd_example.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/COLAMD/Demo/colamd_example.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/COLAMD/MATLAB/symamdmex.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/COLAMD/MATLAB/symamdmex.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/COLAMD/MATLAB/colamdtestmex.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/COLAMD/MATLAB/colamdtestmex.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/COLAMD/MATLAB/colamdmex.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/COLAMD/MATLAB/colamdmex.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/COLAMD/MATLAB/symamdtestmex.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/COLAMD/MATLAB/symamdtestmex.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/COLAMD/Source/colamd.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/COLAMD/Source/colamd.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Include/klu.h` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/include/klu.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Include/klu_internal.h` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Include/klu_internal.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Include/klu_version.h` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Include/klu_version.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Demo/kluldemo.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Demo/kluldemo.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Demo/klu_simple.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Demo/klu_simple.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Demo/kludemo.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Demo/kludemo.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/MATLAB/klu_mex.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/MATLAB/klu_mex.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/User/klu_cholmod.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/User/klu_cholmod.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/User/klu_l_cholmod.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/User/klu_l_cholmod.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Tcov/klutest.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Tcov/klutest.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Source/klu_sort.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Source/klu_sort.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Source/klu_diagnostics.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Source/klu_diagnostics.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Source/klu_extract.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Source/klu_extract.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Source/klu_solve.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Source/klu_solve.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Source/klu_scale.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Source/klu_scale.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Source/klu_defaults.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Source/klu_defaults.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Source/klu_refactor.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Source/klu_refactor.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Source/klu_memory.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Source/klu_memory.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Source/klu_free_numeric.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Source/klu_free_numeric.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Source/klu.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Source/klu.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Source/klu_free_symbolic.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Source/klu_free_symbolic.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Source/klu_factor.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Source/klu_factor.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Source/klu_analyze_given.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Source/klu_analyze_given.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Source/klu_analyze.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Source/klu_analyze.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Source/klu_tsolve.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Source/klu_tsolve.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Source/klu_kernel.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Source/klu_kernel.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/KLU/Source/klu_dump.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/KLU/Source/klu_dump.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/CAMD/Include/camd_internal.h` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/CAMD/Include/camd_internal.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/CAMD/Include/camd.h` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/include/camd.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/CAMD/Demo/camd_simple.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/CAMD/Demo/camd_simple.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/CAMD/Demo/camd_l_demo.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/CAMD/Demo/camd_l_demo.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/CAMD/Demo/camd_demo.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/CAMD/Demo/camd_demo.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/CAMD/Demo/camd_demo2.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/CAMD/Demo/camd_demo2.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/CAMD/MATLAB/camd_mex.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/CAMD/MATLAB/camd_mex.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_postorder.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_postorder.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_aat.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_aat.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_control.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_control.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_1.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_1.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_order.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_order.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_global.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_global.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_info.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_info.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_dump.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_dump.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_defaults.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_defaults.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_2.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_2.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_valid.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_valid.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_preprocess.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/CAMD/Source/camd_preprocess.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/SuiteSparse_config/SuiteSparse_config.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/SuiteSparse_config/SuiteSparse_config.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/SuiteSparse_config/SuiteSparse_config.h` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/include/SuiteSparse_config.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/AMD/Include/amd_internal.h` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/AMD/Include/amd_internal.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/AMD/Include/amd.h` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/include/amd.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/AMD/Demo/amd_simple.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/AMD/Demo/amd_simple.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/AMD/Demo/amd_demo2.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/AMD/Demo/amd_demo2.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/AMD/Demo/amd_demo.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/AMD/Demo/amd_demo.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/AMD/Demo/amd_l_demo.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/AMD/Demo/amd_l_demo.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/AMD/Demo/amd_f77wrapper.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/AMD/Demo/amd_f77wrapper.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/AMD/MATLAB/amd_mex.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/AMD/MATLAB/amd_mex.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/AMD/Source/amd_info.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/AMD/Source/amd_info.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/AMD/Source/amd_post_tree.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/AMD/Source/amd_post_tree.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/AMD/Source/amd_preprocess.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/AMD/Source/amd_preprocess.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/AMD/Source/amd_control.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/AMD/Source/amd_control.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/AMD/Source/amd_dump.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/AMD/Source/amd_dump.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/AMD/Source/amd_postorder.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/AMD/Source/amd_postorder.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/AMD/Source/amd_order.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/AMD/Source/amd_order.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/AMD/Source/amd_2.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/AMD/Source/amd_2.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/AMD/Source/amd_defaults.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/AMD/Source/amd_defaults.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/AMD/Source/amd_aat.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/AMD/Source/amd_aat.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/AMD/Source/amd_global.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/AMD/Source/amd_global.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/AMD/Source/amd_1.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/AMD/Source/amd_1.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ThirdParty/SuiteSparse/AMD/Source/amd_valid.c` & `amici-0.9.5/amici/ThirdParty/SuiteSparse/AMD/Source/amd_valid.c`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/include/amici/model_dae.h` & `amici-0.9.5/amici/include/amici/model_dae.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/include/amici/abstract_model.h` & `amici-0.9.5/amici/include/amici/abstract_model.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/include/amici/sundials_matrix_wrapper.h` & `amici-0.9.5/amici/include/amici/sundials_matrix_wrapper.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/include/amici/rdata.h` & `amici-0.9.5/amici/include/amici/rdata.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/include/amici/defines.h` & `amici-0.9.5/amici/include/amici/defines.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/include/amici/model.h` & `amici-0.9.5/amici/include/amici/model.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/include/amici/newton_solver.h` & `amici-0.9.5/amici/include/amici/newton_solver.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/include/amici/edata.h` & `amici-0.9.5/amici/include/amici/edata.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/include/amici/misc.h` & `amici-0.9.5/amici/include/amici/misc.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/include/amici/steadystateproblem.h` & `amici-0.9.5/amici/include/amici/steadystateproblem.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/include/amici/model_ode.h` & `amici-0.9.5/amici/include/amici/model_ode.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/include/amici/backwardproblem.h` & `amici-0.9.5/amici/include/amici/backwardproblem.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/include/amici/hdf5.h` & `amici-0.9.5/amici/include/amici/hdf5.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/include/amici/cblas.h` & `amici-0.9.5/amici/include/amici/cblas.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/include/amici/vector.h` & `amici-0.9.5/amici/include/amici/vector.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/include/amici/exception.h` & `amici-0.9.5/amici/include/amici/exception.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/include/amici/interface_matlab.h` & `amici-0.9.5/amici/include/amici/interface_matlab.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/include/amici/symbolic_functions.h` & `amici-0.9.5/amici/include/amici/symbolic_functions.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/include/amici/solver_idas.h` & `amici-0.9.5/amici/include/amici/solver_idas.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/include/amici/returndata_matlab.h` & `amici-0.9.5/amici/include/amici/returndata_matlab.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/include/amici/solver.h` & `amici-0.9.5/amici/include/amici/solver.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/include/amici/serialization.h` & `amici-0.9.5/amici/include/amici/serialization.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/include/amici/solver_cvodes.h` & `amici-0.9.5/amici/include/amici/solver_cvodes.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/include/amici/forwardproblem.h` & `amici-0.9.5/amici/include/amici/forwardproblem.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/include/amici/amici.h` & `amici-0.9.5/amici/include/amici/amici.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/amici_wrap_without_hdf5.cxx` & `amici-0.9.5/amici/amici_wrap_without_hdf5.cxx`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/__init__.template.py` & `amici-0.9.5/amici/__init__.template.py`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/__init__.py` & `amici-0.9.5/amici/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -88,24 +88,27 @@
 if _commitfile:
     with open(_commitfile) as f:
         __commit__ = str(re.search(r'^([\w]*)', f.read().strip()).group())
 else:
     __commit__ = 'unknown'
 
 
-if has_clibs:
-    # these module require the swig interface
-    from .sbml_import import SbmlImporter, assignmentRules2observables, \
-        constantSpeciesToParameters
+try:
+    # These module require the swig interface and other dependencies which will
+    # be installed if the the AMICI package was properly installed. If not,
+    # AMICI was probably imported from setup.py and we don't need those.
+    from .sbml_import import SbmlImporter, assignmentRules2observables
     from .numpy import rdataToNumPyArrays, edataToNumPyArrays
     from .pandas import getEdataFromDataFrame, \
         getDataObservablesAsDataFrame, getSimulationObservablesAsDataFrame, \
         getSimulationStatesAsDataFrame, getResidualsAsDataFrame
     from .ode_export import ODEModel, ODEExporter
     from .pysb_import import pysb2amici, ODEModel_from_pysb_importer
+except ImportError:
+    pass
 
 
 def runAmiciSimulation(model, solver, edata=None):
     """ Convenience wrapper around amici.runAmiciSimulation (generated by swig)
 
     Arguments:
         model: Model instance
```

### Comparing `amici-0.9.4/amici/plotting.py` & `amici-0.9.5/amici/plotting.py`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/amici_wrap.cxx` & `amici-0.9.5/amici/amici_wrap.cxx`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/numpy.py` & `amici-0.9.5/amici/numpy.py`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/pysb_import.py` & `amici-0.9.5/amici/pysb_import.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from .ode_export import (
     ODEExporter, ODEModel, State, Constant, Parameter, Observable, SigmaY,
-    Expression, LogLikelihood, sanitize_basic_sympy
+    Expression, LogLikelihood
 )
 
 import sympy as sp
 import numpy as np
 import itertools
 
-
 try:
     import pysb.bng
     ## bool indicating whether pysb is available
     pysb_available = True
 except ImportError:
     pysb_available = False
 
@@ -167,22 +166,23 @@
         init = sp.sympify('0.0')
         for ic in model.odes.model.initial_conditions:
             if str(ic[0]) == str(specie):
                 # we don't want to allow expressions in initial conditions
                 if ic[1] in model.expressions:
                     init = model.expressions[ic[1].name].expand_expr()
                 else:
-                    init = sp.Symbol(ic[1].name)
+                    init = ic[1]
 
         ODE.add_component(
             State(
                 sp.Symbol(f'__s{ix}'),
                 f'{specie}',
                 init,
-                xdot[ix])
+                xdot[ix]
+            )
         )
 
 
 def _process_pysb_parameters(model, ODE, constants):
     """Converts pysb parameters into Parameters or Constants and adds them to
     the ODEModel instance
 
@@ -334,15 +334,15 @@
 
     Raises:
 
     """
     # only add those pysb observables that occur in the added
     # Observables as expressions
     for obs in model.observables:
-        if sp.Symbol(obs.name) in ODE.eq('y').free_symbols:
+        if obs in ODE.eq('y').free_symbols:
             ODE.add_component(
                 Expression(
                     obs,
                     f'{obs.name}',
                     obs.expand_obs()
                 )
             )
@@ -398,25 +398,24 @@
         set of monomer names
 
     Raises:
 
     """
     monomers_with_fixed_initial_conditions = set()
 
-    if hasattr(model, 'initial_conditions_fixed'):
-        for monomer in model.monomers:
-            # check if monomer has an initial condition that is fixed (means
-            #  that corresponding state is constant and all conservation
-            # laws are broken)
-            if any([
-                model.initial_conditions_fixed[ix] # true or false
-                for ix, cp in enumerate(model.initial_conditions)
-                if monomer.name in extract_monomers(cp[0])
-            ]):
-                monomers_with_fixed_initial_conditions |= {monomer.name}
+    for monomer in model.monomers:
+        # check if monomer has an initial condition that is fixed (means
+        # that corresponding state is constant and all conservation
+        # laws are broken)
+        if any([
+            ic.fixed  # true or false
+            for ic in model.initials
+            if monomer.name in extract_monomers(ic.pattern)
+        ]):
+            monomers_with_fixed_initial_conditions |= {monomer.name}
 
     return monomers_with_fixed_initial_conditions
 
 
 def _generate_cl_prototypes(excluded_monomers, model, ODE):
     """Constructs a dict that contains preprocessed information for the
     construction of conservation laws
@@ -432,14 +431,15 @@
 
     Raises:
 
     """
     cl_prototypes = dict()
 
     _compute_possible_indices(cl_prototypes, model, ODE, excluded_monomers)
+    _compute_dependency_idx(cl_prototypes)
     _compute_target_index(cl_prototypes, ODE)
 
     return cl_prototypes
 
 
 def _compute_possible_indices(cl_prototypes, model, ODE, excluded_monomers):
     """Computes viable choices for target_index, ie species that could be
@@ -450,16 +450,14 @@
         cl_prototypes: dict in which possible indices will be written @type
         dict
         model: pysb model @type pysb.core.Model
         ODE: ODEModel instance @type ODEModel
         excluded_monomers: monomers for which no conservation laws will be
         computed @type list
 
-
-
     Returns:
 
     Raises:
 
     """
     for monomer in model.monomers:
         if monomer.name not in excluded_monomers:
@@ -494,14 +492,60 @@
                 prototype['possible_indices']
             )
 
             if prototype['possible_indices']:
                 cl_prototypes[monomer.name] = prototype
 
 
+def _compute_dependency_idx(cl_prototypes):
+    """Compute connecting species, this allows us to efficiently compute
+    whether the respective conservation law would induce a cyclic dependency.
+    Adds a 'dependency_idx' field to the prototype dict that
+    itself is a dict where keys correspond to indexes that, when used as
+    target index yield dependencies on conservation laws of monomers in
+    the respective values
+
+    Arguments:
+        cl_prototypes: dict in which possible indices will be written @type
+        dict
+
+    Returns:
+
+    Raises:
+
+    """
+    #
+    for monomer_i, prototype_i in cl_prototypes.items():
+        if 'dependency_idx' not in prototype_i:
+            prototype_i['dependency_idx'] = dict()
+
+        for monomer_j, prototype_j in cl_prototypes.items():
+            if monomer_i == monomer_j:
+                continue
+
+            if 'dependency_idx' not in prototype_j:
+                prototype_j['dependency_idx'] = dict()
+
+            idx_overlap = set(prototype_i['possible_indices']).intersection(
+                set(prototype_j['possible_indices'])
+            )
+            if len(idx_overlap) == 0:
+                continue
+
+            for idx in idx_overlap:
+                if idx not in prototype_i['dependency_idx']:
+                    prototype_i['dependency_idx'][idx] = set()
+
+                if idx not in prototype_j['dependency_idx']:
+                    prototype_j['dependency_idx'][idx] = set()
+
+                prototype_i['dependency_idx'][idx] |= {monomer_j}
+                prototype_j['dependency_idx'][idx] |= {monomer_i}
+
+
 def _compute_target_index(cl_prototypes, ODE):
     """Computes the target index for every monomer
 
 
     Arguments:
         cl_prototypes: dict that contains possible indices for every monomer
         @type dict
@@ -522,14 +566,16 @@
     # are also populated from conservation laws. In case there are many
     # state heavy expressions in the model (should not be the case for mass
     # action kinetics). This may lead to suboptimal results and could improved.
     # As this would require substantial code shuffling, this will only be
     # fixed if this becomes an actual problem
     appearance_counts = ODE.get_appearance_counts(possible_indices)
 
+    # in this initial guess we ignore the cost of having cyclic dependencies
+    # between conservation laws
     for monomer in cl_prototypes:
         prototype = cl_prototypes[monomer]
         # extract monomer specific appearance counts
         prototype['appearance_counts'] = \
             [
                 appearance_counts[possible_indices.index(idx)]
                 for idx in prototype['possible_indices']
@@ -553,20 +599,120 @@
         # vary too much across conservation laws, this approximation
         # should be fine
         prototype['fillin'] = \
             prototype['appearance_count'] * prototype['species_count']
 
     # we might end up with the same index for multiple monomers, so loop until
     # we have a set of unique target indices
-    while len(cl_prototypes) > len(set(get_target_indices(cl_prototypes))):
+    while not _cl_prototypes_are_valid(cl_prototypes):
         _greedy_target_index_update(cl_prototypes)
 
+def _cl_prototypes_are_valid(cl_prototypes):
+    """Checks consistency of cl_prototypes by asserting that target indices
+    are unique and there are no cyclic dependencies
+
+    Arguments:
+        cl_prototypes: dict that contains dependency and target indexes for
+        every monomer @type dict
+
+    Returns:
+
+    Raises:
+
+    """
+    # target indices are unique
+    if len(cl_prototypes) != len(set(get_target_indices(cl_prototypes))):
+        return False
+    # conservation law dependencies are cycle free
+    if any(
+        _cl_has_cycle(monomer, cl_prototypes)
+        for monomer in cl_prototypes
+    ):
+        return False
+
+    return True
+
+def _cl_has_cycle(monomer, cl_prototypes):
+    """Checks whether monomer has a conservation law that is part of a
+    cyclic dependency
+
+    Arguments:
+        monomer: name of monomer for which conservation law is to be checked
+        cl_prototypes: dict that contains dependency and target indexes for
+        every monomer @type dict
+
+    Returns:
+
+    Raises:
+
+    """
+
+    prototype = cl_prototypes[monomer]
+
+    if prototype['target_index'] not in prototype['dependency_idx']:
+        return False
+
+    visited = [monomer]
+    root = monomer
+    return any(
+        _is_in_cycle(
+            connecting_monomer,
+            cl_prototypes,
+            visited,
+            root
+        )
+        for connecting_monomer in prototype['dependency_idx'][
+            prototype['target_index']
+        ]
+    )
+
+def _is_in_cycle(monomer, cl_prototypes, visited, root):
+    """Recursively checks for cycles in conservation law dependencies via
+    Depth First Search
+
+    Arguments:
+        monomer: current location in cl dependency graph
+        cl_prototypes: dict that contains dependency and target indexes for
+        every monomer @type dict
+        visited: history of visited monomers with conservation laws
+        root: monomer at which the cycle search was started
+
+    Returns:
+
+    Raises:
+
+    """
+    if monomer == root:
+        return True # we found a cycle and root is part of it
+
+    if monomer in visited:
+        return False # we found a cycle but root is not part of it
+
+    visited.append(monomer)
+
+    prototype = cl_prototypes[monomer]
+
+    if prototype['target_index'] not in prototype['dependency_idx']:
+        return False
+
+    return any(
+        _is_in_cycle(
+            connecting_monomer,
+            cl_prototypes,
+            visited,
+            root
+        )
+        for connecting_monomer in prototype['dependency_idx'][
+            prototype['target_index']
+        ]
+    )
+
 
 def _greedy_target_index_update(cl_prototypes):
-    """Computes unique target indices for conservation laws from prossible
+    """Computes unique target indices for conservation laws from possible
     indices  such that expected fill in in symbolic derivatives is minimized
 
 
     Arguments:
         cl_prototypes: dict that contains possible indices and non-unique
         target indices for every monomer @type dict
 
@@ -575,17 +721,17 @@
     Raises:
         Exception if no suitable solution could be found
 
     """
 
     target_indices = get_target_indices(cl_prototypes)
 
-    for monomer in cl_prototypes:
-        prototype = cl_prototypes[monomer]
-        if target_indices.count(prototype['target_index']) > 1:
+    for monomer, prototype in cl_prototypes.items():
+        if target_indices.count(prototype['target_index']) > 1 or \
+                _cl_has_cycle(monomer, cl_prototypes):
             # compute how much fillin the next best target_index would yield
 
             # we exclude already existing target indices to avoid that
             # updating the target index removes uniqueness from already unique
             # target indices, this may slightly reduce chances of finding a
             # solution but prevents infinite loops
             for target_index in list(set(target_indices)):
@@ -597,18 +743,16 @@
                     local_idx = None
 
                 if local_idx:
                     del prototype['possible_indices'][local_idx]
                     del prototype['appearance_counts'][local_idx]
 
             if len(prototype['possible_indices']) == 0:
-                # we have exhausted all possible target indices, nothing left
-                # we can do
-                raise Exception('Could not compute a valid set of '
-                                'conservation laws for this model')
+                prototype['diff_fillin'] = -1
+                continue
 
             idx = np.argmin(prototype['appearance_counts'])
 
             prototype['local_index'] = idx
             prototype['alternate_target_index'] = \
                 prototype['possible_indices'][idx]
             prototype['alternate_appearance_count'] = \
@@ -617,15 +761,22 @@
             prototype['alternate_fillin'] = \
                 prototype['alternate_appearance_count'] \
                 * prototype['species_count']
 
             prototype['diff_fillin'] = \
                 prototype['alternate_fillin'] - prototype['fillin']
         else:
-            prototype['diff_fillin'] = 0
+            prototype['diff_fillin'] = -1
+
+    if all(
+        prototype['diff_fillin'] == -1
+        for prototype in cl_prototypes.values()
+    ):
+        raise Exception('Could not compute a valid set of conservation '
+                        'laws for this model!')
 
     # this puts prototypes with high diff_fillin last
     cl_prototypes = sorted(
         cl_prototypes.items(), key=lambda kv: kv[1]['diff_fillin']
     )
     cl_prototypes = {
         proto[0]: proto[1]
@@ -633,23 +784,27 @@
     }
 
     for monomer in cl_prototypes:
         prototype = cl_prototypes[monomer]
         # we check that we
         # A) have an alternative index computed, i.e. that
         # that monomer originally had a non-unique target_index
-        # B) that the target_index still is not unique. due to the sorting,
-        # this will always be the monomer with the highest diff_fillin (note
-        # that the target indice counts are recomputed on the fly
-
-        if prototype['diff_fillin'] > 0 \
-                and get_target_indices(cl_prototypes).count(
-                    prototype['target_index']
-                ) > 1:
+        # B) that the target_index still is not unique or part of a cyclic
+        # dependency. due to the sorting, this will always be the monomer
+        # with the highest diff_fillin (note that the target index counts
+        # are recomputed on the fly)
+
 
+        if prototype['diff_fillin'] > -1 \
+                and (
+                    get_target_indices(cl_prototypes).count(
+                        prototype['target_index']
+                    ) > 1
+                    or _cl_has_cycle(monomer, cl_prototypes)
+        ):
             prototype['fillin'] = prototype['alternate_fillin']
             prototype['target_index'] = prototype['alternate_target_index']
             prototype['appearance_count'] = \
                 prototype['alternate_appearance_count']
 
             del prototype['possible_indices'][prototype['local_index']]
             del prototype['appearance_counts'][prototype['local_index']]
@@ -691,24 +846,21 @@
     for monomer_name in cl_prototypes:
         target_index = cl_prototypes[monomer_name]['target_index']
 
         # T = sum_i(a_i * x_i)
         # x_j = (T - sum_i≠j(a_i * x_i))/a_j
         # law: sum_i≠j(a_i * x_i))/a_j
         # state: x_j
-        target_expression = sanitize_basic_sympy(
-            sum(
-                sp.Symbol(f'__s{ix}')
-                * extract_monomers(specie).count(monomer_name)
-                for ix, specie in enumerate(model.species)
-                if ix != target_index
-            )
-            /
-            extract_monomers(model.species[target_index]).count(monomer_name)
-        )  # normalize by the stoichiometry of the target species
+        target_expression = sum(
+            sp.Symbol(f'__s{ix}')
+            * extract_monomers(specie).count(monomer_name)
+            for ix, specie in enumerate(model.species)
+            if ix != target_index
+        ) / extract_monomers(model.species[target_index]).count(monomer_name)
+        # normalize by the stoichiometry of the target species
         target_state = sp.Symbol(f'__s{target_index}')
         # = x_j
 
         total_abundance = sp.Symbol(f'tcl__s{target_index}')
         # = T/a_j
 
         state_expr = total_abundance - target_expression
@@ -767,20 +919,81 @@
 
     Raises:
 
     """
     conservation_law_subs = \
         _get_conservation_law_subs(conservation_laws)
 
-    # we actually need to ma
     while len(conservation_law_subs):
         for cl in conservation_laws:
-            cl['state_expr'] = cl['state_expr'].subs(conservation_law_subs)
-            conservation_law_subs = \
-                _get_conservation_law_subs(conservation_laws)
+            if _sub_matches_cl(
+                    conservation_law_subs,
+                    cl['state_expr'],
+                    cl['state']
+            ):
+                # this optimization is done by subs anyways, but we dont
+                # want to recompute the subs if we did not change anything
+                valid_subs = _select_valid_cls(
+                    conservation_law_subs,
+                    cl['state']
+                )
+                if len(valid_subs) > 0:
+                    cl['state_expr'] = cl['state_expr'].subs(valid_subs)
+                    conservation_law_subs = \
+                        _get_conservation_law_subs(conservation_laws)
+
+def _select_valid_cls(subs, state):
+    """ Subselect substitutions such that we do not end up with conservation
+    laws that are self-referential
+
+    Arguments:
+        subs: substitutions in tuple format
+        state: target symbolic state to which substitutions will
+        be applied
+
+    Returns:
+    list of valid substitutions
+
+    Raises:
+
+    """
+    return [
+        sub
+        for sub in subs
+        if str(state) not in [str(symbol) for symbol in sub[1].free_symbols]
+    ]
+
+
+def _sub_matches_cl(subs, state_expr, state):
+    """ Checks whether any of the substitutions in subs will be applied to
+    state_expr
+
+    Arguments:
+        subs: substitutions in tuple format
+        state_expr: target symbolic expressions in which substitutions will
+        be applied
+        state: target symbolic state to which substitutions will
+        be applied
+
+    Returns:
+    boolean indicating positive match
+
+    Raises:
+
+    """
+
+    sub_symbols = set(
+        sub[0]
+        for sub in subs
+        if str(state) not in [
+            str(symbol) for symbol in sub[1].free_symbols
+        ]
+    )
+
+    return len(sub_symbols.intersection(state_expr.free_symbols)) > 0
 
 
 def _get_conservation_law_subs(conservation_laws):
     """ Returns a list of (state, law) tuples for conservation laws that still
     appear in other conservation laws
 
     Arguments:
```

### Comparing `amici-0.9.4/amici/swig/amici.i` & `amici-0.9.5/amici/swig/amici.i`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/swig/std_unique_ptr.i` & `amici-0.9.5/amici/swig/std_unique_ptr.i`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/swig/CMakeLists_model.txt` & `amici-0.9.5/amici/swig/CMakeLists_model.txt`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/swig/stdvec2numpy.h` & `amici-0.9.5/amici/swig/stdvec2numpy.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/setuptools.py` & `amici-0.9.5/amici/setuptools.py`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/setup.template.py` & `amici-0.9.5/amici/setup.template.py`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/sbml_import.py` & `amici-0.9.5/amici/sbml_import.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 """ @package amici.sbml_import The python sbml import module for python
 """
 
 import sympy as sp
 import libsbml as sbml
 import re
 import math
+import warnings
 from sympy.logic.boolalg import BooleanTrue as spTrue
 from sympy.logic.boolalg import BooleanFalse as spFalse
 
 from .ode_export import ODEExporter, ODEModel
-
+from . import has_clibs
 
 class SBMLException(Exception):
     pass
 
 ## default dict for symbols
 default_symbols = {
     'species': {},
@@ -23,14 +24,15 @@
     'observable': {},
     'expression': {},
     'sigmay': {},
     'my': {},
     'llhy': {},
 }
 
+
 class SbmlImporter:
     """The SbmlImporter class generates AMICI C++ files for a model provided in
     the Systems Biology Markup Language (SBML).
 
     Attributes:
 
         show_sbml_warnings: indicates whether libSBML warnings should be
@@ -147,50 +149,54 @@
         # check the error log just once after all conversion/validation calls.
         checkLibSBMLErrors(self.sbml_doc, self.show_sbml_warnings)
 
         self.sbml = self.sbml_doc.getModel()
 
     def sbml2amici(self,
                    modelName,
-                   output_dir=None,
-                   observables=None,
-                   constantParameters=None,
-                   sigmas=None,
-                   verbose=False,
-                   assume_pow_positivity=False,
-                   compiler=None,
-                   allow_reinit_fixpar_initcond = True
+                   output_dir = None,
+                   observables = None,
+                   constantParameters = None,
+                   sigmas = None,
+                   verbose = False,
+                   assume_pow_positivity = False,
+                   compiler = None,
+                   allow_reinit_fixpar_initcond = True,
+                   compile = True
                    ):
         """Generate AMICI C++ files for the model provided to the constructor.
 
         Arguments:
             modelName: name of the model/model directory @type str
 
-            output_dir: see sbml_import.setPaths()  @type str
+            output_dir: see sbml_import.setPaths() @type str
 
             observables: dictionary( observableId:{'name':observableName
-            (optional), 'formula':formulaString)}) to be added to the model
-            @type dict
+                (optional), 'formula':formulaString)}) to be added to the model
+                @type dict
 
-            sigmas: dictionary(observableId: sigma value or (existing)
-            parameter name) @type dict
+            sigmas: dictionary(observableId: sigma value or (existing) parameter name)
+                @type dict
 
-            constantParameters: list of SBML Ids identifying constant
-            parameters @type dict
+            constantParameters: list of SBML Ids identifying constant parameters
+                @type list
 
             verbose: more verbose output if True @type bool
 
             assume_pow_positivity: if set to true, a special pow function is
-            used to avoid problems with state variables that may become
-            negative due to numerical errors @type bool
+                used to avoid problems with state variables that may become
+                negative due to numerical errors @type bool
 
             compiler: distutils/setuptools compiler selection to build the
-            python extension @type str
+                python extension @type str
 
-            allow_reinit_fixpar_initcond: see ode_export.ODEExporter
+            allow_reinit_fixpar_initcond: see ode_export.ODEExporter @type bool
+
+            compile: If True, compile the generated Python package, if False, just
+                generate code. @type bool
 
         Returns:
 
         Raises:
 
         """
         if observables is None:
@@ -214,15 +220,20 @@
             assume_pow_positivity=assume_pow_positivity,
             compiler=compiler,
             allow_reinit_fixpar_initcond=allow_reinit_fixpar_initcond
         )
         exporter.setName(modelName)
         exporter.setPaths(output_dir)
         exporter.generateModelCode()
-        exporter.compileModel()
+
+        if compile:
+            if not has_clibs:
+                warnings.warn('AMICI C++ extensions have not been built. '
+                              'Generated model code, but unable to compile.')
+            exporter.compileModel()
 
     def processSBML(self, constantParameters=None):
         """Read parameters, species, reactions, and so on from SBML model
 
         Arguments:
             constantParameters: SBML Ids identifying constant parameters
             @type list
@@ -348,29 +359,23 @@
                 symMath = sp.sympify(
                     sbml.formulaToL3String(initial_assignment.getMath())
                 )
                 if symMath is not None:
                     _check_unsupported_functions(symMath, 'InitialAssignment')
                     speciesInitial[index] = symMath
 
+        for ix, (symbol, init) in enumerate(zip(
+                    self.symbols['species']['identifier'], speciesInitial
+        )):
+            if symbol == init:
+                speciesInitial[ix] = sp.sympify(0.0)
+
         # flatten initSpecies
         while any([species in speciesInitial.free_symbols
                    for species in self.symbols['species']['identifier']]):
-            identical_assignment = next((
-                symbol == init
-                for symbol, init in zip(
-                    self.symbols['species']['identifier'], speciesInitial
-                )
-            ), None)
-            if identical_assignment is not None:
-                raise SBMLException('Species without initial assignment are '
-                                    'currently not supported (this is error '
-                                    'is likely to be due to the existence of '
-                                    'a species assignment rule, which is '
-                                    'also not supported)!')
             speciesInitial = speciesInitial.subs([
                 (symbol, init)
                 for symbol, init in zip(
                     self.symbols['species']['identifier'], speciesInitial
                 )
             ])
 
@@ -680,15 +685,16 @@
 
             if variable in volumevars:
                 self.compartmentVolume = \
                     self.compartmentVolume.subs(variable, formula)
 
             if variable in rulevars:
                 for nested_rule in rules:
-                    nested_formula = sp.sympify(nested_rule.getFormula())
+                    nested_formula = sp.sympify(
+                        sbml.formulaToL3String(nested_rule.getMath()))
                     nested_formula = \
                         nested_formula.subs(variable, formula)
                     nested_rule.setFormula(str(nested_formula))
 
                 for variable in assignments:
                     assignments[variable].subs(variable, formula)
 
@@ -942,103 +948,19 @@
     Returns:
     Tuple of free symbolic variables in the formulas all provided rules
 
     Raises:
 
     """
     return sp.Matrix(
-        [sp.sympify(rule.getFormula()) for rule in rules
+        [sp.sympify(sbml.formulaToL3String(rule.getMath())) for rule in rules
          if rule.getFormula() != '']
     ).free_symbols
 
 
-def assignmentRules2observables(sbml_model,
-                                filter_function=lambda *_: True):
-    """Turn assignment rules into observables.
-
-    Arguments:
-    sbml_model: an sbml Model instance
-
-    filter_function: callback function taking assignment variable as input
-    and returning True/False to indicate if the respective rule should be
-    turned into an observable
-
-    Returns:
-    A dictionary(observableId:{
-        'name': observableName,
-        'formula': formulaString
-    })
-
-    Raises:
-
-    """
-    observables = {}
-    for p in sbml_model.getListOfParameters():
-        parameter_id = p.getId()
-        if filter_function(p):
-            observables[parameter_id] = {
-                'name': p.getName(),
-                'formula': sbml_model.getAssignmentRuleByVariable(
-                    parameter_id
-                ).getFormula()
-            }
-
-    for parameter_id in observables:
-        sbml_model.removeRuleByVariable(parameter_id)
-        sbml_model.removeParameter(parameter_id)
-
-    return observables
-
-
-def constantSpeciesToParameters(sbml_model):
-    """Convert constant species in the SBML model to constant parameters
-
-    Arguments:
-
-    sbml_model: libsbml model instance
-
-    Returns:
-    species IDs that have been turned into constants
-
-    Raises:
-
-    """
-    transformable = []
-    for species in sbml_model.getListOfSpecies():
-        if not species.getConstant() and not species.getBoundaryCondition():
-            continue
-        if species.getHasOnlySubstanceUnits():
-            print(f"Ignoring {species.getId()} which has only substance units."
-                  " Conversion not yet implemented.")
-            continue
-        if math.isnan(species.getInitialConcentration()):
-            print(f"Ignoring {species.getId()} which has no initial "
-                  "concentration. Amount conversion not yet implemented.")
-            continue
-        transformable.append(species.getId())
-
-    # Must not remove species while iterating over getListOfSpecies()
-    for speciesId in transformable:
-        species = sbml_model.removeSpecies(speciesId)
-        par = sbml_model.createParameter()
-        par.setId(species.getId())
-        par.setName(species.getName())
-        par.setConstant(True)
-        par.setValue(species.getInitialConcentration())
-        par.setUnits(species.getUnits())
-
-    # Remove from reactants and products
-    for reaction in sbml_model.getListOfReactions():
-        for speciesId in transformable:
-            reaction.removeReactant(speciesId)
-            reaction.removeProduct(speciesId)
-
-    return transformable
-
-
 def replaceLogAB(x):
     """Replace log(a, b) in the given string by ln(b)/ln(a)
 
     Works for nested parentheses and nested 'log's. This can be used to
     circumvent the incompatible argument order between symengine (log(x,
     basis)) and libsbml (log(basis, x)).
 
@@ -1181,7 +1103,43 @@
         if unsupp_fun_type:
             raise SBMLException(f'Encountered unsupported expression '
                                 f'"{fun}" of type '
                                 f'"{unsupp_fun_type}" as part of a '
                                 f'{expression_type}: "{full_sym}"!')
         if fun is not sym:
             _check_unsupported_functions(fun, expression_type)
+
+
+def assignmentRules2observables(sbml_model,
+                                filter_function=lambda *_: True):
+    """Turn assignment rules into observables.
+    Arguments:
+    sbml_model: an sbml Model instance
+    filter_function: callback function taking assignment variable as input
+    and returning True/False to indicate if the respective rule should be
+    turned into an observable
+    Returns:
+    A dictionary(observableId:{
+        'name': observableName,
+        'formula': formulaString
+    })
+    Raises:
+    """
+    warnings.warn("This function will be removed in future releases. "
+                  "This functionality is now included in "
+                  "https://github.com/ICB-DCM/PEtab .", DeprecationWarning)
+    observables = {}
+    for p in sbml_model.getListOfParameters():
+        parameter_id = p.getId()
+        if filter_function(p):
+            observables[parameter_id] = {
+                'name': p.getName(),
+                'formula': sbml_model.getAssignmentRuleByVariable(
+                    parameter_id
+                ).getFormula()
+            }
+
+    for parameter_id in observables:
+        sbml_model.removeRuleByVariable(parameter_id)
+        sbml_model.removeParameter(parameter_id)
+
+    return observables
```

### Comparing `amici-0.9.4/amici/amici.py` & `amici-0.9.5/amici/amici.py`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/amici_without_hdf5.py` & `amici-0.9.5/amici/amici_without_hdf5.py`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/src/forwardproblem.cpp` & `amici-0.9.5/amici/src/forwardproblem.cpp`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/src/misc.cpp` & `amici-0.9.5/amici/src/misc.cpp`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/src/steadystateproblem.cpp` & `amici-0.9.5/amici/src/steadystateproblem.cpp`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/src/CMakeLists.template.txt` & `amici-0.9.5/amici/src/CMakeLists.template.txt`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/src/spline.cpp` & `amici-0.9.5/amici/src/spline.cpp`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/src/solver_idas.cpp` & `amici-0.9.5/amici/src/solver_idas.cpp`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/src/model_header.ODE_template.h` & `amici-0.9.5/amici/src/model_header.ODE_template.h`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/src/rdata.cpp` & `amici-0.9.5/amici/src/rdata.cpp`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/src/amici.cpp` & `amici-0.9.5/amici/src/amici.cpp`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/src/sundials_matrix_wrapper.cpp` & `amici-0.9.5/amici/src/sundials_matrix_wrapper.cpp`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/src/model_ode.cpp` & `amici-0.9.5/amici/src/model_ode.cpp`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/src/model_dae.cpp` & `amici-0.9.5/amici/src/model_dae.cpp`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/src/hdf5.cpp` & `amici-0.9.5/amici/src/hdf5.cpp`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/src/backwardproblem.cpp` & `amici-0.9.5/amici/src/backwardproblem.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
     /* we still need to integrate from first datapoint to tstart */
     if (t > model->t0()) {
         /* solve for backward problems */
         solver->solveB(model->t0(), AMICI_NORMAL);
         solver->getQuadB(which, &(t), &xQB);
         solver->getB(which, &(t), &xB, &dxB);
-        solver->getDiagnosisB(it, rdata, this->which);
+        solver->getDiagnosisB(0, rdata, this->which);
     }
 
     computeLikelihoodSensitivities();
 }
 
 
 void BackwardProblem::handleEventB(const int iroot) {
```

### Comparing `amici-0.9.4/amici/src/symbolic_functions.cpp` & `amici-0.9.5/amici/src/symbolic_functions.cpp`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/src/abstract_model.cpp` & `amici-0.9.5/amici/src/abstract_model.cpp`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/src/solver_cvodes.cpp` & `amici-0.9.5/amici/src/solver_cvodes.cpp`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/src/cblas.cpp` & `amici-0.9.5/amici/src/cblas.cpp`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/src/model.cpp` & `amici-0.9.5/amici/src/model.cpp`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/src/newton_solver.cpp` & `amici-0.9.5/amici/src/newton_solver.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -366,14 +366,15 @@
      * linsolveSPBCG
      *
      * @param rhs containing the RHS of the linear system, will be
      * overwritten by solution to the linear system
      */
 
     linsolveSPBCG(newton_try, i_newton, rhs);
+    rhs->minus();
 }
 
 
 void NewtonSolverIterative::linsolveSPBCG(int ntry,int nnewt, AmiVector *ns_delta) {
     /**
      * Iterative linear solver created from SPILS BiCG-Stab.
      * Solves the linear system within each Newton step if iterative solver is
```

### Comparing `amici-0.9.4/amici/src/edata.cpp` & `amici-0.9.5/amici/src/edata.cpp`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/src/main.template.cpp` & `amici-0.9.5/amici/src/main.template.cpp`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/src/solver.cpp` & `amici-0.9.5/amici/src/solver.cpp`

 * *Files identical despite different names*

### Comparing `amici-0.9.4/amici/ode_export.py` & `amici-0.9.5/amici/ode_export.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import re
 import shutil
 import subprocess
 import sys
 import os
 import copy
 import numbers
+import itertools
 try:
     import pysb
 except ImportError:
     ## pysb import dummy
     pysb = None
 
 
@@ -299,17 +300,15 @@
 class ModelQuantity:
     """Base class for model components
 
     Attributes:
 
     """
     def __init__(self, identifier,  name, value):
-        """Create a new ModelQuantity instance. This function sanitizes
-        input from pysb to make sure we are operating on flat symby.Symbol and
-        sympy.Basic and not respective derived pysb classes
+        """Create a new ModelQuantity instance.
 
         Arguments:
             identifier: unique identifier of the quantity @type sympy.Symbol
 
             name: individual name of the quantity (does not need to be unique)
             @type str
 
@@ -318,40 +317,31 @@
         Returns:
         ModelQuantity instance
 
         Raises:
         TypeError:
             is thrown if input types do not match documented types
         """
+
         if not isinstance(identifier, sp.Symbol):
             raise TypeError(f'identifier must be sympy.Symbol, was '
                             f'{type(identifier)}')
-        if pysb and isinstance(identifier, pysb.Component):
-            # strip pysb type and transform into a flat sympy.Symbol.
-            # this prevents issues where pysb expressions, observables or
-            # parameters are not recognized as an sp.Symbol with same
-            # symbolic name
-            self._identifier = sp.Symbol(identifier.name)
-        else:
-            self._identifier = identifier
+        self._identifier = identifier
 
         if not isinstance(name, str):
             raise TypeError(f'name must be str, was {type(name)}')
         self._name = name
 
         if isinstance(value, sp.RealNumber) \
                 or isinstance(value, numbers.Number):
             value = float(value)
         if not isinstance(value, sp.Basic) and not isinstance(value, float):
             raise TypeError(f'value must be sympy.Symbol or float, was '
                             f'{type(value)}')
-        if isinstance(value, sp.Basic):
-            self._value = sanitize_basic_sympy(value)
-        else:
-            self._value = value
+        self._value = value
 
     def __repr__(self):
         """Representation of the ModelQuantity object
 
         Arguments:
 
         Returns:
@@ -435,15 +425,15 @@
             is thrown if input types do not match documented types
         """
         super(State, self).__init__(identifier, name, value)
         if not isinstance(dt, sp.Basic):
             raise TypeError(f'dt must have type sympy.Basic, was '
                             f'{type(dt)}')
 
-        self._dt = sanitize_basic_sympy(dt)
+        self._dt = dt
         self.conservation_law = None
 
     def set_conservation_law(self, law):
         """Sets the conservation law of a state. If the a conservation law
         is set, the respective state will be replaced by an algebraic
         formula according to the respective conservation law.
 
@@ -1214,29 +1204,29 @@
             component = self._variable_prototype[name]
             self._syms[name] = sp.Matrix([
                 comp.get_id()
                 for comp in getattr(self, component)
             ])
             if name == 'y':
                 self._syms['my'] = sp.Matrix([
-                    sp.Symbol(f'm{comp.get_id()}')
+                    sp.Symbol(f'm{strip_pysb(comp.get_id())}')
                     for comp in getattr(self, component)
                 ])
             return
         elif name == 'x':
             self._syms[name] = sp.Matrix([
                 state.get_id()
                 for state in self._states
                 if state.conservation_law is None
             ])
             return
         elif name == 'dtcldp':
             self._syms[name] = sp.Matrix([
                 [
-                    sp.Symbol(f's{tcl.get_id()}{ip}')
+                    sp.Symbol(f's{strip_pysb(tcl.get_id())}_{ip}')
                     for ip in range(len(self.sym('p')))
                 ]
                 for tcl in self._conservationlaws
             ])
             return
         elif name in sparse_functions:
             self._generateSparseSymbol(name)
@@ -1277,24 +1267,34 @@
         Returns:
             list of counts for the states ordered according to the provided
             indices
 
         Raises:
 
         """
+        free_symbols_dt = list(itertools.chain.from_iterable(
+            [
+                str(symbol)
+                for symbol in state.get_dt().free_symbols
+            ]
+            for state in self._states
+        ))
+
+        free_symbols_expr = list(itertools.chain.from_iterable(
+            [
+                str(symbol)
+                for symbol in expr.get_val().free_symbols
+            ]
+            for expr in self._expressions
+        ))
+
         return [
-            sum(
-                self._states[idx].get_id() in state.get_dt().free_symbols
-                for state in self._states
-            )
+            free_symbols_dt.count(str(self._states[idx].get_id()))
             +
-            sum(
-                self._states[idx].get_id() in expr.get_val().free_symbols
-                for expr in self._expressions
-            )
+            free_symbols_expr.count(str(self._states[idx].get_id()))
             for idx in idxs
         ]
 
     def _generateSparseSymbol(self, name):
         """Generates the sparse symbolic identifiers, symbolic identifiers,
         sparse equations, column pointers and row values for a symbolic
         variable
@@ -1540,15 +1540,16 @@
                           dydx_name=None, dxdz_name=None):
         """Creates a new symbolic variable according to a total derivative
         using the chain rule
 
         Arguments:
             name: name of resulting symbolic variable @type str
 
-            eq: name of the symbolic variable that defines the formula @type str
+            eq: name of the symbolic variable that defines the formula
+            @type str
 
             chainvars: names of the symbolic variable that define the
             identifiers with respect to which the chain rules are applied
             @type list
 
             var: name of the symbolic variable that defines the identifiers
             whith respect to which the derivatives are to be computed @type str
@@ -1875,25 +1876,27 @@
 
         # To only generate a subset of functions, apply subselection here
         self.functions = copy.deepcopy(functions)
 
         self.allow_reinit_fixpar_initcond = allow_reinit_fixpar_initcond
 
     def generateModelCode(self):
-        """Generates the native C++ code for the loaded model
+        """Generates the native C++ code for the loaded model and a Matlab
+        script that can be run to compile a mex file from the C++ code
 
         Arguments:
 
         Returns:
 
         Raises:
 
         """
         self._prepareModelFolder()
         self._generateCCode()
+        self._generateMCode()
 
     def compileModel(self):
         """Compiles the generated code it into a simulatable module
 
         Arguments:
 
         Returns:
@@ -1940,15 +1943,14 @@
         self._writeCMakeFile()
         self._writeSwigFiles()
         self._writeModuleSetup()
 
         shutil.copy(os.path.join(amiciSrcPath, 'main.template.cpp'),
                     os.path.join(self.modelPath, 'main.cpp'))
 
-
     def _compileCCode(self, verbose=False, compiler=None):
         """Compile the generated model code
 
         Arguments:
             verbose: Make model compilation verbose @type bool
 
             compiler: distutils/setuptools compiler selection to build the
@@ -1985,14 +1987,62 @@
         except subprocess.CalledProcessError as e:
             print(e.output.decode('utf-8'))
             raise
 
         if verbose:
             print(result.stdout.decode('utf-8'))
 
+    def _generateMCode(self):
+        """Create a Matlab script for compiling code files to a mex file
+
+        Arguments:
+
+        Returns:
+
+        Raises:
+
+        """
+        # creating the code lines for the Matlab compile script
+        lines = []
+
+        # Events are not yet implemented. Once this is done, the variable nz
+        # will have to be replaced by "self.model.nz()"
+        nz = 0
+
+        # Second order code is not yet implemented. Once this is done,
+        # those variables will have to be replaced by
+        # "self.model.<var>true()", or the corresponding "model.self.o2flag"
+        nxtrue_rdata = self.model.nx_rdata()
+        nytrue = self.model.ny()
+        o2flag = 0
+
+        # a preliminary comment
+        lines.append('% This compile script was automatically created from Python SBML import.')
+        lines.append('% If mex compiler is set up within MATLAB, it can be run from MATLAB ')
+        lines.append('% in order to compile a mex-file from the Python generated C++ files.')
+        lines.append('')
+
+        # write the actual compiling code
+        lines.append('''modelName = '{model_name}';'''.format(
+            model_name=self.modelName))
+        lines.append('''amimodel.compileAndLinkModel(modelName, '', [], [], [], []);''')
+        lines.append('''amimodel.generateMatlabWrapper({nx}, {ny}, {np}, {nk}, {nz}, {o2flag}, [], ...
+            ['simulate_' modelName '.m'], modelName, 'lin', 1, 1);'''.format(
+            nx=nxtrue_rdata,
+            ny=nytrue,
+            np=self.model.np(),
+            nk=self.model.nk(),
+            nz=nz,
+            o2flag=o2flag
+            ))
+
+        # write compile script (for mex)
+        with open(os.path.join(self.modelPath, 'compileMexFile.m'), 'w') as fileout:
+            fileout.write('\n'.join(lines))
+
     def _writeIndexFiles(self, name):
         """Write index file for a symbolic array.
 
         Arguments:
             name: key in self.model._syms for which the respective file should
             be written @type str
 
@@ -2008,24 +2058,25 @@
                 symbols = self.model.sparsesym(name)
             else:
                 symbols = self.model.sym(name).T
         else:
             raise Exception('Unknown symbolic array')
 
         for index, symbol in enumerate(symbols):
-            symbol_name = str(symbol)
+            symbol_name = strip_pysb(symbol)
             lines.append(
                 f'#define {symbol_name} {name}[{index}]'
             )
 
-        with open(os.path.join(self.modelPath,f'{name}.h'), 'w') as fileout:
+        with open(os.path.join(self.modelPath, f'{name}.h'), 'w') as fileout:
             fileout.write('\n'.join(lines))
 
     def _writeFunctionFile(self, function):
-        """Generate equations and write the C++ code for the function `function`.
+        """Generate equations and write the C++ code for the function
+        `function`.
 
         Arguments:
             function: name of the function to be written (see self.functions)
             @type str
 
         Returns:
 
@@ -2053,15 +2104,15 @@
             '#include <cmath>',
             ''
         ]
 
         # function signature
         signature = self.functions[function]['signature']
 
-        if not signature.find('SlsMat') == -1:
+        if 'SlsMat' in signature:
             lines.append('#include <sundials/sundials_sparse.h>')
 
         lines.append('')
 
         for sym in self.model.symNames():
             # added |double for data
             # added '[0]*' for initial conditions
@@ -2111,15 +2162,16 @@
         """
 
         lines = []
 
         if min(symbol.shape) == 0:
             return lines
 
-        if not self.allow_reinit_fixpar_initcond and function in ['sx0_fixedParameters', 'x0_fixedParameters']:
+        if not self.allow_reinit_fixpar_initcond \
+                and function in ['sx0_fixedParameters', 'x0_fixedParameters']:
             return lines
 
         if function == 'sx0_fixedParameters':
             # here we only want to overwrite values where x0_fixedParameters
             # was applied
             cases = dict()
             for ipar in range(self.model.np()):
@@ -2259,44 +2311,51 @@
         applyTemplate(
             os.path.join(amiciSrcPath, 'model_header.ODE_template.h'),
             os.path.join(self.modelPath, f'{self.modelName}.h'),
             tplData
         )
 
     def _getSymbolNameInitializerList(self, name):
-        """Get SBML name initializer list for vector of names for the given model
-        entity
+        """Get SBML name initializer list for vector of names for the given
+        model entity
 
         Arguments:
             name: any key present in self.model._syms @type str
 
         Returns:
         Template initializer list of names
 
         Raises:
 
         """
         return '\n'.join(
-            [f'"{symbol}",' for symbol in self.model.name(name)]
+            [
+                f'"{strip_pysb(symbol)}",'
+                for symbol in self.model.name(name)
+            ]
         )
 
     def _getSymbolIDInitializerList(self, name):
-        """Get C++ initializer list for vector of names for the given model entity
+        """Get C++ initializer list for vector of names for the given model
+        entity
 
         Arguments:
             name: any key present in self.model._syms @type str
 
         Returns:
         Template initializer list of ids
 
         Raises:
 
         """
         return '\n'.join(
-            [f'"{symbol}",' for symbol in self.model.sym(name)]
+            [
+                f'"{strip_pysb(symbol)}",'
+                for symbol in self.model.sym(name)
+            ]
         )
 
     def _writeCMakeFile(self):
         """Write CMake CMakeLists.txt file for this model.
 
         Arguments:
 
@@ -2483,14 +2542,15 @@
         Returns:
 
         Raises:
 
         """
         self.modelName = modelName
 
+
 def getSymbolicDiagonal(matrix):
     """Get symbolic matrix with diagonal of matrix `matrix`.
 
     Arguments:
         matrix: Matrix from which to return the diagonal
         @type symengine.DenseMatrix
 
@@ -2503,14 +2563,15 @@
     if not matrix.cols == matrix.rows:
         raise Exception('Provided matrix is not square!')
 
     diagonal = [matrix[index,index] for index in range(matrix.cols)]
 
     return sp.Matrix(diagonal)
 
+
 class TemplateAmici(Template):
     """Template format used in AMICI (see string.template for more details).
 
     Attributes:
         delimiter: delimiter that identifies template variables @type str
 
     """
@@ -2537,48 +2598,34 @@
     with open(sourceFile) as filein:
         src = TemplateAmici(filein.read())
     result = src.safe_substitute(templateData)
     with open(targetFile, 'w') as fileout:
         fileout.write(result)
 
 
-def sanitize_basic_sympy(basic):
-    """Strips pysb info from the sympy.Basic object
+def strip_pysb(symbol):
+    """Strips pysb info from a pysb.Component object
 
     Arguments:
-        basic: symbolic expression @type sympy.Basic
+        symbol: symbolic expression @type sympy.Basic
 
     Returns:
-    sanitized sympy.Basic
+    stripped sympy.Basic
 
     Raises:
 
     """
     # strip pysb type and transform into a flat sympy.Basic.
-    # this prevents issues where pysb expressions, observables or
-    # parameters are not recognized as an sp.Symbol with same
-    # symbolic name
-    if pysb and isinstance(basic, pysb.Component):
-        # this is the case where value only consists of a
-        # pysb.Component, here str(value) would print the full
-        # value.__repr__
-        return sp.Symbol(basic.name)
+    # this ensures that the pysb type specific __repr__ is used when converting
+    # to string
+    if pysb and isinstance(symbol, pysb.Component):
+        return sp.Symbol(symbol.name)
     else:
-        # if this expression contains any pysb.Components, we can
-        # safely apply str() to the full expression as str will do
-        # the right thing here
-
-        # ensure that pysb symbols are correctly interpreted as symbols and
-        # not as functions etc
-        local_vars = {
-            fs.name: sp.Symbol(fs.name)
-            for fs in list(basic.expr_free_symbols)
-            if pysb and isinstance(fs, pysb.core.Component)
-        }
-        return sp.sympify(str(basic), locals=local_vars)
+        # in this case we will use sympy specific transform anyways
+        return symbol
 
 
 def get_function_definition(fun, name):
     """Constructs the function definition for a given function
 
     Arguments:
         fun: function name @type str
```

### Comparing `amici-0.9.4/amici.egg-info/PKG-INFO` & `amici-0.9.5/amici.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amici
-Version: 0.9.4
+Version: 0.9.5
 Summary: Advanced multi-language Interface to CVODES and IDAS (%s)
 Home-page: https://github.com/ICB-DCM/AMICI
 Author: Fabian Froehlich, Jan Hasenauer, Daniel Weindl and Paul Stapor
 Author-email: fabian_froehlich@hms.harvard.edu
 License: BSD
 Description: # About AMICI
```

### Comparing `amici-0.9.4/amici.egg-info/SOURCES.txt` & `amici-0.9.5/amici.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 amici/ThirdParty/SuiteSparse/include/amd.h
 amici/ThirdParty/SuiteSparse/include/btf.h
 amici/ThirdParty/SuiteSparse/include/camd.h
 amici/ThirdParty/SuiteSparse/include/colamd.h
 amici/ThirdParty/SuiteSparse/include/klu.h
 amici/ThirdParty/sundials/LICENSE
 amici/ThirdParty/sundials/build/CMakeFiles/feature_tests.c
-amici/ThirdParty/sundials/build/CMakeFiles/3.9.2/CompilerIdC/CMakeCCompilerId.c
+amici/ThirdParty/sundials/build/CMakeFiles/3.12.4/CompilerIdC/CMakeCCompilerId.c
 amici/ThirdParty/sundials/build/KLUTest/ltest.c
 amici/ThirdParty/sundials/build/include/cvodes/cvodes.h
 amici/ThirdParty/sundials/build/include/cvodes/cvodes_band.h
 amici/ThirdParty/sundials/build/include/cvodes/cvodes_bandpre.h
 amici/ThirdParty/sundials/build/include/cvodes/cvodes_bbdpre.h
 amici/ThirdParty/sundials/build/include/cvodes/cvodes_dense.h
 amici/ThirdParty/sundials/build/include/cvodes/cvodes_diag.h
@@ -583,8 +583,9 @@
 amici/swig/model_ode.i
 amici/swig/modelname.template.i
 amici/swig/rdata.i
 amici/swig/solver.i
 amici/swig/solver_cvodes.i
 amici/swig/solver_idas.i
 amici/swig/std_unique_ptr.i
-amici/swig/stdvec2numpy.h
+amici/swig/stdvec2numpy.h
+bin/amici_import_petab.py
```


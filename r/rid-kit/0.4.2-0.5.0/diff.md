# Comparing `tmp/rid-kit-0.4.2.tar.gz` & `tmp/rid-kit-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rid-kit-0.4.2.tar", last modified: Mon Jun 26 06:31:04 2023, max compression
+gzip compressed data, was "rid-kit-0.5.0.tar", last modified: Mon Jun 26 06:36:47 2023, max compression
```

## Comparing `rid-kit-0.4.2.tar` & `rid-kit-0.5.0.tar`

### file list

```diff
@@ -1,230 +1,230 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:31:04.551446 rid-kit-0.4.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:31:04.527445 rid-kit-0.4.2/.eggs/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-26 06:30:57.000000 rid-kit-0.4.2/.eggs/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:31:04.523445 rid-kit-0.4.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:31:04.527445 rid-kit-0.4.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-26 06:30:57.000000 rid-kit-0.4.2/.github/workflows/mirror_gitee.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-26 06:30:57.000000 rid-kit-0.4.2/.github/workflows/pipy_release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-26 06:30:57.000000 rid-kit-0.4.2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-26 06:30:57.000000 rid-kit-0.4.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-26 06:30:57.000000 rid-kit-0.4.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-26 06:30:57.000000 rid-kit-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9415 2023-06-26 06:31:04.551446 rid-kit-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9071 2023-06-26 06:30:57.000000 rid-kit-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:31:04.527445 rid-kit-0.4.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:31:04.527445 rid-kit-0.4.2/docs/.eggs/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-26 06:30:57.000000 rid-kit-0.4.2/docs/.eggs/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-26 06:30:57.000000 rid-kit-0.4.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-26 06:30:57.000000 rid-kit-0.4.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:31:04.527445 rid-kit-0.4.2/docs/pics/
--rw-r--r--   0 runner    (1001) docker     (123)   567861 2023-06-26 06:30:57.000000 rid-kit-0.4.2/docs/pics/mcmc_ala_1cv.png
--rw-r--r--   0 runner    (1001) docker     (123)   738823 2023-06-26 06:30:57.000000 rid-kit-0.4.2/docs/pics/mcmc_ala_2cv.png
--rw-r--r--   0 runner    (1001) docker     (123)   639421 2023-06-26 06:30:57.000000 rid-kit-0.4.2/docs/pics/rid_workflow.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)      146 2023-06-26 06:30:57.000000 rid-kit-0.4.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:31:04.531446 rid-kit-0.4.2/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:31:04.531446 rid-kit-0.4.2/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:30:57.000000 rid-kit-0.4.2/docs/source/_static/.gitkeep
--rwxr-xr-x   0 runner    (1001) docker     (123)     2693 2023-06-26 06:30:57.000000 rid-kit-0.4.2/docs/source/conf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1114 2023-06-26 06:30:57.000000 rid-kit-0.4.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-06-26 06:30:57.000000 rid-kit-0.4.2/docs/source/install.md
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-06-26 06:30:57.000000 rid-kit-0.4.2/docs/source/install_dp.md
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-06-26 06:30:57.000000 rid-kit-0.4.2/docs/source/mcmc_configuration.md
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-06-26 06:30:57.000000 rid-kit-0.4.2/docs/source/prepare_files.md
--rw-r--r--   0 runner    (1001) docker     (123)    16232 2023-06-26 06:30:57.000000 rid-kit-0.4.2/docs/source/rid_configuration.md
--rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-06-26 06:30:57.000000 rid-kit-0.4.2/docs/source/rid_download.md
--rw-r--r--   0 runner    (1001) docker     (123)    13074 2023-06-26 06:30:57.000000 rid-kit-0.4.2/docs/source/rid_machine.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:31:04.531446 rid-kit-0.4.2/docs/source/troubleshooting/
--rwxr-xr-x   0 runner    (1001) docker     (123)      345 2023-06-26 06:30:57.000000 rid-kit-0.4.2/docs/source/troubleshooting/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-26 06:30:57.000000 rid-kit-0.4.2/docs/source/troubleshooting/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-06-26 06:30:57.000000 rid-kit-0.4.2/docs/source/troubleshooting/minikube.md
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-26 06:30:57.000000 rid-kit-0.4.2/docs/source/troubleshooting/submit.md
--rw-r--r--   0 runner    (1001) docker     (123)    16827 2023-06-26 06:30:57.000000 rid-kit-0.4.2/docs/source/tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11213 2023-06-26 06:30:57.000000 rid-kit-0.4.2/docs/source/tutorial.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:31:04.531446 rid-kit-0.4.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:31:04.531446 rid-kit-0.4.2/examples/JSON/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-26 06:30:57.000000 rid-kit-0.4.2/examples/JSON/rid.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     3448 2023-06-26 06:30:57.000000 rid-kit-0.4.2/examples/install-linux-cn.sh
--rw-r--r--   0 runner    (1001) docker     (123)    49439 2023-06-26 06:30:57.000000 rid-kit-0.4.2/examples/quick-start-postgres-stable-cn.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    25032 2023-06-26 06:30:57.000000 rid-kit-0.4.2/examples/tutorial.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:31:04.531446 rid-kit-0.4.2/install/
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-06-26 06:30:57.000000 rid-kit-0.4.2/install/DeePFE.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-26 06:30:57.000000 rid-kit-0.4.2/install/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-06-26 06:30:57.000000 rid-kit-0.4.2/install/gmx_exploration.dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-26 06:30:57.000000 rid-kit-0.4.2/install/gmx_plumed.dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-26 06:30:57.000000 rid-kit-0.4.2/install/gmx_tf.Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-06-26 06:30:57.000000 rid-kit-0.4.2/install/lmp_exploration_dp.dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-26 06:30:57.000000 rid-kit-0.4.2/install/tf_cpu.dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-26 06:30:57.000000 rid-kit-0.4.2/install/tf_gpu.Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-26 06:30:57.000000 rid-kit-0.4.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:31:04.531446 rid-kit-0.4.2/rid/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:31:04.531446 rid-kit-0.4.2/rid/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:31:04.531446 rid-kit-0.4.2/rid/common/gromacs/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/common/gromacs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/common/gromacs/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/common/gromacs/gmx_constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/common/gromacs/mdp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/common/gromacs/trjconv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:31:04.531446 rid-kit-0.4.2/rid/common/lammps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/common/lammps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/common/lammps/command.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/common/lammps/lmp_constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/common/mol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/common/mol_dpdata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:31:04.535446 rid-kit-0.4.2/rid/common/plumed/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/common/plumed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/common/plumed/check_plumed.py
--rw-r--r--   0 runner    (1001) docker     (123)    12420 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/common/plumed/make_plumed.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/common/plumed/plumed_constant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:31:04.535446 rid-kit-0.4.2/rid/common/sampler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/common/sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/common/sampler/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:31:04.535446 rid-kit-0.4.2/rid/common/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/common/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/common/tensorflow/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:31:04.535446 rid-kit-0.4.2/rid/entrypoint/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/entrypoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/entrypoint/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/entrypoint/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/entrypoint/explore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/entrypoint/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/entrypoint/label.py
--rw-r--r--   0 runner    (1001) docker     (123)    16066 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/entrypoint/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/entrypoint/redim.py
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/entrypoint/relabel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/entrypoint/reredim.py
--rw-r--r--   0 runner    (1001) docker     (123)     7629 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/entrypoint/resubmit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/entrypoint/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/entrypoint/submit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/entrypoint/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:31:04.535446 rid-kit-0.4.2/rid/flow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/flow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21137 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/flow/loop.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:31:04.535446 rid-kit-0.4.2/rid/mcmc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/mcmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/mcmc/walker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:31:04.535446 rid-kit-0.4.2/rid/nn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/nn/freeze.py
--rw-r--r--   0 runner    (1001) docker     (123)    27197 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/nn/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/nn/train_net.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:31:04.539446 rid-kit-0.4.2/rid/op/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/op/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/op/adjust_trust_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/op/label_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    11437 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/op/mcmc_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/op/mcmc_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/op/prep_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/op/prep_exploration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/op/prep_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     9938 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/op/prep_rid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/op/prep_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/op/recorder.py
--rw-r--r--   0 runner    (1001) docker     (123)    14599 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/op/run_exploration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/op/run_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/op/run_model_devi.py
--rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/op/run_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/op/run_train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:31:04.539446 rid-kit-0.4.2/rid/select/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/select/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/select/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/select/conf_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/select/model_devi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:31:04.539446 rid-kit-0.4.2/rid/superop/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/superop/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27192 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/superop/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/superop/data.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10888 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/superop/exploration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11594 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/superop/label.py
--rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/superop/mcmc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12664 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/superop/selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:31:04.539446 rid-kit-0.4.2/rid/task/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11234 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/task/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/task/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:31:04.543446 rid-kit-0.4.2/rid/template/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5905 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/template/machine_bohrium.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     5120 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/template/machine_bohrium_k8s.json
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/template/machine_bohrium_k8s_mcmc.json
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/template/machine_local_k8s.json
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/template/machine_slurm_k8s.json
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/template/machine_slurm_k8s_mcmc.json
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/template/machine_slurm_local.json
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/template/machine_slurm_local_mcmc.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     2026 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/template/rid_gmx_dih.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     2031 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/template/rid_gmx_dis.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     2536 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/template/rid_gmx_dp.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     1505 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/template/rid_lmp_dp.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     3013 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/template/rid_lmp_gmx_dp.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      465 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/template/rid_mcmc_cv_dih.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      696 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/template/rid_mcmc_cv_dis.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     1160 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/template/rid_mcmc_path.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:31:04.543446 rid-kit-0.4.2/rid/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12217 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/tools/estimator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:31:04.543446 rid-kit-0.4.2/rid/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/utils/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/utils/format.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-26 06:30:57.000000 rid-kit-0.4.2/rid/utils/set_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:31:04.543446 rid-kit-0.4.2/rid_kit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9415 2023-06-26 06:31:04.000000 rid-kit-0.4.2/rid_kit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-06-26 06:31:04.000000 rid-kit-0.4.2/rid_kit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 06:31:04.000000 rid-kit-0.4.2/rid_kit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-26 06:31:04.000000 rid-kit-0.4.2/rid_kit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-26 06:31:04.000000 rid-kit-0.4.2/rid_kit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-26 06:31:04.000000 rid-kit-0.4.2/rid_kit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 06:31:04.551446 rid-kit-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-26 06:31:00.000000 rid-kit-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:31:04.543446 rid-kit-0.4.2/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)      629 2023-06-26 06:30:57.000000 rid-kit-0.4.2/tests/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:31:04.547446 rid-kit-0.4.2/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:31:04.547446 rid-kit-0.4.2/tests/data/000/
--rw-r--r--   0 runner    (1001) docker     (123)    80843 2023-06-26 06:30:57.000000 rid-kit-0.4.2/tests/data/000/conf.gro
--rw-r--r--   0 runner    (1001) docker     (123)     7156 2023-06-26 06:30:57.000000 rid-kit-0.4.2/tests/data/000/topol.top
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-26 06:30:57.000000 rid-kit-0.4.2/tests/data/centers.out
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-26 06:30:57.000000 rid-kit-0.4.2/tests/data/cls_sel.ndx
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-26 06:30:57.000000 rid-kit-0.4.2/tests/data/cls_sel.out
--rw-r--r--   0 runner    (1001) docker     (123)    80843 2023-06-26 06:30:57.000000 rid-kit-0.4.2/tests/data/conf.gro
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-26 06:30:57.000000 rid-kit-0.4.2/tests/data/conf.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-06-26 06:30:57.000000 rid-kit-0.4.2/tests/data/cv_forces.out
--rwxr-xr-x   0 runner    (1001) docker     (123)        7 2023-06-26 06:30:57.000000 rid-kit-0.4.2/tests/data/kappa.out
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:31:04.547446 rid-kit-0.4.2/tests/data/models/
--rw-r--r--   0 runner    (1001) docker     (123)   536959 2023-06-26 06:30:57.000000 rid-kit-0.4.2/tests/data/models/model_000.pb
--rw-r--r--   0 runner    (1001) docker     (123)   536959 2023-06-26 06:30:57.000000 rid-kit-0.4.2/tests/data/models/model_001.pb
--rw-r--r--   0 runner    (1001) docker     (123)   536959 2023-06-26 06:30:57.000000 rid-kit-0.4.2/tests/data/models/model_002.pb
--rw-r--r--   0 runner    (1001) docker     (123)   536959 2023-06-26 06:30:57.000000 rid-kit-0.4.2/tests/data/models/model_003.pb
--rwxr-xr-x   0 runner    (1001) docker     (123)     4238 2023-06-26 06:30:57.000000 rid-kit-0.4.2/tests/data/plm.out
--rwxr-xr-x   0 runner    (1001) docker     (123)    15119 2023-06-26 06:30:57.000000 rid-kit-0.4.2/tests/data/plm_label.out
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-26 06:30:57.000000 rid-kit-0.4.2/tests/data/plumed.dat
--rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-06-26 06:30:57.000000 rid-kit-0.4.2/tests/data/rid.json
--rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-06-26 06:30:57.000000 rid-kit-0.4.2/tests/data/topol.top
--rw-r--r--   0 runner    (1001) docker     (123)   217160 2023-06-26 06:30:57.000000 rid-kit-0.4.2/tests/data/traj_comp.xtc
--rwxr-xr-x   0 runner    (1001) docker     (123)    12799 2023-06-26 06:30:57.000000 rid-kit-0.4.2/tests/mocked_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:31:04.551446 rid-kit-0.4.2/tests/op/
--rwxr-xr-x   0 runner    (1001) docker     (123)      113 2023-06-26 06:30:57.000000 rid-kit-0.4.2/tests/op/context.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1470 2023-06-26 06:30:57.000000 rid-kit-0.4.2/tests/op/test_adjust_trust_l.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2507 2023-06-26 06:30:57.000000 rid-kit-0.4.2/tests/op/test_prep_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-06-26 06:30:57.000000 rid-kit-0.4.2/tests/op/test_prep_explore.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-06-26 06:30:57.000000 rid-kit-0.4.2/tests/op/test_prep_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-26 06:30:57.000000 rid-kit-0.4.2/tests/op/test_prep_rid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-26 06:30:57.000000 rid-kit-0.4.2/tests/op/test_prep_select.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      874 2023-06-26 06:30:57.000000 rid-kit-0.4.2/tests/op/test_recorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-26 06:30:57.000000 rid-kit-0.4.2/tests/op/test_run_explore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-06-26 06:30:57.000000 rid-kit-0.4.2/tests/op/test_run_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-06-26 06:30:57.000000 rid-kit-0.4.2/tests/op/test_run_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-26 06:30:57.000000 rid-kit-0.4.2/tests/op/test_run_train.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-26 06:30:57.000000 rid-kit-0.4.2/tests/op/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4405 2023-06-26 06:30:57.000000 rid-kit-0.4.2/tests/test_data.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6897 2023-06-26 06:30:57.000000 rid-kit-0.4.2/tests/test_exploration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-06-26 06:30:57.000000 rid-kit-0.4.2/tests/test_init-block.py
--rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-06-26 06:30:57.000000 rid-kit-0.4.2/tests/test_iter-block.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6882 2023-06-26 06:30:57.000000 rid-kit-0.4.2/tests/test_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-06-26 06:30:57.000000 rid-kit-0.4.2/tests/test_select.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:47.547716 rid-kit-0.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:47.523715 rid-kit-0.5.0/.eggs/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-26 06:36:40.000000 rid-kit-0.5.0/.eggs/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:47.519715 rid-kit-0.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:47.523715 rid-kit-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-26 06:36:40.000000 rid-kit-0.5.0/.github/workflows/mirror_gitee.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-26 06:36:40.000000 rid-kit-0.5.0/.github/workflows/pipy_release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-26 06:36:40.000000 rid-kit-0.5.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-26 06:36:40.000000 rid-kit-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-26 06:36:40.000000 rid-kit-0.5.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-26 06:36:40.000000 rid-kit-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9415 2023-06-26 06:36:47.547716 rid-kit-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9071 2023-06-26 06:36:40.000000 rid-kit-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:47.523715 rid-kit-0.5.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:47.523715 rid-kit-0.5.0/docs/.eggs/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-26 06:36:40.000000 rid-kit-0.5.0/docs/.eggs/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-26 06:36:40.000000 rid-kit-0.5.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-26 06:36:40.000000 rid-kit-0.5.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:47.527715 rid-kit-0.5.0/docs/pics/
+-rw-r--r--   0 runner    (1001) docker     (123)   567861 2023-06-26 06:36:40.000000 rid-kit-0.5.0/docs/pics/mcmc_ala_1cv.png
+-rw-r--r--   0 runner    (1001) docker     (123)   738823 2023-06-26 06:36:40.000000 rid-kit-0.5.0/docs/pics/mcmc_ala_2cv.png
+-rw-r--r--   0 runner    (1001) docker     (123)   639421 2023-06-26 06:36:40.000000 rid-kit-0.5.0/docs/pics/rid_workflow.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      146 2023-06-26 06:36:40.000000 rid-kit-0.5.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:47.527715 rid-kit-0.5.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:47.527715 rid-kit-0.5.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:40.000000 rid-kit-0.5.0/docs/source/_static/.gitkeep
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2693 2023-06-26 06:36:40.000000 rid-kit-0.5.0/docs/source/conf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1114 2023-06-26 06:36:40.000000 rid-kit-0.5.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-06-26 06:36:40.000000 rid-kit-0.5.0/docs/source/install.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-06-26 06:36:40.000000 rid-kit-0.5.0/docs/source/install_dp.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-06-26 06:36:40.000000 rid-kit-0.5.0/docs/source/mcmc_configuration.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-06-26 06:36:40.000000 rid-kit-0.5.0/docs/source/prepare_files.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16232 2023-06-26 06:36:40.000000 rid-kit-0.5.0/docs/source/rid_configuration.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-06-26 06:36:40.000000 rid-kit-0.5.0/docs/source/rid_download.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13074 2023-06-26 06:36:40.000000 rid-kit-0.5.0/docs/source/rid_machine.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:47.527715 rid-kit-0.5.0/docs/source/troubleshooting/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      345 2023-06-26 06:36:40.000000 rid-kit-0.5.0/docs/source/troubleshooting/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-26 06:36:40.000000 rid-kit-0.5.0/docs/source/troubleshooting/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-06-26 06:36:40.000000 rid-kit-0.5.0/docs/source/troubleshooting/minikube.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-26 06:36:40.000000 rid-kit-0.5.0/docs/source/troubleshooting/submit.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16827 2023-06-26 06:36:40.000000 rid-kit-0.5.0/docs/source/tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11213 2023-06-26 06:36:40.000000 rid-kit-0.5.0/docs/source/tutorial.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:47.527715 rid-kit-0.5.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:47.531715 rid-kit-0.5.0/examples/JSON/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-26 06:36:40.000000 rid-kit-0.5.0/examples/JSON/rid.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3448 2023-06-26 06:36:40.000000 rid-kit-0.5.0/examples/install-linux-cn.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    49439 2023-06-26 06:36:40.000000 rid-kit-0.5.0/examples/quick-start-postgres-stable-cn.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    25032 2023-06-26 06:36:40.000000 rid-kit-0.5.0/examples/tutorial.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:47.531715 rid-kit-0.5.0/install/
+-rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-06-26 06:36:40.000000 rid-kit-0.5.0/install/DeePFE.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-26 06:36:40.000000 rid-kit-0.5.0/install/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-06-26 06:36:40.000000 rid-kit-0.5.0/install/gmx_exploration.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-26 06:36:40.000000 rid-kit-0.5.0/install/gmx_plumed.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-26 06:36:40.000000 rid-kit-0.5.0/install/gmx_tf.Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-06-26 06:36:40.000000 rid-kit-0.5.0/install/lmp_exploration_dp.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-26 06:36:40.000000 rid-kit-0.5.0/install/tf_cpu.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-26 06:36:40.000000 rid-kit-0.5.0/install/tf_gpu.Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-26 06:36:40.000000 rid-kit-0.5.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:47.531715 rid-kit-0.5.0/rid/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:47.531715 rid-kit-0.5.0/rid/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:47.531715 rid-kit-0.5.0/rid/common/gromacs/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/common/gromacs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/common/gromacs/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/common/gromacs/gmx_constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/common/gromacs/mdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/common/gromacs/trjconv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:47.531715 rid-kit-0.5.0/rid/common/lammps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/common/lammps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/common/lammps/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/common/lammps/lmp_constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/common/mol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/common/mol_dpdata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:47.531715 rid-kit-0.5.0/rid/common/plumed/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/common/plumed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/common/plumed/check_plumed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12420 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/common/plumed/make_plumed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/common/plumed/plumed_constant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:47.531715 rid-kit-0.5.0/rid/common/sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/common/sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/common/sampler/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:47.531715 rid-kit-0.5.0/rid/common/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/common/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/common/tensorflow/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:47.535715 rid-kit-0.5.0/rid/entrypoint/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/entrypoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/entrypoint/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/entrypoint/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/entrypoint/explore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/entrypoint/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/entrypoint/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16066 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/entrypoint/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/entrypoint/redim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/entrypoint/relabel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/entrypoint/reredim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7629 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/entrypoint/resubmit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/entrypoint/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/entrypoint/submit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/entrypoint/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:47.535715 rid-kit-0.5.0/rid/flow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/flow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21137 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/flow/loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:47.535715 rid-kit-0.5.0/rid/mcmc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/mcmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/mcmc/walker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:47.535715 rid-kit-0.5.0/rid/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/nn/freeze.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27197 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/nn/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/nn/train_net.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:47.539715 rid-kit-0.5.0/rid/op/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/op/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/op/adjust_trust_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/op/label_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11437 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/op/mcmc_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/op/mcmc_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/op/prep_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/op/prep_exploration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/op/prep_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9938 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/op/prep_rid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/op/prep_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/op/recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14599 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/op/run_exploration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/op/run_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/op/run_model_devi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/op/run_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/op/run_train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:47.539715 rid-kit-0.5.0/rid/select/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/select/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/select/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/select/conf_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/select/model_devi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:47.539715 rid-kit-0.5.0/rid/superop/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/superop/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27192 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/superop/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/superop/data.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10888 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/superop/exploration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11594 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/superop/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/superop/mcmc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12664 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/superop/selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:47.539715 rid-kit-0.5.0/rid/task/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11234 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/task/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/task/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:47.539715 rid-kit-0.5.0/rid/template/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5905 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/template/machine_bohrium.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5120 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/template/machine_bohrium_k8s.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/template/machine_bohrium_k8s_mcmc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/template/machine_local_k8s.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/template/machine_slurm_k8s.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/template/machine_slurm_k8s_mcmc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/template/machine_slurm_local.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/template/machine_slurm_local_mcmc.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2026 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/template/rid_gmx_dih.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2031 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/template/rid_gmx_dis.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2536 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/template/rid_gmx_dp.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1505 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/template/rid_lmp_dp.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3013 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/template/rid_lmp_gmx_dp.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      465 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/template/rid_mcmc_cv_dih.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      696 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/template/rid_mcmc_cv_dis.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1160 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/template/rid_mcmc_path.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:47.539715 rid-kit-0.5.0/rid/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12217 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/tools/estimator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:47.543715 rid-kit-0.5.0/rid/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/utils/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/utils/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-26 06:36:40.000000 rid-kit-0.5.0/rid/utils/set_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:47.543715 rid-kit-0.5.0/rid_kit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9415 2023-06-26 06:36:47.000000 rid-kit-0.5.0/rid_kit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-06-26 06:36:47.000000 rid-kit-0.5.0/rid_kit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 06:36:47.000000 rid-kit-0.5.0/rid_kit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-26 06:36:47.000000 rid-kit-0.5.0/rid_kit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-26 06:36:47.000000 rid-kit-0.5.0/rid_kit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-26 06:36:47.000000 rid-kit-0.5.0/rid_kit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 06:36:47.547716 rid-kit-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-26 06:36:43.000000 rid-kit-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:47.543715 rid-kit-0.5.0/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      629 2023-06-26 06:36:40.000000 rid-kit-0.5.0/tests/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:47.543715 rid-kit-0.5.0/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:47.543715 rid-kit-0.5.0/tests/data/000/
+-rw-r--r--   0 runner    (1001) docker     (123)    80843 2023-06-26 06:36:40.000000 rid-kit-0.5.0/tests/data/000/conf.gro
+-rw-r--r--   0 runner    (1001) docker     (123)     7156 2023-06-26 06:36:40.000000 rid-kit-0.5.0/tests/data/000/topol.top
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-26 06:36:40.000000 rid-kit-0.5.0/tests/data/centers.out
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-26 06:36:40.000000 rid-kit-0.5.0/tests/data/cls_sel.ndx
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-26 06:36:40.000000 rid-kit-0.5.0/tests/data/cls_sel.out
+-rw-r--r--   0 runner    (1001) docker     (123)    80843 2023-06-26 06:36:40.000000 rid-kit-0.5.0/tests/data/conf.gro
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-26 06:36:40.000000 rid-kit-0.5.0/tests/data/conf.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-06-26 06:36:40.000000 rid-kit-0.5.0/tests/data/cv_forces.out
+-rwxr-xr-x   0 runner    (1001) docker     (123)        7 2023-06-26 06:36:40.000000 rid-kit-0.5.0/tests/data/kappa.out
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:47.547716 rid-kit-0.5.0/tests/data/models/
+-rw-r--r--   0 runner    (1001) docker     (123)   536959 2023-06-26 06:36:40.000000 rid-kit-0.5.0/tests/data/models/model_000.pb
+-rw-r--r--   0 runner    (1001) docker     (123)   536959 2023-06-26 06:36:40.000000 rid-kit-0.5.0/tests/data/models/model_001.pb
+-rw-r--r--   0 runner    (1001) docker     (123)   536959 2023-06-26 06:36:40.000000 rid-kit-0.5.0/tests/data/models/model_002.pb
+-rw-r--r--   0 runner    (1001) docker     (123)   536959 2023-06-26 06:36:40.000000 rid-kit-0.5.0/tests/data/models/model_003.pb
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4238 2023-06-26 06:36:40.000000 rid-kit-0.5.0/tests/data/plm.out
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15119 2023-06-26 06:36:40.000000 rid-kit-0.5.0/tests/data/plm_label.out
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-26 06:36:40.000000 rid-kit-0.5.0/tests/data/plumed.dat
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-06-26 06:36:40.000000 rid-kit-0.5.0/tests/data/rid.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-06-26 06:36:40.000000 rid-kit-0.5.0/tests/data/topol.top
+-rw-r--r--   0 runner    (1001) docker     (123)   217160 2023-06-26 06:36:40.000000 rid-kit-0.5.0/tests/data/traj_comp.xtc
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12799 2023-06-26 06:36:40.000000 rid-kit-0.5.0/tests/mocked_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:36:47.547716 rid-kit-0.5.0/tests/op/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      113 2023-06-26 06:36:40.000000 rid-kit-0.5.0/tests/op/context.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1470 2023-06-26 06:36:40.000000 rid-kit-0.5.0/tests/op/test_adjust_trust_l.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2507 2023-06-26 06:36:40.000000 rid-kit-0.5.0/tests/op/test_prep_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-06-26 06:36:40.000000 rid-kit-0.5.0/tests/op/test_prep_explore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-06-26 06:36:40.000000 rid-kit-0.5.0/tests/op/test_prep_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-26 06:36:40.000000 rid-kit-0.5.0/tests/op/test_prep_rid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-26 06:36:40.000000 rid-kit-0.5.0/tests/op/test_prep_select.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      874 2023-06-26 06:36:40.000000 rid-kit-0.5.0/tests/op/test_recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-26 06:36:40.000000 rid-kit-0.5.0/tests/op/test_run_explore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-06-26 06:36:40.000000 rid-kit-0.5.0/tests/op/test_run_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-06-26 06:36:40.000000 rid-kit-0.5.0/tests/op/test_run_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-26 06:36:40.000000 rid-kit-0.5.0/tests/op/test_run_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-26 06:36:40.000000 rid-kit-0.5.0/tests/op/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4405 2023-06-26 06:36:40.000000 rid-kit-0.5.0/tests/test_data.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6897 2023-06-26 06:36:40.000000 rid-kit-0.5.0/tests/test_exploration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-06-26 06:36:40.000000 rid-kit-0.5.0/tests/test_init-block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-06-26 06:36:40.000000 rid-kit-0.5.0/tests/test_iter-block.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6882 2023-06-26 06:36:40.000000 rid-kit-0.5.0/tests/test_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-06-26 06:36:40.000000 rid-kit-0.5.0/tests/test_select.py
```

### Comparing `rid-kit-0.4.2/.github/workflows/pipy_release.yml` & `rid-kit-0.5.0/.github/workflows/pipy_release.yml`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/.readthedocs.yaml` & `rid-kit-0.5.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/LICENSE` & `rid-kit-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/PKG-INFO` & `rid-kit-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rid-kit
-Version: 0.4.2
+Version: 0.5.0
 Summary: RiD package for enhanced sampling
 Home-page: https://github.com/deepmodeling/rid-kit
 Author: Yanze Wang, Jiahao Fan
 Author-email: yanze039@mit.edu,jiahaofan@pku.edu.cn
 License: UNKNOWN
 Keywords: enhanced sampling reinforced dynamics RiD
 Platform: UNKNOWN
```

### Comparing `rid-kit-0.4.2/README.md` & `rid-kit-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/docs/Makefile` & `rid-kit-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/docs/make.bat` & `rid-kit-0.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/docs/pics/mcmc_ala_1cv.png` & `rid-kit-0.5.0/docs/pics/mcmc_ala_1cv.png`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/docs/pics/mcmc_ala_2cv.png` & `rid-kit-0.5.0/docs/pics/mcmc_ala_2cv.png`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/docs/pics/rid_workflow.jpg` & `rid-kit-0.5.0/docs/pics/rid_workflow.jpg`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/docs/source/conf.py` & `rid-kit-0.5.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/docs/source/index.rst` & `rid-kit-0.5.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/docs/source/install.md` & `rid-kit-0.5.0/docs/source/install.md`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/docs/source/install_dp.md` & `rid-kit-0.5.0/docs/source/install_dp.md`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/docs/source/mcmc_configuration.md` & `rid-kit-0.5.0/docs/source/mcmc_configuration.md`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/docs/source/prepare_files.md` & `rid-kit-0.5.0/docs/source/prepare_files.md`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/docs/source/rid_configuration.md` & `rid-kit-0.5.0/docs/source/rid_configuration.md`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/docs/source/rid_download.md` & `rid-kit-0.5.0/docs/source/rid_download.md`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/docs/source/rid_machine.md` & `rid-kit-0.5.0/docs/source/rid_machine.md`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/docs/source/troubleshooting/installation.md` & `rid-kit-0.5.0/docs/source/troubleshooting/installation.md`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/docs/source/troubleshooting/minikube.md` & `rid-kit-0.5.0/docs/source/troubleshooting/minikube.md`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/docs/source/troubleshooting/submit.md` & `rid-kit-0.5.0/docs/source/troubleshooting/submit.md`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/docs/source/tutorial.ipynb` & `rid-kit-0.5.0/docs/source/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/docs/source/tutorial.md` & `rid-kit-0.5.0/docs/source/tutorial.md`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/examples/install-linux-cn.sh` & `rid-kit-0.5.0/examples/install-linux-cn.sh`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/examples/quick-start-postgres-stable-cn.yaml` & `rid-kit-0.5.0/examples/quick-start-postgres-stable-cn.yaml`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/examples/tutorial.ipynb` & `rid-kit-0.5.0/examples/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/install/DeePFE.cpp` & `rid-kit-0.5.0/install/DeePFE.cpp`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/install/gmx_exploration.dockerfile` & `rid-kit-0.5.0/install/gmx_exploration.dockerfile`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/install/gmx_plumed.dockerfile` & `rid-kit-0.5.0/install/gmx_plumed.dockerfile`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/install/gmx_tf.Dockerfile` & `rid-kit-0.5.0/install/gmx_tf.Dockerfile`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/install/lmp_exploration_dp.dockerfile` & `rid-kit-0.5.0/install/lmp_exploration_dp.dockerfile`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/common/gromacs/command.py` & `rid-kit-0.5.0/rid/common/gromacs/command.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/common/gromacs/gmx_constant.py` & `rid-kit-0.5.0/rid/common/gromacs/gmx_constant.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/common/gromacs/mdp.py` & `rid-kit-0.5.0/rid/common/gromacs/mdp.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/common/gromacs/trjconv.py` & `rid-kit-0.5.0/rid/common/gromacs/trjconv.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/common/mol.py` & `rid-kit-0.5.0/rid/common/mol.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/common/mol_dpdata.py` & `rid-kit-0.5.0/rid/common/mol_dpdata.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/common/plumed/check_plumed.py` & `rid-kit-0.5.0/rid/common/plumed/check_plumed.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/common/plumed/make_plumed.py` & `rid-kit-0.5.0/rid/common/plumed/make_plumed.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/common/plumed/plumed_constant.py` & `rid-kit-0.5.0/rid/common/plumed/plumed_constant.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/common/sampler/command.py` & `rid-kit-0.5.0/rid/common/sampler/command.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/common/tensorflow/graph.py` & `rid-kit-0.5.0/rid/common/tensorflow/graph.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/constants.py` & `rid-kit-0.5.0/rid/constants.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/entrypoint/cli.py` & `rid-kit-0.5.0/rid/entrypoint/cli.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/entrypoint/download.py` & `rid-kit-0.5.0/rid/entrypoint/download.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/entrypoint/explore.py` & `rid-kit-0.5.0/rid/entrypoint/explore.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/entrypoint/info.py` & `rid-kit-0.5.0/rid/entrypoint/info.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/entrypoint/label.py` & `rid-kit-0.5.0/rid/entrypoint/label.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/entrypoint/main.py` & `rid-kit-0.5.0/rid/entrypoint/main.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/entrypoint/redim.py` & `rid-kit-0.5.0/rid/entrypoint/redim.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/entrypoint/relabel.py` & `rid-kit-0.5.0/rid/entrypoint/relabel.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/entrypoint/reredim.py` & `rid-kit-0.5.0/rid/entrypoint/reredim.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/entrypoint/resubmit.py` & `rid-kit-0.5.0/rid/entrypoint/resubmit.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/entrypoint/server.py` & `rid-kit-0.5.0/rid/entrypoint/server.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/entrypoint/submit.py` & `rid-kit-0.5.0/rid/entrypoint/submit.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/entrypoint/train.py` & `rid-kit-0.5.0/rid/entrypoint/train.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/flow/loop.py` & `rid-kit-0.5.0/rid/flow/loop.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/mcmc/walker.py` & `rid-kit-0.5.0/rid/mcmc/walker.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/nn/freeze.py` & `rid-kit-0.5.0/rid/nn/freeze.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/nn/model.py` & `rid-kit-0.5.0/rid/nn/model.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/nn/train_net.py` & `rid-kit-0.5.0/rid/nn/train_net.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/op/adjust_trust_level.py` & `rid-kit-0.5.0/rid/op/adjust_trust_level.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/op/label_stats.py` & `rid-kit-0.5.0/rid/op/label_stats.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/op/mcmc_plot.py` & `rid-kit-0.5.0/rid/op/mcmc_plot.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/op/mcmc_run.py` & `rid-kit-0.5.0/rid/op/mcmc_run.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/op/prep_data.py` & `rid-kit-0.5.0/rid/op/prep_data.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/op/prep_exploration.py` & `rid-kit-0.5.0/rid/op/prep_exploration.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/op/prep_label.py` & `rid-kit-0.5.0/rid/op/prep_label.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/op/prep_rid.py` & `rid-kit-0.5.0/rid/op/prep_rid.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/op/prep_select.py` & `rid-kit-0.5.0/rid/op/prep_select.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/op/recorder.py` & `rid-kit-0.5.0/rid/op/recorder.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/op/run_exploration.py` & `rid-kit-0.5.0/rid/op/run_exploration.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/op/run_label.py` & `rid-kit-0.5.0/rid/op/run_label.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/op/run_model_devi.py` & `rid-kit-0.5.0/rid/op/run_model_devi.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/op/run_select.py` & `rid-kit-0.5.0/rid/op/run_select.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/op/run_train.py` & `rid-kit-0.5.0/rid/op/run_train.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/select/cluster.py` & `rid-kit-0.5.0/rid/select/cluster.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/select/conf_select.py` & `rid-kit-0.5.0/rid/select/conf_select.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/select/model_devi.py` & `rid-kit-0.5.0/rid/select/model_devi.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/superop/blocks.py` & `rid-kit-0.5.0/rid/superop/blocks.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/superop/data.py` & `rid-kit-0.5.0/rid/superop/data.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/superop/exploration.py` & `rid-kit-0.5.0/rid/superop/exploration.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/superop/label.py` & `rid-kit-0.5.0/rid/superop/label.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/superop/mcmc.py` & `rid-kit-0.5.0/rid/superop/mcmc.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/superop/selector.py` & `rid-kit-0.5.0/rid/superop/selector.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/task/builder.py` & `rid-kit-0.5.0/rid/task/builder.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/task/task.py` & `rid-kit-0.5.0/rid/task/task.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/template/machine_bohrium.json` & `rid-kit-0.5.0/rid/template/machine_bohrium.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/template/machine_bohrium_k8s.json` & `rid-kit-0.5.0/rid/template/machine_bohrium_k8s.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/template/machine_bohrium_k8s_mcmc.json` & `rid-kit-0.5.0/rid/template/machine_bohrium_k8s_mcmc.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/template/machine_local_k8s.json` & `rid-kit-0.5.0/rid/template/machine_local_k8s.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/template/machine_slurm_k8s.json` & `rid-kit-0.5.0/rid/template/machine_slurm_k8s.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/template/machine_slurm_k8s_mcmc.json` & `rid-kit-0.5.0/rid/template/machine_slurm_k8s_mcmc.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/template/machine_slurm_local.json` & `rid-kit-0.5.0/rid/template/machine_slurm_local.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/template/machine_slurm_local_mcmc.json` & `rid-kit-0.5.0/rid/template/machine_slurm_local_mcmc.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/template/rid_gmx_dih.json` & `rid-kit-0.5.0/rid/template/rid_gmx_dih.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/template/rid_gmx_dis.json` & `rid-kit-0.5.0/rid/template/rid_gmx_dis.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/template/rid_gmx_dp.json` & `rid-kit-0.5.0/rid/template/rid_gmx_dp.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/template/rid_lmp_dp.json` & `rid-kit-0.5.0/rid/template/rid_lmp_dp.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/template/rid_lmp_gmx_dp.json` & `rid-kit-0.5.0/rid/template/rid_lmp_gmx_dp.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/template/rid_mcmc_cv_dis.json` & `rid-kit-0.5.0/rid/template/rid_mcmc_cv_dis.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/template/rid_mcmc_path.json` & `rid-kit-0.5.0/rid/template/rid_mcmc_path.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/tools/estimator.py` & `rid-kit-0.5.0/rid/tools/estimator.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/utils/command.py` & `rid-kit-0.5.0/rid/utils/command.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/utils/files.py` & `rid-kit-0.5.0/rid/utils/files.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/utils/path.py` & `rid-kit-0.5.0/rid/utils/path.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid/utils/set_config.py` & `rid-kit-0.5.0/rid/utils/set_config.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/rid_kit.egg-info/PKG-INFO` & `rid-kit-0.5.0/rid_kit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rid-kit
-Version: 0.4.2
+Version: 0.5.0
 Summary: RiD package for enhanced sampling
 Home-page: https://github.com/deepmodeling/rid-kit
 Author: Yanze Wang, Jiahao Fan
 Author-email: yanze039@mit.edu,jiahaofan@pku.edu.cn
 License: UNKNOWN
 Keywords: enhanced sampling reinforced dynamics RiD
 Platform: UNKNOWN
```

### Comparing `rid-kit-0.4.2/rid_kit.egg-info/SOURCES.txt` & `rid-kit-0.5.0/rid_kit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/setup.py` & `rid-kit-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 readme_file = Path(__file__).parent / "README.md"
 readme = readme_file.read_text(encoding="utf-8")
 
 setuptools.setup(
     name='rid-kit',
     author="Yanze Wang, Jiahao Fan",
     author_email="yanze039@mit.edu,jiahaofan@pku.edu.cn",
-    version='0.4.2',
+    version='0.5.0',
     description="RiD package for enhanced sampling",
     setup_requires=['setuptools_scm'],
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/deepmodeling/rid-kit",
     python_requires=">=3.6",
     packages=[
```

### Comparing `rid-kit-0.4.2/tests/context.py` & `rid-kit-0.5.0/tests/context.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/tests/data/000/conf.gro` & `rid-kit-0.5.0/tests/data/000/conf.gro`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/tests/data/000/topol.top` & `rid-kit-0.5.0/tests/data/000/topol.top`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/tests/data/conf.gro` & `rid-kit-0.5.0/tests/data/conf.gro`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/tests/data/models/model_000.pb` & `rid-kit-0.5.0/tests/data/models/model_000.pb`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/tests/data/models/model_001.pb` & `rid-kit-0.5.0/tests/data/models/model_001.pb`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/tests/data/models/model_002.pb` & `rid-kit-0.5.0/tests/data/models/model_002.pb`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/tests/data/models/model_003.pb` & `rid-kit-0.5.0/tests/data/models/model_003.pb`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/tests/data/plm.out` & `rid-kit-0.5.0/tests/data/plm.out`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/tests/data/plm_label.out` & `rid-kit-0.5.0/tests/data/plm_label.out`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/tests/data/rid.json` & `rid-kit-0.5.0/tests/data/rid.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/tests/data/topol.top` & `rid-kit-0.5.0/tests/data/topol.top`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/tests/data/traj_comp.xtc` & `rid-kit-0.5.0/tests/data/traj_comp.xtc`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/tests/mocked_ops.py` & `rid-kit-0.5.0/tests/mocked_ops.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/tests/op/test_adjust_trust_l.py` & `rid-kit-0.5.0/tests/op/test_adjust_trust_l.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/tests/op/test_prep_data.py` & `rid-kit-0.5.0/tests/op/test_prep_data.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/tests/op/test_prep_explore.py` & `rid-kit-0.5.0/tests/op/test_prep_explore.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/tests/op/test_prep_label.py` & `rid-kit-0.5.0/tests/op/test_prep_label.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/tests/op/test_prep_rid.py` & `rid-kit-0.5.0/tests/op/test_prep_rid.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/tests/op/test_prep_select.py` & `rid-kit-0.5.0/tests/op/test_prep_select.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/tests/op/test_recorder.py` & `rid-kit-0.5.0/tests/op/test_recorder.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/tests/op/test_run_explore.py` & `rid-kit-0.5.0/tests/op/test_run_explore.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/tests/op/test_run_label.py` & `rid-kit-0.5.0/tests/op/test_run_label.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/tests/op/test_run_select.py` & `rid-kit-0.5.0/tests/op/test_run_select.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/tests/op/test_run_train.py` & `rid-kit-0.5.0/tests/op/test_run_train.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/tests/op/utils.py` & `rid-kit-0.5.0/tests/op/utils.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/tests/test_data.py` & `rid-kit-0.5.0/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/tests/test_exploration.py` & `rid-kit-0.5.0/tests/test_exploration.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/tests/test_init-block.py` & `rid-kit-0.5.0/tests/test_init-block.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/tests/test_iter-block.py` & `rid-kit-0.5.0/tests/test_iter-block.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/tests/test_label.py` & `rid-kit-0.5.0/tests/test_label.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.4.2/tests/test_select.py` & `rid-kit-0.5.0/tests/test_select.py`

 * *Files identical despite different names*


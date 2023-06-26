# Comparing `tmp/egobox-0.8.2.tar.gz` & `tmp/egobox-0.9.0.tar.gz`

## Comparing `egobox-0.8.2.tar` & `egobox-0.9.0.tar`

### file list

```diff
@@ -1,77 +1,80 @@
--rw-r--r--   0        0        0     1746 1970-01-01 00:00:00.000000 egobox-0.8.2/local_dependencies/egobox-ego/Cargo.toml
--rw-r--r--   0        0        0     1046 2022-10-05 08:24:51.000000 egobox-0.8.2/local_dependencies/egobox-ego/README.md
--rw-r--r--   0        0        0      992 2023-03-06 15:20:45.000000 egobox-0.8.2/local_dependencies/egobox-ego/examples/ackley.rs
--rw-r--r--   0        0        0     8068 2023-03-27 15:22:25.000000 egobox-0.8.2/local_dependencies/egobox-ego/examples/mopta08.rs
--rw-r--r--   0        0        0      840 2023-03-06 15:20:45.000000 egobox-0.8.2/local_dependencies/egobox-ego/examples/rosenbrock.rs
--rw-r--r--   0        0        0    22747 2023-03-28 15:47:43.000000 egobox-0.8.2/local_dependencies/egobox-ego/src/egor.rs
--rw-r--r--   0        0        0    52191 2023-03-29 09:38:32.000000 egobox-0.8.2/local_dependencies/egobox-ego/src/egor_solver.rs
--rw-r--r--   0        0        0    29196 2023-03-29 09:38:32.000000 egobox-0.8.2/local_dependencies/egobox-ego/src/egor_state.rs
--rw-r--r--   0        0        0     1423 2023-01-11 09:58:59.000000 egobox-0.8.2/local_dependencies/egobox-ego/src/errors.rs
--rw-r--r--   0        0        0     6075 2023-03-03 16:02:22.000000 egobox-0.8.2/local_dependencies/egobox-ego/src/lhs_optimizer.rs
--rw-r--r--   0        0        0     4547 2023-03-09 17:13:31.000000 egobox-0.8.2/local_dependencies/egobox-ego/src/lib.rs
--rw-r--r--   0        0        0    26236 2023-03-09 17:13:31.000000 egobox-0.8.2/local_dependencies/egobox-ego/src/mixint.rs
--rw-r--r--   0        0        0     7718 2022-04-13 12:11:37.000000 egobox-0.8.2/local_dependencies/egobox-ego/src/sort_axis.rs
--rw-r--r--   0        0        0     5093 2023-03-27 15:14:32.000000 egobox-0.8.2/local_dependencies/egobox-ego/src/types.rs
--rw-r--r--   0        0        0    11061 2023-03-03 16:02:22.000000 egobox-0.8.2/local_dependencies/egobox-ego/src/utils.rs
--rw-r--r--   0        0        0     1657 1970-01-01 00:00:00.000000 egobox-0.8.2/local_dependencies/egobox-moe/Cargo.toml
--rw-r--r--   0        0        0     1036 2022-10-05 08:24:51.000000 egobox-0.8.2/local_dependencies/egobox-moe/README.md
--rw-r--r--   0        0        0     1431 2022-12-14 13:14:49.000000 egobox-0.8.2/local_dependencies/egobox-moe/benches/bench_find_nb_clusters.rs
--rw-r--r--   0        0        0     1506 2022-08-18 12:20:53.000000 egobox-0.8.2/local_dependencies/egobox-moe/examples/clustering.rs
--rw-r--r--   0        0        0     1564 2023-01-30 08:37:24.000000 egobox-0.8.2/local_dependencies/egobox-moe/examples/moe_norm1.rs
--rw-r--r--   0        0        0     1260 2022-08-18 12:20:53.000000 egobox-0.8.2/local_dependencies/egobox-moe/examples/norm1.rs
--rw-r--r--   0        0        0    12658 2022-04-13 12:11:37.000000 egobox-0.8.2/local_dependencies/egobox-moe/examples/norm1_D2_200.csv
--rw-r--r--   0        0        0    46305 2023-03-27 15:22:25.000000 egobox-0.8.2/local_dependencies/egobox-moe/src/algorithm.rs
--rw-r--r--   0        0        0    17244 2023-02-11 16:49:33.000000 egobox-0.8.2/local_dependencies/egobox-moe/src/clustering.rs
--rw-r--r--   0        0        0     1574 2023-02-11 16:49:34.000000 egobox-0.8.2/local_dependencies/egobox-moe/src/errors.rs
--rw-r--r--   0        0        0     4569 2023-03-27 15:22:25.000000 egobox-0.8.2/local_dependencies/egobox-moe/src/expertise_macros.rs
--rw-r--r--   0        0        0    14971 2023-01-30 08:37:24.000000 egobox-0.8.2/local_dependencies/egobox-moe/src/gaussian_mixture.rs
--rw-r--r--   0        0        0     4070 2022-12-20 08:24:26.000000 egobox-0.8.2/local_dependencies/egobox-moe/src/lib.rs
--rw-r--r--   0        0        0    11012 2023-01-30 08:37:24.000000 egobox-0.8.2/local_dependencies/egobox-moe/src/parameters.rs
--rw-r--r--   0        0        0     8879 2023-02-08 08:11:35.000000 egobox-0.8.2/local_dependencies/egobox-moe/src/surrogates.rs
--rw-r--r--   0        0        0     1328 1970-01-01 00:00:00.000000 egobox-0.8.2/local_dependencies/egobox-gp/Cargo.toml
--rw-r--r--   0        0        0     1090 2022-10-05 08:24:51.000000 egobox-0.8.2/local_dependencies/egobox-gp/README.md
--rw-r--r--   0        0        0     2796 2023-01-30 08:37:24.000000 egobox-0.8.2/local_dependencies/egobox-gp/benches/gp.rs
--rw-r--r--   0        0        0     1206 2022-04-13 12:11:37.000000 egobox-0.8.2/local_dependencies/egobox-gp/examples/kriging.rs
--rw-r--r--   0        0        0    53115 2023-03-06 15:20:45.000000 egobox-0.8.2/local_dependencies/egobox-gp/src/algorithm.rs
--rw-r--r--   0        0        0    21783 2022-12-13 14:13:12.000000 egobox-0.8.2/local_dependencies/egobox-gp/src/correlation_models.rs
--rw-r--r--   0        0        0     1035 2022-08-18 12:20:53.000000 egobox-0.8.2/local_dependencies/egobox-gp/src/errors.rs
--rw-r--r--   0        0        0     4239 2022-10-05 08:24:51.000000 egobox-0.8.2/local_dependencies/egobox-gp/src/lib.rs
--rw-r--r--   0        0        0     7471 2023-01-30 08:37:24.000000 egobox-0.8.2/local_dependencies/egobox-gp/src/mean_models.rs
--rw-r--r--   0        0        0     4576 2023-03-06 15:20:45.000000 egobox-0.8.2/local_dependencies/egobox-gp/src/parameters.rs
--rw-r--r--   0        0        0     7096 2022-12-05 16:09:19.000000 egobox-0.8.2/local_dependencies/egobox-gp/src/utils.rs
--rw-r--r--   0        0        0      851 1970-01-01 00:00:00.000000 egobox-0.8.2/local_dependencies/egobox-doe/Cargo.toml
--rw-r--r--   0        0        0      970 2022-04-13 12:11:37.000000 egobox-0.8.2/local_dependencies/egobox-doe/README.md
--rw-r--r--   0        0        0      585 2023-01-30 08:37:24.000000 egobox-0.8.2/local_dependencies/egobox-doe/benches/lhs.rs
--rw-r--r--   0        0        0      841 2023-01-30 08:37:24.000000 egobox-0.8.2/local_dependencies/egobox-doe/examples/samplings.rs
--rw-r--r--   0        0        0     3416 2022-12-28 17:44:23.000000 egobox-0.8.2/local_dependencies/egobox-doe/src/full_factorial.rs
--rw-r--r--   0        0        0    14760 2023-03-03 16:02:22.000000 egobox-0.8.2/local_dependencies/egobox-doe/src/lhs.rs
--rw-r--r--   0        0        0     1701 2022-12-14 13:14:49.000000 egobox-0.8.2/local_dependencies/egobox-doe/src/lib.rs
--rw-r--r--   0        0        0     3350 2022-12-28 17:44:23.000000 egobox-0.8.2/local_dependencies/egobox-doe/src/random.rs
--rw-r--r--   0        0        0     1743 2022-09-08 08:39:18.000000 egobox-0.8.2/local_dependencies/egobox-doe/src/traits.rs
--rw-r--r--   0        0        0     2247 2022-04-13 12:11:37.000000 egobox-0.8.2/local_dependencies/egobox-doe/src/utils.rs
--rw-r--r--   0        0        0     1627 1970-01-01 00:00:00.000000 egobox-0.8.2/Cargo.toml
--rw-r--r--   0        0        0      586 2023-02-07 14:17:13.000000 egobox-0.8.2/.gitignore
--rw-r--r--   0        0        0     5332 2023-03-28 15:47:43.000000 egobox-0.8.2/CHANGELOG.md
--rw-r--r--   0        0        0     2177 2022-10-05 08:24:51.000000 egobox-0.8.2/CONTRIBUTING.md
--rw-r--r--   0        0        0      410 2022-08-18 12:20:53.000000 egobox-0.8.2/Dockerfile
--rw-r--r--   0        0        0    11558 2022-04-13 12:11:37.000000 egobox-0.8.2/LICENSE
--rw-r--r--   0        0        0     6361 2023-03-28 16:12:28.000000 egobox-0.8.2/README.md
--rw-r--r--   0        0        0    37898 2023-03-09 07:55:59.000000 egobox-0.8.2/doc/Egor_Tutorial.ipynb
--rw-r--r--   0        0        0   249207 2023-03-09 07:55:59.000000 egobox-0.8.2/doc/Gpx_MaunaLoaCO2.ipynb
--rw-r--r--   0        0        0    49162 2023-03-09 07:55:59.000000 egobox-0.8.2/doc/Gpx_Tutorial.ipynb
--rw-r--r--   0        0        0   117618 2022-10-10 20:47:14.000000 egobox-0.8.2/joss/egobox_architecture.png
--rw-r--r--   0        0        0     4293 2022-10-10 20:47:14.000000 egobox-0.8.2/joss/paper.bib
--rw-r--r--   0        0        0     5424 2022-10-10 20:47:14.000000 egobox-0.8.2/joss/paper.md
--rw-r--r--   0        0        0      997 2023-03-29 09:38:32.000000 egobox-0.8.2/pyproject.toml
--rw-r--r--   0        0        0       23 2022-04-13 12:11:37.000000 egobox-0.8.2/python/egobox/__init__.py
--rw-r--r--   0        0        0      791 2022-10-10 20:47:14.000000 egobox-0.8.2/python/egobox/examples/kriging.py
--rw-r--r--   0        0        0     1660 2023-03-09 07:55:59.000000 egobox-0.8.2/python/egobox/examples/optim_g24.py
--rw-r--r--   0        0        0     5812 2023-03-09 08:58:12.000000 egobox-0.8.2/python/egobox/tests/test_egor.py
--rw-r--r--   0        0        0     1841 2022-10-10 20:47:14.000000 egobox-0.8.2/python/egobox/tests/test_gpmix.py
--rw-r--r--   0        0        0      776 2023-03-29 09:38:32.000000 egobox-0.8.2/python/egobox/tests/test_mixintegor.py
--rw-r--r--   0        0        0      980 2023-03-09 17:13:31.000000 egobox-0.8.2/python/egobox/tests/test_utils.py
--rw-r--r--   0        0        0    14468 2023-03-28 13:42:02.000000 egobox-0.8.2/src/egor.rs
--rw-r--r--   0        0        0     7660 2022-12-14 13:14:49.000000 egobox-0.8.2/src/gpmix.rs
--rw-r--r--   0        0        0      928 2023-03-09 17:13:31.000000 egobox-0.8.2/src/lib.rs
--rw-r--r--   0        0        0     3232 2023-03-09 17:13:31.000000 egobox-0.8.2/src/types.rs
--rw-r--r--   0        0        0     7267 1970-01-01 00:00:00.000000 egobox-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1328 1970-01-01 00:00:00.000000 egobox-0.9.0/local_dependencies/egobox-gp/Cargo.toml
+-rw-r--r--   0        0        0     1090 2022-10-05 08:24:51.000000 egobox-0.9.0/local_dependencies/egobox-gp/README.md
+-rw-r--r--   0        0        0     2796 2023-01-30 08:37:24.000000 egobox-0.9.0/local_dependencies/egobox-gp/benches/gp.rs
+-rw-r--r--   0        0        0     1206 2022-04-13 12:11:37.000000 egobox-0.9.0/local_dependencies/egobox-gp/examples/kriging.rs
+-rw-r--r--   0        0        0    53115 2023-03-06 15:20:45.000000 egobox-0.9.0/local_dependencies/egobox-gp/src/algorithm.rs
+-rw-r--r--   0        0        0    21783 2022-12-13 14:13:12.000000 egobox-0.9.0/local_dependencies/egobox-gp/src/correlation_models.rs
+-rw-r--r--   0        0        0     1035 2022-08-18 12:20:53.000000 egobox-0.9.0/local_dependencies/egobox-gp/src/errors.rs
+-rw-r--r--   0        0        0     4239 2022-10-05 08:24:51.000000 egobox-0.9.0/local_dependencies/egobox-gp/src/lib.rs
+-rw-r--r--   0        0        0     7471 2023-01-30 08:37:24.000000 egobox-0.9.0/local_dependencies/egobox-gp/src/mean_models.rs
+-rw-r--r--   0        0        0     4576 2023-03-06 15:20:45.000000 egobox-0.9.0/local_dependencies/egobox-gp/src/parameters.rs
+-rw-r--r--   0        0        0     7096 2022-12-05 16:09:19.000000 egobox-0.9.0/local_dependencies/egobox-gp/src/utils.rs
+-rw-r--r--   0        0        0      851 1970-01-01 00:00:00.000000 egobox-0.9.0/local_dependencies/egobox-doe/Cargo.toml
+-rw-r--r--   0        0        0      970 2022-04-13 12:11:37.000000 egobox-0.9.0/local_dependencies/egobox-doe/README.md
+-rw-r--r--   0        0        0      585 2023-01-30 08:37:24.000000 egobox-0.9.0/local_dependencies/egobox-doe/benches/lhs.rs
+-rw-r--r--   0        0        0      841 2023-01-30 08:37:24.000000 egobox-0.9.0/local_dependencies/egobox-doe/examples/samplings.rs
+-rw-r--r--   0        0        0     3416 2022-12-28 17:44:23.000000 egobox-0.9.0/local_dependencies/egobox-doe/src/full_factorial.rs
+-rw-r--r--   0        0        0    14760 2023-03-03 16:02:22.000000 egobox-0.9.0/local_dependencies/egobox-doe/src/lhs.rs
+-rw-r--r--   0        0        0     1701 2022-12-14 13:14:49.000000 egobox-0.9.0/local_dependencies/egobox-doe/src/lib.rs
+-rw-r--r--   0        0        0     3350 2022-12-28 17:44:23.000000 egobox-0.9.0/local_dependencies/egobox-doe/src/random.rs
+-rw-r--r--   0        0        0     1743 2022-09-08 08:39:18.000000 egobox-0.9.0/local_dependencies/egobox-doe/src/traits.rs
+-rw-r--r--   0        0        0     2247 2022-04-13 12:11:37.000000 egobox-0.9.0/local_dependencies/egobox-doe/src/utils.rs
+-rw-r--r--   0        0        0     1657 1970-01-01 00:00:00.000000 egobox-0.9.0/local_dependencies/egobox-moe/Cargo.toml
+-rw-r--r--   0        0        0     1036 2022-10-05 08:24:51.000000 egobox-0.9.0/local_dependencies/egobox-moe/README.md
+-rw-r--r--   0        0        0     1431 2022-12-14 13:14:49.000000 egobox-0.9.0/local_dependencies/egobox-moe/benches/bench_find_nb_clusters.rs
+-rw-r--r--   0        0        0     1506 2022-08-18 12:20:53.000000 egobox-0.9.0/local_dependencies/egobox-moe/examples/clustering.rs
+-rw-r--r--   0        0        0     1564 2023-01-30 08:37:24.000000 egobox-0.9.0/local_dependencies/egobox-moe/examples/moe_norm1.rs
+-rw-r--r--   0        0        0     1260 2022-08-18 12:20:53.000000 egobox-0.9.0/local_dependencies/egobox-moe/examples/norm1.rs
+-rw-r--r--   0        0        0    12658 2022-04-13 12:11:37.000000 egobox-0.9.0/local_dependencies/egobox-moe/examples/norm1_D2_200.csv
+-rw-r--r--   0        0        0    46305 2023-03-27 15:22:25.000000 egobox-0.9.0/local_dependencies/egobox-moe/src/algorithm.rs
+-rw-r--r--   0        0        0    17244 2023-02-11 16:49:33.000000 egobox-0.9.0/local_dependencies/egobox-moe/src/clustering.rs
+-rw-r--r--   0        0        0     1574 2023-02-11 16:49:34.000000 egobox-0.9.0/local_dependencies/egobox-moe/src/errors.rs
+-rw-r--r--   0        0        0     4569 2023-03-27 15:22:25.000000 egobox-0.9.0/local_dependencies/egobox-moe/src/expertise_macros.rs
+-rw-r--r--   0        0        0    14971 2023-01-30 08:37:24.000000 egobox-0.9.0/local_dependencies/egobox-moe/src/gaussian_mixture.rs
+-rw-r--r--   0        0        0     4070 2022-12-20 08:24:26.000000 egobox-0.9.0/local_dependencies/egobox-moe/src/lib.rs
+-rw-r--r--   0        0        0    11012 2023-01-30 08:37:24.000000 egobox-0.9.0/local_dependencies/egobox-moe/src/parameters.rs
+-rw-r--r--   0        0        0     8879 2023-02-08 08:11:35.000000 egobox-0.9.0/local_dependencies/egobox-moe/src/surrogates.rs
+-rw-r--r--   0        0        0     1781 1970-01-01 00:00:00.000000 egobox-0.9.0/local_dependencies/egobox-ego/Cargo.toml
+-rw-r--r--   0        0        0     1046 2022-10-05 08:24:51.000000 egobox-0.9.0/local_dependencies/egobox-ego/README.md
+-rw-r--r--   0        0        0      992 2023-06-02 12:43:09.000000 egobox-0.9.0/local_dependencies/egobox-ego/examples/ackley.rs
+-rw-r--r--   0        0        0     8050 2023-06-02 12:43:11.000000 egobox-0.9.0/local_dependencies/egobox-ego/examples/mopta08.rs
+-rw-r--r--   0        0        0      840 2023-06-02 12:43:15.000000 egobox-0.9.0/local_dependencies/egobox-ego/examples/rosenbrock.rs
+-rw-r--r--   0        0        0     3504 2023-05-25 18:46:53.000000 egobox-0.9.0/local_dependencies/egobox-ego/src/criteria/ei.rs
+-rw-r--r--   0        0        0     1178 2023-05-25 18:46:53.000000 egobox-0.9.0/local_dependencies/egobox-ego/src/criteria/mod.rs
+-rw-r--r--   0        0        0     6226 2023-05-25 18:46:53.000000 egobox-0.9.0/local_dependencies/egobox-ego/src/criteria/wb2.rs
+-rw-r--r--   0        0        0    22816 2023-06-02 20:39:23.000000 egobox-0.9.0/local_dependencies/egobox-ego/src/egor.rs
+-rw-r--r--   0        0        0    52489 2023-06-02 14:33:24.000000 egobox-0.9.0/local_dependencies/egobox-ego/src/egor_solver.rs
+-rw-r--r--   0        0        0    29196 2023-03-29 09:38:32.000000 egobox-0.9.0/local_dependencies/egobox-ego/src/egor_state.rs
+-rw-r--r--   0        0        0     1423 2023-01-11 09:58:59.000000 egobox-0.9.0/local_dependencies/egobox-ego/src/errors.rs
+-rw-r--r--   0        0        0     6075 2023-03-03 16:02:22.000000 egobox-0.9.0/local_dependencies/egobox-ego/src/lhs_optimizer.rs
+-rw-r--r--   0        0        0     9321 2023-06-02 20:47:16.000000 egobox-0.9.0/local_dependencies/egobox-ego/src/lib.rs
+-rw-r--r--   0        0        0    26236 2023-03-09 17:13:31.000000 egobox-0.9.0/local_dependencies/egobox-ego/src/mixint.rs
+-rw-r--r--   0        0        0     7718 2022-04-13 12:11:37.000000 egobox-0.9.0/local_dependencies/egobox-ego/src/sort_axis.rs
+-rw-r--r--   0        0        0     5151 2023-06-02 20:12:27.000000 egobox-0.9.0/local_dependencies/egobox-ego/src/types.rs
+-rw-r--r--   0        0        0     3377 2023-05-25 18:46:53.000000 egobox-0.9.0/local_dependencies/egobox-ego/src/utils.rs
+-rw-r--r--   0        0        0     1627 1970-01-01 00:00:00.000000 egobox-0.9.0/Cargo.toml
+-rw-r--r--   0        0        0      586 2023-02-07 14:17:13.000000 egobox-0.9.0/.gitignore
+-rw-r--r--   0        0        0     5917 2023-06-02 20:58:12.000000 egobox-0.9.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2177 2022-10-05 08:24:51.000000 egobox-0.9.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      410 2022-08-18 12:20:53.000000 egobox-0.9.0/Dockerfile
+-rw-r--r--   0        0        0    11558 2022-04-13 12:11:37.000000 egobox-0.9.0/LICENSE
+-rw-r--r--   0        0        0     6361 2023-06-02 21:03:26.000000 egobox-0.9.0/README.md
+-rw-r--r--   0        0        0    37898 2023-03-09 07:55:59.000000 egobox-0.9.0/doc/Egor_Tutorial.ipynb
+-rw-r--r--   0        0        0   249207 2023-03-09 07:55:59.000000 egobox-0.9.0/doc/Gpx_MaunaLoaCO2.ipynb
+-rw-r--r--   0        0        0    49162 2023-03-09 07:55:59.000000 egobox-0.9.0/doc/Gpx_Tutorial.ipynb
+-rw-r--r--   0        0        0   117618 2022-10-10 20:47:14.000000 egobox-0.9.0/joss/egobox_architecture.png
+-rw-r--r--   0        0        0     4293 2022-10-10 20:47:14.000000 egobox-0.9.0/joss/paper.bib
+-rw-r--r--   0        0        0     5424 2022-10-10 20:47:14.000000 egobox-0.9.0/joss/paper.md
+-rw-r--r--   0        0        0      997 2023-06-02 20:44:34.000000 egobox-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0       23 2022-04-13 12:11:37.000000 egobox-0.9.0/python/egobox/__init__.py
+-rw-r--r--   0        0        0      791 2022-10-10 20:47:14.000000 egobox-0.9.0/python/egobox/examples/kriging.py
+-rw-r--r--   0        0        0     1660 2023-03-09 07:55:59.000000 egobox-0.9.0/python/egobox/examples/optim_g24.py
+-rw-r--r--   0        0        0     5812 2023-03-09 08:58:12.000000 egobox-0.9.0/python/egobox/tests/test_egor.py
+-rw-r--r--   0        0        0     1841 2022-10-10 20:47:14.000000 egobox-0.9.0/python/egobox/tests/test_gpmix.py
+-rw-r--r--   0        0        0      776 2023-03-29 09:38:32.000000 egobox-0.9.0/python/egobox/tests/test_mixintegor.py
+-rw-r--r--   0        0        0      980 2023-03-09 17:13:31.000000 egobox-0.9.0/python/egobox/tests/test_utils.py
+-rw-r--r--   0        0        0    14705 2023-06-02 20:39:21.000000 egobox-0.9.0/src/egor.rs
+-rw-r--r--   0        0        0     8122 2023-06-01 09:43:34.000000 egobox-0.9.0/src/gpmix.rs
+-rw-r--r--   0        0        0      928 2023-03-09 17:13:31.000000 egobox-0.9.0/src/lib.rs
+-rw-r--r--   0        0        0     3306 2023-05-23 12:35:44.000000 egobox-0.9.0/src/types.rs
+-rw-r--r--   0        0        0     7267 1970-01-01 00:00:00.000000 egobox-0.9.0/PKG-INFO
```

### Comparing `egobox-0.8.2/local_dependencies/egobox-ego/Cargo.toml` & `egobox-0.9.0/local_dependencies/egobox-ego/Cargo.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "egobox-ego"
-version = "0.8.2"
+version = "0.9.0"
 authors = ["Rémi Lafage <remi.lafage@onera.fr>"]
 edition = "2018"
 description = "A library for efficient global optimization"
 license = "Apache-2.0"
 repository = "https://github.com/relf/egobox"
 keywords = ["machine-learning", "bayesian", "optimization"]
 categories = ["algorithms", "mathematics", "science"]
@@ -12,17 +12,17 @@
 [features]
 default = []
 
 persistent = ["serde_json"]
 blas = ["ndarray-linalg", "linfa/ndarray-linalg", "linfa-pls/blas"]
 
 [dependencies]
-egobox-doe = { version = "0.8.1", path = "../egobox-doe", features = ["serializable"] }
-egobox-gp = { version = "0.8.1", path = "../egobox-gp", features = ["serializable"] }
-egobox-moe = { version = "0.8.1", path = "../egobox-moe", features = ["serializable"] }
+egobox-doe = { version = "0.9.0", path = "../egobox-doe", features = ["serializable"] }
+egobox-gp = { version = "0.9.0", path = "../egobox-gp", features = ["serializable"] }
+egobox-moe = { version = "0.9.0", path = "../egobox-moe", features = ["serializable"] }
 
 linfa = { version = "0.6.1", default-features = false }
 linfa-pls = { version = "0.6.1", default-features = false }
 linfa-linalg = { version = "0.1", default-features = false }
 
 ndarray = { version = "0.15", features = ["rayon", "approx"]}
 ndarray-linalg = { version = "0.15", optional = true }
@@ -44,13 +44,14 @@
 thiserror = "1"
 anyhow = "1"
 clap = { version = "4", features=["derive"] }
 
 serde = { version = "1", features = ["derive", "rc"] }
 serde_json = { version = "1", optional = true }
 typetag = { version = "0.1" }
+dyn-clonable = { version = "0.9" }
 
 [dev-dependencies]
 criterion = "0.4.0"
 approx = "0.4"
 argmin_testfunctions = "0.1"
 serial_test = "0.9.0"
```

### Comparing `egobox-0.8.2/local_dependencies/egobox-ego/README.md` & `egobox-0.9.0/local_dependencies/egobox-ego/README.md`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/local_dependencies/egobox-ego/examples/ackley.rs` & `egobox-0.9.0/local_dependencies/egobox-ego/examples/ackley.rs`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/local_dependencies/egobox-ego/examples/mopta08.rs` & `egobox-0.9.0/local_dependencies/egobox-ego/examples/mopta08.rs`

 * *Files 0% similar despite different names*

```diff
@@ -259,23 +259,23 @@
     let mut xlimits = Array2::zeros((dim, 2));
     xlimits.column_mut(1).assign(&Array1::ones(dim));
 
     let res = EgorBuilder::optimize(mopta_func(dim))
         .min_within(&xlimits)
         .n_cstr(68)
         .cstr_tol(cstr_tol)
-        .n_clusters(Some(1))
+        .n_clusters(1)
         .n_start(50)
         .n_doe(n_doe)
         .n_iter(n_iter)
         .regression_spec(RegressionSpec::CONSTANT)
         .correlation_spec(CorrelationSpec::SQUAREDEXPONENTIAL)
         .infill_optimizer(InfillOptimizer::Slsqp)
-        .kpls_dim(Some(kpls_dim))
-        .outdir(Some(outdir))
+        .kpls_dim(kpls_dim)
+        .outdir(outdir)
         .hot_start(true)
         .run()
         .expect("Minimize failure");
     println!(
         "Mopta08 dim={} minimum y = {} at x = {}",
         dim, res.y_opt, res.x_opt
     );
```

### Comparing `egobox-0.8.2/local_dependencies/egobox-ego/examples/rosenbrock.rs` & `egobox-0.9.0/local_dependencies/egobox-ego/examples/rosenbrock.rs`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/local_dependencies/egobox-ego/src/egor.rs` & `egobox-0.9.0/local_dependencies/egobox-ego/src/egor.rs`

 * *Files 3% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 //! let xlimits = array![[0., 3.], [0., 4.]];
 //! let doe = Lhs::new(&xlimits).sample(10);
 //! let res = EgorBuilder::optimize(f_g24)
 //!            .min_within(&xlimits)
 //!            .n_cstr(2)
 //!            .infill_strategy(InfillStrategy::EI)
 //!            .infill_optimizer(InfillOptimizer::Cobyla)
-//!            .doe(Some(doe))
+//!            .doe(&doe)
 //!            .n_iter(40)
 //!            .target(-5.5080)
 //!            .run()
 //!            .expect("g24 minimized");
 //! println!("G24 min result = {:?}", res);
 //! ```
 //!
@@ -122,16 +122,17 @@
     /// reproducible runs.
     pub fn random_seed(mut self, seed: u64) -> Self {
         self.seed = Some(seed);
         self
     }
 
     /// Build an Egor optimizer to minimize the function within
-    /// the continuous xlimits specified as [[lower, upper], ...]
-    /// number of rows gives the dimension of the inputs (continuous optimization).
+    /// the continuous `xlimits` specified as [[lower, upper], ...] array where the
+    /// number of rows gives the dimension of the inputs (continuous optimization)
+    /// and the ith row is the interval of the ith component of the input x.
     pub fn min_within(
         self,
         xlimits: &ArrayBase<impl Data<Elem = f64>, Ix2>,
     ) -> Egor<O, MoeParams<f64, Xoshiro256Plus>> {
         let rng = if let Some(seed) = self.seed {
             Xoshiro256Plus::seed_from_u64(seed)
         } else {
@@ -142,15 +143,15 @@
             solver: EgorSolver::new(xlimits, rng),
         }
     }
 
     /// Build an Egor optimizer to minimize the function R^n -> R^p taking
     /// inputs specified with given xtypes where some of components may be
     /// discrete variables (mixed-integer optimization).
-    pub fn min_within_mixed_space(self, xtypes: &[XType]) -> Egor<O, MixintMoeParams> {
+    pub fn min_within_mixint_space(self, xtypes: &[XType]) -> Egor<O, MixintMoeParams> {
         let rng = if let Some(seed) = self.seed {
             Xoshiro256Plus::seed_from_u64(seed)
         } else {
             Xoshiro256Plus::from_entropy()
         };
         Egor {
             fobj: ObjFunc::new(self.fobj),
@@ -203,33 +204,33 @@
 
     /// Sets the tolerance on constraints violation (cstr < tol)
     pub fn cstr_tol(mut self, tol: f64) -> Self {
         self.solver = self.solver.cstr_tol(tol);
         self
     }
 
-    /// Sets an initial DOE containing ns samples
+    /// Sets an initial DOE \['ns', `nt`\] containing `ns` samples.
     ///
-    /// Either nt = nx then only x are specified and ns evals are done to get y doe values,
-    /// or nt = nx + ny then x = doe(:, :nx) and y = doe(:, nx:) are specified
-    pub fn doe(mut self, doe: Option<Array2<f64>>) -> Self {
+    /// Either `nt` = `nx` then only `x` input values are specified and `ns` evals are done to get y ouput doe values,
+    /// or `nt = nx + ny` then `x = doe\[:, :nx\]` and `y = doe\[:, nx:\]` are specified
+    pub fn doe(mut self, doe: &Array2<f64>) -> Self {
         self.solver = self.solver.doe(doe);
         self
     }
 
     /// Sets the parallel infill strategy
     ///
-    /// Parallel infill criteria to get virtual next promising points in order to allow
+    /// Parallel infill criterion to get virtual next promising points in order to allow
     /// n parallel evaluations of the function under optimization.
     pub fn qei_strategy(mut self, q_ei: QEiStrategy) -> Self {
         self.solver = self.solver.qei_strategy(q_ei);
         self
     }
 
-    /// Sets the nfill criteria
+    /// Sets the infill strategy
     pub fn infill_strategy(mut self, infill: InfillStrategy) -> Self {
         self.solver = self.solver.infill_strategy(infill);
         self
     }
 
     /// Sets the infill optimizer
     pub fn infill_optimizer(mut self, optimizer: InfillOptimizer) -> Self {
@@ -247,50 +248,51 @@
     pub fn correlation_spec(mut self, correlation_spec: CorrelationSpec) -> Self {
         self.solver = self.solver.correlation_spec(correlation_spec);
         self
     }
 
     /// Sets the number of components to be used specifiying PLS projection is used (a.k.a KPLS method).
     ///
-    /// This is used to address high-dimensional problems typically when nx > 9.
-    pub fn kpls_dim(mut self, kpls_dim: Option<usize>) -> Self {
+    /// This is used to address high-dimensional problems typically when `nx` > 9 wher `nx` is the dimension of `x`.
+    pub fn kpls_dim(mut self, kpls_dim: usize) -> Self {
         self.solver = self.solver.kpls_dim(kpls_dim);
         self
     }
 
     /// Sets the number of clusters used by the mixture of surrogate experts.
     ///
     /// When set to 0, the number of clusters is determined automatically
-    pub fn n_clusters(mut self, n_clusters: Option<usize>) -> Self {
+    /// (warning in this case the optimizer runs slower)
+    pub fn n_clusters(mut self, n_clusters: usize) -> Self {
         self.solver = self.solver.n_clusters(n_clusters);
         self
     }
 
     /// Sets a known target minimum to be used as a stopping criterion.
     pub fn target(mut self, target: f64) -> Self {
         self.solver = self.solver.target(target);
         self
     }
 
     /// Sets a directory to write optimization history and used as search path for hot start doe
-    pub fn outdir(mut self, outdir: Option<String>) -> Self {
+    pub fn outdir(mut self, outdir: impl Into<String>) -> Self {
         self.solver = self.solver.outdir(outdir);
         self
     }
 
     /// Whether we start by loading last DOE saved in `outdir` as initial DOE
     pub fn hot_start(mut self, hot_start: bool) -> Self {
         self.solver = self.solver.hot_start(hot_start);
         self
     }
 
     /// Given an evaluated doe (x, y) data, return the next promising x point
     /// where optimum may occurs regarding the infill criterium.
     /// This function inverse the control of the optimization and can used
-    /// ask-and-tell interface to the EGO optmizer.
+    /// ask-and-tell interface to the EGO optimizer.
     pub fn suggest(
         &self,
         x_data: &ArrayBase<impl Data<Elem = f64>, Ix2>,
         y_data: &ArrayBase<impl Data<Elem = f64>, Ix2>,
     ) -> Array2<f64> {
         self.solver.suggest(x_data, y_data)
     }
@@ -368,17 +370,17 @@
         let initial_doe = array![[0.], [7.], [25.]];
         let res = EgorBuilder::optimize(xsinx)
             .min_within(&array![[0.0, 25.0]])
             .infill_strategy(InfillStrategy::EI)
             .regression_spec(RegressionSpec::QUADRATIC)
             .correlation_spec(CorrelationSpec::ALL)
             .n_iter(30)
-            .doe(Some(initial_doe.to_owned()))
+            .doe(&initial_doe)
             .target(-15.1)
-            .outdir(Some("target/tests".to_string()))
+            .outdir("target/tests")
             .run()
             .expect("Egor should minimize xsinx");
         let expected = array![-15.1];
         assert_abs_diff_eq!(expected, res.y_opt, epsilon = 0.5);
         let saved_doe: Array2<f64> = read_npy(format!("target/tests/{DOE_INITIAL_FILE}")).unwrap();
         assert_abs_diff_eq!(initial_doe, saved_doe.slice(s![..3, ..1]), epsilon = 1e-6);
     }
@@ -398,15 +400,15 @@
     }
 
     #[test]
     #[serial]
     fn test_xsinx_auto_clustering_egor_builder() {
         let res = EgorBuilder::optimize(xsinx)
             .min_within(&array![[0.0, 25.0]])
-            .n_clusters(Some(0))
+            .n_clusters(0)
             .n_iter(20)
             .run()
             .expect("Egor with auto clustering should minimize xsinx");
         let expected = array![18.9];
         assert_abs_diff_eq!(expected, res.x_opt, epsilon = 1e-1);
     }
 
@@ -415,26 +417,26 @@
     fn test_xsinx_with_hotstart_egor_builder() {
         let xlimits = array![[0.0, 25.0]];
         let doe = Lhs::new(&xlimits).sample(10);
         let res = EgorBuilder::optimize(xsinx)
             .random_seed(42)
             .min_within(&xlimits)
             .n_iter(15)
-            .doe(Some(doe))
-            .outdir(Some("target/tests".to_string()))
+            .doe(&doe)
+            .outdir("target/tests")
             .run()
             .expect("Minimize failure");
         let expected = array![18.9];
         assert_abs_diff_eq!(expected, res.x_opt, epsilon = 1e-1);
 
         let res = EgorBuilder::optimize(xsinx)
             .random_seed(42)
             .min_within(&xlimits)
             .n_iter(5)
-            .outdir(Some("target/tests".to_string()))
+            .outdir("target/tests")
             .hot_start(true)
             .run()
             .expect("Egor should minimize xsinx");
         let expected = array![18.9];
         assert_abs_diff_eq!(expected, res.x_opt, epsilon = 1e-1);
     }
 
@@ -477,15 +479,15 @@
         let xlimits = array![[-2., 2.], [-2., 2.]];
         let doe = Lhs::new(&xlimits)
             .with_rng(Xoshiro256Plus::seed_from_u64(42))
             .sample(10);
         let res = EgorBuilder::optimize(rosenb)
             .random_seed(42)
             .min_within(&xlimits)
-            .doe(Some(doe))
+            .doe(&doe)
             .n_iter(100)
             .regression_spec(RegressionSpec::ALL)
             .correlation_spec(CorrelationSpec::ALL)
             .target(1e-2)
             .run()
             .expect("Minimize failure");
         println!("Rosenbrock optim result = {res:?}");
@@ -527,15 +529,15 @@
         let doe = Lhs::new(&xlimits)
             .with_rng(Xoshiro256Plus::seed_from_u64(42))
             .sample(3);
         let res = EgorBuilder::optimize(f_g24)
             .random_seed(42)
             .min_within(&xlimits)
             .n_cstr(2)
-            .doe(Some(doe))
+            .doe(&doe)
             .n_iter(20)
             .run()
             .expect("Minimize failure");
         println!("G24 optim result = {res:?}");
         let expected = array![2.3295, 3.1785];
         assert_abs_diff_eq!(expected, res.x_opt, epsilon = 2e-2);
     }
@@ -550,15 +552,15 @@
             .random_seed(42)
             .min_within(&xlimits)
             .regression_spec(RegressionSpec::ALL)
             .correlation_spec(CorrelationSpec::ALL)
             .n_cstr(2)
             .q_points(2)
             .qei_strategy(QEiStrategy::KrigingBeliever)
-            .doe(Some(doe))
+            .doe(&doe)
             .target(-5.508013)
             .n_iter(30)
             .run()
             .expect("Egor minimization");
         println!("G24 optim result = {res:?}");
         let expected = array![2.3295, 3.1785];
         assert_abs_diff_eq!(expected, res.x_opt, epsilon = 2e-2);
@@ -579,16 +581,16 @@
     fn test_mixsinx_ei_mixint_egor_builder() {
         let n_iter = 30;
         let doe = array![[0.], [7.], [25.]];
         let xtypes = vec![XType::Int(0, 25)];
 
         let res = EgorBuilder::optimize(mixsinx)
             .random_seed(42)
-            .min_within_mixed_space(&xtypes)
-            .doe(Some(doe))
+            .min_within_mixint_space(&xtypes)
+            .doe(&doe)
             .n_iter(n_iter)
             .target(-15.1)
             .infill_strategy(InfillStrategy::EI)
             .run()
             .unwrap();
         assert_abs_diff_eq!(array![18.], res.x_opt, epsilon = 2.);
     }
@@ -597,16 +599,16 @@
     fn test_mixsinx_reclustering_mixint_egor_builder() {
         let n_iter = 30;
         let doe = array![[0.], [7.], [25.]];
         let xtypes = vec![XType::Int(0, 25)];
 
         let res = EgorBuilder::optimize(mixsinx)
             .random_seed(42)
-            .min_within_mixed_space(&xtypes)
-            .doe(Some(doe))
+            .min_within_mixint_space(&xtypes)
+            .doe(&doe)
             .n_iter(n_iter)
             .target(-15.1)
             .infill_strategy(InfillStrategy::EI)
             .run()
             .unwrap();
         assert_abs_diff_eq!(array![18.], res.x_opt, epsilon = 2.);
     }
@@ -615,17 +617,16 @@
     #[serial]
     fn test_mixsinx_wb2_mixint_egor_builder() {
         let n_iter = 30;
         let xtypes = vec![XType::Int(0, 25)];
 
         let res = EgorBuilder::optimize(mixsinx)
             .random_seed(42)
-            .min_within_mixed_space(&xtypes)
+            .min_within_mixint_space(&xtypes)
             .regression_spec(egobox_moe::RegressionSpec::CONSTANT)
             .correlation_spec(egobox_moe::CorrelationSpec::SQUAREDEXPONENTIAL)
             .n_iter(n_iter)
-            .infill_strategy(InfillStrategy::WB2)
             .run()
             .unwrap();
         assert_abs_diff_eq!(&array![18.], &res.x_opt, epsilon = 3.);
     }
 }
```

### Comparing `egobox-0.8.2/local_dependencies/egobox-ego/src/egor_solver.rs` & `egobox-0.9.0/local_dependencies/egobox-ego/src/egor_solver.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 //! Egor implementation as a [argmin::core::Solver] to be used to benefit from
 //! features coming with the argmin framework such as checkpointing or observers.
 //!
 //! Note: Depending on your need you can either use the `EgorSolver` or the provided
 //! `EgorBuilder` which allows to build an `Egor` struct which wraps the `argmin::Executor`
-//! running an `EgorSolver` on `ObjFun`. See [`EgorBuilder`]
+//! running an `EgorSolver` on `ObjFun`. See [`crate::EgorBuilder`]
 //!
 //! ```no_run
 //! use ndarray::{array, Array2, ArrayView1, ArrayView2, Zip};
 //! use egobox_doe::{Lhs, SamplingMethod};
 //! use egobox_ego::{EgorBuilder, InfillStrategy, InfillOptimizer, ObjFunc, EgorSolver};
 //! use egobox_moe::MoeParams;
 //! use rand_xoshiro::Xoshiro256Plus;
@@ -85,32 +85,32 @@
 //!
 //! let fobj = ObjFunc::new(f_g24);
 //! let solver: EgorSolver<MoeParams<f64, Xoshiro256Plus>> =
 //!   EgorSolver::new(&xlimits, rng)             
 //!     .n_cstr(2)
 //!     .infill_strategy(InfillStrategy::EI)
 //!     .infill_optimizer(InfillOptimizer::Cobyla)
-//!     .doe(Some(doe))
+//!     .doe(&doe)
 //!     .target(-5.5080);
 //!
 //! let res = Executor::new(fobj, solver)
 //!             .configure(|state| state.max_iters(40))
 //!             .run()
 //!             .expect("g24 minimized");
 //! println!("G24 min result = {:?}", res.state);
 //! ```
 //!
+use crate::criteria::*;
 use crate::egor_state::{find_best_result_index, EgorState, MAX_POINT_ADDITION_RETRY};
 use crate::errors::{EgoError, Result};
 use crate::lhs_optimizer::LhsOptimizer;
 use crate::mixint::*;
 use crate::types::*;
-use crate::utils::{compute_cstr_scales, compute_wb2s_scale, grad_wbs2};
-use crate::utils::{ei, wb2s};
-use crate::utils::{grad_ei, update_data};
+use crate::utils::compute_cstr_scales;
+use crate::utils::update_data;
 
 use egobox_doe::{Lhs, LhsKind, SamplingMethod};
 use egobox_moe::{ClusteredSurrogate, Clustering, CorrelationSpec, MoeParams, RegressionSpec};
 use env_logger::{Builder, Env};
 use finitediff::FiniteDiff;
 use linfa::ParamGuard;
 use log::{debug, info, warn};
@@ -154,32 +154,32 @@
     pub(crate) n_doe: usize,
     /// Number of Constraints
     /// Note: dim function ouput = 1 objective + n_cstr constraints
     pub(crate) n_cstr: usize,
     /// Constraints violation tolerance meaning cstr < cstr_tol is considered valid
     pub(crate) cstr_tol: f64,
     /// Initial doe can be either \[x\] with x inputs only or an evaluated doe \[x, y\]
-    /// Note: x dimension is determined using xlimits
+    /// Note: x dimension is determined using `xlimits.nrows()`
     pub(crate) doe: Option<Array2<f64>>,
     /// Multipoint strategy used to get several points to be evaluated at each iteration
     pub(crate) q_ei: QEiStrategy,
-    /// Criterium to select next point to evaluate
-    pub(crate) infill: InfillStrategy,
+    /// Criterion to select next point to evaluate
+    pub(crate) infill_criterion: Box<dyn InfillCriterion>,
     /// The optimizer used to optimize infill criterium
     pub(crate) infill_optimizer: InfillOptimizer,
     /// Regression specification for GP models used by mixture of experts (see [egobox_moe])
     pub(crate) regression_spec: RegressionSpec,
     /// Correlation specification for GP models used by mixture of experts (see [egobox_moe])
     pub(crate) correlation_spec: CorrelationSpec,
     /// Optional dimension reduction (see [egobox_moe])
     pub(crate) kpls_dim: Option<usize>,
     /// Number of clusters used by mixture of experts (see [egobox_moe])
     /// When set to 0 the clusters are computes automatically and refreshed
     /// every 10-points (tentative) additions
-    pub(crate) n_clusters: Option<usize>,
+    pub(crate) n_clusters: usize,
     /// Specification of a target objective value which is used to stop the algorithm once reached
     pub(crate) target: f64,
     /// Directory to save intermediate results: inital doe + evalutions at each iteration
     pub(crate) outdir: Option<String>,
     /// If true use `outdir` to retrieve and start from previous results
     pub(crate) hot_start: bool,
     /// Matrix (nx, 2) of [lower bound, upper bound] of the nx components of x
@@ -262,20 +262,20 @@
             n_start: 20,
             q_points: 1,
             n_doe: 0,
             n_cstr: 0,
             cstr_tol: 1e-6,
             doe: None,
             q_ei: QEiStrategy::KrigingBeliever,
-            infill: InfillStrategy::WB2,
+            infill_criterion: Box::new(WB2),
             infill_optimizer: InfillOptimizer::Slsqp,
             regression_spec: RegressionSpec::CONSTANT,
             correlation_spec: CorrelationSpec::SQUAREDEXPONENTIAL,
             kpls_dim: None,
-            n_clusters: Some(1),
+            n_clusters: 1,
             target: f64::NEG_INFINITY,
             outdir: None,
             hot_start: false,
             xlimits: xlimits.to_owned(),
             xtypes: Some(continuous_xlimits_to_xtypes(xlimits)),
             no_discrete: true,
             surrogate_builder: SB::new_with_xtypes_rng(&continuous_xlimits_to_xtypes(xlimits)),
@@ -284,15 +284,15 @@
     }
 
     /// Constructor of the optimization of the function `f` with specified random generator
     /// to get reproducibility. This constructor is used  for mixed-integer optimization
     /// when `f` has discrete inputs to be specified with list of xtypes.
     ///
     /// The function `f` should return an objective but also constraint values if any.
-    /// Design space is specified by a list of types for input variables `x` of `f` (see [XType]).
+    /// Design space is specified by a list of types for input variables `x` of `f` (see [`XType`]).
     pub fn new_with_xtypes(xtypes: &[XType], rng: Xoshiro256Plus) -> Self {
         let env = Env::new().filter_or("EGOBOX_LOG", "info");
         let mut builder = Builder::from_env(env);
         let builder = builder.target(env_logger::Target::Stdout);
         builder.try_init().ok();
         let v_xtypes = xtypes.to_vec();
         let xlimits = unfold_xtypes_as_continuous_limits(xtypes);
@@ -301,33 +301,38 @@
             n_start: 20,
             q_points: 1,
             n_doe: 0,
             n_cstr: 0,
             cstr_tol: 1e-6,
             doe: None,
             q_ei: QEiStrategy::KrigingBeliever,
-            infill: InfillStrategy::WB2,
+            infill_criterion: Box::new(WB2),
             infill_optimizer: InfillOptimizer::Slsqp,
             regression_spec: RegressionSpec::CONSTANT,
             correlation_spec: CorrelationSpec::SQUAREDEXPONENTIAL,
             kpls_dim: None,
-            n_clusters: Some(1),
+            n_clusters: 1,
             target: f64::NEG_INFINITY,
             outdir: None,
             hot_start: false,
             xlimits,
             xtypes: Some(v_xtypes),
             surrogate_builder: SB::new_with_xtypes_rng(xtypes),
             no_discrete: !xtypes
                 .iter()
                 .any(|t| matches!(t, &XType::Int(_, _) | &XType::Ord(_) | &XType::Enum(_))),
             rng,
         }
     }
 
+    pub fn infill_criterion(mut self, infill_criterion: Box<dyn InfillCriterion>) -> Self {
+        self.infill_criterion = infill_criterion;
+        self
+    }
+
     /// Sets allowed number of evaluation of the function under optimization
     pub fn n_iter(mut self, n_iter: usize) -> Self {
         self.n_iter = n_iter;
         self
     }
 
     /// Sets the number of runs of infill strategy optimizations (best result taken)
@@ -353,41 +358,51 @@
 
     /// Sets the number of constraint functions
     pub fn n_cstr(mut self, n_cstr: usize) -> Self {
         self.n_cstr = n_cstr;
         self
     }
 
-    /// Sets the tolerance on constraints violation (cstr < tol)
+    /// Sets the tolerance on constraints violation (`cstr < tol`)
     pub fn cstr_tol(mut self, tol: f64) -> Self {
         self.cstr_tol = tol;
         self
     }
 
-    /// Sets an initial DOE containing ns samples
+    /// Sets an initial DOE \['ns', `nt`\] containing `ns` samples.
     ///
-    /// Either nt = nx then only x are specified and ns evals are done to get y doe values,
-    /// or nt = nx + ny then x = doe(:, :nx) and y = doe(:, nx:) are specified
-    pub fn doe(mut self, doe: Option<Array2<f64>>) -> Self {
-        self.doe = doe.map(|x| x.to_owned());
+    /// Either `nt` = `nx` then only `x` input values are specified and `ns` evals are done to get y ouput doe values,
+    /// or `nt = nx + ny` then `x = doe\[:, :nx\]` and `y = doe\[:, nx:\]` are specified
+    pub fn doe(mut self, doe: &Array2<f64>) -> Self {
+        self.doe = Some(doe.to_owned());
+        self
+    }
+
+    /// Removes any previously specified initial doe to get the default doe usage
+    pub fn default_doe(mut self) -> Self {
+        self.doe = None;
         self
     }
 
     /// Sets the parallel infill strategy
     ///
     /// Parallel infill criterion to get virtual next promising points in order to allow
     /// n parallel evaluations of the function under optimization.
     pub fn qei_strategy(mut self, q_ei: QEiStrategy) -> Self {
         self.q_ei = q_ei;
         self
     }
 
-    /// Sets the nfill criteria
+    /// Sets the infill strategy
     pub fn infill_strategy(mut self, infill: InfillStrategy) -> Self {
-        self.infill = infill;
+        self.infill_criterion = match infill {
+            InfillStrategy::EI => Box::new(EI),
+            InfillStrategy::WB2 => Box::new(WB2),
+            InfillStrategy::WB2S => Box::new(WB2S),
+        };
         self
     }
 
     /// Sets the infill optimizer
     pub fn infill_optimizer(mut self, optimizer: InfillOptimizer) -> Self {
         self.infill_optimizer = optimizer;
         self
@@ -403,51 +418,62 @@
     pub fn correlation_spec(mut self, correlation_spec: CorrelationSpec) -> Self {
         self.correlation_spec = correlation_spec;
         self
     }
 
     /// Sets the number of components to be used specifiying PLS projection is used (a.k.a KPLS method).
     ///
-    /// This is used to address high-dimensional problems typically when nx > 9.
-    pub fn kpls_dim(mut self, kpls_dim: Option<usize>) -> Self {
-        self.kpls_dim = kpls_dim;
+    /// This is used to address high-dimensional problems typically when `nx` > 9 wher `nx` is the dimension of `x`.
+    pub fn kpls_dim(mut self, kpls_dim: usize) -> Self {
+        self.kpls_dim = Some(kpls_dim);
+        self
+    }
+
+    /// Removes any PLS dimension reduction usage
+    pub fn no_kpls(mut self) -> Self {
+        self.kpls_dim = None;
         self
     }
 
     /// Sets the number of clusters used by the mixture of surrogate experts.
     ///
     /// When set to Some(0), the number of clusters is determined automatically
     /// When set None, default to 1
-    pub fn n_clusters(mut self, n_clusters: Option<usize>) -> Self {
+    pub fn n_clusters(mut self, n_clusters: usize) -> Self {
         self.n_clusters = n_clusters;
         self
     }
 
     /// Sets a known target minimum to be used as a stopping criterion.
     pub fn target(mut self, target: f64) -> Self {
         self.target = target;
         self
     }
 
     /// Sets a directory to write optimization history and used as search path for hot start doe
-    pub fn outdir(mut self, outdir: Option<String>) -> Self {
-        self.outdir = outdir;
+    pub fn outdir(mut self, outdir: impl Into<String>) -> Self {
+        self.outdir = Some(outdir.into());
+        self
+    }
+    /// Do not write optimization history
+    pub fn no_outdir(mut self) -> Self {
+        self.outdir = None;
         self
     }
 
     /// Whether we start by loading last DOE saved in `outdir` as initial DOE
     pub fn hot_start(mut self, hot_start: bool) -> Self {
         self.hot_start = hot_start;
         self
     }
 
     /// Given an evaluated doe (x, y) data, return the next promising x point
     /// where optimum may occurs regarding the infill criterium.
     /// This function inverse the control of the optimization and can used
-    /// ask-and-tell interface to the EGO optmizer.
+    /// ask-and-tell interface to the EGO optimizer.
     pub fn suggest(
         &self,
         x_data: &ArrayBase<impl Data<Elem = f64>, Ix2>,
         y_data: &ArrayBase<impl Data<Elem = f64>, Ix2>,
     ) -> Array2<f64> {
         let rng = self.rng.clone();
         let sampling = Lhs::new(&self.xlimits).with_rng(rng).kind(LhsKind::Maximin);
@@ -718,19 +744,15 @@
 }
 
 impl<SB> EgorSolver<SB>
 where
     SB: SurrogateBuilder,
 {
     fn have_to_recluster(&self, added: usize, prev_added: usize) -> bool {
-        if let Some(nc) = self.n_clusters {
-            nc == 0 && (added != 0 && added % 10 == 0 && added - prev_added > 0)
-        } else {
-            false
-        }
+        self.n_clusters == 0 && (added != 0 && added % 10 == 0 && added - prev_added > 0)
     }
 
     fn make_clustered_surrogate(
         &self,
         xt: &ArrayBase<impl Data<Elem = f64>, Ix2>,
         yt: &ArrayBase<impl Data<Elem = f64>, Ix2>,
         init: bool,
@@ -738,15 +760,15 @@
         clustering: &Option<Clustering>,
         model_name: &str,
     ) -> Box<dyn ClusteredSurrogate> {
         let mut builder = self.surrogate_builder.clone();
         builder.set_kpls_dim(self.kpls_dim);
         builder.set_regression_spec(self.regression_spec);
         builder.set_correlation_spec(self.correlation_spec);
-        builder.set_n_clusters(self.n_clusters.unwrap_or(1));
+        builder.set_n_clusters(self.n_clusters);
 
         if init || recluster {
             if recluster {
                 info!("{} reclustering and training...", model_name);
             } else {
                 info!("{} initial clustering and training...", model_name);
             }
@@ -877,22 +899,18 @@
         let scale_cstr = if cstr_models.is_empty() {
             Array1::zeros((0,))
         } else {
             let scale_cstr = compute_cstr_scales(&scaling_points.view(), cstr_models);
             info!("Constraints scaling is updated to {}", scale_cstr);
             scale_cstr
         };
-        let scale_wb2 = if self.infill == InfillStrategy::WB2S {
-            let scale = compute_wb2s_scale(&scaling_points.view(), obj_model, f_min);
-            info!("WB2S scaling factor is updated to {}", scale);
-            scale
-        } else {
-            1.
-        };
-        (scale_infill_obj, scale_cstr, scale_wb2)
+        let scale_ic = self
+            .infill_criterion
+            .scaling(&scaling_points.view(), obj_model, f_min);
+        (scale_infill_obj, scale_cstr, scale_ic)
     }
 
     fn find_best_point(
         &self,
         x_data: &ArrayBase<impl Data<Elem = f64>, Ix2>,
         y_data: &ArrayBase<impl Data<Elem = f64>, Ix2>,
         sampling: &Lhs<f64, Xoshiro256Plus>,
@@ -1161,39 +1179,35 @@
 
     fn eval_infill_obj(
         &self,
         x: &[f64],
         obj_model: &dyn ClusteredSurrogate,
         f_min: f64,
         scale: f64,
-        scale_wb2: f64,
+        scale_ic: f64,
     ) -> f64 {
         let x_f = x.to_vec();
-        let obj = match self.infill {
-            InfillStrategy::EI => -ei(&x_f, obj_model, f_min),
-            InfillStrategy::WB2 => -wb2s(&x_f, obj_model, f_min, 1.),
-            InfillStrategy::WB2S => -wb2s(&x_f, obj_model, f_min, scale_wb2),
-        };
+        let obj = -(self
+            .infill_criterion
+            .value(&x_f, obj_model, f_min, Some(scale_ic)));
         obj / scale
     }
 
     pub fn eval_grad_infill_obj(
         &self,
         x: &[f64],
         obj_model: &dyn ClusteredSurrogate,
         f_min: f64,
         scale: f64,
-        scale_wb2: f64,
+        scale_ic: f64,
     ) -> Vec<f64> {
         let x_f = x.to_vec();
-        let grad = match self.infill {
-            InfillStrategy::EI => -grad_ei(&x_f, obj_model, f_min),
-            InfillStrategy::WB2 => -grad_wbs2(&x_f, obj_model, f_min, 1.),
-            InfillStrategy::WB2S => -grad_wbs2(&x_f, obj_model, f_min, scale_wb2),
-        };
+        let grad = -(self
+            .infill_criterion
+            .grad(&x_f, obj_model, f_min, Some(scale_ic)));
         (grad / scale).to_vec()
     }
 
     fn eval_obj<O: CostFunction<Param = Array2<f64>, Output = Array2<f64>>>(
         &self,
         pb: &mut Problem<O>,
         x: &Array2<f64>,
```

### Comparing `egobox-0.8.2/local_dependencies/egobox-ego/src/egor_state.rs` & `egobox-0.9.0/local_dependencies/egobox-ego/src/egor_state.rs`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/local_dependencies/egobox-ego/src/errors.rs` & `egobox-0.9.0/local_dependencies/egobox-ego/src/errors.rs`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/local_dependencies/egobox-ego/src/lhs_optimizer.rs` & `egobox-0.9.0/local_dependencies/egobox-ego/src/lhs_optimizer.rs`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/local_dependencies/egobox-ego/src/mixint.rs` & `egobox-0.9.0/local_dependencies/egobox-ego/src/mixint.rs`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/local_dependencies/egobox-ego/src/sort_axis.rs` & `egobox-0.9.0/local_dependencies/egobox-ego/src/sort_axis.rs`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/local_dependencies/egobox-ego/src/types.rs` & `egobox-0.9.0/local_dependencies/egobox-ego/src/types.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 use crate::errors::Result;
 use argmin::core::CostFunction;
 use egobox_moe::{ClusteredSurrogate, Clustering};
-use egobox_moe::{CorrelationSpec, RegressionSpec};
 use linfa::Float;
 use ndarray::{Array1, Array2, ArrayView2};
 use serde::{Deserialize, Serialize};
 
+/// Enums for regression and correlation selection
+pub use egobox_moe::{CorrelationSpec, RegressionSpec};
+
 /// Optimization result
 #[derive(Clone, Debug)]
 pub struct OptimResult<F: Float> {
     /// Optimum x value
     pub x_opt: Array1<F>,
     /// Optimum y value (e.g. f(x_opt))
     pub y_opt: Array1<F>,
```

### Comparing `egobox-0.8.2/local_dependencies/egobox-moe/Cargo.toml` & `egobox-0.9.0/local_dependencies/egobox-moe/Cargo.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "egobox-moe"
-version = "0.8.1"
+version = "0.9.0"
 authors = ["Rémi Lafage <remi.lafage@onera.fr>"]
 edition = "2018"
 description = "A library for mixture of expert gaussian processes"
 license = "Apache-2.0"
 repository = "https://github.com/relf/egobox"
 keywords = ["machine-learning", "mixture", "clustering", "surrogate", "gaussian-process"]
 categories = ["algorithms", "mathematics", "science"]
@@ -13,16 +13,16 @@
 default = []
 
 persistent = ["serializable", "serde_json"]
 serializable = ["serde", "typetag", "linfa-clustering/serde", "egobox-gp/serializable"]
 blas = ["ndarray-linalg", "linfa/ndarray-linalg", "linfa-clustering/blas", "linfa-pls/blas"]
 
 [dependencies]
-egobox-doe = { version = "0.8.1", path = "../egobox-doe" }
-egobox-gp = { version = "0.8.1", path = "../egobox-gp" }
+egobox-doe = { version = "0.9.0", path = "../egobox-doe" }
+egobox-gp = { version = "0.9.0", path = "../egobox-gp" }
 
 linfa = { version = "0.6.1", default-features = false }
 linfa-clustering = { version = "0.6.1", default-features = false }
 linfa-pls = { version = "0.6.1", default-features = false }
 linfa-linalg = { version = "0.1", default-features = false }
 
 ndarray = { version = "0.15", features = ["rayon", "approx"]}
```

### Comparing `egobox-0.8.2/local_dependencies/egobox-moe/README.md` & `egobox-0.9.0/local_dependencies/egobox-moe/README.md`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/local_dependencies/egobox-moe/benches/bench_find_nb_clusters.rs` & `egobox-0.9.0/local_dependencies/egobox-moe/benches/bench_find_nb_clusters.rs`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/local_dependencies/egobox-moe/examples/clustering.rs` & `egobox-0.9.0/local_dependencies/egobox-moe/examples/clustering.rs`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/local_dependencies/egobox-moe/examples/moe_norm1.rs` & `egobox-0.9.0/local_dependencies/egobox-moe/examples/moe_norm1.rs`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/local_dependencies/egobox-moe/examples/norm1.rs` & `egobox-0.9.0/local_dependencies/egobox-moe/examples/norm1.rs`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/local_dependencies/egobox-moe/examples/norm1_D2_200.csv` & `egobox-0.9.0/local_dependencies/egobox-moe/examples/norm1_D2_200.csv`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/local_dependencies/egobox-moe/src/algorithm.rs` & `egobox-0.9.0/local_dependencies/egobox-moe/src/algorithm.rs`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/local_dependencies/egobox-moe/src/clustering.rs` & `egobox-0.9.0/local_dependencies/egobox-moe/src/clustering.rs`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/local_dependencies/egobox-moe/src/errors.rs` & `egobox-0.9.0/local_dependencies/egobox-moe/src/errors.rs`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/local_dependencies/egobox-moe/src/expertise_macros.rs` & `egobox-0.9.0/local_dependencies/egobox-moe/src/expertise_macros.rs`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/local_dependencies/egobox-moe/src/gaussian_mixture.rs` & `egobox-0.9.0/local_dependencies/egobox-moe/src/gaussian_mixture.rs`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/local_dependencies/egobox-moe/src/lib.rs` & `egobox-0.9.0/local_dependencies/egobox-moe/src/lib.rs`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/local_dependencies/egobox-moe/src/parameters.rs` & `egobox-0.9.0/local_dependencies/egobox-moe/src/parameters.rs`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/local_dependencies/egobox-moe/src/surrogates.rs` & `egobox-0.9.0/local_dependencies/egobox-moe/src/surrogates.rs`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/local_dependencies/egobox-gp/README.md` & `egobox-0.9.0/local_dependencies/egobox-gp/README.md`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/local_dependencies/egobox-gp/benches/gp.rs` & `egobox-0.9.0/local_dependencies/egobox-gp/benches/gp.rs`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/local_dependencies/egobox-gp/examples/kriging.rs` & `egobox-0.9.0/local_dependencies/egobox-gp/examples/kriging.rs`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/local_dependencies/egobox-gp/src/algorithm.rs` & `egobox-0.9.0/local_dependencies/egobox-gp/src/algorithm.rs`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/local_dependencies/egobox-gp/src/correlation_models.rs` & `egobox-0.9.0/local_dependencies/egobox-gp/src/correlation_models.rs`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/local_dependencies/egobox-gp/src/errors.rs` & `egobox-0.9.0/local_dependencies/egobox-gp/src/errors.rs`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/local_dependencies/egobox-gp/src/lib.rs` & `egobox-0.9.0/local_dependencies/egobox-gp/src/lib.rs`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/local_dependencies/egobox-gp/src/mean_models.rs` & `egobox-0.9.0/local_dependencies/egobox-gp/src/mean_models.rs`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/local_dependencies/egobox-gp/src/parameters.rs` & `egobox-0.9.0/local_dependencies/egobox-gp/src/parameters.rs`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/local_dependencies/egobox-gp/src/utils.rs` & `egobox-0.9.0/local_dependencies/egobox-gp/src/utils.rs`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/local_dependencies/egobox-doe/Cargo.toml` & `egobox-0.9.0/local_dependencies/egobox-doe/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "egobox-doe"
-version = "0.8.1"
+version = "0.9.0"
 authors = ["Rémi Lafage <remi.lafage@onera.fr>"]
 edition = "2018"
 description = "A library for design of experiments"
 license = "Apache-2.0"
 repository = "https://github.com/relf/egobox"
 keywords = ["machine-learning", "design", "experiments", "lhs", "full-factorial"]
 categories = ["algorithms", "mathematics", "science"]
```

### Comparing `egobox-0.8.2/local_dependencies/egobox-doe/README.md` & `egobox-0.9.0/local_dependencies/egobox-doe/README.md`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/local_dependencies/egobox-doe/benches/lhs.rs` & `egobox-0.9.0/local_dependencies/egobox-doe/benches/lhs.rs`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/local_dependencies/egobox-doe/examples/samplings.rs` & `egobox-0.9.0/local_dependencies/egobox-doe/examples/samplings.rs`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/local_dependencies/egobox-doe/src/full_factorial.rs` & `egobox-0.9.0/local_dependencies/egobox-doe/src/full_factorial.rs`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/local_dependencies/egobox-doe/src/lhs.rs` & `egobox-0.9.0/local_dependencies/egobox-doe/src/lhs.rs`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/local_dependencies/egobox-doe/src/lib.rs` & `egobox-0.9.0/local_dependencies/egobox-doe/src/lib.rs`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/local_dependencies/egobox-doe/src/random.rs` & `egobox-0.9.0/local_dependencies/egobox-doe/src/random.rs`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/local_dependencies/egobox-doe/src/traits.rs` & `egobox-0.9.0/local_dependencies/egobox-doe/src/traits.rs`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/local_dependencies/egobox-doe/src/utils.rs` & `egobox-0.9.0/local_dependencies/egobox-doe/src/utils.rs`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/Cargo.toml` & `egobox-0.9.0/Cargo.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "egobox"
-version = "0.8.2"
+version = "0.9.0"
 authors = ["Rémi Lafage <remi.lafage@onera.fr>"]
 edition = "2018"
 description = "A toolbox for efficient global optimization"
 license = "Apache-2.0"
 repository = "https://github.com/relf/egobox"
 keywords = ["machine-learning", "doe", "gaussian-process", 
             "mixture-of-experts", "optimization"]
@@ -21,34 +21,34 @@
 
 serializable-gp = ["egobox-gp/serializable"]
 persistent-moe = ["egobox-moe/persistent"]
 persistent-ego = ["egobox-ego/persistent"]
 blas = ["ndarray/blas", "egobox-gp/blas", "egobox-moe/blas", "egobox-ego/blas"]
 
 [dependencies]
-egobox-doe = { version = "0.8.1", path= "local_dependencies/egobox-doe" }
-egobox-gp = { version = "0.8.1", path= "local_dependencies/egobox-gp" }
-egobox-moe = { version = "0.8.1", path= "local_dependencies/egobox-moe", features=["persistent"] }
-egobox-ego = { version = "0.8.2", path= "local_dependencies/egobox-ego", features=["persistent"] }
+egobox-doe = { version = "0.9.0", path= "local_dependencies/egobox-doe" }
+egobox-gp = { version = "0.9.0", path= "local_dependencies/egobox-gp" }
+egobox-moe = { version = "0.9.0", path= "local_dependencies/egobox-moe", features=["persistent"] }
+egobox-ego = { version = "0.9.0", path= "local_dependencies/egobox-ego", features=["persistent"] }
 
 linfa = { version = "0.6.1", default-features = false }
 
 ndarray = { version = "0.15", features = ["rayon", "approx"]}
 ndarray-rand = "0.14"
-numpy = "0.17"
+numpy = "0.18"
 anyhow = "1"
 rayon = "1"
 
 rand_xoshiro = "0.6"
 libm = "0.2"
 finitediff = { version="0.1.4", features = ["ndarray"] }
 env_logger = "0.10.0"
 log = "0.4"
-pyo3 = { version = "0.17", features = ["extension-module"] }
-pyo3-log = "0.7.0"
+pyo3 = { version = "0.18.0", features = ["extension-module"] }
+pyo3-log = "0.8"
 
 [dev-dependencies]
 criterion = "0.4"
 serde_json = "1"
 approx = "0.4"
 argmin_testfunctions = "0.1"
```

### Comparing `egobox-0.8.2/.gitignore` & `egobox-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/CHANGELOG.md` & `egobox-0.9.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,30 @@
 Changes
 -------
 
-Version 0.9.0 - unreleased
+Version 0.10.0 - unreleased
 ==========================
 
+Version 0.9.0 - 02/06/2023
+==========================
+
+* `ego`:
+    * Infill criterion is now a trait object in `EgorSolver` structure (#92)
+    * `Egor` and `EgorSolver` API: methods taking argument of type Option<T> now take argument of type T (#94)
+    * `EgorBuilder::min_within_mixed_space()` is now `EgorBuilder::min_within_mixint_space()` (#96)
+    * `egobox-ego` library doc updated (#95)
+
+* `egobox` Python binding: Upgrade to PyO3 0.18 (#91)
+
+Version 0.8.2 - 31/03/2023
+==========================
+
+* `ego`:
+   * Fix Egor solver best iter computation (#89)
+
 Version 0.8.1 - 28/03/2023
 ==========================
 
 * `ego`:
   * Make objective and constraints training in parallel (#86)
   * Lock mopta execution to allow concurrent computations (#84)
   * Fix and adjust infill criterion optimmization retries strategy (#87)
```

### Comparing `egobox-0.8.2/CONTRIBUTING.md` & `egobox-0.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/LICENSE` & `egobox-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/README.md` & `egobox-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,18 +24,18 @@
 
 ### Usage
 
 Depending on the sub-packages you want to use, you have to add following declarations to your `Cargo.toml`
 
 ```text
 [dependencies]
-egobox-doe = { version = "0.8.0" }
-egobox-gp  = { version = "0.8.0" }
-egobox-moe = { version = "0.8.0" }
-egobox-ego = { version = "0.8.0" }
+egobox-doe = { version = "0.9.0" }
+egobox-gp  = { version = "0.9.0" }
+egobox-moe = { version = "0.9.0" }
+egobox-ego = { version = "0.9.0" }
 ```
 
 ### Features
 #### `serializable-gp` 
 
 The `serializable-gp` feature enables the serialization of GP models using the [serde crate](https://serde.rs/). 
 
@@ -70,15 +70,15 @@
 As for `linfa`, the linear algebra routines used in `gp`, `moe` ad `ego` are provided by the pure-Rust [linfa-linalg](https://github.com/rust-ml/linfa-linalg) crate, the default linear algebra provider.
 
 Otherwise, you can choose an external BLAS/LAPACK backend available through the [ndarray-linalg](https://github.com/rust-ndarray/ndarray-linalg) crate. In this case, you have to specify the `blas` feature and a `linfa` [BLAS/LAPACK backend feature](https://github.com/rust-ml/linfa#blaslapack-backend) (more information in [linfa features](https://github.com/rust-ml/linfa#blaslapack-backend)).
 
 Thus, for instance, to use `gp` with the Intel MKL BLAS/LAPACK backend, you could specify in your `Cargo.toml` the following features:
 ```text
 [dependencies]
-egobox-gp = { version = "0.8.0", features = ["blas", "linfa/intel-mkl-static"] }
+egobox-gp = { version = "0.9.0", features = ["blas", "linfa/intel-mkl-static"] }
 ```
 or you could run the `gp` example as follows:
 ``` bash
 $ cd gp && cargo run --example kriging --release --features blas,linfa/intel-mkl-static
 ```
 
 ## The Python module
```

### Comparing `egobox-0.8.2/doc/Egor_Tutorial.ipynb` & `egobox-0.9.0/doc/Egor_Tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/doc/Gpx_MaunaLoaCO2.ipynb` & `egobox-0.9.0/doc/Gpx_MaunaLoaCO2.ipynb`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/doc/Gpx_Tutorial.ipynb` & `egobox-0.9.0/doc/Gpx_Tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/joss/egobox_architecture.png` & `egobox-0.9.0/joss/egobox_architecture.png`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/joss/paper.bib` & `egobox-0.9.0/joss/paper.bib`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/joss/paper.md` & `egobox-0.9.0/joss/paper.md`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/pyproject.toml` & `egobox-0.9.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 [tool.maturin]
 python-source="python"
 # Optional usage of BLAS backend 
 # cargo-extra-args = "--features linfa/intel-mkl-static"
 
 [tool.poetry]
 name = "egobox"
-version = "0.8.2"
+version = "0.9.0"
 description = "Python binding for egobox EGO optimizer written in Rust"
 authors = ["Rémi Lafage <remi.lafage@onera.fr>"]
 
 [tool.poetry.dependencies]
 numpy = ">=1.18"
 python = ">=3.7"
```

### Comparing `egobox-0.8.2/python/egobox/examples/kriging.py` & `egobox-0.9.0/python/egobox/examples/kriging.py`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/python/egobox/examples/optim_g24.py` & `egobox-0.9.0/python/egobox/examples/optim_g24.py`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/python/egobox/tests/test_egor.py` & `egobox-0.9.0/python/egobox/tests/test_egor.py`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/python/egobox/tests/test_gpmix.py` & `egobox-0.9.0/python/egobox/tests/test_gpmix.py`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/python/egobox/tests/test_mixintegor.py` & `egobox-0.9.0/python/egobox/tests/test_mixintegor.py`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/python/egobox/tests/test_utils.py` & `egobox-0.9.0/python/egobox/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/src/egor.rs` & `egobox-0.9.0/src/egor.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 //! `egobox`, Rust toolbox for efficient global optimization
 //!
 //! Thanks to the [PyO3 project](https://pyo3.rs), which makes Rust well suited for building Python extensions,
-//! the EGO algorithm written in Rust (aka `egor`) is binded in Python. You can install the Python package using:
+//! the EGO algorithm written in Rust (aka `Egor`) is binded in Python. You can install the Python package using:
 //!
 //! ```bash
 //! pip install egobox
 //! ```
 //!
-//! See the [tutorial notebook](https://github.com/relf/egobox/doc/TutorialEgor.ipynb) for usage.
+//! See the [tutorial notebook](https://github.com/relf/egobox/doc/Egor_Tutorial.ipynb) for usage.
 //!
 
 use crate::types::*;
 use egobox_doe::SamplingMethod;
 use numpy::ndarray::{Array2, ArrayView2};
 use numpy::{IntoPyArray, PyArray1, PyArray2, PyReadonlyArray2};
 use pyo3::exceptions::PyValueError;
@@ -190,35 +190,35 @@
     #[pyo3(get)]
     y_hist: Py<PyArray2<f64>>,
 }
 
 #[pymethods]
 impl Egor {
     #[new]
-    #[args(
+    #[pyo3(signature = (
         fun,
         xspecs,
-        n_cstr = "0",
-        cstr_tol = "1e-6",
-        n_start = "20",
-        n_doe = "0",
-        doe = "None",
-        regr_spec = "RegressionSpec::CONSTANT",
-        corr_spec = "CorrelationSpec::SQUARED_EXPONENTIAL",
-        infill_strategy = "InfillStrategy::WB2",
-        q_points = "1",
-        par_infill_strategy = "ParInfillStrategy::KB",
-        infill_optimizer = "InfillOptimizer::COBYLA",
-        kpls_dim = "None",
-        n_clusters = "1",
-        target = "f64::NEG_INFINITY",
-        outdir = "None",
-        hot_start = "false",
-        seed = "None"
-    )]
+        n_cstr = 0,
+        cstr_tol = 1e-6,
+        n_start = 20,
+        n_doe = 0,
+        doe = None,
+        regr_spec = RegressionSpec::CONSTANT,
+        corr_spec = CorrelationSpec::SQUARED_EXPONENTIAL,
+        infill_strategy = InfillStrategy::WB2,
+        q_points = 1,
+        par_infill_strategy = ParInfillStrategy::KB,
+        infill_optimizer = InfillOptimizer::COBYLA,
+        kpls_dim = None,
+        n_clusters = 1,
+        target = f64::NEG_INFINITY,
+        outdir = None,
+        hot_start = false,
+        seed = None
+    ))]
     #[allow(clippy::too_many_arguments)]
     fn new(
         py: Python,
         fun: PyObject,
         xspecs: PyObject,
         n_cstr: usize,
         cstr_tol: f64,
@@ -269,16 +269,15 @@
     ///         the iteration budget, number of fun calls is n_doe + q_points * n_iter.
     ///
     /// # Returns
     ///     optimization result
     ///         x_opt (array[1, nx]): x value  where fun is at its minimum subject to constraint
     ///         y_opt (array[1, nx]): fun(x_opt)
     ///
-    #[args(n_iter = "20")]
-    #[pyo3(text_signature = "(n_iter=20)")]
+    #[pyo3(signature = (n_iter = 20))]
     fn minimize(&self, py: Python, n_iter: usize) -> PyResult<OptimResult> {
         let fun = self.fun.to_object(py);
         let obj = move |x: &ArrayView2<f64>| -> Array2<f64> {
             Python::with_gil(|py| {
                 let args = (x.to_owned().into_pyarray(py),);
                 let res = fun.call1(py, args).unwrap();
                 let pyarray: &PyArray2<f64> = res.extract(py).unwrap();
@@ -300,16 +299,14 @@
         };
 
         let infill_optimizer = match self.infill_optimizer {
             InfillOptimizer::COBYLA => egobox_ego::InfillOptimizer::Cobyla,
             InfillOptimizer::SLSQP => egobox_ego::InfillOptimizer::Slsqp,
         };
 
-        let doe = self.doe.as_ref().map(|v| v.to_owned());
-
         let xspecs: Vec<XSpec> = self.xspecs.extract(py).expect("Error in xspecs conversion");
         if xspecs.is_empty() {
             panic!("Error: xspecs argument cannot be empty")
         }
 
         let xtypes: Vec<egobox_ego::XType> = xspecs
             .iter()
@@ -323,41 +320,48 @@
                     XType::FLOAT,
                     XType::INT,
                     i
                 ),
             })
             .collect();
 
-        let mut mixintegor = egobox_ego::EgorBuilder::optimize(obj);
-
+        let mut mixintegor_build = egobox_ego::EgorBuilder::optimize(obj);
         if let Some(seed) = self.seed {
-            mixintegor = mixintegor.random_seed(seed);
+            mixintegor_build = mixintegor_build.random_seed(seed);
         };
 
-        let mixintegor = mixintegor
-            .min_within_mixed_space(&xtypes)
+        let mut mixintegor = mixintegor_build
+            .min_within_mixint_space(&xtypes)
             .n_cstr(self.n_cstr)
             .n_iter(n_iter)
             .n_start(self.n_start)
             .n_doe(self.n_doe)
             .cstr_tol(self.cstr_tol)
-            .doe(doe)
             .regression_spec(egobox_moe::RegressionSpec::from_bits(self.regression_spec.0).unwrap())
             .correlation_spec(
                 egobox_moe::CorrelationSpec::from_bits(self.correlation_spec.0).unwrap(),
             )
             .infill_strategy(infill_strategy)
             .q_points(self.q_points)
             .qei_strategy(qei_strategy)
             .infill_optimizer(infill_optimizer)
-            .kpls_dim(self.kpls_dim)
-            .n_clusters(self.n_clusters)
             .target(self.target)
-            .outdir(self.outdir.as_ref().cloned())
             .hot_start(self.hot_start);
+        if let Some(doe) = self.doe.as_ref() {
+            mixintegor = mixintegor.doe(doe);
+        };
+        if let Some(kpls_dim) = self.kpls_dim {
+            mixintegor = mixintegor.kpls_dim(kpls_dim);
+        };
+        if let Some(n_clusters) = self.n_clusters {
+            mixintegor = mixintegor.n_clusters(n_clusters);
+        };
+        if let Some(outdir) = self.outdir.as_ref().cloned() {
+            mixintegor = mixintegor.outdir(outdir);
+        };
 
         let res = py.allow_threads(|| {
             mixintegor
                 .run()
                 .expect("Egor should optimize the objective function")
         });
         let x_opt = res.x_opt.into_pyarray(py).to_owned();
```

### Comparing `egobox-0.8.2/src/gpmix.rs` & `egobox-0.9.0/src/gpmix.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,33 @@
+//! `egobox`, Rust toolbox for efficient global optimization
+//!
+//! Thanks to the [PyO3 project](https://pyo3.rs), which makes Rust well suited for building Python extensions,
+//! the mixture of gaussian process surrogates is binded in Python. You can install the Python package using:
+//!
+//! ```bash
+//! pip install egobox
+//! ```
+//!
+//! See the [tutorial notebook](https://github.com/relf/egobox/doc/Gpx_Tutorial.ipynb) for usage.
+//!
 use crate::types::*;
 use egobox_moe::{Moe, Surrogate};
 use linfa::{traits::Fit, Dataset};
 use ndarray_rand::rand::SeedableRng;
 use numpy::{IntoPyArray, PyArray2, PyReadonlyArray2};
 use pyo3::prelude::*;
 use rand_xoshiro::Xoshiro256Plus;
 
 /// Gaussian processes mixture builder
 ///
 ///     n_clusters (int >= 0)
 ///         Number of clusters used by the mixture of surrogate experts.
 ///         When set to 0, the number of cluster is determined automatically and refreshed every
 ///         10-points addition (should say 'tentative addition' because addition may fail for some points
-///         but it is counted anyway).
+///         but failures are counted anyway).
 ///
 ///     regr_spec (RegressionSpec flags, an int in [1, 7]):
 ///         Specification of regression models used in mixture.
 ///         Can be RegressionSpec.CONSTANT (1), RegressionSpec.LINEAR (2), RegressionSpec.QUADRATIC (4) or
 ///         any bit-wise union of these values (e.g. RegressionSpec.CONSTANT | RegressionSpec.LINEAR)
 ///
 ///     corr_spec (CorrelationSpec flags, an int in [1, 15]):
@@ -50,22 +61,22 @@
     pub seed: Option<u64>,
     pub training_data: Option<Dataset<f64, f64>>,
 }
 
 #[pymethods]
 impl GpMix {
     #[new]
-    #[args(
-        n_clusters = "1",
-        regr_spec = "RegressionSpec::CONSTANT",
-        corr_spec = "CorrelationSpec::SQUARED_EXPONENTIAL",
-        recombination = "Recombination::Smooth",
-        kpls_dim = "None",
-        seed = "None"
-    )]
+    #[pyo3(signature = (
+        n_clusters = 1,
+        regr_spec = RegressionSpec::CONSTANT,
+        corr_spec = CorrelationSpec::SQUARED_EXPONENTIAL,
+        recombination = Recombination::Smooth,
+        kpls_dim = None,
+        seed = None
+    ))]
     #[allow(clippy::too_many_arguments)]
     fn new(
         n_clusters: usize,
         regr_spec: u8,
         corr_spec: u8,
         recombination: Recombination,
         kpls_dim: Option<usize>,
@@ -132,22 +143,22 @@
 
 #[pymethods]
 impl Gpx {
     /// Get Gaussian processes mixture builder aka `GpMix`
     ///
     /// See `GpMix` constructor
     #[staticmethod]
-    #[args(
-        n_clusters = "1",
-        regr_spec = "RegressionSpec::CONSTANT",
-        corr_spec = "CorrelationSpec::SQUARED_EXPONENTIAL",
-        recombination = "Recombination::Smooth",
-        kpls_dim = "None",
-        seed = "None"
-    )]
+    #[pyo3(signature = (
+        n_clusters = 1,
+        regr_spec = RegressionSpec::CONSTANT,
+        corr_spec = CorrelationSpec::SQUARED_EXPONENTIAL,
+        recombination = Recombination::Smooth,
+        kpls_dim = None,
+        seed = None
+    ))]
     fn builder(
         n_clusters: usize,
         regr_spec: u8,
         corr_spec: u8,
         recombination: Recombination,
         kpls_dim: Option<usize>,
         seed: Option<u64>,
```

### Comparing `egobox-0.8.2/src/lib.rs` & `egobox-0.9.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `egobox-0.8.2/src/types.rs` & `egobox-0.9.0/src/types.rs`

 * *Files 3% similar despite different names*

```diff
@@ -84,17 +84,20 @@
     #[pyo3(get)]
     pub(crate) tol: f64,
 }
 
 #[pymethods]
 impl ExpectedOptimum {
     #[new]
-    #[args(value, tolerance = "1e-6")]
-    fn new(val: f64, tol: f64) -> Self {
-        ExpectedOptimum { val, tol }
+    #[pyo3(signature = (value, tolerance = 1e-6))]
+    fn new(value: f64, tolerance: f64) -> Self {
+        ExpectedOptimum {
+            val: value,
+            tol: tolerance,
+        }
     }
 }
 
 #[pyclass]
 #[derive(Clone, Copy, Debug)]
 pub(crate) struct XType(pub(crate) u8);
```

### Comparing `egobox-0.8.2/PKG-INFO` & `egobox-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: egobox
-Version: 0.8.2
+Version: 0.9.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Rust
 Classifier: Topic :: Software Development
@@ -46,18 +46,18 @@
 
 ### Usage
 
 Depending on the sub-packages you want to use, you have to add following declarations to your `Cargo.toml`
 
 ```text
 [dependencies]
-egobox-doe = { version = "0.8.0" }
-egobox-gp  = { version = "0.8.0" }
-egobox-moe = { version = "0.8.0" }
-egobox-ego = { version = "0.8.0" }
+egobox-doe = { version = "0.9.0" }
+egobox-gp  = { version = "0.9.0" }
+egobox-moe = { version = "0.9.0" }
+egobox-ego = { version = "0.9.0" }
 ```
 
 ### Features
 #### `serializable-gp` 
 
 The `serializable-gp` feature enables the serialization of GP models using the [serde crate](https://serde.rs/). 
 
@@ -92,15 +92,15 @@
 As for `linfa`, the linear algebra routines used in `gp`, `moe` ad `ego` are provided by the pure-Rust [linfa-linalg](https://github.com/rust-ml/linfa-linalg) crate, the default linear algebra provider.
 
 Otherwise, you can choose an external BLAS/LAPACK backend available through the [ndarray-linalg](https://github.com/rust-ndarray/ndarray-linalg) crate. In this case, you have to specify the `blas` feature and a `linfa` [BLAS/LAPACK backend feature](https://github.com/rust-ml/linfa#blaslapack-backend) (more information in [linfa features](https://github.com/rust-ml/linfa#blaslapack-backend)).
 
 Thus, for instance, to use `gp` with the Intel MKL BLAS/LAPACK backend, you could specify in your `Cargo.toml` the following features:
 ```text
 [dependencies]
-egobox-gp = { version = "0.8.0", features = ["blas", "linfa/intel-mkl-static"] }
+egobox-gp = { version = "0.9.0", features = ["blas", "linfa/intel-mkl-static"] }
 ```
 or you could run the `gp` example as follows:
 ``` bash
 $ cd gp && cargo run --example kriging --release --features blas,linfa/intel-mkl-static
 ```
 
 ## The Python module
```


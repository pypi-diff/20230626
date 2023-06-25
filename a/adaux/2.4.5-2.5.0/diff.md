# Comparing `tmp/adaux-2.4.5.tar.gz` & `tmp/adaux-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adaux-2.4.5.tar", last modified: Fri Jun  9 12:50:40 2023, max compression
+gzip compressed data, was "adaux-2.5.0.tar", last modified: Sun Jun 25 23:31:03 2023, max compression
```

## Comparing `adaux-2.4.5.tar` & `adaux-2.5.0.tar`

### file list

```diff
@@ -1,151 +1,155 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 12:50:40.494532 adaux-2.4.5/
--rw-rw-rw-   0 root         (0) root         (0)     1059 2023-06-09 07:59:40.000000 adaux-2.4.5/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      314 2023-06-09 12:50:40.494532 adaux-2.4.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      974 2023-06-09 12:50:40.498532 adaux-2.4.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      144 2022-07-30 13:12:02.000000 adaux-2.4.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 12:50:40.370528 adaux-2.4.5/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 12:50:40.402529 adaux-2.4.5/source/adaux/
--rw-rw-rw-   0 root         (0) root         (0)      302 2023-06-09 12:17:23.000000 adaux-2.4.5/source/adaux/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      978 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/_base_parser.py
--rw-rw-rw-   0 root         (0) root         (0)    14267 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/_cli.py
--rw-rw-rw-   0 root         (0) root         (0)    14719 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/_cli_mixin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 12:50:40.426530 adaux-2.4.5/source/adaux/_components/
--rw-rw-rw-   0 root         (0) root         (0)      261 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/_components/_00_extra_level.py
--rw-rw-rw-   0 root         (0) root         (0)     4879 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/_components/_01_file_io_support.py
--rw-rw-rw-   0 root         (0) root         (0)     5076 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/_components/_02_base.py
--rw-rw-rw-   0 root         (0) root         (0)     3208 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/_components/_03_meta.py
--rw-rw-rw-   0 root         (0) root         (0)     1471 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/_components/_04_monotonic_version.py
--rw-rw-rw-   0 root         (0) root         (0)     6664 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/_components/_05_project.py
--rw-rw-rw-   0 root         (0) root         (0)     5033 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/_components/_06_dependency.py
--rw-rw-rw-   0 root         (0) root         (0)     1192 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/_components/_07_package.py
--rw-rw-rw-   0 root         (0) root         (0)     3686 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/_components/_08_pip.py
--rw-rw-rw-   0 root         (0) root         (0)     1888 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/_components/_09_gitignore.py
--rw-rw-rw-   0 root         (0) root         (0)     4135 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/_components/_10_gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)     5813 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/_components/_11_precommit.py
--rw-rw-rw-   0 root         (0) root         (0)     6494 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/_components/_12_pylint.py
--rw-rw-rw-   0 root         (0) root         (0)     1473 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/_components/_13_executable.py
--rw-rw-rw-   0 root         (0) root         (0)     2305 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/_components/_14_mypy.py
--rw-rw-rw-   0 root         (0) root         (0)     3025 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/_components/_15_pytest.py
--rw-rw-rw-   0 root         (0) root         (0)      340 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/_components/_16_coverage.py
--rw-rw-rw-   0 root         (0) root         (0)     2801 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/_components/_17_docs.py
--rw-rw-rw-   0 root         (0) root         (0)    20260 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/_components/_18_payload.py
--rw-rw-rw-   0 root         (0) root         (0)    16664 2023-06-09 12:25:02.000000 adaux-2.4.5/source/adaux/_components/_19_docker.py
--rw-rw-rw-   0 root         (0) root         (0)    11985 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/_components/_20_ci.py
--rw-rw-rw-   0 root         (0) root         (0)     3637 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/_components/_98_sentinel.py
--rw-rw-rw-   0 root         (0) root         (0)     1221 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/_components/_99_all.py
--rw-rw-rw-   0 root         (0) root         (0)      215 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/_components/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12673 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/_components/_aux_ci.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 12:50:40.434530 adaux-2.4.5/source/adaux/_components/_payload/
--rw-rw-rw-   0 root         (0) root         (0)      683 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/_components/_payload/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      530 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/_components/_payload/_base.py
--rw-rw-rw-   0 root         (0) root         (0)     1618 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/_components/_payload/_docker.py
--rw-rw-rw-   0 root         (0) root         (0)     1141 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/_components/_payload/_docker_build.py
--rw-rw-rw-   0 root         (0) root         (0)      382 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/_components/_payload/_docker_compose.py
--rw-rw-rw-   0 root         (0) root         (0)    15887 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/_components/_payload/_docker_executors.py
--rw-rw-rw-   0 root         (0) root         (0)      490 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/_components/_payload/_docker_run.py
--rw-rw-rw-   0 root         (0) root         (0)     1450 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/_components/_payload/_python.py
--rw-rw-rw-   0 root         (0) root         (0)     1323 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/_components/_payload/_with_dependency.py
--rwxrwxrwx   0 root         (0) root         (0)     1629 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/_create_badge.py
--rw-rw-rw-   0 root         (0) root         (0)    14742 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/_gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)      107 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/_logging.py
--rw-rw-rw-   0 root         (0) root         (0)     7090 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     1245 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/_proto_namespace.py
--rw-rw-rw-   0 root         (0) root         (0)     2513 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/_tick.py
--rw-rw-rw-   0 root         (0) root         (0)     3414 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/_todo.py
--rw-rw-rw-   0 root         (0) root         (0)     2751 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/_util.py
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/_yaml.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 12:50:40.434530 adaux-2.4.5/source/adaux/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 12:50:40.434530 adaux-2.4.5/source/adaux/src/CI/
--rw-rw-rw-   0 root         (0) root         (0)     2316 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/CI/00-main.yml.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      922 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/CI/01-rules.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 12:50:40.438530 adaux-2.4.5/source/adaux/src/CI/jinja-snippets/
--rw-rw-rw-   0 root         (0) root         (0)       50 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/CI/jinja-snippets/coverage.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       94 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/CI/jinja-snippets/tags.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 12:50:40.438530 adaux-2.4.5/source/adaux/src/docker/
--rw-rw-rw-   0 root         (0) root         (0)      417 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/docker/comp-helper.sh.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 12:50:40.382528 adaux-2.4.5/source/adaux/src/docker/services/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 12:50:40.438530 adaux-2.4.5/source/adaux/src/docker/services/ansible-deploy/
--rw-rw-rw-   0 root         (0) root         (0)      914 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/docker/services/ansible-deploy/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      547 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/docker/services/ansible-deploy/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 12:50:40.442530 adaux-2.4.5/source/adaux/src/docker/services/docs/
--rw-rw-rw-   0 root         (0) root         (0)     1688 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/docker/services/docs/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      459 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/docker/services/docs/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 12:50:40.442530 adaux-2.4.5/source/adaux/src/docker/services/gitlab-release-run/
--rw-rw-rw-   0 root         (0) root         (0)      608 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/docker/services/gitlab-release-run/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 12:50:40.446530 adaux-2.4.5/source/adaux/src/docker/services/image/
--rw-rw-rw-   0 root         (0) root         (0)     1564 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/docker/services/image/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      407 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/docker/services/image/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 12:50:40.446530 adaux-2.4.5/source/adaux/src/docker/services/image-pytest/
--rw-rw-rw-   0 root         (0) root         (0)      617 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/docker/services/image-pytest/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      415 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/docker/services/image-pytest/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 12:50:40.458531 adaux-2.4.5/source/adaux/src/docker/services/jinja-snippets/
--rw-rw-rw-   0 root         (0) root         (0)      505 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/docker/services/jinja-snippets/apt_install.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       87 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/docker/services/jinja-snippets/apt_install_root.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/docker/services/jinja-snippets/base_arg.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      529 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/docker/services/jinja-snippets/docker-build.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      169 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/docker/services/jinja-snippets/extra_script.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      437 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/docker/services/jinja-snippets/macros.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      326 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/docker/services/jinja-snippets/pip_install.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/docker/services/jinja-snippets/platform.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      247 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/docker/services/jinja-snippets/pytest_command.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       58 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/docker/services/jinja-snippets/sdist_untar.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 12:50:40.458531 adaux-2.4.5/source/adaux/src/docker/services/pkg-gitlab/
--rw-rw-rw-   0 root         (0) root         (0)      547 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/docker/services/pkg-gitlab/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 12:50:40.458531 adaux-2.4.5/source/adaux/src/docker/services/pkg-pypi/
--rw-rw-rw-   0 root         (0) root         (0)      485 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/docker/services/pkg-pypi/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 12:50:40.462531 adaux-2.4.5/source/adaux/src/docker/services/pre-commit/
--rw-rw-rw-   0 root         (0) root         (0)     1176 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/docker/services/pre-commit/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      544 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/docker/services/pre-commit/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 12:50:40.462531 adaux-2.4.5/source/adaux/src/docker/services/pycov/
--rw-rw-rw-   0 root         (0) root         (0)      482 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/docker/services/pycov/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 12:50:40.462531 adaux-2.4.5/source/adaux/src/docker/services/pytest/
--rw-rw-rw-   0 root         (0) root         (0)      342 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/docker/services/pytest/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      409 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/docker/services/pytest/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 12:50:40.466531 adaux-2.4.5/source/adaux/src/docker/services/pytest-standalone/
--rw-rw-rw-   0 root         (0) root         (0)      569 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/docker/services/pytest-standalone/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      409 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/docker/services/pytest-standalone/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 12:50:40.466531 adaux-2.4.5/source/adaux/src/docker/services/python-deps/
--rw-rw-rw-   0 root         (0) root         (0)      648 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/docker/services/python-deps/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      211 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/docker/services/python-deps/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 12:50:40.466531 adaux-2.4.5/source/adaux/src/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4843 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/docs/default_conf.py.jinja2
--rwxrwxrwx   0 root         (0) root         (0)     1873 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/docs/postprocess_html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 12:50:40.466531 adaux-2.4.5/source/adaux/src/docs/static/
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/docs/static/git-link-color.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 12:50:40.470531 adaux-2.4.5/source/adaux/src/docs/user/
--rw-rw-rw-   0 root         (0) root         (0)      468 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/docs/user/conf.py.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       45 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/docs/user/gitignore
--rw-rw-rw-   0 root         (0) root         (0)      283 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/docs/user/index.rst.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       74 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/gitignore
--rwxrwxrwx   0 root         (0) root         (0)      410 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/install-dev.sh.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 12:50:40.470531 adaux-2.4.5/source/adaux/src/license/
--rw-rw-rw-   0 root         (0) root         (0)      591 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/license/Apache-2.0.txt.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1495 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/license/BSD-3_clause.txt.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1090 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/license/MIT.txt.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 12:50:40.382528 adaux-2.4.5/source/adaux/src/payload/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 12:50:40.474531 adaux-2.4.5/source/adaux/src/payload/python/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 12:50:40.474531 adaux-2.4.5/source/adaux/src/payload/python/__pycache__/
--rw-r--r--   0 root         (0) root         (0)     2530 2023-06-09 12:49:37.000000 adaux-2.4.5/source/adaux/src/payload/python/__pycache__/functions.cpython-310.pyc
--rw-rw-rw-   0 root         (0) root         (0)     3046 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/payload/python/functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 12:50:40.474531 adaux-2.4.5/source/adaux/src/pip/
--rw-rw-rw-   0 root         (0) root         (0)      160 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/pip/pip.conf.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 12:50:40.478531 adaux-2.4.5/source/adaux/src/pre-commit/
--rwxrwxrwx   0 root         (0) root         (0)     1680 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/pre-commit/add_copy_right.py.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     5098 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/pre-commit/config.yaml.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/pre-commit/mypy.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 12:50:40.478531 adaux-2.4.5/source/adaux/src/root/
--rw-rw-rw-   0 root         (0) root         (0)      144 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/root/_setup.py
--rw-rw-rw-   0 root         (0) root         (0)      146 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/root/gitignore.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      487 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/root/setup.cfg.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 12:50:40.494532 adaux-2.4.5/source/adaux/src/root/source/
--rw-rw-rw-   0 root         (0) root         (0)      126 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/root/source/gitignore.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-06-09 07:59:41.000000 adaux-2.4.5/source/adaux/src/temp-combination
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 12:50:40.410529 adaux-2.4.5/source/adaux.egg-info/
--rw-r--r--   0 root         (0) root         (0)      314 2023-06-09 12:50:40.000000 adaux-2.4.5/source/adaux.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5236 2023-06-09 12:50:40.000000 adaux-2.4.5/source/adaux.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 12:50:40.000000 adaux-2.4.5/source/adaux.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-06-09 12:50:40.000000 adaux-2.4.5/source/adaux.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 12:49:36.000000 adaux-2.4.5/source/adaux.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      203 2023-06-09 12:50:40.000000 adaux-2.4.5/source/adaux.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-06-09 12:50:40.000000 adaux-2.4.5/source/adaux.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.471931 adaux-2.5.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1059 2023-06-09 07:59:40.000000 adaux-2.5.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      314 2023-06-25 23:31:03.471931 adaux-2.5.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      974 2023-06-25 23:31:03.475932 adaux-2.5.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      144 2022-07-30 13:12:02.000000 adaux-2.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.127919 adaux-2.5.0/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.239923 adaux-2.5.0/source/adaux/
+-rw-rw-rw-   0 root         (0) root         (0)      302 2023-06-25 21:24:58.000000 adaux-2.5.0/source/adaux/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      978 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_base_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)    14267 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    14719 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_cli_mixin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.319926 adaux-2.5.0/source/adaux/_components/
+-rw-rw-rw-   0 root         (0) root         (0)      261 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_00_extra_level.py
+-rw-rw-rw-   0 root         (0) root         (0)     4879 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_01_file_io_support.py
+-rw-rw-rw-   0 root         (0) root         (0)     5076 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_02_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3208 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_03_meta.py
+-rw-rw-rw-   0 root         (0) root         (0)     1471 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_04_monotonic_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     6664 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_05_project.py
+-rw-rw-rw-   0 root         (0) root         (0)     5033 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_06_dependency.py
+-rw-rw-rw-   0 root         (0) root         (0)     1192 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_07_package.py
+-rw-rw-rw-   0 root         (0) root         (0)     3686 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_08_pip.py
+-rw-rw-rw-   0 root         (0) root         (0)     1888 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_09_gitignore.py
+-rw-rw-rw-   0 root         (0) root         (0)     4211 2023-06-25 21:32:20.000000 adaux-2.5.0/source/adaux/_components/_10_gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)     5813 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_11_precommit.py
+-rw-rw-rw-   0 root         (0) root         (0)     6494 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_12_pylint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1473 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_13_executable.py
+-rw-rw-rw-   0 root         (0) root         (0)     2305 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_14_mypy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3025 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_15_pytest.py
+-rw-rw-rw-   0 root         (0) root         (0)      340 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_16_coverage.py
+-rw-rw-rw-   0 root         (0) root         (0)     2801 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_17_docs.py
+-rw-rw-rw-   0 root         (0) root         (0)    20260 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_18_payload.py
+-rw-rw-rw-   0 root         (0) root         (0)    17195 2023-06-25 23:21:24.000000 adaux-2.5.0/source/adaux/_components/_19_docker.py
+-rw-rw-rw-   0 root         (0) root         (0)    11985 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_20_ci.py
+-rw-rw-rw-   0 root         (0) root         (0)     3637 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_98_sentinel.py
+-rw-rw-rw-   0 root         (0) root         (0)     1221 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_99_all.py
+-rw-rw-rw-   0 root         (0) root         (0)      215 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12673 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_aux_ci.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.339927 adaux-2.5.0/source/adaux/_components/_payload/
+-rw-rw-rw-   0 root         (0) root         (0)      683 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_payload/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      530 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_payload/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1618 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_payload/_docker.py
+-rw-rw-rw-   0 root         (0) root         (0)     1141 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_payload/_docker_build.py
+-rw-rw-rw-   0 root         (0) root         (0)      382 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_payload/_docker_compose.py
+-rw-rw-rw-   0 root         (0) root         (0)    15864 2023-06-25 22:36:13.000000 adaux-2.5.0/source/adaux/_components/_payload/_docker_executors.py
+-rw-rw-rw-   0 root         (0) root         (0)      564 2023-06-25 22:36:13.000000 adaux-2.5.0/source/adaux/_components/_payload/_docker_run.py
+-rw-rw-rw-   0 root         (0) root         (0)     1450 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_payload/_python.py
+-rw-rw-rw-   0 root         (0) root         (0)     1323 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_components/_payload/_with_dependency.py
+-rwxrwxrwx   0 root         (0) root         (0)     1629 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_create_badge.py
+-rw-rw-rw-   0 root         (0) root         (0)    14742 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     7090 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     1245 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_proto_namespace.py
+-rw-rw-rw-   0 root         (0) root         (0)     2513 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_tick.py
+-rw-rw-rw-   0 root         (0) root         (0)     3414 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_todo.py
+-rw-rw-rw-   0 root         (0) root         (0)     2751 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_util.py
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/_yaml.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.343927 adaux-2.5.0/source/adaux/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.351927 adaux-2.5.0/source/adaux/src/CI/
+-rw-rw-rw-   0 root         (0) root         (0)     2316 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/CI/00-main.yml.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      922 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/CI/01-rules.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.355927 adaux-2.5.0/source/adaux/src/CI/jinja-snippets/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/CI/jinja-snippets/coverage.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       94 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/CI/jinja-snippets/tags.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.359927 adaux-2.5.0/source/adaux/src/docker/
+-rw-rw-rw-   0 root         (0) root         (0)      417 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/comp-helper.sh.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.171920 adaux-2.5.0/source/adaux/src/docker/services/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.371928 adaux-2.5.0/source/adaux/src/docker/services/ansible-deploy/
+-rw-rw-rw-   0 root         (0) root         (0)      599 2023-06-25 21:24:58.000000 adaux-2.5.0/source/adaux/src/docker/services/ansible-deploy/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      414 2023-06-25 23:21:24.000000 adaux-2.5.0/source/adaux/src/docker/services/ansible-deploy/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.371928 adaux-2.5.0/source/adaux/src/docker/services/ansible-deploy-ext/
+-rw-rw-rw-   0 root         (0) root         (0)      258 2023-06-25 23:21:24.000000 adaux-2.5.0/source/adaux/src/docker/services/ansible-deploy-ext/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.379928 adaux-2.5.0/source/adaux/src/docker/services/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     1688 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/docs/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      459 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/docs/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.379928 adaux-2.5.0/source/adaux/src/docker/services/gitlab-release-run/
+-rw-rw-rw-   0 root         (0) root         (0)      608 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/gitlab-release-run/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.383928 adaux-2.5.0/source/adaux/src/docker/services/image/
+-rw-rw-rw-   0 root         (0) root         (0)     1760 2023-06-25 21:24:58.000000 adaux-2.5.0/source/adaux/src/docker/services/image/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      642 2023-06-25 21:24:58.000000 adaux-2.5.0/source/adaux/src/docker/services/image/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.383928 adaux-2.5.0/source/adaux/src/docker/services/image-pytest/
+-rw-rw-rw-   0 root         (0) root         (0)      617 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/image-pytest/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      415 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/image-pytest/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.407929 adaux-2.5.0/source/adaux/src/docker/services/jinja-snippets/
+-rw-rw-rw-   0 root         (0) root         (0)      354 2023-06-25 21:24:58.000000 adaux-2.5.0/source/adaux/src/docker/services/jinja-snippets/ansible_deploy.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      184 2023-06-25 23:21:24.000000 adaux-2.5.0/source/adaux/src/docker/services/jinja-snippets/ansible_env.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      505 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/jinja-snippets/apt_install.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/jinja-snippets/apt_install_root.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/jinja-snippets/base_arg.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      529 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/jinja-snippets/docker-build.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      169 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/jinja-snippets/extra_script.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      571 2023-06-25 23:21:24.000000 adaux-2.5.0/source/adaux/src/docker/services/jinja-snippets/macros.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      326 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/jinja-snippets/pip_install.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/jinja-snippets/platform.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      247 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/jinja-snippets/pytest_command.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/jinja-snippets/sdist_untar.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.411929 adaux-2.5.0/source/adaux/src/docker/services/pkg-gitlab/
+-rw-rw-rw-   0 root         (0) root         (0)      547 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/pkg-gitlab/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.415929 adaux-2.5.0/source/adaux/src/docker/services/pkg-pypi/
+-rw-rw-rw-   0 root         (0) root         (0)      485 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/pkg-pypi/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.419929 adaux-2.5.0/source/adaux/src/docker/services/pre-commit/
+-rw-rw-rw-   0 root         (0) root         (0)     1176 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/pre-commit/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      544 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/pre-commit/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.419929 adaux-2.5.0/source/adaux/src/docker/services/pycov/
+-rw-rw-rw-   0 root         (0) root         (0)      482 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/pycov/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.427930 adaux-2.5.0/source/adaux/src/docker/services/pytest/
+-rw-rw-rw-   0 root         (0) root         (0)      342 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/pytest/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      409 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/pytest/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.431930 adaux-2.5.0/source/adaux/src/docker/services/pytest-standalone/
+-rw-rw-rw-   0 root         (0) root         (0)      569 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/pytest-standalone/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      409 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/pytest-standalone/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.435930 adaux-2.5.0/source/adaux/src/docker/services/python-deps/
+-rw-rw-rw-   0 root         (0) root         (0)      648 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/python-deps/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      211 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docker/services/python-deps/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.439930 adaux-2.5.0/source/adaux/src/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4843 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docs/default_conf.py.jinja2
+-rwxrwxrwx   0 root         (0) root         (0)     1873 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docs/postprocess_html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.439930 adaux-2.5.0/source/adaux/src/docs/static/
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docs/static/git-link-color.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.443930 adaux-2.5.0/source/adaux/src/docs/user/
+-rw-rw-rw-   0 root         (0) root         (0)      468 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docs/user/conf.py.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       45 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docs/user/gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      283 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/docs/user/index.rst.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       74 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/gitignore
+-rwxrwxrwx   0 root         (0) root         (0)      410 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/install-dev.sh.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.447930 adaux-2.5.0/source/adaux/src/license/
+-rw-rw-rw-   0 root         (0) root         (0)      591 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/license/Apache-2.0.txt.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1495 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/license/BSD-3_clause.txt.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/license/MIT.txt.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.187921 adaux-2.5.0/source/adaux/src/payload/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.447930 adaux-2.5.0/source/adaux/src/payload/python/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.447930 adaux-2.5.0/source/adaux/src/payload/python/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)     2530 2023-06-25 23:29:48.000000 adaux-2.5.0/source/adaux/src/payload/python/__pycache__/functions.cpython-310.pyc
+-rw-rw-rw-   0 root         (0) root         (0)     3046 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/payload/python/functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.447930 adaux-2.5.0/source/adaux/src/pip/
+-rw-rw-rw-   0 root         (0) root         (0)      160 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/pip/pip.conf.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.459931 adaux-2.5.0/source/adaux/src/pre-commit/
+-rwxrwxrwx   0 root         (0) root         (0)     1680 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/pre-commit/add_copy_right.py.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     5098 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/pre-commit/config.yaml.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/pre-commit/mypy.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.467931 adaux-2.5.0/source/adaux/src/root/
+-rw-rw-rw-   0 root         (0) root         (0)      144 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/root/_setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      146 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/root/gitignore.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      487 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/root/setup.cfg.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.471931 adaux-2.5.0/source/adaux/src/root/source/
+-rw-rw-rw-   0 root         (0) root         (0)      126 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/root/source/gitignore.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-06-09 07:59:41.000000 adaux-2.5.0/source/adaux/src/temp-combination
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:31:03.263924 adaux-2.5.0/source/adaux.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      314 2023-06-25 23:31:02.000000 adaux-2.5.0/source/adaux.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5451 2023-06-25 23:31:03.000000 adaux-2.5.0/source/adaux.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-25 23:31:02.000000 adaux-2.5.0/source/adaux.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-06-25 23:31:02.000000 adaux-2.5.0/source/adaux.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-25 23:29:46.000000 adaux-2.5.0/source/adaux.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      203 2023-06-25 23:31:02.000000 adaux-2.5.0/source/adaux.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-25 23:31:02.000000 adaux-2.5.0/source/adaux.egg-info/top_level.txt
```

### Comparing `adaux-2.4.5/LICENSE.txt` & `adaux-2.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/setup.cfg` & `adaux-2.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/_base_parser.py` & `adaux-2.5.0/source/adaux/_base_parser.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/_cli.py` & `adaux-2.5.0/source/adaux/_cli.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/_cli_mixin.py` & `adaux-2.5.0/source/adaux/_cli_mixin.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/_components/_01_file_io_support.py` & `adaux-2.5.0/source/adaux/_components/_01_file_io_support.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/_components/_02_base.py` & `adaux-2.5.0/source/adaux/_components/_02_base.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/_components/_03_meta.py` & `adaux-2.5.0/source/adaux/_components/_03_meta.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/_components/_04_monotonic_version.py` & `adaux-2.5.0/source/adaux/_components/_04_monotonic_version.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/_components/_05_project.py` & `adaux-2.5.0/source/adaux/_components/_05_project.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/_components/_06_dependency.py` & `adaux-2.5.0/source/adaux/_components/_06_dependency.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/_components/_07_package.py` & `adaux-2.5.0/source/adaux/_components/_07_package.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/_components/_08_pip.py` & `adaux-2.5.0/source/adaux/_components/_08_pip.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/_components/_09_gitignore.py` & `adaux-2.5.0/source/adaux/_components/_09_gitignore.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/_components/_10_gitlab.py` & `adaux-2.5.0/source/adaux/_components/_10_gitlab.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,15 @@
         # https://docs.gitlab.com/ee/api/protected_branches.html
         default_branch_settings = {
             (False, False): dict(
                 allow_force_push=True, push_access_level=30, merge_access_level=30
             ),
             (True, False): dict(push_access_level=0, merge_access_level=30),
             (False, True): dict(push_access_level=0, merge_access_level=40),
+            (True, True): dict(push_access_level=0, merge_access_level=40),
         }
         for key, val in data.vip_branches.items():
             mark = (key == data.default_branch, key == data.release_branch)
             for skey, sval in default_branch_settings[mark].items():
                 val.setdefault(skey, sval)
 
         if "remote_user" in data and "remote_url" in data:
```

### Comparing `adaux-2.4.5/source/adaux/_components/_11_precommit.py` & `adaux-2.5.0/source/adaux/_components/_11_precommit.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/_components/_12_pylint.py` & `adaux-2.5.0/source/adaux/_components/_12_pylint.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/_components/_13_executable.py` & `adaux-2.5.0/source/adaux/_components/_13_executable.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/_components/_14_mypy.py` & `adaux-2.5.0/source/adaux/_components/_14_mypy.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/_components/_15_pytest.py` & `adaux-2.5.0/source/adaux/_components/_15_pytest.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/_components/_17_docs.py` & `adaux-2.5.0/source/adaux/_components/_17_docs.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/_components/_18_payload.py` & `adaux-2.5.0/source/adaux/_components/_18_payload.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/_components/_19_docker.py` & `adaux-2.5.0/source/adaux/_components/_19_docker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Copyright (c) 2021-2023 Mario S. Könz; License: MIT
 # pylint: disable=too-many-lines
 import typing as tp
 
+from .._logging import logger
 from .._parser import Jinja2Parser
 from .._parser import YamlParser
 from .._proto_namespace import _ProtoNamespace
 from ._03_meta import MetaMixin
 from ._05_project import ProjectMixin
 from ._06_dependency import DependencyMixin
 from ._18_payload import PayloadMixin
@@ -139,15 +140,15 @@
             self._adjust_base_on_match_entry(param, self.auxe)
 
             param.setdefault("apt_req", {})
 
             self._set_name_and_version(param, name)
 
             if "mode" in param:
-                supported = ["django", "django+nginx"]
+                supported = ["django", "django+nginx", "ansible"]
                 if param.mode not in supported:
                     raise RuntimeError(
                         f"mode {param.mode} is not supported {supported}"
                     )
 
             # branch matching and dep settings
             fallback = extra_req_default.get(param.docker_name, [])
@@ -323,14 +324,27 @@
 
     def _update_config(
         self,
         payload: _ProtoNamespace,
         custom_services: _ProtoNamespace,
         config: _ProtoNamespace,
     ) -> None:
+        opts = payload.param
+
+        if (
+            opts.docker_name not in custom_services
+            and opts.docker_name not in config["services"]
+        ):
+            if opts.services == [opts.service_name]:
+                raise RuntimeError(f"could not find service {opts.docker_name}")
+            logger.debug(
+                "%s found no match, but is accepted as a collection of services: %s",
+                opts.docker_name,
+                opts.services,
+            )
         for service_name, val in custom_services.items():
             for key in list(val):
                 if payload.flavor == "docker_build":
                     if key not in ["build", "image"]:
                         del val[key]
                 elif payload.flavor == "docker_run":
                     if key in ["build"]:
```

### Comparing `adaux-2.4.5/source/adaux/_components/_20_ci.py` & `adaux-2.5.0/source/adaux/_components/_20_ci.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/_components/_98_sentinel.py` & `adaux-2.5.0/source/adaux/_components/_98_sentinel.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/_components/_99_all.py` & `adaux-2.5.0/source/adaux/_components/_99_all.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/_components/_aux_ci.py` & `adaux-2.5.0/source/adaux/_components/_aux_ci.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/_components/_payload/__init__.py` & `adaux-2.5.0/source/adaux/_components/_payload/__init__.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/_components/_payload/_base.py` & `adaux-2.5.0/source/adaux/_components/_payload/_base.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/_components/_payload/_docker.py` & `adaux-2.5.0/source/adaux/_components/_payload/_docker.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/_components/_payload/_docker_build.py` & `adaux-2.5.0/source/adaux/_components/_payload/_docker_build.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/_components/_payload/_docker_executors.py` & `adaux-2.5.0/source/adaux/_components/_payload/_docker_executors.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from ..._logging import logger
 
 
 @dc.dataclass(frozen=True)
 class DockerShared:
     slug: str
     parents: tp.Tuple["DockerShared", ...] = tuple()
+    images: tp.List[str] = dc.field(default_factory=list)
 
     # Run local registry:
     # docker run -d -p 5000:5000 --name registry registry:2
     # docker container stop registry && docker container rm -v registry
     # export CI_REGISTRY=localhost:5000
     @property
     def registry_host(self) -> str:
@@ -58,43 +59,48 @@
                     tag_image(remote_tag, job.local_tag)
 
             # I tag every time as it allows different dependencies to
             # map to the same service name without raising issues
             # (useful for local development)
             tag_image(job.local_tag, job.use_tag)
 
+        # download other images which are not a direct dependency (cross-repo)
+        for image_tag in self.images:
+            image_remote_tag = (
+                f"{self.registry_host}/{self._remove_namespace_local(image_tag)}"
+            )
+            check_and_pull_if_not_existent(image_remote_tag, image_tag)
+
     def _get_tag_parts(self) -> tp.Iterator[tp.Union[bytes, str]]:
         for job in self.build_deps:
             yield job.tag
 
+    def _remove_namespace_local(self, image: str) -> str:
+        if self.registry_host.startswith("localhost"):
+            return image.rsplit("/", 1)[1]
+        return image
+
 
 @dc.dataclass(frozen=True)
 class _DockerBuildMixinState:
     service: str
     image_name: str
 
 
 @dc.dataclass(frozen=True)
 class DockerBuildMixin(DockerShared, _DockerBuildMixinState):
-    images: tp.List[str] = dc.field(default_factory=list)
     files: tp.List[str] = dc.field(default_factory=list)
     always_build: bool = False
 
     def script(self) -> None:
         super().script()
         local_tag = self.local_tag
         if self.remote_exists():
             remote_tag = self.remote_tag
             check_and_pull_if_not_existent(remote_tag, local_tag, self.service)
-            # download other images which are not a direct dependency (cross-repo)
-            for image_tag in self.images:
-                image_remote_tag = (
-                    f"{self.registry_host}/{self._remove_namespace_local(image_tag)}"
-                )
-                check_and_pull_if_not_existent(image_remote_tag, image_tag)
 
         if not exists_locally(self.local_tag) or self.always_build:
             cmd = [
                 "docker",
                 "--log-level",
                 "ERROR",
                 "compose",
@@ -169,19 +175,14 @@
         return headers, url
 
     def is_up_to_date(self) -> bool:
         if self.remote_exists():
             return self.exists_remotely()
         return exists_locally(self.local_tag)
 
-    def _remove_namespace_local(self, image: str) -> str:
-        if self.registry_host.startswith("localhost"):
-            return image.rsplit("/", 1)[1]
-        return image
-
     def exists_remotely(self) -> bool:
         headers, api_url = self._docker_registry_header_and_url(self.get_image_name())
         try:
             req = requests.get(
                 api_url + f"/{self.get_image_name()}/tags/list",
                 headers=headers,
                 timeout=10,
```

### Comparing `adaux-2.4.5/source/adaux/_components/_payload/_python.py` & `adaux-2.5.0/source/adaux/_components/_payload/_python.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/_components/_payload/_with_dependency.py` & `adaux-2.5.0/source/adaux/_components/_payload/_with_dependency.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/_create_badge.py` & `adaux-2.5.0/source/adaux/_create_badge.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/_gitlab.py` & `adaux-2.5.0/source/adaux/_gitlab.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/_parser.py` & `adaux-2.5.0/source/adaux/_parser.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/_proto_namespace.py` & `adaux-2.5.0/source/adaux/_proto_namespace.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/_tick.py` & `adaux-2.5.0/source/adaux/_tick.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/_todo.py` & `adaux-2.5.0/source/adaux/_todo.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/_util.py` & `adaux-2.5.0/source/adaux/_util.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/src/CI/00-main.yml.jinja2` & `adaux-2.5.0/source/adaux/src/CI/00-main.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/src/CI/01-rules.yml.jinja2` & `adaux-2.5.0/source/adaux/src/CI/01-rules.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/src/docker/services/ansible-deploy/docker-compose.yml.jinja2` & `adaux-2.5.0/source/adaux/src/docker/services/image/docker-compose.yml.jinja2`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 version: '3.6'
 {% import "macros.jinja2" as x %}
 services:
     {{ opts.service_name }}:
         {{ x.include_docker_build(aux, opts) }}
         {{ x.include_platform(aux) }}
         image: {{ opts.image_name }}
-        volumes:
-            - {{ aux.payload.docker_settings.project_dir }}/deploy:/home/container/workdir:rw
-        working_dir: /home/container/workdir
+        {% if opts.get("mode") == "django" %}
+        ports:
+            - 80:8000
+        {% elif opts.get("mode") == "django+nginx" %}
+        ports:
+            - 8004:8004
+        {% elif opts.get("mode") == "ansible" %}
         environment:
-        - CI_JOB_TOKEN=$CI_JOB_TOKEN
-        - ANSIBLE_VAULT_PASS=$ANSIBLE_VAULT_PASS
-        - ANSIBLE_TARGET=deploy.yml -i inventory/${CI_COMMIT_BRANCH}.cfg
+        -   CI_JOB_TOKEN=$CI_JOB_TOKEN
+        -   ANSIBLE_VAULT_PASS=$ANSIBLE_VAULT_PASS
+        -   ANSIBLE_TARGET=deploy.yml -i inventory/${CI_COMMIT_BRANCH}.cfg
+        {% endif %}
```

### Comparing `adaux-2.4.5/source/adaux/src/docker/services/docs/Dockerfile.jinja2` & `adaux-2.5.0/source/adaux/src/docker/services/docs/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/src/docker/services/gitlab-release-run/docker-compose.yml.jinja2` & `adaux-2.5.0/source/adaux/src/docker/services/gitlab-release-run/docker-compose.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/src/docker/services/image/Dockerfile.jinja2` & `adaux-2.5.0/source/adaux/src/docker/services/image/Dockerfile.jinja2`

 * *Files 5% similar despite different names*

```diff
@@ -25,8 +25,11 @@
 CMD ["/bin/sh", "-c", "python manage.py collectstatic -c --noinput && python manage.py wait_for_database && python manage.py migrate && uwsgi --ini uwsgi.ini --http :8000"]
 {% elif opts.get("mode") == "django+nginx" %}
 EXPOSE 8004
 WORKDIR /home/container/code/{{ aux.project.second_name }}/{{aux.project.source_dir}}
 COPY --chown=container "{{aux.project.source_dir}}/manage.py" "manage.py"
 COPY --chown=container "{{aux.project.source_dir}}/uwsgi.ini" "uwsgi.ini"
 CMD ["/bin/sh", "-c", "python manage.py collectstatic -c --noinput && python manage.py wait_for_database && python manage.py migrate && uwsgi --ini uwsgi.ini --socket :8004"]
+{% elif opts.get("mode") == "ansible" %}
+WORKDIR /home/container/code/{{ aux.project.second_name }}/{{aux.project.source_dir}}/{{ aux.project.second_name }}
+{% include 'ansible_deploy.jinja2' -%}
 {% endif %}
```

### Comparing `adaux-2.4.5/source/adaux/src/docker/services/image-pytest/Dockerfile.jinja2` & `adaux-2.5.0/source/adaux/src/docker/services/image-pytest/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/src/docker/services/jinja-snippets/docker-build.jinja2` & `adaux-2.5.0/source/adaux/src/docker/services/jinja-snippets/docker-build.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/src/docker/services/pkg-gitlab/docker-compose.yml.jinja2` & `adaux-2.5.0/source/adaux/src/docker/services/pkg-gitlab/docker-compose.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/src/docker/services/pre-commit/Dockerfile.jinja2` & `adaux-2.5.0/source/adaux/src/docker/services/pre-commit/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/src/docker/services/pre-commit/docker-compose.yml.jinja2` & `adaux-2.5.0/source/adaux/src/docker/services/pre-commit/docker-compose.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/src/docker/services/pytest-standalone/Dockerfile.jinja2` & `adaux-2.5.0/source/adaux/src/docker/services/pytest-standalone/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/src/docker/services/python-deps/Dockerfile.jinja2` & `adaux-2.5.0/source/adaux/src/docker/services/python-deps/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/src/docs/default_conf.py.jinja2` & `adaux-2.5.0/source/adaux/src/docs/default_conf.py.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/src/docs/postprocess_html.py` & `adaux-2.5.0/source/adaux/src/docs/postprocess_html.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/src/license/Apache-2.0.txt.jinja2` & `adaux-2.5.0/source/adaux/src/license/Apache-2.0.txt.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/src/license/BSD-3_clause.txt.jinja2` & `adaux-2.5.0/source/adaux/src/license/BSD-3_clause.txt.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/src/license/MIT.txt.jinja2` & `adaux-2.5.0/source/adaux/src/license/MIT.txt.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/src/payload/python/__pycache__/functions.cpython-310.pyc` & `adaux-2.5.0/source/adaux/src/payload/python/__pycache__/functions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/src/payload/python/functions.py` & `adaux-2.5.0/source/adaux/src/payload/python/functions.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/src/pre-commit/add_copy_right.py.jinja2` & `adaux-2.5.0/source/adaux/src/pre-commit/add_copy_right.py.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux/src/pre-commit/config.yaml.jinja2` & `adaux-2.5.0/source/adaux/src/pre-commit/config.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.5/source/adaux.egg-info/SOURCES.txt` & `adaux-2.5.0/source/adaux.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -62,21 +62,24 @@
 source/adaux/src/CI/00-main.yml.jinja2
 source/adaux/src/CI/01-rules.yml.jinja2
 source/adaux/src/CI/jinja-snippets/coverage.jinja2
 source/adaux/src/CI/jinja-snippets/tags.jinja2
 source/adaux/src/docker/comp-helper.sh.jinja2
 source/adaux/src/docker/services/ansible-deploy/Dockerfile.jinja2
 source/adaux/src/docker/services/ansible-deploy/docker-compose.yml.jinja2
+source/adaux/src/docker/services/ansible-deploy-ext/docker-compose.yml.jinja2
 source/adaux/src/docker/services/docs/Dockerfile.jinja2
 source/adaux/src/docker/services/docs/docker-compose.yml.jinja2
 source/adaux/src/docker/services/gitlab-release-run/docker-compose.yml.jinja2
 source/adaux/src/docker/services/image/Dockerfile.jinja2
 source/adaux/src/docker/services/image/docker-compose.yml.jinja2
 source/adaux/src/docker/services/image-pytest/Dockerfile.jinja2
 source/adaux/src/docker/services/image-pytest/docker-compose.yml.jinja2
+source/adaux/src/docker/services/jinja-snippets/ansible_deploy.jinja2
+source/adaux/src/docker/services/jinja-snippets/ansible_env.jinja2
 source/adaux/src/docker/services/jinja-snippets/apt_install.jinja2
 source/adaux/src/docker/services/jinja-snippets/apt_install_root.jinja2
 source/adaux/src/docker/services/jinja-snippets/base_arg.jinja2
 source/adaux/src/docker/services/jinja-snippets/docker-build.jinja2
 source/adaux/src/docker/services/jinja-snippets/extra_script.jinja2
 source/adaux/src/docker/services/jinja-snippets/macros.jinja2
 source/adaux/src/docker/services/jinja-snippets/pip_install.jinja2
```


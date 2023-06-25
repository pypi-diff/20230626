# Comparing `tmp/ctfcli-0.0.8.tar.gz` & `tmp/ctfcli-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctfcli-0.0.8.tar", last modified: Tue Jun 22 03:14:55 2021, max compression
+gzip compressed data, was "ctfcli-0.0.9.tar", last modified: Sat Aug  7 02:48:25 2021, max compression
```

## Comparing `ctfcli-0.0.8.tar` & `ctfcli-0.0.9.tar`

### file list

```diff
@@ -1,114 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 03:14:55.925502 ctfcli-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)    11339 2021-06-22 03:14:39.000000 ctfcli-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      136 2021-06-22 03:14:39.000000 ctfcli-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5527 2021-06-22 03:14:55.925502 ctfcli-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4243 2021-06-22 03:14:39.000000 ctfcli-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 03:14:55.917502 ctfcli-0.0.8/ctfcli/
--rw-r--r--   0 runner    (1001) docker     (121)       42 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1997 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 03:14:55.921502 ctfcli-0.0.8/ctfcli/cli/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10630 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/cli/challenges.py
--rw-r--r--   0 runner    (1001) docker     (121)      948 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      739 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/cli/plugins.py
--rw-r--r--   0 runner    (1001) docker     (121)      890 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/cli/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 03:14:55.921502 ctfcli-0.0.8/ctfcli/spec/
--rw-r--r--   0 runner    (1001) docker     (121)     3268 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/spec/challenge-example.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 03:14:55.917502 ctfcli-0.0.8/ctfcli/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 03:14:55.917502 ctfcli-0.0.8/ctfcli/templates/binary/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 03:14:55.921502 ctfcli-0.0.8/ctfcli/templates/binary/default/
--rw-r--r--   0 runner    (1001) docker     (121)       23 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/binary/default/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 03:14:55.921502 ctfcli-0.0.8/ctfcli/templates/binary/default/{{cookiecutter.name}}/
--rw-r--r--   0 runner    (1001) docker     (121)      156 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/binary/default/{{cookiecutter.name}}/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (121)      206 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/binary/default/{{cookiecutter.name}}/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)       50 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/binary/default/{{cookiecutter.name}}/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     3268 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/binary/default/{{cookiecutter.name}}/challenge.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 03:14:55.921502 ctfcli-0.0.8/ctfcli/templates/binary/default/{{cookiecutter.name}}/src/
--rw-r--r--   0 runner    (1001) docker     (121)      138 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/binary/default/{{cookiecutter.name}}/src/{{cookiecutter.name}}.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 03:14:55.921502 ctfcli-0.0.8/ctfcli/templates/binary/default/{{cookiecutter.name}}/writeup/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/binary/default/{{cookiecutter.name}}/writeup/WRITEUP.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 03:14:55.917502 ctfcli-0.0.8/ctfcli/templates/blank/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 03:14:55.921502 ctfcli-0.0.8/ctfcli/templates/blank/default/
--rw-r--r--   0 runner    (1001) docker     (121)       27 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/blank/default/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 03:14:55.921502 ctfcli-0.0.8/ctfcli/templates/blank/default/{{cookiecutter.name}}/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/blank/default/{{cookiecutter.name}}/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     3268 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/blank/default/{{cookiecutter.name}}/challenge.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 03:14:55.921502 ctfcli-0.0.8/ctfcli/templates/blank/default/{{cookiecutter.name}}/src/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/blank/default/{{cookiecutter.name}}/src/placeholder
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 03:14:55.921502 ctfcli-0.0.8/ctfcli/templates/blank/default/{{cookiecutter.name}}/writeup/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/blank/default/{{cookiecutter.name}}/writeup/WRITEUP.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 03:14:55.917502 ctfcli-0.0.8/ctfcli/templates/crypto/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 03:14:55.921502 ctfcli-0.0.8/ctfcli/templates/crypto/default/
--rw-r--r--   0 runner    (1001) docker     (121)       23 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/crypto/default/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 03:14:55.921502 ctfcli-0.0.8/ctfcli/templates/crypto/default/{{cookiecutter.name}}/
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/crypto/default/{{cookiecutter.name}}/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)       70 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/crypto/default/{{cookiecutter.name}}/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)       50 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/crypto/default/{{cookiecutter.name}}/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     3268 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/crypto/default/{{cookiecutter.name}}/challenge.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 03:14:55.921502 ctfcli-0.0.8/ctfcli/templates/crypto/default/{{cookiecutter.name}}/src/
--rw-r--r--   0 runner    (1001) docker     (121)      246 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/crypto/default/{{cookiecutter.name}}/src/encrypt.py
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/crypto/default/{{cookiecutter.name}}/src/flag.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 03:14:55.921502 ctfcli-0.0.8/ctfcli/templates/crypto/default/{{cookiecutter.name}}/writeup/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/crypto/default/{{cookiecutter.name}}/writeup/WRITEUP.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 03:14:55.917502 ctfcli-0.0.8/ctfcli/templates/programming/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 03:14:55.921502 ctfcli-0.0.8/ctfcli/templates/programming/default/
--rw-r--r--   0 runner    (1001) docker     (121)       65 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/programming/default/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 03:14:55.921502 ctfcli-0.0.8/ctfcli/templates/programming/default/{{cookiecutter.name}}/
--rw-r--r--   0 runner    (1001) docker     (121)      156 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/programming/default/{{cookiecutter.name}}/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/programming/default/{{cookiecutter.name}}/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      432 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/programming/default/{{cookiecutter.name}}/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)       50 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/programming/default/{{cookiecutter.name}}/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     3268 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/programming/default/{{cookiecutter.name}}/challenge.yml
--rw-r--r--   0 runner    (1001) docker     (121)       88 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/programming/default/{{cookiecutter.name}}/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 03:14:55.921502 ctfcli-0.0.8/ctfcli/templates/programming/default/{{cookiecutter.name}}/src/
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/programming/default/{{cookiecutter.name}}/src/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)      160 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/programming/default/{{cookiecutter.name}}/src/serve.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      375 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/programming/default/{{cookiecutter.name}}/src/server.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 03:14:55.925502 ctfcli-0.0.8/ctfcli/templates/programming/default/{{cookiecutter.name}}/writeup/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/programming/default/{{cookiecutter.name}}/writeup/WRITEUP.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 03:14:55.917502 ctfcli-0.0.8/ctfcli/templates/web/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 03:14:55.925502 ctfcli-0.0.8/ctfcli/templates/web/default/
--rw-r--r--   0 runner    (1001) docker     (121)       23 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/web/default/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 03:14:55.925502 ctfcli-0.0.8/ctfcli/templates/web/default/{{cookiecutter.name}}/
--rw-r--r--   0 runner    (1001) docker     (121)      156 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/web/default/{{cookiecutter.name}}/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (121)      337 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/web/default/{{cookiecutter.name}}/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)       50 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/web/default/{{cookiecutter.name}}/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     3268 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/web/default/{{cookiecutter.name}}/challenge.yml
--rw-r--r--   0 runner    (1001) docker     (121)       76 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/web/default/{{cookiecutter.name}}/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 03:14:55.925502 ctfcli-0.0.8/ctfcli/templates/web/default/{{cookiecutter.name}}/src/
--rwxr-xr-x   0 runner    (1001) docker     (121)     2605 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/web/default/{{cookiecutter.name}}/src/app.py
--rw-r--r--   0 runner    (1001) docker     (121)      191 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/web/default/{{cookiecutter.name}}/src/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      618 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/web/default/{{cookiecutter.name}}/src/models.py
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/web/default/{{cookiecutter.name}}/src/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)      127 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/web/default/{{cookiecutter.name}}/src/serve.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 03:14:55.917502 ctfcli-0.0.8/ctfcli/templates/web/default/{{cookiecutter.name}}/src/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 03:14:55.925502 ctfcli-0.0.8/ctfcli/templates/web/default/{{cookiecutter.name}}/src/static/css/
--rw-r--r--   0 runner    (1001) docker     (121)       31 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/web/default/{{cookiecutter.name}}/src/static/css/main.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 03:14:55.925502 ctfcli-0.0.8/ctfcli/templates/web/default/{{cookiecutter.name}}/src/templates/
--rw-r--r--   0 runner    (1001) docker     (121)     2202 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/web/default/{{cookiecutter.name}}/src/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/web/default/{{cookiecutter.name}}/src/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (121)      997 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/web/default/{{cookiecutter.name}}/src/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (121)      231 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/web/default/{{cookiecutter.name}}/src/templates/profile.html
--rw-r--r--   0 runner    (1001) docker     (121)     1007 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/web/default/{{cookiecutter.name}}/src/templates/register.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 03:14:55.925502 ctfcli-0.0.8/ctfcli/templates/web/default/{{cookiecutter.name}}/writeup/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/templates/web/default/{{cookiecutter.name}}/writeup/WRITEUP.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 03:14:55.925502 ctfcli-0.0.8/ctfcli/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      730 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/utils/api.py
--rw-r--r--   0 runner    (1001) docker     (121)    12158 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/utils/challenge.py
--rw-r--r--   0 runner    (1001) docker     (121)     1529 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1580 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/utils/deploy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1322 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/utils/images.py
--rw-r--r--   0 runner    (1001) docker     (121)      336 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/utils/plugins.py
--rw-r--r--   0 runner    (1001) docker     (121)     2883 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/utils/spec.py
--rw-r--r--   0 runner    (1001) docker     (121)      340 2021-06-22 03:14:39.000000 ctfcli-0.0.8/ctfcli/utils/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 03:14:55.921502 ctfcli-0.0.8/ctfcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5527 2021-06-22 03:14:55.000000 ctfcli-0.0.8/ctfcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3972 2021-06-22 03:14:55.000000 ctfcli-0.0.8/ctfcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-22 03:14:55.000000 ctfcli-0.0.8/ctfcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2021-06-22 03:14:55.000000 ctfcli-0.0.8/ctfcli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-22 03:14:55.000000 ctfcli-0.0.8/ctfcli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      119 2021-06-22 03:14:55.000000 ctfcli-0.0.8/ctfcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-06-22 03:14:55.000000 ctfcli-0.0.8/ctfcli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-06-22 03:14:55.925502 ctfcli-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1198 2021-06-22 03:14:39.000000 ctfcli-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-07 02:48:25.208829 ctfcli-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11339 2021-08-07 02:48:06.000000 ctfcli-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      136 2021-08-07 02:48:06.000000 ctfcli-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     5527 2021-08-07 02:48:25.208829 ctfcli-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4243 2021-08-07 02:48:06.000000 ctfcli-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-07 02:48:25.196829 ctfcli-0.0.9/ctfcli/
+-rw-r--r--   0 runner    (1001) docker     (121)       42 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1997 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-07 02:48:25.200829 ctfcli-0.0.9/ctfcli/cli/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12016 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/cli/challenges.py
+-rw-r--r--   0 runner    (1001) docker     (121)      948 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)      739 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/cli/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (121)      890 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/cli/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-07 02:48:25.200829 ctfcli-0.0.9/ctfcli/spec/
+-rw-r--r--   0 runner    (1001) docker     (121)     3603 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/spec/challenge-example.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-07 02:48:25.196829 ctfcli-0.0.9/ctfcli/templates/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-07 02:48:25.192829 ctfcli-0.0.9/ctfcli/templates/binary/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-07 02:48:25.200829 ctfcli-0.0.9/ctfcli/templates/binary/default/
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/binary/default/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-07 02:48:25.200829 ctfcli-0.0.9/ctfcli/templates/binary/default/{{cookiecutter.name}}/
+-rw-r--r--   0 runner    (1001) docker     (121)      156 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/binary/default/{{cookiecutter.name}}/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (121)      206 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/binary/default/{{cookiecutter.name}}/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)       50 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/binary/default/{{cookiecutter.name}}/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     3603 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/binary/default/{{cookiecutter.name}}/challenge.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-07 02:48:25.200829 ctfcli-0.0.9/ctfcli/templates/binary/default/{{cookiecutter.name}}/src/
+-rw-r--r--   0 runner    (1001) docker     (121)      138 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/binary/default/{{cookiecutter.name}}/src/{{cookiecutter.name}}.c
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-07 02:48:25.200829 ctfcli-0.0.9/ctfcli/templates/binary/default/{{cookiecutter.name}}/writeup/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/binary/default/{{cookiecutter.name}}/writeup/WRITEUP.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-07 02:48:25.196829 ctfcli-0.0.9/ctfcli/templates/blank/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-07 02:48:25.200829 ctfcli-0.0.9/ctfcli/templates/blank/default/
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/blank/default/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-07 02:48:25.200829 ctfcli-0.0.9/ctfcli/templates/blank/default/{{cookiecutter.name}}/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/blank/default/{{cookiecutter.name}}/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     3603 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/blank/default/{{cookiecutter.name}}/challenge.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-07 02:48:25.200829 ctfcli-0.0.9/ctfcli/templates/blank/default/{{cookiecutter.name}}/src/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/blank/default/{{cookiecutter.name}}/src/placeholder
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-07 02:48:25.200829 ctfcli-0.0.9/ctfcli/templates/blank/default/{{cookiecutter.name}}/writeup/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/blank/default/{{cookiecutter.name}}/writeup/WRITEUP.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-07 02:48:25.196829 ctfcli-0.0.9/ctfcli/templates/crypto/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-07 02:48:25.200829 ctfcli-0.0.9/ctfcli/templates/crypto/default/
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/crypto/default/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-07 02:48:25.200829 ctfcli-0.0.9/ctfcli/templates/crypto/default/{{cookiecutter.name}}/
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/crypto/default/{{cookiecutter.name}}/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)       70 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/crypto/default/{{cookiecutter.name}}/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)       50 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/crypto/default/{{cookiecutter.name}}/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     3603 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/crypto/default/{{cookiecutter.name}}/challenge.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-07 02:48:25.200829 ctfcli-0.0.9/ctfcli/templates/crypto/default/{{cookiecutter.name}}/src/
+-rw-r--r--   0 runner    (1001) docker     (121)      246 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/crypto/default/{{cookiecutter.name}}/src/encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/crypto/default/{{cookiecutter.name}}/src/flag.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-07 02:48:25.200829 ctfcli-0.0.9/ctfcli/templates/crypto/default/{{cookiecutter.name}}/writeup/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/crypto/default/{{cookiecutter.name}}/writeup/WRITEUP.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-07 02:48:25.196829 ctfcli-0.0.9/ctfcli/templates/programming/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-07 02:48:25.200829 ctfcli-0.0.9/ctfcli/templates/programming/default/
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/programming/default/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-07 02:48:25.204829 ctfcli-0.0.9/ctfcli/templates/programming/default/{{cookiecutter.name}}/
+-rw-r--r--   0 runner    (1001) docker     (121)      156 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/programming/default/{{cookiecutter.name}}/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/programming/default/{{cookiecutter.name}}/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      432 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/programming/default/{{cookiecutter.name}}/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (121)       50 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/programming/default/{{cookiecutter.name}}/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     3603 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/programming/default/{{cookiecutter.name}}/challenge.yml
+-rw-r--r--   0 runner    (1001) docker     (121)       88 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/programming/default/{{cookiecutter.name}}/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-07 02:48:25.204829 ctfcli-0.0.9/ctfcli/templates/programming/default/{{cookiecutter.name}}/src/
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/programming/default/{{cookiecutter.name}}/src/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (121)      160 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/programming/default/{{cookiecutter.name}}/src/serve.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)      375 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/programming/default/{{cookiecutter.name}}/src/server.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-07 02:48:25.204829 ctfcli-0.0.9/ctfcli/templates/programming/default/{{cookiecutter.name}}/writeup/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/programming/default/{{cookiecutter.name}}/writeup/WRITEUP.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-07 02:48:25.196829 ctfcli-0.0.9/ctfcli/templates/web/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-07 02:48:25.204829 ctfcli-0.0.9/ctfcli/templates/web/default/
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/web/default/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-07 02:48:25.204829 ctfcli-0.0.9/ctfcli/templates/web/default/{{cookiecutter.name}}/
+-rw-r--r--   0 runner    (1001) docker     (121)      156 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/web/default/{{cookiecutter.name}}/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (121)      337 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/web/default/{{cookiecutter.name}}/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (121)       50 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/web/default/{{cookiecutter.name}}/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     3603 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/web/default/{{cookiecutter.name}}/challenge.yml
+-rw-r--r--   0 runner    (1001) docker     (121)       76 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/web/default/{{cookiecutter.name}}/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-07 02:48:25.204829 ctfcli-0.0.9/ctfcli/templates/web/default/{{cookiecutter.name}}/src/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2605 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/web/default/{{cookiecutter.name}}/src/app.py
+-rw-r--r--   0 runner    (1001) docker     (121)      191 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/web/default/{{cookiecutter.name}}/src/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)      618 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/web/default/{{cookiecutter.name}}/src/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/web/default/{{cookiecutter.name}}/src/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (121)      127 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/web/default/{{cookiecutter.name}}/src/serve.sh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-07 02:48:25.196829 ctfcli-0.0.9/ctfcli/templates/web/default/{{cookiecutter.name}}/src/static/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-07 02:48:25.204829 ctfcli-0.0.9/ctfcli/templates/web/default/{{cookiecutter.name}}/src/static/css/
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/web/default/{{cookiecutter.name}}/src/static/css/main.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-07 02:48:25.208829 ctfcli-0.0.9/ctfcli/templates/web/default/{{cookiecutter.name}}/src/templates/
+-rw-r--r--   0 runner    (1001) docker     (121)     2202 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/web/default/{{cookiecutter.name}}/src/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/web/default/{{cookiecutter.name}}/src/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (121)      997 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/web/default/{{cookiecutter.name}}/src/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (121)      231 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/web/default/{{cookiecutter.name}}/src/templates/profile.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1007 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/web/default/{{cookiecutter.name}}/src/templates/register.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-07 02:48:25.208829 ctfcli-0.0.9/ctfcli/templates/web/default/{{cookiecutter.name}}/writeup/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/templates/web/default/{{cookiecutter.name}}/writeup/WRITEUP.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-07 02:48:25.208829 ctfcli-0.0.9/ctfcli/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      730 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/utils/api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13761 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/utils/challenge.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1529 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1580 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/utils/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (121)      356 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1322 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/utils/images.py
+-rw-r--r--   0 runner    (1001) docker     (121)      336 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/utils/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2883 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/utils/spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)      340 2021-08-07 02:48:06.000000 ctfcli-0.0.9/ctfcli/utils/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-07 02:48:25.200829 ctfcli-0.0.9/ctfcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5527 2021-08-07 02:48:25.000000 ctfcli-0.0.9/ctfcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3992 2021-08-07 02:48:25.000000 ctfcli-0.0.9/ctfcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-07 02:48:25.000000 ctfcli-0.0.9/ctfcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2021-08-07 02:48:25.000000 ctfcli-0.0.9/ctfcli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-07 02:48:25.000000 ctfcli-0.0.9/ctfcli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      119 2021-08-07 02:48:25.000000 ctfcli-0.0.9/ctfcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-08-07 02:48:25.000000 ctfcli-0.0.9/ctfcli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-08-07 02:48:25.208829 ctfcli-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1198 2021-08-07 02:48:06.000000 ctfcli-0.0.9/setup.py
```

### Comparing `ctfcli-0.0.8/LICENSE` & `ctfcli-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ctfcli-0.0.8/PKG-INFO` & `ctfcli-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctfcli
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tool for creating and running Capture The Flag competitions
 Home-page: UNKNOWN
 Author: Kevin Chung
 Author-email: kchung@ctfd.io
 License: Apache 2.0
 Description: # ctfcli
```

### Comparing `ctfcli-0.0.8/README.md` & `ctfcli-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ctfcli-0.0.8/ctfcli/__main__.py` & `ctfcli-0.0.9/ctfcli/__main__.py`

 * *Files identical despite different names*

### Comparing `ctfcli-0.0.8/ctfcli/cli/challenges.py` & `ctfcli-0.0.9/ctfcli/cli/challenges.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-import shutil
 import subprocess
 from pathlib import Path
 from urllib.parse import urlparse
 
 import click
 import yaml
 from cookiecutter.main import cookiecutter
@@ -20,14 +19,15 @@
     get_config_path,
     get_project_path,
     load_config,
 )
 from ctfcli.utils.deploy import DEPLOY_HANDLERS
 from ctfcli.utils.spec import CHALLENGE_SPEC_DOCS, blank_challenge_spec
 from ctfcli.utils.templates import get_template_dir
+from ctfcli.utils.git import get_git_repo_head_branch
 
 
 class Challenge(object):
     def new(self, type="blank"):
         if type == "blank":
             path = Path(get_base_path())
             path = path / "templates" / type / "default"
@@ -54,28 +54,40 @@
     def add(self, repo):
         config = load_config()
 
         if repo.endswith(".git"):
             # Get relative path from project root to current directory
             challenge_path = Path(os.path.relpath(os.getcwd(), get_project_path()))
 
-            # Get new directory that will exist after clone
+            # Get new directory that will add the git subtree
             base_repo_path = Path(os.path.basename(repo).rsplit(".", maxsplit=1)[0])
 
             # Join targets
             challenge_path = challenge_path / base_repo_path
             print(challenge_path)
 
             config["challenges"][str(challenge_path)] = repo
 
+            head_branch = get_git_repo_head_branch(repo)
+            subprocess.call(
+                [
+                    "git",
+                    "subtree",
+                    "add",
+                    "--prefix",
+                    challenge_path,
+                    repo,
+                    head_branch,
+                    "--squash",
+                ],
+                cwd=get_project_path(),
+            )
             with open(get_config_path(), "w+") as f:
                 config.write(f)
 
-            subprocess.call(["git", "clone", "--depth", "1", repo])
-            shutil.rmtree(str(base_repo_path / ".git"))
         elif Path(repo).exists():
             config["challenges"][repo] = repo
             with open(get_config_path(), "w+") as f:
                 config.write(f)
         else:
             click.secho(
                 "Couldn't process that challenge path. Please check it for errors.",
@@ -85,17 +97,29 @@
     def restore(self, challenge=None):
         config = load_config()
         challenges = dict(config["challenges"])
         for folder, url in challenges.items():
             if url.endswith(".git"):
                 if challenge is not None and folder != challenge:
                     continue
-                click.echo(f"Cloning {url} to {folder}")
-                subprocess.call(["git", "clone", "--depth", "1", url, folder])
-                shutil.rmtree(str(Path(folder) / ".git"))
+                click.echo(f"Adding git repo {url} to {folder} as subtree")
+                head_branch = get_git_repo_head_branch(url)
+                subprocess.call(
+                    [
+                        "git",
+                        "subtree",
+                        "add",
+                        "--prefix",
+                        folder,
+                        url,
+                        head_branch,
+                        "--squash",
+                    ],
+                    cwd=get_project_path(),
+                )
             else:
                 click.echo(f"Skipping {url} - {folder}")
 
     def install(self, challenge=None, force=False, ignore=()):
         if challenge is None:
             # Get all challenges if not specifying a challenge
             config = load_config()
@@ -174,30 +198,32 @@
     def update(self, challenge=None):
         config = load_config()
         challenges = dict(config["challenges"])
         for folder, url in challenges.items():
             if challenge and challenge != folder:
                 continue
             if url.endswith(".git"):
-                click.echo(f"Cloning {url} to {folder}")
-                subprocess.call(["git", "init"], cwd=folder)
-                subprocess.call(["git", "remote", "add", "origin", url], cwd=folder)
-                subprocess.call(["git", "add", "-A"], cwd=folder)
+                click.echo(f"Pulling latest {url} to {folder}")
+                head_branch = get_git_repo_head_branch(url)
                 subprocess.call(
-                    ["git", "commit", "-m", "Persist local changes (ctfcli)"],
-                    cwd=folder,
-                )
-                subprocess.call(
-                    ["git", "pull", "--allow-unrelated-histories", "origin", "master"],
-                    cwd=folder,
+                    [
+                        "git",
+                        "subtree",
+                        "pull",
+                        "--prefix",
+                        folder,
+                        url,
+                        head_branch,
+                        "--squash",
+                    ],
+                    cwd=get_project_path(),
                 )
                 subprocess.call(["git", "mergetool"], cwd=folder)
                 subprocess.call(["git", "clean", "-f"], cwd=folder)
                 subprocess.call(["git", "commit", "--no-edit"], cwd=folder)
-                shutil.rmtree(str(Path(folder) / ".git"))
             else:
                 click.echo(f"Skipping {url} - {folder}")
 
     def finalize(self, challenge=None):
         if challenge is None:
             challenge = os.getcwd()
 
@@ -295,7 +321,27 @@
             click.secho(
                 f"Challenge deployed at {domain}:{port}", fg="green",
             )
         else:
             click.secho(
                 f"An error occured during deployment", fg="red",
             )
+
+    def push(self, challenge=None):
+        config = load_config()
+        challenges = dict(config["challenges"])
+        if challenge is None:
+            # Get relative path from project root to current directory
+            challenge_path = Path(os.path.relpath(os.getcwd(), get_project_path()))
+            challenge = str(challenge_path)
+
+        try:
+            url = challenges[challenge]
+            head_branch = get_git_repo_head_branch(url)
+            subprocess.call(
+                ["git", "subtree", "push", "--prefix", challenge, url, head_branch],
+                cwd=get_project_path(),
+            )
+        except KeyError:
+            click.echo(
+                "Couldn't process that challenge path. Please check that the challenge is added to .ctf/config and that your path matches."
+            )
```

### Comparing `ctfcli-0.0.8/ctfcli/cli/config.py` & `ctfcli-0.0.9/ctfcli/cli/config.py`

 * *Files identical despite different names*

### Comparing `ctfcli-0.0.8/ctfcli/cli/plugins.py` & `ctfcli-0.0.9/ctfcli/cli/plugins.py`

 * *Files identical despite different names*

### Comparing `ctfcli-0.0.8/ctfcli/cli/templates.py` & `ctfcli-0.0.9/ctfcli/cli/templates.py`

 * *Files identical despite different names*

### Comparing `ctfcli-0.0.8/ctfcli/spec/challenge-example.yml` & `ctfcli-0.0.9/ctfcli/spec/challenge-example.yml`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,18 @@
 # The currently supported URI schemes are ssh:// and registry://
 # ssh is an ssh URI where the above image will be copied to and deployed (e.g. ssh://root@123.123.123.123)
 # registry is a Docker registry tag (e.g registry://registry.example.com/test/image)
 # host can also be specified during the deploy process: `ctf challenge deploy challenge --host=ssh://root@123.123.123.123`
 host: null
 
 # Optional settings
+
+# connection_info is used to provide a link, hostname, or instructions on how to connect to a challenge
+connection_info: nc hostname 12345
+
 # Can be removed if unused
 attempts: 5
 
 # Flags specify answers that your challenge use. You should generally provide at least one.
 # Can be removed if unused
 # Accepts strings or dictionaries of CTFd API data
 flags:
@@ -55,16 +59,23 @@
     # A regex case insensitive flag
     - {
         type: "regex",
         content: "(.*)STUFF(.*)",
         data: "case_insensitive",
     }
 
-# Tags are used to classify your challenge with topics. You should provide at
-# least one.
+# Topics are used to help tell what techniques/information a challenge involves
+# They are generally only visible to admins
+# Accepts strings
+topics:
+    - information disclosure
+    - buffer overflow
+    - memory forensics
+
+# Tags are used to provide additional public tagging to a challenge
 # Can be removed if unused
 # Accepts strings
 tags:
     - web
     - sandbox
     - js
 
@@ -87,15 +98,14 @@
 # Requirements are used to make a challenge require another challenge to be
 # solved before being available.
 # Can be removed if unused
 # Accepts challenge names as strings or challenge IDs as integers
 requirements:
     - "Warmup"
     - "Are you alive"
-    - 1
 
 # The state of the challenge.
 # If the field is omitted, the challenge is visible by default.
 # If provided, the field can take one of two values: hidden, visible.
 state: hidden
 
 # Specifies what version of the challenge specification was used.
```

### Comparing `ctfcli-0.0.8/ctfcli/templates/binary/default/{{cookiecutter.name}}/challenge.yml` & `ctfcli-0.0.9/ctfcli/templates/binary/default/{{cookiecutter.name}}/challenge.yml`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,18 @@
 # The currently supported URI schemes are ssh:// and registry://
 # ssh is an ssh URI where the above image will be copied to and deployed (e.g. ssh://root@123.123.123.123)
 # registry is a Docker registry tag (e.g registry://registry.example.com/test/image)
 # host can also be specified during the deploy process: `ctf challenge deploy challenge --host=ssh://root@123.123.123.123`
 host: null
 
 # Optional settings
+
+# connection_info is used to provide a link, hostname, or instructions on how to connect to a challenge
+connection_info: nc hostname 12345
+
 # Can be removed if unused
 attempts: 5
 
 # Flags specify answers that your challenge use. You should generally provide at least one.
 # Can be removed if unused
 # Accepts strings or dictionaries of CTFd API data
 flags:
@@ -55,16 +59,23 @@
     # A regex case insensitive flag
     - {
         type: "regex",
         content: "(.*)STUFF(.*)",
         data: "case_insensitive",
     }
 
-# Tags are used to classify your challenge with topics. You should provide at
-# least one.
+# Topics are used to help tell what techniques/information a challenge involves
+# They are generally only visible to admins
+# Accepts strings
+topics:
+    - information disclosure
+    - buffer overflow
+    - memory forensics
+
+# Tags are used to provide additional public tagging to a challenge
 # Can be removed if unused
 # Accepts strings
 tags:
     - web
     - sandbox
     - js
 
@@ -87,15 +98,14 @@
 # Requirements are used to make a challenge require another challenge to be
 # solved before being available.
 # Can be removed if unused
 # Accepts challenge names as strings or challenge IDs as integers
 requirements:
     - "Warmup"
     - "Are you alive"
-    - 1
 
 # The state of the challenge.
 # If the field is omitted, the challenge is visible by default.
 # If provided, the field can take one of two values: hidden, visible.
 state: hidden
 
 # Specifies what version of the challenge specification was used.
```

### Comparing `ctfcli-0.0.8/ctfcli/templates/blank/default/{{cookiecutter.name}}/challenge.yml` & `ctfcli-0.0.9/ctfcli/templates/blank/default/{{cookiecutter.name}}/challenge.yml`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,18 @@
 # The currently supported URI schemes are ssh:// and registry://
 # ssh is an ssh URI where the above image will be copied to and deployed (e.g. ssh://root@123.123.123.123)
 # registry is a Docker registry tag (e.g registry://registry.example.com/test/image)
 # host can also be specified during the deploy process: `ctf challenge deploy challenge --host=ssh://root@123.123.123.123`
 host: null
 
 # Optional settings
+
+# connection_info is used to provide a link, hostname, or instructions on how to connect to a challenge
+connection_info: nc hostname 12345
+
 # Can be removed if unused
 attempts: 5
 
 # Flags specify answers that your challenge use. You should generally provide at least one.
 # Can be removed if unused
 # Accepts strings or dictionaries of CTFd API data
 flags:
@@ -55,16 +59,23 @@
     # A regex case insensitive flag
     - {
         type: "regex",
         content: "(.*)STUFF(.*)",
         data: "case_insensitive",
     }
 
-# Tags are used to classify your challenge with topics. You should provide at
-# least one.
+# Topics are used to help tell what techniques/information a challenge involves
+# They are generally only visible to admins
+# Accepts strings
+topics:
+    - information disclosure
+    - buffer overflow
+    - memory forensics
+
+# Tags are used to provide additional public tagging to a challenge
 # Can be removed if unused
 # Accepts strings
 tags:
     - web
     - sandbox
     - js
 
@@ -87,15 +98,14 @@
 # Requirements are used to make a challenge require another challenge to be
 # solved before being available.
 # Can be removed if unused
 # Accepts challenge names as strings or challenge IDs as integers
 requirements:
     - "Warmup"
     - "Are you alive"
-    - 1
 
 # The state of the challenge.
 # If the field is omitted, the challenge is visible by default.
 # If provided, the field can take one of two values: hidden, visible.
 state: hidden
 
 # Specifies what version of the challenge specification was used.
```

### Comparing `ctfcli-0.0.8/ctfcli/templates/crypto/default/{{cookiecutter.name}}/challenge.yml` & `ctfcli-0.0.9/ctfcli/templates/crypto/default/{{cookiecutter.name}}/challenge.yml`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,18 @@
 # The currently supported URI schemes are ssh:// and registry://
 # ssh is an ssh URI where the above image will be copied to and deployed (e.g. ssh://root@123.123.123.123)
 # registry is a Docker registry tag (e.g registry://registry.example.com/test/image)
 # host can also be specified during the deploy process: `ctf challenge deploy challenge --host=ssh://root@123.123.123.123`
 host: null
 
 # Optional settings
+
+# connection_info is used to provide a link, hostname, or instructions on how to connect to a challenge
+connection_info: nc hostname 12345
+
 # Can be removed if unused
 attempts: 5
 
 # Flags specify answers that your challenge use. You should generally provide at least one.
 # Can be removed if unused
 # Accepts strings or dictionaries of CTFd API data
 flags:
@@ -55,16 +59,23 @@
     # A regex case insensitive flag
     - {
         type: "regex",
         content: "(.*)STUFF(.*)",
         data: "case_insensitive",
     }
 
-# Tags are used to classify your challenge with topics. You should provide at
-# least one.
+# Topics are used to help tell what techniques/information a challenge involves
+# They are generally only visible to admins
+# Accepts strings
+topics:
+    - information disclosure
+    - buffer overflow
+    - memory forensics
+
+# Tags are used to provide additional public tagging to a challenge
 # Can be removed if unused
 # Accepts strings
 tags:
     - web
     - sandbox
     - js
 
@@ -87,15 +98,14 @@
 # Requirements are used to make a challenge require another challenge to be
 # solved before being available.
 # Can be removed if unused
 # Accepts challenge names as strings or challenge IDs as integers
 requirements:
     - "Warmup"
     - "Are you alive"
-    - 1
 
 # The state of the challenge.
 # If the field is omitted, the challenge is visible by default.
 # If provided, the field can take one of two values: hidden, visible.
 state: hidden
 
 # Specifies what version of the challenge specification was used.
```

### Comparing `ctfcli-0.0.8/ctfcli/templates/programming/default/{{cookiecutter.name}}/challenge.yml` & `ctfcli-0.0.9/ctfcli/templates/programming/default/{{cookiecutter.name}}/challenge.yml`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,18 @@
 # The currently supported URI schemes are ssh:// and registry://
 # ssh is an ssh URI where the above image will be copied to and deployed (e.g. ssh://root@123.123.123.123)
 # registry is a Docker registry tag (e.g registry://registry.example.com/test/image)
 # host can also be specified during the deploy process: `ctf challenge deploy challenge --host=ssh://root@123.123.123.123`
 host: null
 
 # Optional settings
+
+# connection_info is used to provide a link, hostname, or instructions on how to connect to a challenge
+connection_info: nc hostname 12345
+
 # Can be removed if unused
 attempts: 5
 
 # Flags specify answers that your challenge use. You should generally provide at least one.
 # Can be removed if unused
 # Accepts strings or dictionaries of CTFd API data
 flags:
@@ -55,16 +59,23 @@
     # A regex case insensitive flag
     - {
         type: "regex",
         content: "(.*)STUFF(.*)",
         data: "case_insensitive",
     }
 
-# Tags are used to classify your challenge with topics. You should provide at
-# least one.
+# Topics are used to help tell what techniques/information a challenge involves
+# They are generally only visible to admins
+# Accepts strings
+topics:
+    - information disclosure
+    - buffer overflow
+    - memory forensics
+
+# Tags are used to provide additional public tagging to a challenge
 # Can be removed if unused
 # Accepts strings
 tags:
     - web
     - sandbox
     - js
 
@@ -87,15 +98,14 @@
 # Requirements are used to make a challenge require another challenge to be
 # solved before being available.
 # Can be removed if unused
 # Accepts challenge names as strings or challenge IDs as integers
 requirements:
     - "Warmup"
     - "Are you alive"
-    - 1
 
 # The state of the challenge.
 # If the field is omitted, the challenge is visible by default.
 # If provided, the field can take one of two values: hidden, visible.
 state: hidden
 
 # Specifies what version of the challenge specification was used.
```

### Comparing `ctfcli-0.0.8/ctfcli/templates/web/default/{{cookiecutter.name}}/challenge.yml` & `ctfcli-0.0.9/ctfcli/templates/web/default/{{cookiecutter.name}}/challenge.yml`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,18 @@
 # The currently supported URI schemes are ssh:// and registry://
 # ssh is an ssh URI where the above image will be copied to and deployed (e.g. ssh://root@123.123.123.123)
 # registry is a Docker registry tag (e.g registry://registry.example.com/test/image)
 # host can also be specified during the deploy process: `ctf challenge deploy challenge --host=ssh://root@123.123.123.123`
 host: null
 
 # Optional settings
+
+# connection_info is used to provide a link, hostname, or instructions on how to connect to a challenge
+connection_info: nc hostname 12345
+
 # Can be removed if unused
 attempts: 5
 
 # Flags specify answers that your challenge use. You should generally provide at least one.
 # Can be removed if unused
 # Accepts strings or dictionaries of CTFd API data
 flags:
@@ -55,16 +59,23 @@
     # A regex case insensitive flag
     - {
         type: "regex",
         content: "(.*)STUFF(.*)",
         data: "case_insensitive",
     }
 
-# Tags are used to classify your challenge with topics. You should provide at
-# least one.
+# Topics are used to help tell what techniques/information a challenge involves
+# They are generally only visible to admins
+# Accepts strings
+topics:
+    - information disclosure
+    - buffer overflow
+    - memory forensics
+
+# Tags are used to provide additional public tagging to a challenge
 # Can be removed if unused
 # Accepts strings
 tags:
     - web
     - sandbox
     - js
 
@@ -87,15 +98,14 @@
 # Requirements are used to make a challenge require another challenge to be
 # solved before being available.
 # Can be removed if unused
 # Accepts challenge names as strings or challenge IDs as integers
 requirements:
     - "Warmup"
     - "Are you alive"
-    - 1
 
 # The state of the challenge.
 # If the field is omitted, the challenge is visible by default.
 # If provided, the field can take one of two values: hidden, visible.
 state: hidden
 
 # Specifies what version of the challenge specification was used.
```

### Comparing `ctfcli-0.0.8/ctfcli/templates/web/default/{{cookiecutter.name}}/src/app.py` & `ctfcli-0.0.9/ctfcli/templates/web/default/{{cookiecutter.name}}/src/app.py`

 * *Files identical despite different names*

### Comparing `ctfcli-0.0.8/ctfcli/templates/web/default/{{cookiecutter.name}}/src/models.py` & `ctfcli-0.0.9/ctfcli/templates/web/default/{{cookiecutter.name}}/src/models.py`

 * *Files identical despite different names*

### Comparing `ctfcli-0.0.8/ctfcli/templates/web/default/{{cookiecutter.name}}/src/templates/base.html` & `ctfcli-0.0.9/ctfcli/templates/web/default/{{cookiecutter.name}}/src/templates/base.html`

 * *Files identical despite different names*

### Comparing `ctfcli-0.0.8/ctfcli/templates/web/default/{{cookiecutter.name}}/src/templates/login.html` & `ctfcli-0.0.9/ctfcli/templates/web/default/{{cookiecutter.name}}/src/templates/login.html`

 * *Files identical despite different names*

### Comparing `ctfcli-0.0.8/ctfcli/templates/web/default/{{cookiecutter.name}}/src/templates/register.html` & `ctfcli-0.0.9/ctfcli/templates/web/default/{{cookiecutter.name}}/src/templates/register.html`

 * *Files identical despite different names*

### Comparing `ctfcli-0.0.8/ctfcli/utils/api.py` & `ctfcli-0.0.9/ctfcli/utils/api.py`

 * *Files identical despite different names*

### Comparing `ctfcli-0.0.8/ctfcli/utils/challenge.py` & `ctfcli-0.0.9/ctfcli/utils/challenge.py`

 * *Files 13% similar despite different names*

```diff
@@ -42,14 +42,17 @@
     # We can't send it to CTFd because we don't know the current value
     if challenge["value"] is None:
         del challenge["value"]
 
     if challenge.get("attempts") and "attempts" not in ignore:
         data["max_attempts"] = challenge.get("attempts")
 
+    if challenge.get("connection_info") and "connection_info" not in ignore:
+        data["connection_info"] = challenge.get("connection_info")
+
     data["state"] = "hidden"
 
     installed_challenges = load_installed_challenges()
     for c in installed_challenges:
         if c["name"] == challenge["name"]:
             challenge_id = c["id"]
             break
@@ -72,33 +75,59 @@
         for flag in current_flags:
             if flag["challenge_id"] == challenge_id:
                 flag_id = flag["id"]
                 r = s.delete(f"/api/v1/flags/{flag_id}", json=True)
                 r.raise_for_status()
         for flag in challenge["flags"]:
             if type(flag) == str:
-                data = {"content": flag, "type": "static", "challenge": challenge_id}
+                data = {"content": flag, "type": "static", "challenge_id": challenge_id}
                 r = s.post(f"/api/v1/flags", json=data)
                 r.raise_for_status()
             elif type(flag) == dict:
-                flag["challenge"] = challenge_id
+                flag["challenge_id"] = challenge_id
                 r = s.post(f"/api/v1/flags", json=flag)
                 r.raise_for_status()
 
+    # Update topics
+    if challenge.get("topics") and "topics" not in ignore:
+        # Delete existing challenge topics
+        current_topics = s.get(
+            f"/api/v1/challenges/{challenge_id}/topics", json=""
+        ).json()["data"]
+        for topic in current_topics:
+            topic_id = topic["id"]
+            r = s.delete(
+                f"/api/v1/topics?type=challenge&target_id={topic_id}", json=True
+            )
+            r.raise_for_status()
+        # Add new challenge topics
+        for topic in challenge["topics"]:
+            r = s.post(
+                f"/api/v1/topics",
+                json={
+                    "value": topic,
+                    "type": "challenge",
+                    "challenge_id": challenge_id,
+                },
+            )
+            r.raise_for_status()
+
     # Update tags
     if challenge.get("tags") and "tags" not in ignore:
         # Delete existing tags
         current_tags = s.get(f"/api/v1/tags", json=data).json()["data"]
         for tag in current_tags:
             if tag["challenge_id"] == challenge_id:
                 tag_id = tag["id"]
                 r = s.delete(f"/api/v1/tags/{tag_id}", json=True)
                 r.raise_for_status()
         for tag in challenge["tags"]:
-            r = s.post(f"/api/v1/tags", json={"challenge": challenge_id, "value": tag})
+            r = s.post(
+                f"/api/v1/tags", json={"challenge_id": challenge_id, "value": tag}
+            )
             r.raise_for_status()
 
     # Upload files
     if challenge.get("files") and "files" not in ignore:
         # Delete existing files
         all_current_files = s.get(f"/api/v1/files?type=challenge", json=data).json()[
             "data"
@@ -115,15 +144,15 @@
             if file_path.exists():
                 file_object = ("file", file_path.open(mode="rb"))
                 files.append(file_object)
             else:
                 click.secho(f"File {file_path} was not found", fg="red")
                 raise Exception(f"File {file_path} was not found")
 
-        data = {"challenge": challenge_id, "type": "challenge"}
+        data = {"challenge_id": challenge_id, "type": "challenge"}
         # Specifically use data= here instead of json= to send multipart/form-data
         r = s.post(f"/api/v1/files", files=files, data=data)
         r.raise_for_status()
 
     # Create hints
     if challenge.get("hints") and "hints" not in ignore:
         # Delete existing hints
@@ -132,20 +161,20 @@
             if hint["challenge_id"] == challenge_id:
                 hint_id = hint["id"]
                 r = s.delete(f"/api/v1/hints/{hint_id}", json=True)
                 r.raise_for_status()
 
         for hint in challenge["hints"]:
             if type(hint) == str:
-                data = {"content": hint, "cost": 0, "challenge": challenge_id}
+                data = {"content": hint, "cost": 0, "challenge_id": challenge_id}
             else:
                 data = {
                     "content": hint["content"],
                     "cost": hint["cost"],
-                    "challenge": challenge_id,
+                    "challenge_id": challenge_id,
                 }
 
             r = s.post(f"/api/v1/hints", json=data)
             r.raise_for_status()
 
     # Update requirements
     if challenge.get("requirements") and "requirements" not in ignore:
@@ -189,67 +218,85 @@
     # We can't send it to CTFd because we don't know the current value
     if challenge["value"] is None:
         del challenge["value"]
 
     if challenge.get("attempts") and "attempts" not in ignore:
         data["max_attempts"] = challenge.get("attempts")
 
+    if challenge.get("connection_info") and "connection_info" not in ignore:
+        data["connection_info"] = challenge.get("connection_info")
+
     s = generate_session()
 
     r = s.post("/api/v1/challenges", json=data)
     r.raise_for_status()
 
     challenge_data = r.json()
     challenge_id = challenge_data["data"]["id"]
 
     # Create flags
     if challenge.get("flags") and "flags" not in ignore:
         for flag in challenge["flags"]:
             if type(flag) == str:
-                data = {"content": flag, "type": "static", "challenge": challenge_id}
+                data = {"content": flag, "type": "static", "challenge_id": challenge_id}
                 r = s.post(f"/api/v1/flags", json=data)
                 r.raise_for_status()
             elif type(flag) == dict:
                 flag["challenge"] = challenge_id
                 r = s.post(f"/api/v1/flags", json=flag)
                 r.raise_for_status()
 
+    # Create topics
+    if challenge.get("topics") and "topics" not in ignore:
+        for topic in challenge["topics"]:
+            r = s.post(
+                f"/api/v1/topics",
+                json={
+                    "value": topic,
+                    "type": "challenge",
+                    "challenge_id": challenge_id,
+                },
+            )
+            r.raise_for_status()
+
     # Create tags
     if challenge.get("tags") and "tags" not in ignore:
         for tag in challenge["tags"]:
-            r = s.post(f"/api/v1/tags", json={"challenge": challenge_id, "value": tag})
+            r = s.post(
+                f"/api/v1/tags", json={"challenge_id": challenge_id, "value": tag}
+            )
             r.raise_for_status()
 
     # Upload files
     if challenge.get("files") and "files" not in ignore:
         files = []
         for f in challenge["files"]:
             file_path = Path(challenge.directory, f)
             if file_path.exists():
                 file_object = ("file", file_path.open(mode="rb"))
                 files.append(file_object)
             else:
                 click.secho(f"File {file_path} was not found", fg="red")
                 raise Exception(f"File {file_path} was not found")
 
-        data = {"challenge": challenge_id, "type": "challenge"}
+        data = {"challenge_id": challenge_id, "type": "challenge"}
         # Specifically use data= here instead of json= to send multipart/form-data
         r = s.post(f"/api/v1/files", files=files, data=data)
         r.raise_for_status()
 
     # Add hints
     if challenge.get("hints") and "hints" not in ignore:
         for hint in challenge["hints"]:
             if type(hint) == str:
-                data = {"content": hint, "cost": 0, "challenge": challenge_id}
+                data = {"content": hint, "cost": 0, "challenge_id": challenge_id}
             else:
                 data = {
                     "content": hint["content"],
                     "cost": hint["cost"],
-                    "challenge": challenge_id,
+                    "challenge_id": challenge_id,
                 }
 
             r = s.post(f"/api/v1/hints", json=data)
             r.raise_for_status()
 
     # Add requirements
     if challenge.get("requirements") and "requirements" not in ignore:
```

### Comparing `ctfcli-0.0.8/ctfcli/utils/config.py` & `ctfcli-0.0.9/ctfcli/utils/config.py`

 * *Files identical despite different names*

### Comparing `ctfcli-0.0.8/ctfcli/utils/deploy.py` & `ctfcli-0.0.9/ctfcli/utils/deploy.py`

 * *Files identical despite different names*

### Comparing `ctfcli-0.0.8/ctfcli/utils/images.py` & `ctfcli-0.0.9/ctfcli/utils/images.py`

 * *Files identical despite different names*

### Comparing `ctfcli-0.0.8/ctfcli/utils/spec.py` & `ctfcli-0.0.9/ctfcli/utils/spec.py`

 * *Files identical despite different names*

### Comparing `ctfcli-0.0.8/ctfcli.egg-info/PKG-INFO` & `ctfcli-0.0.9/ctfcli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctfcli
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tool for creating and running Capture The Flag competitions
 Home-page: UNKNOWN
 Author: Kevin Chung
 Author-email: kchung@ctfd.io
 License: Apache 2.0
 Description: # ctfcli
```

### Comparing `ctfcli-0.0.8/ctfcli.egg-info/SOURCES.txt` & `ctfcli-0.0.9/ctfcli.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -67,11 +67,12 @@
 ctfcli/templates/web/default/{{cookiecutter.name}}/src/templates/register.html
 ctfcli/templates/web/default/{{cookiecutter.name}}/writeup/WRITEUP.md
 ctfcli/utils/__init__.py
 ctfcli/utils/api.py
 ctfcli/utils/challenge.py
 ctfcli/utils/config.py
 ctfcli/utils/deploy.py
+ctfcli/utils/git.py
 ctfcli/utils/images.py
 ctfcli/utils/plugins.py
 ctfcli/utils/spec.py
 ctfcli/utils/templates.py
```

### Comparing `ctfcli-0.0.8/setup.py` & `ctfcli-0.0.9/setup.py`

 * *Files identical despite different names*


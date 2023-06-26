# Comparing `tmp/adafruit-circuitpython-bno055-5.4.8.tar.gz` & `tmp/adafruit-circuitpython-bno055-5.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-bno055-5.4.8.tar", last modified: Mon Nov 28 18:14:59 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-bno055-5.4.9.tar", last modified: Mon Feb 20 03:52:53 2023, max compression
```

## Comparing `adafruit-circuitpython-bno055-5.4.8.tar` & `adafruit-circuitpython-bno055-5.4.9.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:14:59.240826 adafruit-circuitpython-bno055-5.4.8/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:14:59.224826 adafruit-circuitpython-bno055-5.4.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:14:59.224826 adafruit-circuitpython-bno055-5.4.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (122)      880 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:14:59.224826 adafruit-circuitpython-bno055-5.4.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      303 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (122)      479 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (122)      423 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (122)      475 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1648 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1239 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    13069 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (122)      388 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     6147 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (122)     1119 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:14:59.224826 adafruit-circuitpython-bno055-5.4.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (122)    16814 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1211 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (122)     3952 2022-11-28 18:14:59.240826 adafruit-circuitpython-bno055-5.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3119 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/README.rst.license
--rwxr-xr-x   0 runner    (1001) docker     (122)    37027 2022-11-28 18:14:49.000000 adafruit-circuitpython-bno055-5.4.8/adafruit_bno055.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:14:59.228826 adafruit-circuitpython-bno055-5.4.8/adafruit_circuitpython_bno055.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3952 2022-11-28 18:14:59.000000 adafruit-circuitpython-bno055-5.4.8/adafruit_circuitpython_bno055.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3837 2022-11-28 18:14:59.000000 adafruit-circuitpython-bno055-5.4.8/adafruit_circuitpython_bno055.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-28 18:14:59.000000 adafruit-circuitpython-bno055-5.4.8/adafruit_circuitpython_bno055.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       93 2022-11-28 18:14:59.000000 adafruit-circuitpython-bno055-5.4.8/adafruit_circuitpython_bno055.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2022-11-28 18:14:59.000000 adafruit-circuitpython-bno055-5.4.8/adafruit_circuitpython_bno055.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:14:59.228826 adafruit-circuitpython-bno055-5.4.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:14:59.228826 adafruit-circuitpython-bno055-5.4.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (122)     4414 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (122)      105 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (122)       46 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)       96 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     5724 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      505 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (122)       96 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     1248 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)       96 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)      123 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:14:59.228826 adafruit-circuitpython-bno055-5.4.8/examples/
--rw-r--r--   0 runner    (1001) docker     (122)     1713 2022-11-28 18:14:49.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_i2c-gpio_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1445 2022-11-28 18:14:49.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:14:59.228826 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/
--rw-r--r--   0 runner    (1001) docker     (122)     6309 2022-11-28 18:14:49.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/server.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:14:59.232826 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/
--rw-r--r--   0 runner    (1001) docker     (122)      212 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/bunny.mtl
--rw-r--r--   0 runner    (1001) docker     (122)       94 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/bunny.mtl.license
--rw-r--r--   0 runner    (1001) docker     (122)  2302743 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/bunny.obj
--rw-r--r--   0 runner    (1001) docker     (122)       94 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/bunny.obj.license
--rw-r--r--   0 runner    (1001) docker     (122)  2124784 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/cat-top.stl
--rw-r--r--   0 runner    (1001) docker     (122)       94 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/cat-top.stl.license
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:14:59.236826 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/css/
--rw-r--r--   0 runner    (1001) docker     (122)    26132 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/css/bootstrap-theme.css
--rw-r--r--   0 runner    (1001) docker     (122)       81 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/css/bootstrap-theme.css.license
--rw-r--r--   0 runner    (1001) docker     (122)    47722 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/css/bootstrap-theme.css.map
--rw-r--r--   0 runner    (1001) docker     (122)       81 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/css/bootstrap-theme.css.map.license
--rw-r--r--   0 runner    (1001) docker     (122)    23358 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/css/bootstrap-theme.min.css
--rw-r--r--   0 runner    (1001) docker     (122)       81 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/css/bootstrap-theme.min.css.license
--rw-r--r--   0 runner    (1001) docker     (122)   147430 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/css/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (122)       81 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/css/bootstrap.css.license
--rw-r--r--   0 runner    (1001) docker     (122)   390519 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/css/bootstrap.css.map
--rw-r--r--   0 runner    (1001) docker     (122)       81 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/css/bootstrap.css.map.license
--rw-r--r--   0 runner    (1001) docker     (122)   122541 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (122)       81 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/css/bootstrap.min.css.license
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:14:59.236826 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (122)    20127 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 runner    (1001) docker     (122)       94 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/fonts/glyphicons-halflings-regular.eot.license
--rw-r--r--   0 runner    (1001) docker     (122)   108738 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 runner    (1001) docker     (122)       94 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/fonts/glyphicons-halflings-regular.svg.license
--rw-r--r--   0 runner    (1001) docker     (122)    45404 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (122)       94 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/fonts/glyphicons-halflings-regular.ttf.license
--rw-r--r--   0 runner    (1001) docker     (122)    23424 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 runner    (1001) docker     (122)       94 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/fonts/glyphicons-halflings-regular.woff.license
--rw-r--r--   0 runner    (1001) docker     (122)    18028 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/fonts/glyphicons-halflings-regular.woff2
--rw-r--r--   0 runner    (1001) docker     (122)       94 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/fonts/glyphicons-halflings-regular.woff2.license
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:14:59.240826 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/js/
--rw-r--r--   0 runner    (1001) docker     (122)     5439 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/js/DDSLoader.js
--rw-r--r--   0 runner    (1001) docker     (122)       85 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/js/DDSLoader.js.license
--rw-r--r--   0 runner    (1001) docker     (122)     9032 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/js/MTLLoader.js
--rw-r--r--   0 runner    (1001) docker     (122)       71 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/js/MTLLoader.js.license
--rw-r--r--   0 runner    (1001) docker     (122)     7774 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/js/OBJLoader.js
--rw-r--r--   0 runner    (1001) docker     (122)       85 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/js/OBJLoader.js.license
--rw-r--r--   0 runner    (1001) docker     (122)     8379 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/js/OBJMTLLoader.js
--rw-r--r--   0 runner    (1001) docker     (122)      126 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/js/OBJMTLLoader.js.license
--rw-r--r--   0 runner    (1001) docker     (122)    10838 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/js/STLLoader.js
--rw-r--r--   0 runner    (1001) docker     (122)      203 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/js/STLLoader.js.license
--rw-r--r--   0 runner    (1001) docker     (122)    36817 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/js/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (122)       81 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/js/bootstrap.min.js.license
--rw-r--r--   0 runner    (1001) docker     (122)    84345 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/js/jquery-2.1.4.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      113 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/js/jquery-2.1.4.min.js.license
--rw-r--r--   0 runner    (1001) docker     (122)   419938 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/js/three.min.js
--rw-r--r--   0 runner    (1001) docker     (122)       84 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/js/three.min.js.license
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:14:59.240826 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/templates/
--rw-r--r--   0 runner    (1001) docker     (122)    12780 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (122)       94 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/templates/index.html.license
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1321 2022-11-28 18:14:49.000000 adafruit-circuitpython-bno055-5.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      190 2022-11-28 18:14:32.000000 adafruit-circuitpython-bno055-5.4.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-28 18:14:59.240826 adafruit-circuitpython-bno055-5.4.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 03:52:53.605774 adafruit-circuitpython-bno055-5.4.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 03:52:53.589774 adafruit-circuitpython-bno055-5.4.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 03:52:53.589774 adafruit-circuitpython-bno055-5.4.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 03:52:53.589774 adafruit-circuitpython-bno055-5.4.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 03:52:53.589774 adafruit-circuitpython-bno055-5.4.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-02-20 03:52:53.605774 adafruit-circuitpython-bno055-5.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/README.rst.license
+-rwxr-xr-x   0 runner    (1001) docker     (123)    37059 2023-02-20 03:52:46.000000 adafruit-circuitpython-bno055-5.4.9/adafruit_bno055.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 03:52:53.593774 adafruit-circuitpython-bno055-5.4.9/adafruit_circuitpython_bno055.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-02-20 03:52:53.000000 adafruit-circuitpython-bno055-5.4.9/adafruit_circuitpython_bno055.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-02-20 03:52:53.000000 adafruit-circuitpython-bno055-5.4.9/adafruit_circuitpython_bno055.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 03:52:53.000000 adafruit-circuitpython-bno055-5.4.9/adafruit_circuitpython_bno055.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-02-20 03:52:53.000000 adafruit-circuitpython-bno055-5.4.9/adafruit_circuitpython_bno055.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-20 03:52:53.000000 adafruit-circuitpython-bno055-5.4.9/adafruit_circuitpython_bno055.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 03:52:53.593774 adafruit-circuitpython-bno055-5.4.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 03:52:53.593774 adafruit-circuitpython-bno055-5.4.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 03:52:53.593774 adafruit-circuitpython-bno055-5.4.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-02-20 03:52:46.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_i2c-gpio_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-02-20 03:52:46.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 03:52:53.593774 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/
+-rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-02-20 03:52:46.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 03:52:53.597774 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/bunny.mtl
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/bunny.mtl.license
+-rw-r--r--   0 runner    (1001) docker     (123)  2302743 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/bunny.obj
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/bunny.obj.license
+-rw-r--r--   0 runner    (1001) docker     (123)  2124784 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/cat-top.stl
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/cat-top.stl.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 03:52:53.601774 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    26132 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/css/bootstrap-theme.css
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/css/bootstrap-theme.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)    47722 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/css/bootstrap-theme.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/css/bootstrap-theme.css.map.license
+-rw-r--r--   0 runner    (1001) docker     (123)    23358 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/css/bootstrap-theme.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/css/bootstrap-theme.min.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)   147430 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/css/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/css/bootstrap.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)   390519 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/css/bootstrap.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/css/bootstrap.css.map.license
+-rw-r--r--   0 runner    (1001) docker     (123)   122541 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/css/bootstrap.min.css.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 03:52:53.601774 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    20127 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/fonts/glyphicons-halflings-regular.eot.license
+-rw-r--r--   0 runner    (1001) docker     (123)   108738 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/fonts/glyphicons-halflings-regular.svg.license
+-rw-r--r--   0 runner    (1001) docker     (123)    45404 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/fonts/glyphicons-halflings-regular.ttf.license
+-rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/fonts/glyphicons-halflings-regular.woff.license
+-rw-r--r--   0 runner    (1001) docker     (123)    18028 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/fonts/glyphicons-halflings-regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/fonts/glyphicons-halflings-regular.woff2.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 03:52:53.601774 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/js/DDSLoader.js
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/js/DDSLoader.js.license
+-rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/js/MTLLoader.js
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/js/MTLLoader.js.license
+-rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/js/OBJLoader.js
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/js/OBJLoader.js.license
+-rw-r--r--   0 runner    (1001) docker     (123)     8379 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/js/OBJMTLLoader.js
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/js/OBJMTLLoader.js.license
+-rw-r--r--   0 runner    (1001) docker     (123)    10838 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/js/STLLoader.js
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/js/STLLoader.js.license
+-rw-r--r--   0 runner    (1001) docker     (123)    36817 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/js/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/js/bootstrap.min.js.license
+-rw-r--r--   0 runner    (1001) docker     (123)    84345 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/js/jquery-2.1.4.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/js/jquery-2.1.4.min.js.license
+-rw-r--r--   0 runner    (1001) docker     (123)   419938 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/js/three.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/js/three.min.js.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 03:52:53.605774 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    12780 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/templates/index.html.license
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-02-20 03:52:46.000000 adafruit-circuitpython-bno055-5.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-02-20 03:52:34.000000 adafruit-circuitpython-bno055-5.4.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-20 03:52:53.605774 adafruit-circuitpython-bno055-5.4.9/setup.cfg
```

### Comparing `adafruit-circuitpython-bno055-5.4.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-bno055-5.4.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno055-5.4.8/.gitignore` & `adafruit-circuitpython-bno055-5.4.9/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 _build
 
 # This file results from running `pip -e install .` in a local repository
 *.egg-info
 
 # Virtual environment-specific files
 .env
+.venv
 
 # MacOS-specific files
 *.DS_Store
 
 # IDE-specific files
 .idea
 .vscode
```

### Comparing `adafruit-circuitpython-bno055-5.4.8/.pre-commit-config.yaml` & `adafruit-circuitpython-bno055-5.4.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno055-5.4.8/.pylintrc` & `adafruit-circuitpython-bno055-5.4.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno055-5.4.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-bno055-5.4.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno055-5.4.8/LICENSE` & `adafruit-circuitpython-bno055-5.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno055-5.4.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-bno055-5.4.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno055-5.4.8/LICENSES/MIT.txt` & `adafruit-circuitpython-bno055-5.4.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno055-5.4.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-bno055-5.4.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno055-5.4.8/PKG-INFO` & `adafruit-circuitpython-bno055-5.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-bno055
-Version: 5.4.8
+Version: 5.4.9
 Summary: CircuitPython library for BNO055 9-DOF absolute orientation sensor.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BNO055
 Keywords: adafruit,9-dof,absolute,orientation,accelerometer,velocity,temperature,gravitymagnetic,breakout,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-bno055-5.4.8/README.rst` & `adafruit-circuitpython-bno055-5.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno055-5.4.8/adafruit_bno055.py` & `adafruit-circuitpython-bno055-5.4.9/adafruit_bno055.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 try:
     from typing import Any, Optional, Tuple, Type, Union
     from busio import I2C, UART
 except ImportError:
     pass
 
-__version__ = "5.4.8"
+__version__ = "5.4.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BNO055.git"
 
 _CHIP_ID = const(0xA0)
 
 CONFIG_MODE = const(0x00)
 ACCONLY_MODE = const(0x01)
 MAGONLY_MODE = const(0x02)
@@ -456,17 +456,19 @@
         return (None, None, None)
 
     @property
     def _euler(self) -> None:
         raise NotImplementedError("Must be implemented.")
 
     @property
-    def quaternion(self) -> Tuple[Optional[float], Optional[float], Optional[float]]:
+    def quaternion(
+        self,
+    ) -> Tuple[Optional[float], Optional[float], Optional[float], Optional[float]]:
         """Gives the calculated orientation as a quaternion.
-        Returns an empty tuple of length 3 when this property has been disabled by the current mode.
+        Returns an empty tuple of length 4 when this property has been disabled by the current mode.
         """
         if self.mode in [0x08, 0x09, 0x0A, 0x0B, 0x0C]:
             return self._quaternion
         return (None, None, None, None)
 
     @property
     def _quaternion(self) -> None:
```

### Comparing `adafruit-circuitpython-bno055-5.4.8/adafruit_circuitpython_bno055.egg-info/PKG-INFO` & `adafruit-circuitpython-bno055-5.4.9/adafruit_circuitpython_bno055.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-bno055
-Version: 5.4.8
+Version: 5.4.9
 Summary: CircuitPython library for BNO055 9-DOF absolute orientation sensor.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BNO055
 Keywords: adafruit,9-dof,absolute,orientation,accelerometer,velocity,temperature,gravitymagnetic,breakout,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-bno055-5.4.8/adafruit_circuitpython_bno055.egg-info/SOURCES.txt` & `adafruit-circuitpython-bno055-5.4.9/adafruit_circuitpython_bno055.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno055-5.4.8/docs/_static/favicon.ico` & `adafruit-circuitpython-bno055-5.4.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno055-5.4.8/docs/conf.py` & `adafruit-circuitpython-bno055-5.4.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno055-5.4.8/docs/index.rst` & `adafruit-circuitpython-bno055-5.4.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno055-5.4.8/examples/bno055_i2c-gpio_simpletest.py` & `adafruit-circuitpython-bno055-5.4.9/examples/bno055_i2c-gpio_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno055-5.4.8/examples/bno055_simpletest.py` & `adafruit-circuitpython-bno055-5.4.9/examples/bno055_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/server.py` & `adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/server.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/bunny.obj` & `adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/bunny.obj`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/cat-top.stl` & `adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/cat-top.stl`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/css/bootstrap-theme.css` & `adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/css/bootstrap-theme.css.map` & `adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/css/bootstrap-theme.css.map`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/css/bootstrap-theme.min.css` & `adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/css/bootstrap.css` & `adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/css/bootstrap.css.map` & `adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/css/bootstrap.min.css` & `adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/fonts/glyphicons-halflings-regular.eot` & `adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/fonts/glyphicons-halflings-regular.svg` & `adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/fonts/glyphicons-halflings-regular.ttf` & `adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/fonts/glyphicons-halflings-regular.woff` & `adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/fonts/glyphicons-halflings-regular.woff2` & `adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/js/DDSLoader.js` & `adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/js/DDSLoader.js`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/js/MTLLoader.js` & `adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/js/MTLLoader.js`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/js/OBJLoader.js` & `adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/js/OBJLoader.js`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/js/OBJMTLLoader.js` & `adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/js/OBJMTLLoader.js`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/js/STLLoader.js` & `adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/js/STLLoader.js`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/js/bootstrap.min.js` & `adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/js/jquery-2.1.4.min.js` & `adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/js/jquery-2.1.4.min.js`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/static/js/three.min.js` & `adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/static/js/three.min.js`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno055-5.4.8/examples/bno055_webgl_demo/templates/index.html` & `adafruit-circuitpython-bno055-5.4.9/examples/bno055_webgl_demo/templates/index.html`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno055-5.4.8/pyproject.toml` & `adafruit-circuitpython-bno055-5.4.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-bno055"
 description = "CircuitPython library for BNO055 9-DOF absolute orientation sensor."
-version = "5.4.8"
+version = "5.4.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_BNO055"}
 keywords = [
     "adafruit",
```


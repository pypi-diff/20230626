# Comparing `tmp/robot-soccer-kit-2.1.0.tar.gz` & `tmp/robot-soccer-kit-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robot-soccer-kit-2.1.0.tar", last modified: Mon Jun 26 12:26:17 2023, max compression
+gzip compressed data, was "robot-soccer-kit-2.1.1.tar", last modified: Mon Jun 26 12:37:59 2023, max compression
```

## Comparing `robot-soccer-kit-2.1.0.tar` & `robot-soccer-kit-2.1.1.tar`

### file list

```diff
@@ -1,163 +1,164 @@
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:26:17.952185 robot-soccer-kit-2.1.0/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      262 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/LICENSE
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1157 2023-06-26 12:26:17.952185 robot-soccer-kit-2.1.0/PKG-INFO
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      588 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/README.md
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:26:17.940185 robot-soccer-kit-2.1.0/robot_soccer_kit.egg-info/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1157 2023-06-26 12:26:17.000000 robot-soccer-kit-2.1.0/robot_soccer_kit.egg-info/PKG-INFO
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4874 2023-06-26 12:26:17.000000 robot-soccer-kit-2.1.0/robot_soccer_kit.egg-info/SOURCES.txt
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)        1 2023-06-26 12:26:17.000000 robot-soccer-kit-2.1.0/robot_soccer_kit.egg-info/dependency_links.txt
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       82 2023-06-26 12:26:17.000000 robot-soccer-kit-2.1.0/robot_soccer_kit.egg-info/requires.txt
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)        4 2023-06-26 12:26:17.000000 robot-soccer-kit-2.1.0/robot_soccer_kit.egg-info/top_level.txt
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:26:17.944185 robot-soccer-kit-2.1.0/rsk/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      102 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/__init__.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      571 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/api.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5422 2023-04-29 10:15:19.000000 robot-soccer-kit-2.1.0/rsk/backend.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    10981 2023-06-26 12:26:02.000000 robot-soccer-kit-2.1.0/rsk/client.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      277 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/config.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3224 2023-06-26 12:24:11.000000 robot-soccer-kit-2.1.0/rsk/constants.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    13616 2023-06-26 12:24:11.000000 robot-soccer-kit-2.1.0/rsk/control.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       35 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/debug.sh
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    18552 2023-04-29 10:39:09.000000 robot-soccer-kit-2.1.0/rsk/detection.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1058 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/dumb_ia.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      571 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/dump_referee.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       73 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/em.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    10173 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/field.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2379 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/game_controller.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2462 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/kinematics.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      445 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/logger.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      602 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/place.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    23739 2023-06-26 12:26:02.000000 robot-soccer-kit-2.1.0/rsk/referee.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2362 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/robot.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    11752 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/robot_serial.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6030 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/robots.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    10231 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/simulator.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2321 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/state.py
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:26:17.944185 robot-soccer-kit-2.1.0/rsk/static/
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:26:17.940185 robot-soccer-kit-2.1.0/rsk/static/bootstrap/
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:26:17.944185 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    75616 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-grid.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   226018 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-grid.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    56464 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-grid.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   142342 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-grid.min.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    75690 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-grid.rtl.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   226022 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-grid.rtl.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    56539 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   142419 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    11735 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-reboot.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   126626 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-reboot.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     9817 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-reboot.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    51406 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-reboot.min.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    11728 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   126641 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     9889 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    63643 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    96254 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-utilities.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   250681 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-utilities.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    74887 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-utilities.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   163881 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-utilities.min.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    96121 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   250622 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    74815 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   163716 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   267476 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   658460 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   220780 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   568408 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap.min.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   267055 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap.rtl.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   658305 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap.rtl.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   220887 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap.rtl.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   567947 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap.rtl.min.css.map
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:26:17.948185 robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   208288 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.bundle.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   448884 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.bundle.js.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    80599 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.bundle.min.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   333974 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.bundle.min.js.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   136243 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.esm.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   305274 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.esm.js.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    74135 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.esm.min.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   222070 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.esm.min.js.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   145819 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   306458 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.js.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    60554 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.min.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   217885 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.min.js.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      215 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/camera-setting.html
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:26:17.948185 robot-soccer-kit-2.1.0/rsk/static/css/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2566 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/css/app.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1150 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/favicon.ico
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:26:17.948185 robot-soccer-kit-2.1.0/rsk/static/icons/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      376 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/.browserslistrc
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      167 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/.editorconfig
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       40 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/.eslintignore
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      375 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/.eslintrc.json
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      922 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/.fantasticonrc.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       43 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/.gitattributes
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:26:17.948185 robot-soccer-kit-2.1.0/rsk/static/icons/.github/
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:26:17.948185 robot-soccer-kit-2.1.0/rsk/static/icons/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      583 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      122 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/.github/ISSUE_TEMPLATE/icon-request.md
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      433 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/.github/dependabot.yml
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   248086 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/.github/preview.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      572 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/.github/release-drafter.yml
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:26:17.948185 robot-soccer-kit-2.1.0/rsk/static/icons/.github/workflows/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      662 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/.github/workflows/codeql.yml
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1190 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/.github/workflows/deploy.yml
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      243 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/.github/workflows/release-notes.yml
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      575 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/.github/workflows/test.yml
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       63 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/.gitignore
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      125 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/.stylelintrc
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1093 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/LICENSE.md
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3312 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/README.md
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   881772 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/bootstrap-icons.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      425 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/composer.json
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2052 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/config.yml
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:26:17.948185 robot-soccer-kit-2.1.0/rsk/static/icons/font/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    80510 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/font/bootstrap-icons.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    42897 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/font/bootstrap-icons.json
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:26:17.948185 robot-soccer-kit-2.1.0/rsk/static/icons/font/fonts/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   137124 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/font/fonts/bootstrap-icons.woff
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   102536 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/font/fonts/bootstrap-icons.woff2
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   200995 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/font/index.html
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   643115 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/package-lock.json
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3152 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/package.json
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3085 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/svg-sprite.json
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      654 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/svgo.config.js
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:26:17.952185 robot-soccer-kit-2.1.0/rsk/static/imgs/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3287 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/imgs/ball.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1251 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/imgs/ball_16x16.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1856 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/imgs/ball_24x24.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    43069 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/imgs/ball_256x256.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2654 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/imgs/ball_32x32.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4470 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/imgs/ball_48x48.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    19402 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/imgs/field.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    17815 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/imgs/field.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   249649 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/imgs/robot.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   507520 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/imgs/robotblue1.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   524385 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/imgs/robotblue2.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   498488 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/imgs/robotgreen1.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   522425 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/imgs/robotgreen2.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    27029 2023-06-26 12:25:23.000000 robot-soccer-kit-2.1.0/rsk/static/index.html
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:26:17.952185 robot-soccer-kit-2.1.0/rsk/static/jquery/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   288580 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/jquery/jquery.js
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:26:17.952185 robot-soccer-kit-2.1.0/rsk/static/js/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1714 2023-06-26 12:24:11.000000 robot-soccer-kit-2.1.0/rsk/static/js/app.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1567 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/js/control.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    13425 2023-06-26 12:26:02.000000 robot-soccer-kit-2.1.0/rsk/static/js/referee.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6005 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/js/robots.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    14606 2023-06-26 12:26:02.000000 robot-soccer-kit-2.1.0/rsk/static/js/simulator.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      426 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/js/tabs.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      329 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/js/utils.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5997 2023-06-26 12:24:11.000000 robot-soccer-kit-2.1.0/rsk/static/js/video.js
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:26:17.952185 robot-soccer-kit-2.1.0/rsk/static/markers/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6021 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/markers/blue1.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6023 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/markers/blue2.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6009 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/markers/green1.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5098 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/markers/green2.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      337 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/referee_event_neutral.html
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      632 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/referee_event_team.html
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1029 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/robot.html
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      569 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/team.html
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3865 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/tasks.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4154 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/utils.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     9469 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/video.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       38 2023-06-26 12:26:17.952185 robot-soccer-kit-2.1.0/setup.cfg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1391 2023-06-26 12:25:51.000000 robot-soccer-kit-2.1.0/setup.py
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:37:59.220193 robot-soccer-kit-2.1.1/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      262 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/LICENSE
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1157 2023-06-26 12:37:59.220193 robot-soccer-kit-2.1.1/PKG-INFO
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      588 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/README.md
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:37:59.212193 robot-soccer-kit-2.1.1/robot_soccer_kit.egg-info/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1157 2023-06-26 12:37:59.000000 robot-soccer-kit-2.1.1/robot_soccer_kit.egg-info/PKG-INFO
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4903 2023-06-26 12:37:59.000000 robot-soccer-kit-2.1.1/robot_soccer_kit.egg-info/SOURCES.txt
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)        1 2023-06-26 12:37:59.000000 robot-soccer-kit-2.1.1/robot_soccer_kit.egg-info/dependency_links.txt
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       82 2023-06-26 12:37:59.000000 robot-soccer-kit-2.1.1/robot_soccer_kit.egg-info/requires.txt
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)        4 2023-06-26 12:37:59.000000 robot-soccer-kit-2.1.1/robot_soccer_kit.egg-info/top_level.txt
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:37:59.212193 robot-soccer-kit-2.1.1/rsk/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      102 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/__init__.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      571 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/api.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5543 2023-06-26 12:35:06.000000 robot-soccer-kit-2.1.1/rsk/backend.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    10981 2023-06-26 12:35:04.000000 robot-soccer-kit-2.1.1/rsk/client.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      277 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/config.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3224 2023-06-26 12:24:11.000000 robot-soccer-kit-2.1.1/rsk/constants.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    13616 2023-06-26 12:24:11.000000 robot-soccer-kit-2.1.1/rsk/control.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       35 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/debug.sh
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    18552 2023-04-29 10:39:09.000000 robot-soccer-kit-2.1.1/rsk/detection.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1058 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/dumb_ia.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      571 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/dump_referee.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       73 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/em.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    10173 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/field.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2461 2023-06-26 12:35:06.000000 robot-soccer-kit-2.1.1/rsk/game_controller.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2462 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/kinematics.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      445 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/logger.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      602 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/place.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    23739 2023-06-26 12:35:04.000000 robot-soccer-kit-2.1.1/rsk/referee.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2362 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/robot.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    11752 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/robot_serial.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6030 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/robots.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    10231 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/simulator.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2321 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/state.py
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:37:59.212193 robot-soccer-kit-2.1.1/rsk/static/
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:37:59.212193 robot-soccer-kit-2.1.1/rsk/static/bootstrap/
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:37:59.216193 robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    75616 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-grid.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   226018 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-grid.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    56464 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-grid.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   142342 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-grid.min.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    75690 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-grid.rtl.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   226022 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-grid.rtl.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    56539 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   142419 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    11735 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-reboot.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   126626 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-reboot.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     9817 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-reboot.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    51406 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-reboot.min.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    11728 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   126641 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     9889 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    63643 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    96254 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-utilities.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   250681 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-utilities.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    74887 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-utilities.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   163881 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-utilities.min.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    96121 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   250622 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    74815 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   163716 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   267476 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   658460 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   220780 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   568408 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap.min.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   267055 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap.rtl.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   658305 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap.rtl.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   220887 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap.rtl.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   567947 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap.rtl.min.css.map
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:37:59.216193 robot-soccer-kit-2.1.1/rsk/static/bootstrap/js/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   208288 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/bootstrap/js/bootstrap.bundle.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   448884 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/bootstrap/js/bootstrap.bundle.js.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    80599 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/bootstrap/js/bootstrap.bundle.min.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   333974 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/bootstrap/js/bootstrap.bundle.min.js.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   136243 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/bootstrap/js/bootstrap.esm.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   305274 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/bootstrap/js/bootstrap.esm.js.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    74135 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/bootstrap/js/bootstrap.esm.min.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   222070 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/bootstrap/js/bootstrap.esm.min.js.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   145819 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/bootstrap/js/bootstrap.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   306458 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/bootstrap/js/bootstrap.js.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    60554 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/bootstrap/js/bootstrap.min.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   217885 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/bootstrap/js/bootstrap.min.js.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      215 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/camera-setting.html
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:37:59.216193 robot-soccer-kit-2.1.1/rsk/static/css/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2606 2023-06-26 12:35:06.000000 robot-soccer-kit-2.1.1/rsk/static/css/app.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1150 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/favicon.ico
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:37:59.216193 robot-soccer-kit-2.1.1/rsk/static/icons/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      376 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/icons/.browserslistrc
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      167 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/icons/.editorconfig
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       40 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/icons/.eslintignore
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      375 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/icons/.eslintrc.json
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      922 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/icons/.fantasticonrc.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       43 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/icons/.gitattributes
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:37:59.216193 robot-soccer-kit-2.1.1/rsk/static/icons/.github/
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:37:59.216193 robot-soccer-kit-2.1.1/rsk/static/icons/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      583 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/icons/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      122 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/icons/.github/ISSUE_TEMPLATE/icon-request.md
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      433 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/icons/.github/dependabot.yml
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   248086 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/icons/.github/preview.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      572 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/icons/.github/release-drafter.yml
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:37:59.216193 robot-soccer-kit-2.1.1/rsk/static/icons/.github/workflows/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      662 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/icons/.github/workflows/codeql.yml
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1190 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/icons/.github/workflows/deploy.yml
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      243 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/icons/.github/workflows/release-notes.yml
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      575 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/icons/.github/workflows/test.yml
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       63 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/icons/.gitignore
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      125 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/icons/.stylelintrc
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1093 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/icons/LICENSE.md
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3312 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/icons/README.md
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   881772 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/icons/bootstrap-icons.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      425 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/icons/composer.json
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2052 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/icons/config.yml
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:37:59.220193 robot-soccer-kit-2.1.1/rsk/static/icons/font/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    80510 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/icons/font/bootstrap-icons.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    42897 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/icons/font/bootstrap-icons.json
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:37:59.220193 robot-soccer-kit-2.1.1/rsk/static/icons/font/fonts/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   137124 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/icons/font/fonts/bootstrap-icons.woff
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   102536 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/icons/font/fonts/bootstrap-icons.woff2
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   200995 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/icons/font/index.html
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   643115 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/icons/package-lock.json
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3152 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/icons/package.json
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3085 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/icons/svg-sprite.json
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      654 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/icons/svgo.config.js
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:37:59.220193 robot-soccer-kit-2.1.1/rsk/static/imgs/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3287 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/imgs/ball.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1251 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/imgs/ball_16x16.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1856 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/imgs/ball_24x24.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    43069 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/imgs/ball_256x256.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2654 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/imgs/ball_32x32.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4470 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/imgs/ball_48x48.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    19402 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/imgs/field.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    17815 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/imgs/field.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   249649 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/imgs/robot.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   507520 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/imgs/robotblue1.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   524385 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/imgs/robotblue2.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   498488 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/imgs/robotgreen1.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   522425 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/imgs/robotgreen2.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    33563 2023-06-26 12:35:06.000000 robot-soccer-kit-2.1.1/rsk/static/index.html
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:37:59.220193 robot-soccer-kit-2.1.1/rsk/static/jquery/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   288580 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/jquery/jquery.js
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:37:59.220193 robot-soccer-kit-2.1.1/rsk/static/js/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1900 2023-06-26 12:35:06.000000 robot-soccer-kit-2.1.1/rsk/static/js/app.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1738 2023-06-26 12:35:06.000000 robot-soccer-kit-2.1.1/rsk/static/js/competition.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1567 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/js/control.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    13425 2023-06-26 12:35:04.000000 robot-soccer-kit-2.1.1/rsk/static/js/referee.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6005 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/js/robots.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    14606 2023-06-26 12:35:04.000000 robot-soccer-kit-2.1.1/rsk/static/js/simulator.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      426 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/js/tabs.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      329 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/js/utils.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5997 2023-06-26 12:24:11.000000 robot-soccer-kit-2.1.1/rsk/static/js/video.js
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:37:59.220193 robot-soccer-kit-2.1.1/rsk/static/markers/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6021 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/markers/blue1.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6023 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/markers/blue2.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6009 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/markers/green1.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5098 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/markers/green2.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      337 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/referee_event_neutral.html
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      632 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/referee_event_team.html
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1029 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/static/robot.html
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      569 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.1/rsk/static/team.html
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3865 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/tasks.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4154 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/utils.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     9469 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.1/rsk/video.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       38 2023-06-26 12:37:59.220193 robot-soccer-kit-2.1.1/setup.cfg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1391 2023-06-26 12:37:49.000000 robot-soccer-kit-2.1.1/setup.py
```

### Comparing `robot-soccer-kit-2.1.0/PKG-INFO` & `robot-soccer-kit-2.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robot-soccer-kit
-Version: 2.1.0
+Version: 2.1.1
 Summary: Robot Soccer Kit
 Home-page: https://github.com/rhoban/robot-soccer-kit/
 Author: Rhoban team
 Author-email: team@rhoban.com
 License: UNKNOWN
 Keywords: robot holonomic omniwheel ssl robocup junior soccer standard localized tracking
 Platform: UNKNOWN
```

### Comparing `robot-soccer-kit-2.1.0/README.md` & `robot-soccer-kit-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/robot_soccer_kit.egg-info/PKG-INFO` & `robot-soccer-kit-2.1.1/robot_soccer_kit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robot-soccer-kit
-Version: 2.1.0
+Version: 2.1.1
 Summary: Robot Soccer Kit
 Home-page: https://github.com/rhoban/robot-soccer-kit/
 Author: Rhoban team
 Author-email: team@rhoban.com
 License: UNKNOWN
 Keywords: robot holonomic omniwheel ssl robocup junior soccer standard localized tracking
 Platform: UNKNOWN
```

### Comparing `robot-soccer-kit-2.1.0/robot_soccer_kit.egg-info/SOURCES.txt` & `robot-soccer-kit-2.1.1/robot_soccer_kit.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -126,14 +126,15 @@
 rsk/static/imgs/robot.svg
 rsk/static/imgs/robotblue1.svg
 rsk/static/imgs/robotblue2.svg
 rsk/static/imgs/robotgreen1.svg
 rsk/static/imgs/robotgreen2.svg
 rsk/static/jquery/jquery.js
 rsk/static/js/app.js
+rsk/static/js/competition.js
 rsk/static/js/control.js
 rsk/static/js/referee.js
 rsk/static/js/robots.js
 rsk/static/js/simulator.js
 rsk/static/js/tabs.js
 rsk/static/js/utils.js
 rsk/static/js/video.js
```

### Comparing `robot-soccer-kit-2.1.0/rsk/api.py` & `robot-soccer-kit-2.1.1/rsk/api.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/backend.py` & `robot-soccer-kit-2.1.1/rsk/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,20 @@
     utils,
     constants,
     simulator,
 )
 
 
 class Backend:
-    def __init__(self, simulated=False):
+    def __init__(self, simulated=False, competition=False):
         super().__init__()
         robots.Robots.protocols["serial"] = robot_serial.RobotSerial
 
         self.simulated = simulated
+        self.competition = competition
 
         self.state: state.State = state.State(30, self.simulated)
         self.state.start_pub()
 
         self.referee: referee.Referee = referee.Referee(self.state)
         self.control: control.Control = self.referee.control
         self.robots: robots.Robots = robots.Robots(self.state)
@@ -37,14 +38,17 @@
             self.detection: detection.Detection = self.video.detection
             self.detection.state = self.state
             self.detection.referee = self.referee
 
         self.control.robots = self.robots
         self.control.start()
 
+    def is_competition(self):
+        return self.competition
+
     def is_simulated(self):
         return self.simulated
 
     def cameras(self):
         return self.video.cameras()
 
     def constants(self) -> dict:
```

### Comparing `robot-soccer-kit-2.1.0/rsk/client.py` & `robot-soccer-kit-2.1.1/rsk/client.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/constants.py` & `robot-soccer-kit-2.1.1/rsk/constants.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/control.py` & `robot-soccer-kit-2.1.1/rsk/control.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/detection.py` & `robot-soccer-kit-2.1.1/rsk/detection.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/dumb_ia.py` & `robot-soccer-kit-2.1.1/rsk/dumb_ia.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/dump_referee.py` & `robot-soccer-kit-2.1.1/rsk/dump_referee.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/field.py` & `robot-soccer-kit-2.1.1/rsk/field.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/game_controller.py` & `robot-soccer-kit-2.1.1/rsk/game_controller.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,19 +17,20 @@
 logging.getLogger("werkzeug").setLevel(logging.CRITICAL)
 logging.getLogger("robot-soccer-kit").info("Starting robot-soccer-kit Game Controller")
 
 parser = argparse.ArgumentParser()
 parser.add_argument("--port", "-p", type=str, default="7070")
 parser.add_argument("--ip", "-ip", type=str, default="127.0.0.1")
 parser.add_argument("--simulated", "-s", action="store_true")
+parser.add_argument("--competition", "-c", action="store_true")
 args = parser.parse_args()
 
 
 has_client: bool = False
-backend: Backend = Backend(args.simulated)
+backend: Backend = Backend(args.simulated, args.competition)
 api.register(backend)
 
 # Starting a Flask app serving API requests and files of static/ directory
 static = os.path.dirname(__file__) + "/static/"
 app = Flask("Game controller", static_folder=static)
 CORS(app)
```

### Comparing `robot-soccer-kit-2.1.0/rsk/kinematics.py` & `robot-soccer-kit-2.1.1/rsk/kinematics.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/place.py` & `robot-soccer-kit-2.1.1/rsk/place.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/referee.py` & `robot-soccer-kit-2.1.1/rsk/referee.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/robot.py` & `robot-soccer-kit-2.1.1/rsk/robot.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/robot_serial.py` & `robot-soccer-kit-2.1.1/rsk/robot_serial.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/robots.py` & `robot-soccer-kit-2.1.1/rsk/robots.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/simulator.py` & `robot-soccer-kit-2.1.1/rsk/simulator.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/state.py` & `robot-soccer-kit-2.1.1/rsk/state.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-grid.css` & `robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-grid.css.map` & `robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-grid.min.css` & `robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-grid.min.css.map` & `robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-grid.rtl.css` & `robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-grid.rtl.css.map` & `robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-grid.rtl.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css` & `robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css.map` & `robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-reboot.css` & `robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-reboot.css.map` & `robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-reboot.min.css` & `robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-reboot.min.css.map` & `robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css` & `robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css.map` & `robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css` & `robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css.map` & `robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-utilities.css` & `robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-utilities.css.map` & `robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-utilities.min.css` & `robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-utilities.min.css.map` & `robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-utilities.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css` & `robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css.map` & `robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css` & `robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css.map` & `robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap.css` & `robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap.css.map` & `robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap.min.css` & `robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap.min.css.map` & `robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap.rtl.css` & `robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap.rtl.css.map` & `robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap.rtl.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap.rtl.min.css` & `robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap.rtl.min.css.map` & `robot-soccer-kit-2.1.1/rsk/static/bootstrap/css/bootstrap.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.bundle.js` & `robot-soccer-kit-2.1.1/rsk/static/bootstrap/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.bundle.js.map` & `robot-soccer-kit-2.1.1/rsk/static/bootstrap/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.bundle.min.js` & `robot-soccer-kit-2.1.1/rsk/static/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.bundle.min.js.map` & `robot-soccer-kit-2.1.1/rsk/static/bootstrap/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.esm.js` & `robot-soccer-kit-2.1.1/rsk/static/bootstrap/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.esm.js.map` & `robot-soccer-kit-2.1.1/rsk/static/bootstrap/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.esm.min.js` & `robot-soccer-kit-2.1.1/rsk/static/bootstrap/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.esm.min.js.map` & `robot-soccer-kit-2.1.1/rsk/static/bootstrap/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.js` & `robot-soccer-kit-2.1.1/rsk/static/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.js.map` & `robot-soccer-kit-2.1.1/rsk/static/bootstrap/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.min.js` & `robot-soccer-kit-2.1.1/rsk/static/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.min.js.map` & `robot-soccer-kit-2.1.1/rsk/static/bootstrap/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/css/app.css` & `robot-soccer-kit-2.1.1/rsk/static/css/app.css`

 * *Files 2% similar despite different names*

```diff
@@ -183,7 +183,11 @@
 .progress-large{
     height: 20px;
 }
 
 .card-header {
     text-transform: capitalize;
 }
+
+.competition-mode {
+    display:none;
+}
```

### Comparing `robot-soccer-kit-2.1.0/rsk/static/favicon.ico` & `robot-soccer-kit-2.1.1/rsk/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/icons/.fantasticonrc.js` & `robot-soccer-kit-2.1.1/rsk/static/icons/.fantasticonrc.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/icons/.github/ISSUE_TEMPLATE/bug_report.md` & `robot-soccer-kit-2.1.1/rsk/static/icons/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/icons/.github/preview.png` & `robot-soccer-kit-2.1.1/rsk/static/icons/.github/preview.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/icons/.github/release-drafter.yml` & `robot-soccer-kit-2.1.1/rsk/static/icons/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/icons/.github/workflows/codeql.yml` & `robot-soccer-kit-2.1.1/rsk/static/icons/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/icons/.github/workflows/deploy.yml` & `robot-soccer-kit-2.1.1/rsk/static/icons/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/icons/.github/workflows/test.yml` & `robot-soccer-kit-2.1.1/rsk/static/icons/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/icons/LICENSE.md` & `robot-soccer-kit-2.1.1/rsk/static/icons/LICENSE.md`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/icons/README.md` & `robot-soccer-kit-2.1.1/rsk/static/icons/README.md`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/icons/bootstrap-icons.svg` & `robot-soccer-kit-2.1.1/rsk/static/icons/bootstrap-icons.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/icons/config.yml` & `robot-soccer-kit-2.1.1/rsk/static/icons/config.yml`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/icons/font/bootstrap-icons.css` & `robot-soccer-kit-2.1.1/rsk/static/icons/font/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/icons/font/bootstrap-icons.json` & `robot-soccer-kit-2.1.1/rsk/static/icons/font/bootstrap-icons.json`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/icons/font/fonts/bootstrap-icons.woff` & `robot-soccer-kit-2.1.1/rsk/static/icons/font/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/icons/font/fonts/bootstrap-icons.woff2` & `robot-soccer-kit-2.1.1/rsk/static/icons/font/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/icons/font/index.html` & `robot-soccer-kit-2.1.1/rsk/static/icons/font/index.html`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/icons/package-lock.json` & `robot-soccer-kit-2.1.1/rsk/static/icons/package-lock.json`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/icons/package.json` & `robot-soccer-kit-2.1.1/rsk/static/icons/package.json`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/icons/svg-sprite.json` & `robot-soccer-kit-2.1.1/rsk/static/icons/svg-sprite.json`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/icons/svgo.config.js` & `robot-soccer-kit-2.1.1/rsk/static/icons/svgo.config.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/imgs/ball.png` & `robot-soccer-kit-2.1.1/rsk/static/imgs/ball.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/imgs/ball_16x16.png` & `robot-soccer-kit-2.1.1/rsk/static/imgs/ball_16x16.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/imgs/ball_24x24.png` & `robot-soccer-kit-2.1.1/rsk/static/imgs/ball_24x24.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/imgs/ball_256x256.png` & `robot-soccer-kit-2.1.1/rsk/static/imgs/ball_256x256.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/imgs/ball_32x32.png` & `robot-soccer-kit-2.1.1/rsk/static/imgs/ball_32x32.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/imgs/ball_48x48.png` & `robot-soccer-kit-2.1.1/rsk/static/imgs/ball_48x48.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/imgs/field.png` & `robot-soccer-kit-2.1.1/rsk/static/imgs/field.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/imgs/field.svg` & `robot-soccer-kit-2.1.1/rsk/static/imgs/field.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/imgs/robot.svg` & `robot-soccer-kit-2.1.1/rsk/static/imgs/robot.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/imgs/robotblue1.svg` & `robot-soccer-kit-2.1.1/rsk/static/imgs/robotblue1.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/imgs/robotblue2.svg` & `robot-soccer-kit-2.1.1/rsk/static/imgs/robotblue2.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/imgs/robotgreen1.svg` & `robot-soccer-kit-2.1.1/rsk/static/imgs/robotgreen1.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/imgs/robotgreen2.svg` & `robot-soccer-kit-2.1.1/rsk/static/imgs/robotgreen2.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/index.html` & `robot-soccer-kit-2.1.1/rsk/static/index.html`

 * *Files 11% similar despite different names*

```diff
@@ -1,214 +1,225 @@
 <!DOCTYPE html>
 <html>
-    <head>
-        <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
-        <link rel="stylesheet" type="text/css" href="static/bootstrap/css/bootstrap.min.css" />
-        <link rel="stylesheet" type="text/css" href="static/icons/font/bootstrap-icons.css" />
-        <link rel="stylesheet" type="text/css" href="static/css/app.css" />
-        <script type="text/javascript" src="static/jquery/jquery.js"></script>
-        <script type="text/javascript" src="static/bootstrap/js/bootstrap.bundle.min.js"></script>
-        <script type="text/javascript" src="static/js/utils.js"></script>
-        <script type="text/javascript" src="static/js/video.js"></script>
-        <script type="text/javascript" src="static/js/robots.js"></script>
-        <script type="text/javascript" src="static/js/referee.js"></script>
-        <script type="text/javascript" src="static/js/simulator.js"></script>
-        <script type="text/javascript" src="static/js/control.js"></script>
-        <script type="text/javascript" src="static/js/tabs.js"></script>
-        <script type="text/javascript" src="static/js/app.js"></script>
-        <link rel="shortcut icon" href="static/favicon.ico" type="image/x-icon">
-        <title>Robot Soccer Kit</title>
-    </head>
-
-      <nav class="navbar navbar-expand navbar-dark bg-dark">
-        <div class="container-fluid">
-          <a class="navbar-brand" href="#">
+<head>
+<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
+<link rel="stylesheet" type="text/css" href="static/bootstrap/css/bootstrap.min.css" />
+<link rel="stylesheet" type="text/css" href="static/icons/font/bootstrap-icons.css" />
+<link rel="stylesheet" type="text/css" href="static/css/app.css" />
+<script type="text/javascript" src="static/jquery/jquery.js"></script>
+<script type="text/javascript" src="static/bootstrap/js/bootstrap.bundle.min.js"></script>
+<script type="text/javascript" src="static/js/utils.js"></script>
+<script type="text/javascript" src="static/js/video.js"></script>
+<script type="text/javascript" src="static/js/robots.js"></script>
+<script type="text/javascript" src="static/js/referee.js"></script>
+<script type="text/javascript" src="static/js/simulator.js"></script>
+<script type="text/javascript" src="static/js/competition.js"></script>
+<script type="text/javascript" src="static/js/control.js"></script>
+<script type="text/javascript" src="static/js/tabs.js"></script>
+<script type="text/javascript" src="static/js/app.js"></script>
+<link rel="shortcut icon" href="static/favicon.ico" type="image/x-icon">
+<title>Robot Soccer Kit</title>
+</head>
+
+<nav class="navbar navbar-expand navbar-dark bg-dark">
+    <div class="container-fluid">
+        <a class="navbar-brand" href="#">
             <img src="static/imgs/ball.png" width="32" />
             Robot Soccer Kit
-          </a>
-          
-          <ul class="navbar-nav">
-            <li  class="nav-item secondary nav-tab not_show_simulated" rel="vision">
-              <a class="nav-link active" aria-current="page" href="#">
-                <span class="input-group">
-                  <i class="bi bi-webcam"></i>&nbsp;
-                  Vision&nbsp;
-                  <i class="text-warning bi bi-exclamation-circle vision-has-error"></i>
-                  <i class="text-success bi bi-check-lg vision-has-no-error"></i>
-                </span>
-              </a>
+        </a>
+
+        <ul class="navbar-nav">
+            <li class="nav-item secondary nav-tab not_show_simulated" rel="vision">
+                <a class="nav-link active" aria-current="page" href="#">
+                    <span class="input-group">
+                        <i class="bi bi-webcam"></i>&nbsp;
+                        Vision&nbsp;
+                        <i class="text-warning bi bi-exclamation-circle vision-has-error"></i>
+                        <i class="text-success bi bi-check-lg vision-has-no-error"></i>
+                    </span>
+                </a>
             </li>
             <li class="nav-item secondary nav-tab not_show_simulated" rel="robots">
-              <a class="nav-link" href="#">
-                <i class="bi bi-gear"></i>&nbsp;
-                Robots&nbsp;
-                [<span class="text-success robots-ok">0</span>/<span class="text-success robots-count">0</span>]
-                <i class="text-warning bi bi-exclamation-circle robots-show-warning"></i>
-              </a>
+                <a class="nav-link" href="#">
+                    <i class="bi bi-gear"></i>&nbsp;
+                    Robots&nbsp;
+                    [<span class="text-success robots-ok">0</span>/<span class="text-success robots-count">0</span>]
+                    <i class="text-warning bi bi-exclamation-circle robots-show-warning"></i>
+                </a>
             </li>
             <li class="nav-item rounded nav-tab" rel="control">
-              <a class="nav-link" href="#">
-                <i class="bi bi-arrows-move"></i>&nbsp;
-                Control
-                <i class="text-warning bi bi-exclamation-circle control-show-warning"></i>
-              </a>
+                <a class="nav-link" href="#">
+                    <i class="bi bi-arrows-move"></i>&nbsp;
+                    Control
+                    <i class="text-warning bi bi-exclamation-circle control-show-warning"></i>
+                </a>
             </li>
             <li class="nav-item rounded nav-tab" rel="referee">
-              <a class="nav-link" href="#">
-                <i class="bi bi-binoculars"></i>&nbsp;
-                Referee
-              </a>
+                <a class="nav-link" href="#">
+                    <i class="bi bi-binoculars"></i>&nbsp;
+                    Referee
+                </a>
             </li>
-          </ul>
-          
-          <ul class="navbar-nav p-2">
-            <li class="style_fps rounded">
-              <span class="navbar-text p-2 fps">
-              </span>
+            <li class="nav-item rounded nav-tab competition-mode" rel="competition">
+                <a class="nav-link" href="#">
+                    <i class="bi bi-award"></i>&nbsp;
+                    Competition
+                </a>
             </li>
-          </ul>
-        </div>
-      </nav>
-      
-      <div class="p-3 pt-2">
-      <div class="page page-vision">
-        <div class="vision-hide-running">
+        </ul>
 
-          <div class="card">
-            <div class="card-header">
-              <b>Camera detection</b>
-            </div>
-            <div class="card-body">
-              <div class="mb-3">
-                <label>Camera source</label>
-                <select class="m-1 cameras form-select"></select>
-                <select class="m-1 resolutions form-select"></select>
-              </div>
-              <div class="d-flex justify-content-end">
-                <span class="m-1 btn btn-primary refresh-cameras">
-                  <i class="bi bi-arrow-repeat"></i>
-                  Refresh cameras
-                </span>
-                <span class="m-1 btn btn-success start-capture">
-                  <i class="bi bi-play-fill"></i>
-                  Start Vision
+        <ul class="navbar-nav p-2">
+            <li class="style_fps rounded">
+                <span class="navbar-text p-2 fps">
                 </span>
-              </div>
-            </div>  
-          </div>
-        </div>
+            </li>
+        </ul>
+    </div>
+</nav>
 
-        
-        <div class="vision-show-running">
-          <div class="row">
-            <div class="col-md-6">
-              <div class="camera-area d-flex">
-                  <img class="card camera-image w-100" />
-              </div>
-            </div>
+<div class="p-3 pt-2">
+    <div class="page page-vision">
+        <div class="vision-hide-running">
 
-            <div class="col-md-6">
-              <div class="card">
+            <div class="card">
                 <div class="card-header">
-                    <b>Camera detection settings</b>
+                    <b>Camera detection</b>
                 </div>
-                <div class="p-2 card-body ">
-                  <div class="mx-1 row d-flex align-items-center"> 
-                    <div class="col-9 px-0">
-                      <span class="calibrated">
-                      </span>
+                <div class="card-body">
+                    <div class="mb-3">
+                        <label>Camera source</label>
+                        <select class="m-1 cameras form-select"></select>
+                        <select class="m-1 resolutions form-select"></select>
+                    </div>
+                    <div class="d-flex justify-content-end">
+                        <span class="m-1 btn btn-primary refresh-cameras">
+                            <i class="bi bi-arrow-repeat"></i>
+                            Refresh cameras
+                        </span>
+                        <span class="m-1 btn btn-success start-capture">
+                            <i class="bi bi-play-fill"></i>
+                            Start Vision
+                        </span>
                     </div>
-                    <div class="col-3 px-0 text-end">
-                      <span class="btn btn-secondary calibrate-camera">
-                        Calibrate Field
-                      </span>
+                </div>
+            </div>
+        </div>
+
+
+        <div class="vision-show-running">
+            <div class="row">
+                <div class="col-md-6">
+                    <div class="camera-area d-flex">
+                        <img class="card camera-image w-100" />
                     </div>
-                  </div>
+                </div>
 
-                  <hr class="m-2" />
+                <div class="col-md-6">
+                    <div class="card">
+                        <div class="card-header">
+                            <b>Camera detection settings</b>
+                        </div>
+                        <div class="p-2 card-body ">
+                            <div class="mx-1 row d-flex align-items-center">
+                                <div class="col-9 px-0">
+                                    <span class="calibrated">
+                                    </span>
+                                </div>
+                                <div class="col-3 px-0 text-end">
+                                    <span class="btn btn-secondary calibrate-camera">
+                                        Calibrate Field
+                                    </span>
+                                </div>
+                            </div>
 
-                  <div class="camera-settings row">
-                  </div>
-                </label>
+                            <hr class="m-2" />
 
-                  <hr/>
-                  <div class="detection-wrapper">
-                  <code class="detection"></code>
-                  </div>
+                            <div class="camera-settings row">
+                            </div>
+                            </label>
 
-                  <hr/>
-                  <span class="btn btn-danger stop-capture">
-                    <i class="bi bi-stop-fill"></i>&nbsp;
-                    Stop Vision
-                  </span>
+                            <hr />
+                            <div class="detection-wrapper">
+                                <code class="detection"></code>
+                            </div>
+
+                            <hr />
+                            <span class="btn btn-danger stop-capture">
+                                <i class="bi bi-stop-fill"></i>&nbsp;
+                                Stop Vision
+                            </span>
+                        </div>
+                    </div>
                 </div>
-              </div>
             </div>
-          </div>
         </div>
-        <button class="btn btn-outline-light btn-lg settings-button border-0 vision-show-running display-python-settings" type="button" data-bs-toggle="offcanvas" data-bs-target="#offcanvasSettings" aria-controls="offcanvasSettings">
-          <i class="bi bi-gear-fill"></i>
-       </button>
-      </div>
+        <button
+            class="btn btn-outline-light btn-lg settings-button border-0 vision-show-running display-python-settings"
+            type="button" data-bs-toggle="offcanvas" data-bs-target="#offcanvasSettings"
+            aria-controls="offcanvasSettings">
+            <i class="bi bi-gear-fill"></i>
+        </button>
+    </div>
 
-      <div class="page page-robots">
+    <div class="page page-robots">
         <div class="card">
-          <div class="card-header">
-            <b>Adding a robot</b>
-          </div>
-          <div class="card-body">
-            <div class="justify-content-center">
-              <div class="mb-3">
-                <label>URLs</label>
-                <select class="m-1 urls form-select"></select>
-              </div>
-              </div>
-              <div class="d-flex justify-content-end">
-                <span class="m-1 btn btn-danger remove-offline">
-                  <i class="bi bi-trash"></i>
-                  Remove offline
-                </span>
-                <span class="m-1 btn btn-primary refresh-urls">
-                  <i class="bi bi-arrow-repeat"></i>
-                  Refresh URLs
-                </span>
-                <span class="m-1 btn btn-secondary identify">
-                  <i class="bi bi-bullseye"></i>
-                  Identify
-                </span>
-                <span class="m-1 btn btn-success add-all-robots">
-                  <i class="bi bi-asterisk"></i>
-                  Add all
-                </span>
-                <span class="m-1 btn btn-success add-robot">
-                  <i class="bi bi-plus-circle"></i>
-                  Add
-                </span>
-              </div>
+            <div class="card-header">
+                <b>Adding a robot</b>
+            </div>
+            <div class="card-body">
+                <div class="justify-content-center">
+                    <div class="mb-3">
+                        <label>URLs</label>
+                        <select class="m-1 urls form-select"></select>
+                    </div>
+                </div>
+                <div class="d-flex justify-content-end">
+                    <span class="m-1 btn btn-danger remove-offline">
+                        <i class="bi bi-trash"></i>
+                        Remove offline
+                    </span>
+                    <span class="m-1 btn btn-primary refresh-urls">
+                        <i class="bi bi-arrow-repeat"></i>
+                        Refresh URLs
+                    </span>
+                    <span class="m-1 btn btn-secondary identify">
+                        <i class="bi bi-bullseye"></i>
+                        Identify
+                    </span>
+                    <span class="m-1 btn btn-success add-all-robots">
+                        <i class="bi bi-asterisk"></i>
+                        Add all
+                    </span>
+                    <span class="m-1 btn btn-success add-robot">
+                        <i class="bi bi-plus-circle"></i>
+                        Add
+                    </span>
+                </div>
             </div>
         </div>
 
         <div class="robots">
         </div>
-      </div>
+    </div>
 
-      <div class="page page-control">
+    <div class="page page-control">
         <div class="teams"></div>
-      </div>
+    </div>
 
-      <div class="page page-referee">
+    <div class="page page-referee">
         <div class="referee"></div>
 
         <div class="vision-hide-running">
-          <div class="alert alert-warning d-flex align-items-center" role="alert">
-            <div>
-              <i class="bi bi-exclamation-triangle-fill"></i>&nbsp;
-              Detection algorithm is not running, please go to <a href="#" class="alert-link goto-tab" rel="vision">Vision tab</a> to start it.
+            <div class="alert alert-warning d-flex align-items-center" role="alert">
+                <div>
+                    <i class="bi bi-exclamation-triangle-fill"></i>&nbsp;
+                    Detection algorithm is not running, please go to <a href="#" class="alert-link goto-tab"
+                        rel="vision">Vision tab</a> to start it.
+                </div>
             </div>
-          </div>
         </div>
 
         <div class="row">
             <div id="first-col" class="col-7">
                 <div class="row">
                     <div class="col-12">
                         <div class="vision-show-running">
@@ -220,392 +231,430 @@
                                 <canvas id="blue2" class="sim_vim"></canvas>
                                 <canvas id="ball" class="sim_vim"></canvas>
                                 <img id="vision" class="card camera-image m-0" />
                             </div>
                         </div>
                     </div>
                 </div>
-              </div>
-            </div>
-            <div class="row">
-              <div class="col-12 py-2 text-center">
-                <button id="MidTimeChange" class="btn btn-warning btn-sm" data-bs-toggle="modal" data-bs-target="#staticBackdrop" disabled>
-                  <i class="bi bi-arrow-repeat"></i> Half time Change 
-                </button>
-
-                <button id="ViewChange" class="btn btn-secondary btn-sm not_show_simulated" z-index="0">
-                  <i class="bi bi-camera" ></i> Simulated View
-                </button>
-              </div>
-            </div>
-            <div class="row d-flex robot-penalize-tab">
-              <div id="XnegPenalty" class="col-6">
-                <div class="card text-center border-blue">
-                  <div class="card-header bg-head-blue text-light">
-                    <b class="second-team-name">Team 2 Name</b>
-                  </div>
-                  <div class="p-2 card-body bg-body-blue">
-                    <div class="row vert-align mb-3 mt-1 robot-penalty" rel="blue1">
-                      <div class="col-2">
-                        <img
-                        src="static/imgs/robotblue1.svg"
-                        alt="Robot Blue 1"
-                        height="50px"/>
-                      </div>
-                      <div class="col-7">
-                        <div class="row">
-                          <div class="col-12 robot-state">
-                            <h6>Blue 1 State</h6>
-                          </div>
-                        </div>
-                        <div class="row">
-                          <div class="col-12">
-                            <div class="progress progress-large">
-                              <div class="progress-bar progress-bar-striped" role="progressbar" style="width: 100%"></div>
-                            </div>
-                          </div>
-                        </div>
-                      </div>
-                      <div class="col-1 p-0 m-0">
-                        <button class="btn btn-primary btn-sm penalize" disabled>
-                          5s
-                        </button>
-                      </div>
-                      <div class="col-1 p-2 m-0">
-                        <button class="btn btn-danger btn-sm unpenalize" disabled>
-                          <i class="bi bi-x-circle"></i>
-                        </button>
-                      </div>
-                    </div>
-                    <div class="row vert-align mb-1 robot-penalty" rel="blue2">
-                      <div class="col-2">
-                        <img
-                        src="static/imgs/robotblue2.svg"
-                        alt="Robot Blue 2"
-                        height="50px"/>
-                      </div>
-                      <div class="col-7">
-                        <div class="row">
-                          <div class="col-12 robot-state">
-                            <h6>Blue 2 State</h6>
-                          </div>
-                        </div>
-                        <div class="row">
-                          <div class="col-12">
-                            <div class="progress progress-large">
-                              <div class="progress-bar progress-bar-striped" role="progressbar" style="width: 100%"></div>
-                            </div>
-                          </div>
-                        </div>
-                      </div>
-                      <div class="col-1 p-0 m-0">
-                        <button class="btn btn-primary btn-sm penalize" disabled>
-                          5s
+                <div class="row">
+                    <div class="col-12 py-2 text-center">
+                        <button id="MidTimeChange" class="btn btn-warning btn-sm" data-bs-toggle="modal"
+                            data-bs-target="#staticBackdrop" disabled>
+                            <i class="bi bi-arrow-repeat"></i> Half time Change
                         </button>
-                      </div>
-                      <div class="col-1 p-2 m-0">
-                        <button class="btn btn-danger btn-sm unpenalize" disabled>
-                          <i class="bi bi-x-circle"></i>
+
+                        <button id="ViewChange" class="btn btn-secondary btn-sm not_show_simulated" z-index="0">
+                            <i class="bi bi-camera"></i> Simulated View
                         </button>
-                      </div>
                     </div>
-                  </div>
                 </div>
-              </div>
-              <div id="XposPenalty" class="col-6">
-                <div class="card text-center border-green">
-                  <div class="card-header bg-head-green text-light">
-                    <b class="first-team-name">Team 1 Name</b>
-                  </div>
-                  <div id ="green-referee-body" class="p-2 card-body bg-body-green">
-                    <div class="row vert-align mb-3 mt-1 robot-penalty" rel="green1">
-                      <div class="col-2">
-                        <img
-                        src="static/imgs/robotgreen1.svg"
-                        alt="Robot Green 1"
-                        height="50"/>
-                      </div>
-                      <div class="col-7">
-                        <div class="row">
-                          <div class="col-12 robot-state">
-                            <h6>Green 1 State</h6>
-                          </div>
-                        </div>
-                        <div class="row">
-                          <div class="col-12">
-                            <div class="progress progress-large">
-                              <div class="progress-bar progress-bar-striped bg-success" role="progressbar" style="width: 100%"></div>
+                <div class="row d-flex robot-penalize-tab">
+                    <div id="XnegPenalty" class="col-6">
+                        <div class="card text-center border-blue">
+                            <div class="card-header bg-head-blue text-light">
+                                <b class="second-team-name">Team 2 Name</b>
+                            </div>
+                            <div class="p-2 card-body bg-body-blue">
+                                <div class="row vert-align mb-3 mt-1 robot-penalty" rel="blue1">
+                                    <div class="col-2">
+                                        <img src="static/imgs/robotblue1.svg" alt="Robot Blue 1" height="50px" />
+                                    </div>
+                                    <div class="col-7">
+                                        <div class="row">
+                                            <div class="col-12 robot-state">
+                                                <h6>Blue 1 State</h6>
+                                            </div>
+                                        </div>
+                                        <div class="row">
+                                            <div class="col-12">
+                                                <div class="progress progress-large">
+                                                    <div class="progress-bar progress-bar-striped" role="progressbar"
+                                                        style="width: 100%"></div>
+                                                </div>
+                                            </div>
+                                        </div>
+                                    </div>
+                                    <div class="col-1 p-0 m-0">
+                                        <button class="btn btn-primary btn-sm penalize" disabled>
+                                            5s
+                                        </button>
+                                    </div>
+                                    <div class="col-1 p-2 m-0">
+                                        <button class="btn btn-danger btn-sm unpenalize" disabled>
+                                            <i class="bi bi-x-circle"></i>
+                                        </button>
+                                    </div>
+                                </div>
+                                <div class="row vert-align mb-1 robot-penalty" rel="blue2">
+                                    <div class="col-2">
+                                        <img src="static/imgs/robotblue2.svg" alt="Robot Blue 2" height="50px" />
+                                    </div>
+                                    <div class="col-7">
+                                        <div class="row">
+                                            <div class="col-12 robot-state">
+                                                <h6>Blue 2 State</h6>
+                                            </div>
+                                        </div>
+                                        <div class="row">
+                                            <div class="col-12">
+                                                <div class="progress progress-large">
+                                                    <div class="progress-bar progress-bar-striped" role="progressbar"
+                                                        style="width: 100%"></div>
+                                                </div>
+                                            </div>
+                                        </div>
+                                    </div>
+                                    <div class="col-1 p-0 m-0">
+                                        <button class="btn btn-primary btn-sm penalize" disabled>
+                                            5s
+                                        </button>
+                                    </div>
+                                    <div class="col-1 p-2 m-0">
+                                        <button class="btn btn-danger btn-sm unpenalize" disabled>
+                                            <i class="bi bi-x-circle"></i>
+                                        </button>
+                                    </div>
+                                </div>
                             </div>
-                          </div>
                         </div>
-                      </div>
-                      <div class="col-1 p-0 m-0">
-                        <button class="btn btn-success btn-sm penalize" disabled>
-                          5s
-                        </button>
-                      </div>
-                      <div class="col-1 p-2 m-0">
-                        <button class="btn btn-danger btn-sm unpenalize" disabled>
-                          <i class="bi bi-x-circle"></i>
-                        </button>
-                      </div>
                     </div>
-                    <div class="row vert-align mb-1 robot-penalty" rel="green2">
-                      <div class="col-2">
-                        <img
-                        src="static/imgs/robotgreen2.svg"
-                        alt="Robot Green 2"
-                        height="50px"/>
-                      </div>
-                      <div class="col-7">
-                        <div class="row">
-                          <div class="col-12 robot-state">
-                            <h6>Green 2 State</h6>
-                          </div>
-                        </div>
-                        <div class="row">
-                          <div class="col-12">
-                            <div class="progress progress-large">
-                              <div class="progress-bar progress-bar-striped bg-success" role="progressbar" style="width: 100%"></div>
+                    <div id="XposPenalty" class="col-6">
+                        <div class="card text-center border-green">
+                            <div class="card-header bg-head-green text-light">
+                                <b class="first-team-name">Team 1 Name</b>
+                            </div>
+                            <div id="green-referee-body" class="p-2 card-body bg-body-green">
+                                <div class="row vert-align mb-3 mt-1 robot-penalty" rel="green1">
+                                    <div class="col-2">
+                                        <img src="static/imgs/robotgreen1.svg" alt="Robot Green 1" height="50" />
+                                    </div>
+                                    <div class="col-7">
+                                        <div class="row">
+                                            <div class="col-12 robot-state">
+                                                <h6>Green 1 State</h6>
+                                            </div>
+                                        </div>
+                                        <div class="row">
+                                            <div class="col-12">
+                                                <div class="progress progress-large">
+                                                    <div class="progress-bar progress-bar-striped bg-success"
+                                                        role="progressbar" style="width: 100%"></div>
+                                                </div>
+                                            </div>
+                                        </div>
+                                    </div>
+                                    <div class="col-1 p-0 m-0">
+                                        <button class="btn btn-success btn-sm penalize" disabled>
+                                            5s
+                                        </button>
+                                    </div>
+                                    <div class="col-1 p-2 m-0">
+                                        <button class="btn btn-danger btn-sm unpenalize" disabled>
+                                            <i class="bi bi-x-circle"></i>
+                                        </button>
+                                    </div>
+                                </div>
+                                <div class="row vert-align mb-1 robot-penalty" rel="green2">
+                                    <div class="col-2">
+                                        <img src="static/imgs/robotgreen2.svg" alt="Robot Green 2" height="50px" />
+                                    </div>
+                                    <div class="col-7">
+                                        <div class="row">
+                                            <div class="col-12 robot-state">
+                                                <h6>Green 2 State</h6>
+                                            </div>
+                                        </div>
+                                        <div class="row">
+                                            <div class="col-12">
+                                                <div class="progress progress-large">
+                                                    <div class="progress-bar progress-bar-striped bg-success"
+                                                        role="progressbar" style="width: 100%"></div>
+                                                </div>
+                                            </div>
+                                        </div>
+                                    </div>
+                                    <div class="col-1 p-0 m-0">
+                                        <button class="btn btn-success btn-sm penalize" disabled>
+                                            5s
+                                        </button>
+                                    </div>
+                                    <div class="col-1 p-2 m-0">
+                                        <button class="btn btn-danger btn-sm unpenalize" disabled>
+                                            <i class="bi bi-x-circle"></i>
+                                        </button>
+                                    </div>
+                                </div>
                             </div>
-                          </div>
                         </div>
-                      </div>
-                      <div class="col-1 p-0 m-0">
-                        <button class="btn btn-success btn-sm penalize" disabled>
-                          5s
-                        </button>
-                      </div>
-                      <div class="col-1 p-2 m-0">
-                        <button class="btn btn-danger btn-sm unpenalize" disabled>
-                          <i class="bi bi-x-circle"></i>
-                        </button>
-                      </div>
                     </div>
-                  </div>
                 </div>
-              </div>
             </div>
-          </div>
-          <div class="col-5">
-            <div class="row">
-              <div class="col-12">
-                <span class="mb-2 btn btn-success w-100 start-game">
-                  <i class="bi bi-play-fill"></i>&nbsp;
-                  Start Game
-                </span>
-                <span class="mb-2 btn-group pause-game-grp d-flex d-none" role="group">
-                  <span class="btn btn-warning pause-game w-100">
-                    <i class="bi bi-pause-fill"></i>&nbsp;
-                    Pause Game
-                  </span>
-                  <span class="btn btn-danger stop-game w-100">
-                    <i class="bi bi-stop-fill"></i>&nbsp;
-                    End Game
-                  </span>
-                </span>
-                <span class="mb-2 btn-group resume-game-grp d-flex d-none" role="group">
-                  <button class="btn btn-success resume-game w-100">
-                    <i class="bi bi-play-fill"></i>&nbsp;
-                    Resume Game
-                  </button>
-                  <span class="btn btn-danger stop-game w-100">
-                    <i class="bi bi-stop-fill"></i>&nbsp;
-                    End Game
-                  </span>
-                </span>
-              </div>
-            </div>
-            <div class="row">
-              <div class="col-12">
-                <div class="card text-center">
-                  <div class="card-header">
-                    <h5 class="mb-0 GameState">...</h5>
-                  </div>
-                  <div class="p-2 card-body">
-                    <div class="row align-items-center">
-                      <div class="col-3">
-                        <div class="card bg-body-green m-1">
-                          <div class="card-body p-2" >
-                            <h1 class="mb-1" id="GreenScore"></h1>
-                          </div>
-                        </div>
-                      </div>
-                      <div class="col-1 p-0 score-zone" rel="green">
-                        <div class="row">
-                          <div class="col-12">
-                            <button class="btn rounded-circle btn-success btn-sm up-score bg-head-green" disabled>
-                              <i class="bi bi-caret-up-fill"></i>
-                            </button>
-                          </div>
-                        </div>
-                        <div class="row">
-                          <div class="col-12">
-                            <button class="btn rounded-circle btn-success btn-sm down-score bg-head-green" disabled>
-                              <i class="bi bi-caret-down-fill"></i>
+            <div class="col-5">
+                <div class="row">
+                    <div class="col-12">
+                        <span class="mb-2 btn btn-success w-100 start-game">
+                            <i class="bi bi-play-fill"></i>&nbsp;
+                            Start Game
+                        </span>
+                        <span class="mb-2 btn-group pause-game-grp d-flex d-none" role="group">
+                            <span class="btn btn-warning pause-game w-100">
+                                <i class="bi bi-pause-fill"></i>&nbsp;
+                                Pause Game
+                            </span>
+                            <span class="btn btn-danger stop-game w-100">
+                                <i class="bi bi-stop-fill"></i>&nbsp;
+                                End Game
+                            </span>
+                        </span>
+                        <span class="mb-2 btn-group resume-game-grp d-flex d-none" role="group">
+                            <button class="btn btn-success resume-game w-100">
+                                <i class="bi bi-play-fill"></i>&nbsp;
+                                Resume Game
                             </button>
-                          </div>
-                        </div>
-                      </div>
-                      <div class="col-4 p-0">
-                        <div class="card bg-body-grey m-1 mx-4">
-                          <div class="card-body p-2" >
-                            <h2 class="TimerMinutes mb-1"></h2>
-                          </div>
-                        </div>
-                        <!-- <span class="btn btn-danger reset-score">
+                            <span class="btn btn-danger stop-game w-100">
+                                <i class="bi bi-stop-fill"></i>&nbsp;
+                                End Game
+                            </span>
+                        </span>
+                    </div>
+                </div>
+                <div class="row">
+                    <div class="col-12">
+                        <div class="card text-center">
+                            <div class="card-header">
+                                <h5 class="mb-0 GameState">...</h5>
+                            </div>
+                            <div class="p-2 card-body">
+                                <div class="row align-items-center">
+                                    <div class="col-3">
+                                        <div class="card bg-body-green m-1">
+                                            <div class="card-body p-2">
+                                                <h1 class="mb-1" id="GreenScore"></h1>
+                                            </div>
+                                        </div>
+                                    </div>
+                                    <div class="col-1 p-0 score-zone" rel="green">
+                                        <div class="row">
+                                            <div class="col-12">
+                                                <button
+                                                    class="btn rounded-circle btn-success btn-sm up-score bg-head-green"
+                                                    disabled>
+                                                    <i class="bi bi-caret-up-fill"></i>
+                                                </button>
+                                            </div>
+                                        </div>
+                                        <div class="row">
+                                            <div class="col-12">
+                                                <button
+                                                    class="btn rounded-circle btn-success btn-sm down-score bg-head-green"
+                                                    disabled>
+                                                    <i class="bi bi-caret-down-fill"></i>
+                                                </button>
+                                            </div>
+                                        </div>
+                                    </div>
+                                    <div class="col-4 p-0">
+                                        <div class="card bg-body-grey m-1 mx-4">
+                                            <div class="card-body p-2">
+                                                <h2 class="TimerMinutes mb-1"></h2>
+                                            </div>
+                                        </div>
+                                        <!-- <span class="btn btn-danger reset-score">
                           Reset
                         </span> -->
-                      </div>
-                      <div class="col-1 p-0 score-zone" rel="blue">
-                        <div class="row">
-                          <div class="col-12">
-                            <button class="btn rounded-circle btn-primary btn-sm up-score bg-head-blue" disabled>
-                              <i class="bi bi-caret-up-fill"></i>
-                            </button>
-                          </div>
-                        </div>
-                        <div class="row">
-                          <div class="col-12">
-                            <button class="btn rounded-circle btn-primary btn-sm down-score bg-head-blue" disabled>
-                              <i class="bi bi-caret-down-fill"></i>
-                            </button>
-                          </div>
-                        </div>
-                      </div>
-                      <div class="col-3">
-                        <div class="card bg-body-blue m-1">
-                          <div class="card-body p-2">
-                            <h1 class="mb-1" id="BlueScore"></h1>
-                          </div>
+                                    </div>
+                                    <div class="col-1 p-0 score-zone" rel="blue">
+                                        <div class="row">
+                                            <div class="col-12">
+                                                <button
+                                                    class="btn rounded-circle btn-primary btn-sm up-score bg-head-blue"
+                                                    disabled>
+                                                    <i class="bi bi-caret-up-fill"></i>
+                                                </button>
+                                            </div>
+                                        </div>
+                                        <div class="row">
+                                            <div class="col-12">
+                                                <button
+                                                    class="btn rounded-circle btn-primary btn-sm down-score bg-head-blue"
+                                                    disabled>
+                                                    <i class="bi bi-caret-down-fill"></i>
+                                                </button>
+                                            </div>
+                                        </div>
+                                    </div>
+                                    <div class="col-3">
+                                        <div class="card bg-body-blue m-1">
+                                            <div class="card-body p-2">
+                                                <h1 class="mb-1" id="BlueScore"></h1>
+                                            </div>
+                                        </div>
+                                    </div>
+                                </div>
+                                <div class="row">
+                                    <div class="col-5 pe-5">
+                                        <input class="form-control team-name form_green_border" rel="green" type="text"
+                                            placeholder="Green Team Name">
+                                    </div>
+                                    <div class="col-2">
+                                    </div>
+                                    <div class="col-5 ps-5">
+                                        <input class="form-control team-name text-end" rel="blue" type="text"
+                                            placeholder="Blue Team Name">
+                                    </div>
+                                </div>
+
+                                <div class="row">
+                                    <h6 class="mt-3 mb-0 text-center">
+                                        Set Robots Configuration
+                                    </h6>
+                                    <div class="mt-2 btn-group btn-group-sm d-flex" role="group">
+                                        <button class="btn btn-outline-secondary w-100 side-place">
+                                            Side
+                                        </button>
+                                        <button class="btn btn-secondary w-100 strd-place">
+                                            Standard
+                                        </button>
+                                        <button class="btn btn-outline-secondary w-100 dots-place">
+                                            Dots
+                                        </button>
+                                    </div>
+                                </div>
+                            </div>
                         </div>
-                      </div>
                     </div>
-                    <div  class="row">
-                      <div class="col-5 pe-5">
-                        <input class="form-control team-name form_green_border" rel="green" type="text" placeholder="Green Team Name">
-                      </div>
-                      <div class="col-2">
-                      </div>
-                      <div class="col-5 ps-5">
-                        <input class="form-control team-name text-end" rel="blue" type="text" placeholder="Blue Team Name">
-                      </div>
-                    </div>
-                    
-                    <div class="row">
-                      <h6 class ="mt-3 mb-0 text-center"> 
-                        Set Robots Configuration
-                      </h6>
-                      <div class="mt-2 btn-group btn-group-sm d-flex"  role="group">
-                        <button class="btn btn-outline-secondary w-100 side-place">
-                          Side
-                        </button>
-                        <button class="btn btn-secondary w-100 strd-place">
-                          Standard
-                        </button>
-                        <button class="btn btn-outline-secondary w-100 dots-place">
-                          Dots
-                        </button>
-                      </div>
-                    </div>
-                  </div>
                 </div>
-              </div>
-            </div>
-            <div class="row">
-              <div class="col-12">
-                <div class="card text-center">
-                  <div class="card-header">
-                    <h5 class="mb-0">Referee History</h5>
-                  </div>
-                  <div id="tchat" class="p-2 card-body overflow-auto tchat-dim">
-                    <h6 id="NoHistory"class="text-muted">No History</h6>
-                    <div id="RefereeHistory" class="neutral-position-relative top-0 px-3 w-100">
+                <div class="row">
+                    <div class="col-12">
+                        <div class="card text-center">
+                            <div class="card-header">
+                                <h5 class="mb-0">Referee History</h5>
+                            </div>
+                            <div id="tchat" class="p-2 card-body overflow-auto tchat-dim">
+                                <h6 id="NoHistory" class="text-muted">No History</h6>
+                                <div id="RefereeHistory" class="neutral-position-relative top-0 px-3 w-100">
+                                </div>
+                            </div>
+                        </div>
                     </div>
-                  </div>
                 </div>
-              </div>
             </div>
-          </div>
         </div>
-        <span class="btn btn-outline-dark btn-lg settings-button border-0 vision-show-running display-python-settings" type="button" data-bs-toggle="offcanvas" data-bs-target="#offcanvasSettings" aria-controls="offcanvasSettings">
-          <i class="bi bi-gear-fill"></i>
+        <span class="btn btn-outline-dark btn-lg settings-button border-0 vision-show-running display-python-settings"
+            type="button" data-bs-toggle="offcanvas" data-bs-target="#offcanvasSettings"
+            aria-controls="offcanvasSettings">
+            <i class="bi bi-gear-fill"></i>
         </span>
-      </div>
+    </div>
 
 
-      <!-- Modal -->
-      <div class="modal fade" id="staticBackdrop" data-bs-backdrop="static" data-bs-keyboard="false" tabindex="-1" aria-labelledby="staticBackdropLabel" aria-hidden="true">
+    <!-- Modal -->
+    <div class="modal fade" id="staticBackdrop" data-bs-backdrop="static" data-bs-keyboard="false" tabindex="-1"
+        aria-labelledby="staticBackdropLabel" aria-hidden="true">
         <div class="modal-dialog">
-          <div class="modal-content">
-            <div class="modal-header">
-              <h5 class="modal-title" id="staticBackdropLabel">Half-Time Waiting Room</h5>
-            </div>
-            <div class="modal-body pb-0 text-center">
-              <div class="card bg-body-grey m-1 mx-4">
-                <div class="card-body p-2" >
-                  <h2 class="TimerMinutes mb-1"></h2>
-                </div>
-              </div>
-              <div class="ChangeCover m-2">
-                Do you want to swap robot covers ?
-              </div>
-              <div class="MidTimeIdentifyBefore m-2 d-none">
-                When covers are swapped, please click on "Identify" and wait for Robots identification
-              </div>
-              <div class="MidTimeIdentifyWait m-2 d-none">
-                Wait for Robots identification...
-              </div>
-              <div class="MidTimeIdentifyDone m-2 d-none">
-                Identification Done. Please Continue
-              </div>
-              <div class="SecondHalfTime m-2 d-none">
-                When Half-Time has ended, click on "Start Second Half-Time" to continue the Game
-              </div>
-            </div>
-            <div class="ChangeCover modal-footer d-flex justify-content-center">
-              <button id="Y_ChangeCover" type="button" class="btn btn-success">Yes</button>
-              <button id="N_ChangeCover" type="button" class="btn btn-danger" >No</button>
-            </div>
-            <div class="MidTimeIdentify modal-footer d-flex justify-content-center d-none">
-              <span id="BtnMidTimeIdentify"class="m-1 btn btn-secondary identify">
-                <i class="bi bi-bullseye"></i>
-                Identify
-              </span>
-              <button id="Next_MidTimeIdentify" type="button" class="btn btn-success d-none">Continue</button>
-            </div>
-            <div class="SecondHalfTime modal-footer d-flex justify-content-center d-none">
-              <button id="BtnSecondHalfTime" type="button" class="btn btn-secondary" data-bs-dismiss="modal">Start Second Half-Time</button>
+            <div class="modal-content">
+                <div class="modal-header">
+                    <h5 class="modal-title" id="staticBackdropLabel">Half-Time Waiting Room</h5>
+                </div>
+                <div class="modal-body pb-0 text-center">
+                    <div class="card bg-body-grey m-1 mx-4">
+                        <div class="card-body p-2">
+                            <h2 class="TimerMinutes mb-1"></h2>
+                        </div>
+                    </div>
+                    <div class="ChangeCover m-2">
+                        Do you want to swap robot covers ?
+                    </div>
+                    <div class="MidTimeIdentifyBefore m-2 d-none">
+                        When covers are swapped, please click on "Identify" and wait for Robots identification
+                    </div>
+                    <div class="MidTimeIdentifyWait m-2 d-none">
+                        Wait for Robots identification...
+                    </div>
+                    <div class="MidTimeIdentifyDone m-2 d-none">
+                        Identification Done. Please Continue
+                    </div>
+                    <div class="SecondHalfTime m-2 d-none">
+                        When Half-Time has ended, click on "Start Second Half-Time" to continue the Game
+                    </div>
+                </div>
+                <div class="ChangeCover modal-footer d-flex justify-content-center">
+                    <button id="Y_ChangeCover" type="button" class="btn btn-success">Yes</button>
+                    <button id="N_ChangeCover" type="button" class="btn btn-danger">No</button>
+                </div>
+                <div class="MidTimeIdentify modal-footer d-flex justify-content-center d-none">
+                    <span id="BtnMidTimeIdentify" class="m-1 btn btn-secondary identify">
+                        <i class="bi bi-bullseye"></i>
+                        Identify
+                    </span>
+                    <button id="Next_MidTimeIdentify" type="button" class="btn btn-success d-none">Continue</button>
+                </div>
+                <div class="SecondHalfTime modal-footer d-flex justify-content-center d-none">
+                    <button id="BtnSecondHalfTime" type="button" class="btn btn-secondary" data-bs-dismiss="modal">Start
+                        Second Half-Time</button>
+                </div>
             </div>
-          </div>
         </div>
-      </div>
+    </div>
 
-      <!-- Settings Panel -->
-      <div class="offcanvas offcanvas-start" tabindex="-1" id="offcanvasSettings" aria-labelledby="offcanvasSettingsLabel">
+    <!-- Settings Panel -->
+    <div class="offcanvas offcanvas-start" tabindex="-1" id="offcanvasSettings"
+        aria-labelledby="offcanvasSettingsLabel">
         <div class="offcanvas-header">
-          <h4 class="offcanvas-title" id="offcanvasSettingsLabel">Settings</h4>
-          <button type="button" class="btn-close text-reset" data-bs-dismiss="offcanvas" aria-label="Close"></button>
+            <h4 class="offcanvas-title" id="offcanvasSettingsLabel">Settings</h4>
+            <button type="button" class="btn-close text-reset" data-bs-dismiss="offcanvas" aria-label="Close"></button>
         </div>
         <div class="offcanvas-body pt-0">
-          <div class="pb-4">
-            Here, you can change what is drawn on the camera image (disabling drawings can improve performances for slow computers)
-          </div>
-          <div class="display-settings"></div>
-          <div class="btn-group pt-4" role="group" aria-label="Basic mixed styles example">
-            <button type="button" id = "default-settings" class="btn btn-outline-warning">
-              Default
-              <i class="bi bi-arrow-counterclockwise"></i>
-            </button>
-          </div>
+            <div class="pb-4">
+                Here, you can change what is drawn on the camera image (disabling drawings can improve performances for
+                slow computers)
+            </div>
+            <div class="display-settings"></div>
+            <div class="btn-group pt-4" role="group" aria-label="Basic mixed styles example">
+                <button type="button" id="default-settings" class="btn btn-outline-warning">
+                    Default
+                    <i class="bi bi-arrow-counterclockwise"></i>
+                </button>
+            </div>
+        </div>
+    </div>
+    <!-- End Settings Panel -->
+
+    <div class="page page-competition competition-mode">
+        <table class="table table-striped">
+            <tr>
+                <th>
+                    Team
+                </th>
+                <th>
+                    Action
+                </th>
+            </tr>
+            
+            <tbody class="competition-teams">
+            </tbody>
+        </table>
+
+        <hr/>
+
+        <div class="card">
+            <div class="card-header col-sm-10">
+                Add a team
+            </div>
+            <div class="card-body">
+                Team name: <input class="form-control add-team-name" type="text" /><br/>
+                Team password: <input class="form-control add-team-password" type="password" />
+                <hr/>
+                <input type="submit" class="form-control btn btn-success add-team">
+            </div>
         </div>
-      </div>
-      <!-- End Settings Panel -->
+    </div>
 
     <div class="emergency-button p-2">
-      <span class="btn emergency btn-danger">
-        <i class="bi bi-slash-circle"></i>
-        Emergency
-      </span>
+        <span class="btn emergency btn-danger">
+            <i class="bi bi-slash-circle"></i>
+            Emergency
+        </span>
     </div>
     </body>
+
 </html>
```

#### html2text {}

```diff
@@ -3,14 +3,15 @@
 
 
 [static/imgs/ball.png]_Robot_Soccer_Kit
     *   _Vision 
     *  _Robots _[0/0]
     *  _Control
     *  _Referee
+    *  _Competition
     *
 Camera detection
   Refresh cameras    Start Vision
 [Image]
 Camera detection settings
 
  Calibrate Field
@@ -67,8 +68,15 @@
 Yes No
   Identify  Continue
 Start Second Half-Time
 *** Settings ***
 Here, you can change what is drawn on the camera image (disabling drawings can
 improve performances for slow computers)
  Default
+Team Action
+===============================================================================
+Add a team
+Team name: [                    ]
+Team password: [********************]
+===============================================================================
+[Submit]
   Emergency
```

### Comparing `robot-soccer-kit-2.1.0/rsk/static/jquery/jquery.js` & `robot-soccer-kit-2.1.1/rsk/static/jquery/jquery.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/js/control.js` & `robot-soccer-kit-2.1.1/rsk/static/js/control.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/js/referee.js` & `robot-soccer-kit-2.1.1/rsk/static/js/referee.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/js/robots.js` & `robot-soccer-kit-2.1.1/rsk/static/js/robots.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/js/simulator.js` & `robot-soccer-kit-2.1.1/rsk/static/js/simulator.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/js/video.js` & `robot-soccer-kit-2.1.1/rsk/static/js/video.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/markers/blue1.svg` & `robot-soccer-kit-2.1.1/rsk/static/markers/blue1.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/markers/blue2.svg` & `robot-soccer-kit-2.1.1/rsk/static/markers/blue2.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/markers/green1.svg` & `robot-soccer-kit-2.1.1/rsk/static/markers/green1.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/markers/green2.svg` & `robot-soccer-kit-2.1.1/rsk/static/markers/green2.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/referee_event_team.html` & `robot-soccer-kit-2.1.1/rsk/static/referee_event_team.html`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/robot.html` & `robot-soccer-kit-2.1.1/rsk/static/robot.html`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/static/team.html` & `robot-soccer-kit-2.1.1/rsk/static/team.html`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/tasks.py` & `robot-soccer-kit-2.1.1/rsk/tasks.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/utils.py` & `robot-soccer-kit-2.1.1/rsk/utils.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/rsk/video.py` & `robot-soccer-kit-2.1.1/rsk/video.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.0/setup.py` & `robot-soccer-kit-2.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         for filename in filenames:
             if '__pycache__' not in path:
                 paths.append(os.path.join('..', path, filename))
     return paths
 
 setuptools.setup(
     name="robot-soccer-kit",
-    version="2.1.0",
+    version="2.1.1",
     author="Rhoban team",
     author_email="team@rhoban.com",
     description="Robot Soccer Kit",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rhoban/robot-soccer-kit/",
     packages=setuptools.find_packages(),
```


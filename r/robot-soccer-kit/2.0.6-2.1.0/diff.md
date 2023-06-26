# Comparing `tmp/robot-soccer-kit-2.0.6.tar.gz` & `tmp/robot-soccer-kit-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robot-soccer-kit-2.0.6.tar", last modified: Sun May 28 14:11:33 2023, max compression
+gzip compressed data, was "robot-soccer-kit-2.1.0.tar", last modified: Mon Jun 26 12:26:17 2023, max compression
```

## Comparing `robot-soccer-kit-2.0.6.tar` & `robot-soccer-kit-2.1.0.tar`

### file list

```diff
@@ -1,164 +1,163 @@
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-05-28 14:11:33.920112 robot-soccer-kit-2.0.6/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      262 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/LICENSE
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1157 2023-05-28 14:11:33.920112 robot-soccer-kit-2.0.6/PKG-INFO
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      588 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/README.md
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-05-28 14:11:33.908112 robot-soccer-kit-2.0.6/robot_soccer_kit.egg-info/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1157 2023-05-28 14:11:33.000000 robot-soccer-kit-2.0.6/robot_soccer_kit.egg-info/PKG-INFO
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4903 2023-05-28 14:11:33.000000 robot-soccer-kit-2.0.6/robot_soccer_kit.egg-info/SOURCES.txt
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)        1 2023-05-28 14:11:33.000000 robot-soccer-kit-2.0.6/robot_soccer_kit.egg-info/dependency_links.txt
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       82 2023-05-28 14:11:33.000000 robot-soccer-kit-2.0.6/robot_soccer_kit.egg-info/requires.txt
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)        4 2023-05-28 14:11:33.000000 robot-soccer-kit-2.0.6/robot_soccer_kit.egg-info/top_level.txt
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-05-28 14:11:33.908112 robot-soccer-kit-2.0.6/rsk/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      102 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/__init__.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      571 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/api.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5422 2023-04-29 10:15:19.000000 robot-soccer-kit-2.0.6/rsk/backend.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    10981 2023-05-28 13:09:30.000000 robot-soccer-kit-2.0.6/rsk/client.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      277 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/config.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3224 2023-05-13 07:36:16.000000 robot-soccer-kit-2.0.6/rsk/constants.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    13616 2023-05-13 07:36:16.000000 robot-soccer-kit-2.0.6/rsk/control.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       35 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/debug.sh
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    18552 2023-04-29 10:39:09.000000 robot-soccer-kit-2.0.6/rsk/detection.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1058 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/dumb_ia.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      571 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/dump_referee.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       73 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/em.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    10173 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/field.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2379 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/game_controller.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2462 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/kinematics.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      445 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/logger.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      602 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/place.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    23624 2023-05-13 07:36:16.000000 robot-soccer-kit-2.0.6/rsk/referee.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2362 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/robot.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    11752 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/robot_serial.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6030 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/robots.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    10231 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/simulator.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2321 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/state.py
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-05-28 14:11:33.908112 robot-soccer-kit-2.0.6/rsk/static/
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-05-28 14:11:33.908112 robot-soccer-kit-2.0.6/rsk/static/bootstrap/
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-05-28 14:11:33.912112 robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    75616 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-grid.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   226018 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-grid.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    56464 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-grid.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   142342 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-grid.min.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    75690 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-grid.rtl.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   226022 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-grid.rtl.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    56539 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   142419 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    11735 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-reboot.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   126626 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-reboot.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     9817 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-reboot.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    51406 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-reboot.min.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    11728 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   126641 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     9889 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    63643 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    96254 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-utilities.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   250681 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-utilities.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    74887 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-utilities.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   163881 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-utilities.min.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    96121 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   250622 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    74815 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   163716 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   267476 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   658460 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   220780 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   568408 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap.min.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   267055 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap.rtl.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   658305 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap.rtl.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   220887 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap.rtl.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   567947 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap.rtl.min.css.map
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-05-28 14:11:33.916112 robot-soccer-kit-2.0.6/rsk/static/bootstrap/js/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   208288 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/bootstrap/js/bootstrap.bundle.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   448884 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/bootstrap/js/bootstrap.bundle.js.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    80599 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/bootstrap/js/bootstrap.bundle.min.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   333974 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/bootstrap/js/bootstrap.bundle.min.js.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   136243 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/bootstrap/js/bootstrap.esm.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   305274 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/bootstrap/js/bootstrap.esm.js.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    74135 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/bootstrap/js/bootstrap.esm.min.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   222070 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/bootstrap/js/bootstrap.esm.min.js.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   145819 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/bootstrap/js/bootstrap.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   306458 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/bootstrap/js/bootstrap.js.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    60554 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/bootstrap/js/bootstrap.min.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   217885 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/bootstrap/js/bootstrap.min.js.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      215 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/camera-setting.html
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-05-28 14:11:33.916112 robot-soccer-kit-2.0.6/rsk/static/css/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2566 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/css/app.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1150 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/favicon.ico
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-05-28 14:11:33.916112 robot-soccer-kit-2.0.6/rsk/static/icons/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      376 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/icons/.browserslistrc
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      167 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/icons/.editorconfig
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       40 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/icons/.eslintignore
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      375 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/icons/.eslintrc.json
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      922 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/icons/.fantasticonrc.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       43 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/icons/.gitattributes
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-05-28 14:11:33.916112 robot-soccer-kit-2.0.6/rsk/static/icons/.github/
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-05-28 14:11:33.916112 robot-soccer-kit-2.0.6/rsk/static/icons/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      583 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/icons/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      122 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/icons/.github/ISSUE_TEMPLATE/icon-request.md
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      433 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/icons/.github/dependabot.yml
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   248086 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/icons/.github/preview.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      572 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/icons/.github/release-drafter.yml
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-05-28 14:11:33.916112 robot-soccer-kit-2.0.6/rsk/static/icons/.github/workflows/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      662 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/icons/.github/workflows/codeql.yml
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1190 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/icons/.github/workflows/deploy.yml
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      243 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/icons/.github/workflows/release-notes.yml
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      575 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/icons/.github/workflows/test.yml
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       63 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/icons/.gitignore
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      125 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/icons/.stylelintrc
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1093 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/icons/LICENSE.md
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3312 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/icons/README.md
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   881772 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/icons/bootstrap-icons.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      425 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/icons/composer.json
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2052 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/icons/config.yml
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-05-28 14:11:33.916112 robot-soccer-kit-2.0.6/rsk/static/icons/font/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    80510 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/icons/font/bootstrap-icons.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    42897 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/icons/font/bootstrap-icons.json
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-05-28 14:11:33.916112 robot-soccer-kit-2.0.6/rsk/static/icons/font/fonts/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   137124 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/icons/font/fonts/bootstrap-icons.woff
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   102536 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/icons/font/fonts/bootstrap-icons.woff2
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   200995 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/icons/font/index.html
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   643115 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/icons/package-lock.json
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3152 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/icons/package.json
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3085 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/icons/svg-sprite.json
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      654 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/icons/svgo.config.js
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-05-28 14:11:33.920112 robot-soccer-kit-2.0.6/rsk/static/imgs/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3287 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/imgs/ball.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1251 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/imgs/ball_16x16.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1856 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/imgs/ball_24x24.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    43069 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/imgs/ball_256x256.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2654 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/imgs/ball_32x32.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4470 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/imgs/ball_48x48.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    19402 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/imgs/field.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    17815 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/imgs/field.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   249649 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/imgs/robot.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   507520 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/imgs/robotblue1.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   524385 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/imgs/robotblue2.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   498488 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/imgs/robotgreen1.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   522425 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/imgs/robotgreen2.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    34869 2023-05-13 07:41:39.000000 robot-soccer-kit-2.0.6/rsk/static/index.html
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-05-28 14:11:33.920112 robot-soccer-kit-2.0.6/rsk/static/jquery/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   288580 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/jquery/jquery.js
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-05-28 14:11:33.920112 robot-soccer-kit-2.0.6/rsk/static/js/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1714 2023-05-13 07:36:16.000000 robot-soccer-kit-2.0.6/rsk/static/js/app.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1713 2023-05-12 17:27:02.000000 robot-soccer-kit-2.0.6/rsk/static/js/competition.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1567 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/js/control.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    13460 2023-05-13 07:36:16.000000 robot-soccer-kit-2.0.6/rsk/static/js/referee.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6005 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/js/robots.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    13773 2023-05-28 14:10:51.000000 robot-soccer-kit-2.0.6/rsk/static/js/simulator.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      426 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/js/tabs.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      329 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/js/utils.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5997 2023-05-13 07:36:16.000000 robot-soccer-kit-2.0.6/rsk/static/js/video.js
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-05-28 14:11:33.920112 robot-soccer-kit-2.0.6/rsk/static/markers/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6021 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/markers/blue1.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6023 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/markers/blue2.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6009 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/markers/green1.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5098 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/markers/green2.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      337 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/referee_event_neutral.html
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      632 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/referee_event_team.html
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1029 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/static/robot.html
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      569 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.6/rsk/static/team.html
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3865 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/tasks.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4154 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/utils.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     9469 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.6/rsk/video.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       38 2023-05-28 14:11:33.920112 robot-soccer-kit-2.0.6/setup.cfg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1391 2023-05-28 14:11:23.000000 robot-soccer-kit-2.0.6/setup.py
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:26:17.952185 robot-soccer-kit-2.1.0/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      262 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/LICENSE
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1157 2023-06-26 12:26:17.952185 robot-soccer-kit-2.1.0/PKG-INFO
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      588 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/README.md
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:26:17.940185 robot-soccer-kit-2.1.0/robot_soccer_kit.egg-info/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1157 2023-06-26 12:26:17.000000 robot-soccer-kit-2.1.0/robot_soccer_kit.egg-info/PKG-INFO
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4874 2023-06-26 12:26:17.000000 robot-soccer-kit-2.1.0/robot_soccer_kit.egg-info/SOURCES.txt
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)        1 2023-06-26 12:26:17.000000 robot-soccer-kit-2.1.0/robot_soccer_kit.egg-info/dependency_links.txt
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       82 2023-06-26 12:26:17.000000 robot-soccer-kit-2.1.0/robot_soccer_kit.egg-info/requires.txt
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)        4 2023-06-26 12:26:17.000000 robot-soccer-kit-2.1.0/robot_soccer_kit.egg-info/top_level.txt
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:26:17.944185 robot-soccer-kit-2.1.0/rsk/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      102 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/__init__.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      571 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/api.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5422 2023-04-29 10:15:19.000000 robot-soccer-kit-2.1.0/rsk/backend.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    10981 2023-06-26 12:26:02.000000 robot-soccer-kit-2.1.0/rsk/client.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      277 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/config.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3224 2023-06-26 12:24:11.000000 robot-soccer-kit-2.1.0/rsk/constants.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    13616 2023-06-26 12:24:11.000000 robot-soccer-kit-2.1.0/rsk/control.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       35 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/debug.sh
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    18552 2023-04-29 10:39:09.000000 robot-soccer-kit-2.1.0/rsk/detection.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1058 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/dumb_ia.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      571 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/dump_referee.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       73 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/em.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    10173 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/field.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2379 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/game_controller.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2462 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/kinematics.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      445 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/logger.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      602 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/place.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    23739 2023-06-26 12:26:02.000000 robot-soccer-kit-2.1.0/rsk/referee.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2362 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/robot.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    11752 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/robot_serial.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6030 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/robots.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    10231 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/simulator.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2321 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/state.py
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:26:17.944185 robot-soccer-kit-2.1.0/rsk/static/
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:26:17.940185 robot-soccer-kit-2.1.0/rsk/static/bootstrap/
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:26:17.944185 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    75616 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-grid.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   226018 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-grid.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    56464 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-grid.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   142342 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-grid.min.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    75690 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-grid.rtl.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   226022 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-grid.rtl.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    56539 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   142419 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    11735 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-reboot.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   126626 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-reboot.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     9817 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-reboot.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    51406 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-reboot.min.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    11728 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   126641 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     9889 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    63643 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    96254 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-utilities.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   250681 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-utilities.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    74887 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-utilities.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   163881 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-utilities.min.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    96121 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   250622 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    74815 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   163716 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   267476 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   658460 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   220780 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   568408 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap.min.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   267055 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap.rtl.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   658305 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap.rtl.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   220887 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap.rtl.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   567947 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap.rtl.min.css.map
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:26:17.948185 robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   208288 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.bundle.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   448884 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.bundle.js.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    80599 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.bundle.min.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   333974 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.bundle.min.js.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   136243 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.esm.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   305274 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.esm.js.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    74135 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.esm.min.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   222070 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.esm.min.js.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   145819 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   306458 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.js.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    60554 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.min.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   217885 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.min.js.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      215 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/camera-setting.html
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:26:17.948185 robot-soccer-kit-2.1.0/rsk/static/css/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2566 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/css/app.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1150 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/favicon.ico
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:26:17.948185 robot-soccer-kit-2.1.0/rsk/static/icons/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      376 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/.browserslistrc
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      167 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/.editorconfig
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       40 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/.eslintignore
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      375 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/.eslintrc.json
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      922 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/.fantasticonrc.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       43 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/.gitattributes
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:26:17.948185 robot-soccer-kit-2.1.0/rsk/static/icons/.github/
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:26:17.948185 robot-soccer-kit-2.1.0/rsk/static/icons/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      583 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      122 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/.github/ISSUE_TEMPLATE/icon-request.md
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      433 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/.github/dependabot.yml
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   248086 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/.github/preview.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      572 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/.github/release-drafter.yml
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:26:17.948185 robot-soccer-kit-2.1.0/rsk/static/icons/.github/workflows/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      662 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/.github/workflows/codeql.yml
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1190 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/.github/workflows/deploy.yml
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      243 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/.github/workflows/release-notes.yml
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      575 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/.github/workflows/test.yml
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       63 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/.gitignore
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      125 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/.stylelintrc
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1093 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/LICENSE.md
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3312 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/README.md
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   881772 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/bootstrap-icons.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      425 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/composer.json
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2052 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/config.yml
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:26:17.948185 robot-soccer-kit-2.1.0/rsk/static/icons/font/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    80510 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/font/bootstrap-icons.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    42897 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/font/bootstrap-icons.json
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:26:17.948185 robot-soccer-kit-2.1.0/rsk/static/icons/font/fonts/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   137124 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/font/fonts/bootstrap-icons.woff
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   102536 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/font/fonts/bootstrap-icons.woff2
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   200995 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/font/index.html
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   643115 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/package-lock.json
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3152 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/package.json
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3085 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/svg-sprite.json
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      654 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/icons/svgo.config.js
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:26:17.952185 robot-soccer-kit-2.1.0/rsk/static/imgs/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3287 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/imgs/ball.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1251 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/imgs/ball_16x16.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1856 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/imgs/ball_24x24.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    43069 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/imgs/ball_256x256.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2654 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/imgs/ball_32x32.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4470 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/imgs/ball_48x48.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    19402 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/imgs/field.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    17815 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/imgs/field.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   249649 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/imgs/robot.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   507520 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/imgs/robotblue1.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   524385 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/imgs/robotblue2.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   498488 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/imgs/robotgreen1.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   522425 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/imgs/robotgreen2.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    27029 2023-06-26 12:25:23.000000 robot-soccer-kit-2.1.0/rsk/static/index.html
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:26:17.952185 robot-soccer-kit-2.1.0/rsk/static/jquery/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   288580 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/jquery/jquery.js
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:26:17.952185 robot-soccer-kit-2.1.0/rsk/static/js/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1714 2023-06-26 12:24:11.000000 robot-soccer-kit-2.1.0/rsk/static/js/app.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1567 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/js/control.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    13425 2023-06-26 12:26:02.000000 robot-soccer-kit-2.1.0/rsk/static/js/referee.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6005 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/js/robots.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    14606 2023-06-26 12:26:02.000000 robot-soccer-kit-2.1.0/rsk/static/js/simulator.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      426 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/js/tabs.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      329 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/js/utils.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5997 2023-06-26 12:24:11.000000 robot-soccer-kit-2.1.0/rsk/static/js/video.js
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-06-26 12:26:17.952185 robot-soccer-kit-2.1.0/rsk/static/markers/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6021 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/markers/blue1.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6023 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/markers/blue2.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6009 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/markers/green1.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5098 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/markers/green2.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      337 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/referee_event_neutral.html
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      632 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/referee_event_team.html
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1029 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/static/robot.html
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      569 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.0/rsk/static/team.html
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3865 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/tasks.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4154 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/utils.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     9469 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.0/rsk/video.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       38 2023-06-26 12:26:17.952185 robot-soccer-kit-2.1.0/setup.cfg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1391 2023-06-26 12:25:51.000000 robot-soccer-kit-2.1.0/setup.py
```

### Comparing `robot-soccer-kit-2.0.6/PKG-INFO` & `robot-soccer-kit-2.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robot-soccer-kit
-Version: 2.0.6
+Version: 2.1.0
 Summary: Robot Soccer Kit
 Home-page: https://github.com/rhoban/robot-soccer-kit/
 Author: Rhoban team
 Author-email: team@rhoban.com
 License: UNKNOWN
 Keywords: robot holonomic omniwheel ssl robocup junior soccer standard localized tracking
 Platform: UNKNOWN
```

### Comparing `robot-soccer-kit-2.0.6/README.md` & `robot-soccer-kit-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/robot_soccer_kit.egg-info/PKG-INFO` & `robot-soccer-kit-2.1.0/robot_soccer_kit.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robot-soccer-kit
-Version: 2.0.6
+Version: 2.1.0
 Summary: Robot Soccer Kit
 Home-page: https://github.com/rhoban/robot-soccer-kit/
 Author: Rhoban team
 Author-email: team@rhoban.com
 License: UNKNOWN
 Keywords: robot holonomic omniwheel ssl robocup junior soccer standard localized tracking
 Platform: UNKNOWN
```

### Comparing `robot-soccer-kit-2.0.6/robot_soccer_kit.egg-info/SOURCES.txt` & `robot-soccer-kit-2.1.0/robot_soccer_kit.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,14 @@
 rsk/static/imgs/robot.svg
 rsk/static/imgs/robotblue1.svg
 rsk/static/imgs/robotblue2.svg
 rsk/static/imgs/robotgreen1.svg
 rsk/static/imgs/robotgreen2.svg
 rsk/static/jquery/jquery.js
 rsk/static/js/app.js
-rsk/static/js/competition.js
 rsk/static/js/control.js
 rsk/static/js/referee.js
 rsk/static/js/robots.js
 rsk/static/js/simulator.js
 rsk/static/js/tabs.js
 rsk/static/js/utils.js
 rsk/static/js/video.js
```

### Comparing `robot-soccer-kit-2.0.6/rsk/api.py` & `robot-soccer-kit-2.1.0/rsk/api.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/backend.py` & `robot-soccer-kit-2.1.0/rsk/backend.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/client.py` & `robot-soccer-kit-2.1.0/rsk/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,24 +35,24 @@
     "side": [
         ["green", 1, (0.2, constants.field_width / 2, -np.pi / 2)],
         ["green", 2, (0.6, constants.field_width / 2, -np.pi / 2)],
         ["blue", 1, (-0.2, constants.field_width / 2, -np.pi / 2)],
         ["blue", 2, (-0.6, constants.field_width / 2, -np.pi / 2)],
     ],
     "swap_covers_green_positive": [
-        ["green", 1, (0.09, -0.2, np.pi)],
-        ["green", 2, (0.09, 0.2, np.pi)],
-        ["blue", 1, (-0.09, -0.2, 0)],
-        ["blue", 2, (-0.09, 0.2, 0)],
+        ["green", 1, (0.15, -0.2, np.pi)],
+        ["green", 2, (0.15, 0.2, np.pi)],
+        ["blue", 1, (-0.15, -0.2, 0)],
+        ["blue", 2, (-0.15, 0.2, 0)],
     ],
     "swap_covers_blue_positive": [
-        ["green", 1, (-0.09, -0.2, 0)],
-        ["green", 2, (-0.09, 0.2, 0)],
-        ["blue", 1, (0.09, -0.2, np.pi)],
-        ["blue", 2, (0.09, 0.2, np.pi)],
+        ["green", 1, (-0.15, -0.2, 0)],
+        ["green", 2, (-0.15, 0.2, 0)],
+        ["blue", 1, (0.15, -0.2, np.pi)],
+        ["blue", 2, (0.15, 0.2, np.pi)],
     ],
     "gently_swap_side": [
         ["green", 1, (0, -0.15, 0)],
         ["green", 2, (0, 0.5, 0)],
         ["blue", 1, (0, -0.5, np.pi)],
         ["blue", 2, (0, 0.15, np.pi)],
     ],
```

### Comparing `robot-soccer-kit-2.0.6/rsk/constants.py` & `robot-soccer-kit-2.1.0/rsk/constants.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/control.py` & `robot-soccer-kit-2.1.0/rsk/control.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/detection.py` & `robot-soccer-kit-2.1.0/rsk/detection.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/dumb_ia.py` & `robot-soccer-kit-2.1.0/rsk/dumb_ia.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/dump_referee.py` & `robot-soccer-kit-2.1.0/rsk/dump_referee.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/field.py` & `robot-soccer-kit-2.1.0/rsk/field.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/game_controller.py` & `robot-soccer-kit-2.1.0/rsk/game_controller.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/kinematics.py` & `robot-soccer-kit-2.1.0/rsk/kinematics.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/place.py` & `robot-soccer-kit-2.1.0/rsk/place.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/referee.py` & `robot-soccer-kit-2.1.0/rsk/referee.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,14 +203,15 @@
         self.game_state["game_state_msg"] = "Game is ready to start"
 
     def start_half_time(self):
         """
         Start an half time break
         """
         self.game_state["timer"] = constants.halftime_duration
+        self.chrono_is_running = True
         self.game_state["game_is_running"] = False
         self.game_state["halftime_is_running"] = True
         self.game_state["game_paused"] = True
         self.game_state["game_state_msg"] = "Half Time"
 
         task = tasks.StopAllTask("half-time")
         self.control.add_task(task)
@@ -219,14 +220,16 @@
         self.control.remove_task("sideline-crossed")
         self.control.remove_task("goal")
 
     def start_second_half_time(self):
         """
         Resume after an half time break
         """
+        self.pause_game("game-start")
+        self.chrono_is_running = False
         self.game_state["timer"] = constants.game_duration
         self.game_state["halftime_is_running"] = False
         self.game_state["game_is_running"] = True
         self.game_state["game_state_msg"] = "Game is running..."
         self.wait_for_ball_placement()
 
     def force_place(self, configuration: str):
```

### Comparing `robot-soccer-kit-2.0.6/rsk/robot.py` & `robot-soccer-kit-2.1.0/rsk/robot.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/robot_serial.py` & `robot-soccer-kit-2.1.0/rsk/robot_serial.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/robots.py` & `robot-soccer-kit-2.1.0/rsk/robots.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/simulator.py` & `robot-soccer-kit-2.1.0/rsk/simulator.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/state.py` & `robot-soccer-kit-2.1.0/rsk/state.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-grid.css` & `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-grid.css.map` & `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-grid.min.css` & `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-grid.min.css.map` & `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-grid.rtl.css` & `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-grid.rtl.css.map` & `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-grid.rtl.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css` & `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css.map` & `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-reboot.css` & `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-reboot.css.map` & `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-reboot.min.css` & `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-reboot.min.css.map` & `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css` & `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css.map` & `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css` & `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css.map` & `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-utilities.css` & `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-utilities.css.map` & `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-utilities.min.css` & `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-utilities.min.css.map` & `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-utilities.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css` & `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css.map` & `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css` & `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css.map` & `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap.css` & `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap.css.map` & `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap.min.css` & `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap.min.css.map` & `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap.rtl.css` & `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap.rtl.css.map` & `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap.rtl.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap.rtl.min.css` & `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/bootstrap/css/bootstrap.rtl.min.css.map` & `robot-soccer-kit-2.1.0/rsk/static/bootstrap/css/bootstrap.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/bootstrap/js/bootstrap.bundle.js` & `robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/bootstrap/js/bootstrap.bundle.js.map` & `robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/bootstrap/js/bootstrap.bundle.min.js` & `robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/bootstrap/js/bootstrap.bundle.min.js.map` & `robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/bootstrap/js/bootstrap.esm.js` & `robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/bootstrap/js/bootstrap.esm.js.map` & `robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/bootstrap/js/bootstrap.esm.min.js` & `robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/bootstrap/js/bootstrap.esm.min.js.map` & `robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/bootstrap/js/bootstrap.js` & `robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/bootstrap/js/bootstrap.js.map` & `robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/bootstrap/js/bootstrap.min.js` & `robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/bootstrap/js/bootstrap.min.js.map` & `robot-soccer-kit-2.1.0/rsk/static/bootstrap/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/css/app.css` & `robot-soccer-kit-2.1.0/rsk/static/css/app.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/favicon.ico` & `robot-soccer-kit-2.1.0/rsk/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/icons/.fantasticonrc.js` & `robot-soccer-kit-2.1.0/rsk/static/icons/.fantasticonrc.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/icons/.github/ISSUE_TEMPLATE/bug_report.md` & `robot-soccer-kit-2.1.0/rsk/static/icons/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/icons/.github/preview.png` & `robot-soccer-kit-2.1.0/rsk/static/icons/.github/preview.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/icons/.github/release-drafter.yml` & `robot-soccer-kit-2.1.0/rsk/static/icons/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/icons/.github/workflows/codeql.yml` & `robot-soccer-kit-2.1.0/rsk/static/icons/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/icons/.github/workflows/deploy.yml` & `robot-soccer-kit-2.1.0/rsk/static/icons/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/icons/.github/workflows/test.yml` & `robot-soccer-kit-2.1.0/rsk/static/icons/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/icons/LICENSE.md` & `robot-soccer-kit-2.1.0/rsk/static/icons/LICENSE.md`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/icons/README.md` & `robot-soccer-kit-2.1.0/rsk/static/icons/README.md`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/icons/bootstrap-icons.svg` & `robot-soccer-kit-2.1.0/rsk/static/icons/bootstrap-icons.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/icons/config.yml` & `robot-soccer-kit-2.1.0/rsk/static/icons/config.yml`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/icons/font/bootstrap-icons.css` & `robot-soccer-kit-2.1.0/rsk/static/icons/font/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/icons/font/bootstrap-icons.json` & `robot-soccer-kit-2.1.0/rsk/static/icons/font/bootstrap-icons.json`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/icons/font/fonts/bootstrap-icons.woff` & `robot-soccer-kit-2.1.0/rsk/static/icons/font/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/icons/font/fonts/bootstrap-icons.woff2` & `robot-soccer-kit-2.1.0/rsk/static/icons/font/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/icons/font/index.html` & `robot-soccer-kit-2.1.0/rsk/static/icons/font/index.html`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/icons/package-lock.json` & `robot-soccer-kit-2.1.0/rsk/static/icons/package-lock.json`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/icons/package.json` & `robot-soccer-kit-2.1.0/rsk/static/icons/package.json`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/icons/svg-sprite.json` & `robot-soccer-kit-2.1.0/rsk/static/icons/svg-sprite.json`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/icons/svgo.config.js` & `robot-soccer-kit-2.1.0/rsk/static/icons/svgo.config.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/imgs/ball.png` & `robot-soccer-kit-2.1.0/rsk/static/imgs/ball.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/imgs/ball_16x16.png` & `robot-soccer-kit-2.1.0/rsk/static/imgs/ball_16x16.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/imgs/ball_24x24.png` & `robot-soccer-kit-2.1.0/rsk/static/imgs/ball_24x24.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/imgs/ball_256x256.png` & `robot-soccer-kit-2.1.0/rsk/static/imgs/ball_256x256.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/imgs/ball_32x32.png` & `robot-soccer-kit-2.1.0/rsk/static/imgs/ball_32x32.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/imgs/ball_48x48.png` & `robot-soccer-kit-2.1.0/rsk/static/imgs/ball_48x48.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/imgs/field.png` & `robot-soccer-kit-2.1.0/rsk/static/imgs/field.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/imgs/field.svg` & `robot-soccer-kit-2.1.0/rsk/static/imgs/field.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/imgs/robot.svg` & `robot-soccer-kit-2.1.0/rsk/static/imgs/robot.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/imgs/robotblue1.svg` & `robot-soccer-kit-2.1.0/rsk/static/imgs/robotblue1.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/imgs/robotblue2.svg` & `robot-soccer-kit-2.1.0/rsk/static/imgs/robotblue2.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/imgs/robotgreen1.svg` & `robot-soccer-kit-2.1.0/rsk/static/imgs/robotgreen1.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/imgs/robotgreen2.svg` & `robot-soccer-kit-2.1.0/rsk/static/imgs/robotgreen2.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/jquery/jquery.js` & `robot-soccer-kit-2.1.0/rsk/static/jquery/jquery.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/js/app.js` & `robot-soccer-kit-2.1.0/rsk/static/js/app.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/js/control.js` & `robot-soccer-kit-2.1.0/rsk/static/js/control.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/js/referee.js` & `robot-soccer-kit-2.1.0/rsk/static/js/referee.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -200,14 +200,15 @@
     });
 
 
     // Half Time
     $('#MidTimeChange').click(function() {
 
         $("#RefereeHistory").append('<h5 class="text-muted m-3">Half Time</h5>');
+        backend.swap_team_sides();
         backend.start_half_time();
     });
 
     $('#ViewChange').click(function() {
 
     });
 
@@ -216,15 +217,14 @@
         $('.MidTimeIdentify').removeClass('d-none');
         $('.MidTimeIdentifyBefore').removeClass('d-none');
         backend.place_game('swap_covers');
     });
 
     $('#N_ChangeCover').click(function() {
         backend.place_game('gently_swap_side');
-        backend.swap_team_sides();
         $('.ChangeCover').addClass('d-none');
         $('.SecondHalfTime').removeClass('d-none');
         setTimeout(function() {
             backend.place_game('standard');
         }, 5000);
 
     });
@@ -234,19 +234,18 @@
         $('.MidTimeIdentifyWait').removeClass('d-none');
         setTimeout(function() {
             $('.MidTimeIdentifyWait').addClass('d-none');
             $('#Next_MidTimeIdentify').removeClass('d-none');
             $('.MidTimeIdentifyDone').removeClass('d-none');
             $('.MidTimeIdentifyDone').removeClass('d-none');
             $('.MidTimeIdentifyWait').addClass('d-none');
-        }, 4000);
+        }, 5000);
     });
 
     $('#Next_MidTimeIdentify').click(function() {
-        backend.swap_team_sides();
         $('#HalfTimePlaceStd').removeClass('d-none');
         $('#Next_MidTimeIdentify').addClass('d-none');
         $('.MidTimeIdentifyDone').addClass('d-none');
         $('.MidTimeIdentify').addClass('d-none');
         $('.MidTimeIdentifyBefore').addClass('d-none');
         $('.SecondHalfTime').removeClass('d-none');
         backend.place_game('standard');
```

### Comparing `robot-soccer-kit-2.0.6/rsk/static/js/robots.js` & `robot-soccer-kit-2.1.0/rsk/static/js/robots.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/js/simulator.js` & `robot-soccer-kit-2.1.0/rsk/static/js/simulator.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -76,15 +76,14 @@
             drawCircle(ball, ballRadius, "orange", ballCanvas, true)
         }
 
         function UpdateView() {
 
             // FPS Limit
             backend.get_state(function(state) {
-
                 if (state.simulated) {
                     tick += 1
                     if (Date.now() - T0 > 100) {
                         $('.fps').text("FPS : " + Math.round(1000 / ((Date.now() - T0) / tick)));
                         T0 = Date.now()
                         tick = 0
                     }
@@ -203,15 +202,15 @@
                 markers[key]["image"].src = "static/imgs/robot" + key + ".svg"
                 canvas = resizeCanvas(document.getElementById(key))
                 markers[key]["context"] = canvas.getContext('2d')
             }
             resizeCanvas(document.getElementById("ball"))
 
             clearInterval(intervalId)
-            intervalId = setInterval(UpdateView, 1000 / 30)
+            intervalId = setInterval(UpdateView, 1000 / fps_limit)
         }
 
         function clearView() {
             clearInterval(intervalId)
             intervalId = NaN
             $('#ViewChange').html("<i class='bi bi-camera'></i> Simulated View")
             $('#vision').removeClass('d-none')
@@ -231,50 +230,69 @@
         function get_display_settings() {
             let html = ''
             for (setting_name in display_settings) {
                 let setting = display_settings[setting_name]
                 let checked = setting["value"] ? 'checked="checked"' : ''
 
                 html += '<div class="form-check form-switch">'
-                html += '    <input class="form-check-input display-setting" type="checkbox" '
+                html += '    <input class="form-check-input display-setting" type="checkbox"'
                 html += 'role="switch" rel="' + setting_name + '" ' + checked + '>'
                 html += '    <label class="form-check-label" for="flexSwitchCheckDefault">'
                 html += '    ' + setting['label']
                 html += '    </label>'
                 html += '</div>'
             }
+            html += '<div class="range">'
+            html += '<label class="form-label" for="flexSwitchCheckDefault">FPS Limit : ' + fps_limit + '</label>'
+            html += '<input id="aaaa" type="range" class="form-range" min="10" max="65" step="5" value="' + fps_limit + '", >'
+            html += '</div>'
+
             $('.display-settings').html(html)
             $('.display-setting').click(function() {
-                console.log($(this).attr('rel'))
-                console.log($(this).is(':checked'))
                 display_settings[$(this).attr('rel')]["value"] = $(this).is(':checked')
             });
+
+            document.querySelector(".range .form-range").addEventListener('input', function(aa) {
+                fps_limit = this.value
+                clearInterval(intervalId)
+                if (fps_limit == 65) {
+                    intervalId = setInterval(UpdateView, 1000 / 240)
+                    $('.form-label').text("FPS Limit : unlimited")
+                } else {
+                    intervalId = setInterval(UpdateView, 1000 / fps_limit)
+                    $('.form-label').text("FPS Limit : " + fps_limit)
+                }
+            })
+
         }
         $('.display-python-settings').click(function() {
             get_display_settings()
         });
 
         display_settings = {
             "landmark": {
                 "label": "Center Landmark",
-                "default": true
+                "default": true,
+                "type": ""
             },
             "timed_circle": {
                 "label": "Timed Circle",
-                "default": false
+                "default": false,
+                "type": ""
             },
         }
         for (setting_name in display_settings) {
             display_settings[setting_name]["value"] = display_settings[setting_name]["default"]
         }
 
 
 
         const carpetSize = [constants["carpet_length"], constants["carpet_width"]]
         intervalId = NaN
+        let fps_limit = 30
         let selectedObjet = "ball"
         let tick = 0
         let T0 = Date.now()
 
         if (isView) {
             setTimeout(runView, 1000)
             runView()
```

### Comparing `robot-soccer-kit-2.0.6/rsk/static/js/video.js` & `robot-soccer-kit-2.1.0/rsk/static/js/video.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/markers/blue1.svg` & `robot-soccer-kit-2.1.0/rsk/static/markers/blue1.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/markers/blue2.svg` & `robot-soccer-kit-2.1.0/rsk/static/markers/blue2.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/markers/green1.svg` & `robot-soccer-kit-2.1.0/rsk/static/markers/green1.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/markers/green2.svg` & `robot-soccer-kit-2.1.0/rsk/static/markers/green2.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/referee_event_team.html` & `robot-soccer-kit-2.1.0/rsk/static/referee_event_team.html`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/robot.html` & `robot-soccer-kit-2.1.0/rsk/static/robot.html`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/static/team.html` & `robot-soccer-kit-2.1.0/rsk/static/team.html`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/tasks.py` & `robot-soccer-kit-2.1.0/rsk/tasks.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/utils.py` & `robot-soccer-kit-2.1.0/rsk/utils.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/rsk/video.py` & `robot-soccer-kit-2.1.0/rsk/video.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.6/setup.py` & `robot-soccer-kit-2.1.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         for filename in filenames:
             if '__pycache__' not in path:
                 paths.append(os.path.join('..', path, filename))
     return paths
 
 setuptools.setup(
     name="robot-soccer-kit",
-    version="2.0.6",
+    version="2.1.0",
     author="Rhoban team",
     author_email="team@rhoban.com",
     description="Robot Soccer Kit",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rhoban/robot-soccer-kit/",
     packages=setuptools.find_packages(),
```

